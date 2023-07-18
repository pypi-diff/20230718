# Comparing `tmp/talkytimes_package-0.3.4.tar.gz` & `tmp/talkytimes_package-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytimes_package-0.3.4.tar", last modified: Mon Jul 17 14:22:00 2023, max compression
+gzip compressed data, was "talkytimes_package-0.3.5.tar", last modified: Tue Jul 18 01:15:01 2023, max compression
```

## Comparing `talkytimes_package-0.3.4.tar` & `talkytimes_package-0.3.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 14:22:00.212663 talkytimes_package-0.3.4/
--rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.3.4/LICENSE
--rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-17 14:22:00.212663 talkytimes_package-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.3.4/README.md
--rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.3.4/pyproject.toml
--rw-rw-rw-   0        0        0      121 2023-07-17 14:22:00.213664 talkytimes_package-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 14:22:00.154663 talkytimes_package-0.3.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-17 14:22:00.178662 talkytimes_package-0.3.4/src/dynamodb/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.3.4/src/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.3.4/src/dynamodb/base.py
--rw-rw-rw-   0        0        0     2684 2023-07-17 14:21:25.000000 talkytimes_package-0.3.4/src/dynamodb/dynamodb.py
-drwxrwxrwx   0        0        0        0 2023-07-17 14:22:00.193663 talkytimes_package-0.3.4/src/talkytimes/
--rw-rw-rw-   0        0        0       49 2023-07-17 14:21:58.000000 talkytimes_package-0.3.4/src/talkytimes/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.3.4/src/talkytimes/base.py
--rw-rw-rw-   0        0        0     3960 2023-07-16 08:50:22.000000 talkytimes_package-0.3.4/src/talkytimes/talkytimes.py
-drwxrwxrwx   0        0        0        0 2023-07-17 14:22:00.211662 talkytimes_package-0.3.4/src/talkytimes_package.egg-info/
--rw-rw-rw-   0        0        0      265 2023-07-17 14:22:00.000000 talkytimes_package-0.3.4/src/talkytimes_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-07-17 14:22:00.000000 talkytimes_package-0.3.4/src/talkytimes_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 14:22:00.000000 talkytimes_package-0.3.4/src/talkytimes_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-17 14:22:00.000000 talkytimes_package-0.3.4/src/talkytimes_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-17 14:22:00.000000 talkytimes_package-0.3.4/src/talkytimes_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 01:15:01.207677 talkytimes_package-0.3.5/
+-rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-18 01:15:01.207677 talkytimes_package-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.3.5/README.md
+-rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0      121 2023-07-18 01:15:01.212676 talkytimes_package-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 01:15:01.184673 talkytimes_package-0.3.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 01:15:01.190673 talkytimes_package-0.3.5/src/dynamodb/
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.3.5/src/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.3.5/src/dynamodb/base.py
+-rw-rw-rw-   0        0        0     2040 2023-07-18 01:13:02.000000 talkytimes_package-0.3.5/src/dynamodb/dynamodb.py
+drwxrwxrwx   0        0        0        0 2023-07-18 01:15:01.193674 talkytimes_package-0.3.5/src/talkytimes/
+-rw-rw-rw-   0        0        0       49 2023-07-18 01:12:48.000000 talkytimes_package-0.3.5/src/talkytimes/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.3.5/src/talkytimes/base.py
+-rw-rw-rw-   0        0        0     4004 2023-07-18 01:11:05.000000 talkytimes_package-0.3.5/src/talkytimes/talkytimes.py
+drwxrwxrwx   0        0        0        0 2023-07-18 01:15:01.206676 talkytimes_package-0.3.5/src/talkytimes_package.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-07-18 01:15:01.000000 talkytimes_package-0.3.5/src/talkytimes_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-07-18 01:15:01.000000 talkytimes_package-0.3.5/src/talkytimes_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 01:15:01.000000 talkytimes_package-0.3.5/src/talkytimes_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-18 01:15:01.000000 talkytimes_package-0.3.5/src/talkytimes_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-18 01:15:01.000000 talkytimes_package-0.3.5/src/talkytimes_package.egg-info/top_level.txt
```

### Comparing `talkytimes_package-0.3.4/LICENSE` & `talkytimes_package-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.3.4/src/dynamodb/dynamodb.py` & `talkytimes_package-0.3.5/src/dynamodb/dynamodb.py`

 * *Files 19% similar despite different names*

```diff
@@ -39,62 +39,39 @@
         )
         self.put_item(data=data)
 
     def update_user(
         self,
         *,
         external_id: str,
+        user_info: str,
         status: str,
         messages: Optional[str] = "0",
         emails: Optional[str] = "0"
     ) -> None:
-        user_info = json.dumps(
+        new_user_info = json.dumps(
             dict(
                 status=status,
                 messages=messages,
                 emails=emails
             )
         )
         self.table.update_item(
             ExpressionAttributeNames={
                 '#UI': 'user_info',
             },
             ExpressionAttributeValues={
                 ':user_info': {
-                    'S': user_info,
+                    'S': new_user_info,
                 },
             },
             Key={
                 'external_id': {
                     'S': external_id,
                 },
                 "user_info": {
-                    'S': json.dumps(dict(status="True", messages="0", emails="0"))
+                    'S': user_info
                 }
             },
             ReturnValues='UPDATED_NEW',
             UpdateExpression='SET #UI = :user_info',
         )
-
-    def create_or_update(
-        self,
-        *,
-        external_id: str,
-        status: str,
-        messages: Optional[str] = "0",
-        emails: Optional[str] = "0"
-    ):
-        user = self.get_user(external_id=external_id)
-        if user:
-            self.update_user(
-                external_id=external_id,
-                status=status,
-                messages=messages,
-                emails=emails
-            )
-        else:
-            self.create_user(
-                external_id=external_id,
-                status=status,
-                messages=messages,
-                emails=emails
-            )
```

### Comparing `talkytimes_package-0.3.4/src/talkytimes/base.py` & `talkytimes_package-0.3.5/src/talkytimes/base.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.3.4/src/talkytimes/talkytimes.py` & `talkytimes_package-0.3.5/src/talkytimes/talkytimes.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                     user_url = _user.find_element(by=By.TAG_NAME, value="a").get_attribute("href")
                     user_id = user_url.split("/")[-1]
                     status = _user.find_element(
                         by=By.CSS_SELECTOR,
                         value=".person-card__name svg"
                     ).value_of_css_property("fill")
                     status = True if status.__contains__("65") else False
-                    self.db.create_or_update(external_id=user_id, status=str(status))
+                    self.db.create_user(external_id=user_id, status=str(status))
                     count -= 1
                 time.sleep(2)
                 self.driver.find_element(by=By.XPATH, value=next_button).click()
                 element_button = self.driver.find_element(by=By.CLASS_NAME, value='next')
             except Exception as e:
                 print("Error get users page", page_count, e)
                 break
@@ -77,11 +77,12 @@
                         mails = user_pop_array[3]
                 else:
                     if not user_pop_array[3] == "no":
                         messages = user_pop_array[3]
                     mails = user_pop_array[0]
             self.db.update_user(
                 external_id=external_id,
+                user_info=user.get("user_info"),
                 status=status,
                 messages=messages,
                 emails=mails
             )
```

