# Comparing `tmp/visualtest_python-1.5.0-py3-none-any.whl.zip` & `tmp/visualtest_python-1.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 20477 bytes, number of entries: 11
--rw-r--r--  2.0 unx      121 b- defN 23-Jun-27 15:00 sbvt/__init__.py
--rw-r--r--  2.0 unx     6904 b- defN 23-Jun-27 14:39 sbvt/api.py
--rw-r--r--  2.0 unx    35671 b- defN 23-Jun-20 12:05 sbvt/browser.py
+Zip file size: 20781 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      121 b- defN 23-Jul-18 11:44 sbvt/__init__.py
+-rw-r--r--  2.0 unx     7694 b- defN 23-Jul-11 11:50 sbvt/api.py
+-rw-r--r--  2.0 unx    36548 b- defN 23-Jul-11 11:50 sbvt/browser.py
 -rw-r--r--  2.0 unx     6269 b- defN 23-Jun-09 14:01 sbvt/imagetools.py
 -rw-r--r--  2.0 unx      548 b- defN 23-May-11 09:06 sbvt/timer.py
--rw-r--r--  2.0 unx    15818 b- defN 23-Jun-27 14:39 sbvt/visualtest.py
--rw-r--r--  2.0 unx     1073 b- defN 23-Jun-27 15:01 visualtest_python-1.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3876 b- defN 23-Jun-27 15:01 visualtest_python-1.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 15:01 visualtest_python-1.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-27 15:01 visualtest_python-1.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      868 b- defN 23-Jun-27 15:01 visualtest_python-1.5.0.dist-info/RECORD
-11 files, 71245 bytes uncompressed, 19019 bytes compressed:  73.3%
+-rw-r--r--  2.0 unx    16070 b- defN 23-Jul-18 11:45 sbvt/visualtest.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jul-18 11:46 visualtest_python-1.5.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3876 b- defN 23-Jul-18 11:46 visualtest_python-1.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-18 11:46 visualtest_python-1.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-18 11:46 visualtest_python-1.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      868 b- defN 23-Jul-18 11:46 visualtest_python-1.5.1.dist-info/RECORD
+11 files, 73164 bytes uncompressed, 19323 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: sbvt/timer.py
 Comment: 
 
 Filename: sbvt/visualtest.py
 Comment: 
 
-Filename: visualtest_python-1.5.0.dist-info/LICENSE
+Filename: visualtest_python-1.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: visualtest_python-1.5.0.dist-info/METADATA
+Filename: visualtest_python-1.5.1.dist-info/METADATA
 Comment: 
 
-Filename: visualtest_python-1.5.0.dist-info/WHEEL
+Filename: visualtest_python-1.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: visualtest_python-1.5.0.dist-info/top_level.txt
+Filename: visualtest_python-1.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: visualtest_python-1.5.0.dist-info/RECORD
+Filename: visualtest_python-1.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbvt/__init__.py

```diff
@@ -1,4 +1,4 @@
 # this import statement is here for context.py in tests folder
 from .visualtest import VisualTest
 
-__version__ = '1.5.0'
+__version__ = '1.5.1'
```

## sbvt/api.py

```diff
@@ -141,22 +141,41 @@
             result = response.json()
         else:
             log.error(f'Failed to create image. HTTP Response: {response.json()}')
             raise Exception(f'Failed to create image. HTTP Response: {response.json()}')
 
         log.info(f'uploading image to: {result["uploadUrl"]}')
 
-        response = s3.put(result['uploadUrl'], data=imageBinary)
-        log.info(f'upload image response: {response}')
+        try:
+            response = s3.put(result['uploadUrl'], data=imageBinary)
+            log.info(f'upload image response: {response.status_code}')
 
-        if response.status_code in range(200, 300):
-            return result
-        else:
-            log.error(f'Failed to upload image. HTTP Response: {response.json()}')
-            raise Exception(f'Failed to upload image. HTTP Response: {response.json()}')
+            if response.status_code in range(200, 300):
+                return result
+            else:
+                log.error(f'Failed to upload image.')
+                raise Exception(f'{response.text}')
+
+        except Exception as e:
+            log.debug(f'error: {e.__str__()}')
+            errorMessage = {"errorMessage": e.__str__()}
+            url = f'{Api.baseUrl}/projects/{self.projectId}/testruns/{self.testRun["testRunId"]}/images/{result["imageId"]}'
+
+            response = api.patch(url, json=errorMessage)
+            log.info(f'calling API to add error: {url}')
+            log.debug(f'errorMessage: {errorMessage}')
+
+            if response.status_code in range(200, 300):
+                log.debug(f'errorResult: {response.json()}')
+                return result
+            else:
+                log.error(
+                    f'Failed to send error. HTTP Response: {response.text}')
+                raise Exception(
+                    f'Failed to send error. HTTP Response: {response.text}')
 
     @staticmethod
     def getToolkit(scriptName=None):
         if scriptName in ['user-agent','dom-capture','freeze-page','chrome-os-version','detect-chrome-headless']:
             url = f'{Api.cdnUrl}/{scriptName}.min.js'
             response = api.get(url)
             return response.text
```

