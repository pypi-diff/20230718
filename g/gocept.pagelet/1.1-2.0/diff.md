# Comparing `tmp/gocept.pagelet-1.1.tar.gz` & `tmp/gocept.pagelet-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gocept.pagelet-1.1.tar", last modified: Mon Jun 10 05:18:17 2019, max compression
+gzip compressed data, was "gocept.pagelet-2.0.tar", last modified: Tue Jul 18 05:39:25 2023, max compression
```

## Comparing `gocept.pagelet-1.1.tar` & `gocept.pagelet-2.0.tar`

### file list

```diff
@@ -1,33 +1,30 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2019-06-10 05:18:17.000000 gocept.pagelet-1.1/
--rw-r--r--   0 mac        (501) staff       (20)     7953 2019-06-10 05:18:17.000000 gocept.pagelet-1.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      448 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/COPYRIGHT.txt
--rw-r--r--   0 mac        (501) staff       (20)       54 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/pytest.ini
--rw-r--r--   0 mac        (501) staff       (20)      241 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/buildout.cfg
--rw-r--r--   0 mac        (501) staff       (20)      199 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/.hgignore
--rw-r--r--   0 mac        (501) staff       (20)      270 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/.hgtags
--rw-r--r--   0 mac        (501) staff       (20)      254 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)       93 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/.coveragerc
--rw-r--r--   0 mac        (501) staff       (20)     2180 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/setup.py
--rw-r--r--   0 mac        (501) staff       (20)      615 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/tox.ini
--rw-r--r--   0 mac        (501) staff       (20)       38 2019-06-10 05:18:17.000000 gocept.pagelet-1.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)       94 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/README.rst
--rw-r--r--   0 mac        (501) staff       (20)     2071 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)     1118 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/CHANGES.rst
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2019-06-10 05:18:17.000000 gocept.pagelet-1.1/src/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2019-06-10 05:18:17.000000 gocept.pagelet-1.1/src/gocept/
--rw-r--r--   0 mac        (501) staff       (20)       76 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/src/gocept/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2019-06-10 05:18:17.000000 gocept.pagelet-1.1/src/gocept/pagelet/
--rw-r--r--   0 mac        (501) staff       (20)     6570 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/src/gocept/pagelet/zcml.py
--rw-r--r--   0 mac        (501) staff       (20)       72 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/src/gocept/pagelet/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)       30 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/src/gocept/pagelet/test-template.pt
--rw-r--r--   0 mac        (501) staff       (20)      724 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/src/gocept/pagelet/viewletpage.py
--rw-r--r--   0 mac        (501) staff       (20)      637 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/src/gocept/pagelet/meta.zcml
--rw-r--r--   0 mac        (501) staff       (20)     3281 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/src/gocept/pagelet/README.rst
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2019-06-10 05:18:17.000000 gocept.pagelet-1.1/src/gocept.pagelet.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     7953 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/src/gocept.pagelet.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)        1 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/src/gocept.pagelet.egg-info/not-zip-safe
--rw-r--r--   0 mac        (501) staff       (20)        7 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/src/gocept.pagelet.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (501) staff       (20)      642 2019-06-10 05:18:17.000000 gocept.pagelet-1.1/src/gocept.pagelet.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)      149 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/src/gocept.pagelet.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        7 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/src/gocept.pagelet.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2019-06-10 05:18:16.000000 gocept.pagelet-1.1/src/gocept.pagelet.egg-info/dependency_links.txt
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-18 05:39:25.379551 gocept.pagelet-2.0/
+-rw-r--r--   0 mac        (513) staff       (20)      145 2023-07-18 05:39:24.000000 gocept.pagelet-2.0/.coveragerc
+-rw-r--r--   0 mac        (513) staff       (20)     1239 2023-07-18 05:39:24.000000 gocept.pagelet-2.0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      448 2023-07-18 05:39:24.000000 gocept.pagelet-2.0/COPYRIGHT.txt
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-07-18 05:39:24.000000 gocept.pagelet-2.0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      189 2023-07-18 05:39:24.000000 gocept.pagelet-2.0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)     6331 2023-07-18 05:39:25.379671 gocept.pagelet-2.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)       94 2023-07-18 05:39:24.000000 gocept.pagelet-2.0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)       91 2023-07-18 05:39:24.000000 gocept.pagelet-2.0/pytest.ini
+-rw-r--r--   0 mac        (513) staff       (20)      213 2023-07-18 05:39:25.380360 gocept.pagelet-2.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     2185 2023-07-18 05:39:24.000000 gocept.pagelet-2.0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-18 05:39:25.369784 gocept.pagelet-2.0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-18 05:39:25.374627 gocept.pagelet-2.0/src/gocept/
+-rw-r--r--   0 mac        (513) staff       (20)       76 2023-07-18 05:39:24.000000 gocept.pagelet-2.0/src/gocept/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-18 05:39:25.379315 gocept.pagelet-2.0/src/gocept/pagelet/
+-rw-r--r--   0 mac        (513) staff       (20)     3281 2023-07-18 05:39:24.000000 gocept.pagelet-2.0/src/gocept/pagelet/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)       72 2023-07-18 05:39:24.000000 gocept.pagelet-2.0/src/gocept/pagelet/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)      636 2023-07-18 05:39:24.000000 gocept.pagelet-2.0/src/gocept/pagelet/meta.zcml
+-rw-r--r--   0 mac        (513) staff       (20)       30 2023-07-18 05:39:24.000000 gocept.pagelet-2.0/src/gocept/pagelet/test-template.pt
+-rw-r--r--   0 mac        (513) staff       (20)      707 2023-07-18 05:39:24.000000 gocept.pagelet-2.0/src/gocept/pagelet/viewletpage.py
+-rw-r--r--   0 mac        (513) staff       (20)     6552 2023-07-18 05:39:24.000000 gocept.pagelet-2.0/src/gocept/pagelet/zcml.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-18 05:39:25.377405 gocept.pagelet-2.0/src/gocept.pagelet.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)     6331 2023-07-18 05:39:25.000000 gocept.pagelet-2.0/src/gocept.pagelet.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      621 2023-07-18 05:39:25.000000 gocept.pagelet-2.0/src/gocept.pagelet.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-07-18 05:39:25.000000 gocept.pagelet-2.0/src/gocept.pagelet.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        7 2023-07-18 05:39:25.000000 gocept.pagelet-2.0/src/gocept.pagelet.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-07-18 05:39:25.000000 gocept.pagelet-2.0/src/gocept.pagelet.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)      149 2023-07-18 05:39:25.000000 gocept.pagelet-2.0/src/gocept.pagelet.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        7 2023-07-18 05:39:25.000000 gocept.pagelet-2.0/src/gocept.pagelet.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)      499 2023-07-18 05:39:24.000000 gocept.pagelet-2.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gocept.pagelet-1.1/setup.py` & `gocept.pagelet-2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,60 @@
+from setuptools import find_packages
+from setuptools import setup
 import os.path
