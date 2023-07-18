# Comparing `tmp/openedx-filters-1.3.0.tar.gz` & `tmp/openedx-filters-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-filters-1.3.0.tar", last modified: Thu May 25 17:56:40 2023, max compression
+gzip compressed data, was "openedx-filters-1.4.0.tar", last modified: Tue Jul 18 15:46:02 2023, max compression
```

## Comparing `openedx-filters-1.3.0.tar` & `openedx-filters-1.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:56:40.085341 openedx-filters-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9745 2023-05-25 17:56:40.085341 openedx-filters-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5391 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:56:40.085341 openedx-filters-1.3.0/openedx_filters/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:56:40.085341 openedx-filters-1.3.0/openedx_filters/learning/
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20822 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/learning/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:56:40.085341 openedx-filters-1.3.0/openedx_filters/learning/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/learning/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18503 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/learning/tests/test_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:56:40.085341 openedx-filters-1.3.0/openedx_filters/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      942 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)    17309 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/tests/test_tooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     8532 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/tooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:56:40.085341 openedx-filters-1.3.0/openedx_filters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9745 2023-05-25 17:56:40.000000 openedx-filters-1.3.0/openedx_filters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-05-25 17:56:40.000000 openedx-filters-1.3.0/openedx_filters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 17:56:40.000000 openedx-filters-1.3.0/openedx_filters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 17:56:40.000000 openedx-filters-1.3.0/openedx_filters.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-25 17:56:40.000000 openedx-filters-1.3.0/openedx_filters.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-25 17:56:40.000000 openedx-filters-1.3.0/openedx_filters.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:56:40.085341 openedx-filters-1.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-25 17:56:40.085341 openedx-filters-1.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     2867 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:56:40.085341 openedx-filters-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/tests/test_openedx_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 15:46:02.010656 openedx-filters-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     3848 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9986 2023-07-18 15:46:02.010656 openedx-filters-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5453 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 15:46:02.006656 openedx-filters-1.4.0/openedx_filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 15:46:02.006656 openedx-filters-1.4.0/openedx_filters/learning/
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23553 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/learning/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 15:46:02.006656 openedx-filters-1.4.0/openedx_filters/learning/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/learning/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19937 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/learning/tests/test_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 15:46:02.010656 openedx-filters-1.4.0/openedx_filters/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      942 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17309 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/tests/test_tooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8532 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/tooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/openedx_filters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 15:46:02.006656 openedx-filters-1.4.0/openedx_filters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9986 2023-07-18 15:46:01.000000 openedx-filters-1.4.0/openedx_filters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-18 15:46:02.000000 openedx-filters-1.4.0/openedx_filters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 15:46:01.000000 openedx-filters-1.4.0/openedx_filters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 15:46:01.000000 openedx-filters-1.4.0/openedx_filters.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-18 15:46:01.000000 openedx-filters-1.4.0/openedx_filters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-18 15:46:01.000000 openedx-filters-1.4.0/openedx_filters.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 15:46:02.010656 openedx-filters-1.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-07-18 15:46:02.010656 openedx-filters-1.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2867 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 15:46:02.010656 openedx-filters-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-07-18 15:45:57.000000 openedx-filters-1.4.0/tests/test_openedx_filters.py
```

### Comparing `openedx-filters-1.3.0/CHANGELOG.rst` & `openedx-filters-1.4.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,24 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+
+[1.4.0] - 2023-07-18
+--------------------
+
+Added
+~~~~~
+
+* InstructorDashboardRenderStarted filter added which can be used to modify the instructor dashboard rendering process.
+
+
 [1.3.0] - 2023-05-25
 --------------------
 
 Added
 ~~~~~
 
 * CourseHomeUrlCreationStarted filter added which can be used to modify the course_home_url for externally hosted courses.
```

### Comparing `openedx-filters-1.3.0/LICENSE.txt` & `openedx-filters-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.3.0/PKG-INFO` & `openedx-filters-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-filters
-Version: 1.3.0
+Version: 1.4.0
 Summary: Open edX Filters from Hooks Extensions Framework (OEP-50).
 Home-page: https://github.com/openedx/openedx-filters
 Author: eduNEXT
 Author-email: technical@edunext.co
 License: AGPL 3.0
 Keywords: Python openedx
 Classifier: Development Status :: 3 - Alpha
@@ -101,15 +101,15 @@
 
 Getting Help
 ************
 
 Documentation
 =============
 
-See `documentation on Read the Docs <https://openedx-filters.readthedocs.io/en/latest/>`_.
+See the `Open edX Hooks Extension Framework guide <https://github.com/openedx/edx-platform/blob/master/docs/guides/hooks/index.rst>`_ in edx-platform.
 
 More Help
 =========
 
 If you're having trouble, we have discussion forums at
 https://discuss.openedx.org where you can connect with others in the
 community.
@@ -165,15 +165,15 @@
 file in this repo.
 
 .. _Backstage: https://backstage.openedx.org/catalog/default/component/openedx-filters
 
 Reporting Security Issues
 *************************
 
