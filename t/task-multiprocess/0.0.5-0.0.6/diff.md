# Comparing `tmp/task_multiprocess-0.0.5.tar.gz` & `tmp/task_multiprocess-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task_multiprocess-0.0.5.tar", last modified: Mon Jul 10 14:24:52 2023, max compression
+gzip compressed data, was "task_multiprocess-0.0.6.tar", last modified: Tue Jul 18 07:49:35 2023, max compression
```

## Comparing `task_multiprocess-0.0.5.tar` & `task_multiprocess-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:24:52.548000 task_multiprocess-0.0.5/
--rw-r--r--   0 root         (0) root         (0)     1088 2023-07-07 07:05:10.000000 task_multiprocess-0.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1247 2023-07-10 14:24:52.548000 task_multiprocess-0.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      896 2023-07-10 07:37:23.000000 task_multiprocess-0.0.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 14:24:52.548000 task_multiprocess-0.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      589 2023-07-10 14:24:44.000000 task_multiprocess-0.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:24:52.548000 task_multiprocess-0.0.5/task_multiprocess/
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-07 15:18:02.000000 task_multiprocess-0.0.5/task_multiprocess/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2241 2023-07-10 14:23:36.000000 task_multiprocess-0.0.5/task_multiprocess/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:24:52.548000 task_multiprocess-0.0.5/task_multiprocess.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1247 2023-07-10 14:24:52.000000 task_multiprocess-0.0.5/task_multiprocess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      246 2023-07-10 14:24:52.000000 task_multiprocess-0.0.5/task_multiprocess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 14:24:52.000000 task_multiprocess-0.0.5/task_multiprocess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-10 14:24:52.000000 task_multiprocess-0.0.5/task_multiprocess.egg-info/top_level.txt
+drwxr-xr-x   0 raymo1    (1013) raymo1    (1014)        0 2023-07-18 07:49:35.220000 task_multiprocess-0.0.6/
+-rw-r--r--   0 raymo1    (1013) raymo1    (1014)     1088 2023-07-07 07:05:10.000000 task_multiprocess-0.0.6/LICENSE
+-rw-r--r--   0 raymo1    (1013) raymo1    (1014)     1895 2023-07-18 07:49:35.220000 task_multiprocess-0.0.6/PKG-INFO
+-rw-r--r--   0 raymo1    (1013) raymo1    (1014)     1566 2023-07-18 07:47:13.000000 task_multiprocess-0.0.6/README.md
+-rw-r--r--   0 raymo1    (1013) raymo1    (1014)       38 2023-07-18 07:49:35.220000 task_multiprocess-0.0.6/setup.cfg
+-rw-r--r--   0 raymo1    (1013) raymo1    (1014)      589 2023-07-18 07:49:06.000000 task_multiprocess-0.0.6/setup.py
+drwxr-xr-x   0 raymo1    (1013) raymo1    (1014)        0 2023-07-18 07:49:35.220000 task_multiprocess-0.0.6/task_multiprocess/
+-rw-r--r--   0 raymo1    (1013) raymo1    (1014)       20 2023-07-07 15:18:02.000000 task_multiprocess-0.0.6/task_multiprocess/__init__.py
+-rw-r--r--   0 raymo1    (1013) raymo1    (1014)     2077 2023-07-18 07:47:13.000000 task_multiprocess-0.0.6/task_multiprocess/main.py
+drwxr-xr-x   0 raymo1    (1013) raymo1    (1014)        0 2023-07-18 07:49:35.220000 task_multiprocess-0.0.6/task_multiprocess.egg-info/
+-rw-r--r--   0 raymo1    (1013) raymo1    (1014)     1895 2023-07-18 07:49:35.000000 task_multiprocess-0.0.6/task_multiprocess.egg-info/PKG-INFO
+-rw-r--r--   0 raymo1    (1013) raymo1    (1014)      246 2023-07-18 07:49:35.000000 task_multiprocess-0.0.6/task_multiprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 raymo1    (1013) raymo1    (1014)        1 2023-07-18 07:49:35.000000 task_multiprocess-0.0.6/task_multiprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 raymo1    (1013) raymo1    (1014)       18 2023-07-18 07:49:35.000000 task_multiprocess-0.0.6/task_multiprocess.egg-info/top_level.txt
```

### Comparing `task_multiprocess-0.0.5/LICENSE` & `task_multiprocess-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `task_multiprocess-0.0.5/PKG-INFO` & `task_multiprocess-0.0.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task_multiprocess
-Version: 0.0.5
+Version: 0.0.6
 Summary: run tasks in parallel
 Home-page: 
 Author: raymond
 Author-email: lei20190123@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,10 +20,30 @@
 q, q_size, lock, public_list = generate_queue(sample_list,num=2) # num means how many public_list do you want,you can use index to use them like public_list[0] or others
  
 def add(ids):
     index = ids[0]  
     index = int(index)
     fun(index) # fun is an function defined by yourself
     
-common_multiprocess(add,1,cpu_num=cpu_num,q=q, q_size=q_size, lock=lock) # add is a function defined by yourself \
-params 1 means how many variable do you want to get each time \
+common_multiprocess(add,1,cpu_num=cpu_num,q=q, q_size=q_size, lock=lock) 
+
+
+
+-----------------------------------------------------------------------------
+new version
+
+from task_multiprocess.main import TaskMultiprocess
+TaskMultiprocess.cpu_num = 2
+tm = TaskMultiprocess()
+sample_list = list(range(1000))[:] # [int,int,...] or [str,str,...] or ...
+q, q_size, lock, public_list = tm.generate_queue(sample_list,num=2) # num means how many public_list do you want,you can use index to use them like public_list[0] or others
+
+def add(ids):
+    index = ids[0]  
+    index = int(index)
+    fun(index) # fun is an function defined by yourself
+
+tm.common_multiprocess(add,q_num=1,q=q, cpu_num=tm.cpu_num,q_size=q_size, lock=lock) 
+
+# add is a function defined by yourself \
+q_num means how many variable do you want to get each time \
 in this example only use index 0 to get one variable -> (index = ids[0]), you can also get 2,3 or more (a, b = ids[0],ids[1]), remember to replace 1 to the number you want
```