-from setuptools import setup, find_packages
 
 
 def read(rel_path):
     rel_path = rel_path.split('/')
     base_path = os.path.dirname(__file__)
     path = (base_path,) + tuple(rel_path)
     with open(os.path.join(*path)) as f:
         return f.read()
 
+
 setup(
     name='gocept.pagelet',
-    version='1.1',
+    version='2.0',
     author="Christian Zagrodnick",
     author_email="mail@gocept.com",
     description="Easier z3c.pagelet handling",
     long_description='\n\n'.join([
         read('README.rst'),
         read('COPYRIGHT.txt'),
         read('CHANGES.rst'),
         read('src/gocept/pagelet/README.rst')]),
     license="ZPL 2.1",
-    url='https://bitbucket.org/gocept/gocept.pagelet',
+    url='https://github.com/gocept/gocept.pagelet',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Framework :: Zope3',
         'Intended Audience :: Developers',
         'License :: OSI Approved',
         'License :: OSI Approved :: Zope Public License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules'
+        'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     keywords='easy z3c.pagelet zope3 pagelet zope',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     include_package_data=True,
     zip_safe=False,
     namespace_packages=['gocept'],
+    python_requires='>=3.7',
     install_requires=[
         'setuptools',
         'zope.interface',
         'zope.component',
         'zope.publisher',
         'zope.viewlet',
         'z3c.template',
```

### Comparing `gocept.pagelet-1.1/LICENSE.txt` & `gocept.pagelet-2.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,8 +37,7 @@
 EVENT SHALL THE COPYRIGHT HOLDERS BE LIABLE FOR ANY DIRECT, INDIRECT,
 INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
 PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
```

### Comparing `gocept.pagelet-1.1/CHANGES.rst` & `gocept.pagelet-2.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =========
  Changes
 =========
 
+2.0 (2023-07-18)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.9, 3.10, 3.11.
+
+
 1.1 (2019-06-10)
 ================
 
 - Claim support of Python 3.5, 3.6, 3.7, 3.8, PyPy and PyPy3.
 
 - Use tox for testing.
```

### Comparing `gocept.pagelet-1.1/src/gocept/pagelet/zcml.py` & `gocept.pagelet-2.0/src/gocept/pagelet/zcml.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,47 +12,47 @@
 import zope.viewlet.metaconfigure
 
 
 class IPageletDirective(z3c.pagelet.zcml.IPageletDirective):
     """A directive to easily register a new pagelet with a layout template."""
 
     for_ = zope.configuration.fields.Tokens(
-        title=u"Specifications of the objects to be viewed",
-        description=u"""This should be a list of interfaces or classes""",
+        title="Specifications of the objects to be viewed",
+        description="""This should be a list of interfaces or classes""",
         required=True,
         value_type=zope.configuration.fields.GlobalObject(
               missing_value=object(),
         ),
     )
 
     class_ = zope.configuration.fields.GlobalObject(
-        title=u"Class",
-        description=u"A class that provides attributes used by the pagelet.",
+        title="Class",
+        description="A class that provides attributes used by the pagelet.",
         required=False,
     )
 
     template = zope.configuration.fields.Path(
-        title=u'Layout template.',
-        description=u"Refers to a file containing a page template (should "
+        title='Layout template.',
+        description="Refers to a file containing a page template (should "
         "end in extension ``.pt`` or ``.html``).",
         required=False,
     )
 
     title = zope.configuration.fields.MessageID(
-        title=u"The browser menu label for the page (view)",
-        description=u"""
+        title="The browser menu label for the page (view)",
+        description="""
           This attribute must be supplied if a menu attribute is
           supplied.
           """,
         required=False
     )
 
     menu = zope.browsermenu.field.MenuField(
-        title=u"The browser menu to include the page (view) in.",
-        description=u"""
+        title="The browser menu to include the page (view) in.",
+        description="""
           Many views are included in menus. It's convenient to name
           the menu in the page directive, rather than having to give a
           separate menuItem directive.  'zmi_views' is the menu most often
           used in the Zope management interface.
           </description>
           """,
         required=False
@@ -84,15 +84,15 @@
         z3c.template.zcml.templateDirective(
             _context, template, for_=new_class, layer=layer)
 
     zope.browserpage.metaconfigure._handle_menu(
         _context, menu, title, tuple(for_), name, permission, layer)
 
 
-class ViewletPageDirective(object):
+class ViewletPageDirective:
     """Directive to register a new pagelet with a layout template."""
 
     def __init__(self, _context, name, permission,
                  class_=gocept.pagelet.viewletpage.ViewletPage,
                  **kwargs):
         self._context = _context
         self.name = name
```

### Comparing `gocept.pagelet-1.1/src/gocept/pagelet/viewletpage.py` & `gocept.pagelet-2.0/src/gocept/pagelet/viewletpage.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) 2007 gocept gmbh & co. kg
 # See also LICENSE.txt
 # $Id$
 
+import z3c.pagelet.browser
 import zope.viewlet.interfaces
 import zope.viewlet.manager
-import z3c.pagelet.browser
 
 
 class IViewletPageManager(zope.viewlet.interfaces.IViewletManager):
     pass
 
 
 ViewletPageManager = zope.viewlet.manager.ViewletManager(
@@ -16,15 +16,15 @@
 
 
 class ViewletPage(z3c.pagelet.browser.BrowserPagelet):
 
     template = None
 
     def __init__(self, context, request):
-        super(ViewletPage, self).__init__(context, request)
+        super().__init__(context, request)
         self.vm = ViewletPageManager(context, request, self)
         self.vm.template = self.template
 
     def update(self):
         self.vm.update()
 
     def render(self):
```

### Comparing `gocept.pagelet-1.1/src/gocept/pagelet/meta.zcml` & `gocept.pagelet-2.0/src/gocept/pagelet/meta.zcml`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,7 @@
          />
 
     </meta:complexDirective>
 
   </meta:directives>
 
 </configure>
-
```

### Comparing `gocept.pagelet-1.1/src/gocept/pagelet/README.rst` & `gocept.pagelet-2.0/src/gocept/pagelet/README.rst`

 * *Files identical despite different names*

### Comparing `gocept.pagelet-1.1/src/gocept.pagelet.egg-info/SOURCES.txt` & `gocept.pagelet-2.0/src/gocept.pagelet.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 .coveragerc
-.hgignore
-.hgtags
 CHANGES.rst
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
-buildout.cfg
 pytest.ini
+setup.cfg
 setup.py
 tox.ini
 src/gocept/__init__.py
 src/gocept.pagelet.egg-info/PKG-INFO
 src/gocept.pagelet.egg-info/SOURCES.txt
 src/gocept.pagelet.egg-info/dependency_links.txt
 src/gocept.pagelet.egg-info/namespace_packages.txt
```

