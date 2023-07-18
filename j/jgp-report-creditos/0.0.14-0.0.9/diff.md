# Comparing `tmp/jgp_report_creditos-0.0.14.tar.gz` & `tmp/jgp_report_creditos-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jgp_report_creditos-0.0.14.tar", last modified: Tue Jul 18 05:12:53 2023, max compression
+gzip compressed data, was "jgp_report_creditos-0.0.9.tar", last modified: Mon Jun  5 16:17:06 2023, max compression
```

## Comparing `jgp_report_creditos-0.0.14.tar` & `jgp_report_creditos-0.0.9.tar`

### file list

```diff
@@ -1,40 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 05:12:53.637903 jgp_report_creditos-0.0.14/
--rw-rw-rw-   0        0        0     1074 2023-06-15 20:54:52.000000 jgp_report_creditos-0.0.14/LICENSE
--rw-rw-rw-   0        0        0     6723 2023-07-18 05:12:53.637903 jgp_report_creditos-0.0.14/PKG-INFO
--rw-rw-rw-   0        0        0     6246 2023-06-15 20:54:52.000000 jgp_report_creditos-0.0.14/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 05:12:53.615960 jgp_report_creditos-0.0.14/jgp_report_creditos/
--rw-rw-rw-   0        0        0       83 2023-06-15 20:54:52.000000 jgp_report_creditos-0.0.14/jgp_report_creditos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 05:12:53.624936 jgp_report_creditos-0.0.14/jgp_report_creditos/core/
--rw-rw-rw-   0        0        0       56 2023-06-19 20:47:24.000000 jgp_report_creditos-0.0.14/jgp_report_creditos/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 05:12:53.625933 jgp_report_creditos-0.0.14/jgp_report_creditos/core/contrato/
--rw-rw-rw-   0        0        0        0 2023-06-15 20:54:52.000000 jgp_report_creditos-0.0.14/jgp_report_creditos/core/contrato/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 05:12:53.628925 jgp_report_creditos-0.0.14/jgp_report_creditos/core/contrato/v1/
--rw-rw-rw-   0        0        0     4711 2023-06-16 14:55:12.000000 jgp_report_creditos-0.0.14/jgp_report_creditos/core/contrato/v1/Controlar tablas de firmas.py
--rw-rw-rw-   0        0        0        0 2023-06-15 20:54:52.000000 jgp_report_creditos-0.0.14/jgp_report_creditos/core/contrato/v1/__init__.py
--rw-rw-rw-   0        0        0   149447 2023-07-18 05:07:24.000000 jgp_report_creditos-0.0.14/jgp_report_creditos/core/contrato/v1/base.py
--rw-rw-rw-   0        0        0    20081 2023-06-24 15:53:30.000000 jgp_report_creditos-0.0.14/jgp_report_creditos/core/contrato/v1/contratos.py
--rw-rw-rw-   0        0        0    36882 2023-07-13 16:07:40.000000 jgp_report_creditos-0.0.14/jgp_report_creditos/core/deposito.py
-drwxrwxrwx   0        0        0        0 2023-07-18 05:12:53.630919 jgp_report_creditos-0.0.14/jgp_report_creditos/core/exception/
--rw-rw-rw-   0        0        0       37 2023-06-15 20:54:52.000000 jgp_report_creditos-0.0.14/jgp_report_creditos/core/exception/__init__.py
--rw-rw-rw-   0        0        0      309 2023-06-15 20:54:52.000000 jgp_report_creditos-0.0.14/jgp_report_creditos/core/exception/exception.py
--rw-rw-rw-   0        0        0     6588 2023-07-13 18:43:00.000000 jgp_report_creditos-0.0.14/jgp_report_creditos/core/rutas.py
--rw-rw-rw-   0        0        0    21974 2023-07-17 19:38:22.000000 jgp_report_creditos-0.0.14/jgp_report_creditos/report.py
-drwxrwxrwx   0        0        0        0 2023-07-18 05:12:53.610973 jgp_report_creditos-0.0.14/jgp_report_creditos/resources/
-drwxrwxrwx   0        0        0        0 2023-07-18 05:12:53.630919 jgp_report_creditos-0.0.14/jgp_report_creditos/resources/img/
--rw-rw-rw-   0        0        0    57446 2023-06-15 20:54:52.000000 jgp_report_creditos-0.0.14/jgp_report_creditos/resources/img/logo_jgp.png
-drwxrwxrwx   0        0        0        0 2023-07-18 05:12:53.633912 jgp_report_creditos-0.0.14/jgp_report_creditos/template/
--rw-rw-rw-   0        0        0        0 2023-06-17 16:56:44.000000 jgp_report_creditos-0.0.14/jgp_report_creditos/template/__init__.py
--rw-rw-rw-   0        0        0    22964 2023-07-12 19:53:26.000000 jgp_report_creditos-0.0.14/jgp_report_creditos/template/components.py
--rw-rw-rw-   0        0        0      660 2023-06-17 16:08:06.000000 jgp_report_creditos-0.0.14/jgp_report_creditos/template/template.py
--rw-rw-rw-   0        0        0      714 2023-06-15 21:23:54.000000 jgp_report_creditos-0.0.14/jgp_report_creditos/test.py
-drwxrwxrwx   0        0        0        0 2023-07-18 05:12:53.635907 jgp_report_creditos-0.0.14/jgp_report_creditos/tests/
--rw-rw-rw-   0        0        0        0 2023-06-17 16:57:48.000000 jgp_report_creditos-0.0.14/jgp_report_creditos/tests/__init__.py
--rw-rw-rw-   0        0        0     1036 2023-07-18 05:02:35.000000 jgp_report_creditos-0.0.14/jgp_report_creditos/tests/test_contratos.py
--rw-rw-rw-   0        0        0    33149 2023-07-13 18:42:44.000000 jgp_report_creditos-0.0.14/jgp_report_creditos/tests/test_deposito.py
-drwxrwxrwx   0        0        0        0 2023-07-18 05:12:53.621945 jgp_report_creditos-0.0.14/jgp_report_creditos.egg-info/
--rw-rw-rw-   0        0        0     6723 2023-07-18 05:12:53.000000 jgp_report_creditos-0.0.14/jgp_report_creditos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1045 2023-07-18 05:12:53.000000 jgp_report_creditos-0.0.14/jgp_report_creditos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 05:12:53.000000 jgp_report_creditos-0.0.14/jgp_report_creditos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-18 05:12:53.000000 jgp_report_creditos-0.0.14/jgp_report_creditos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 05:12:53.638899 jgp_report_creditos-0.0.14/setup.cfg
--rw-rw-rw-   0        0        0      975 2023-07-17 13:45:00.000000 jgp_report_creditos-0.0.14/setup.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-05 16:17:06.772341 jgp_report_creditos-0.0.9/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     7363 2023-06-05 16:17:06.772341 jgp_report_creditos-0.0.9/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)     6246 2023-06-05 15:25:25.000000 jgp_report_creditos-0.0.9/README.md
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-05 16:17:06.768340 jgp_report_creditos-0.0.9/jgp_report_creditos/
+-rw-rw-r--   0 axel      (1000) axel      (1000)       83 2023-05-15 21:24:18.000000 jgp_report_creditos-0.0.9/jgp_report_creditos/__init__.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-05 16:17:06.772341 jgp_report_creditos-0.0.9/jgp_report_creditos/core/
+-rw-rw-r--   0 axel      (1000) axel      (1000)        0 2023-05-04 12:51:20.000000 jgp_report_creditos-0.0.9/jgp_report_creditos/core/__init__.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-05 16:17:06.772341 jgp_report_creditos-0.0.9/jgp_report_creditos/core/contrato/
+-rw-rw-r--   0 axel      (1000) axel      (1000)        0 2023-05-08 15:26:09.000000 jgp_report_creditos-0.0.9/jgp_report_creditos/core/contrato/__init__.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-05 16:17:06.772341 jgp_report_creditos-0.0.9/jgp_report_creditos/core/contrato/v1/
+-rw-rw-r--   0 axel      (1000) axel      (1000)        0 2023-05-08 15:26:09.000000 jgp_report_creditos-0.0.9/jgp_report_creditos/core/contrato/v1/__init__.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)   145944 2023-06-05 16:03:31.000000 jgp_report_creditos-0.0.9/jgp_report_creditos/core/contrato/v1/base.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)    19761 2023-05-16 19:16:33.000000 jgp_report_creditos-0.0.9/jgp_report_creditos/core/contrato/v1/contratos.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-05 16:17:06.772341 jgp_report_creditos-0.0.9/jgp_report_creditos/core/exception/
+-rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-05-15 21:24:18.000000 jgp_report_creditos-0.0.9/jgp_report_creditos/core/exception/__init__.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      309 2023-05-15 21:24:18.000000 jgp_report_creditos-0.0.9/jgp_report_creditos/core/exception/exception.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     3791 2023-06-01 17:41:20.000000 jgp_report_creditos-0.0.9/jgp_report_creditos/report.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      714 2023-06-01 17:41:20.000000 jgp_report_creditos-0.0.9/jgp_report_creditos/test.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-05 16:17:06.772341 jgp_report_creditos-0.0.9/jgp_report_creditos.egg-info/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     7363 2023-06-05 16:17:06.000000 jgp_report_creditos-0.0.9/jgp_report_creditos.egg-info/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)      602 2023-06-05 16:17:06.000000 jgp_report_creditos-0.0.9/jgp_report_creditos.egg-info/SOURCES.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-06-05 16:17:06.000000 jgp_report_creditos-0.0.9/jgp_report_creditos.egg-info/dependency_links.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       20 2023-06-05 16:17:06.000000 jgp_report_creditos-0.0.9/jgp_report_creditos.egg-info/top_level.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-06-05 16:17:06.772341 jgp_report_creditos-0.0.9/setup.cfg
+-rw-rw-r--   0 axel      (1000) axel      (1000)      976 2023-06-05 16:16:28.000000 jgp_report_creditos-0.0.9/setup.py
```

### Comparing `jgp_report_creditos-0.0.14/PKG-INFO` & `jgp_report_creditos-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-Metadata-Version: 2.1
-Name: jgp_report_creditos
-Version: 0.0.14
-Summary: Librería con funciones y herramientas útiles exclusivas para jgp
-Home-page: https://gitlab.com/develop-team-jdgp/jgp-report-creditos.git
-Author: JGP Dev
-Author-email: jgpdev20@gmail.com
-License: MIT
-Keywords: python,primer paquete jgp
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# jgp-report-creditos
-
-
-
-## Getting started
-
-To make it easy for you to get started with GitLab, here's a list of recommended next steps.
-
-Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!
-
-## Add your files
-
-- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
-- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
-
-```
-cd existing_repo
-git remote add origin https://gitlab.com/develop-team-jdgp/jgp-report-creditos.git
-git branch -M main
-git push -uf origin main
-```
-
-## Integrate with your tools
-
-- [ ] [Set up project integrations](https://gitlab.com/develop-team-jdgp/jgp-report-creditos/-/settings/integrations)
-
-## Collaborate with your team
-
-- [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
-- [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
-- [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
-- [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
-- [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)
-
-## Test and Deploy
-
-Use the built-in continuous integration in GitLab.
-
-- [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)
-- [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
-- [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
-- [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
-- [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)
-
-***
-
-# Editing this README
-
-When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.
-
-## Suggestions for a good README
-Every project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.
-
-## Name
-Choose a self-explaining name for your project.
-
-## Description
-Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
-
-## Badges
-On some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.
-
-## Visuals
-Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.
-
-## Installation
-Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.
-
-## Usage
-Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
-
-## Support
-Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.
-
-## Roadmap
-If you have ideas for releases in the future, it is a good idea to list them in the README.
-
-## Contributing
-State if you are open to contributions and what your requirements are for accepting them.
-
-For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.
-
-You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.
-
-## Authors and acknowledgment
-Show your appreciation to those who have contributed to the project.
-
-## License
-For open source projects, say how it is licensed.
-
-## Project status
-If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
+Metadata-Version: 2.1
+Name: jgp_report_creditos
+Version: 0.0.9
+Summary: Librería con funciones y herramientas útiles exclusivas para jgp
+Home-page: https://gitlab.com/develop-team-jdgp/jgp-report-creditos.git
+Author: JGP Dev
+Author-email: jgpdev20@gmail.com
+License: MIT
+Description: # jgp-report-creditos
+        
+        
+        
+        ## Getting started
+        
+        To make it easy for you to get started with GitLab, here's a list of recommended next steps.
+        
+        Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!
+        
+        ## Add your files
+        
+        - [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
+        - [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
+        
+        ```
+        cd existing_repo
+        git remote add origin https://gitlab.com/develop-team-jdgp/jgp-report-creditos.git
+        git branch -M main
+        git push -uf origin main
+        ```
+        
+        ## Integrate with your tools
+        
+        - [ ] [Set up project integrations](https://gitlab.com/develop-team-jdgp/jgp-report-creditos/-/settings/integrations)
+        
+        ## Collaborate with your team
+        
+        - [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
+        - [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
+        - [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
+        - [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
+        - [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)
+        
+        ## Test and Deploy
+        
+        Use the built-in continuous integration in GitLab.
+        
+        - [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)
+        - [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
+        - [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
+        - [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
+        - [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)
+        
+        ***
+        
+        # Editing this README
+        
+        When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.
+        
+        ## Suggestions for a good README
+        Every project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.
+        
+        ## Name
+        Choose a self-explaining name for your project.
+        
+        ## Description
+        Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
+        
+        ## Badges
+        On some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.
+        
+        ## Visuals
+        Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.
+        
+        ## Installation
+        Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.
+        
+        ## Usage
+        Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
+        
+        ## Support
+        Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.
+        
+        ## Roadmap
+        If you have ideas for releases in the future, it is a good idea to list them in the README.
+        
+        ## Contributing
+        State if you are open to contributions and what your requirements are for accepting them.
+        
+        For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.
+        
+        You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.
+        
+        ## Authors and acknowledgment
+        Show your appreciation to those who have contributed to the project.
+        
+        ## License
+        For open source projects, say how it is licensed.
+        
+        ## Project status
+        If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
+        
+Keywords: python,primer paquete jgp
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `jgp_report_creditos-0.0.14/README.md` & `jgp_report_creditos-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `jgp_report_creditos-0.0.14/jgp_report_creditos/core/contrato/v1/base.py` & `jgp_report_creditos-0.0.9/jgp_report_creditos/core/contrato/v1/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from reportlab.lib.pagesizes import A4
 from reportlab.lib.units import mm, inch, cm
 from reportlab.lib.enums import TA_JUSTIFY, TA_CENTER, TA_LEFT
 from reportlab.lib.pagesizes import letter
 from reportlab.platypus import SimpleDocTemplate, Paragraph, Spacer, ListFlowable
 from reportlab.lib.styles import getSampleStyleSheet, ParagraphStyle
 from reportlab.lib.units import inch
-from reportlab.platypus import (SimpleDocTemplate, Spacer, Paragraph, Table, PageBreak)
+from reportlab.platypus import (SimpleDocTemplate, Spacer, Paragraph, Table)
 from reportlab.lib.styles import getSampleStyleSheet
 from reportlab.lib import colors
 from io import BytesIO
 import datetime
 import os.path
 
 #Add styles
@@ -27,89 +27,71 @@
 estilos.add(ParagraphStyle(name = 'Inciso', alignment=TA_JUSTIFY, bulletAnchor = 'start', fontSize=9.1, fontName = 'Helvetica'))
 
 estilos.add(ParagraphStyle(name = 'Terror', alignment=TA_CENTER, fontSize=40, textColor= 'red', fontName = 'Helvetica'))
 estilos.add(ParagraphStyle(name = 'Derror', alignment=TA_CENTER, fontSize=12, textColor= 'black', fontName = 'Helvetica'))
 
 #"Contrato Personal Base1.pdf"
 def documentos(nombre_document):
-    return SimpleDocTemplate(nombre_document, pagesize=letter, rightMargin=19*mm, leftMargin=19*mm,
+    return SimpleDocTemplate(nombre_document, pagesize=letter, rightMargin=10.1*mm, leftMargin=16*mm,
                             topMargin=24*mm, bottomMargin=17*mm)
 
-
-class NumberedCanvas(canvas.Canvas):
-    def __init__(self, *args, **kwargs):
-        canvas.Canvas.__init__(self, *args, **kwargs)
-        self.Canvas = canvas.Canvas
-        self._saved_page_states = []
-    def showPage(self):
-        self._saved_page_states.append(dict(self.__dict__))
-        self._startPage()
-    def save(self):
-        """add page info to each page (page x of y)"""
-        num_pages = len(self._saved_page_states)
-        for state in self._saved_page_states:
-            self.__dict__.update(state)
-            self.draw_page_number(num_pages)
-            self.Canvas.showPage(self)
-        self.Canvas.save(self)
-    def draw_page_number(self, page_count):  
-        self.setFont('Helvetica',8)
-        ancho, alto = letter
-        x,y= letter
-        page = " %s de %s" % (self._pageNumber, page_count)       
-        self.saveState()
-        """ PIE DE PAGINA """
-        # Agregar footer en cada página
-        self.drawString(x/2, 1*cm, page)
-        self.restoreState()
-        
-
-
 # -------------------PARRAFOS DE LOS CONTRATOS----------------------
 class BaseContrato :   
     _parrafos = []
     #creacion de cosntructores
-    def __init__(self, contrato, usuario):
+    def __init__(self, contrato):
         self.__contrato = contrato
-        self.usuario = usuario
     
     # footer and header
-    
     def _encabezado(self,canvas,doc):
         """Header of page"""
         canvas.saveState()
         #tipo y tamaño de letra
-        canvas.setFont('Helvetica',5.8)
+        canvas.setFont('Helvetica',6)
         #obtengo la fecha actual
         x= datetime.datetime.now()
         #setting model of date
         formatoFecha= x.strftime("%d/%m/%Y")
+        usuario= "150"
         codigo_operacion=self.__contrato["codigo_operacion"]
-
+        usuario_actualizacion=self.__contrato["testimonio_poder"]["usuario_actualizacion"]
+        
         #posicion del encabezado(x, y, texto)
-        canvas.drawString(2*cm, A4[1]-86, formatoFecha)
-        canvas.drawString(2*cm, A4[1]-94, str(self.usuario))
-        canvas.drawString(2*cm, A4[1]-103, codigo_operacion)
+        canvas.drawString(0.68*inch, A4[1]-78, formatoFecha)
+        canvas.drawString(0.68*inch, A4[1]-87, str(usuario_actualizacion))
+        canvas.drawString(0.68*inch, A4[1]-96, codigo_operacion)
         canvas.restoreState()
-
         """footer of page"""
         canvas.saveState()
         canvas.setFont('Helvetica',7)
-        
-        
+        #para colocar la posicion del pie de pagina (x, y, texto)
+        canvas.drawString(4.2 *inch, 0.5 * inch, " %d" % doc.page)
         #ssetting only page 2k+1
         if(doc.page%2!=0):
             # Dibujamos una imagen (IMAGEN, X,Y, WIDTH, HEIGH)
             img = os.path.join(os.path.dirname(os.path.abspath(__file__)),'../../../resources/img/logo_jgp.png')
-            canvas.drawImage(img, 14*cm, 730, 160, 35, mask=None)     
+            canvas.drawImage(img, 420, 730, 160, 35, mask=None)     
         canvas.restoreState()
     
     #
     def _error_mensaje1(self,message):
         self._parrafos.clear()
+        
+        """
+        packet = io.BytesIO()
+
+        mi_canvas = canvas.Canvas(packet, pagesize=letter)
+        mi_canvas.saveState()    
+        usuario_actualizacion= "ERROR AL GENERAR CONTRATO!!!!!!!!11"       
+        mi_canvas.setFillColorRGB(1,0,0) #choose your font colour
+        mi_canvas.setFont("Helvetica", 30) #choose your font type and font size
+        mi_canvas.drawString(0.68*inch, A4[1]-67, usuario_actualizacion)
+        mi_canvas.restoreState()
+        return packet
+        """
 
     # pdf en blanco ERROR
     def _error_mensaje(self, title_error, description_error):
         self._parrafos.clear()
         titulo=f'<b>{title_error}</b> <br/> '
         self._parrafos.append(Paragraph(titulo, estilos["Terror"]))
         self._parrafos.append(Paragraph("________________", estilos["Terror"]))
@@ -142,15 +124,15 @@
         cargo = testimonio_poder["representante_legal"]["rol"]       
         numero_testimonio = testimonio_poder["numero_testimonio"]
         fecha_testimonio = Utils.get_fecha(self, testimonio_poder["fecha_testimonio"])
         numero_notaria = testimonio_poder["numero_notaria_publica"]
         responsable_notaria = testimonio_poder["nombre_notario_publico"]
         texto = f'<b><u>{numeral}</u>.- (PARTES CONTRATANTES)</b>.- Intervienen en la suscripción del presente contrato:'
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
-        a = f'<b>GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A.</b>, sociedad \
+        a = f'<b>GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.</b>, sociedad \
             legalmente constituida bajo las leyes del Estado Plurinacional de Bolivia, con Matrícula de \
             Comercio y Número de Identificación Tributaria 173788022, con domicilio en la \
             {domicilio_legal} de esta ciudad, representada legalmente por <b>{apoderado}</b>, con C.I. Nº {numero_ci_apoderado}, mayor de edad, hábil \
             por derecho y vecino(a) de esta ciudad, en su condición de {cargo} en mérito al \
             Testimonio Poder No. {numero_testimonio} de fecha {fecha_testimonio} otorgado por ante la \
             Notaría de Fe Pública Nº {numero_notaria} del Distrito Judicial de La Paz a cargo de(la) Dr(a).\
             {responsable_notaria}, quien en adelante se denominará <b>"EL ACREEDOR"</b>.'
@@ -181,15 +163,14 @@
         if(len(fiadores)>0):
             c=""
             c = "El(la)(los) señor(a)(es) "
             j=0
             for item in fiadores:
                 j+=1
                 nombreFiador = item['nombre_completo'].upper()
-                
                 numeroCiFiador = item['ci']
                 estadoCivilFiador = self.get_estado_civil(item['estado_civil'],item['genero'])
                 domicilioFiador = item['direccion']
                 domicilio_fiador = self.get_articulo_direccion(domicilioFiador)
                 auxfiador = f'<b>{nombreFiador}</b> con <b>C.I. Nº {numeroCiFiador}</b>, de nacionalidad \
                 boliviana, de estado civil {estadoCivilFiador}, domiciliado(a)(s) en {domicilio_fiador}'
                 c = c + auxfiador
@@ -228,26 +209,26 @@
         cargo = testimonio_poder["representante_legal"]["rol"]       
         numero_testimonio = testimonio_poder["numero_testimonio"]
         fecha_testimonio = Utils.get_fecha(self, testimonio_poder["fecha_testimonio"])
         numero_notaria = testimonio_poder["numero_notaria_publica"]
         responsable_notaria = testimonio_poder["nombre_notario_publico"]
         texto = f'<b><u>{numeral}</u>.- (PARTES CONTRATANTES)</b>.- Intervienen en la suscripción del presente contrato:'
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
-        a = f'<b>GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A.</b>, sociedad \
+        a = f'<b>GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.</b>, sociedad \
             legalmente constituida bajo las leyes del Estado Plurinacional de Bolivia, con Matrícula de \
             Comercio y Número de Identificación Tributaria 173788022, con domicilio en la \
             {domicilio_legal} de esta ciudad, representada legalmente por <b>{apoderado}</b>, con C.I. Nº {numero_ci_apoderado}, mayor de edad, hábil \
             por derecho y vecino(a) de esta ciudad, en su condición de {cargo} en mérito al \
             Testimonio Poder No. {numero_testimonio} de fecha {fecha_testimonio} otorgado por ante la \
             Notaría de Fe Pública Nº {numero_notaria} del Distrito Judicial de La Paz a cargo de(la) Dr(a).\
             {responsable_notaria}, quien en adelante se denominará <b>"EL ACREEDOR"</b>.'
-        # Insiso b)
         b = "El(la)(los) señor(a)(es) "
         deudores = self.get_deudores()
         i=0
+        #55555555555555555555555555555555555555
         for item in deudores:
             i+=1
             nombreDeudor = item['nombre_completo'].upper()
             numeroCiDeudor = item['ci']
             estadoCivilDeudor = self.get_estado_civil(item['estado_civil'],item['genero'])
             domicilioDeudor = item['direccion']
             domicilio_deudor = self.get_articulo_direccion(domicilioDeudor)
@@ -256,15 +237,15 @@
             b = b + aux
             if (i != len(deudores)-1):
                 b = b + ","+" "
             else:
                 b = b + " y"+" "
         aux1='mayor(es) de edad y hábil(es) por derecho, que en lo sucesivo se denominará(n) <b>"El(la)(los) DEUDOR(A)(ES)"</b>.'
         b=b+aux1
-        #Insiso c)
+        #para el inciso c
         fiadores = self.get_fiadores()
         c=""
         #5555555555555555555555555
         if(len(fiadores)>0):
             c = "El(la)(los) señor(a)(es) "
             j=0
             for item in fiadores:
@@ -296,15 +277,15 @@
             bulletFontName='Helvetica-Bold',
             bulletFontSize=9.1,
             bulletOffsetY=0,
             bulletDedent=20        
             )
             self._parrafos.append(incisos)
         else:   
-            raise ContratoError("Campo requerido", "El contrato requiere los Datos del(los) Garante(es)")
+            raise ContratoError("Campo requerido", "El contrato requiere los Datos de fiadores")
     
 
     def _objeto_del_contrato(self, numeral):
         monto1=float(self.__contrato["monto_aprobado"])
         monto = Utils.literalEnteroMontoPrestamo(monto1)
         motivo_prestamo = self.__contrato["motivo_prestamo"].upper()
         texto_objeto = f'<b><u>{numeral}</u>.- (OBJETO DEL CONTRATO, MONTO, MONEDA Y DESTINO DEL PRÉSTAMO)</b>.- \
@@ -524,26 +505,26 @@
         garantias=self.__contrato["garantias_reales"]
         sw=False
         for item in garantias:
             if(item['concepto']=="Descripcion"):
                 prendaria=item['detalle_garantia']  
                 sw=True
         if(sw==False):
-            raise ContratoError("Campo requerido", "El contrato requiere los Datos de la garantia por concepto de: Descripción")
+            raise ContratoError("Campo requerido", "El contrato requiere los Datos de concepto: Descripcion")
         return prendaria
 
     def get_direccion_g(self):
         garantias=self.__contrato["garantias_reales"]
         sw=False
         for item in garantias:
             if(item['concepto']=="Ubicacion"):
                 ubicacion=item['detalle_garantia']
                 sw=True 
         if(sw==False):
-            raise ContratoError("Campo requerido", "El contrato requiere los Datos de la garantia por concepto de: Ubicación")            
+            raise ContratoError("Campo requerido", "El contrato requiere los Datos de concepto: Ubicacion")            
         return ubicacion.upper()
         
     #METODOS PARA detalle_garantia
     def isNumeric(self,s):
         try:
             int(s)
             return True
@@ -594,15 +575,15 @@
             texto_10_2 = f' <b>10.2. "El(la)(los) DEUDOR(A)(ES)"</b> otorgará(n) al <b>ACREEDOR</b> como garantía {prendaria}, cuyas \
                 características se encuentran detalladas y descritas en el formulario <b>"Avalúo de Garantía Prendaria"</b>, misma \
                 que forma parte integrante de este contrato sin necesidad de ser transcrito, siendo aplicable para esta operación la \
                 normativa legal vigente consignada en los artículos 1403 y siguientes del Código Civil.<br/> \
                 A solicitud expresa del(la)(los) <b>DEPOSITARIO(S)</b> los bienes constituidos en prenda permanecerán en la <b>{direccion_garantia}</b>, bienes que quedarán en depósito y/o poder de '
             c=texto_10_2
         else:
-            raise ContratoError("Campo requerido", "El contrato requiere los Datos de la garantia real, revisar la garantia por concepto de: Ubicacion ó Descripcion")
+            raise ContratoError("Campo requerido", "El contrato requiere los Datos de al menos dos garantias reales")
 
         if(len(fiadores)>0):
             c = c+ '<b>"El(la)(los) GARANTE(S) DEPOSITARIO(S)"</b>'
             j=0
             for item in fiadores:
                 j+=1
                 nombreFiador = item['nombre_completo'].upper()
@@ -614,15 +595,15 @@
                 else:
                     c = c + " y"+" "
             aux3='quien(es) a la suscripción del presente documento se declara(n) en posesión física, material y real de los bienes otorgados en prenda, los mismos que se encuentran en perfecto estado de conservación y/o funcionamiento, con las obligaciones y responsabilidades correspondientes al depositario gratuito, quedando encargado(s) de su cuidado, guarda y conservación por su cuenta exclusiva, asumiendo solidariamente todas las obligaciones y responsabilidades civiles y penales propias a su(s) condición(es) de depositario(s) que establecen disposiciones relativas al depósito y prenda, facultando a <b>"EL ACREEDOR"</b> a exigir su permanente exhibición, debiendo <b>"El(la)(los) DEPOSITARIO(S)"</b> mantener informado a <b>"EL ACREEDOR"</b> del lugar donde se encuentra la prenda, sobre cualquier cambio que se produzca respecto de la conservación o cualquier riesgo que puedan sufrir los bienes otorgados en prenda, dicha información debe realizarse por escrito dentro de los quinde (15) días siguientes de ocurrido el hecho. Trasladar la prenda a donde y cuando lo disponga <b>"EL ACREEDOR"</b>. Los bienes dados en prenda, no podrán ser cambiados del lugar de ubicación salvo consentimiento expreso de <b>"EL ACREEDOR".</b><br/> \
             Sobre los bienes de la prenda no existen obligaciones ni restricciones de ninguna clase que pudieran reclamar terceros, según declaración expresa que hace <b>"El(la)(los) DEUDOR(A)(ES)".</b>'
 
             self._parrafos.append(Paragraph(c+aux3, estilos['Justify']))
         else:
-            raise ContratoError("Campo requerido", "El contrato requiere los Datos de al menos un Garante")
+            raise ContratoError("Campo requerido", "El contrato requiere los Datos de al menos dos garantias reales")
         
         
         #LLAMAMOS A LOS FIADORES
         texto_10_3 = "<b>10.3.</b> Con la Garantía personal, solidaria, mancomunada e indivisible del (la)(los) señor(a)(es)"
         fiadores = self.get_fiadores()
         i=0
         for item in fiadores:
@@ -657,14 +638,17 @@
                 y cuenta con el acuerdo y consentimiento de éste(a).<br/>\
                 <b>"El(la)(los) DEUDOR(A)(ES)"</b> y/o <b>"El(la)(los) GARANTE(S) PERSONAL(ES)"</b> autoriza(n) que, \
                 mediante una Fianza al contrato principal pueda mejorarse la garantía del préstamo solicitado sin \
                 necesidad que la fianza este firmada por todos los integrantes del presente contrato.'
         texto_10_3=texto_10_3+aux1
         self._parrafos.append(Paragraph(texto_10_3, estilos['Justify']))
 
+
+    
+
     #Convenio y garantia personal
     def _garantias_cygp(self, numeral):       
         texto = f'<b><u>{numeral}</u>.- (GARANTIAS).- "El(la)(los) DEUDOR(A)(ES)"</b> garantiza(n) el fiel y estricto cumplimiento del \
             presente contrato y de todas las obligaciones señaladas, inherentes y emergentes al mismo de la \
         siguiente manera:' 
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
         texto_10_1 = '<b>10.1.</b> Con la generalidad de sus bienes, mercaderías, muebles e inmuebles, presentes descritas en el \
@@ -676,15 +660,15 @@
         self._parrafos.append(Paragraph(texto_10_1, estilos['Justify']))
         #Sacado 10.2 de convenio
         if(self.__contrato["convenio"]):
             asociacion=self.__contrato["convenio"][0]["sindicato"].upper() 
             convenio_con=self.__contrato["convenio"][0]["abreviatura"].upper()
             texto_10_2 =f' <b>10.2.</b> En forma señalada, con la garantía del(los) <b>DERECHO(S) DE LINEA</b> que posee(n) como \
                 propietario(s) en <b>{asociacion}</b>, y que \
-                pone a disposición de GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A. de \
+                pone a disposición de GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A. de \
                 acuerdo al Convenio Interinstitucional suscrito con <b>{convenio_con}</b>. Consiguientemente la(s) acción(es) de \
                 línea se constituye(n) en forma incondicional e irrestricta en garantía(s), dispuestas a hacerse líquidas \
                 para cubrir de forma total o parcial las obligaciones producto del presente contrato de <b>"El(la)(los) \
                 DEUDOR(A)(ES)"</b> con <b>"EL ACREEDOR"</b>, sin reserva, ni limitación alguna. Obligándose <b>"El(la)(los) \
                 DEUDOR(A)(ES)"</b> a mantener dicha(s) línea(s) libre(s) de multas y obligaciones con su sindicato o \
                 cualquier otra persona natural o jurídica.' 
             self._parrafos.append(Paragraph(texto_10_2, estilos['Justify']))
@@ -727,14 +711,19 @@
                 y cuenta con el acuerdo y consentimiento de éste(a).<br/>\
                 <b>"El(la)(los) DEUDOR(A)(ES)"</b> y/o <b>"El(la)(los) FIADOR(A)(ES) PERSONAL(ES)"</b> autoriza(n) que, \
                 mediante una Fianza al contrato principal pueda mejorarse la garantía del préstamo solicitado sin \
                 necesidad que la fianza este firmada por todos los integrantes del presente contrato.'
         texto_10_3=texto_10_3+aux1
         self._parrafos.append(Paragraph(texto_10_3, estilos['Justify']))
     
+
+
+
+
+
     def _supervision(self, numeral):
         texto = f'<b><u>{numeral}</u>.- (SUPERVISION Y VISITAS DE INSPECCION E INFORMACION).-  "EL \
             ACREEDOR"</b> tiene el más amplio derecho para supervisar, inspeccionar y constatar periódicamente,\
             por medio de sus propios inspectores o por delegados contratados, la veracidad de la información \
             proporcionada por <b>"El(la)(los) DEUDOR(A)(ES)"</b>. Las partes se obligan a facilitar todas y cada una de \
             las labores de supervisión, inspección o control que <b>"EL ACREEDOR"</b> estime por conveniente.'
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
@@ -747,22 +736,22 @@
             <b>"El(la)(los) DEUDOR(A)(ES)"</b>, limitando su accionar a comunicar dicha cesión al domicilio señalado en \
             la cláusula primera.'
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
     
     def _autorizacion(self, numeral):
         texto = f'<b><u>{numeral}</u>.- (AUTORIZACION DE INVESTIGACION DE ANTECEDENTES CREDITICIOS).- \
             "El(la)(los) DEUDOR(A)(ES)" y "El(la)(los) FIADOR(A)(ES) PERSONAL(ES)"</b>, autoriza(n) en forma \
-            expresa a GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A. a solicitar \
+            expresa a GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A. a solicitar \
             información sobre sus antecedentes crediticios y otras cuentas por pagar de carácter económico, \
             financiero y comercial registrados en el BI y la CIC de la Autoridad de Supervisión del Sistema \
             Financiero (ASFI), mientras dure su relación contractual con el citado usuario.<br/>\
             Asimismo, autoriza(n):'
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
         a = '<bullet></bullet> Incorporar los datos crediticios y de otras cuentas por pagar de carácter económico, financiero y \
-            comercial derivados de la relación con GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL \
+            comercial derivados de la relación con GESTION Y SOPORTE DE PROYECTOS JESUS DEL \
             GRAN PODER S.A., en la(s) base(s) de datos de propiedad de los Burós de Información que \
             cuenten con Licencia de Funcionamiento de ASFI y en la CIC.' 
         b = '<bullet></bullet> Al registro de sus datos crediticios en las bases de datos de INFOCENTER S.A, con licencia de \
             funcionamiento del Organismo de Supervisión, ASFI.' 
         incisos = ListFlowable(
         [
             Paragraph(a,estilos['Inciso']),
@@ -779,22 +768,22 @@
         )
         self._parrafos.append(incisos)
     
     #12
     def _autorizacion4(self, numeral):
         texto = f'<b><u>{numeral}</u>.- (AUTORIZACION DE INVESTIGACION DE ANTECEDENTES CREDITICIOS).- \
             "El(la)(los) DEUDOR(A)(ES)" y "El(la)(los) GARANTE(S) PERSONAL(ES)"</b>, autoriza(n) en forma \
-            expresa a GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A. a solicitar \
+            expresa a GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A. a solicitar \
             información sobre sus antecedentes crediticios y otras cuentas por pagar de carácter económico, \
             financiero y comercial registrados en el BI y la CIC de la Autoridad de Supervisión del Sistema \
             Financiero (ASFI), mientras dure su relación contractual con el citado usuario.<br/>\
             Asimismo, autoriza(n):'
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
         a = '<bullet></bullet> Incorporar los datos crediticios y de otras cuentas por pagar de carácter económico, financiero y \
-            comercial derivados de la relación con GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL \
+            comercial derivados de la relación con GESTION Y SOPORTE DE PROYECTOS JESUS DEL \
             GRAN PODER S.A., en la(s) base(s) de datos de propiedad de los Burós de Información que \
             cuenten con Licencia de Funcionamiento de ASFI y en la CIC.' 
         b = '<bullet></bullet> Al registro de sus datos crediticios en las bases de datos de INFOCENTER S.A, con licencia de \
             funcionamiento del Organismo de Supervisión, ASFI.' 
         incisos = ListFlowable(
         [
             Paragraph(a,estilos['Inciso']),
@@ -954,34 +943,31 @@
     #PRIMERA 2
     def nombreCompleto_repre(self):
         nombre = (self.__contrato["testimonio_poder"]["representante_legal"]["first_name"]+" "+self.__contrato["testimonio_poder"]["representante_legal"]["last_name"]).upper()
         return nombre
     
     def get_deudores(self):   
         deudores=self.__contrato["deudores"]     
-        if(len(deudores)>0):
-            deudores_ = [item for item in deudores if (item["tipo_obligado"]=="1A" or item["tipo_obligado"]=="4A" or item["tipo_obligado"]=="5A" or item["tipo_obligado"]=="1B")]
-            return deudores_
-        else:
-            raise ContratoError("Campo requerido", "El contrato requiere los dados del(los) Deudor(es)")
+        deudores_ = [item for item in deudores if (item["tipo_obligado"]=="1A" or item["tipo_obligado"]=="4A" or item["tipo_obligado"]=="5A" or item["tipo_obligado"]=="1B")]
+        return deudores_
     
     def get_estado_civil(self,_estado_civil, genero):
         #diccionario para comprobar
         estados_civiles = {"S": "solter","C": "casad","V": "viud","D": "divorciad", "N":"solter"}
         if(genero =="F"): 
             return estados_civiles.get(_estado_civil) +"a"
         else:
             return estados_civiles.get(_estado_civil) +"o"
 
     def get_articulo_direccion(self,direccion_dato):
         #diccionario para comprobar  
         direccion = direccion_dato.split(' ')
         direccion_uno= direccion[0].lower()
         articulo=""
-        if(direccion_uno =="avenida" or direccion_uno =="calle" or direccion_uno =="av." or direccion_uno =="av"): 
+        if(direccion_uno =="avenida" or direccion_uno =="calle" or direccion_uno =="av."): 
             articulo = "la "
         if(direccion_uno =="pasaje" or direccion_uno =="callejon" or direccion_uno =="psje." or direccion_uno =="pje."): 
             articulo = "el "
         
         return articulo + direccion_dato
         
     def _partes_contratantes2(self, numeral):
@@ -993,15 +979,15 @@
         cargo = testimonio_poder["representante_legal"]["rol"]       
         numero_testimonio = testimonio_poder["numero_testimonio"]
         fecha_testimonio = Utils.get_fecha(self, testimonio_poder["fecha_testimonio"])
         numero_notaria = testimonio_poder["numero_notaria_publica"]
         responsable_notaria = testimonio_poder["nombre_notario_publico"]
         texto = f'<b><u>{numeral}</u>.- (PARTES CONTRATANTES)</b>.- Intervienen en la suscripción del presente contrato:' 
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
-        a = f'<b>GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A.</b>, sociedad \
+        a = f'<b>GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.</b>, sociedad \
             legalmente constituida bajo las leyes del Estado Plurinacional de Bolivia, con Matrícula de \
             Comercio y Número de Identificación Tributaria 173788022, con domicilio en la \
             {domicilio_legal} de esta ciudad, representada legalmente por <b>{apoderado}</b>, con C.I. Nº {numero_ci_apoderado}, mayor de edad, hábil \
             por derecho y vecino(a) de esta ciudad, en su condición de {cargo} en mérito al \
             Testimonio Poder No. {numero_testimonio} de fecha {fecha_testimonio} otorgado por ante la \
             Notaría de Fe Pública Nº {numero_notaria} del Distrito Judicial de La Paz a cargo de(la) Dr(a).\
             {responsable_notaria}, quien en adelante se denominará <b>"EL ACREEDOR"</b>.'      
@@ -1053,15 +1039,15 @@
         cargo = testimonio_poder["representante_legal"]["rol"]       
         numero_testimonio = testimonio_poder["numero_testimonio"]
         fecha_testimonio = Utils.get_fecha(self, testimonio_poder["fecha_testimonio"])
         numero_notaria = testimonio_poder["numero_notaria_publica"]
         responsable_notaria = testimonio_poder["nombre_notario_publico"]
         texto = f'<b><u>{numeral}</u>.- (PARTES CONTRATANTES)</b>.- Intervienen en la suscripción del presente contrato:' 
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
-        a = f'<b>GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A.</b>, sociedad \
+        a = f'<b>GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.</b>, sociedad \
             legalmente constituida bajo las leyes del Estado Plurinacional de Bolivia, con Matrícula de \
             Comercio y Número de Identificación Tributaria 173788022, con domicilio en la \
             {domicilio_legal} de esta ciudad, representada legalmente por <b>{apoderado}</b>, con C.I. Nº {numero_ci_apoderado}, mayor de edad, hábil \
             por derecho y vecino(a) de esta ciudad, en su condición de {cargo} en mérito al \
             Testimonio Poder No. {numero_testimonio} de fecha {fecha_testimonio} otorgado por ante la \
             Notaría de Fe Pública Nº {numero_notaria} del Distrito Judicial de La Paz a cargo de(la) Dr(a).\
             {responsable_notaria}, quien en adelante se denominará <b>"EL ACREEDOR"</b>.'      
@@ -1098,15 +1084,15 @@
             bulletFontName='Helvetica-Bold',
             bulletFontSize=9.1,
             bulletOffsetY=0,
             bulletDedent=20        
             )
             self._parrafos.append(incisos)
         else:
-            raise ContratoError("Campo requerido", "Este tipo de garantia: Solidario, Requiere 3 deudores minimamente")
+            raise ContratoError("Campo requerido", "Requiere Solidario 3 deudores minimamente")
     #CUARTA 2
     def _gestion_cobranza2(self, numeral):
         texto_gestion = f'<b><u>{numeral}</u>.- (GESTIONES DE COBRANZA)</b>.- Las partes acuerdan que los Gastos Operativos que \
         genere las Gestiones de Cobranza "in situ", serán cubiertas por <b>"El(la)(los) DEUDOR(A)(ES)"</b>, éste \
         acuerdo es pactado y autorizado de forma voluntaria y expresa por <b>"El(la)(los) DEUDOR(A)(ES)"</b>.'
         self._parrafos.append(Paragraph(texto_gestion, estilos['Justify']))
     
@@ -1278,15 +1264,15 @@
         # LA API(http://192.168.100.5:8000/api/v1/contratos/501231701701/) DEVUEVE UN DICCIONAIO PERO EN EL ADMI SE 
         # ALMACENA COMO UNA ARRAY, SE AJUSTO A LO QUE SE TIENE EN EL ADMI
         if(self.__contrato["convenio"]):
             asociacion=self.__contrato["convenio"][0]["sindicato"].upper() 
             convenio_con=self.__contrato["convenio"][0]["abreviatura"].upper()
             texto_10_2 =f' <b>10.2.</b> En forma señalada, con la garantía del(los) <b>DERECHO(S) DE LINEA</b> que posee(n) como \
                 propietario(s) en <b>{asociacion}</b>, y que \
-                pone a disposición de GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A. de \
+                pone a disposición de GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A. de \
                 acuerdo al Convenio Interinstitucional suscrito con <b>{convenio_con}</b>. Consiguientemente la(s) acción(es) de \
                 línea se constituye(n) en forma incondicional e irrestricta en garantía(s), dispuestas a hacerse líquidas \
                 para cubrir de forma total o parcial las obligaciones producto del presente contrato de <b>"El(la)(los) \
                 DEUDOR(A)(ES)"</b> con <b>"EL ACREEDOR"</b>, sin reserva, ni limitación alguna. Obligándose <b>"El(la)(los) \
                 DEUDOR(A)(ES)"</b> a mantener dicha(s) línea(s) libre(s) de multas y obligaciones con su sindicato o \
                 cualquier otra persona natural o jurídica.<br/>\
                 Queda establecido que mientras no se haga efectivo el pago total y definitivo de la deuda y demás \
@@ -1307,15 +1293,15 @@
             sw=False
             for item in garantias:
                 if(item['concepto']=="Matricula" or item['concepto']=="Partida"):
                     concepto=item['concepto']
                     matricula=item['detalle_garantia']  
                     sw=True
             if(sw==False):
-                raise ContratoError("Campo requerido", "El contrato requiere los Datos de garantias reales por Concepto: Matricula")
+                raise ContratoError("Campo requerido", "El contrato requiere los Datos de concepto de garantias reales")
             return concepto+" "+matricula
         else:
             raise ContratoError("Campo requerido", "El contrato requiere los Datos de garantias reales")
         
     # DECIMO 3 (solo hasta el 10.3)
     def _garantias3(self, numeral):
         texto = f'<b><u>{numeral}</u>.- (GARANTIAS).- "El(la)(los) DEUDOR(A)(ES)"</b> garantiza(n) el fiel y estricto cumplimiento del \
@@ -1330,15 +1316,15 @@
             SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.'
         self._parrafos.append(Paragraph(texto_10_1, estilos['Justify']))
         if(self.__contrato["convenio"]):
             asociacion=self.__contrato["convenio"][0]["sindicato"].upper()
             convenio_con=self.__contrato["convenio"][0]["abreviatura"].upper()
             texto_10_2 = f' <b>10.2.</b> En forma señalada, con la garantía del(los) <b>DERECHO(S) DE LINEA</b> que posee(n) como \
                 propietario(s) en <b>{asociacion}</b>, y que \
-                pone a disposición de GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A. de \
+                pone a disposición de GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A. de \
                 acuerdo al Convenio Interinstitucional suscrito con <b>{convenio_con}</b>. Consiguientemente la(s) acción(es) de \
                 línea se constituye(n) en forma incondicional e irrestricta en garantía(s), dispuestas a hacerse líquidas \
                 para cubrir de forma total o parcial las obligaciones producto del presente contrato de <b>"El(la)(los) \
                 DEUDOR(A)(ES)"</b> con <b>"EL ACREEDOR"</b>, sin reserva, ni limitación alguna. Obligándose <b>"El(la)(los) \
                 DEUDOR(A)(ES)"</b> a mantener dicha(s) línea(s) libre(s) de multas y obligaciones con su sindicato o \
                 cualquier otra persona natural o jurídica' 
             self._parrafos.append(Paragraph(texto_10_2, estilos['Justify']))
@@ -1348,16 +1334,14 @@
         
         matricula=self.get_matricula()
         texto_10_3 =f' <b>10.3.</b> En especial y en forma señalada, con la(s) garantía(s) de <b>DOCUMENTOS EN CUSTODIA DE \
             INMUEBLE</b>  registrado en DD.RR. bajo la <b>{matricula}</b>, bajo el siguiente detalle: ' 
         self._parrafos.append(Paragraph(texto_10_3, estilos['Justify']))
         #jalo al json
         datos_garantias = self.__contrato["garantias_reales"]=self.filtrar_datos()
-        self._parrafos.append(Spacer(0, 8))
-
         P0 = Paragraph('''
             <b>Nº</b>''')
         P1 = Paragraph('''
             <b>DETALLE DEL DOCUMENTO</b>''')
         P2 = Paragraph('''
             <b>FOJAS</b>''')
         t = Table([
@@ -1365,16 +1349,14 @@
         colWidths=[30,230,86], rowHeights=None
         )
         t.setStyle([
             ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
             ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
             ('ALIGN',(0,-1),(-1,-1),'CENTER'),
             ('VALIGN',(0,-1),(-1,-1),'MIDDLE'),
-            ('BOTTOMPADDING',(0,0),(-1,-1),1),
-            ('TOPPADDING',(0,0),(-1,-1),1),
         ])
         self._parrafos.append(t)
         estilo = getSampleStyleSheet()
         P1 = Paragraph('''El tux templario''', estilo["BodyText"])
         i=0
         t = Table(
             data=[                
@@ -1386,22 +1368,20 @@
                 #para modificar el ancho de las columnas
             ], 
             colWidths=[30,230,86], rowHeights=None           
         )
         t.setStyle([
             ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
             ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
-            ('VALIGN', (0,0), (-1, -1), 'TOP'),    
-            ('BOTTOMPADDING',(0,0),(-1,-1),0),
-            ('TOPPADDING',(0,0),(-1,-1),0),         
+            ('VALIGN', (0,0), (-1, -1), 'TOP'),            
         ])
         self._parrafos.append(t)
         linea=Table(data=[''],colWidths=12.2*cm,rowHeights=0.02*cm,style=[('LINEABOVE',(0, 0), (-1, 0),1,colors.black)])
         self._parrafos.append(linea)
-        self._parrafos.append(Spacer(0, 8))
+        self._parrafos.append(Spacer(0, 10))
         texto_10_3_continue ='Documentos originales de propiedad de <b>"El(la)(los) DEUDOR(A)(ES)"</b> y depositados en las oficinas de <b>"EL \
             ACREEDOR"</b> bajo libre y espontánea voluntad y sin presión alguna por parte del(la)(los) propietario(a)(s).<br/> \
             Consiguientemente los Documentos del Inmueble se constituye(n) en forma incondicional e irrestricta en \
             garantía(s), dispuesta(s) a hacerse liquida para cubrir de forma total o parcial las obligaciones producto del \
             presente contrato de <b>"El(la)(los) DEUDOR(A)(ES)"</b> con <b>"EL ACREEDOR"</b>, sin reserva, ni limitación alguna.<br/> \
             Queda establecido que mientras no se haga efectivo el pago total y definitivo de la deuda y demás \
             obligaciones asumidas por <b>"El(la)(los) DEUDOR(A)(ES)"</b> en el presente contrato, ninguna causa extinguirá \
@@ -1426,15 +1406,15 @@
             SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.'
         self._parrafos.append(Paragraph(texto_10_1, estilos['Justify']))
         if(self.__contrato["convenio"]):
             asociacion=self.__contrato["convenio"][0]["sindicato"].upper()
             convenio_con=self.__contrato["convenio"][0]["abreviatura"].upper()
             texto_10_2 = f' <b>10.2.</b> En forma señalada, con la garantía del(los) <b>DERECHO(S) DE LINEA</b> que posee(n) como \
                 propietario(s) en <b>{asociacion}</b>, y que \
-                pone a disposición de GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A. de \
+                pone a disposición de GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A. de \
                 acuerdo al Convenio Interinstitucional suscrito con <b>{convenio_con}</b>. Consiguientemente la(s) acción(es) de \
                 línea se constituye(n) en forma incondicional e irrestricta en garantía(s), dispuestas a hacerse líquidas \
                 para cubrir de forma total o parcial las obligaciones producto del presente contrato de <b>"El(la)(los) \
                 DEUDOR(A)(ES)"</b> con <b>"EL ACREEDOR"</b>, sin reserva, ni limitación alguna. Obligándose <b>"El(la)(los) \
                 DEUDOR(A)(ES)"</b> a mantener dicha(s) línea(s) libre(s) de multas y obligaciones con su sindicato o \
                 cualquier otra persona natural o jurídica'
             self._parrafos.append(Paragraph(texto_10_2, estilos['Justify']))
@@ -1442,15 +1422,14 @@
             raise ContratoError("Campo requerido", "El contrato requiere los Datos de Convenio")
         placa=self.get_placa()
         texto_10_3 =f' <b>10.3.</b> En especial y en forma señalada, con la(s) garantía(s) de <b>DOCUMENTOS EN CUSTODIA DEL \
             VEHICULO</b> con <b>{placa}</b>, bajo el siguiente detalle: ' 
         self._parrafos.append(Paragraph(texto_10_3, estilos['Justify']))
         #tabla; jalo al json
         datos_garantias = self.__contrato["garantias_reales"]=self.filtrar_datos()
-        self._parrafos.append(Spacer(0, 8))
         P0 = Paragraph('''
             <b>Nº</b>''')
         P1 = Paragraph('''
             <b>DETALLE DEL DOCUMENTO</b>''')
         P2 = Paragraph('''
             <b>FOJAS</b>''')
         t = Table([
@@ -1458,16 +1437,14 @@
         colWidths=[30,230,86], rowHeights=None
         )
         t.setStyle([
             ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
             ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
             ('ALIGN',(0,-1),(-1,-1),'CENTER'),
             ('VALIGN',(0,-1),(-1,-1),'MIDDLE'),
-            ('BOTTOMPADDING',(0,0),(-1,-1),1),
-            ('TOPPADDING',(0,0),(-1,-1),1),
         ])
         self._parrafos.append(t)
         estilo = getSampleStyleSheet()
         P1 = Paragraph('''El tux templario''', estilo["BodyText"])
         i=0
         t = Table(
             data=[                
@@ -1479,22 +1456,20 @@
                 #para modificar el ancho de las columnas
             ], 
             colWidths=[30,230,86], rowHeights=None           
         )
         t.setStyle([
             ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
             ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
-            ('VALIGN', (0,0), (-1, -1), 'TOP'),  
-            ('BOTTOMPADDING',(0,0),(-1,-1),0),
-            ('TOPPADDING',(0,0),(-1,-1),0),           
+            ('VALIGN', (0,0), (-1, -1), 'TOP'),            
         ])
         self._parrafos.append(t)
         linea=Table(data=[''],colWidths=12.2*cm,rowHeights=0.02*cm,style=[('LINEABOVE',(0, 0), (-1, 0),1,colors.black)])
         self._parrafos.append(linea)
-        self._parrafos.append(Spacer(0, 8))
+        self._parrafos.append(Spacer(0, 10))
         texto_10_3_continue ='<br/>Documentos originales de propiedad de <b>"El(la)(los) DEUDOR(A)(ES)"</b> y depositados en las oficinas de <b>"EL \
             ACREEDOR"</b> bajo libre y espontánea voluntad y sin presión alguna por parte del(la)(los) propietario(a)(s).<br/>\
             Consiguientemente los Documentos del Vehiculo se constituye(n) en forma incondicional e irrestricta en \
             garantía(s), dispuesta(s) a hacerse liquida para cubrir de forma total o parcial las obligaciones producto del \
             presente contrato de <b>"El(la)(los) DEUDOR(A)(ES)"</b> con <b>"EL ACREEDOR"</b>, sin reserva, ni limitación alguna.<br/> \
             Queda establecido que mientras no se haga efectivo el pago total y definitivo de la deuda y demás \
             obligaciones asumidas por <b>"El(la)(los) DEUDOR(A)(ES)"</b> en el presente contrato, ninguna causa extinguirá \
@@ -1549,21 +1524,20 @@
         texto_10_1 = '<b>10.1.</b> Con la generalidad de sus bienes, mercaderías, muebles e inmuebles, presentes descritas en el \
             formulario "Declaración Patrimonial" que forma parte íntegra del presente contrato sin necesidad de ser \
             transcrito, bienes, mercaderías, muebles e inmuebles, futuros sin exclusión ni limitación alguna. <b>"El(la)(los) \
             DEUDOR(A)(ES)"</b> se obliga(n) a no vender, ceder, transferir, etc., bajo ningún título los bienes \
             descritos en el formulario de Declaración Patrimonial, mientras perdure la obligación con GESTION Y \
             SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.'
         self._parrafos.append(Paragraph(texto_10_1, estilos['Justify']))
-
+        #eliminado matricula
         texto_10_3 =f' <b>10.2.</b> En especial y en forma señalada, con la(s) garantía(s) de <b>OTROS DOCUMENTOS EN CUSTODIA</b> \
             registrado(s) bajo el siguiente detalle: '
         self._parrafos.append(Paragraph(texto_10_3, estilos['Justify']))
+        #jalo al json
         datos_garantias = self.__contrato["garantias_reales"]=self.filtrar_datos()
-        self._parrafos.append(Spacer(0, 8))
-
         if(len(datos_garantias)>0):
             P0 = Paragraph('''
                 <b>Nº</b>''')
             P1 = Paragraph('''
                 <b>DETALLE DEL DOCUMENTO</b>''')
             P2 = Paragraph('''
                 <b>FOJAS</b>''')
@@ -1572,16 +1546,14 @@
             colWidths=[30,230,86], rowHeights=None
             )
             t.setStyle([
                 ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
                 ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
                 ('ALIGN',(0,-1),(-1,-1),'CENTER'),
                 ('VALIGN',(0,-1),(-1,-1),'MIDDLE'),
-                ('BOTTOMPADDING',(0,0),(-1,-1),1),
-                ('TOPPADDING',(0,0),(-1,-1),1),
             ])
             self._parrafos.append(t)
             estilo = getSampleStyleSheet()
             P1 = Paragraph('''El tux templario''', estilo["BodyText"])
             i=0
             t = Table(
                 data=[                
@@ -1593,25 +1565,23 @@
                     #para modificar el ancho de las columnas
                 ], 
                 colWidths=[30,230,86], rowHeights=None           
             )
             t.setStyle([
                 ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
                 ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
-                ('VALIGN', (0,0), (-1, -1), 'TOP'),  
-                ('BOTTOMPADDING',(0,0),(-1,-1),0),
-                ('TOPPADDING',(0,0),(-1,-1),0),           
+                ('VALIGN', (0,0), (-1, -1), 'TOP'),            
             ])
             self._parrafos.append(t)
             linea=Table(data=[''],colWidths=12.2*cm,rowHeights=0.02*cm,style=[('LINEABOVE',(0, 0), (-1, 0),1,colors.black)])
             self._parrafos.append(linea)
-                        
+            self._parrafos.append(Spacer(0, 10))
         else:
                 raise ContratoError("Campo requerido", "El contrato requiere los Datos de garantias reales")
-        self._parrafos.append(Spacer(0, 8))
+
         texto_10_3_continue ='Documentos originales de propiedad de <b>"El(la)(los) DEUDOR(A)(ES)"</b> y depositados en las oficinas de <b>"EL \
             ACREEDOR"</b> bajo libre y espontánea voluntad y sin presión alguna por parte del(la)(los) propietario(a)(s).<br/>\
             Consiguientemente los Documentos del Inmueble se constituye(n) en forma incondicional e irrestricta en \
             garantía(s), dispuesta(s) a hacerse liquida para cubrir de forma total o parcial las obligaciones producto del \
             presente contrato de <b>"El(la)(los) DEUDOR(A)(ES)"</b> con <b>"EL ACREEDOR"</b>, sin reserva, ni limitación alguna.<br/>\
             Queda establecido que mientras no se haga efectivo el pago total y definitivo de la deuda y demás \
             obligaciones asumidas por <b>"El(la)(los) DEUDOR(A)(ES)"</b> en el presente contrato, ninguna causa extinguirá \
@@ -1636,15 +1606,14 @@
         self._parrafos.append(Paragraph(texto_10_1, estilos['Justify']))
         matricula=self.get_matricula()
         texto_10_3 =f' <b>10.2.</b> En especial y en forma señalada, con la(s) garantía(s) de <b>DOCUMENTOS EN CUSTODIA DE \
             INMUEBLE</b>  registrado en DD.RR. bajo la <b>{matricula}</b> bajo el siguiente detalle: '
         self._parrafos.append(Paragraph(texto_10_3, estilos['Justify']))
         #jalo al json
         datos_garantias = self.__contrato["garantias_reales"]=self.filtrar_datos()
-        self._parrafos.append(Spacer(0, 8))
         
         P0 = Paragraph('''
             <b>Nº</b>''')
         P1 = Paragraph('''
             <b>DETALLE DEL DOCUMENTO</b>''')
         P2 = Paragraph('''
             <b>FOJAS</b>''')
@@ -1653,16 +1622,14 @@
         colWidths=[30,230,86], rowHeights=None
         )
         t.setStyle([
             ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
             ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
             ('ALIGN',(0,-1),(-1,-1),'CENTER'),
             ('VALIGN',(0,-1),(-1,-1),'MIDDLE'),
-            ('BOTTOMPADDING',(0,0),(-1,-1),1),
-            ('TOPPADDING',(0,0),(-1,-1),1),
         ])
         self._parrafos.append(t)
         estilo = getSampleStyleSheet()
         P1 = Paragraph('''El tux templario''', estilo["BodyText"])
         i=0
         t = Table(
             data=[                
@@ -1674,22 +1641,21 @@
                 #para modificar el ancho de las columnas
             ], 
             colWidths=[30,230,86], rowHeights=None           
         )
         t.setStyle([
             ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
             ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
-            ('VALIGN', (0,0), (-1, -1), 'TOP'),     
-            ('BOTTOMPADDING',(0,0),(-1,-1),0),
-            ('TOPPADDING',(0,0),(-1,-1),0),        
+            ('VALIGN', (0,0), (-1, -1), 'TOP'),            
         ])
         self._parrafos.append(t)
         linea=Table(data=[''],colWidths=12.2*cm,rowHeights=0.02*cm,style=[('LINEABOVE',(0, 0), (-1, 0),1,colors.black)])
         self._parrafos.append(linea)
-        self._parrafos.append(Spacer(0, 8))
+        self._parrafos.append(Spacer(0, 10))
+        
         texto_10_3_continue ='Documentos originales de propiedad de <b>"El(la)(los) DEUDOR(A)(ES)"</b> y depositados en las oficinas de <b>"EL \
             ACREEDOR"</b> bajo libre y espontánea voluntad y sin presión alguna por parte del(la)(los) propietario(a)(s).<br/>\
             Consiguientemente los Documentos del Inmueble se constituye(n) en forma incondicional e irrestricta en \
             garantía(s), dispuesta(s) a hacerse liquida para cubrir de forma total o parcial las obligaciones producto del \
             presente contrato de <b>"El(la)(los) DEUDOR(A)(ES)"</b> con <b>"EL ACREEDOR"</b>, sin reserva, ni limitación alguna.<br/> \
             Queda establecido que mientras no se haga efectivo el pago total y definitivo de la deuda y demás \
             obligaciones asumidas por <b>"El(la)(los) DEUDOR(A)(ES)"</b> en el presente contrato, ninguna causa extinguirá \
@@ -1766,16 +1732,14 @@
 
         placa=self.get_placa()
         texto_10_3 =f' <b>10.3.</b> Y en especial y en forma señalada, con la(s) garantía(s) de <b>DOCUMENTOS EN CUSTODIA DEL \
         VEHICULO</b> con <b>"{placa}</b> y bajo el siguiente detalle: ' 
         self._parrafos.append(Paragraph(texto_10_3, estilos['Justify']))
         #jalo al json
         datos_garantias = self.__contrato["garantias_reales"]=self.filtrar_datos()
-        self._parrafos.append(Spacer(0, 8))
-
         P0 = Paragraph('''
             <b>Nº</b>''')
         P1 = Paragraph('''
             <b>DETALLE DEL DOCUMENTO</b>''')
         P2 = Paragraph('''
             <b>FOJAS</b>''')
         t = Table([
@@ -1783,16 +1747,14 @@
         colWidths=[30,230,86], rowHeights=None
         )
         t.setStyle([
             ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
             ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
             ('ALIGN',(0,-1),(-1,-1),'CENTER'),
             ('VALIGN',(0,-1),(-1,-1),'MIDDLE'),
-            ('BOTTOMPADDING',(0,0),(-1,-1),1),
-            ('TOPPADDING',(0,0),(-1,-1),1),
         ])
         self._parrafos.append(t)
         estilo = getSampleStyleSheet()
         P1 = Paragraph('''El tux templario''', estilo["BodyText"])
         i=0
         t = Table(
             data=[                
@@ -1804,22 +1766,20 @@
                 #para modificar el ancho de las columnas
             ], 
             colWidths=[30,230,86], rowHeights=None           
         )
         t.setStyle([
             ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
             ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
-            ('VALIGN', (0,0), (-1, -1), 'TOP'), 
-            ('BOTTOMPADDING',(0,0),(-1,-1),0),
-            ('TOPPADDING',(0,0),(-1,-1),0),            
+            ('VALIGN', (0,0), (-1, -1), 'TOP'),            
         ])
         self._parrafos.append(t)
         linea=Table(data=[''],colWidths=12.2*cm,rowHeights=0.02*cm,style=[('LINEABOVE',(0, 0), (-1, 0),1,colors.black)])
         self._parrafos.append(linea)
-        self._parrafos.append(Spacer(0, 8))
+        self._parrafos.append(Spacer(0, 10))
         texto_10_3_continue ='Documentos originales de propiedad de <b>"El(la)(los) DEUDOR(A)(ES)"</b> y depositados en las oficinas de <b>"EL \
         ACREEDOR"</b> bajo libre y espontánea voluntad y sin presión alguna por parte del(la)(los) propietario(a)(s).<br/>\
         Consiguientemente los Documentos del Inmueble se constituye(n) en forma incondicional e irrestricta en \
         garantía(s), dispuesta(s) a hacerse liquida para cubrir de forma total o parcial las obligaciones producto del \
         presente contrato de <b>"El(la)(los) DEUDOR(A)(ES)"</b> con <b>"EL ACREEDOR"</b>, sin reserva, ni limitación alguna.<br/>\
         Queda establecido que mientras no se haga efectivo el pago total y definitivo de la deuda y demás \
         obligaciones asumidas por <b>"El(la)(los) DEUDOR(A)(ES)"</b> en el presente contrato, ninguna causa extinguirá \
@@ -1836,15 +1796,15 @@
             sw=False
             for item in datos_garantias:
                 if(item['concepto']=="Placa"):
                     concepto=item['concepto']
                     placa=item['detalle_garantia']   
                     sw=True
             if(sw==False):
-                raise ContratoError("Campo requerido", "El contrato requiere los Datos de garantias reales por Concepto: Placa")
+                raise ContratoError("Campo requerido", "El contrato requiere los Datos de concepto de garantias reales")
             return concepto+" Nº "+placa
         else:
             raise ContratoError("Campo requerido", "El contrato requiere los Datos de garantias reales")
             
     #NUEVA FUNCION ELIMINA PLACA
     def filtrar_datos(self):  
         # Eliminar la garantía con el concepto "Placa" del conjunto de garantías reales
@@ -1869,17 +1829,17 @@
             descritos en el formulario de Declaración Patrimonial, mientras perdure la obligación con GESTION Y \
             SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.'
         self._parrafos.append(Paragraph(texto_10_1, estilos['Justify']))
         placa=self.get_placa()
         texto_10_2 =f' <b>10.2.</b> En especial y en forma señalada, con la(s) garantía(s) de <b>DOCUMENTOS EN CUSTODIA DEL \
             VEHÍCULO</b> con <b>{placa}</b>, bajo el siguiente detalle: ' 
         self._parrafos.append(Paragraph(texto_10_2, estilos['Justify']))
-        datos_garantias = self.__contrato["garantias_reales"]=self.filtrar_datos()
-        self._parrafos.append(Spacer(0, 8))
 
+        datos_garantias = self.__contrato["garantias_reales"]=self.filtrar_datos()
+        
         P0 = Paragraph('''
             <b>Nº</b>''')
         P1 = Paragraph('''
             <b>DETALLE DEL DOCUMENTO</b>''')
         P2 = Paragraph('''
             <b>FOJAS</b>''')
         t = Table([
@@ -1887,40 +1847,39 @@
         colWidths=[30,230,86], rowHeights=None
         )
         t.setStyle([
             ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
             ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
             ('ALIGN',(0,-1),(-1,-1),'CENTER'),
             ('VALIGN',(0,-1),(-1,-1),'MIDDLE'),
-            ('BOTTOMPADDING',(0,0),(-1,-1),1),
-            ('TOPPADDING',(0,0),(-1,-1),1),
         ])
         self._parrafos.append(t)
+        estilo = getSampleStyleSheet()
+        P1 = Paragraph('''El tux templario''', estilo["BodyText"])
+        i=0
         t = Table(
             data=[                
                 (
                     str(i)+".",                    
                     Paragraph(items["concepto"].upper()+" "+items["detalle_garantia"].upper(),estilos["left"]),
                     Paragraph(items["fojas"],estilos["left"])
                 ) for i,items in enumerate(datos_garantias,1)
                 #para modificar el ancho de las columnas
             ], 
             colWidths=[30,230,86], rowHeights=None          
         )
         t.setStyle([
             ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
             ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
-            ('VALIGN', (0,0), (-1, -1), 'TOP'),   
-            ('BOTTOMPADDING',(0,0),(-1,-1),0),
-            ('TOPPADDING',(0,0),(-1,-1),0),         
+            ('VALIGN', (0,0), (-1, -1), 'TOP'),            
         ])
         self._parrafos.append(t)
         linea=Table(data=[''],colWidths=12.2*cm,rowHeights=0.02*cm,style=[('LINEABOVE',(0, 0), (-1, 0),1,colors.black)])
         self._parrafos.append(linea)
-        self._parrafos.append(Spacer(0, 8))
+        self._parrafos.append(Spacer(0, 10))
         texto_10_2_continue ='Documentos originales de propiedad de <b>"El(la)(los) DEUDOR(A)(ES)"</b> y depositados en las oficinas de <b>"EL \
         ACREEDOR"</b> bajo libre y espontánea voluntad y sin presión alguna por parte del(la)(los) propietario(a)(s).<br/>\
         Consiguientemente los Documentos del Vehículo se constituye(n) en forma incondicional e irrestricta en \
         garantía(s), dispuesta(s) a hacerse liquida para cubrir de forma total o parcial las obligaciones producto del \
         presente contrato de <b>"El(la)(los) DEUDOR(A)(ES)"</b> con <b>"EL ACREEDOR"</b>, sin reserva, ni limitación alguna.<br/>\
         Queda establecido que mientras no se haga efectivo el pago total y definitivo de la deuda y demás \
         obligaciones asumidas por <b>"El(la)(los) DEUDOR(A)(ES)"</b> en el presente contrato, ninguna causa extinguirá \
@@ -1997,22 +1956,22 @@
             así como a no constituir sobre el(los) mismo(s) ningún otro derecho especial a favor de terceras personales naturales o jurídicas, sin la expresa autorización escrita de <b>“EL \
             ACREEDOR"</b>.'
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
     
     #DÉCIMA TERCERA 2 
     def _autorizacion2(self, numeral):
         texto = f'<b><u>{numeral}</u>.- (AUTORIZACION DE INVESTIGACION DE ANTECEDENTES CREDITICIOS).- "El(la)(los) \
-            DEUDOR(A)(ES)"</b> autoriza(n) en forma expresa a GESTIÓN Y SOPORTE DE PROYECTOS JESÚS \
+            DEUDOR(A)(ES)"</b> autoriza(n) en forma expresa a GESTION Y SOPORTE DE PROYECTOS JESUS \
             DEL GRAN PODER S.A. a solicitar información sobre sus antecedentes crediticios y otras cuentas por pagar \
             de carácter económico, financiero y comercial registrados en el BI y la CIC de la Autoridad de Supervisión \
             del Sistema Financiero (ASFI), mientras dure su relación contractual con el citado usuario.<br/>\
             Asimismo, autoriza(n):'
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
         a = 'Incorporar los datos crediticios y de otras cuentas por pagar de carácter económico, financiero y \
-            comercial derivados de la relación con GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL \
+            comercial derivados de la relación con GESTION Y SOPORTE DE PROYECTOS JESUS DEL \
             GRAN PODER S.A., en la(s) base(s) de datos de propiedad de los Burós de Información que \
             cuenten con Licencia de Funcionamiento de ASFI y en la CIC.' 
         b = 'Al registro de sus datos crediticios en las bases de datos de INFOCENTER S.A, con licencia de \
             funcionamiento del Organismo de Supervisión, ASFI.' 
         incisos = ListFlowable(
         [
             Paragraph(a, estilos['Inciso']),
@@ -2028,22 +1987,22 @@
         bulletDedent=20        
         )
         self._parrafos.append(incisos)
     
     #DÉCIMA TERCERA 3'''Personal y Documentos en Custodia de Vehículo'''
     def _autorizacion3(self, numeral):
         texto = f'<b><u>{numeral}</u>.- (AUTORIZACION DE INVESTIGACION DE ANTECEDENTES CREDITICIOS).- "El(la) \
-            (los) DEUDOR(A)(ES)"</b> y <b>"El(la)(los) FIADOR(A)(ES) PERSONAL(ES)"</b>, autoriza(n) en forma expresa a GESTIÓN Y SOPORTE DE PROYECTOS JESÚS \
+            (los) DEUDOR(A)(ES)"</b> y <b>"El(la)(los) FIADOR(A)(ES) PERSONAL(ES)"</b>, autoriza(n) en forma expresa a GESTION Y SOPORTE DE PROYECTOS JESUS \
             DEL GRAN PODER S.A. a solicitar información sobre sus antecedentes crediticios y otras cuentas por pagar \
             de carácter económico, financiero y comercial registrados en el BI y la CIC de la Autoridad de Supervisión \
             del Sistema Financiero (ASFI), mientras dure su relación contractual con el citado usuario.<br/>\
             Asimismo, autoriza(n):'
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
         a = 'Incorporar los datos crediticios y de otras cuentas por pagar de carácter económico, financiero y \
-            comercial derivados de la relación con GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL \
+            comercial derivados de la relación con GESTION Y SOPORTE DE PROYECTOS JESUS DEL \
             GRAN PODER S.A., en la(s) base(s) de datos de propiedad de los Burós de Información que \
             cuenten con Licencia de Funcionamiento de ASFI y en la CIC.' 
         b = 'Al registro de sus datos crediticios en las bases de datos de INFOCENTER S.A, con licencia de \
             funcionamiento del Organismo de Supervisión, ASFI.' 
         incisos = ListFlowable(
         [
             Paragraph(a, estilos['Inciso']),
@@ -2090,119 +2049,88 @@
     def get_fiadores(self):   
         deudores = self.__contrato["deudores"]     
         fiadores = [item for item in deudores if item['tipo_obligado']=='2A']
         return fiadores
     
     # FIRMAS
     def _firmas(self):
-        tipo_garantia=self.__contrato["tipo_garantia"]["descripcion"]
-        print()
-        print("!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!111")
-        print(tipo_garantia) 
         fiadores= self.get_fiadores()
-        deudores= self.get_deudores()    
+        deudores= self.get_deudores()
         self._parrafos.append(Spacer(0,15))
-        # Modi para Prendaria y Personal
-        if(tipo_garantia=="Prendaria y Personal" and (len(fiadores)+len(deudores)!=5)):
-            a=self._parrafos.append
-            a(PageBreak())
-        # Modi para Prendaria y Personal
-        if(tipo_garantia=="Personal y  Doc. custodia Vehiculo"):
-            a=self._parrafos.append
-            a(PageBreak())
-        # Doc. Custodia de Vehiculo    y    Convenio y Doc. Custodia Inmueble    y    Convenio y Doc. Custodia Vehiculo
-        if((tipo_garantia=="Doc. Custodia de Vehiculo" and  len(deudores)>4) or (tipo_garantia=="Convenio y Doc. Custodia Inmueble" and  len(deudores)>4) or (tipo_garantia=="Convenio y Doc. Custodia Vehiculo" and  len(deudores)>4)):
-            a=self._parrafos.append
-            a(PageBreak())
-        # Personal    y    Convenio y Garantia personal 
-        if(tipo_garantia=="Convenio y Garantia personal" and len(deudores)>2):
-            a=self._parrafos.append
-            a(PageBreak())
-        
-        # Doc. Custodia de Vehiculo    y    Convenio y Doc. Custodia Inmueble   y    Convenio y Doc. Custodia Vehiculo
         texto= ('POR SI, COMO DEUDOR(A)(ES) o PRESTATARIO(A)(S):')
         self._parrafos.append(Paragraph(texto,style = estilos["Justify"]))        
         self._posicion_firmas(deudores)
         self._parrafos.append(Spacer(0,0.5*cm))
-        sw_personal=0
-        # Personal
-        if((tipo_garantia == "Personal" and len(deudores)==2) or (tipo_garantia == "Personal" and len(fiadores)==2)):
-            sw_personal=1
-        if((tipo_garantia == "Personal" and len(deudores)>2)):
-            sw_personal=2
-        # Personal
-        
-        if((tipo_garantia=="Convenio y Garantia personal" and len(deudores)<=2)):
-            a=self._parrafos.append
-            a(PageBreak())
-            
         if (len(fiadores) > 0):
-            # Personal    y    Convenio y Garantia personal 
-            if(sw_personal==2):
-                a=self._parrafos.append
-                a(PageBreak())
-            # Personal    y    Convenio y Garantia personal 
-            if(tipo_garantia=="Prendaria y Personal"):
-                texto= ('Y COMO DEPOSITARIO(S) Y/O GARANTE(S) SOLIDARIO(A)(S), MANCOMUNADO(A)(S) E INDIVISIBLE(S): ')
-            if(tipo_garantia!="Prendaria y Personal"):
-                texto= ('Y COMO FIADOR(A)(ES) SOLIDARIO(A)(S), MANCOMUNADO(A)(S) E INDIVISIBLE(S): ')
+            self._parrafos.append(Spacer(0,1))
+            texto= ('Y COMO FIADOR(A)(ES) SOLIDARIO(A)(S), MANCOMUNADO(A)(S) E INDIVISIBLE(S): ')
             self._parrafos.append(Paragraph(texto,style = estilos["Justify"]))            
             self._posicion_firmas(fiadores)
             self._parrafos.append(Spacer(0,0.5*cm))
-            
-        if(sw_personal==1):
-            a=self._parrafos.append
-            a(PageBreak())   
-        
-        # Doc. Custodia de Vehiculo    y    Convenio y Doc. Custodia Inmueble   y    Convenio y Doc. Custodia Vehiculo
-        if((tipo_garantia=="Doc. Custodia de Vehiculo" and  2<len(deudores)<=4) or (tipo_garantia=="Convenio y Doc. Custodia Inmueble" and  2<len(deudores)<=4) or (tipo_garantia=="Convenio y Doc. Custodia Vehiculo" and  2<len(deudores)<=4)):
-            a=self._parrafos.append
-            a(PageBreak())
-        # Doc. Custodia de Vehiculo    y   Convenio y Doc. Custodia Inmueble     y    Convenio y Doc. Custodia Vehiculo
-        # Otros Doc. En Custodia
-        if(tipo_garantia=="Otros Doc. En Custodia" and  len(deudores)>4):
-            a=self._parrafos.append
-            a(PageBreak())
-        # Otros Doc. En Custodia
-
-        texto= ('POR <b>GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A.</b>')
+        texto= ('POR <b>GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.</b>')
         self._parrafos.append(Paragraph(texto,style = estilos["Justify"]))  
         self._parrafos.append(Spacer(0,2.3*cm))
         dato_nombre = self.nombreCompleto_repre()
         dato_cargo = self.__contrato["testimonio_poder"]["representante_legal"]["rol"]
         t_firmas=Table(
                     data=[[dato_nombre+'\n'+dato_cargo]],colWidths=8*cm,
-                    style=[('ALIGN',(0,0),(-1,-1),'CENTER'),('FONT', (0,0), (-1,-1), 'Helvetica-Bold', 9.1),])
+                    style=[('ALIGN',(0,0),(-1,-1),'CENTER'),('FONT', (0,0), (-1,-1), 'Helvetica-Bold', 10),])
         self._parrafos.append(t_firmas)
 
     def _posicion_firmas(self, dato):
         for indice,item in enumerate(dato):
             if(indice!=len(dato)-1):
                 if(indice%2==0):
                     self._parrafos.append(Spacer(0,2.3*cm))
                     dato_1=dato[indice]
                     dato_2=dato[indice+1]
                     t_firmas=Table(
                         data=[[dato_1['nombre_completo'].upper()+'\nC.I. N° '+dato_1['ci'], dato_2['nombre_completo'].upper()+'\nC.I. N° '+dato_2['ci']]],colWidths=8*cm,
-                        style=[('ALIGN',(0,0),(-1,-1),'CENTER'),('FONT', (0,0), (-1,-1), 'Helvetica-Bold', 9.1),])
+                        style=[('ALIGN',(0,0),(-1,-1),'CENTER'),('FONT', (0,0), (-1,-1), 'Helvetica-Bold', 10),])
                     self._parrafos.append(t_firmas)
             else:
                 dato_1=dato[indice]
                 if(len(dato)%2!=0):
                     self._parrafos.append(Spacer(0,2.3*cm))
                     t_firmas=Table(
                         data=[[dato_1['nombre_completo'].upper()+'\nC.I. N° '+dato_1['ci']]],colWidths=8*cm,
-                        style=[('ALIGN',(0,0),(-1,-1),'CENTER'),('FONT', (0,0), (-1,-1), 'Helvetica-Bold', 9.1)])
+                        style=[('ALIGN',(0,0),(-1,-1),'CENTER'),('FONT', (0,0), (-1,-1), 'Helvetica-Bold', 10)])
                     self._parrafos.append(t_firmas)
                 else:
                     if(len(dato)==1):
                         self._parrafos.append(Spacer(0,2.3*cm))
                         t_firmas=Table(
                             data=[[dato_1[0]+'\nC.I. N° '+dato_1[1]]],colWidths=8*cm,
-                            style=[('ALIGN',(0,0),(-1,-1),'CENTER'),('FONT', (0,0), (-1,-1), 'Helvetica-Bold', 9.1)])
+                            style=[('ALIGN',(0,0),(-1,-1),'CENTER'),('FONT', (0,0), (-1,-1), 'Helvetica-Bold', 10)])
                         self._parrafos.append(t_firmas)
+    #FIRMAS GARANTE
+    # FIRMAS
+    def _firmas2(self):
+        fiadores= self.get_fiadores()
+        deudores= self.get_deudores()
+        self._parrafos.append(Spacer(0,15))
+        texto= ('POR SI, COMO DEUDOR(A)(ES) o PRESTATARIO(A)(S):')
+        self._parrafos.append(Paragraph(texto,style = estilos["Justify"]))        
+        self._posicion_firmas(deudores)
+        self._parrafos.append(Spacer(0,0.5*cm))
+        if (len(fiadores) > 0):
+            self._parrafos.append(Spacer(0,1))
+            texto= ('Y COMO GARANTE(S) SOLIDARIO(A)(S), MANCOMUNADO(A)(S) E INDIVISIBLE(S): ')
+            self._parrafos.append(Paragraph(texto,style = estilos["Justify"]))            
+            self._posicion_firmas(fiadores)
+            self._parrafos.append(Spacer(0,0.5*cm))
+        texto= ('POR <b>GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.</b>')
+        self._parrafos.append(Paragraph(texto,style = estilos["Justify"]))  
+        self._parrafos.append(Spacer(0,2.3*cm))
+        dato_nombre = self.nombreCompleto_repre()
+        dato_cargo = self.__contrato["testimonio_poder"]["representante_legal"]["rol"]
+        t_firmas=Table(
+                    data=[[dato_nombre+'\n'+dato_cargo]],colWidths=8*cm,
+                    style=[('ALIGN',(0,0),(-1,-1),'CENTER'),('FONT', (0,0), (-1,-1), 'Helvetica-Bold', 10),])
+        self._parrafos.append(t_firmas)
+
     
     def generar1(self):
         buffer = BytesIO()   
-        documentos(buffer).build(self._parrafos, onFirstPage=self._encabezado,  onLaterPages=self._encabezado,canvasmaker=NumberedCanvas)
+        documentos(buffer).build(self._parrafos, onFirstPage=self._encabezado,  onLaterPages=self._encabezado)
         return buffer
```

### Comparing `jgp_report_creditos-0.0.14/jgp_report_creditos/core/contrato/v1/contratos.py` & `jgp_report_creditos-0.0.9/jgp_report_creditos/core/contrato/v1/contratos.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from reportlab.pdfgen import canvas
 from jgp_report_creditos.core.exception.exception import ContratoError
 
 from .base import BaseContrato
 
 class ContratoPersonal (BaseContrato):
     
-    def __init__(self, json_enviado, usuario):
+    def __init__(self, json_enviado):
         try:
-            super().__init__(json_enviado, usuario)
+            super().__init__(json_enviado)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía Personal')
             self._partes_contratantes('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza('CUARTA')
             self._intereses('QUINTA')
             self._plazo('SEXTA')
@@ -36,17 +36,17 @@
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))  
         finally:
             print("TERMINADO")
 
 #11 CONVENIO Y GARANTIA PERSONAL
 class ContratoConvenioGarantiaPersonal (BaseContrato):
-    def __init__(self, json_enviado, usuario):
+    def __init__(self, contrato):
         try:
-            super().__init__(json_enviado, usuario)
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía de Derecho de Línea y garantía Personal')
             self._partes_contratantes('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza('CUARTA')
             self._intereses_pyv('QUINTA')#garantes
             self._plazo('SEXTA')
@@ -73,17 +73,17 @@
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))  
         finally:
             print("TERMINADO")
 
 # 12 GARANTE DEPOSITARIO
 class ContratoPrendariayPersonal(BaseContrato):
-    def __init__(self, json_enviado, usuario):
+    def __init__(self, contrato):
         try:
-            super().__init__(json_enviado, usuario)
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía Prendaria y Personal')
             self._partes_contratantes3('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza3('CUARTA')
             self._intereses3('QUINTA')
             self._plazo('SEXTA')
@@ -97,29 +97,29 @@
             self._cesion_obligacion('DÉCIMA TERCERA')
             self._autorizacion4('DÉCIMA CUARTA')
             self._titulo_ejecutivo('DÉCIMA QUINTA')
             self._gastos('DÉCIMA SEXTA')
             self._derechos_deudor('DÉCIMA SÉPTIMA')
             self._domicilio_especial('DÉCIMA OCTAVA')
             self._aceptacion3('DÉCIMA NOVENA')
-            self._firmas()
+            self._firmas2()
         except ContratoError as ex:
             p1, p2 = ex.args
             print("°°°°°°°°°°° ERROR PERSONALIZADO: °°°°°°°°°°")
             self._error_mensaje(p1,p2)
         except Exception as e:
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))   
         finally:
             print("TERMINADO")
 # CONVENIO
 class ContratoConvenio (BaseContrato):
-    def __init__(self, json_enviado, usuario):
+    def __init__(self, contrato):    
         try:
-            super().__init__(json_enviado, usuario)
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía de Derecho de Línea')
             self._partes_contratantes2('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza2('CUARTA')
             self._intereses2('QUINTA')
             self._plazo('SEXTA')
@@ -146,17 +146,17 @@
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))  
         finally:
             print("TERMINADO")
 
 # CONVENIO Y DOC. CUSTODIA DE INMUEBLE   -------------------------REVISADO 1-1
 class ContratoConvenioCustodiaInmueble (BaseContrato):
-    def __init__(self, json_enviado, usuario):
-        try:
-            super().__init__(json_enviado, usuario)
+    def __init__(self, contrato):
+        try:    
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía de Derecho de Línea y Garantía de Documentos en Custodia de Inmueble')        
             self._partes_contratantes2('PRIMERA')       
             self._objeto_del_contrato('SEGUNDA')       
             self._desembolso('TERCERA')       
             self._gestion_cobranza2('CUARTA')        
             self._intereses2('QUINTA')        
             self._plazo('SEXTA')        
@@ -183,17 +183,17 @@
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))   
         finally:
             print("TERMINADO")
 
 # CONVENIO Y DOC. CUSTODIA DE VEHÍCULO   
 class ContratoConvenioCustodiaVehiculo (BaseContrato):
-    def __init__(self, json_enviado, usuario):
+    def __init__(self, contrato):
         try:
-            super().__init__(json_enviado, usuario)
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía de Derecho de Línea y Garantía de Documentos en Custodia de Vehículo')
             self._partes_contratantes2('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza2('CUARTA')
             self._intereses2('QUINTA')
             self._plazo('SEXTA')
@@ -220,17 +220,17 @@
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e)) 
         finally:
             print("TERMINADO")
 
 # DOC. CUSTODIA DE INMUEBLE DE PAMPAHASI M
 class ContratoCustosiaInmueblePampahasi (BaseContrato):
-    def __init__(self, json_enviado, usuario):
+    def __init__(self, contrato):
         try:
-            super().__init__(json_enviado, usuario)
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía de Documentos en Custodia de Inmueble')
             self._partes_contratantes2('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza2('CUARTA')
             self._intereses2('QUINTA')
             self._plazo('SEXTA')
@@ -257,17 +257,17 @@
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))    
         finally:
             print("TERMINADO")
 
 # Documentos en Custodia de Vehículo M  ------EN REV
 class ContratoDocumentoCustodiaVehiculo (BaseContrato):
-    def __init__(self, json_enviado, usuario):
+    def __init__(self, contrato):
         try:
-            super().__init__(json_enviado, usuario)
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía de Documentos en Custodia de vehículo')
             self._partes_contratantes2('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza2('CUARTA')
             self._intereses2('QUINTA')
             self._plazo('SEXTA')
@@ -294,17 +294,17 @@
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))    
         finally:
             print("TERMINADO")
 
 # Otros Documentos en Custodia (patente) M
 class ContratoOtroDocumentoCustodiaPatente (BaseContrato):
-    def __init__(self, json_enviado, usuario):
+    def __init__(self, contrato):
         try:
-            super().__init__(json_enviado, usuario)
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía de Otros Documentos en Custodia')
             self._partes_contratantes2('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza2('CUARTA')
             self._intereses2('QUINTA')
             self._plazo('SEXTA')
@@ -330,17 +330,17 @@
         except Exception as e:
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))    
         finally:
             print("TERMINADO")
 # Personal y Documentos en Custodia de Vehículo M
 class ContratoPersonalDocumentosCustodiaVehiculo (BaseContrato):
-    def __init__(self, json_enviado, usuario):
+    def __init__(self, contrato):
         try:
-            super().__init__(json_enviado, usuario)
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía Personal y Documentos en Custodia de vehículo')
             self._partes_contratantes('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza('CUARTA')
             self._intereses_pyv('QUINTA')
             self._plazo('SEXTA')
@@ -366,17 +366,17 @@
         except Exception as e:
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))    
         finally:
             print("TERMINADO")
 # Quirografaria OFICINA EL CARMEN
 class ContratoQuirografariaOficinaElCarmen (BaseContrato):
-    def __init__(self, json_enviado, usuario):
-        try:
-            super().__init__(json_enviado, usuario)
+    def __init__(self, contrato):
+        try :
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía Quirografaria')
             self._partes_contratantes2('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza2('CUARTA')
             self._intereses2('QUINTA')
             self._plazo('SEXTA')
@@ -403,17 +403,17 @@
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))   
         finally:
             print("TERMINADO")
             
 # Solidario
 class ContratoSolidario (BaseContrato):
-    def __init__(self, json_enviado, usuario):
+    def __init__(self, contrato):
         try:
-            super().__init__(json_enviado, usuario)
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía Solidaria')
             self._partes_contratantes2Soli('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza2('CUARTA')
             self._intereses2('QUINTA')
             self._plazo('SEXTA')
@@ -438,10 +438,10 @@
         except Exception as e:
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))    
         finally:
             print("TERMINADO")
 # CONTRATO ERROR BASE
 class ContratoErrorBase(BaseContrato):
-    def __init__(self, json_enviado, usuario):
-        super().__init__(json_enviado, usuario)
+    def __init__(self, contrato):
+        super().__init__(contrato)
         self._error_mensaje("Error en el contrato","Tipo de garantia desconocido")
```

### Comparing `jgp_report_creditos-0.0.14/jgp_report_creditos/test.py` & `jgp_report_creditos-0.0.9/jgp_report_creditos/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 #from report import makeContato
 from jgp_report_creditos import makeContato
 
 if  __name__ == '__main__':     
     print(" ªªªªªªªªªªªªªªªªªªªªªªªªªªªªªªªªª test ªªªªªªªªªªªªªªªªªªªªªªªªªª")
-    parametros ="401211601714"
+    parametros ="501211601894"
     #datos_json= json.load(requests.get("http://190.181.25.202:8003/api/v1/cre/contrato/"+parametros).text)
     #http://192.168.100.5:8000/api/v1/contratos/501211601894/
     datos_json = requests.get("http://192.168.100.5:8000/api/v1/contratos/"+parametros).text
     print("ddddddddddddddddddddddddddddddddddddddd")
 
     #ESTA LLAMADA CREA EL PDF
     print(datos_json)
```

### Comparing `jgp_report_creditos-0.0.14/jgp_report_creditos.egg-info/PKG-INFO` & `jgp_report_creditos-0.0.9/jgp_report_creditos.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-Metadata-Version: 2.1
-Name: jgp-report-creditos
-Version: 0.0.14
-Summary: Librería con funciones y herramientas útiles exclusivas para jgp
-Home-page: https://gitlab.com/develop-team-jdgp/jgp-report-creditos.git
-Author: JGP Dev
-Author-email: jgpdev20@gmail.com
-License: MIT
-Keywords: python,primer paquete jgp
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# jgp-report-creditos
-
-
-
-## Getting started
-
-To make it easy for you to get started with GitLab, here's a list of recommended next steps.
-
-Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!
-
-## Add your files
-
-- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
-- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
-
-```
-cd existing_repo
-git remote add origin https://gitlab.com/develop-team-jdgp/jgp-report-creditos.git
-git branch -M main
-git push -uf origin main
-```
-
-## Integrate with your tools
-
-- [ ] [Set up project integrations](https://gitlab.com/develop-team-jdgp/jgp-report-creditos/-/settings/integrations)
-
-## Collaborate with your team
-
-- [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
-- [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
-- [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
-- [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
-- [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)
-
-## Test and Deploy
-
-Use the built-in continuous integration in GitLab.
-
-- [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)
-- [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
-- [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
-- [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
-- [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)
-
-***
-
-# Editing this README
-
-When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.
-
-## Suggestions for a good README
-Every project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.
-
-## Name
-Choose a self-explaining name for your project.
-
-## Description
-Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
-
-## Badges
-On some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.
-
-## Visuals
-Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.
-
-## Installation
-Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.
-
-## Usage
-Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
-
-## Support
-Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.
-
-## Roadmap
-If you have ideas for releases in the future, it is a good idea to list them in the README.
-
-## Contributing
-State if you are open to contributions and what your requirements are for accepting them.
-
-For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.
-
-You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.
-
-## Authors and acknowledgment
-Show your appreciation to those who have contributed to the project.
-
-## License
-For open source projects, say how it is licensed.
-
-## Project status
-If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
+Metadata-Version: 2.1
+Name: jgp-report-creditos
+Version: 0.0.9
+Summary: Librería con funciones y herramientas útiles exclusivas para jgp
+Home-page: https://gitlab.com/develop-team-jdgp/jgp-report-creditos.git
+Author: JGP Dev
+Author-email: jgpdev20@gmail.com
+License: MIT
+Description: # jgp-report-creditos
+        
+        
+        
+        ## Getting started
+        
+        To make it easy for you to get started with GitLab, here's a list of recommended next steps.
+        
+        Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!
+        
+        ## Add your files
+        
+        - [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
+        - [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
+        
+        ```
+        cd existing_repo
+        git remote add origin https://gitlab.com/develop-team-jdgp/jgp-report-creditos.git
+        git branch -M main
+        git push -uf origin main
+        ```
+        
+        ## Integrate with your tools
+        
+        - [ ] [Set up project integrations](https://gitlab.com/develop-team-jdgp/jgp-report-creditos/-/settings/integrations)
+        
+        ## Collaborate with your team
+        
+        - [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
+        - [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
+        - [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
+        - [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
+        - [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)
+        
+        ## Test and Deploy
+        
+        Use the built-in continuous integration in GitLab.
+        
+        - [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)
+        - [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
+        - [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
+        - [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
+        - [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)
+        
+        ***
+        
+        # Editing this README
+        
+        When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.
+        
+        ## Suggestions for a good README
+        Every project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.
+        
+        ## Name
+        Choose a self-explaining name for your project.
+        
+        ## Description
+        Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
+        
+        ## Badges
+        On some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.
+        
+        ## Visuals
+        Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.
+        
+        ## Installation
+        Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.
+        
+        ## Usage
+        Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
+        
+        ## Support
+        Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.
+        
+        ## Roadmap
+        If you have ideas for releases in the future, it is a good idea to list them in the README.
+        
+        ## Contributing
+        State if you are open to contributions and what your requirements are for accepting them.
+        
+        For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.
+        
+        You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.
+        
+        ## Authors and acknowledgment
+        Show your appreciation to those who have contributed to the project.
+        
+        ## License
+        For open source projects, say how it is licensed.
+        
+        ## Project status
+        If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
+        
+Keywords: python,primer paquete jgp
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `jgp_report_creditos-0.0.14/jgp_report_creditos.egg-info/SOURCES.txt` & `jgp_report_creditos-0.0.9/jgp_report_creditos.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,16 @@
-LICENSE
 README.md
 setup.py
 jgp_report_creditos/__init__.py
 jgp_report_creditos/report.py
 jgp_report_creditos/test.py
 jgp_report_creditos.egg-info/PKG-INFO
 jgp_report_creditos.egg-info/SOURCES.txt
 jgp_report_creditos.egg-info/dependency_links.txt
 jgp_report_creditos.egg-info/top_level.txt
 jgp_report_creditos/core/__init__.py
-jgp_report_creditos/core/deposito.py
-jgp_report_creditos/core/rutas.py
 jgp_report_creditos/core/contrato/__init__.py
-jgp_report_creditos/core/contrato/v1/Controlar tablas de firmas.py
 jgp_report_creditos/core/contrato/v1/__init__.py
 jgp_report_creditos/core/contrato/v1/base.py
 jgp_report_creditos/core/contrato/v1/contratos.py
 jgp_report_creditos/core/exception/__init__.py
-jgp_report_creditos/core/exception/exception.py
-jgp_report_creditos/resources/img/logo_jgp.png
-jgp_report_creditos/template/__init__.py
-jgp_report_creditos/template/components.py
-jgp_report_creditos/template/template.py
-jgp_report_creditos/tests/__init__.py
-jgp_report_creditos/tests/test_contratos.py
-jgp_report_creditos/tests/test_deposito.py
+jgp_report_creditos/core/exception/exception.py
```

### Comparing `jgp_report_creditos-0.0.14/setup.py` & `jgp_report_creditos-0.0.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.14' 
+VERSION = '0.0.9' 
 PACKAGE_NAME = 'jgp_report_creditos' 
 AUTHOR = 'JGP Dev' 
 AUTHOR_EMAIL = 'jgpdev20@gmail.com' 
 URL = 'https://gitlab.com/develop-team-jdgp/jgp-report-creditos.git'
 
 LICENSE = 'MIT' 
 DESCRIPTION = 'Librería con funciones y herramientas útiles exclusivas para jgp'
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8')
 LONG_DESC_TYPE = "text/markdown"
 
 
 INSTALL_REQUIRES = [
       #'locale'
-    ]
+      ]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type=LONG_DESC_TYPE,
```

