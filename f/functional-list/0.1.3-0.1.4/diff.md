# Comparing `tmp/functional_list-0.1.3-py3-none-any.whl.zip` & `tmp/functional_list-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5385 bytes, number of entries: 8
--rw-r--r--  2.0 unx       62 b- defN 23-Mar-16 18:39 functional_list/__init__.py
--rw-r--r--  2.0 unx     8866 b- defN 23-Mar-16 18:39 functional_list/list_functional_mapper.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-16 18:39 functional_list/utils/__init__.py
--rw-r--r--  2.0 unx      553 b- defN 23-Mar-16 18:39 functional_list/utils/tools_for_main_class.py
--rw-r--r--  2.0 unx     2902 b- defN 23-Mar-16 18:40 functional_list-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-16 18:40 functional_list-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Mar-16 18:40 functional_list-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      698 b- defN 23-Mar-16 18:40 functional_list-0.1.3.dist-info/RECORD
-8 files, 13189 bytes uncompressed, 4143 bytes compressed:  68.6%
+Zip file size: 5485 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       62 b- defN 23-Jul-18 16:01 functional_list/__init__.py
+-rw-r--r--  2.0 unx     9344 b- defN 23-Jul-18 16:01 functional_list/list_functional_mapper.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-18 16:01 functional_list/utils/__init__.py
+-rw-r--r--  2.0 unx      557 b- defN 23-Jul-18 16:01 functional_list/utils/tools_for_main_class.py
+-rw-r--r--  2.0 unx     2912 b- defN 23-Jul-18 16:01 functional_list-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-18 16:01 functional_list-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-18 16:01 functional_list-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      698 b- defN 23-Jul-18 16:01 functional_list-0.1.4.dist-info/RECORD
+8 files, 13681 bytes uncompressed, 4243 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: functional_list/utils/__init__.py
 Comment: 
 
 Filename: functional_list/utils/tools_for_main_class.py
 Comment: 
 
-Filename: functional_list-0.1.3.dist-info/METADATA
+Filename: functional_list-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: functional_list-0.1.3.dist-info/WHEEL
+Filename: functional_list-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: functional_list-0.1.3.dist-info/top_level.txt
+Filename: functional_list-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: functional_list-0.1.3.dist-info/RECORD
+Filename: functional_list-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## functional_list/list_functional_mapper.py