### Comparing `task_multiprocess-0.0.5/setup.py` & `task_multiprocess-0.0.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="task_multiprocess",
-    version="0.0.5",
+    version="0.0.6",
     author="raymond",
     author_email="lei20190123@gmail.com",
     description="run tasks in parallel",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=['task_multiprocess'],
```

### Comparing `task_multiprocess-0.0.5/task_multiprocess/main.py` & `task_multiprocess-0.0.6/task_multiprocess/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,53 @@
 import os
 
 
 class TaskMultiprocess:
-    cpu_num = os.cpu_count()
+    cpu_num = os.cpu_count() // 2
 
     # 配合多进程使用的队列
     def generate_queue(self, queue_list, num=2, desc='generate_queue'):
         # queue_list 将列表形式的数据存放在队列中，返回队列,队列的大小,进程共享的list
         from multiprocessing import Manager
         from tqdm import tqdm
         lock = Manager().Lock()
         q = Manager().Queue()
         for i in tqdm(queue_list, position=0, desc=desc):
             q.put(str(i))
         q_size = q.qsize()
         return q, q_size, lock, [Manager().list() for i in range(num)]
 
     # 多进程装饰器
-    def multiprocess_decorator(self,cpu_num=os.cpu_count()):
-        def wrapper(func):
-            from multiprocessing import Process
-            def main(*args, **kwargs):
-                process_list = []
-                for _ in range(cpu_num):  # 开启多个子进程执行func函数
-                    p = Process(target=func, args=(*args,), kwargs=kwargs)  # 实例化进程对象
-                    p.start()
-                    process_list.append(p)
-                for p in process_list:
-                    p.join()
-
-            #         return  # 不需要子进程函数执行结果
-            return main
+    def multiprocess_decorator(func):
+        from multiprocessing import Process
+        def wrapper(*args, **kwargs):
+            process_list = []
+            for _ in range(TaskMultiprocess.cpu_num):  # 开启多个子进程执行func函数
+                p = Process(target=func, args=(*args,), kwargs=kwargs)  # 实例化进程对象
+                p.start()
+                process_list.append(p)
+            for p in process_list:
+                p.join()
 
+        #         return  # 不需要子进程函数执行结果
         return wrapper
 
-    @multiprocess_decorator(cpu_num)
-    def common_multiprocess(self, fun, q_num, cpu_num=os.cpu_count(), q=None, q_size=0,
+    @multiprocess_decorator
+    def common_multiprocess(self, fun, q_num, cpu_num=cpu_num, q=None, q_size=0,
                             lock=None, block=True, timeout=2):
         from tqdm import tqdm
         pbar = tqdm(total=q_size, position=0, desc='')
         try:
             while q.qsize():
                 lock.acquire()
                 # q_element_list = [q.get(block=block, timeout=timeout) for i in range(q_num)]
                 q_element_list = [q.get_nowait() for i in range(q_num)]
                 lock.release()
                 # print(q_element_list)
                 fun(q_element_list)
-                # process_id_list.append(os.getpid())
                 pbar.update(q_num * cpu_num)
         except Exception as e:
             print(e)
             pass
 
 
 """
```

### Comparing `task_multiprocess-0.0.5/task_multiprocess.egg-info/PKG-INFO` & `task_multiprocess-0.0.6/task_multiprocess.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task-multiprocess
-Version: 0.0.5
+Version: 0.0.6
 Summary: run tasks in parallel
 Home-page: 
 Author: raymond
 Author-email: lei20190123@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,10 +20,30 @@
 q, q_size, lock, public_list = generate_queue(sample_list,num=2) # num means how many public_list do you want,you can use index to use them like public_list[0] or others
  
 def add(ids):
     index = ids[0]  
     index = int(index)
     fun(index) # fun is an function defined by yourself
     
-common_multiprocess(add,1,cpu_num=cpu_num,q=q, q_size=q_size, lock=lock) # add is a function defined by yourself \
-params 1 means how many variable do you want to get each time \
+common_multiprocess(add,1,cpu_num=cpu_num,q=q, q_size=q_size, lock=lock) 
+
+
+
+-----------------------------------------------------------------------------
+new version
+
+from task_multiprocess.main import TaskMultiprocess
+TaskMultiprocess.cpu_num = 2
+tm = TaskMultiprocess()
+sample_list = list(range(1000))[:] # [int,int,...] or [str,str,...] or ...
+q, q_size, lock, public_list = tm.generate_queue(sample_list,num=2) # num means how many public_list do you want,you can use index to use them like public_list[0] or others
+
+def add(ids):
+    index = ids[0]  
+    index = int(index)
+    fun(index) # fun is an function defined by yourself
+
+tm.common_multiprocess(add,q_num=1,q=q, cpu_num=tm.cpu_num,q_size=q_size, lock=lock) 
+
+# add is a function defined by yourself \
+q_num means how many variable do you want to get each time \
 in this example only use index 0 to get one variable -> (index = ids[0]), you can also get 2,3 or more (a, b = ids[0],ids[1]), remember to replace 1 to the number you want
```