-Please do not report security issues in public. Please email security@tcril.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/openedx-filters.svg
     :target: https://pypi.python.org/pypi/openedx-filters/
     :alt: PyPI
 
 .. |ci-badge| image:: https://github.com/openedx/openedx-filters/workflows/Python%20CI/badge.svg?branch=main
     :target: https://github.com/openedx/openedx-filters/actions
@@ -209,14 +209,24 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+
+[1.4.0] - 2023-07-18
+--------------------
+
+Added
+~~~~~
+
+* InstructorDashboardRenderStarted filter added which can be used to modify the instructor dashboard rendering process.
+
+
 [1.3.0] - 2023-05-25
 --------------------
 
 Added
 ~~~~~
 
 * CourseHomeUrlCreationStarted filter added which can be used to modify the course_home_url for externally hosted courses.
```

### Comparing `openedx-filters-1.3.0/README.rst` & `openedx-filters-1.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 Getting Help
 ************
 
 Documentation
 =============
 
-See `documentation on Read the Docs <https://openedx-filters.readthedocs.io/en/latest/>`_.
+See the `Open edX Hooks Extension Framework guide <https://github.com/openedx/edx-platform/blob/master/docs/guides/hooks/index.rst>`_ in edx-platform.
 
 More Help
 =========
 
 If you're having trouble, we have discussion forums at
 https://discuss.openedx.org where you can connect with others in the
 community.
@@ -146,15 +146,15 @@
 file in this repo.
 
 .. _Backstage: https://backstage.openedx.org/catalog/default/component/openedx-filters
 
 Reporting Security Issues
 *************************
 
-Please do not report security issues in public. Please email security@tcril.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/openedx-filters.svg
     :target: https://pypi.python.org/pypi/openedx-filters/
     :alt: PyPI
 
 .. |ci-badge| image:: https://github.com/openedx/openedx-filters/workflows/Python%20CI/badge.svg?branch=main
     :target: https://github.com/openedx/openedx-filters/actions
```

### Comparing `openedx-filters-1.3.0/openedx_filters/exceptions.py` & `openedx-filters-1.4.0/openedx_filters/exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.3.0/openedx_filters/filters.py` & `openedx-filters-1.4.0/openedx_filters/filters.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.3.0/openedx_filters/learning/filters.py` & `openedx-filters-1.4.0/openedx_filters/learning/filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -585,7 +585,80 @@
 
         Arguments:
             course_key (CourseKey): The course key for which the home url is being requested.
             course_home_url (String): The url string for the course home
         """
         data = super().run_pipeline(course_key=course_key, course_home_url=course_home_url)
         return data.get("course_key"), data.get("course_home_url")
+
+
+class InstructorDashboardRenderStarted(OpenEdxPublicFilter):
+    """
+    Custom class used to create instructor dashboard filters and its custom methods.
+    """
+
+    filter_type = "org.openedx.learning.instructor.dashboard.render.started.v1"
+
+    class RedirectToPage(OpenEdxFilterException):
+        """
+        Custom class used to stop the instructor dashboard render by redirecting to a new page.
+        """
+
+        def __init__(self, message, redirect_to=""):
+            """
+            Override init that defines specific arguments used in the instructor dashboard render process.
+
+            Arguments:
+                message: error message for the exception.
+                redirect_to: URL to redirect to.
+            """
+            super().__init__(message, redirect_to=redirect_to)
+
+    class RenderInvalidDashboard(OpenEdxFilterException):
+        """
+        Custom class used to render a custom template instead of the instructor dashboard.
+        """
+
+        def __init__(self, message, instructor_template="", template_context=None):
+            """
+            Override init that defines specific arguments used in the instructor dashboard render process.
+
+            Arguments:
+                message: error message for the exception.
+                instructor_template: template path rendered instead.
+                template_context: context used to the new instructor_template.
+            """
+            super().__init__(
+                message,
+                instructor_template=instructor_template,
+                template_context=template_context,
+            )
+
+    class RenderCustomResponse(OpenEdxFilterException):
+        """
+        Custom class used to stop the instructor dashboard rendering by returning a custom response.
+        """
+
+        def __init__(self, message, response=None):
+            """
+            Override init that defines specific arguments used in the instructor dashboard render process.
+
+            Arguments:
+                message: error message for the exception.
+                response: custom response which will be returned by the dashboard view.
+            """
+            super().__init__(
+                message,
+                response=response,
+            )
+
+    @classmethod
+    def run_filter(cls, context, template_name):
+        """
+        Execute a filter with the signature specified.
+
+        Arguments:
+            context (dict): context dictionary for instructor's tab template.
+            template_name (str): template name to be rendered by the instructor's tab.
+        """
+        data = super().run_pipeline(context=context, template_name=template_name)
+        return data.get("context"), data.get("template_name")
```

### Comparing `openedx-filters-1.3.0/openedx_filters/learning/tests/test_filters.py` & `openedx-filters-1.4.0/openedx_filters/learning/tests/test_filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     CohortChangeRequested,
     CourseAboutRenderStarted,
     CourseEnrollmentQuerysetRequested,
     CourseEnrollmentStarted,
     CourseHomeUrlCreationStarted,
     CourseUnenrollmentStarted,
     DashboardRenderStarted,
+    InstructorDashboardRenderStarted,
     StudentLoginRequested,
     StudentRegistrationRequested,
     VerticalBlockChildRenderStarted,
     VerticalBlockRenderCompleted,
 )
 
 
@@ -504,14 +505,49 @@
         Expected behavior:
             - The exception must have the attributes specified.
         """
         exception = AccountSettingsException(message="You can't access this page", **attributes)
 
         self.assertDictContainsSubset(attributes, exception.__dict__)
 