```diff
@@ -4,33 +4,37 @@
 a functional programming behavior.
 
 The main class is the ListMapper
 that contains a lot of method
 """
 
 import sys
-from typing import Any, List
+from typing import Any, List, Callable, TypeVar, Generic, Optional
 
 from functional_list.utils.tools_for_main_class import ListMapperIterator
 
 sys.setrecursionlimit(150000)
 
+T = TypeVar("T")
 
-class ListMapper:
+
+class ListMapper(Generic[T]):
     """
     This class object aim to emulate the same behavior of a list object
-    but the difference is that we will use it to make a functionnal
+    but the difference is that we will use it to make a functional
     programming.
     """
 
-    def __init__(self, *args):
+    ma_list: List[T]
+
+    def __init__(self, *args: T):
         self.ma_list = list(args)
 
     def __str__(self):
-        return 'List' + str(self.ma_list)
+        return "List" + str(self.ma_list)
 
     def __repr__(self):
         return self.__str__()
 
     def __iter__(self):
         return ListMapperIterator(self)
 
@@ -44,31 +48,38 @@
         """
         Copy a ListMapper
         :return: an object of ListMapper type
         """
         temp = self.ma_list[:]
         return ListMapper(*temp)
 
-    def to_list(self) -> List[Any]:
+    def to_list(self) -> Optional[List[T]]:
         """
         :return a list
         Example:
         >> ListMapper(1,2).tolist()
         >> [1,2]
         """
         return self.ma_list
 
-    def map(self, function) -> "ListMapper":
+    @property
+    def length(self) -> int:
+        """
+        return length of ListMapper object.
+        """
+        return len(self.ma_list)
+
+    def map(self, function: Callable) -> "ListMapper":
         """
-          :function a function as params
-          :return ListMapper
-          Example:
-          >> test=ListMapper(2,3,4)
-          >> test.map(lambda x:x*x)
-          >> List[4, 9, 16]
+        :function a function as params
+        :return ListMapper
+        Example:
+        >> test=ListMapper(2,3,4)
+        >> test.map(lambda x:x*x)
+        >> List[4, 9, 16]
         """
         res: ListMapper = self.copy()
         res.ma_list = list(map(function, self.ma_list))
         return res
 
     @property
     def flatten(self) -> "ListMapper":
@@ -76,72 +87,81 @@
         :return ListMapper
         Example:
         >> test = ListMapper([1,2,4], ListMapper(3,5,6))
         >> test.flatten()
         >> List[1, 2, 4, 3, 5, 6]
         """
         res = self.copy()
-        args = [list(val) if isinstance(val, ListMapper) else val for val in self.ma_list]
-        res.ma_list = sum(args, [])
+        init_list: List[T] = []
+        res.foreach(
+            lambda data: init_list.extend(data.ma_list)
+            if isinstance(data, ListMapper)
+            else init_list.extend(data)
+        )
+        init_list.sort()
+        res.ma_list = init_list
         return res
 
-    def flat_map(self, function) -> "ListMapper":
+    def flat_map(self, function: Callable) -> "ListMapper":
         """
         :param function: function
         :return: ListMapper
         Example:
         >> test = ListMapper("where are you?","I am here")
         >> test.flat_map(lambda x: x.split(" ")
         >> List["where","are","you","I","am","here"]
         """
         temp = self.map(function).ma_list[:]
         res = self.copy()
         res.ma_list = temp
         return res.flatten
 
-    def reduce(self, function) -> Any:
+    def reduce(self, function: Callable) -> Any:
         """
         :param function:
         :return: Any
         Example:
         >> test=ListMapper(1,2,3,4)
         >> test.reduce(lambda x,y:x+y)
         >> 10
         """
         result = self.ma_list[0]
         for k in range(1, len(self.ma_list)):
             result = function(self.ma_list[k], result)
         return result
 
-    def order_by_key(self):
+    def order_by_key(self) -> "ListMapper":
         """
         :return: ListMapper
         Example:
         >> test = ListMapper(("I", 1), ("a", 6), ("am", 5), ("here", 4))
         >> test.reduce_by_key()
         >> List[('I', 1), ('a', 6), ('am', 5), ('here', 4)]
         """
-        temp = sorted(self.ma_list)
         res = self.copy()
-        res.ma_list = temp
+        res.ma_list.sort()
         return res
 
     def group_by_key(self):
         """
         :return: ListMapper
         Example:
         >> test= ListMapper(("I",2),("am",1),("here",1),("here",4),("am",1),("I",1))
         >> test.group_by_key()
         >> List[("I",List[2,1]),("am",List[1, 1]),("here",List[4,1]))
         """
         to_map_list = self.map(lambda x: x)
         res = to_map_list.map(lambda x: x[0]).unique
         res = res.map(
-            lambda x: (x, to_map_list.map(lambda y: y[1] if x == y[0] else None)
-                       .filter(lambda x: x is not None))
+            lambda x: (
+                x,
+                to_map_list.map(lambda y: y[1] if x == y[0] else None).filter(
+                    lambda x: x is not None
+                ),
+            )
         )
 
         return res
 
     def reduce_by_key(self, function) -> "ListMapper":
         """
         :param function:
@@ -149,30 +169,30 @@
         Example:
         >> test= ListMapper(("I",2),("am",1),("here",1),("here",4),("am",1),("I",1))
         >> test.reduce_by_key(lambda x,y:x+y)
         >> List[("I",3),("am",2),("here",5)]
         """
         return self.group_by_key().map(lambda x: (x[0], x[1].reduce(function)))
 
-    def foreach(self, function):
+    def foreach(self, function) -> None:
         """
         :param function:
         :return:
         Example:
         >> test=ListMapper(1,2,3)
         >> test.foreach(lambda x: print("the value equals={}".format(x)))
         >> "the value equals=1"
         >> "the value equals=2"
         >>  "the value equals=3"
         """
         for k in self:
             function(k)
 
     @property
-    def unique(self):
+    def unique(self) -> "ListMapper":
         """
         :return: ListMapper
         Example:
         >> test = ListMapper(1,2,3,3,2,1)
         >> test.unique
         >> List[1, 2, 3]
         """
@@ -189,88 +209,88 @@
         >> test.filter(lambda x: x%2==0)
         >> List[2, 4, 6]
         """
         res = self.copy()
         res.ma_list = list(filter(function, self.ma_list))
         return res
 
-    def append(self, value):
+    def append(self, value: T) -> "ListMapper":
         """
         :param value: Element to append
         :return: ListMapper
         example:
         >> test = ListMapper(1,2,3)
         >> test.append(4)
         >> List[1, 2, 3, 4]
         """
         self.ma_list.append(value)
         return self
 
-    def extend(self, *list_value) -> "ListMapper":
+    def extend(self, *list_value: T) -> "ListMapper":
         """
         :param list_value: list python of element
         :return: ListMapper
         example:
         >> test1 = ListMapper(1,2,3)
         >> test2 = [4,5,6]
         >> test1.append(*test2)
         >> List[1, 2, 3, 4, 5, 6]
         """
         self.ma_list.extend(list_value)
         return self
 
-    def insert(self, index: int, value: Any) -> "ListMapper":
+    def insert(self, index: int, value: T) -> "ListMapper":
         """
         :param index: index to insert
         :param value: the new value
         :return: ListMapper
         example:
         >> test = ListMapper(1,2,3)
         >> test.insert(1,4)
         >> List[1, 4, 2, 3, 4]
         """
         self.ma_list.insert(index, value)
         return self
 
     @property
-    def head(self) -> Any:
+    def head(self) -> T:
         """
         :return Any
         Example:
         >> test=ListMapper(10,30,42,89)
         >> test.head
         >> 10
         """
         return self.ma_list[0]
 
     @property
-    def tail(self):
+    def tail(self) -> T:
         """
         :return Any
         Example:
         >> test=ListMapper(10,30,42,89)
         >> test.head
         >> 89
         """
         return self.ma_list[-1]
 
-    def remove(self, elem: Any) -> None:
+    def remove(self, elem: T) -> None:
         """
 
         :param elem:
         :return:
         Example:
         >> test = ListMapper(2,8,1,8)
         >> test.remove(8)
         >> print(test)
         >> List[2, 8, 1]
         """
         self.ma_list.remove(elem)
 
-    def remove_all(self, value: Any) -> "ListMapper":
+    def remove_all(self, value: T) -> "ListMapper":
         """
         This method remove all value equals to value in
         the ListMapper
         :param value: ListMapper(Any)
         :return:
         Example:
         >> test1 = ListMapper(2, 8, 1, 2)
@@ -287,15 +307,15 @@
         :return: ListMapper
         Example:
         >> test = ListMapper(3,4,8,5)
         >> test.remove_index(3)
         >> List[3, 4, 5]
         """
         if len(self.ma_list) <= index:
-            raise IndexError('list index out of range')
+            raise IndexError("list index out of range")
         self.ma_list = [k for i, k in enumerate(self.ma_list) if i != index]
         return self
 
     def remove_list_index(self, list_index: List[int]) -> "ListMapper":
         """
         :param list_index:
         :return: ListMapper
@@ -304,19 +324,19 @@
         >> list_to_remove = [0, 3, 5]
         >> test.remove_list_index(list_to_remove)
         >> List[4, 3, 7, 8, 2]
         """
         nb_element = len(self.ma_list)
         sum_elem = sum(k >= nb_element for k in list_index)
         if sum_elem > 0:
-            raise IndexError('list index out of range')
+            raise IndexError("list index out of range")
         self.ma_list = [k for i, k in enumerate(self.ma_list) if i not in list_index]
         return self
 
-    def remove_list_value(self, list_value: List[Any]) -> "ListMapper":
+    def remove_list_value(self, list_value: List[T]) -> "ListMapper":
         """
         :param list_value:
         :return: ListMapper
         Example:
         >> test = ListMapper(1,2,3,4,5)
         >> list_element_to_remove=[1, 3, 5]
         >> test.remove_list_value(list_element_to_remove)
```

