# Comparing `tmp/clife_svc-1.14.tar.gz` & `tmp/clife_svc-1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\clife_svc-1.14.tar", last modified: Wed Jun 14 01:54:50 2023, max compression
+gzip compressed data, was "clife_svc-1.15.tar", last modified: Tue Jul 18 07:06:46 2023, max compression
```

## Comparing `clife_svc-1.14.tar` & `clife_svc-1.15.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 01:54:50.000000 clife_svc-1.14/
-drwxrwxrwx   0        0        0        0 2023-06-14 01:54:50.000000 clife_svc-1.14/clife_svc/
--rw-rw-rw-   0        0        0    11780 2023-06-13 07:15:59.000000 clife_svc-1.14/clife_svc/application.py
-drwxrwxrwx   0        0        0        0 2023-06-14 01:54:50.000000 clife_svc-1.14/clife_svc/config/
--rw-rw-rw-   0        0        0     2078 2023-01-13 06:38:28.000000 clife_svc-1.14/clife_svc/config/configmap.py
--rw-rw-rw-   0        0        0     5582 2023-04-27 09:54:37.000000 clife_svc-1.14/clife_svc/config/disconf.py
--rw-rw-rw-   0        0        0        0 2023-01-13 06:18:27.000000 clife_svc-1.14/clife_svc/config/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 01:54:50.000000 clife_svc-1.14/clife_svc/errors/
--rw-rw-rw-   0        0        0     3589 2022-09-01 09:09:26.000000 clife_svc-1.14/clife_svc/errors/error_code.py
--rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.14/clife_svc/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 01:54:50.000000 clife_svc-1.14/clife_svc/libs/
--rw-rw-rw-   0        0        0      284 2021-12-23 09:51:21.000000 clife_svc-1.14/clife_svc/libs/context.py
--rw-rw-rw-   0        0        0    14499 2023-06-13 07:17:16.000000 clife_svc-1.14/clife_svc/libs/http_request.py
--rw-rw-rw-   0        0        0     2649 2023-05-15 11:06:18.000000 clife_svc-1.14/clife_svc/libs/log.py
--rw-rw-rw-   0        0        0     3510 2023-06-13 07:17:16.000000 clife_svc-1.14/clife_svc/libs/mq_handler.py
--rw-rw-rw-   0        0        0     1282 2023-01-13 07:00:07.000000 clife_svc-1.14/clife_svc/libs/utils.py
--rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.14/clife_svc/libs/__init__.py
--rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.14/clife_svc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 01:54:50.000000 clife_svc-1.14/clife_svc.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-14 01:54:50.000000 clife_svc-1.14/clife_svc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      420 2023-06-14 01:54:50.000000 clife_svc-1.14/clife_svc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      141 2023-06-14 01:54:50.000000 clife_svc-1.14/clife_svc.egg-info/requires.txt
--rw-rw-rw-   0        0        0      535 2023-06-14 01:54:50.000000 clife_svc-1.14/clife_svc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2023-06-14 01:54:50.000000 clife_svc-1.14/clife_svc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      420 2023-06-14 01:54:50.000000 clife_svc-1.14/PKG-INFO
--rw-rw-rw-   0        0        0       12 2021-12-20 11:08:06.000000 clife_svc-1.14/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 01:54:50.000000 clife_svc-1.14/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-06-14 01:54:48.000000 clife_svc-1.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:06:46.443737 clife_svc-1.15/
+-rw-rw-rw-   0        0        0      437 2023-07-18 07:06:46.442739 clife_svc-1.15/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2021-12-20 11:08:06.000000 clife_svc-1.15/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 07:06:46.168467 clife_svc-1.15/clife_svc/
+-rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.15/clife_svc/__init__.py
+-rw-rw-rw-   0        0        0    11768 2023-07-18 07:06:22.000000 clife_svc-1.15/clife_svc/application.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:06:46.241275 clife_svc-1.15/clife_svc/config/
+-rw-rw-rw-   0        0        0        0 2023-01-13 06:18:27.000000 clife_svc-1.15/clife_svc/config/__init__.py
+-rw-rw-rw-   0        0        0     2078 2023-01-13 06:38:28.000000 clife_svc-1.15/clife_svc/config/configmap.py
+-rw-rw-rw-   0        0        0     5582 2023-04-27 09:54:37.000000 clife_svc-1.15/clife_svc/config/disconf.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:06:46.281168 clife_svc-1.15/clife_svc/errors/
+-rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.15/clife_svc/errors/__init__.py
+-rw-rw-rw-   0        0        0     3589 2022-09-01 09:09:26.000000 clife_svc-1.15/clife_svc/errors/error_code.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:06:46.439747 clife_svc-1.15/clife_svc/libs/
+-rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc-1.15/clife_svc/libs/__init__.py
+-rw-rw-rw-   0        0        0      284 2021-12-23 09:51:21.000000 clife_svc-1.15/clife_svc/libs/context.py
+-rw-rw-rw-   0        0        0    14499 2023-06-13 07:17:16.000000 clife_svc-1.15/clife_svc/libs/http_request.py
+-rw-rw-rw-   0        0        0     2649 2023-05-15 11:06:18.000000 clife_svc-1.15/clife_svc/libs/log.py
+-rw-rw-rw-   0        0        0     3510 2023-06-13 07:17:16.000000 clife_svc-1.15/clife_svc/libs/mq_handler.py
+-rw-rw-rw-   0        0        0     1282 2023-01-13 07:00:07.000000 clife_svc-1.15/clife_svc/libs/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:06:46.182431 clife_svc-1.15/clife_svc.egg-info/
+-rw-rw-rw-   0        0        0      437 2023-07-18 07:06:45.000000 clife_svc-1.15/clife_svc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2023-07-18 07:06:45.000000 clife_svc-1.15/clife_svc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 07:06:45.000000 clife_svc-1.15/clife_svc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2023-07-18 07:06:45.000000 clife_svc-1.15/clife_svc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-18 07:06:45.000000 clife_svc-1.15/clife_svc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 07:06:46.443737 clife_svc-1.15/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-07-18 07:06:22.000000 clife_svc-1.15/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `clife_svc-1.14/clife_svc/application.py` & `clife_svc-1.15/clife_svc/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,16 @@
             response: Response = await original_route_handler(request)
             duration = time.time() - before
             if request.scope['path'] == '/time':
                 tlogger.info('Request Cost: {}s'.format(round(duration, 2)))
                 tlogger.info('Response Content: {}'.format(response.body.decode('utf-8')))
             else:
                 klogger.info('Request Cost: {}s'.format(round(duration, 2)))
-                klogger.info('Response Content: {}'.format(response.body.decode('utf-8')))
+                if hasattr(response, 'body'):
+                    klogger.info('Response Content: {}'.format(response.body.decode('utf-8')))
             return response
         return custom_route_handler
 
 
 class App(object):
     """
     http接口服务上下文对象，单实例对象
@@ -68,15 +69,15 @@
         """
         if not cls._instance:
             with cls._instance_lock:
                 if not cls._instance:
                     cls._instance = super().__new__(cls)
         return cls._instance
 
-    def __init__(self, app_name: str, log_root_path: str = '/www/logs', conf: Union[str, list] = None, log_level: str = 'DEBUG'):
+    def __init__(self, app_name: str, log_root_path: str = '/www/logs', conf: Union[str, list] = '', log_level: str = 'DEBUG'):
         """
         构造函数
         :param app_name 项目名称
         :param log_root_path 项目输出的日志根路径，推荐使用/www/logs，便于线上统一采集日志
         :param conf: 配置文件名称列表，提供字符串列表或逗号分隔字符串
         :param log_level: 日志收集器级别，从低到高依次为 TRACE|DEBUG|INFO|SUCCESS|WARNING|ERROR|CRITICAL
         """
@@ -85,47 +86,47 @@
 
         if not re.match(r'^([a-zA-Z0-9]+-?[a-zA-Z0-9]+)+$', app_name):
             raise Exception('app_name can only be letters, numbers, or strike-through!')
 
         self.app_name = app_name
         init_log(os.path.join(log_root_path, app_name), log_level=log_level)
 
-        self.__disconf_item = Disconf('clife-ai', '0.0.1-SNAPSHOT', conf).get_disconf()
+        self.__disconf = Disconf('clife-ai', '0.0.1-SNAPSHOT', conf).get_disconf()
         self.__configmap = ConfigMap()
 
-        self.__ClientRequest = ClientRequest(self)
-        self.__MQHandler = MQHandler(app=self)
+        self.__client = ClientRequest(self)
+        self.__mq_handler = MQHandler(self)
 
         self.__fast_api = FastAPI(title='ai-service', default_response_class=ORJSONResponse)
         self.__ai_router = APIRouter(route_class=AiServiceRoute)
 
     def init_api(self) -> FastAPI:
         """
         在App中初始化服务接口
         :return: FastAPI，作为服务器运行入口对象
         """
         self.__init_middlewares()
         self.__fast_api.add_exception_handler(ApiException, api_exception_handler)
         self.__fast_api.add_exception_handler(Exception, app_exception)
         self.__ai_router.add_api_route('/time', endpoint=index, methods=['GET'], name='time')
         self.__fast_api.include_router(self.__ai_router)
-        self.__MQHandler.start_consumer()
+        self.__mq_handler.start_consumer()
         return self.__fast_api
 
     def __init_middlewares(self):
         self.__fast_api.add_middleware(CORSMiddleware,
                                        allow_credentials=True,
                                        allow_origins=["*"],
                                        allow_methods=["*"],
                                        allow_headers=["*"], )
         self.__fast_api.add_middleware(Interceptor)
 
     def get_conf(self, key: str, default: str = '') -> str:
-        if key in self.__disconf_item:
-            return self.__disconf_item.get(key)
+        if key in self.__disconf:
+            return self.__disconf.get(key)
         item = self.__configmap.get(key)
         if item:
             return item
         item = utils.get_env(key)
         if item:
             return item
         return default
@@ -146,15 +147,15 @@
 
     def get_all_conf(self) -> dict:
         """
         获取所有配置数据
         :return:
         """
         all_config = {}
-        all_config.update(self.__disconf_item)
+        all_config.update(self.__disconf)
         all_config.update(self.__configmap.get_all())
         return all_config
 
     def add_api(self, path: str, endpoint: Callable[..., Any], methods: Optional[Union[Set[str], List[str]]] = None):
         """
         增加服务接口，此函数需要在init_api前调用
         :param path:接口访问路径
@@ -165,15 +166,15 @@
         self.__ai_router.add_api_route(path, endpoint, methods=methods)
 
     def add_subscribe(self, call_back, topic=None):
         """
         :param call_back:回调函数
         :param topic:订阅主题
         """
-        self.__MQHandler.add_subscribe(call_back, topic)
+        self.__mq_handler.add_subscribe(call_back, topic)
 
     async def download_file(self, file_url, retry=2, timeout=None):
         """
         下载文件
         :param timeout:
         :param file_url:文件地址
         :param retry:失败重试次数，默认为2次，建议不大于3次
@@ -185,54 +186,54 @@
         cos_cli = self.__ClientRequest.create_txy_client()
         buckets_list = cos_cli.list_buckets()
         for bucket in buckets_list['Buckets']['Bucket']:
             print(bucket)
             acl = cos_cli.get_bucket_acl(bucket['Name'])
             print(acl)
         '''
-        return await self.__ClientRequest.download_file(file_url, retry, timeout)
+        return await self.__client.download_file(file_url, retry, timeout)
 
     async def upload_file(self, file_path: str, retry=2) -> str:
         """
         :param file_path:本地文件路径
         :param retry:失败重试次数，默认为2次，建议不大于3次
         :return: 文件url
         """
-        return await self.__ClientRequest.upload_file(self.app_name, file_path, retry)
+        return await self.__client.upload_file(self.app_name, file_path, retry)
 
     async def upload_file_from_buffer(self, file_extension: str, body, retry=2) -> str:
         """
         :param file_extension: 文件扩展名，如.txt|.png
         :param body: 文件流,必须实现了read方法
         :param retry: 失败重试次数,默认为2次，建议不大于3次
         :return: 文件url
         """
-        return await self.__ClientRequest.upload_file_from_buffer(self.app_name, file_extension, body, retry)
+        return await self.__client.upload_file_from_buffer(self.app_name, file_extension, body, retry)
 
     async def send_mq_msg(self, body, topic=None, keys=None, tags=None):
         """
         :param body: rocketMQ消息内容
         :param topic: rocketMQ消息主题，非必传，未配置默认主题时必传
         :param keys: rocketMQ消息唯一标识，非必传
         :param tags: rocketMQ消息标签，非必传
         """
-        self.__MQHandler.send_sync(body, topic, keys, tags)
+        self.__mq_handler.send_sync(body, topic, keys, tags)
 
     async def call_back(self, url: str, body: dict, retry=2, timeout=None):
         """
         推理结果回调
         :param url:回调地址
         :param body:回调内容，字典中必须包含‘uuid’的key，且value符合UUID规则
         :param retry:失败重试次数，默认为2次，建议不大于3次
         :param timeout: 回调超时时间（秒），默认为配置文件ai-commons.properties中http.timeout，目前为15秒
         :return:回调请求响应体
         """
         if not re.match(r'[0-9a-f]{8}(-[0-9a-f]{4}){3}-[0-9a-f]{12}', body.get('uuid', '')):
             raise Exception('The request body of call back must contain the correct UUID.')
-        return await self.__ClientRequest.call_back(url, body, retry, timeout)
+        return await self.__client.call_back(url, body, retry, timeout)
 
 
 class Interceptor(BaseHTTPMiddleware):
     """
     拦截所有请求
     """
 
@@ -248,15 +249,15 @@
         else:
             klogger.info('Request URL: {} {}'.format(request.method, request.url))
             response = await call_next(request)
             klogger.info('Response HTTP Status Code: {}'.format(response.status_code))
         return response
 
 
-async def index(q: Optional[str] = None):
+def index(q: Optional[str] = None):
     """k8s 探针 http监控服务请求地址"""
     result = {'code': 0,
               'msg': 'success',
               'data': {'time': time.strftime('%Y-%m-%d-%H-%M', time.localtime())}}
     if q:
         result['data'].update({'q': q})
     return result
```