+    def test_instructor_dashboard_render_started(self):
+        """
+        Test InstructorDashboardRenderStarted filter behavior under normal conditions.
+
+        Expected behavior:
+            - The filter must have the signature specified.
+            - The filter should return context and template_name in that order.
+        """
+        result = InstructorDashboardRenderStarted.run_filter(self.context, self.template_name)
+
+        self.assertTupleEqual((self.context, self.template_name,), result)
+
+    @data(
+        (InstructorDashboardRenderStarted.RedirectToPage, {"redirect_to": "custom-dashboard.html"}),
+        (
+            InstructorDashboardRenderStarted.RenderInvalidDashboard,
+            {
+                "instructor_template": "custom-dasboard.html",
+                "template_context": {"course": Mock()},
+            }
+        ),
+        (InstructorDashboardRenderStarted.RenderCustomResponse, {"response": Mock()}),
+    )
+    @unpack
+    def test_halt_instructor_dashboard_render(self, dashboard_exception, attributes):
+        """
+        Test for the instructor dashboard exceptions attributes.
+
+        Expected behavior:
+            - The exception must have the attributes specified.
+        """
+        exception = dashboard_exception(message="You can't access the dashboard", **attributes)
+
+        self.assertDictContainsSubset(attributes, exception.__dict__)
+
 
 class TestCohortFilters(TestCase):
     """
     Test class to verify standard behavior of the cohort membership filters.
     You'll find test suites for:
 
     - CohortChangeRequested
```

### Comparing `openedx-filters-1.3.0/openedx_filters/tests/test_exceptions.py` & `openedx-filters-1.4.0/openedx_filters/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.3.0/openedx_filters/tests/test_filters.py` & `openedx-filters-1.4.0/openedx_filters/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.3.0/openedx_filters/tests/test_tooling.py` & `openedx-filters-1.4.0/openedx_filters/tests/test_tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.3.0/openedx_filters/tooling.py` & `openedx-filters-1.4.0/openedx_filters/tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.3.0/openedx_filters/utils.py` & `openedx-filters-1.4.0/openedx_filters/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.3.0/openedx_filters.egg-info/PKG-INFO` & `openedx-filters-1.4.0/openedx_filters.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-filters
-Version: 1.3.0
+Version: 1.4.0
 Summary: Open edX Filters from Hooks Extensions Framework (OEP-50).
 Home-page: https://github.com/openedx/openedx-filters
 Author: eduNEXT
 Author-email: technical@edunext.co
 License: AGPL 3.0
 Keywords: Python openedx
 Classifier: Development Status :: 3 - Alpha
@@ -101,15 +101,15 @@
 
 Getting Help
 ************
 
 Documentation
 =============
 
-See `documentation on Read the Docs <https://openedx-filters.readthedocs.io/en/latest/>`_.
+See the `Open edX Hooks Extension Framework guide <https://github.com/openedx/edx-platform/blob/master/docs/guides/hooks/index.rst>`_ in edx-platform.
 
 More Help
 =========
 
 If you're having trouble, we have discussion forums at
 https://discuss.openedx.org where you can connect with others in the
 community.
@@ -165,15 +165,15 @@
 file in this repo.
 
 .. _Backstage: https://backstage.openedx.org/catalog/default/component/openedx-filters
 
 Reporting Security Issues
 *************************
 
-Please do not report security issues in public. Please email security@tcril.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/openedx-filters.svg
     :target: https://pypi.python.org/pypi/openedx-filters/
     :alt: PyPI
 
 .. |ci-badge| image:: https://github.com/openedx/openedx-filters/workflows/Python%20CI/badge.svg?branch=main
     :target: https://github.com/openedx/openedx-filters/actions
@@ -209,14 +209,24 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+
+[1.4.0] - 2023-07-18
+--------------------
+
+Added
+~~~~~
+
+* InstructorDashboardRenderStarted filter added which can be used to modify the instructor dashboard rendering process.
+
+
 [1.3.0] - 2023-05-25
 --------------------
 
 Added
 ~~~~~
 
 * CourseHomeUrlCreationStarted filter added which can be used to modify the course_home_url for externally hosted courses.
```

### Comparing `openedx-filters-1.3.0/openedx_filters.egg-info/SOURCES.txt` & `openedx-filters-1.4.0/openedx_filters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.3.0/setup.py` & `openedx-filters-1.4.0/setup.py`

 * *Files identical despite different names*