## functional_list/utils/tools_for_main_class.py

```diff
@@ -2,15 +2,15 @@
 We will put all utils tools for the main class
 into this module.
 """
 
 
 class ListMapperIterator:
     """
-    This class is use to able the ListMapper class to be iterable.
+    This class is used to be able the ListMapper class to be iterable.
     """
 
     def __init__(self, list_mapper):
         self.current = 0
         self.max = len(list_mapper.ma_list)
         self.list = list_mapper.ma_list
```

## Comparing `functional_list-0.1.3.dist-info/METADATA` & `functional_list-0.1.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functional-list
-Version: 0.1.3
+Version: 0.1.4
 Summary: package for map a list
 Home-page: https://gitlab.com/Tantelitiana22/list-function-python-project
 Author: Andrianarivo Tantelitiana RAKOTOARIJAONA
 Author-email: tantelitiana22@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -50,30 +50,30 @@
 document =[
             "python is good",
             "python is better than x",
             "python is the best",
             ]
 
 ## Now, let tranform the list to a list mapper 
-document = ListMapper(*document)
+document = ListMapper[str](*document)
 
 res = document.flat_map(lambda x:x.split())\
               .map(lambda x:(x,1))\
               .reduce_by_key(lambda x,y:x+y)
 
 ## result will be:
 #List[('than', 1), ('the', 1), ('best', 1),
 #        ('better', 1), ('good', 1), ('is', 3), 
 #        ('python', 3), ('x', 1)]
 # And you have your word count :)
 ```
 The ListMapper object has also the same behavior as a standard
 python list.
 ```