### Comparing `clife_svc-1.14/clife_svc/config/configmap.py` & `clife_svc-1.15/clife_svc/config/configmap.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.14/clife_svc/config/disconf.py` & `clife_svc-1.15/clife_svc/config/disconf.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.14/clife_svc/errors/error_code.py` & `clife_svc-1.15/clife_svc/errors/error_code.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.14/clife_svc/libs/http_request.py` & `clife_svc-1.15/clife_svc/libs/http_request.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.14/clife_svc/libs/log.py` & `clife_svc-1.15/clife_svc/libs/log.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.14/clife_svc/libs/mq_handler.py` & `clife_svc-1.15/clife_svc/libs/mq_handler.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.14/clife_svc/libs/utils.py` & `clife_svc-1.15/clife_svc/libs/utils.py`

 * *Files identical despite different names*

### Comparing `clife_svc-1.14/clife_svc.egg-info/SOURCES.txt` & `clife_svc-1.15/clife_svc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clife_svc-1.14/setup.py` & `clife_svc-1.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         if line.startswith('-e git+'):
             dependency_links.append(line.replace('-e ', ''))
         else:
             requirements.append(line)
 
 setuptools.setup(
     name='clife_svc',   # 需要打包的名字,即本模块要发布的名字
-    version='1.14',     # 版本
+    version='1.15',     # 版本
     author='andy.hu',  # 作者名
     author_email='hlp0@163.com',  # 作者邮件
     description='A module for service',   # 简要描述
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',       # 项目地址,一般是代码托管的网站
     packages=setuptools.find_packages(),
```