## sbvt/browser.py

```diff
@@ -429,14 +429,16 @@
 
         # how many viewports fit into the fullpage 
         totalPages = self._getNumberOfPagesToScroll()
         log.info(f'Total pages to scroll: {totalPages}')
 
         reasonStopped = None
 
+        self.page_has_loaded()
+
         # handle single page as special case
         if totalPages == 1:
             # take the selenium screenshot as final fullpage
             log.info(f'Taking single screenshot for single page')
 
             pageStopWatch = StopWatch()
             pageStopWatch.start()
@@ -446,14 +448,21 @@
             freezePageResult = None
             if 'freezePage' in options:
                 if options['freezePage']:
                     freezePageResult = self._freezePage()
             else:
                 freezePageResult = self._freezePage()
 
+            # update the dimensions of the browser window and webpage
+            self._getPageDimensions()
+
+            # how many viewports fit into the fullpage
+            totalPages = self._getNumberOfPagesToScroll()
+            log.info(f'Total pages to scroll: {totalPages}')
+
             imageBinary = self._driver.get_screenshot_as_png()
 
             if self._debug:
                 debugImageName = '0.png'
                 debugImagePath = os.path.join(debugImageDir, debugImageName)
                 with open(debugImagePath, 'wb') as outfile:
                     outfile.write(imageBinary)
@@ -491,14 +500,21 @@
             freezePageResult = None
             if 'freezePage' in options:
                 if options['freezePage']:
                     freezePageResult = self._freezePage()
             else:
                 freezePageResult = self._freezePage()
 
+            # update the dimensions of the browser window and webpage
+            self._getPageDimensions()
+
+            # how many viewports fit into the fullpage
+            totalPages = self._getNumberOfPagesToScroll()
+            log.info(f'Total pages to scroll: {totalPages}')
+
             # to hide bottom fixed elements, this is a trick that works on most modern browsers
             log.info(f'PREP: Hiding bottom fixed elements: document.body.style.transform="translateY(0)"')
             self._driver.execute_script(f'document.body.style.transform="translateY(0)"')
             time.sleep(0.5) #some browsers need a little time to apply (Safari)
 
             done = False
             pageIndex = 0
@@ -799,8 +815,13 @@
         }
 
         log.info(f'Result: {result}')
         result['dom'] = self.dom #add dom after logging result
         result['imageBinary'] = imageBinary
         return result
 
-
+    def page_has_loaded(self):
+        page_state = self._driver.execute_script('return document.readyState;')
+        while page_state != 'complete':
+            time.sleep(1)
+            page_state = self._driver.execute_script(
+                'return document.readyState;')
```

## sbvt/visualtest.py

```diff
@@ -95,14 +95,20 @@
             self.saveTo = os.path.join(settings['saveTo'])
 
         if 'debug' in settings and type(settings['debug']) == bool:
             self.browser.debug = settings['debug']
 
         # setup api
         self._api = Api(self._settings['projectToken'])
+
+        if "testRunId" in settings:
+            if isinstance(settings['testRunId'], str):
+                self._api.testRun = {'testRunId': settings['testRunId']}
+            else:
+                raise Exception('"testRunId" should be a str type.')
         
         log.info(f'final instance settings: {self._settings}')
 
     @property
     def projectToken(self):
         """
         Get projectToken (str)
```

## Comparing `visualtest_python-1.5.0.dist-info/LICENSE` & `visualtest_python-1.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `visualtest_python-1.5.0.dist-info/METADATA` & `visualtest_python-1.5.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualtest-python
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python SDK for SmartBear VisualTest via Selenium WebDriver
 Home-page: https://github.com/SmartBear/visualtest-python
 Author: Luke Kende
 Author-email: luke.kende@smartbear.com
 Keywords: visual testing,UI testing,GUI testing,UX testing,screenshots,full page screenshots,image comparisons,regression testing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

