# Comparing `tmp/swiftly-windows-0.0.4.tar.gz` & `tmp/swiftly-windows-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-windows-0.0.4.tar", last modified: Sat Jul 15 12:11:28 2023, max compression
+gzip compressed data, was "swiftly-windows-0.0.5.tar", last modified: Tue Jul 18 20:19:31 2023, max compression
```

## Comparing `swiftly-windows-0.0.4.tar` & `swiftly-windows-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 12:11:28.162867 swiftly-windows-0.0.4/
--rw-rw-rw-   0        0        0     1528 2023-07-12 21:41:36.000000 swiftly-windows-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       85 2023-07-15 12:11:28.162867 swiftly-windows-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-15 12:11:28.149811 swiftly-windows-0.0.4/scripts/
--rwxrwxrwx   0        0        0     4477 2023-07-15 11:58:44.000000 swiftly-windows-0.0.4/scripts/swiftly.bat
--rw-rw-rw-   0        0        0       42 2023-07-15 12:11:28.162867 swiftly-windows-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      176 2023-07-15 12:11:22.000000 swiftly-windows-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 12:11:28.149811 swiftly-windows-0.0.4/swiftly_windows/
--rw-rw-rw-   0        0        0        0 2023-07-12 21:41:36.000000 swiftly-windows-0.0.4/swiftly_windows/__init__.py
--rw-rw-rw-   0        0        0       30 2023-07-12 21:41:36.000000 swiftly-windows-0.0.4/swiftly_windows/config.py
--rw-rw-rw-   0        0        0     3266 2023-07-12 21:41:36.000000 swiftly-windows-0.0.4/swiftly_windows/gitignore.py
--rw-rw-rw-   0        0        0     3407 2023-07-12 21:41:36.000000 swiftly-windows-0.0.4/swiftly_windows/init.py
--rw-rw-rw-   0        0        0     2218 2023-07-12 21:41:36.000000 swiftly-windows-0.0.4/swiftly_windows/makeapp.py
--rw-rw-rw-   0        0        0      186 2023-07-12 21:41:36.000000 swiftly-windows-0.0.4/swiftly_windows/runapp.py
-drwxrwxrwx   0        0        0        0 2023-07-15 12:11:28.162867 swiftly-windows-0.0.4/swiftly_windows.egg-info/
--rw-rw-rw-   0        0        0       85 2023-07-15 12:11:28.000000 swiftly-windows-0.0.4/swiftly_windows.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-07-15 12:11:28.000000 swiftly-windows-0.0.4/swiftly_windows.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 12:11:28.000000 swiftly-windows-0.0.4/swiftly_windows.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-15 12:11:28.000000 swiftly-windows-0.0.4/swiftly_windows.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-18 20:19:31.130481 swiftly-windows-0.0.5/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-18 20:18:06.000000 swiftly-windows-0.0.5/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       81 2023-07-18 20:19:31.130335 swiftly-windows-0.0.5/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-18 20:19:31.128465 swiftly-windows-0.0.5/scripts/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     6035 2023-07-18 20:18:06.000000 swiftly-windows-0.0.5/scripts/swiftly.bat
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-18 20:19:31.130523 swiftly-windows-0.0.5/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      169 2023-07-18 20:19:10.000000 swiftly-windows-0.0.5/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-18 20:19:31.129611 swiftly-windows-0.0.5/swiftly_windows/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-18 20:18:06.000000 swiftly-windows-0.0.5/swiftly_windows/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-18 20:18:06.000000 swiftly-windows-0.0.5/swiftly_windows/config.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-18 20:18:06.000000 swiftly-windows-0.0.5/swiftly_windows/gitignore.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3299 2023-07-18 20:18:06.000000 swiftly-windows-0.0.5/swiftly_windows/init.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2172 2023-07-18 20:18:06.000000 swiftly-windows-0.0.5/swiftly_windows/makeapp.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-18 20:18:06.000000 swiftly-windows-0.0.5/swiftly_windows/runapp.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-18 20:19:31.130149 swiftly-windows-0.0.5/swiftly_windows.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       81 2023-07-18 20:19:31.000000 swiftly-windows-0.0.5/swiftly_windows.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      352 2023-07-18 20:19:31.000000 swiftly-windows-0.0.5/swiftly_windows.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-18 20:19:31.000000 swiftly-windows-0.0.5/swiftly_windows.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       16 2023-07-18 20:19:31.000000 swiftly-windows-0.0.5/swiftly_windows.egg-info/top_level.txt
```

### Comparing `swiftly-windows-0.0.4/LICENSE` & `swiftly-windows-0.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-BSD 3-Clause License
-
-Copyright (c) 2023, Shubham Gupta
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2023, Shubham Gupta
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `swiftly-windows-0.0.4/scripts/swiftly.bat` & `swiftly-windows-0.0.5/scripts/swiftly.bat`

 * *Files 26% similar despite different names*