-my_list = ListMapper(2, 4, 9, 13, 15, 20)
+my_list = ListMapper[int](2, 4, 9, 13, 15, 20)
 ## Append element 
 my_list.append(55)
 ## will give List[2, 4, 9, 13, 15, 20, 55]
 ## Let make some ordianry transformation
 my_list.map(lambda x: x*x)\
        .filter(lambda x:x%2==0)\
        .reduce(lambda x,y:x+y)
```

## Comparing `functional_list-0.1.3.dist-info/RECORD` & `functional_list-0.1.4.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 functional_list/__init__.py,sha256=YkgLdlKRVV5Gn_q8ofGm4m9l-krTsc64RF1fKPeS0_A,62
-functional_list/list_functional_mapper.py,sha256=IZ8slXgl-lauYHKOIAzzKK8DaKnAjn1NU7jENSgod4w,8866
+functional_list/list_functional_mapper.py,sha256=P2psx2fzLcM1nHQu4yqiaJEL9Ds4GSkK6-rAnTzPD0s,9344
 functional_list/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-functional_list/utils/tools_for_main_class.py,sha256=ad3zssZ7Xs6JTsfVNeoheTka2sa6GNs36d0yltBRLS4,553
-functional_list-0.1.3.dist-info/METADATA,sha256=Mf7qh3AdexZyYRvbdrEw3UeKZpC6h4J2Qr7r_416BQ4,2902
-functional_list-0.1.3.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-functional_list-0.1.3.dist-info/top_level.txt,sha256=KYRKk8gV7a6xkJkwL65MOKXBfhVm5dsdCVn5dAoTUgQ,16
-functional_list-0.1.3.dist-info/RECORD,,
+functional_list/utils/tools_for_main_class.py,sha256=xoc8ppbQLgoHy66ua2TiZyfMfFxyx5tAweB6IkYLtto,557
+functional_list-0.1.4.dist-info/METADATA,sha256=m6pC9b0U3TfiuB0Y8vZ_tcF3VLARgIfDsIWWE3GtbWo,2912
+functional_list-0.1.4.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+functional_list-0.1.4.dist-info/top_level.txt,sha256=KYRKk8gV7a6xkJkwL65MOKXBfhVm5dsdCVn5dAoTUgQ,16
+functional_list-0.1.4.dist-info/RECORD,,
```