```diff
@@ -1,117 +1,182 @@
-@echo off
-REM Disable echo
-
-REM Check if the first argument is 'init' or 'makeapp'
-IF NOT "%~1"=="init" IF NOT "%~1"=="makeapp" (
-    echo Invalid command.
-    exit /b
-)
-
-IF "%~1"=="init" (
-    REM Call the init function with the second argument as a parameter
-    call:init "%~2"
-    GOTO:EOF
-)
-
-IF "%~1"=="makeapp" (
-    REM Call the makeapp function with the second argument as a parameter
-    call:makeapp "%~2"
-    GOTO:EOF
-)
-
-:init
-    REM Call pip install
-    call pip install swiftly-windows --upgrade > NUL
-    echo installation done
-
-    REM Check if parameter is empty
-    IF "%~1"=="" (
-        REM The commands in this block will execute if the parameter is empty
-
-        call git fetch > NUL 2>&1
-
-        for /f "delims=" %%a in ('git status -uno') do set "git_status=%%a"
-
-        for /f "delims=" %%a in ('python -c "from swiftly_windows.init import pull_changes; print(pull_changes('%git_status%'))"') do set "pull_changes=%%a"
-
-        IF "%pull_changes%"=="True" (
-            call git pull > NUL
-            echo git changes pulled
-        ) ELSE (
-            echo git up to date
-        )
-
-        for /f "delims=" %%a in ('python -c "from swiftly_windows.init import get_project_name; print(get_project_name())"') do set "PROJECT_NAME=%%a"
-        echo  Project '%PROJECT_NAME%' ready
-
-        for /f "delims=" %%a in ('python -c "from swiftly_windows.init import get_venv_location; print(get_venv_location())"') do set "venv_location=%%a"
-        call %venv_location%\Scripts\activate
-        set "PROJECT_VENV_LOCATION=%venv_location%"
-
-        call pip install swiftly-windows --upgrade > NUL 2>&1
-        echo  Virtual environment activated
-
-        for /f "delims=" %%a in ('pip freeze') do set "available_packages=%%a"
-        for /f "delims=" %%a in ('python -c "from swiftly_windows.init import check_new_packages; print(check_new_packages('%available_packages%'))"') do set "new_packages=%%a"
-
-        IF "%new_packages%"=="True" (
-            call pip install -r requirements.txt > NUL
-            echo  New packages installed
-        ) ELSE (
-            echo  All packages already installed
-        )
-
-        call pip install --upgrade pip > NUL 2>&1
-
-        call pip install swiftly-windows --upgrade > NUL 2>&1
-        echo  All checks completed swiftly
-    ) ELSE (
-        REM The commands in this block will execute if the parameter is not empty
-
-        for /f "delims=" %%a in ('python -c "from swiftly_windows.init import is_repo; print(is_repo('%~1'))"') do set "is_github_repo=%%a"
-
-        IF "%is_github_repo%"=="True" (
-            for /f "delims=" %%a in ('git clone %~1 2^>^&1') do set "git_clone=%%a"
-            for /f "delims=" %%a in ('python -c "from swiftly_windows.init import clone_successful; print(clone_successful('%git_clone%'))"') do set "clone_successful=%%a"
-
-            IF "%clone_successful%"=="True" (
-                echo  Git repository cloned
-            ) ELSE (
-                echo  %clone_successful% fail
-                echo Do you want to create a new project? (y/n)
-                set /p user_input="> "
-                set user_input=%user_input:~0,1%
-                IF /I NOT "%user_input%"=="y" (
-                    exit /b 1
-                )
-            )
-        )
-
-        for /f "delims=" %%a in ('python -c "from swiftly_windows.init import initialise; print(initialise('%~1'))"') do set "venv_location=%%a"
-        call %venv_location%\Scripts\activate
-        set "PROJECT_VENV_LOCATION=%venv_location%"
-
-        cd /D %venv_location%
-        cd ..
-
-        call pip install swiftly-windows --upgrade > NUL 2>&1
-
-        for /f "delims=" %%a in ('python -c "from swiftly_windows.init import get_project_name; print(get_project_name())"') do set "PROJECT_NAME=%%a"
-        echo  Project '%PROJECT_NAME%' ready
-
-        call pip install --upgrade pip > NUL 2>&1
-
-        call pip install -r requirements.txt > NUL
-        echo Requirements installed
-
-        call pip install swiftly-windows --upgrade > NUL 2>&1
-        echo  All checks completed swiftly
-    )
-
-    echo ✨ Project '%PROJECT_NAME%' initiated successfully :)
-
-:makeapp
-    REM Call Python function with arguments
-    python -c "from swiftly_windows.makeapp import makeapp; makeapp('%~1', '%PROJECT_VENV_LOCATION%')" > NUL
-    TIMEOUT /T 1 /NOBREAK > NUL
-    echo ✓ App '%~1' created successfully
+@echo off
+REM Disable echo
+REM Check if the first argument is 'init', 'makeapp', 'run', 'install', 'uninstall', or 'push'
+IF NOT "%~1"=="init" IF NOT "%~1"=="makeapp" IF NOT "%~1"=="run" IF NOT "%~1"=="install" IF NOT "%~1"=="uninstall" IF NOT "%~1"=="push" (
+    echo Invalid command.
+    exit /b
+)
+
+IF "%~1"=="init" (
+    REM Call the init function with the second argument as a parameter
+    call:init "%~2"
+    GOTO:EOF
+)
+
+IF "%~1"=="makeapp" (
+    REM Call the makeapp function with the second argument as a parameter
+    call:makeapp "%~2"
+    GOTO:EOF
+)
+
+IF "%~1"=="run" (
+    REM Call the run function with the second argument as a parameter
+    call:run "%~2"
+    GOTO:EOF
+)
+
+IF "%~1"=="install" (
+    REM Call the install function with all the rest arguments as a parameter
+    call:install %*:~2
+    GOTO:EOF
+)
+
+IF "%~1"=="uninstall" (
+    REM Call the uninstall function with all the rest arguments as a parameter
+    call:uninstall %*:~2
+    GOTO:EOF
+)
+
+IF "%~1"=="push" (
+    REM Call the push function with all the rest arguments as a parameter
+    call:push %*:~2
+    GOTO:EOF
+)
+
+:init
+    REM Call pip install
+    call pip install swiftly-windows --upgrade > NUL
+    echo installation done
+
+    REM Check if parameter is empty
+    IF "%~1"=="" (
+        REM The commands in this block will execute if the parameter is empty
+
+        call git fetch > NUL 2>&1
+
+        for /f "delims=" %%a in ('git status -uno') do set "git_status=%%a"
+
+        for /f "delims=" %%a in ('python -c "from swiftly_windows.init import pull_changes; print(pull_changes('%git_status%'))"') do set "pull_changes=%%a"
+
+        IF "%pull_changes%"=="True" (
+            call git pull > NUL
+            echo git changes pulled
+        ) ELSE (
+            echo git up to date
+        )
+
+        for /f "delims=" %%a in ('python -c "from swiftly_windows.init import get_project_name; print(get_project_name())"') do set "PROJECT_NAME=%%a"
+        echo  Project '%PROJECT_NAME%' ready
+
+        for /f "delims=" %%a in ('python -c "from swiftly_windows.init import get_venv_location; print(get_venv_location())"') do set "venv_location=%%a"
+        call %venv_location%\Scripts\activate
+        set "PROJECT_VENV_LOCATION=%venv_location%"
+
+        call pip install swiftly-windows --upgrade > NUL 2>&1
+        echo  Virtual environment activated
+
+        for /f "delims=" %%a in ('pip freeze') do set "available_packages=%%a"
+        for /f "delims=" %%a in ('python -c "from swiftly_windows.init import check_new_packages; print(check_new_packages('%available_packages%'))"') do set "new_packages=%%a"
+
+        IF "%new_packages%"=="True" (
+            call pip install -r requirements.txt > NUL
+            echo  New packages installed
+        ) ELSE (
+            echo  All packages already installed
+        )
+
+        call pip install --upgrade pip > NUL 2>&1
+
+        call pip install swiftly-windows --upgrade > NUL 2>&1
+        echo  All checks completed swiftly
+    ) ELSE (
+        REM The commands in this block will execute if the parameter is not empty
+
+        for /f "delims=" %%a in ('python -c "from swiftly_windows.init import is_repo; print(is_repo('%~1'))"') do set "is_github_repo=%%a"
+
+        IF "%is_github_repo%"=="True" (
+            for /f "delims=" %%a in ('git clone %~1 2^>^&1') do set "git_clone=%%a"
+            for /f "delims=" %%a in ('python -c "from swiftly_windows.init import clone_successful; print(clone_successful('%git_clone%'))"') do set "clone_successful=%%a"
+
+            IF "%clone_successful%"=="True" (
+                echo  Git repository cloned
+            ) ELSE (
+                echo  %clone_successful% fail
+                echo Do you want to create a new project? (y/n)
+                set /p user_input="> "
+                set user_input=%user_input:~0,1%
+                IF /I NOT "%user_input%"=="y" (
+                    exit /b 1
+                )
+            )
+        )
+
+        for /f "delims=" %%a in ('python -c "from swiftly_windows.init import initialise; print(initialise('%~1'))"') do set "venv_location=%%a"
+        call %venv_location%\Scripts\activate
+        set "PROJECT_VENV_LOCATION=%venv_location%"
+
+        cd /D %venv_location%
+        cd ..
+
+        call pip install swiftly-windows --upgrade > NUL 2>&1
+
+        for /f "delims=" %%a in ('python -c "from swiftly_windows.init import get_project_name; print(get_project_name())"') do set "PROJECT_NAME=%%a"
+        echo  Project '%PROJECT_NAME%' ready
+
+        call pip install --upgrade pip > NUL 2>&1
+
+        call pip install -r requirements.txt > NUL
+        echo Requirements installed
+
+        call pip install swiftly-windows --upgrade > NUL 2>&1
+        echo  All checks completed swiftly
+    )
+
+    echo ✨ Project '%PROJECT_NAME%' initiated successfully :)
+
+:makeapp
+    REM Call Python function with arguments
+    echo '%~1'
+    echo '%PROJECT_VENV_LOCATION%'
+    python -c "from swiftly_windows.makeapp import makeapp; makeapp('%~1', '%PROJECT_VENV_LOCATION%')" > NUL
+    TIMEOUT /T 1 /NOBREAK > NUL
+    echo ✓ App '%~1' created successfully
+
+
+:run
+    for /f %%i in ('python -c "from swiftly_windows.runapp import run_app; print(run_app('%~1', '%PROJECT_NAME%'))"') do set script_path=%%i
+    python -m %script_path%
+    goto :eof
+
+:install
+    setlocal EnableDelayedExpansion
+    set "params="
+    for %%a in (%*) do (
+        for /f "delims=: tokens=1" %%b in ("%%~a") do (
+            set "params=!params! %%b"
+        )
+    )
+    pip install !params!
+    echo %PROJECT_VENV_LOCATION%
+    pip freeze > '%PROJECT_VENV_LOCATION%\..\requirements.txt'
+    endlocal
+    goto :eof
+
+:uninstall
+    setlocal EnableDelayedExpansion
+    set "params="
+    for %%a in (%*) do (
+        for /f "delims=: tokens=1" %%b in ("%%~a") do (
+            set "params=!params! %%b"
+        )
+    )
+    pip uninstall !params!
+    echo %PROJECT_VENV_LOCATION%
+    pip freeze > '%PROJECT_VENV_LOCATION%\..\requirements.txt'
+    endlocal
+    goto :eof
+
+:push
+    git add *
+    git commit -m "%*"
+    git push
+    goto :eof
```

### Comparing `swiftly-windows-0.0.4/swiftly_windows/gitignore.py` & `swiftly-windows-0.0.5/swiftly_windows/gitignore.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-GITIGNORE = '''
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-cover/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-.pybuilder/
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-#   For a library or package, you might want to ignore these files since the code is
-#   intended to run in multiple environments; otherwise, check them in:
-# .python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# poetry
-#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
-#   This is especially recommended for binary packages to ensure reproducibility, and is more
-#   commonly ignored for libraries.
-#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
-#poetry.lock
-
-# pdm
-#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
-#pdm.lock
-#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
-#   in version control.
-#   https://pdm.fming.dev/#use-with-ide
-.pdm.toml
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env.py
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
-
-# pytype static type analyzer
-.pytype/
-
-# Cython debug symbols
-cython_debug/
-
-# PyCharm
-#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
-#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
-#  and can be added to the global gitignore or merged into this file.  For a more nuclear
-#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+GITIGNORE = '''
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+cover/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+.pybuilder/
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+# .python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# poetry
+#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
+#   This is especially recommended for binary packages to ensure reproducibility, and is more
+#   commonly ignored for libraries.
+#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
+#poetry.lock
+
+# pdm
+#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
+#pdm.lock
+#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
+#   in version control.
+#   https://pdm.fming.dev/#use-with-ide
+.pdm.toml
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env.py
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+# pytype static type analyzer
+.pytype/
+
+# Cython debug symbols
+cython_debug/
+
+# PyCharm
+#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
+#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
+#  and can be added to the global gitignore or merged into this file.  For a more nuclear
+#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
+#.idea/
 '''
```

### Comparing `swiftly-windows-0.0.4/swiftly_windows/init.py` & `swiftly-windows-0.0.5/swiftly_windows/init.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-import os
-import subprocess
-import configparser
-from swiftly_windows.makeapp import makeapp
-from swiftly_windows.gitignore import GITIGNORE
-from swiftly_windows.config import CONFIG_FILE
-
-def get_venv_location():
-    config = configparser.ConfigParser()
-    config.read(CONFIG_FILE)
-    project_name = config.get('DEFAULT', 'PROJECT_NAME')
-
-    venv_name = f'venv{project_name}'
-    venv_exists = os.path.exists(venv_name)
-
-    if not venv_exists:
-        subprocess.run(['python', '-m', 'venv', venv_name])
-
-        # Add the virtual environment to the .gitignore file
-        if not os.path.exists('.gitignore'):
-            with open('.gitignore', 'w') as f:
-                f.write(GITIGNORE)
-        with open('.gitignore', 'a') as f:
-            f.write(f'\n{venv_name}/')
-
-    venv_location = os.path.abspath(venv_name)
-    return venv_location
-
-def get_project_name():
-    config = configparser.ConfigParser()
-    config.read(CONFIG_FILE)
-    
-    try:
-        project_name = config.get('DEFAULT', 'PROJECT_NAME')
-    except configparser.NoOptionError:
-        # If the project name is not found in the config file, use the name of the current directory
-        dir_name = os.path.basename(os.getcwd())
-        # Replace any '-' characters with '_' to make it a valid Python module name
-        project_name = dir_name.replace('-', '_')
-        # Initialise the new project
-        initialise(project_name, in_place=True)
-    
-    return project_name
-
-
-def pull_changes(git_status):
-    return 'Your branch is behind' in git_status
-
-def check_new_packages(available_packages):
-    with open('requirements.txt', 'r') as f:
-        required_packages = f.read().splitlines()
-
-    available_packages = set(available_packages.split())
-    required_packages = set(required_packages)
-
-    return not required_packages.issubset(available_packages)
-
-def is_repo(name):
-    repo_markers = ["https://", "http://", ".git", "git@"]
-    
-    repo_check = [marker in name for marker in repo_markers]
-    return True in repo_check
-
-def clone_successful(git_clone):
-    if "ERROR:" in git_clone or "fatal:" in git_clone:
-        lines = git_clone.split('=')
-        error_lines = [line for line in lines if line.startswith(("ERROR:", "fatal:"))]
-        return ' '.join(error_lines)
-    else:
-        return True
-
-def initialise(name, in_place=False):
-    if is_repo(name):
-        name = name.split('/')[-1].replace('.git', '')
-
-    if not os.path.exists(name):
-        os.makedirs(name)
-    
-    if not in_place:
-        os.chdir(name)
-
-    if not os.path.exists('requirements.txt'):
-        with open('requirements.txt', 'w') as f:
-            pass
-        
-    if not os.path.exists('env.py'):
-        with open('env.py', 'w') as f:
-            pass
-        
-    if not os.path.exists('__init__.py'):
-        with open('__init__.py', 'w') as f:
-            pass
-
-    if not os.path.exists(CONFIG_FILE):
-        config = configparser.ConfigParser()
-        config['DEFAULT'] = {
-                                'PROJECT_NAME': name,
-                                'OBJECT_ORIENTED': False,
-                            }
-        
-        with open(CONFIG_FILE, 'w') as f:
-            config.write(f)
-
-    venv_location = get_venv_location()
-    
-    makeapp(name, venv_location)
-
-    return venv_location
+import os
+import subprocess
+import configparser
+from swiftly_windows.makeapp import makeapp
+from swiftly_windows.gitignore import GITIGNORE
+from swiftly_windows.config import CONFIG_FILE
+
+def get_venv_location():
+    config = configparser.ConfigParser()
+    config.read(CONFIG_FILE)
+    project_name = config.get('DEFAULT', 'PROJECT_NAME')
+
+    venv_name = f'venv{project_name}'
+    venv_exists = os.path.exists(venv_name)
+
+    if not venv_exists:
+        subprocess.run(['python', '-m', 'venv', venv_name])
+
+        # Add the virtual environment to the .gitignore file
+        if not os.path.exists('.gitignore'):
+            with open('.gitignore', 'w') as f:
+                f.write(GITIGNORE)
+        with open('.gitignore', 'a') as f:
+            f.write(f'\n{venv_name}/')
+
+    venv_location = os.path.abspath(venv_name)
+    return venv_location
+
+def get_project_name():
+    config = configparser.ConfigParser()
+    config.read(CONFIG_FILE)
+    
+    try:
+        project_name = config.get('DEFAULT', 'PROJECT_NAME')
+    except configparser.NoOptionError:
+        # If the project name is not found in the config file, use the name of the current directory
+        dir_name = os.path.basename(os.getcwd())
+        # Replace any '-' characters with '_' to make it a valid Python module name
+        project_name = dir_name.replace('-', '_')
+        # Initialise the new project
+        initialise(project_name, in_place=True)
+    
+    return project_name
+
+
+def pull_changes(git_status):
+    return 'Your branch is behind' in git_status
+
+def check_new_packages(available_packages):
+    with open('requirements.txt', 'r') as f:
+        required_packages = f.read().splitlines()
+
+    available_packages = set(available_packages.split())
+    required_packages = set(required_packages)
+
+    return not required_packages.issubset(available_packages)
+
+def is_repo(name):
+    repo_markers = ["https://", "http://", ".git", "git@"]
+    
+    repo_check = [marker in name for marker in repo_markers]
+    return True in repo_check
+
+def clone_successful(git_clone):
+    if "ERROR:" in git_clone or "fatal:" in git_clone:
+        lines = git_clone.split('=')
+        error_lines = [line for line in lines if line.startswith(("ERROR:", "fatal:"))]
+        return ' '.join(error_lines)
+    else:
+        return True
+
+def initialise(name, in_place=False):
+    if is_repo(name):
+        name = name.split('/')[-1].replace('.git', '')
+
+    if not os.path.exists(name):
+        os.makedirs(name)
+    
+    if not in_place:
+        os.chdir(name)
+
+    if not os.path.exists('requirements.txt'):
+        with open('requirements.txt', 'w') as f:
+            pass
+        
+    if not os.path.exists('env.py'):
+        with open('env.py', 'w') as f:
+            pass
+        
+    if not os.path.exists('__init__.py'):
+        with open('__init__.py', 'w') as f:
+            pass
+
+    if not os.path.exists(CONFIG_FILE):
+        config = configparser.ConfigParser()
+        config['DEFAULT'] = {
+                                'PROJECT_NAME': name,
+                                'OBJECT_ORIENTED': False,
+                            }
+        
+        with open(CONFIG_FILE, 'w') as f:
+            config.write(f)
+
+    venv_location = get_venv_location()
+    
+    makeapp(name, venv_location)
+
+    return venv_location
```

### Comparing `swiftly-windows-0.0.4/swiftly_windows/makeapp.py` & `swiftly-windows-0.0.5/swiftly_windows/makeapp.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-import os
-import configparser
-from swiftly_windows.config import CONFIG_FILE
-
-def makeapp(app_name, venv_location):
-    if '-' in app_name:
-        raise Exception("Not a valid app name. App names can not contain '-'")
-    
-    # Split the app_name into parts
-    app_parts = app_name.split('.')
-    
-    # Set the initial directory to the parent directory of the venv_location
-    current_dir = os.path.dirname(venv_location)
-    
-    # Create directories for each part in app_parts
-    for part in app_parts:
-        current_dir = os.path.join(current_dir, part)
-        os.makedirs(current_dir, exist_ok=True)
-    
-    # Create the __init__.py, __main__.py, app_name.py, and tests.py files in the final directory
-    # Only create the files if they do not already exist
-    if not os.path.exists(os.path.join(current_dir, '__init__.py')):
-        with open(os.path.join(current_dir, '__init__.py'), 'w') as f:
-            f.write(f'from .{app_parts[-1]} import *')
-    
-    if not os.path.exists(os.path.join(current_dir, '__main__.py')):
-        with open(os.path.join(current_dir, '__main__.py'), 'w') as f:
-            f.write(f'from .{app_parts[-1]} import *\n\n# Run the code from {app_parts[-1]}.py here')
-    
-    # Read the configuration file to determine whether to create a class or a function
-    config = configparser.ConfigParser()
-    config.read(os.path.join(venv_location, '..', CONFIG_FILE))
-    object_oriented = config.getboolean('DEFAULT', 'OBJECT_ORIENTED')
-    
-    if not os.path.exists(os.path.join(current_dir, f'{app_parts[-1]}.py')):
-        with open(os.path.join(current_dir, f'{app_parts[-1]}.py'), 'w') as f:
-            if object_oriented:
-                # Convert the app_name to CamelCase
-                class_name = ''.join(word.title() for word in app_parts[-1].split('_'))
-                f.write(f'class {class_name}:\n    def __init__(self):\n        pass')
-            else:
-                f.write(f'def {app_parts[-1]}():\n    pass')
-    
-    if not os.path.exists(os.path.join(current_dir, 'tests.py')):
-        with open(os.path.join(current_dir, 'tests.py'), 'w') as f:
-            f.write('# May all your tests pass :)')
+import os
+import configparser
+from swiftly_windows.config import CONFIG_FILE
+
+def makeapp(app_name, venv_location):
+    if '-' in app_name:
+        raise Exception("Not a valid app name. App names can not contain '-'")
+    
+    # Split the app_name into parts
+    app_parts = app_name.split('.')
+    
+    # Set the initial directory to the parent directory of the venv_location
+    current_dir = os.path.dirname(venv_location)
+    
+    # Create directories for each part in app_parts
+    for part in app_parts:
+        current_dir = os.path.join(current_dir, part)
+        os.makedirs(current_dir, exist_ok=True)
+    
+    # Create the __init__.py, __main__.py, app_name.py, and tests.py files in the final directory
+    # Only create the files if they do not already exist
+    if not os.path.exists(os.path.join(current_dir, '__init__.py')):
+        with open(os.path.join(current_dir, '__init__.py'), 'w') as f:
+            f.write(f'from .{app_parts[-1]} import *')
+    
+    if not os.path.exists(os.path.join(current_dir, '__main__.py')):
+        with open(os.path.join(current_dir, '__main__.py'), 'w') as f:
+            f.write(f'from .{app_parts[-1]} import *\n\n# Run the code from {app_parts[-1]}.py here')
+    
+    # Read the configuration file to determine whether to create a class or a function
+    config = configparser.ConfigParser()
+    config.read(os.path.join(venv_location, '..', CONFIG_FILE))
+    object_oriented = config.getboolean('DEFAULT', 'OBJECT_ORIENTED')
+    
+    if not os.path.exists(os.path.join(current_dir, f'{app_parts[-1]}.py')):
+        with open(os.path.join(current_dir, f'{app_parts[-1]}.py'), 'w') as f:
+            if object_oriented:
+                # Convert the app_name to CamelCase
+                class_name = ''.join(word.title() for word in app_parts[-1].split('_'))
+                f.write(f'class {class_name}:\n    def __init__(self):\n        pass')
+            else:
+                f.write(f'def {app_parts[-1]}():\n    pass')
+    
+    if not os.path.exists(os.path.join(current_dir, 'tests.py')):
+        with open(os.path.join(current_dir, 'tests.py'), 'w') as f:
+            f.write('# May all your tests pass :)')
```

