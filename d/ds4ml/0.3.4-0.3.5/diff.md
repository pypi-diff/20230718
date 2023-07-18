# Comparing `tmp/ds4ml-0.3.4.tar.gz` & `tmp/ds4ml-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds4ml-0.3.4.tar", last modified: Thu May 25 05:07:44 2023, max compression
+gzip compressed data, was "ds4ml-0.3.5.tar", last modified: Tue Jul 18 10:26:15 2023, max compression
```

## Comparing `ds4ml-0.3.4.tar` & `ds4ml-0.3.5.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxr-xr-x   0 i076744    (501) staff       (20)        0 2023-05-25 05:07:44.105912 ds4ml-0.3.4/
--rw-r--r--   0 i076744    (501) staff       (20)    11356 2020-06-08 02:24:17.000000 ds4ml-0.3.4/LICENSE
--rw-r--r--   0 i076744    (501) staff       (20)     1387 2023-05-25 05:07:44.105514 ds4ml-0.3.4/PKG-INFO
--rw-r--r--   0 i076744    (501) staff       (20)     9222 2022-11-17 08:39:17.000000 ds4ml-0.3.4/README.md
-drwxr-xr-x   0 i076744    (501) staff       (20)        0 2023-05-25 05:07:44.046149 ds4ml-0.3.4/ds4ml/
--rw-r--r--   0 i076744    (501) staff       (20)      109 2020-12-02 02:30:48.000000 ds4ml-0.3.4/ds4ml/__init__.py
--rw-r--r--   0 i076744    (501) staff       (20)      296 2023-05-25 05:04:17.000000 ds4ml-0.3.4/ds4ml/__version__.py
--rw-r--r--   0 i076744    (501) staff       (20)    18119 2023-05-25 05:03:27.000000 ds4ml-0.3.4/ds4ml/attribute.py
-drwxr-xr-x   0 i076744    (501) staff       (20)        0 2023-05-25 05:07:44.068088 ds4ml-0.3.4/ds4ml/command/
--rw-r--r--   0 i076744    (501) staff       (20)        0 2020-05-14 09:10:36.000000 ds4ml-0.3.4/ds4ml/command/__init__.py
--rw-r--r--   0 i076744    (501) staff       (20)     3645 2020-12-07 06:14:20.000000 ds4ml-0.3.4/ds4ml/command/evaluate.py
--rw-r--r--   0 i076744    (501) staff       (20)     3871 2022-11-17 08:39:17.000000 ds4ml-0.3.4/ds4ml/command/pattern.py
--rw-r--r--   0 i076744    (501) staff       (20)     1043 2020-11-30 13:10:48.000000 ds4ml-0.3.4/ds4ml/command/runtest.py
--rw-r--r--   0 i076744    (501) staff       (20)     5115 2021-02-01 02:37:59.000000 ds4ml-0.3.4/ds4ml/command/synthesize.py
--rw-r--r--   0 i076744    (501) staff       (20)    11225 2023-05-24 08:19:39.000000 ds4ml-0.3.4/ds4ml/dataset.py
--rw-r--r--   0 i076744    (501) staff       (20)    13556 2023-03-29 05:34:40.000000 ds4ml-0.3.4/ds4ml/evaluator.py
--rw-r--r--   0 i076744    (501) staff       (20)     2169 2020-12-03 08:17:26.000000 ds4ml-0.3.4/ds4ml/metrics.py
--rw-r--r--   0 i076744    (501) staff       (20)     8406 2023-05-24 23:07:17.000000 ds4ml-0.3.4/ds4ml/synthesizer.py
-drwxr-xr-x   0 i076744    (501) staff       (20)        0 2023-05-25 05:07:44.075742 ds4ml-0.3.4/ds4ml/template/
--rw-r--r--   0 i076744    (501) staff       (20)    10969 2020-12-01 09:36:31.000000 ds4ml-0.3.4/ds4ml/template/report.html
--rw-r--r--   0 i076744    (501) staff       (20)    15902 2023-05-25 05:03:33.000000 ds4ml-0.3.4/ds4ml/utils.py
-drwxr-xr-x   0 i076744    (501) staff       (20)        0 2023-05-25 05:07:44.050220 ds4ml-0.3.4/ds4ml.egg-info/
--rw-r--r--   0 i076744    (501) staff       (20)     1387 2023-05-25 05:07:43.000000 ds4ml-0.3.4/ds4ml.egg-info/PKG-INFO
--rw-r--r--   0 i076744    (501) staff       (20)      662 2023-05-25 05:07:43.000000 ds4ml-0.3.4/ds4ml.egg-info/SOURCES.txt
--rw-r--r--   0 i076744    (501) staff       (20)        1 2023-05-25 05:07:43.000000 ds4ml-0.3.4/ds4ml.egg-info/dependency_links.txt
--rw-r--r--   0 i076744    (501) staff       (20)      152 2023-05-25 05:07:43.000000 ds4ml-0.3.4/ds4ml.egg-info/entry_points.txt
--rw-r--r--   0 i076744    (501) staff       (20)      103 2023-05-25 05:07:43.000000 ds4ml-0.3.4/ds4ml.egg-info/requires.txt
--rw-r--r--   0 i076744    (501) staff       (20)        6 2023-05-25 05:07:43.000000 ds4ml-0.3.4/ds4ml.egg-info/top_level.txt
--rw-r--r--   0 i076744    (501) staff       (20)       38 2023-05-25 05:07:44.105967 ds4ml-0.3.4/setup.cfg
--rw-r--r--   0 i076744    (501) staff       (20)     2368 2023-04-17 02:03:40.000000 ds4ml-0.3.4/setup.py
-drwxr-xr-x   0 i076744    (501) staff       (20)        0 2023-05-25 05:07:44.101615 ds4ml-0.3.4/tests/
--rw-r--r--   0 i076744    (501) staff       (20)     9383 2023-03-29 05:43:50.000000 ds4ml-0.3.4/tests/test_attribute.py
--rw-r--r--   0 i076744    (501) staff       (20)     5723 2023-05-25 04:12:19.000000 ds4ml-0.3.4/tests/test_dataset.py
--rw-r--r--   0 i076744    (501) staff       (20)     2969 2020-12-04 10:07:23.000000 ds4ml-0.3.4/tests/test_evaluator.py
--rw-r--r--   0 i076744    (501) staff       (20)     1411 2020-12-03 07:44:47.000000 ds4ml-0.3.4/tests/test_metrics.py
--rw-r--r--   0 i076744    (501) staff       (20)     2513 2022-11-17 08:39:17.000000 ds4ml-0.3.4/tests/test_synthesizer.py
--rw-r--r--   0 i076744    (501) staff       (20)     5770 2023-05-23 21:44:57.000000 ds4ml-0.3.4/tests/test_utils.py
--rw-r--r--   0 i076744    (501) staff       (20)     4843 2020-05-14 09:10:36.000000 ds4ml-0.3.4/tests/testdata.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:26:15.517708 ds4ml-0.3.5/
+-rw-rw-rw-   0        0        0    11556 2023-07-18 05:27:55.000000 ds4ml-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0     1417 2023-07-18 10:26:15.515709 ds4ml-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     9566 2023-07-18 05:27:55.000000 ds4ml-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 10:26:15.383723 ds4ml-0.3.5/ds4ml/
+-rw-rw-rw-   0        0        0      113 2023-07-18 05:27:55.000000 ds4ml-0.3.5/ds4ml/__init__.py
+-rw-rw-rw-   0        0        0      305 2023-07-18 10:23:45.000000 ds4ml-0.3.5/ds4ml/__version__.py
+-rw-rw-rw-   0        0        0    18608 2023-07-18 05:27:55.000000 ds4ml-0.3.5/ds4ml/attribute.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:26:15.439708 ds4ml-0.3.5/ds4ml/command/
+-rw-rw-rw-   0        0        0        0 2023-07-18 05:27:55.000000 ds4ml-0.3.5/ds4ml/command/__init__.py
+-rw-rw-rw-   0        0        0     3735 2023-07-18 05:27:55.000000 ds4ml-0.3.5/ds4ml/command/evaluate.py
+-rw-rw-rw-   0        0        0     3964 2023-07-18 05:27:55.000000 ds4ml-0.3.5/ds4ml/command/pattern.py
+-rw-rw-rw-   0        0        0     5231 2023-07-18 05:27:55.000000 ds4ml-0.3.5/ds4ml/command/synthesize.py
+-rw-rw-rw-   0        0        0    11947 2023-07-18 05:27:55.000000 ds4ml-0.3.5/ds4ml/dataset.py
+-rw-rw-rw-   0        0        0    13891 2023-07-18 05:27:55.000000 ds4ml-0.3.5/ds4ml/evaluator.py
+-rw-rw-rw-   0        0        0     2245 2023-07-18 05:27:55.000000 ds4ml-0.3.5/ds4ml/metrics.py
+-rw-rw-rw-   0        0        0    14977 2023-07-18 05:27:55.000000 ds4ml-0.3.5/ds4ml/synthesizer.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:26:15.444709 ds4ml-0.3.5/ds4ml/template/
+-rw-rw-rw-   0        0        0    11343 2023-07-18 05:27:55.000000 ds4ml-0.3.5/ds4ml/template/report.html
+-rw-rw-rw-   0        0        0    17075 2023-07-18 05:27:55.000000 ds4ml-0.3.5/ds4ml/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:26:15.418712 ds4ml-0.3.5/ds4ml.egg-info/
+-rw-rw-rw-   0        0        0     1417 2023-07-18 10:26:15.000000 ds4ml-0.3.5/ds4ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      637 2023-07-18 10:26:15.000000 ds4ml-0.3.5/ds4ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 10:26:15.000000 ds4ml-0.3.5/ds4ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2023-07-18 10:26:15.000000 ds4ml-0.3.5/ds4ml.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      103 2023-07-18 10:26:15.000000 ds4ml-0.3.5/ds4ml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-18 10:26:15.000000 ds4ml-0.3.5/ds4ml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 10:26:15.518708 ds4ml-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     2441 2023-07-18 05:27:55.000000 ds4ml-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:26:15.510711 ds4ml-0.3.5/tests/
+-rw-rw-rw-   0        0        0     9970 2023-07-18 05:27:55.000000 ds4ml-0.3.5/tests/test_attribute.py
+-rw-rw-rw-   0        0        0     5880 2023-07-18 05:27:55.000000 ds4ml-0.3.5/tests/test_dataset.py
+-rw-rw-rw-   0        0        0     3059 2023-07-18 05:27:55.000000 ds4ml-0.3.5/tests/test_evaluator.py
+-rw-rw-rw-   0        0        0     1460 2023-07-18 05:27:55.000000 ds4ml-0.3.5/tests/test_metrics.py
+-rw-rw-rw-   0        0        0     2641 2023-07-18 05:27:55.000000 ds4ml-0.3.5/tests/test_synthesizer.py
+-rw-rw-rw-   0        0        0     5940 2023-07-18 05:27:55.000000 ds4ml-0.3.5/tests/test_utils.py
+-rw-rw-rw-   0        0        0     4931 2023-07-18 05:27:55.000000 ds4ml-0.3.5/tests/testdata.py
```

### Comparing `ds4ml-0.3.4/LICENSE` & `ds4ml-0.3.5/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
    limitations under the License.
```

### Comparing `ds4ml-0.3.4/PKG-INFO` & `ds4ml-0.3.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1
-Name: ds4ml
-Version: 0.3.4
-Summary: A Python library for data synthesis and evaluation
-Home-page: https://github.com/SAP/data-synthesis-for-machine-learning
-Maintainer: Yan Zhao
-Maintainer-email: yan.zhao01@sap.com
-Project-URL: Bug Tracker, https://github.com/SAP/data-synthesis-for-machine-learning/issues
-Project-URL: Documentation, https://github.com/SAP/data-synthesis-for-machine-learning
-Project-URL: Source Code, https://github.com/SAP/data-synthesis-for-machine-learning
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-The recent enforcement of data privacy protection regulations, such as GDPR,
-has made data sharing more difficult. This tool intends to facilitate data
-sharing from a customer by synthesizing a dataset based on the original dataset
-for later machine learning.
-
-There are two parts to this tool:
-
-- Data synthesizer
-  Synthesize a dataset based on the original dataset. It accepts CSV data as
-  input, and output a synthesized dataset based on Differential Privacy. The
-  algorithm in the data synthesizer reference to the paper (
-  http://dimacs.rutgers.edu/~graham/pubs/papers/privbayes-tods.pdf).
-- Data utility evaluation
-  Evaluate the data utility for the synthesized dataset. The original dataset
-  and the synthesized dataset as the input, one utility evaluation report will
-  be generated with several indicators.
+Metadata-Version: 2.1
+Name: ds4ml
+Version: 0.3.5
+Summary: A Python library for data synthesis and evaluation
+Home-page: https://github.com/SAP/data-synthesis-for-machine-learning
+Maintainer: Yan Zhao
+Maintainer-email: yan.zhao01@sap.com
+Project-URL: Bug Tracker, https://github.com/SAP/data-synthesis-for-machine-learning/issues
+Project-URL: Documentation, https://github.com/SAP/data-synthesis-for-machine-learning
+Project-URL: Source Code, https://github.com/SAP/data-synthesis-for-machine-learning
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+The recent enforcement of data privacy protection regulations, such as GDPR,
+has made data sharing more difficult. This tool intends to facilitate data
+sharing from a customer by synthesizing a dataset based on the original dataset
+for later machine learning.
+
+There are two parts to this tool:
+
+- Data synthesizer
+  Synthesize a dataset based on the original dataset. It accepts CSV data as
+  input, and output a synthesized dataset based on Differential Privacy. The
+  algorithm in the data synthesizer reference to the paper (
+  http://dimacs.rutgers.edu/~graham/pubs/papers/privbayes-tods.pdf).
+- Data utility evaluation
+  Evaluate the data utility for the synthesized dataset. The original dataset
+  and the synthesized dataset as the input, one utility evaluation report will
+  be generated with several indicators.
```

### Comparing `ds4ml-0.3.4/README.md` & `ds4ml-0.3.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,164 +1,168 @@
-# Data Synthesis for Machine Learning
-
-[![REUSE status](https://api.reuse.software/badge/github.com/SAP/data-synthesis-for-machine-learning)](https://api.reuse.software/info/github.com/SAP/data-synthesis-for-machine-learning)
-
-Note: fork of https://github.com/SAP/data-synthesis-for-machine-learning
-
-## Overview
-The recent enforcement of data privacy protection regulations, such as GDPR, has made data sharing more difficult. This tool intends to facilitate data sharing from a customer by synthesizing a dataset based on the original dataset for later machine learning. 
-There are two parts to this tool:
-+ Data synthesizer  
-  Synthesize a dataset based on the original dataset. It accepts CSV data as input, and output a synthesized dataset based on Differential Privacy. The algorithm in the data synthesizer reference to the paper - [PrivBayes 2017](http://dimacs.rutgers.edu/~graham/pubs/papers/privbayes-tods.pdf).
-+ Data utility evaluation  
-  Evaluate the data utility for the synthesized dataset. The original dataset and the synthesized dataset as the input, one utility evaluation report will be generated with several indicators.
-### Positioning
-Our project is independent of any DB and we are focus on the later machine learning. There is also one data anonymization feature in the HANA (not open sourced). Of a customer has HANA, please use this feature within HANA. If a customer does not have HANA and it's about a machine learning use case, please use our tool. Exception: If such a customer wants to try out the algorithm implemented in our tool to figure out if it provides better results than HANA, please use our tool.
-
-## Quickstart
-There are one demo dataset (part of the public dataset from [Adult](https://archive.ics.uci.edu/ml/datasets/Adult)), the synthesized dataset and the utility evaluation report in the folder *example* for your reference.
-### Prerequisites
-+ Install python >= 3.6.0 from [python.org](https://www.python.org/)
-+ Install project: run `pip install ds4ml`;
-+ Download demo data from [example/adult.csv](https://github.com/SAP/data-synthesis-for-machine-learning/blob/master/example/adult.csv)
-### Procedure
-  There are two parts in the project, data synthesizer and data utility evaluation.
-+ Synthesizer:  
-  ```
-  data-synthesize <original-dataset> <-o> <synthesized-dataset-path>
-  ```  
-  Use *adult.csv* as *original-dataset*, the synthesizer dataset *adult_a.csv* is generated under current folder by default.
-  
-  - To save the cost of (synthesized) data transfer, command `data-pattern` can help, which serialize anonymous patterns of a dataset. And then use `data-synthesize` to generate dataset from the pattern.
-  ```
-  data-pattern <original-dataset> <-o> <anonymous-pattern-path>
-  data-synthesize <anonymous-pattern-path> <-o> <synthesized-dataset-path>
-  ```
-+ Evaluation:  
-  ```
-  data-evaluate <original-dataset> <synthesized-dataset> --class-label <attribute1,attribute...>
-  ```  
-  Use *adult.csv* as *original-dataset*, *adult-a.csv* as *synthesized-dataset*, *sex,salary* as *attribute* in "--class-label", one *report.html* is generated under current folder by default.
-
-## Download and Installation
-+ Install Python 
-  Ensure your python >=3.6.0, you can download it from [python.org](https://www.python.org/)
-+ After clone the project, install it as: `python setup.py install`.
-  The project provides three commands: `data-synthesize`, `data-pattern` and `data-evaluate`. Run them with option `-h` for details.
-
-+ Help of `data-synthesize`
-  Run `data-synthesize -h`.
-  ```
-  usage: data-synthesize [-h] [--pseudonym LIST] [--delete LIST]
-                       [--na-values LIST] [-o FILE] [--no-header] [-e FLOAT]
-                       [--category LIST] [--retain LIST]
-                       file
-
-  Synthesize one dataset by Differential Privacy
-
-  positional arguments:
-    file                set path of a csv file to be synthesized or path of a 
-                        pattern file to be generated
-
-  general arguments:
-    -h, --help          show this help message and exit
-    --pseudonym LIST    set candidate columns separated by a comma, which will
-                        be replaced with a pseudonym. It only works on the
-                        string column.
-    --delete LIST       set columns separated by a comma, which will be deleted
-                        when synthesis.
-    --na-values LIST    set additional values to recognize as NA/NaN; (default
-                        null values are from pandas.read_csv)
-    -o, --output FILE   set the file name of output synthesized dataset
-                        (default is input file name with suffix '-a.csv')
-    --no-header         indicate there is no header in a CSV file, and will
-                        take [#0, #1, #2, ...] as header. (default: the tool
-                        will try to detect and take actions)
-    --records INT       specify the records you want to generate; default is the
-                        same records with the original dataset
-    --sep STRING        specify the delimiter of the input file
-
-  advanced arguments:
-    -e, --epsilon FLOAT  set epsilon for differential privacy (default 0.1)
-    --category LIST      set categorical columns separated by a comma.
-    --retain LIST        set columns to retain the values
-  ```
-
-  - Note: argument **epsilon** (ε) defines the privacy guarantee, which depends on the size and features of the dataset to be anonymized. The lower the value of epsilon, the more noise is applied, and the less the utility. 
-
-
-+ Help of `data-pattern`
-  Run `data-pattern -h`.
-  ```
-  usage: data-pattern [-h] [--pseudonym LIST] [--delete LIST] [--na-values LIST]
-                    [-o FILE] [--no-header] [--sep STRING] [-e FLOAT]
-                    [--category LIST] [--retain LIST]
-                    file
-
-  Serialize patterns of a dataset anonymously
-
-  positional arguments:
-    file                 set path of a csv file to be patterned anonymously
-
-  general arguments:
-    -h, --help           show this help message and exit
-    --pseudonym LIST     set candidate columns separated by a comma, which will
-                         be replaced with a pseudonym. It only works on the
-                         string column.
-    --delete LIST        set columns separated by a comma, which will be deleted
-                         when synthesis.
-    --na-values LIST     set additional values to recognize as NA/NaN; (default
-                         null values are from pandas.read_csv)
-    -o, --output FILE    set the file name of anonymous patterns (default is
-                         input file name with a suffix '-pattern.json')
-    --no-header          indicate there is no header in a CSV file, and will
-                         take [#0, #1, #2, ...] as header. (default: the tool
-                         will try to detect and take actions)
-    --sep STRING         specify the delimiter of the input file
-
-  advanced arguments:
-    -e, --epsilon FLOAT  set epsilon for differential privacy (default 0.1)
-    --category LIST      set categorical columns separated by a comma.
-  ```
-
-  - Note: after the pattern (.json) file is generated by `data-pattern` anonymously, then run command `data-synthesize *-pattern.json` to synthesize the data.
-
-
-+ Help of `data-evaluate`
-  Run `data-evaluate -h`.
-  ```
-  usage: data-evaluate [-h] [--na-values LIST] [-o FILE] [-t TEST]
-                      [--class-label LIST]
-                      source target
-
-  Evaluate the utility of the synthesized dataset compared with the source dataset.
-
-  positional arguments:
-    source              set file path of source (raw) dataset to be compared with
-                        synthesized dataset, only support CSV files
-    target              set file path of target (synthesized) dataset to evaluate
-
-  general arguments:
-    -h, --help          show this help message and exit
-    --na-values LIST    set additional values to recognize as NA/NaN; (default
-                        null values are from pandas.read_csv)
-    -o, --output FILE   set output path for evaluation report; (default is
-                        "report.html" under current work directory)
-
-  advanced arguments:
-    -t, --test TEST     set test dataset for classification or regression task;
-                        (default take 20 percent from source dataset)
-    --category LIST     set categorical columns separated by a comma.
-    --class-label LIST  set column name as a class label for classification or
-                        regression task; supports one or multiple columns
-                        (separated by comma)
-  ```
-  
-## How to obtain support
-If you encounter an issue, you can open an issue in GitHub.
-
-## Contribute
-Please check our [Contribution Guidelines](/CONTRIBUTING.md).
-
-## Licensing
-
-Copyright 2019-2021 SAP SE or an SAP affiliate company and data-synthesis-for-machine-learning contributors. Please see our [LICENSE](LICENSE) for copyright and license information. Detailed information including third-party components and their licensing/copyright information is available [via the REUSE tool](https://api.reuse.software/info/github.com/SAP/data-synthesis-for-machine-learning).
+# Data Synthesis for Machine Learning
+
+[![REUSE status](https://api.reuse.software/badge/github.com/SAP/data-synthesis-for-machine-learning)](https://api.reuse.software/info/github.com/SAP/data-synthesis-for-machine-learning)
+
+Note: fork of https://github.com/SAP/data-synthesis-for-machine-learning
+
+## Overview
+The recent enforcement of data privacy protection regulations, such as GDPR, has made data sharing more difficult. This tool intends to facilitate data sharing from a customer by synthesizing a dataset based on the original dataset for later machine learning. 
+There are two parts to this tool:
++ Data synthesizer  
+  Synthesize a dataset based on the original dataset. It accepts CSV data as input, 
+and output a synthesized dataset based on Differential Privacy. The algorithm in
+the data synthesizer reference to the paper - [PrivBayes 2014](https://www.dimacs.rutgers.edu/~graham/pubs/papers/PrivBayes.pdf)
+and [PrivBayes 2017](https://www.dimacs.rutgers.edu/~graham/pubs/papers/privbayes-tods.pdf) (implement based on the 
+algorithm guideline in paper, and add some optimizations).
++ Data utility evaluation  
+  Evaluate the data utility for the synthesized dataset. The original dataset and the synthesized dataset as the input, one utility evaluation report will be generated with several indicators.
+### Positioning
+Our project is independent of any DB and we are focus on the later machine learning. There is also one data anonymization feature in the HANA (not open sourced). Of a customer has HANA, please use this feature within HANA. If a customer does not have HANA and it's about a machine learning use case, please use our tool. Exception: If such a customer wants to try out the algorithm implemented in our tool to figure out if it provides better results than HANA, please use our tool.
+
+## Quickstart
+There are one demo dataset (part of the public dataset from [Adult](https://archive.ics.uci.edu/ml/datasets/Adult)), the synthesized dataset and the utility evaluation report in the folder *example* for your reference.
+### Prerequisites
++ Install python >= 3.6.0 from [python.org](https://www.python.org/)
++ Install project: run `pip install ds4ml`;
++ Download demo data from [example/adult.csv](https://github.com/SAP/data-synthesis-for-machine-learning/blob/master/example/adult.csv)
+### Procedure
+  There are two parts in the project, data synthesizer and data utility evaluation.
++ Synthesizer:  
+  ```
+  data-synthesize <original-dataset> <-o> <synthesized-dataset-path>
+  ```  
+  Use *adult.csv* as *original-dataset*, the synthesizer dataset *adult_a.csv* is generated under current folder by default.
+  
+  - To save the cost of (synthesized) data transfer, command `data-pattern` can help, which serialize anonymous patterns of a dataset. And then use `data-synthesize` to generate dataset from the pattern.
+  ```
+  data-pattern <original-dataset> <-o> <anonymous-pattern-path>
+  data-synthesize <anonymous-pattern-path> <-o> <synthesized-dataset-path>
+  ```
++ Evaluation:  
+  ```
+  data-evaluate <original-dataset> <synthesized-dataset> --class-label <attribute1,attribute...>
+  ```  
+  Use *adult.csv* as *original-dataset*, *adult-a.csv* as *synthesized-dataset*, *sex,salary* as *attribute* in "--class-label", one *report.html* is generated under current folder by default.
+
+## Download and Installation
++ Install Python 
+  Ensure your python >=3.6.0, you can download it from [python.org](https://www.python.org/)
++ After clone the project, install it as: `python setup.py install`.
+  The project provides three commands: `data-synthesize`, `data-pattern` and `data-evaluate`. Run them with option `-h` for details.
+
++ Help of `data-synthesize`
+  Run `data-synthesize -h`.
+  ```
+  usage: data-synthesize [-h] [--pseudonym LIST] [--delete LIST]
+                       [--na-values LIST] [-o FILE] [--no-header] [-e FLOAT]
+                       [--category LIST] [--retain LIST]
+                       file
+
+  Synthesize one dataset by Differential Privacy
+
+  positional arguments:
+    file                set path of a csv file to be synthesized or path of a 
+                        pattern file to be generated
+
+  general arguments:
+    -h, --help          show this help message and exit
+    --pseudonym LIST    set candidate columns separated by a comma, which will
+                        be replaced with a pseudonym. It only works on the
+                        string column.
+    --delete LIST       set columns separated by a comma, which will be deleted
+                        when synthesis.
+    --na-values LIST    set additional values to recognize as NA/NaN; (default
+                        null values are from pandas.read_csv)
+    -o, --output FILE   set the file name of output synthesized dataset
+                        (default is input file name with suffix '-a.csv')
+    --no-header         indicate there is no header in a CSV file, and will
+                        take [#0, #1, #2, ...] as header. (default: the tool
+                        will try to detect and take actions)
+    --records INT       specify the records you want to generate; default is the
+                        same records with the original dataset
+    --sep STRING        specify the delimiter of the input file
+
+  advanced arguments:
+    -e, --epsilon FLOAT  set epsilon for differential privacy (default 0.1)
+    --category LIST      set categorical columns separated by a comma.
+    --retain LIST        set columns to retain the values
+  ```
+
+  - Note: argument **epsilon** (ε) defines the privacy guarantee, which depends on the size and features of the dataset to be anonymized. The lower the value of epsilon, the more noise is applied, and the less the utility. 
+
+
++ Help of `data-pattern`
+  Run `data-pattern -h`.
+  ```
+  usage: data-pattern [-h] [--pseudonym LIST] [--delete LIST] [--na-values LIST]
+                    [-o FILE] [--no-header] [--sep STRING] [-e FLOAT]
+                    [--category LIST] [--retain LIST]
+                    file
+
+  Serialize patterns of a dataset anonymously
+
+  positional arguments:
+    file                 set path of a csv file to be patterned anonymously
+
+  general arguments:
+    -h, --help           show this help message and exit
+    --pseudonym LIST     set candidate columns separated by a comma, which will
+                         be replaced with a pseudonym. It only works on the
+                         string column.
+    --delete LIST        set columns separated by a comma, which will be deleted
+                         when synthesis.
+    --na-values LIST     set additional values to recognize as NA/NaN; (default
+                         null values are from pandas.read_csv)
+    -o, --output FILE    set the file name of anonymous patterns (default is
+                         input file name with a suffix '-pattern.json')
+    --no-header          indicate there is no header in a CSV file, and will
+                         take [#0, #1, #2, ...] as header. (default: the tool
+                         will try to detect and take actions)
+    --sep STRING         specify the delimiter of the input file
+
+  advanced arguments:
+    -e, --epsilon FLOAT  set epsilon for differential privacy (default 0.1)
+    --category LIST      set categorical columns separated by a comma.
+  ```
+
+  - Note: after the pattern (.json) file is generated by `data-pattern` anonymously, then run command `data-synthesize *-pattern.json` to synthesize the data.
+
+
++ Help of `data-evaluate`
+  Run `data-evaluate -h`.
+  ```
+  usage: data-evaluate [-h] [--na-values LIST] [-o FILE] [-t TEST]
+                      [--class-label LIST]
+                      source target
+
+  Evaluate the utility of the synthesized dataset compared with the source dataset.
+
+  positional arguments:
+    source              set file path of source (raw) dataset to be compared with
+                        synthesized dataset, only support CSV files
+    target              set file path of target (synthesized) dataset to evaluate
+
+  general arguments:
+    -h, --help          show this help message and exit
+    --na-values LIST    set additional values to recognize as NA/NaN; (default
+                        null values are from pandas.read_csv)
+    -o, --output FILE   set output path for evaluation report; (default is
+                        "report.html" under current work directory)
+
+  advanced arguments:
+    -t, --test TEST     set test dataset for classification or regression task;
+                        (default take 20 percent from source dataset)
+    --category LIST     set categorical columns separated by a comma.
+    --class-label LIST  set column name as a class label for classification or
+                        regression task; supports one or multiple columns
+                        (separated by comma)
+  ```
+  
+## How to obtain support
+If you encounter an issue, you can open an issue in GitHub.
+
+## Contribute
+Please check our [Contribution Guidelines](/CONTRIBUTING.md).
+
+## Licensing
+
+Copyright 2019-2021 SAP SE or an SAP affiliate company and data-synthesis-for-machine-learning contributors. Please see our [LICENSE](LICENSE) for copyright and license information. Detailed information including third-party components and their licensing/copyright information is available [via the REUSE tool](https://api.reuse.software/info/github.com/SAP/data-synthesis-for-machine-learning).
```

### Comparing `ds4ml-0.3.4/ds4ml/attribute.py` & `ds4ml-0.3.5/ds4ml/attribute.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,489 +1,489 @@
-"""
-Attribute: data structure for 1-dimensional cross-sectional data
-
-This class only handle integer, float, string, datetime columns, and it can be
-labeled as categorical column.
-"""
-from bisect import bisect_right
-from random import uniform
-from pandas import Series, DataFrame
-from dateutil.parser import parse
-from datetime import datetime, timedelta
-
-import numpy as np
-
-from ds4ml import utils
-
-
-# Default environment variables for data processing and analysis
-DEFAULT_BIN_SIZE = 20
-
-
-class AttributePattern:
-    """
-    A helper class of ``Attribute`` to store its patterns.
-    """
-    # _type: date type for handle different kinds of attributes in data
-    # synthesis, only support: integer, float, string, datetime.
-    _type = None
-    categorical = False
-    # min, max has been defined as member function of pandas.Series
-    min_ = None
-    max_ = None
-    _decimals = None
-
-    # probability distribution (pr)
-    bins = None
-    prs = None
-    _counts = None
-    _pattern_generated = False
-
-    # Here _bin_size is int-typed (to show the size of histogram bins), which
-    # is different from bins in np.histogram.
-    _bin_size = DEFAULT_BIN_SIZE
-
-    @property
-    def type(self):
-        return self._type
-
-
-class Attribute(AttributePattern, Series):
-
-    _epoch = datetime(1970, 1, 1)  # for datetime handling
-
-    def __init__(self, *args, **kwargs):
-        """
-        An improved Series with extra pattern information, e.g. categorical,
-        min/max value, and probability distribution.
-
-        The ``Attribute`` class has two modes:
-
-        - it has raw data, and then can calculate its pattern from the data;
-
-        - it doesn't have raw data, and only have the pattern from customer.
-
-        Parameters
-        ----------
-        categorical : bool
-            set categorical label for attribute. If categorical, this attribute
-            takes on a limited and fixed number of possible values. Examples:
-            blood type, gender.
-        """
-        categorical = kwargs.pop('categorical', False)
-        # The `categorical` option can be set to true when the attribute is
-        # string-typed and all values are not unique, and its value can be
-        # overridden by user.
-        if categorical or (
-                isinstance(args[0], Series)
-                and args[0].dtype == 'object'
-                and utils.is_discrete_values(args[0])):
-            kwargs.update({'dtype': 'category'})
-            categorical = True
-        super().__init__(*args, **kwargs)
-        self.set_pattern(categorical=categorical)
-
-    def _calculate_pattern(self):
-        from pandas.api.types import infer_dtype
-        self.categorical = self.dtype == 'category'
-        if self.categorical:
-            self._type = infer_dtype(self.cat.categories, skipna=True)
-        else:
-            self._type = infer_dtype(self, skipna=True)
-        if self._type == 'integer':
-            pass
-        elif self._type == 'floating' or self._type == 'mixed-integer-float':
-            self._type = 'float'
-        elif self._type in ['string', 'mixed-integer', 'mixed']:
-            self._type = 'string'
-            if all(map(utils.is_datetime, self._values)):
-                self._type = 'datetime'
-
-        if self.type == 'string' and not self.categorical:
-            # check string categories (when attribute is set from pattern)
-            if utils.is_discrete_values(self):
-                self._update_categories_inplace([])
-                self.categorical = True
-
-        # fill the missing values with the most frequent value
-        if self.hasnans:
-            self.fillna(self.mode()[0], inplace=True)
-
-        # for datetime attribute is converted to seconds since Unix epoch time
-        if self.type == 'datetime':
-            if self.categorical:
-                # re-order datetime categories in below function
-                self._update_categories_inplace([])
-            else:
-                self.update(self.map(self._to_seconds))
-
-        if self.type == 'float':
-            self._decimals = self.decimals()
-
-        self._set_domain()
-        self._set_distribution()
-
-    # handling functions for datetime attribute
-    def _to_seconds(self, timestr):
-        return int((parse(timestr) - self._epoch).total_seconds())
-
-    def _date_formatter(self, seconds):
-        date = self._epoch + timedelta(seconds=seconds)
-        return '%d/%d/%d' % (date.month, date.day, date.year)
-
-    # Take pandas.Series as manipulation result.
-    @property
-    def _constructor(self):
-        return Series
-
-    @property
-    def _constructor_expanddim(self):
-        from ds4ml.dataset import DataSet
-        return DataSet
-
-    def set_pattern(self, pattern=None, **kwargs):
-        """
-        Set an attribute's pattern, including its type, min/max value, and
-        probability distributions.
-        If patter is None, then calculation its pattern from its data.
-        """
-        if not self._pattern_generated:
-            self.categorical = kwargs.pop("categorical", False)
-            if pattern is None:
-                # to calculate the pattern use its data
-                self._calculate_pattern()
-            else:
-                self._type = pattern['type']
-                if self.type == 'float':
-                    self._decimals = pattern['decimals']
-                self.categorical = pattern['categorical']
-                self.min_ = pattern['min']
-                self.max_ = pattern['max']
-                self.bins = np.array(pattern['bins'])
-                self.prs = np.array(pattern['prs'])
-            self._pattern_generated = True
-
-    @property
-    def is_numerical(self):
-        return self._type == 'integer' or self._type == 'float'
-
-    @property
-    def domain(self):
-        """
-        Return attribute's domain, which can be a list of values for categorical
-        attribute, and an interval with min/max value for non-categorical
-        attribute.
-        """
-        if self.categorical:
-            return self.bins
-        return [self.min_, self.max_]
-
-    def _step(self):
-        """ Return step for numerical or datetime attribute. """
-        return (self.max_ - self.min_) / self._bin_size
-
-    def _update_categories_inplace(self, new_categories):
-        if self.categorical:
-            if self._type in ['string', 'datetime']:
-                new_categories = set(new_categories + self.cat.categories.to_list())
-                if self.type == 'datetime':
-                    new_categories = sorted(new_categories, key=self._to_seconds)
-                else:
-                    new_categories = sorted(new_categories)
-            cat = self.cat.set_categories(new_categories)
-            super().__init__(cat, dtype='category')
-        else:
-            new_categories = sorted(set(new_categories + self.dropna().unique().tolist()))
-            series = self.astype('category')
-            cat = series.cat.set_categories(new_categories)
-            super().__init__(cat, dtype='category')
-
-    @domain.setter
-    def domain(self, domain: list):
-        """
-        Set attribute's domain, includes min, max, frequency, or distribution.
-
-        Generally, the domain of one attribute can be calculated automatically.
-        This method can be manually called for specific purposes, e.g. compare
-        two same attributes based on same domain.
-
-        Parameters
-        ----------
-        domain : list
-            domain of one attribute. For numerical or datetime attributes, it
-            should be a list of two elements [min, max]; For categorical
-            attributes, it should a list of potential values of this attribute.
-        """
-        if self.categorical:
-            self._update_categories_inplace(domain)
-
-        # if a attribute is numerical and categorical and domain's length is
-        # bigger than 2, take it as categorical. e.g. zip code.
-        if self.type == 'datetime' and not self.categorical:
-            domain = list(map(self._to_seconds, domain))
-        if (self.is_numerical and self.categorical and len(domain) > 2) or (
-                self.categorical):
-            self.min_, self.max_ = min(domain), max(domain)
-            self.bins = np.array(domain)
-        elif self.is_numerical:
-            self.min_, self.max_ = domain
-            self.bins = np.array([self.min_, self.max_])
-        elif self._type == 'string':
-            lengths = [len(str(i)) for i in domain]
-            self.min_, self.max_ = min(lengths), max(lengths)
-            self.bins = np.array(domain)
-        self._set_distribution()
-
-    def _set_domain(self):
-        """
-        Compute domain (min, max, distribution bins) from input data
-        """
-        if self.categorical:
-            self.bins = self.cat.categories
-
-        if self._type == 'string':
-            items = self.astype(str).map(len)
-            self.min_ = int(items.min())
-            self.max_ = int(items.max())
-            if not self.categorical:
-                self.bins = np.array([self.min_, self.max_])
-        elif self._type == 'datetime':
-            if not self.categorical:
-                self.min_ = float(self.min())
-                self.max_ = float(self.max())
-                self.bins = np.array([self.min_, self.max_])
-        else:
-            if not self.categorical:
-                self.min_ = float(self.min())
-                self.max_ = float(self.max())
-                self.bins = np.array([self.min_, self.max_])
-
-    def _set_distribution(self):
-        if self.categorical:
-            counts = self.value_counts()
-            for value in set(self.bins) - set(counts.index):
-                counts[value] = 0
-            counts.sort_index(inplace=True)
-            # if self.type == 'datetime':
-            #     counts.index = list(map(self._date_formatter, counts.index))
-            self._counts = counts.values
-            self.prs = utils.normalize_distribution(counts)
-            self.bins = np.array(counts.index)
-        else:
-            # Note: hist, edges = numpy.histogram(), all but the last bin
-            # is half-open. If bins is 20, then len(hist)=20, len(edges)=21
-            if self.type == 'string':
-                hist, edges = np.histogram(self.astype(str).map(len),
-                                           bins=self._bin_size)
-            else:
-                hist, edges = np.histogram(self, bins=self._bin_size,
-                                           range=(self.min_, self.max_))
-            self.bins = edges[:-1]  # Remove the last bin edge
-            self._counts = hist
-            self.prs = utils.normalize_distribution(hist)
-            if self.type == 'integer':
-                self.min_ = int(self.min_)
-                self.max_ = int(self.max_)
-
-    def counts(self, bins=None, normalize=True):
-        """
-        Return an array of counts (or normalized density) of unique values.
-
-        This function works with `attribute.bins`. Combination of both are
-        like `Series.value_counts`. The parameter `bins` can be none, or a list.
-        """
-        if bins is None:
-            return self._counts
-        if self.categorical:
-            self._update_categories_inplace(bins)
-
-            # if self.type == 'datetime':
-            #     bins = list(map(self._to_seconds, bins))
-            counts = self.value_counts()
-            for value in set(bins) - set(counts.index):
-                counts[value] = 0
-            if normalize:
-                return np.array([round(counts.get(b)/sum(counts) * 100, 2)
-                                 for b in bins])
-            return np.array([counts.get(b) for b in bins])
-
-        if len(bins) == 1:
-            return np.array([self.size])
-        hist, _ = np.histogram(self, bins=bins)
-        if normalize:
-            return (hist / hist.sum() * 100).round(2)
-        return hist
-
-    def bin_indexes(self):
-        """
-        Encode values into bin indexes for Bayesian Network.
-        """
-        if self.categorical:
-            # mapping = {value: idx for idx, value in enumerate(self.bins)}
-            # indexes = self.map(lambda x: mapping[x], na_action='ignore')
-            indexes = Series(self.cat.codes)
-        else:
-            indexes = self.map(lambda x: bisect_right(self.bins, x) - 1,
-                               na_action='ignore')
-        indexes.fillna(len(self.bins), inplace=True)
-        return indexes.astype(int, copy=False)
-
-    def to_pattern(self):
-        """
-        Return attribution's metadata information in JSON format or Python
-        dictionary. Usually used in debug and testing.
-        """
-        return {
-            'name': self.name,
-            'type': self._type,
-            'categorical': self.categorical,
-            'min': self.min_,
-            'max': self.max_,
-            'decimals': self._decimals if self.type == 'float' else None,
-            'bins': self.bins.tolist(),
-            'prs': self.prs.tolist()
-        }
-
-    def decimals(self):
-        """
-        Returns number of decimals places for floating attribute. Used for
-        generated dataset to keep consistent decimal places for float attribute.
-        """
-        def decimals_of(value: float):
-            value = str(value)
-            return len(value) - value.rindex('.') - 1
-
-        counts = self.map(decimals_of).value_counts()
-        slot = 0
-        for i in range(len(counts)):
-            if sum(counts.head(i + 1)) / sum(counts) > 0.8:
-                slot = i + 1
-                break
-        return max(counts.index[:slot])
-
-    def pseudonymize(self, size=None):
-        """
-        Return pseudonymized values for this attribute, which is used to
-        substitute identifiable data with a reversible, consistent value.
-        """
-        size = size or self.size
-        if size != self.size:
-            attr = Series(np.random.choice(self.bins, size=size, p=self.prs))
-        else:
-            attr = self
-        if self.categorical:
-            mapping = {b: utils.pseudonymise_string(b) for b in self.bins}
-            return attr.map(lambda x: mapping[x])
-
-        if self.type == 'string':
-            return attr.map(utils.pseudonymise_string)
-        elif self.is_numerical or self.type == 'datetime':
-            return attr.map(str).map(utils.pseudonymise_string)
-
-    def random(self, size=None):
-        """
-        Return an random array with same length (usually used for
-        non-categorical attribute).
-        """
-        size = size or self.size
-        if self.min_ == self.max_:
-            rands = np.ones(size) * self.min_
-        else:
-            rands = np.arange(self.min_, self.max_, (self.max_-self.min_)/size)
-
-        np.random.shuffle(rands)
-        if self.type == 'string':
-            if self.min_ == self.max_:
-                length = self.min_
-            else:
-                length = np.random.randint(self.min_, self.max_)
-            vectorized = np.vectorize(lambda x: utils.randomize_string(length))
-            rands = vectorized(rands)
-        elif self.type == 'integer':
-            rands = list(map(int, rands))
-        elif self.type == 'datetime':
-            rands = list(map(self._date_formatter, rands))
-        return Series(rands)
-
-    def retain(self, size=None):
-        """ Return retained attribute with the size """
-        size = size or self.size
-        if size < self.size:
-            return self.head(size)
-        if size == self.size:
-            return self
-        copies = size // self.size
-        remainder = size - (copies * self.size)
-
-        return Series(self.tolist() * copies + self.head(remainder).tolist())
-
-    def _random_sample_at(self, index: int):
-        """ Sample a value from distribution bins at position 'index'"""
-        if self.categorical:
-            return self.bins[index]
-
-        length = len(self.bins)
-        if index < length - 1:
-            return uniform(self.bins[index], self.bins[index + 1])
-        return uniform(self.bins[-1], self.max_)
-
-    def choice(self, size=None, indexes=None):
-        """
-        Return a random sample based on this attribute's probability and
-        distribution bins (default value is base random distribution bins based
-        on its probability).
-
-        Parameters
-        ----------
-        size : int
-            size of random sample
-
-        indexes : array-like
-            array of indexes in distribution bins
-        """
-        if indexes is None:
-            size = size or self.size
-            indexes = Series(np.random.choice(len(self.prs),
-                                              size=size, p=self.prs))
-        column = indexes.map(self._random_sample_at)
-        if self.type == 'datetime':
-            if not self.categorical:
-                column = column.map(self._date_formatter)
-        elif self.type == 'float':
-            column = column.round(self._decimals)
-        elif self.type == 'integer':
-            column = column.round().astype(int)
-        elif self.type == 'string':
-            if not self.categorical:
-                column = column.map(lambda x: utils.randomize_string(int(x)))
-        return column
-
-    def encode(self, data=None):
-        """
-        Encode labels to normalized encoding.
-
-        Parameters
-        ----------
-        data : array-like
-            target values
-        """
-        if data is None:
-            data = self.copy()
-        else:
-            if self.type == 'datetime':
-                if all(map(utils.is_datetime, data)):
-                    data = data.map(self._to_seconds)
-                else:
-                    data = data.map(int)
-
-        if self.categorical:
-            frame = DataFrame()
-            for col in self.bins:
-                frame[col] = data.apply(lambda v: 1 if v == col else 0)
-            return frame
-
-        if self.type != 'string':
-            step = self._step()
-            return data.apply(lambda v:  # 1e-8 is a small delta
-                              int((v - self.min_) / (step + 1e-8))
-                              / self._bin_size)
-        raise ValueError('Can\'t encode Non-categorical attribute.')
+"""
+Attribute: data structure for 1-dimensional cross-sectional data
+
+This class only handle integer, float, string, datetime columns, and it can be
+labeled as categorical column.
+"""
+from bisect import bisect_right
+from random import uniform
+from pandas import Series, DataFrame
+from dateutil.parser import parse
+from datetime import datetime, timedelta
+
+import numpy as np
+
+from ds4ml import utils
+
+
+# Default environment variables for data processing and analysis
+DEFAULT_BIN_SIZE = 20
+
+
+class AttributePattern:
+    """
+    A helper class of ``Attribute`` to store its patterns.
+    """
+    # _type: date type for handle different kinds of attributes in data
+    # synthesis, only support: integer, float, string, datetime.
+    _type = None
+    categorical = False
+    # min, max has been defined as member function of pandas.Series
+    min_ = None
+    max_ = None
+    _decimals = None
+
+    # probability distribution (pr)
+    bins = None
+    prs = None
+    _counts = None
+    _pattern_generated = False
+
+    # Here _bin_size is int-typed (to show the size of histogram bins), which
+    # is different from bins in np.histogram.
+    _bin_size = DEFAULT_BIN_SIZE
+
+    @property
+    def type(self):
+        return self._type
+
+
+class Attribute(AttributePattern, Series):
+
+    _epoch = datetime(1970, 1, 1)  # for datetime handling
+
+    def __init__(self, *args, **kwargs):
+        """
+        An improved Series with extra pattern information, e.g. categorical,
+        min/max value, and probability distribution.
+
+        The ``Attribute`` class has two modes:
+
+        - it has raw data, and then can calculate its pattern from the data;
+
+        - it doesn't have raw data, and only have the pattern from customer.
+
+        Parameters
+        ----------
+        categorical : bool
+            set categorical label for attribute. If categorical, this attribute
+            takes on a limited and fixed number of possible values. Examples:
+            blood type, gender.
+        """
+        categorical = kwargs.pop('categorical', False)
+        # The `categorical` option can be set to true when the attribute is
+        # string-typed and all values are not unique, and its value can be
+        # overridden by user.
+        if categorical or (
+                isinstance(args[0], Series)
+                and args[0].dtype == 'object'
+                and utils.is_discrete_values(args[0])):
+            kwargs.update({'dtype': 'category'})
+            categorical = True
+        super().__init__(*args, **kwargs)
+        self.set_pattern(categorical=categorical)
+
+    def _calculate_pattern(self):
+        from pandas.api.types import infer_dtype
+        self.categorical = self.dtype == 'category'
+        if self.categorical:
+            self._type = infer_dtype(self.cat.categories, skipna=True)
+        else:
+            self._type = infer_dtype(self, skipna=True)
+        if self._type == 'integer':
+            pass
+        elif self._type == 'floating' or self._type == 'mixed-integer-float':
+            self._type = 'float'
+        elif self._type in ['string', 'mixed-integer', 'mixed']:
+            self._type = 'string'
+            if all(map(utils.is_datetime, self._values)):
+                self._type = 'datetime'
+
+        if self.type == 'string' and not self.categorical:
+            # check string categories (when attribute is set from pattern)
+            if utils.is_discrete_values(self):
+                self._update_categories_inplace([])
+                self.categorical = True
+
+        # fill the missing values with the most frequent value
+        if self.hasnans:
+            self.fillna(self.mode()[0], inplace=True)
+
+        # for datetime attribute is converted to seconds since Unix epoch time
+        if self.type == 'datetime':
+            if self.categorical:
+                # re-order datetime categories in below function
+                self._update_categories_inplace([])
+            else:
+                self.update(self.map(self._to_seconds))
+
+        if self.type == 'float':
+            self._decimals = self.decimals()
+
+        self._set_domain()
+        self._set_distribution()
+
+    # handling functions for datetime attribute
+    def _to_seconds(self, timestr):
+        return int((parse(timestr) - self._epoch).total_seconds())
+
+    def _date_formatter(self, seconds):
+        date = self._epoch + timedelta(seconds=seconds)
+        return '%d/%d/%d' % (date.month, date.day, date.year)
+
+    # Take pandas.Series as manipulation result.
+    @property
+    def _constructor(self):
+        return Series
+
+    @property
+    def _constructor_expanddim(self):
+        from ds4ml.dataset import DataSet
+        return DataSet
+
+    def set_pattern(self, pattern=None, **kwargs):
+        """
+        Set an attribute's pattern, including its type, min/max value, and
+        probability distributions.
+        If patter is None, then calculation its pattern from its data.
+        """
+        if not self._pattern_generated:
+            self.categorical = kwargs.pop("categorical", False)
+            if pattern is None:
+                # to calculate the pattern use its data
+                self._calculate_pattern()
+            else:
+                self._type = pattern['type']
+                if self.type == 'float':
+                    self._decimals = pattern['decimals']
+                self.categorical = pattern['categorical']
+                self.min_ = pattern['min']
+                self.max_ = pattern['max']
+                self.bins = np.array(pattern['bins'])
+                self.prs = np.array(pattern['prs'])
+            self._pattern_generated = True
+
+    @property
+    def is_numerical(self):
+        return self._type == 'integer' or self._type == 'float'
+
+    @property
+    def domain(self):
+        """
+        Return attribute's domain, which can be a list of values for categorical
+        attribute, and an interval with min/max value for non-categorical
+        attribute.
+        """
+        if self.categorical:
+            return self.bins
+        return [self.min_, self.max_]
+
+    def _step(self):
+        """ Return step for numerical or datetime attribute. """
+        return (self.max_ - self.min_) / self._bin_size
+
+    def _update_categories_inplace(self, new_categories):
+        if self.categorical:
+            if self._type in ['string', 'datetime']:
+                new_categories = set(new_categories + self.cat.categories.to_list())
+                if self.type == 'datetime':
+                    new_categories = sorted(new_categories, key=self._to_seconds)
+                else:
+                    new_categories = sorted(new_categories)
+            cat = self.cat.set_categories(new_categories)
+            super().__init__(cat, dtype='category')
+        else:
+            new_categories = sorted(set(new_categories + self.dropna().unique().tolist()))
+            series = self.astype('category')
+            cat = series.cat.set_categories(new_categories)
+            super().__init__(cat, dtype='category')
+
+    @domain.setter
+    def domain(self, domain: list):
+        """
+        Set attribute's domain, includes min, max, frequency, or distribution.
+
+        Generally, the domain of one attribute can be calculated automatically.
+        This method can be manually called for specific purposes, e.g. compare
+        two same attributes based on same domain.
+
+        Parameters
+        ----------
+        domain : list
+            domain of one attribute. For numerical or datetime attributes, it
+            should be a list of two elements [min, max]; For categorical
+            attributes, it should a list of potential values of this attribute.
+        """
+        if self.categorical:
+            self._update_categories_inplace(domain)
+
+        # if a attribute is numerical and categorical and domain's length is
+        # bigger than 2, take it as categorical. e.g. zip code.
+        if self.type == 'datetime' and not self.categorical:
+            domain = list(map(self._to_seconds, domain))
+        if (self.is_numerical and self.categorical and len(domain) > 2) or (
+                self.categorical):
+            self.min_, self.max_ = min(domain), max(domain)
+            self.bins = np.array(domain)
+        elif self.is_numerical:
+            self.min_, self.max_ = domain
+            self.bins = np.array([self.min_, self.max_])
+        elif self._type == 'string':
+            lengths = [len(str(i)) for i in domain]
+            self.min_, self.max_ = min(lengths), max(lengths)
+            self.bins = np.array(domain)
+        self._set_distribution()
+
+    def _set_domain(self):
+        """
+        Compute domain (min, max, distribution bins) from input data
+        """
+        if self.categorical:
+            self.bins = self.cat.categories
+
+        if self._type == 'string':
+            items = self.astype(str).map(len)
+            self.min_ = int(items.min())
+            self.max_ = int(items.max())
+            if not self.categorical:
+                self.bins = np.array([self.min_, self.max_])
+        elif self._type == 'datetime':
+            if not self.categorical:
+                self.min_ = float(self.min())
+                self.max_ = float(self.max())
+                self.bins = np.array([self.min_, self.max_])
+        else:
+            if not self.categorical:
+                self.min_ = float(self.min())
+                self.max_ = float(self.max())
+                self.bins = np.array([self.min_, self.max_])
+
+    def _set_distribution(self):
+        if self.categorical:
+            counts = self.value_counts()
+            for value in set(self.bins) - set(counts.index):
+                counts[value] = 0
+            counts.sort_index(inplace=True)
+            # if self.type == 'datetime':
+            #     counts.index = list(map(self._date_formatter, counts.index))
+            self._counts = counts.values
+            self.prs = utils.normalize_distribution(counts)
+            self.bins = np.array(counts.index)
+        else:
+            # Note: hist, edges = numpy.histogram(), all but the last bin
+            # is half-open. If bins is 20, then len(hist)=20, len(edges)=21
+            if self.type == 'string':
+                hist, edges = np.histogram(self.astype(str).map(len),
+                                           bins=self._bin_size)
+            else:
+                hist, edges = np.histogram(self, bins=self._bin_size,
+                                           range=(self.min_, self.max_))
+            self.bins = edges[:-1]  # Remove the last bin edge
+            self._counts = hist
+            self.prs = utils.normalize_distribution(hist)
+            if self.type == 'integer':
+                self.min_ = int(self.min_)
+                self.max_ = int(self.max_)
+
+    def counts(self, bins=None, normalize=True):
+        """
+        Return an array of counts (or normalized density) of unique values.
+
+        This function works with `attribute.bins`. Combination of both are
+        like `Series.value_counts`. The parameter `bins` can be none, or a list.
+        """
+        if bins is None:
+            return self._counts
+        if self.categorical:
+            self._update_categories_inplace(bins)
+
+            # if self.type == 'datetime':
+            #     bins = list(map(self._to_seconds, bins))
+            counts = self.value_counts()
+            for value in set(bins) - set(counts.index):
+                counts[value] = 0
+            if normalize:
+                return np.array([round(counts.get(b)/sum(counts) * 100, 2)
+                                 for b in bins])
+            return np.array([counts.get(b) for b in bins])
+
+        if len(bins) == 1:
+            return np.array([self.size])
+        hist, _ = np.histogram(self, bins=bins)
+        if normalize:
+            return (hist / hist.sum() * 100).round(2)
+        return hist
+
+    def bin_indexes(self):
+        """
+        Encode values into bin indexes for Bayesian Network.
+        """
+        if self.categorical:
+            # mapping = {value: idx for idx, value in enumerate(self.bins)}
+            # indexes = self.map(lambda x: mapping[x], na_action='ignore')
+            indexes = Series(self.cat.codes)
+        else:
+            indexes = self.map(lambda x: bisect_right(self.bins, x) - 1,
+                               na_action='ignore')
+        indexes.fillna(len(self.bins), inplace=True)
+        return indexes.astype(int, copy=False)
+
+    def to_pattern(self):
+        """
+        Return attribution's metadata information in JSON format or Python
+        dictionary. Usually used in debug and testing.
+        """
+        return {
+            'name': self.name,
+            'type': self._type,
+            'categorical': self.categorical,
+            'min': self.min_,
+            'max': self.max_,
+            'decimals': self._decimals if self.type == 'float' else None,
+            'bins': self.bins.tolist(),
+            'prs': self.prs.tolist()
+        }
+
+    def decimals(self):
+        """
+        Returns number of decimals places for floating attribute. Used for
+        generated dataset to keep consistent decimal places for float attribute.
+        """
+        def decimals_of(value: float):
+            value = str(value)
+            return len(value) - value.rindex('.') - 1
+
+        counts = self.map(decimals_of).value_counts()
+        slot = 0
+        for i in range(len(counts)):
+            if sum(counts.head(i + 1)) / sum(counts) > 0.8:
+                slot = i + 1
+                break
+        return max(counts.index[:slot])
+
+    def pseudonymize(self, size=None):
+        """
+        Return pseudonymized values for this attribute, which is used to
+        substitute identifiable data with a reversible, consistent value.
+        """
+        size = size or self.size
+        if size != self.size:
+            attr = Series(np.random.choice(self.bins, size=size, p=self.prs))
+        else:
+            attr = self
+        if self.categorical:
+            mapping = {b: utils.pseudonymise_string(b) for b in self.bins}
+            return attr.map(lambda x: mapping[x])
+
+        if self.type == 'string':
+            return attr.map(utils.pseudonymise_string)
+        elif self.is_numerical or self.type == 'datetime':
+            return attr.map(str).map(utils.pseudonymise_string)
+
+    def random(self, size=None):
+        """
+        Return an random array with same length (usually used for
+        non-categorical attribute).
+        """
+        size = size or self.size
+        if self.min_ == self.max_:
+            rands = np.ones(size) * self.min_
+        else:
+            rands = np.arange(self.min_, self.max_, (self.max_-self.min_)/size)
+
+        np.random.shuffle(rands)
+        if self.type == 'string':
+            if self.min_ == self.max_:
+                length = self.min_
+            else:
+                length = np.random.randint(self.min_, self.max_)
+            vectorized = np.vectorize(lambda x: utils.randomize_string(length))
+            rands = vectorized(rands)
+        elif self.type == 'integer':
+            rands = list(map(int, rands))
+        elif self.type == 'datetime':
+            rands = list(map(self._date_formatter, rands))
+        return Series(rands)
+
+    def retain(self, size=None):
+        """ Return retained attribute with the size """
+        size = size or self.size
+        if size < self.size:
+            return self.head(size)
+        if size == self.size:
+            return self
+        copies = size // self.size
+        remainder = size - (copies * self.size)
+
+        return Series(self.tolist() * copies + self.head(remainder).tolist())
+
+    def _random_sample_at(self, index: int):
+        """ Sample a value from distribution bins at position 'index'"""
+        if self.categorical:
+            return self.bins[index]
+
+        length = len(self.bins)
+        if index < length - 1:
+            return uniform(self.bins[index], self.bins[index + 1])
+        return uniform(self.bins[-1], self.max_)
+
+    def choice(self, size=None, indexes=None):
+        """
+        Return a random sample based on this attribute's probability and
+        distribution bins (default value is base random distribution bins based
+        on its probability).
+
+        Parameters
+        ----------
+        size : int
+            size of random sample
+
+        indexes : array-like
+            array of indexes in distribution bins
+        """
+        if indexes is None:
+            size = size or self.size
+            indexes = Series(np.random.choice(len(self.prs),
+                                              size=size, p=self.prs))
+        column = indexes.map(self._random_sample_at)
+        if self.type == 'datetime':
+            if not self.categorical:
+                column = column.map(self._date_formatter)
+        elif self.type == 'float':
+            column = column.round(self._decimals)
+        elif self.type == 'integer':
+            column = column.round().astype(int)
+        elif self.type == 'string':
+            if not self.categorical:
+                column = column.map(lambda x: utils.randomize_string(int(x)))
+        return column
+
+    def encode(self, data=None):
+        """
+        Encode labels to normalized encoding.
+
+        Parameters
+        ----------
+        data : array-like
+            target values
+        """
+        if data is None:
+            data = self.copy()
+        else:
+            if self.type == 'datetime':
+                if all(map(utils.is_datetime, data)):
+                    data = data.map(self._to_seconds)
+                else:
+                    data = data.map(int)
+
+        if self.categorical:
+            frame = DataFrame()
+            for col in self.bins:
+                frame[col] = data.apply(lambda v: 1 if v == col else 0)
+            return frame
+
+        if self.type != 'string':
+            step = self._step()
+            return data.apply(lambda v:  # 1e-8 is a small delta
+                              int((v - self.min_) / (step + 1e-8))
+                              / self._bin_size)
+        raise ValueError('Can\'t encode Non-categorical attribute.')
```

### Comparing `ds4ml-0.3.4/ds4ml/command/pattern.py` & `ds4ml-0.3.5/ds4ml/command/pattern.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-"""
-pattern.py
-
-"""
-
-from ds4ml.dataset import DataSet
-from ds4ml.utils import CustomFormatter, read_data_from_csv, file_name, str_to_list
-
-import argparse
-import time
-
-
-def main():
-    parser = argparse.ArgumentParser(
-        description='Serialize patterns of a dataset anonymously',
-        formatter_class=CustomFormatter,
-        add_help=False)
-    parser.add_argument('file', help='set path of a csv file to be patterned '
-                                     'anonymously')
-
-    # optional arguments
-    group = parser.add_argument_group('general arguments')
-    group.add_argument("-h", "--help", action="help",
-                       help="show this help message and exit")
-    group.add_argument('--pseudonym', metavar='LIST',
-                       help='set candidate columns separated by a comma, which '
-                            'will be replaced with a pseudonym. It only works '
-                            'on the string column.')
-    group.add_argument('--delete', metavar='LIST',
-                       help='set columns separated by a comma, which will be '
-                            'deleted when synthesis.')
-    group.add_argument('--na-values', metavar='LIST',
-                       help='set additional values to recognize as NA/NaN; '
-                            '(default null values are from pandas.read_csv)')
-    group.add_argument('-o', '--output', metavar='FILE',
-                       help="set the file name of anonymous patterns (default "
-                            "is input file name with a suffix '-pattern.json')")
-    group.add_argument('--no-header', action='store_true',
-                       help='indicate there is no header in a CSV file, and '
-                            'will take [#0, #1, #2, ...] as header. (default: '
-                            'the tool will try to detect and take actions)')
-    group.add_argument('--sep', metavar='STRING',
-                       help='specify the delimiter of the input file')
-
-    group = parser.add_argument_group('advanced arguments')
-    group.add_argument('-e', '--epsilon', metavar='FLOAT', type=float,
-                       help='set epsilon for differential privacy (default 0.1)',
-                       default=0.1)
-    group.add_argument('--category', metavar='LIST',
-                       help='set categorical columns separated by a comma.')
-
-    args = parser.parse_args()
-    start = time.time()
-
-    pseudonyms = str_to_list(args.pseudonym)
-    deletes = str_to_list(args.delete)
-    categories = str_to_list(args.category)
-    na_values = str_to_list(args.na_values)
-    header = None if args.no_header else 'infer'
-    sep = ',' if args.sep is None else args.sep
-
-    data = read_data_from_csv(args.file, na_values=na_values, header=header,
-                              sep=sep)
-
-    def complement(attrs, full):
-        return set(attrs or []) - set(full)
-
-    # check parameters: pseudonyms, deletes, categories
-    comp = complement(pseudonyms, data.columns)
-    if comp:
-        parser.exit(message=f'--pseudonym columns: {comp} are not in csv file.')
-    comp = complement(deletes, data.columns)
-    if comp:
-        parser.exit(message=f'--delete columns: {comp} are not in csv file.')
-    comp = complement(categories, data.columns)
-    if comp:
-        parser.exit(message=f'--category columns: {comp} are not in csv file.')
-
-    dataset = DataSet(data, categories=categories)
-
-    if args.output is None:
-        name = file_name(args.file)
-        args.output = f'{name}-pattern.json'
-    dataset.to_pattern_file(path=args.output, epsilon=args.epsilon,
-                            deletes=deletes, pseudonyms=pseudonyms, retains=[])
-
-    duration = time.time() - start
-    print(f'Analyze and serialize the patterns of {args.file} at {args.output} '
-          f'in {round(duration, 2)} seconds.')
-
-
-if __name__ == '__main__':
-    main()
+"""
+pattern.py
+
+"""
+
+from ds4ml.dataset import DataSet
+from ds4ml.utils import CustomFormatter, read_data_from_csv, file_name, str_to_list
+
+import argparse
+import time
+
+
+def main():
+    parser = argparse.ArgumentParser(
+        description='Serialize patterns of a dataset anonymously',
+        formatter_class=CustomFormatter,
+        add_help=False)
+    parser.add_argument('file', help='set path of a csv file to be patterned '
+                                     'anonymously')
+
+    # optional arguments
+    group = parser.add_argument_group('general arguments')
+    group.add_argument("-h", "--help", action="help",
+                       help="show this help message and exit")
+    group.add_argument('--pseudonym', metavar='LIST',
+                       help='set candidate columns separated by a comma, which '
+                            'will be replaced with a pseudonym. It only works '
+                            'on the string column.')
+    group.add_argument('--delete', metavar='LIST',
+                       help='set columns separated by a comma, which will be '
+                            'deleted when synthesis.')
+    group.add_argument('--na-values', metavar='LIST',
+                       help='set additional values to recognize as NA/NaN; '
+                            '(default null values are from pandas.read_csv)')
+    group.add_argument('-o', '--output', metavar='FILE',
+                       help="set the file name of anonymous patterns (default "
+                            "is input file name with a suffix '-pattern.json')")
+    group.add_argument('--no-header', action='store_true',
+                       help='indicate there is no header in a CSV file, and '
+                            'will take [#0, #1, #2, ...] as header. (default: '
+                            'the tool will try to detect and take actions)')
+    group.add_argument('--sep', metavar='STRING',
+                       help='specify the delimiter of the input file')
+
+    group = parser.add_argument_group('advanced arguments')
+    group.add_argument('-e', '--epsilon', metavar='FLOAT', type=float,
+                       help='set epsilon for differential privacy (default 0.1)',
+                       default=0.1)
+    group.add_argument('--category', metavar='LIST',
+                       help='set categorical columns separated by a comma.')
+
+    args = parser.parse_args()
+    start = time.time()
+
+    pseudonyms = str_to_list(args.pseudonym)
+    deletes = str_to_list(args.delete)
+    categories = str_to_list(args.category)
+    na_values = str_to_list(args.na_values)
+    header = None if args.no_header else 'infer'
+    sep = ',' if args.sep is None else args.sep
+
+    data = read_data_from_csv(args.file, na_values=na_values, header=header,
+                              sep=sep)
+
+    def complement(attrs, full):
+        return set(attrs or []) - set(full)
+
+    # check parameters: pseudonyms, deletes, categories
+    comp = complement(pseudonyms, data.columns)
+    if comp:
+        parser.exit(message=f'--pseudonym columns: {comp} are not in csv file.')
+    comp = complement(deletes, data.columns)
+    if comp:
+        parser.exit(message=f'--delete columns: {comp} are not in csv file.')
+    comp = complement(categories, data.columns)
+    if comp:
+        parser.exit(message=f'--category columns: {comp} are not in csv file.')
+
+    dataset = DataSet(data, categories=categories)
+
+    if args.output is None:
+        name = file_name(args.file)
+        args.output = f'{name}-pattern.json'
+    dataset.to_pattern_file(path=args.output, epsilon=args.epsilon,
+                            deletes=deletes, pseudonyms=pseudonyms, retains=[])
+
+    duration = time.time() - start
+    print(f'Analyze and serialize the patterns of {args.file} at {args.output} '
+          f'in {round(duration, 2)} seconds.')
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `ds4ml-0.3.4/ds4ml/command/synthesize.py` & `ds4ml-0.3.5/ds4ml/command/synthesize.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-"""ds4ml.command.synthesize
-
-Provides the command line to synthesize a dataset directly (e.g. csv file) or
-from a pattern file which describes the dataset anonymously (and which can be
-got through command `data-pattern`).
-
-"""
-
-from ds4ml.dataset import DataSet
-from ds4ml.utils import (CustomFormatter, read_data_from_csv, file_name,
-                         str_to_list, ends_with_json)
-
-import argparse
-import time
-
-
-def main():
-    parser = argparse.ArgumentParser(
-        description='Synthesize one dataset by differential privacy',
-        formatter_class=CustomFormatter,
-        add_help=False)
-    parser.add_argument('file', help='set path of a csv file to be synthesized '
-                                     'or path of a pattern file to be generated')
-
-    # optional arguments
-    group = parser.add_argument_group('general arguments')
-    group.add_argument("-h", "--help", action="help",
-                       help="show this help message and exit")
-    group.add_argument('--pseudonym', metavar='LIST',
-                       help='set candidate columns separated by a comma, which '
-                            'will be replaced with a pseudonym. It only works '
-                            'on the string column.')
-    group.add_argument('--delete', metavar='LIST',
-                       help='set columns separated by a comma, which will be '
-                            'deleted when synthesis.')
-    group.add_argument('--na-values', metavar='LIST',
-                       help='set additional values to recognize as NA/NaN; '
-                            '(default null values are from pandas.read_csv)')
-    group.add_argument('-o', '--output', metavar='FILE',
-                       help="set the file name of output synthesized dataset ("
-                            "default is input file name with suffix '-a.csv')")
-    group.add_argument('--no-header', action='store_true',
-                       help='indicate there is no header in a CSV file, and '
-                            'will take [#0, #1, #2, ...] as header. (default: '
-                            'the tool will try to detect and take actions)')
-    group.add_argument('--records', metavar='INT', type=int,
-                       help='specify the records you want to generate; default '
-                            'is the same records with the original dataset')
-    group.add_argument('--sep', metavar='STRING', default=',',
-                       help='specify the delimiter of the input file')
-
-    group = parser.add_argument_group('advanced arguments')
-    group.add_argument('-e', '--epsilon', metavar='FLOAT', type=float,
-                       help='set epsilon for differential privacy (default 0.1)',
-                       default=0.1)
-    group.add_argument('--category', metavar='LIST',
-                       help='set categorical columns separated by a comma.')
-    group.add_argument('--retain', metavar='LIST',
-                       help='set columns to retain the values')
-
-    args = parser.parse_args()
-    start = time.time()
-
-    pseudonyms = str_to_list(args.pseudonym)
-    deletes = str_to_list(args.delete)
-    categories = str_to_list(args.category)
-    na_values = str_to_list(args.na_values)
-    retains = str_to_list(args.retain)
-    header = None if args.no_header else 'infer'
-
-    # check the file type from its extension
-    is_pattern = ends_with_json(args.file)
-    if is_pattern:
-        if retains is not None and len(retains) != 0:
-            parser.exit(message='Do not support --retain option when '
-                                'synthesize from pattern file.')
-        # construct DataSet from pattern file
-        dataset = DataSet.from_pattern(args.file)
-    else:
-        data = read_data_from_csv(args.file, na_values=na_values, header=header,
-                                  sep=args.sep)
-
-        def complement(attrs, full):
-            return set(attrs or []) - set(full)
-
-        # check parameters: pseudonyms, deletes, categories
-        comp = complement(pseudonyms, data.columns)
-        if comp:
-            parser.exit(
-                message=f'--pseudonym columns: {comp} are not in csv file.')
-        comp = complement(deletes, data.columns)
-        if comp:
-            parser.exit(
-                message=f'--delete columns: {comp} are not in csv file.')
-        comp = complement(categories, data.columns)
-        if comp:
-            parser.exit(
-                message=f'--category columns: {comp} are not in csv file.')
-
-        dataset = DataSet(data, categories=categories)
-
-    synthesized = dataset.synthesize(epsilon=args.epsilon,
-                                     pseudonyms=pseudonyms, deletes=deletes,
-                                     retains=retains, records=args.records)
-    if args.output is None:
-        name = file_name(args.file)
-        args.output = f'{name}-a.csv'
-    synthesized.to_csv(args.output, index=False, sep=args.sep)
-
-    duration = time.time() - start
-    print(f'Synthesize from {args.file} to file {args.output} in '
-          f'{round(duration, 2)} seconds.')
-
-
-if __name__ == '__main__':
-    main()
+"""ds4ml.command.synthesize
+
+Provides the command line to synthesize a dataset directly (e.g. csv file) or
+from a pattern file which describes the dataset anonymously (and which can be
+got through command `data-pattern`).
+
+"""
+
+from ds4ml.dataset import DataSet
+from ds4ml.utils import (CustomFormatter, read_data_from_csv, file_name,
+                         str_to_list, ends_with_json)
+
+import argparse
+import time
+
+
+def main():
+    parser = argparse.ArgumentParser(
+        description='Synthesize one dataset by differential privacy',
+        formatter_class=CustomFormatter,
+        add_help=False)
+    parser.add_argument('file', help='set path of a csv file to be synthesized '
+                                     'or path of a pattern file to be generated')
+
+    # optional arguments
+    group = parser.add_argument_group('general arguments')
+    group.add_argument("-h", "--help", action="help",
+                       help="show this help message and exit")
+    group.add_argument('--pseudonym', metavar='LIST',
+                       help='set candidate columns separated by a comma, which '
+                            'will be replaced with a pseudonym. It only works '
+                            'on the string column.')
+    group.add_argument('--delete', metavar='LIST',
+                       help='set columns separated by a comma, which will be '
+                            'deleted when synthesis.')
+    group.add_argument('--na-values', metavar='LIST',
+                       help='set additional values to recognize as NA/NaN; '
+                            '(default null values are from pandas.read_csv)')
+    group.add_argument('-o', '--output', metavar='FILE',
+                       help="set the file name of output synthesized dataset ("
+                            "default is input file name with suffix '-a.csv')")
+    group.add_argument('--no-header', action='store_true',
+                       help='indicate there is no header in a CSV file, and '
+                            'will take [#0, #1, #2, ...] as header. (default: '
+                            'the tool will try to detect and take actions)')
+    group.add_argument('--records', metavar='INT', type=int,
+                       help='specify the records you want to generate; default '
+                            'is the same records with the original dataset')
+    group.add_argument('--sep', metavar='STRING', default=',',
+                       help='specify the delimiter of the input file')
+
+    group = parser.add_argument_group('advanced arguments')
+    group.add_argument('-e', '--epsilon', metavar='FLOAT', type=float,
+                       help='set epsilon for differential privacy (default 0.1)',
+                       default=0.1)
+    group.add_argument('--category', metavar='LIST',
+                       help='set categorical columns separated by a comma.')
+    group.add_argument('--retain', metavar='LIST',
+                       help='set columns to retain the values')
+
+    args = parser.parse_args()
+    start = time.time()
+
+    pseudonyms = str_to_list(args.pseudonym)
+    deletes = str_to_list(args.delete)
+    categories = str_to_list(args.category)
+    na_values = str_to_list(args.na_values)
+    retains = str_to_list(args.retain)
+    header = None if args.no_header else 'infer'
+
+    # check the file type from its extension
+    is_pattern = ends_with_json(args.file)
+    if is_pattern:
+        if retains is not None and len(retains) != 0:
+            parser.exit(message='Do not support --retain option when '
+                                'synthesize from pattern file.')
+        # construct DataSet from pattern file
+        dataset = DataSet.from_pattern(args.file)
+    else:
+        data = read_data_from_csv(args.file, na_values=na_values, header=header,
+                                  sep=args.sep)
+
+        def complement(attrs, full):
+            return set(attrs or []) - set(full)
+
+        # check parameters: pseudonyms, deletes, categories
+        comp = complement(pseudonyms, data.columns)
+        if comp:
+            parser.exit(
+                message=f'--pseudonym columns: {comp} are not in csv file.')
+        comp = complement(deletes, data.columns)
+        if comp:
+            parser.exit(
+                message=f'--delete columns: {comp} are not in csv file.')
+        comp = complement(categories, data.columns)
+        if comp:
+            parser.exit(
+                message=f'--category columns: {comp} are not in csv file.')
+
+        dataset = DataSet(data, categories=categories)
+
+    synthesized = dataset.synthesize(epsilon=args.epsilon,
+                                     pseudonyms=pseudonyms, deletes=deletes,
+                                     retains=retains, records=args.records)
+    if args.output is None:
+        name = file_name(args.file)
+        args.output = f'{name}-a.csv'
+    synthesized.to_csv(args.output, index=False, sep=args.sep)
+
+    duration = time.time() - start
+    print(f'Synthesize from {args.file} to file {args.output} in '
+          f'{round(duration, 2)} seconds.')
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `ds4ml-0.3.4/ds4ml/dataset.py` & `ds4ml-0.3.5/ds4ml/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,284 +1,294 @@
-"""
-DataSet: data structure for potentially mixed-type Attribute.
-"""
-
-import json
-
-from pandas import DataFrame, Series
-
-from ds4ml.attribute import Attribute
-from ds4ml.synthesizer import greedy_bayes, noisy_conditionals, noisy_distributions
-from ds4ml.utils import normalize_distribution
-
-
-class DataSetPattern:
-    """
-    A helper class of ``DataSet`` to store its patterns.
-    """
-    # DataSet's pattern data has the following members:
-    _network = None
-    _cond_prs = None
-    _attrs = None
-    _records = None
-
-    # Options of DataSet constructor to preset some properties:
-    _categories = []    # categorical columns setting from command lines
-    _config = None      # configurations for data-pattern command
-    _pattern_generated = False
-
-
-class DataSet(DataSetPattern, DataFrame):
-
-    def __init__(self, *args, **kwargs):
-        """
-        An improved DataFrame with extra patterns information, e.g. its bayesian
-        network structure, conditional probabilities on the network, and pattern
-        information of all its columns.
-
-        The ``DataSet`` class has two modes:
-
-        - it has raw data, and then can calculate its pattern from the data;
-
-        - it doesn't have raw data, and only have the pattern from customer.
-
-        Parameters
-        ----------
-        categories : list of columns (optional)
-            Column names whose values are categorical.
-        """
-        categories = kwargs.pop("categories", [])
-        self._categories = [] if categories is None else categories
-        pattern = kwargs.pop('pattern', None)
-        super(DataSet, self).__init__(*args, **kwargs)
-        self.separator = '_'
-        if pattern is not None and all(k in pattern for k in
-                                       ['network', 'prs', 'attrs', 'records']):
-            self._set_pattern(pattern)
-        else:
-            self._records = self.shape[0]
-
-    @property
-    def _constructor(self):
-        return DataSet
-
-    # disable _constructor_sliced method for single column slicing. Try to
-    # use __getitem__ method.
-    # @property
-    # def _constructor_sliced(self):
-    #     return Attribute
-
-    def __getitem__(self, key):
-        result = super(DataSet, self).__getitem__(key)
-        if isinstance(result, Series):
-            result.__class__ = Attribute
-            if self._attrs is not None:
-                result.set_pattern(self._attrs.get(key),
-                                   categorical=key in self._categories)
-            else:
-                result.set_pattern(categorical=key in self._categories)
-        return result
-
-    @classmethod
-    def from_pattern(cls, pattern: dict):
-        """
-        Alternate constructor to create a ``DataSet`` from a pattern file.
-        """
-        # set columns to DataSet, which will set column name to each Attribute.
-        columns = pattern['attrs'].keys()
-        dataset = DataSet(columns=columns, pattern=pattern)
-        return dataset
-
-    @classmethod
-    def from_pattern_file(cls, filename):
-        with open(filename) as f:
-            pattern = json.load(f)
-        return cls.from_pattern(pattern)
-
-    def _set_pattern(self, pattern=None):
-        """ Set pattern data for the DataSet. """
-        if not self._pattern_generated:
-            self._network = pattern['network']
-            self._cond_prs = pattern['prs']
-            self._attrs = pattern['attrs']
-            self._config = pattern['config']
-            self._records = pattern['records']
-            self._pattern_generated = True
-
-    def mi(self):
-        """ Return mutual information of pairwise attributes. """
-        from ds4ml.metrics import pairwise_mutual_information
-        return pairwise_mutual_information(self)
-
-    def encode(self, data=None):
-        """
-        Transform data set to values by kinds of encoders.
-        If data is set, use this data set's encoders to transform.
-        """
-        # If the data to encode is None, then transform source data _data;
-        frame = DataFrame()
-        for col in self.columns:
-            attr = self[col]
-            if data is not None and col not in data:
-                continue
-            # when attribute is string-typed but not categorical, ignore its
-            # encode method.
-            if attr.categorical:
-                subs = attr.encode(None if data is None else data[col])
-                for label in attr.bins:
-                    frame[col + self.separator + str(label)] = subs[label]
-            elif attr.type != 'string':
-                frame[col] = attr.encode(None if data is None else data[col])
-        return frame
-
-    def _sampling_dataset(self, network, cond_prs, n):
-        """
-        Returns a sampling dataset (n rows) based on bayesian network and
-        conditional probability.
-        """
-        from numpy import random
-        root_col = network[0][1][0]
-        root_prs = cond_prs[root_col]
-
-        columns = [root_col]  # columns from bayesian network
-        for node, _ in network:
-            columns.append(node)
-
-        frame = DataFrame(columns=columns)  # encoded DataFrame
-        frame[root_col] = random.choice(len(root_prs), size=n, p=root_prs)
-
-        for child, parents in network:
-            child_cond_prs = cond_prs[child]
-            for indexes in child_cond_prs.keys():
-                prs = child_cond_prs[indexes]
-                indexes = list(eval(indexes))
-
-                df = frame
-                for parent, value in zip(parents, indexes):
-                    df = df[df[parent] == value]
-                if df.size:
-                    frame.loc[df.index, child] = random.choice(
-                        len(prs), size=df.index.size, p=prs)
-            child_prs = self[child].prs
-            frame.loc[frame[child].isnull(), child] = random.choice(
-                len(child_prs), size=frame[child].isnull().sum(), p=child_prs)
-        frame[frame.columns] = frame[frame.columns].astype(int)
-        return frame
-
-    def _construct_bayesian_network(self, epsilon=0.1, degree=2,
-                                    pseudonyms=None, deletes=None, retains=None):
-        """
-        Construct bayesian network of the DataSet.
-        """
-        deletes = deletes or []
-        pseudonyms = pseudonyms or []
-        retains = retains or []
-
-        columns = [col for col in self.columns.values if col not in deletes]
-        # nodes for bayesian networks, which does not include pseudonym columns
-        # or non-categorical string columns.
-        nodes = set()
-        for col in columns:
-            if col in pseudonyms or (
-                    self[col].type == 'string' and not self[col].categorical):
-                continue
-            nodes.add(col)
-        # main steps of private bayesian network for synthesis
-        # encode dataset into bin indexes for bayesian network
-        indexes = DataFrame()
-        for col in nodes:
-            indexes[col] = self[col].bin_indexes()
-        if indexes.shape[1] < 2:
-            print('Warning: when there is only one attribute in dataset, this '
-                  'algorithm inject noises to its probability distribution.')
-            _cols = list(indexes)
-            prs = noisy_distributions(indexes, _cols, epsilon)
-            probability = {_cols[0]: normalize_distribution(prs['freq']).tolist()}
-            return None, probability
-
-        # Bayesian network is defined as a set of AP (attribute-parent) pairs.
-        # e.g. [(x1, p1), (x2, p2), ...], and pi is the parents of xi.
-        #
-        # The algorithm follows the composability property of differential
-        # privacy, so the privacy budget is split to two parts.
-        network = greedy_bayes(indexes, epsilon / 2, degree=degree,
-                               retains=retains)
-        cond_prs = noisy_conditionals(network, indexes, epsilon / 2)
-        return network, cond_prs
-
-    def to_pattern(self, epsilon=0.1, degree=2, pseudonyms=None,
-                   deletes=None, retains=None) -> dict:
-        """
-        Serialize this dataset's patterns into a dict object.
-        """
-        network, cond_prs = self._construct_bayesian_network(
-            epsilon, degree=degree, pseudonyms=pseudonyms, deletes=deletes,
-            retains=retains)
-        pattern = dict({
-            "attrs": {col: self[col].to_pattern() for col in self.columns
-                      if col not in (deletes or [])},
-            "config": {"pseudonyms": pseudonyms},
-            "network": network,
-            "prs": cond_prs,
-            "records": self._records
-        })
-        return pattern
-
-    def to_pattern_file(self, path, epsilon=0.1, degree=2, pseudonyms=None,
-                        deletes=None, retains=None) -> None:
-        """
-        Serialize this dataset's patterns into a json file.
-        """
-        pattern = self.to_pattern(epsilon, degree, pseudonyms, deletes, retains)
-        with open(path, 'w') as fp:
-            json.dump(pattern, fp, indent=2)
-
-    def synthesize(self, epsilon=0.1, degree=2,
-                   pseudonyms=None, deletes=None, retains=None, records=None):
-        """
-        Synthesize data set by a bayesian network to infer attributes'
-        dependence relationship and differential privacy to keep differentially
-        private.
-        """
-        deletes = deletes or []
-        pseudonyms = pseudonyms or (
-                self._config is not None and self._config['pseudonyms']) or []
-        retains = retains or []
-        records = records if records is not None else self._records
-
-        if self._network is None and self._cond_prs is None:
-            self._network, self._cond_prs = self._construct_bayesian_network(
-                epsilon, degree=degree, pseudonyms=pseudonyms, deletes=deletes,
-                retains=retains)
-
-        # if bayesian network is None, and probability is not None, that means
-        # there is only one column in the dataset.
-        if self._network is None and self._cond_prs is not None:
-            # this is the only column label in this dataset
-            col = self.columns[0]
-            prs = self._cond_prs[col]
-            from numpy import random
-            sampling = Series(random.choice(len(prs), size=records, p=prs))
-            attr = self[col].choice(indexes=sampling)
-            return DataFrame(attr, columns=self.columns)
-
-        columns = [col for col in self.columns.values if col not in deletes]
-        sampling = self._sampling_dataset(self._network, self._cond_prs, records)
-        frame = DataFrame(columns=columns)
-        for col in self.columns:
-            attr = self[col]
-            if col in deletes:
-                continue
-            if col in pseudonyms:  # pseudonym column is not in bayesian network
-                frame[col] = attr.pseudonymize(size=records)
-                continue
-            if col in retains:
-                frame[col] = attr.retain(records)
-                continue
-            if col in sampling:
-                frame[col] = attr.choice(indexes=sampling[col])
-                continue
-            if not attr.categorical:
-                frame[col] = attr.random()
-            else:
-                frame[col] = attr.choice()
-        return frame
+"""
+DataSet: data structure for potentially mixed-type Attribute.
+"""
+
+import json
+
+from pandas import DataFrame, Series
+
+from ds4ml.attribute import Attribute
+from ds4ml.synthesizer import greedy_bayes, noisy_conditionals, noisy_distributions
+from ds4ml.utils import FREQ_NAME, normalize_distribution
+
+
+class DataSetPattern:
+    """
+    A helper class of ``DataSet`` to store its patterns.
+    """
+    # DataSet's pattern data has the following members:
+    _network = None
+    _cond_prs = None
+    _attrs = None
+    _records = None
+
+    # Options of DataSet constructor to preset some properties:
+    _categories = []    # categorical columns setting from command lines
+    _config = None      # configurations for data-pattern command
+    _pattern_generated = False
+
+
+class DataSet(DataSetPattern, DataFrame):
+
+    def __init__(self, *args, **kwargs):
+        """
+        An improved DataFrame with extra patterns information, e.g. its bayesian
+        network structure, conditional probabilities on the network, and pattern
+        information of all its columns.
+
+        The ``DataSet`` class has two modes:
+
+        - it has raw data, and then can calculate its pattern from the data;
+
+        - it doesn't have raw data, and only have the pattern from customer.
+
+        Parameters
+        ----------
+        categories : list of columns (optional)
+            Column names whose values are categorical.
+        """
+        categories = kwargs.pop("categories", [])
+        self._categories = [] if categories is None else categories
+        pattern = kwargs.pop('pattern', None)
+        super(DataSet, self).__init__(*args, **kwargs)
+        self.separator = '_'
+        if pattern is not None and all(k in pattern for k in
+                                       ['network', 'prs', 'attrs', 'records']):
+            self._set_pattern(pattern)
+        else:
+            self._records = self.shape[0]
+
+    @property
+    def _constructor(self):
+        return DataSet
+
+    # disable _constructor_sliced method for single column slicing. Try to
+    # use __getitem__ method.
+    # @property
+    # def _constructor_sliced(self):
+    #     return Attribute
+
+    def __getitem__(self, key):
+        result = super(DataSet, self).__getitem__(key)
+        if isinstance(result, Series):
+            result.__class__ = Attribute
+            if self._attrs is not None:
+                result.set_pattern(self._attrs.get(key),
+                                   categorical=key in self._categories)
+            else:
+                result.set_pattern(categorical=key in self._categories)
+        return result
+
+    @classmethod
+    def from_pattern(cls, pattern: dict):
+        """
+        Alternate constructor to create a ``DataSet`` from a pattern file.
+        """
+        # set columns to DataSet, which will set column name to each Attribute.
+        columns = pattern['attrs'].keys()
+        dataset = DataSet(columns=columns, pattern=pattern)
+        return dataset
+
+    @classmethod
+    def from_pattern_file(cls, filename):
+        with open(filename) as f:
+            pattern = json.load(f)
+        return cls.from_pattern(pattern)
+
+    def _set_pattern(self, pattern=None):
+        """ Set pattern data for the DataSet. """
+        if not self._pattern_generated:
+            self._network = pattern['network']
+            self._cond_prs = pattern['prs']
+            self._attrs = pattern['attrs']
+            self._config = pattern['config']
+            self._records = pattern['records']
+            self._pattern_generated = True
+
+    def mi(self):
+        """ Return mutual information of pairwise attributes. """
+        from ds4ml.metrics import pairwise_mutual_information
+        return pairwise_mutual_information(self)
+
+    def encode(self, data=None):
+        """
+        Transform data set to values by kinds of encoders.
+        If data is set, use this data set's encoders to transform.
+        """
+        # If the data to encode is None, then transform source data _data;
+        frame = DataFrame()
+        for col in self.columns:
+            attr = self[col]
+            if data is not None and col not in data:
+                continue
+            # when attribute is string-typed but not categorical, ignore its
+            # encode method.
+            if attr.categorical:
+                subs = attr.encode(None if data is None else data[col])
+                for label in attr.bins:
+                    frame[col + self.separator + str(label)] = subs[label]
+            elif attr.type != 'string':
+                frame[col] = attr.encode(None if data is None else data[col])
+        return frame
+
+    def _sampling_dataset(self, network, cond_prs, n):
+        """
+        Returns a sampling dataset (n rows) based on bayesian network and
+        conditional probability.
+        """
+        from numpy import random
+
+        root_col = network[0][1][0]
+        root_prs = cond_prs[root_col]
+        columns = [root_col]  # columns from bayesian network
+
+        for node, _ in network:
+            columns.append(node)
+
+        frame = DataFrame(columns=columns)  # encoded DataFrame
+        frame[root_col] = random.choice(len(root_prs), size=n, p=root_prs)
+
+        for child, parents in network:
+            if len(parents) == 0 or (
+                    # for backward compatibility
+                    len(parents) == 1 and parents[0] not in cond_prs):
+                root = child if len(parents) == 0 else parents[0]
+                root_prs = cond_prs[root]
+                frame[root] = random.choice(len(root_prs), size=n, p=root_prs)
+                if len(parents) == 0:
+                    continue
+
+            child_cond_prs = cond_prs[child]
+            for indexes in child_cond_prs.keys():
+                prs = child_cond_prs[indexes]
+                indexes = list(eval(indexes))
+
+                df = frame
+                for parent, value in zip(parents, indexes):
+                    df = df[df[parent] == value]
+                if df.size:
+                    frame.loc[df.index, child] = random.choice(
+                        len(prs), size=df.index.size, p=prs)
+            child_prs = self[child].prs
+            frame.loc[frame[child].isnull(), child] = random.choice(
+                len(child_prs), size=frame[child].isnull().sum(), p=child_prs)
+        frame[frame.columns] = frame[frame.columns].astype(int)
+        return frame
+
+    def _construct_bayesian_network(self, epsilon=0.1, degree=2,
+                                    pseudonyms=None, deletes=None, retains=None):
+        """
+        Construct bayesian network of the DataSet.
+        """
+        deletes = deletes or []
+        pseudonyms = pseudonyms or []
+        retains = retains or []
+
+        columns = [col for col in self.columns.values if col not in deletes]
+        # nodes for bayesian networks, which does not include pseudonym columns
+        # or non-categorical string columns.
+        nodes = set()
+        for col in columns:
+            if col in pseudonyms or (
+                    self[col].type == 'string' and not self[col].categorical):
+                continue
+            nodes.add(col)
+        # main steps of private bayesian network for synthesis
+        # encode dataset into bin indexes for bayesian network
+        indexes = DataFrame()
+        for col in nodes:
+            indexes[col] = self[col].bin_indexes()
+        if indexes.shape[1] < 2:
+            print('Warning: when there is only one attribute in dataset, this '
+                  'algorithm inject noises to its probability distribution.')
+            _cols = list(indexes)
+            prs = noisy_distributions(indexes, _cols, epsilon)
+            probability = {_cols[0]: normalize_distribution(prs[FREQ_NAME]).tolist()}
+            return None, probability
+
+        # Bayesian network is defined as a set of AP (attribute-parent) pairs.
+        # e.g. [(x1, p1), (x2, p2), ...], and pi is the parents of xi.
+        #
+        # The algorithm follows the composability property of differential
+        # privacy, so the privacy budget is split to two parts.
+        network = greedy_bayes(indexes, epsilon / 2, degree=degree,
+                               retains=retains)
+        cond_prs = noisy_conditionals(network, indexes, epsilon / 2)
+        return network, cond_prs
+
+    def to_pattern(self, epsilon=0.1, degree=2, pseudonyms=None,
+                   deletes=None, retains=None) -> dict:
+        """
+        Serialize this dataset's patterns into a dict object.
+        """
+        network, cond_prs = self._construct_bayesian_network(
+            epsilon, degree=degree, pseudonyms=pseudonyms, deletes=deletes,
+            retains=retains)
+        pattern = dict({
+            "attrs": {col: self[col].to_pattern() for col in self.columns
+                      if col not in (deletes or [])},
+            "config": {"pseudonyms": pseudonyms},
+            "network": network,
+            "prs": cond_prs,
+            "records": self._records
+        })
+        return pattern
+
+    def to_pattern_file(self, path, epsilon=0.1, degree=2, pseudonyms=None,
+                        deletes=None, retains=None) -> None:
+        """
+        Serialize this dataset's patterns into a json file.
+        """
+        pattern = self.to_pattern(epsilon, degree, pseudonyms, deletes, retains)
+        with open(path, 'w') as fp:
+            json.dump(pattern, fp, indent=2)
+
+    def synthesize(self, epsilon=0.1, degree=2,
+                   pseudonyms=None, deletes=None, retains=None, records=None):
+        """
+        Synthesize data set by a bayesian network to infer attributes'
+        dependence relationship and differential privacy to keep differentially
+        private.
+        """
+        deletes = deletes or []
+        pseudonyms = pseudonyms or (
+                self._config is not None and self._config['pseudonyms']) or []
+        retains = retains or []
+        records = records if records is not None else self._records
+
+        if self._network is None and self._cond_prs is None:
+            self._network, self._cond_prs = self._construct_bayesian_network(
+                epsilon, degree=degree, pseudonyms=pseudonyms, deletes=deletes,
+                retains=retains)
+
+        # if bayesian network is None, and probability is not None, that means
+        # there is only one column in the dataset.
+        if self._network is None and self._cond_prs is not None:
+            # this is the only column label in this dataset
+            col = self.columns[0]
+            prs = self._cond_prs[col]
+            from numpy import random
+            sampling = Series(random.choice(len(prs), size=records, p=prs))
+            attr = self[col].choice(indexes=sampling)
+            return DataFrame(attr, columns=self.columns)
+
+        columns = [col for col in self.columns.values if col not in deletes]
+        sampling = self._sampling_dataset(self._network, self._cond_prs, records)
+        frame = DataFrame(columns=columns)
+        for col in self.columns:
+            attr = self[col]
+            if col in deletes:
+                continue
+            if col in pseudonyms:  # pseudonym column is not in bayesian network
+                frame[col] = attr.pseudonymize(size=records)
+                continue
+            if col in retains:
+                frame[col] = attr.retain(records)
+                continue
+            if col in sampling:
+                frame[col] = attr.choice(indexes=sampling[col])
+                continue
+            if not attr.categorical:
+                frame[col] = attr.random()
+            else:
+                frame[col] = attr.choice()
+        return frame
```

### Comparing `ds4ml-0.3.4/ds4ml/evaluator.py` & `ds4ml-0.3.5/ds4ml/evaluator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,329 +1,329 @@
-"""
-BiFrame for data synthesis.
-"""
-
-import warnings
-import numpy as np
-import pandas as pd
-
-from pandas import Index
-from sklearn.model_selection import train_test_split
-from sklearn.metrics import confusion_matrix
-
-from ds4ml.dataset import DataSet
-from ds4ml.utils import train_and_predict, normalize_range
-from ds4ml.metrics import jensen_shannon_divergence, relative_error
-
-
-def split_feature_class(label: str, frame: pd.DataFrame):
-    """ Split features and class from encode dataset. `label` is the class, and
-    `frame` is the dataset which has been encoded.
-    """
-    sub_cols = [attr for attr in frame.columns if attr.startswith(label)]
-    if len(sub_cols) <= 1:
-        return frame, None
-    is_one_class = len(sub_cols) == 2
-    if is_one_class:
-        # For one class, there are two sorted values.
-        # e.g. ['Yes', 'No'] => [[0, 1],
-        #                        [1, 0]]
-        # Choose second column to represent this attribute.
-        label_ = sub_cols[1]
-        return frame.drop(sub_cols, axis=1), frame[label_]
-
-    # merge multiple columns into one column: [Name_A, Name_B, ..] => Name
-    y = frame[sub_cols].apply(lambda x: Index(x).get_loc(1), axis=1)
-    return frame.drop(sub_cols, axis=1), y
-
-
-class BiFrame:
-    def __init__(self, first: pd.DataFrame, second: pd.DataFrame,
-                 categories=None):
-        """
-        BiFrame class that contains two data sets, which currently provides
-        kinds of analysis methods from distribution, correlation, and some
-        machine learning tasks.
-        Especially, if the input data sets are source and synthesized dataset,
-        this class can be used to evaluate the utility and privacy of
-        synthesized data set.
-
-        Parameters
-        ----------
-        first : {pandas.DataFrame}
-            first data set (i.e. original dataset)
-
-        second : {pandas.DataFrame}
-            second data set (i.e. synthesized dataset)
-
-        categories : list of columns
-            Column names whose values are categorical.
-        """
-        # To compare two data sets, make sure that they have same columns. If
-        # not, compare them on their common columns.
-        cols = set(first.columns) & set(second.columns)
-        if len(cols) != len(first.columns) or len(cols) != len(second.columns):
-            warnings.warn("Evaluate on partial columns of the datasets",
-                          stacklevel=2)
-
-        categories = [] if categories is None else categories
-        self.fst = DataSet(first[cols], categories=categories)
-        self.snd = DataSet(second[cols], categories=categories)
-
-        # Make sure that two dataset have same domain for categorical
-        # attributes, and same min, max values for numerical attributes.
-        for col in cols.copy():
-            # If current column is not categorical, will ignore it.
-            if not self.fst[col].categorical or not self.snd[col].categorical:
-                continue
-            fst_domain, snd_domain = self.fst[col].domain, self.snd[col].domain
-            if not np.array_equal(fst_domain, snd_domain):
-                # if there is no intersection of two domains, then there may be
-                # zero relationship between the columns.
-                if len(np.intersect1d(fst_domain, snd_domain)) == 0:
-                    self.fst = self.fst.drop(col, axis=1)
-                    self.snd = self.snd.drop(col, axis=1)
-                    cols.remove(col)
-                    continue
-                if self.fst[col].categorical:
-                    domain = np.unique(np.concatenate((fst_domain, snd_domain))).tolist()
-                else:
-                    domain = [min(fst_domain[0], snd_domain[0]),
-                              max(fst_domain[1], snd_domain[1])]
-                self.fst[col].domain = domain
-                self.snd[col].domain = domain
-        self._columns = sorted(cols)
-
-    @property
-    def columns(self):
-        """ Return the common columns of two datasets. """
-        return self._columns
-
-    def err(self):
-        """
-        Return pairwise err (relative error) of columns' distribution.
-        """
-        # merge two frequency counts, and calculate relative difference
-        frame = pd.DataFrame(columns=self.columns, index=['err'])
-        frame.fillna(0)
-        for col in self.columns:
-            frame.at['err', col] = relative_error(self.fst[col].counts(),
-                                                  self.snd[col].counts())
-        return frame
-
-    def jsd(self):
-        """
-        Return pairwise JSD (Jensen-Shannon divergence) of columns' distribution.
-        """
-        frame = pd.DataFrame(columns=self.columns, index=['jsd'])
-        frame.fillna(0)
-        for col in self.columns:
-            frame.at['jsd', col] = jensen_shannon_divergence(
-                self.fst[col].counts(), self.snd[col].counts())
-        return frame
-
-    def corr(self):
-        """
-        Return pairwise correlation and dependence measured by mi (mutual
-        information).
-        """
-        return self.fst.mi(), self.snd.mi()
-
-    def dist(self, column):
-        """
-        Return frequency distribution of one column.
-
-        Parameters
-        ----------
-        column : str
-            column name, whose distribution will be return
-        """
-        if column not in self.columns:
-            raise ValueError(f"{column} is not in current dataset.")
-        if self.fst[column].categorical:
-            bins = self.fst[column].domain.tolist()
-            fst_counts = self.fst[column].counts(bins=bins)
-            snd_counts = self.snd[column].counts(bins=bins)
-        else:
-            min_, max_ = self.fst[column].domain
-            # the domain from two data set are same;
-            # extend the domain to human-readable range
-            bins = normalize_range(min_, max_ + 1)
-            fst_counts = self.fst[column].counts(bins=bins)
-            snd_counts = self.snd[column].counts(bins=bins)
-            # Note: index, value of np.histogram has different length
-            bins = bins[:-1]
-        # stack arrays vertically
-        return bins, np.vstack((fst_counts, snd_counts))
-
-    def describe(self):
-        """
-        Give descriptive difference between two data sets, which concluded
-        relative errors, and jsd divergence.
-        Return a panda.DataFrame, whose columns are two dataset's columns, and
-        indexes are a array of metrics, e.g. ['err', 'jsd'].
-        """
-        err_frame = self.err()
-        jsd_frame = self.jsd()
-        return pd.concat([err_frame, jsd_frame])
-
-    def classify(self, label: str, test: pd.DataFrame = None):
-        """
-        Train two svm classifiers based on data sets, and predict class labels
-        for test data. Return both error rates.
-
-        Parameters
-        ----------
-        label : str
-            classifier feature, key is one column in left data frame.
-            It supports two-class and multi-class.
-
-        test : {pandas.DataFrame}
-            test frame, is test data for machine learning algorithms. If it is
-            not provided, it will split 20% of left data frame as test data.
-
-        Returns
-        -------
-        a DataFrame, e.g.
-                         target                         source     target
-                      male female                    male female male female
-        source male   1    3        or actual male   1    3      1    2
-               female 2    4                  female 2    4      3    4
-        """
-        if not self.fst[label].categorical or not self.snd[label].categorical:
-            raise ValueError(f'Must classify on categorical column')
-
-        # If test dataset is not provided, then split 20% of original dataset
-        # for testing.
-        if test is None:
-            fst_train, test = train_test_split(self.fst, test_size=0.2)
-            snd_train, _ = train_test_split(self.snd, test_size=0.2)
-        else:
-            fst_train = self.fst
-            snd_train = self.snd
-
-        fst_train_x, fst_train_y = split_feature_class(label, self.fst.encode(
-            data=fst_train))
-        snd_train_x, snd_train_y = split_feature_class(label, self.fst.encode(
-            data=snd_train))
-        test_x, test_y = split_feature_class(label, self.fst.encode(data=test))
-
-        # construct svm classifier, and predict on the same test dataset
-        fst_predict_y = train_and_predict(fst_train_x, fst_train_y, test_x)
-        snd_predict_y = train_and_predict(snd_train_x, snd_train_y, test_x)
-
-        columns = self.fst[label].bins
-        labels = range(len(columns))
-        # If test dataset has the columns as class label for prediction, return
-        # two expected scores: (self.fst) original dataset's and (self.snd)
-        # synthesized dataset's confusion matrix.
-        if label in test:
-            fst_matrix = confusion_matrix(test_y, fst_predict_y, labels=labels)
-            snd_matrix = confusion_matrix(test_y, snd_predict_y, labels=labels)
-            return (pd.DataFrame(fst_matrix, columns=columns, index=columns),
-                    pd.DataFrame(snd_matrix, columns=columns, index=columns))
-
-        # If test dataset does not have the class label for prediction, return
-        # their predicted values.
-        matrix = confusion_matrix(fst_predict_y, snd_predict_y, labels=labels)
-        return pd.DataFrame(matrix, columns=columns, index=columns)
-
-    def to_html(self, buffer, title='Evaluation Report', labels=None, test=None):
-        """
-        Render the evaluation result of two datasets to an HTML file.
-
-        The result contains:
-        + basic information of two data set (relative error, and Jensen-Shannon
-            divergence (jsd));
-        + distribution of each attribute;
-        + correlation of pair-wise attributes;
-        + classification result by SVM to train data set on one or more columns
-            (defined by parameter 'labels' and 'test' dataset).
-
-        Parameters
-        ----------
-        buffer
-            buffer to write to
-
-        title : str
-            title of evaluation report
-
-        labels : list of column names
-            column name, or a list of column names separated by comma, used for
-            classification task.
-
-        test : pd.DataFrame
-            test data for classification, and other machine learning tasks.
-        """
-        basics = [self.describe().to_dict('split')]
-        svms = self._get_svm_classifier(labels=labels, test=test)
-
-        template = BiFrame._construct_template()
-        with open(buffer, 'w+', encoding='utf-8') as file:
-            file.write(template.render(title=title, basics=basics,
-                                       dists=self._get_dist(),
-                                       corrs=self._get_corr(),
-                                       svms=svms))
-
-    def _get_svm_classifier(self, labels=None, test=None):
-        if labels is None:
-            return []
-
-        from ds4ml.utils import plot_confusion_matrix
-        svms = []
-        for col in labels:
-            in_test = (test is not None and col in test) or (test is None)
-            if in_test:
-                # When class label in svm classify test data, try to match
-                # two predicted result with the actual data, and so, there
-                # will be two confusion matrix diagrams.
-                src_matrix, tgt_matrix = self.classify(col, test=test)
-                vrange = (
-                    min(src_matrix.values.min(), tgt_matrix.values.min()),
-                    max(src_matrix.values.max(), tgt_matrix.values.max()))
-                path = (
-                    plot_confusion_matrix(src_matrix, vrange=vrange,
-                                          xlabel='raw', ylabel='actual'),
-                    plot_confusion_matrix(tgt_matrix, vrange=vrange,
-                                          xlabel='synth', ylabel='actual'))
-                svms.append({'column': col, 'path': path})
-            else:
-                # If not, will compare two predicted result.
-                matrix = self.classify(col, test=test)
-                # make path's type: 1-tuple
-                path = (plot_confusion_matrix(matrix,
-                                              xlabel='synth', ylabel='raw'))
-                svms.append({'column': col, 'path': path})
-        return svms
-
-    @staticmethod
-    def _construct_template():
-        """ construct template from a html """
-        from mako.template import Template
-        import os
-        old_cwd = os.getcwd()
-        os.chdir(os.path.dirname(__file__))
-        template = Template(filename='template/report.html')
-        os.chdir(old_cwd)
-        return template
-
-    def _get_dist(self):
-        """ return the distribution information """
-        from ds4ml.utils import plot_histogram
-        dists = []
-        for col in self.columns:
-            bins, counts = self.dist(col)
-            svg = plot_histogram(bins, counts)
-            dists.append({'name': col, 'columns': bins, 'data': counts,
-                          'path': svg})
-        return dists
-
-    def _get_corr(self):
-        """ return the pair-wise correlation """
-        from ds4ml.utils import plot_heatmap
-        corrs = []
-        fst_mi, snd_mi = self.corr()
-        fst_svg = plot_heatmap(fst_mi)
-        snd_svg = plot_heatmap(snd_mi)
-        corrs.append({'matrix': fst_mi.to_dict('split'), 'path': fst_svg})
-        corrs.append({'matrix': snd_mi.to_dict('split'), 'path': snd_svg})
-        return corrs
+"""
+BiFrame for data synthesis.
+"""
+
+import warnings
+import numpy as np
+import pandas as pd
+
+from pandas import Index
+from sklearn.model_selection import train_test_split
+from sklearn.metrics import confusion_matrix
+
+from ds4ml.dataset import DataSet
+from ds4ml.utils import train_and_predict, normalize_range
+from ds4ml.metrics import jensen_shannon_divergence, relative_error
+
+
+def split_feature_class(label: str, frame: pd.DataFrame):
+    """ Split features and class from encode dataset. `label` is the class, and
+    `frame` is the dataset which has been encoded.
+    """
+    sub_cols = [attr for attr in frame.columns if attr.startswith(label)]
+    if len(sub_cols) <= 1:
+        return frame, None
+    is_one_class = len(sub_cols) == 2
+    if is_one_class:
+        # For one class, there are two sorted values.
+        # e.g. ['Yes', 'No'] => [[0, 1],
+        #                        [1, 0]]
+        # Choose second column to represent this attribute.
+        label_ = sub_cols[1]
+        return frame.drop(sub_cols, axis=1), frame[label_]
+
+    # merge multiple columns into one column: [Name_A, Name_B, ..] => Name
+    y = frame[sub_cols].apply(lambda x: Index(x).get_loc(1), axis=1)
+    return frame.drop(sub_cols, axis=1), y
+
+
+class BiFrame:
+    def __init__(self, first: pd.DataFrame, second: pd.DataFrame,
+                 categories=None):
+        """
+        BiFrame class that contains two data sets, which currently provides
+        kinds of analysis methods from distribution, correlation, and some
+        machine learning tasks.
+        Especially, if the input data sets are source and synthesized dataset,
+        this class can be used to evaluate the utility and privacy of
+        synthesized data set.
+
+        Parameters
+        ----------
+        first : {pandas.DataFrame}
+            first data set (i.e. original dataset)
+
+        second : {pandas.DataFrame}
+            second data set (i.e. synthesized dataset)
+
+        categories : list of columns
+            Column names whose values are categorical.
+        """
+        # To compare two data sets, make sure that they have same columns. If
+        # not, compare them on their common columns.
+        cols = list(set(first.columns) & set(second.columns))
+        if len(cols) != len(first.columns) or len(cols) != len(second.columns):
+            warnings.warn("Evaluate on partial columns of the datasets",
+                          stacklevel=2)
+
+        categories = [] if categories is None else categories
+        self.fst = DataSet(first[cols], categories=categories)
+        self.snd = DataSet(second[cols], categories=categories)
+
+        # Make sure that two dataset have same domain for categorical
+        # attributes, and same min, max values for numerical attributes.
+        for col in cols.copy():
+            # If current column is not categorical, will ignore it.
+            if not self.fst[col].categorical or not self.snd[col].categorical:
+                continue
+            fst_domain, snd_domain = self.fst[col].domain, self.snd[col].domain
+            if not np.array_equal(fst_domain, snd_domain):
+                # if there is no intersection of two domains, then there may be
+                # zero relationship between the columns.
+                if len(np.intersect1d(fst_domain, snd_domain)) == 0:
+                    self.fst = self.fst.drop(col, axis=1)
+                    self.snd = self.snd.drop(col, axis=1)
+                    cols.remove(col)
+                    continue
+                if self.fst[col].categorical:
+                    domain = np.unique(np.concatenate((fst_domain, snd_domain))).tolist()
+                else:
+                    domain = [min(fst_domain[0], snd_domain[0]),
+                              max(fst_domain[1], snd_domain[1])]
+                self.fst[col].domain = domain
+                self.snd[col].domain = domain
+        self._columns = sorted(cols)
+
+    @property
+    def columns(self):
+        """ Return the common columns of two datasets. """
+        return self._columns
+
+    def err(self):
+        """
+        Return pairwise err (relative error) of columns' distribution.
+        """
+        # merge two frequency counts, and calculate relative difference
+        frame = pd.DataFrame(columns=self.columns, index=['err'])
+        frame.fillna(0)
+        for col in self.columns:
+            frame.at['err', col] = relative_error(self.fst[col].counts(),
+                                                  self.snd[col].counts())
+        return frame
+
+    def jsd(self):
+        """
+        Return pairwise JSD (Jensen-Shannon divergence) of columns' distribution.
+        """
+        frame = pd.DataFrame(columns=self.columns, index=['jsd'])
+        frame.fillna(0)
+        for col in self.columns:
+            frame.at['jsd', col] = jensen_shannon_divergence(
+                self.fst[col].counts(), self.snd[col].counts())
+        return frame
+
+    def corr(self):
+        """
+        Return pairwise correlation and dependence measured by mi (mutual
+        information).
+        """
+        return self.fst.mi(), self.snd.mi()
+
+    def dist(self, column):
+        """
+        Return frequency distribution of one column.
+
+        Parameters
+        ----------
+        column : str
+            column name, whose distribution will be return
+        """
+        if column not in self.columns:
+            raise ValueError(f"{column} is not in current dataset.")
+        if self.fst[column].categorical:
+            bins = self.fst[column].domain.tolist()
+            fst_counts = self.fst[column].counts(bins=bins)
+            snd_counts = self.snd[column].counts(bins=bins)
+        else:
+            min_, max_ = self.fst[column].domain
+            # the domain from two data set are same;
+            # extend the domain to human-readable range
+            bins = normalize_range(min_, max_ + 1)
+            fst_counts = self.fst[column].counts(bins=bins)
+            snd_counts = self.snd[column].counts(bins=bins)
+            # Note: index, value of np.histogram has different length
+            bins = bins[:-1]
+        # stack arrays vertically
+        return bins, np.vstack((fst_counts, snd_counts))
+
+    def describe(self):
+        """
+        Give descriptive difference between two data sets, which concluded
+        relative errors, and jsd divergence.
+        Return a panda.DataFrame, whose columns are two dataset's columns, and
+        indexes are a array of metrics, e.g. ['err', 'jsd'].
+        """
+        err_frame = self.err()
+        jsd_frame = self.jsd()
+        return pd.concat([err_frame, jsd_frame])
+
+    def classify(self, label: str, test: pd.DataFrame = None):
+        """
+        Train two svm classifiers based on data sets, and predict class labels
+        for test data. Return both error rates.
+
+        Parameters
+        ----------
+        label : str
+            classifier feature, key is one column in left data frame.
+            It supports two-class and multi-class.
+
+        test : {pandas.DataFrame}
+            test frame, is test data for machine learning algorithms. If it is
+            not provided, it will split 20% of left data frame as test data.
+
+        Returns
+        -------
+        a DataFrame, e.g.
+                         target                         source     target
+                      male female                    male female male female
+        source male   1    3        or actual male   1    3      1    2
+               female 2    4                  female 2    4      3    4
+        """
+        if not self.fst[label].categorical or not self.snd[label].categorical:
+            raise ValueError(f'Must classify on categorical column')
+
+        # If test dataset is not provided, then split 20% of original dataset
+        # for testing.
+        if test is None:
+            fst_train, test = train_test_split(self.fst, test_size=0.2)
+            snd_train, _ = train_test_split(self.snd, test_size=0.2)
+        else:
+            fst_train = self.fst
+            snd_train = self.snd
+
+        fst_train_x, fst_train_y = split_feature_class(label, self.fst.encode(
+            data=fst_train))
+        snd_train_x, snd_train_y = split_feature_class(label, self.fst.encode(
+            data=snd_train))
+        test_x, test_y = split_feature_class(label, self.fst.encode(data=test))
+
+        # construct svm classifier, and predict on the same test dataset
+        fst_predict_y = train_and_predict(fst_train_x, fst_train_y, test_x)
+        snd_predict_y = train_and_predict(snd_train_x, snd_train_y, test_x)
+
+        columns = self.fst[label].bins
+        labels = range(len(columns))
+        # If test dataset has the columns as class label for prediction, return
+        # two expected scores: (self.fst) original dataset's and (self.snd)
+        # synthesized dataset's confusion matrix.
+        if label in test:
+            fst_matrix = confusion_matrix(test_y, fst_predict_y, labels=labels)
+            snd_matrix = confusion_matrix(test_y, snd_predict_y, labels=labels)
+            return (pd.DataFrame(fst_matrix, columns=columns, index=columns),
+                    pd.DataFrame(snd_matrix, columns=columns, index=columns))
+
+        # If test dataset does not have the class label for prediction, return
+        # their predicted values.
+        matrix = confusion_matrix(fst_predict_y, snd_predict_y, labels=labels)
+        return pd.DataFrame(matrix, columns=columns, index=columns)
+
+    def to_html(self, buffer, title='Evaluation Report', labels=None, test=None):
+        """
+        Render the evaluation result of two datasets to an HTML file.
+
+        The result contains:
+        + basic information of two data set (relative error, and Jensen-Shannon
+            divergence (jsd));
+        + distribution of each attribute;
+        + correlation of pair-wise attributes;
+        + classification result by SVM to train data set on one or more columns
+            (defined by parameter 'labels' and 'test' dataset).
+
+        Parameters
+        ----------
+        buffer
+            buffer to write to
+
+        title : str
+            title of evaluation report
+
+        labels : list of column names
+            column name, or a list of column names separated by comma, used for
+            classification task.
+
+        test : pd.DataFrame
+            test data for classification, and other machine learning tasks.
+        """
+        basics = [self.describe().to_dict('split')]
+        svms = self._get_svm_classifier(labels=labels, test=test)
+
+        template = BiFrame._construct_template()
+        with open(buffer, 'w+', encoding='utf-8') as file:
+            file.write(template.render(title=title, basics=basics,
+                                       dists=self._get_dist(),
+                                       corrs=self._get_corr(),
+                                       svms=svms))
+
+    def _get_svm_classifier(self, labels=None, test=None):
+        if labels is None:
+            return []
+
+        from ds4ml.utils import plot_confusion_matrix
+        svms = []
+        for col in labels:
+            in_test = (test is not None and col in test) or (test is None)
+            if in_test:
+                # When class label in svm classify test data, try to match
+                # two predicted result with the actual data, and so, there
+                # will be two confusion matrix diagrams.
+                src_matrix, tgt_matrix = self.classify(col, test=test)
+                vrange = (
+                    min(src_matrix.values.min(), tgt_matrix.values.min()),
+                    max(src_matrix.values.max(), tgt_matrix.values.max()))
+                path = (
+                    plot_confusion_matrix(src_matrix, vrange=vrange,
+                                          xlabel='raw', ylabel='actual'),
+                    plot_confusion_matrix(tgt_matrix, vrange=vrange,
+                                          xlabel='synth', ylabel='actual'))
+                svms.append({'column': col, 'path': path})
+            else:
+                # If not, will compare two predicted result.
+                matrix = self.classify(col, test=test)
+                # make path's type: 1-tuple
+                path = (plot_confusion_matrix(matrix,
+                                              xlabel='synth', ylabel='raw'))
+                svms.append({'column': col, 'path': path})
+        return svms
+
+    @staticmethod
+    def _construct_template():
+        """ construct template from a html """
+        from mako.template import Template
+        import os
+        old_cwd = os.getcwd()
+        os.chdir(os.path.dirname(__file__))
+        template = Template(filename='template/report.html')
+        os.chdir(old_cwd)
+        return template
+
+    def _get_dist(self):
+        """ return the distribution information """
+        from ds4ml.utils import plot_histogram
+        dists = []
+        for col in self.columns:
+            bins, counts = self.dist(col)
+            svg = plot_histogram(bins, counts)
+            dists.append({'name': col, 'columns': bins, 'data': counts,
+                          'path': svg})
+        return dists
+
+    def _get_corr(self):
+        """ return the pair-wise correlation """
+        from ds4ml.utils import plot_heatmap
+        corrs = []
+        fst_mi, snd_mi = self.corr()
+        fst_svg = plot_heatmap(fst_mi)
+        snd_svg = plot_heatmap(snd_mi)
+        corrs.append({'matrix': fst_mi.to_dict('split'), 'path': fst_svg})
+        corrs.append({'matrix': snd_mi.to_dict('split'), 'path': snd_svg})
+        return corrs
```

### Comparing `ds4ml-0.3.4/ds4ml/metrics.py` & `ds4ml-0.3.5/ds4ml/metrics.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-"""
-Metrics for data synthesis
-"""
-import pandas as pd
-import numpy as np
-from sklearn.metrics import normalized_mutual_info_score, confusion_matrix
-
-
-def pairwise_mutual_information(frame: pd.DataFrame):
-    """
-    Return mutual information matrix for pairwise columns of a DataFrame.
-    """
-    columns = frame.columns.sort_values().to_list()
-    mi = pd.DataFrame(columns=columns, index=columns, dtype=float)
-    for row in columns:
-        for col in columns:
-            if pd.isnull(mi.at[col, row]):
-                mi.at[row, col] = normalized_mutual_info_score(frame[row],
-                                                               frame[col])
-            else:
-                mi.at[row, col] = mi.at[col, row]
-    return mi.round(3)
-
-
-def jensen_shannon_divergence(p, q, base=2):
-    """
-    Return the Jensen-Shannon divergence between two 1-D arrays.
-
-    Parameters
-    ---------
-    p : array
-        left probability array
-    q : array
-        right probability array
-    base : numeric, default 2
-        logarithm base
-
-    Returns
-    -------
-    jsd : float
-        divergence of p and q
-    """
-    # If the sum of probability array p or q does not equal to 1, then normalize
-    p = np.asarray(p)
-    q = np.asarray(q)
-    p = p / np.sum(p, axis=0)
-    q = q / np.sum(q, axis=0)
-    from scipy.spatial.distance import jensenshannon
-    return round(jensenshannon(p, q, base=base), 4)
-
-
-def error_rate(y_true, y_pred=None):
-    """
-    Return error (mis-classification) rate of one classifier result
-
-    If there is only one parameter, it must be the confusion matrix;
-    If there are two parameters, they must be true and predict labels;
-    """
-    if y_pred is None:
-        if isinstance(y_true, pd.DataFrame):
-            cm = y_true.values
-        else:
-            cm = y_true
-    else:
-        cm = confusion_matrix(y_true, y_pred)
-    trace = np.trace(cm)
-    sum_ = np.sum(cm)
-    return round((sum_ - trace) / sum_, 4)
-
-
-def relative_error(x, y):
-    """
-    Return relative error of two variables: |x-y|/max(|x|, |y|)
-    """
-    m = np.maximum(np.abs(x), np.abs(y))
-    return round(np.average(np.abs(x - y) / (m + 1e-6)), 4)
+"""
+Metrics for data synthesis
+"""
+import pandas as pd
+import numpy as np
+from sklearn.metrics import normalized_mutual_info_score, confusion_matrix
+
+
+def pairwise_mutual_information(frame: pd.DataFrame):
+    """
+    Return mutual information matrix for pairwise columns of a DataFrame.
+    """
+    columns = frame.columns.sort_values().to_list()
+    mi = pd.DataFrame(columns=columns, index=columns, dtype=float)
+    for row in columns:
+        for col in columns:
+            if pd.isnull(mi.at[col, row]):
+                mi.at[row, col] = normalized_mutual_info_score(frame[row],
+                                                               frame[col])
+            else:
+                mi.at[row, col] = mi.at[col, row]
+    return mi.round(3)
+
+
+def jensen_shannon_divergence(p, q, base=2):
+    """
+    Return the Jensen-Shannon divergence between two 1-D arrays.
+
+    Parameters
+    ---------
+    p : array
+        left probability array
+    q : array
+        right probability array
+    base : numeric, default 2
+        logarithm base
+
+    Returns
+    -------
+    jsd : float
+        divergence of p and q
+    """
+    # If the sum of probability array p or q does not equal to 1, then normalize
+    p = np.asarray(p)
+    q = np.asarray(q)
+    p = p / np.sum(p, axis=0)
+    q = q / np.sum(q, axis=0)
+    from scipy.spatial.distance import jensenshannon
+    return round(jensenshannon(p, q, base=base), 4)
+
+
+def error_rate(y_true, y_pred=None):
+    """
+    Return error (mis-classification) rate of one classifier result
+
+    If there is only one parameter, it must be the confusion matrix;
+    If there are two parameters, they must be true and predict labels;
+    """
+    if y_pred is None:
+        if isinstance(y_true, pd.DataFrame):
+            cm = y_true.values
+        else:
+            cm = y_true
+    else:
+        cm = confusion_matrix(y_true, y_pred)
+    trace = np.trace(cm)
+    sum_ = np.sum(cm)
+    return round((sum_ - trace) / sum_, 4)
+
+
+def relative_error(x, y):
+    """
+    Return relative error of two variables: |x-y|/max(|x|, |y|)
+    """
+    m = np.maximum(np.abs(x), np.abs(y))
+    return round(np.average(np.abs(x - y) / (m + 1e-6)), 4)
```

### Comparing `ds4ml-0.3.4/ds4ml/template/report.html` & `ds4ml-0.3.5/ds4ml/template/report.html`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,374 +1,374 @@
-<!DOCTYPE html>
-<html lang="en">
-<head>
-    <meta charset="UTF-8">
-    <meta name="viewport" content="width=device-width, initial-scale=1">
-    <title>Evaluation Report</title>
-    <style>
-        * {
-            font-family: Arial, sans-serif;
-        }
-        html {
-            background: white;
-        }
-        .container {
-            margin: auto;
-            width: 1280px;
-            max-width: 1280px;
-            background: #80808029;
-        }
-        .content {
-            padding: 0 10px 20px 10px;
-        }
-        section {
-            padding: 10px 0;
-        }
-        h2 {
-            background: black;
-            color: white;
-            margin: 0;
-            height: 48px;
-            line-height: 2;
-            width: 1280px;
-        }
-        table {
-            width: 100%;
-            max-width: 100%;
-            background-color: #fff;
-            border-collapse: collapse;
-        }
-        table th, td {
-            text-align: center;
-            padding: 5px;
-            vertical-align: top;
-            border: 1px solid #ddd;
-            font-weight: normal;
-        }
-        table {
-            border: none;
-        }
-    
-        table tbody tr td:not(:first-child), ul>li{
-            font-size: 0.9em;
-        }
-        .content ul {
-            padding: 20px;
-        }
-        div.half-img {
-            float: right;
-            width: 45%;
-        }
-        div.wrapper {
-            height: auto;
-            overflow: auto;
-            padding: 5px 0;
-        }
-        div.table-wrapper {
-            overflow: auto;
-            float: left;
-        }
-        div.half-wrapper {
-            width: 54%;
-        }
-        div.full-wrapper {
-            width: 100%;
-            margin-bottom: 8px;
-        }
-
-        .tab {
-            background-color: #f1f1f1;
-            overflow-x: auto;
-        }
-        .tab > a {
-            background-color: inherit;
-            float: left;
-            border: none;
-            outline: none;
-            cursor: pointer;
-            padding: 14px 16px;
-            transition: 0.3s;
-            border-top: 4px solid #f1f1f1;
-            font-size: 16px;
-            border-right: 1px solid #E0E0E0;
-        }
-        .tab > a:hover {
-            background-color: #ddd;
-            border-top: 4px solid #ddd;
-            cursor: pointer;
-        }
-        .tab > a.active {
-            background-color: white;
-            border-top: 4px solid #38bbe8;
-        }
-
-        .dropdown {
-            float: left;
-            overflow: hidden;
-        }
-        .dropdown > .more {
-            font-size: 16px;
-            border: none;
-            outline: none;
-            padding: 14px 16px;
-            font-family: inherit;
-            margin: 0;
-            display: block;
-            border-top: 4px solid #f1f1f1;
-        }
-        .dropdown-content {
-            display: none;
-            position: absolute;
-            background-color: #f9f9f9;
-            z-index: 1;
-            margin-top: 2px;
-        }
-        .dropdown-content > a {
-            float: none;
-            color: black;
-            padding: 12px 16px;
-            text-decoration: none;
-            display: block;
-            text-align: left;
-            border-top: none;
-            border-left: 4px solid #f9f9f9;
-        }
-        .dropdown > .more:hover,
-        .dropdown-content > a:hover {
-            background-color: #ddd;
-            cursor: pointer;
-        }
-        .dropdown > .more:hover {
-            border-top: 4px solid #ddd;
-        }
-        .dropdown-content > a.active {
-            background-color: white;
-            border-left: 4px solid #38bbe8;
-        }
-        .dropdown:hover .dropdown-content {
-            display: block;
-        }
-
-        .tabcontent {
-            display: none;
-            padding: 8px 4px 8px 4px;
-            border-top: none;
-            background: white;
-        }
-
-        div::-webkit-scrollbar {
-            width: 10px;
-            height: 10px;
-            background-color: #F5F5F5;
-        }
-        div::-webkit-scrollbar-thumb {
-            background-color: darkgrey;
-            outline: 1px solid slategrey;
-        }
-    </style>
-    <script>
-    function openColumn(evt, column) {
-        var i, tabcontent, tablinks;
-        section = evt.target.parentNode.parentNode;
-        if (section.tagName != 'SECTION' && section.className == 'dropdown') {
-            section = section.parentNode.parentNode;
-        }
-
-        tabcontent = section.getElementsByClassName("tabcontent");
-        for (i = 0; i < tabcontent.length; i++) {
-            tabcontent[i].style.display = "none";
-        }
-        tablinks = section.getElementsByClassName("tablinks");
-        for (i = 0; i < tablinks.length; i++) {
-            tablinks[i].className = tablinks[i].className.replace(" active", "");
-        }
-        section.querySelectorAll('.tabContent,.' + column)[0].style.display = "block";
-        evt.currentTarget.className += " active";
-    };
-
-    const adapt = (tab) => {
-        width = tab.offsetWidth;
-        items = Array.from(tab.children);
-        wholeWidth = items.reduce((acc, cur) => {
-                                return cur.offsetWidth + acc;
-                            }, 0);
-        if (wholeWidth > width) {
-            tab.insertAdjacentHTML('beforeend',
-                `<div class="dropdown">
-                <a type="button" class="more">
-                    <span>More &darr;</span>
-                </a>
-                <div class="dropdown-content"></div>
-                </div>`);
-            moreWidth = tab.querySelector('.more').offsetWidth;
-            for (i = 0, partWidth = moreWidth; i < items.length; i++) {
-                if (partWidth < width) {
-                    partWidth += items[i].offsetWidth;
-                } else {
-                    last = items[i - 1];
-                    dropDown = tab.querySelector('.dropdown');
-                    last.after(dropDown);
-                    dropDownList = dropDown.querySelector('.dropdown-content');
-                    for (j = i - 1; j < items.length; j++) {
-                        dropDownList.appendChild(items[j]);
-                    }
-                    break;
-                }
-            }
-        }
-    };
-
-    const load = () => {
-        tabs = document.querySelectorAll('.tab');
-        tabs.forEach((tab) => adapt(tab));
-    };
-    window.addEventListener('resize', load);
-    window.addEventListener('load', load);
-    </script>
-</head>
-<body class="container">
-<h2 align="center">${title}</h2>
-
-<div class="content">
-<section>
-<h3 align="center">Basic Information</h3>
-% for basic in basics:
-<div class="table-wrapper full-wrapper">
-<table class="table">
-    <thead>
-        <th></th>
-        % for column in basic['columns']:
-        <th>${column}</th>
-        % endfor
-    </thead>
-    <tbody>
-    % for idx, val in enumerate(basic['index']):
-        <tr>
-            <td>${val}</td>
-            % for datum in basic['data'][idx]:
-            <td>${datum}</td>
-            % endfor
-        </tr>
-    % endfor
-    </tbody>
-</table>
-</div>
-<ul>
-    <li style="list-style-type:none">  range: [0,1] The smaller the value is, the closer the synthesized data is to the raw data.</li>
-    <li>err: relative error, a measure of the discrepancy between raw data and synthesized data.</li>
-    <li>jsd: Jensen-Shannon divergence, a measure of the similarity between the probability distribution of raw and synthesized data.</li>
-</ul>
-% endfor
-</section>
-
-<section>
-<h3 align="center">Attribute Distribution</h3>
-<div class="tab">
-    <%
-        actives = [ ' active' if idx == 0 else '' for idx in range(len(dists))]
-    %>
-    % for active, entry in zip(actives, dists):
-    <a class="tablinks ${active}" onclick="openColumn(event, '${entry['name']}')">${entry['name']}</a>
-    % endfor
-</div>
-<%
-    displays = [ 'block' if idx == 0 else 'none' for idx in range(len(dists))]
-%>
-% for display, entry in zip(displays, dists):
-<div class="tabcontent ${entry['name']}" style="display: ${display};">
-    <div class="table-wrapper full-wrapper">
-    <table class="table">
-        <thead>
-            <th>(%)</th>
-            % for col in entry['columns']:
-            <th>${col}</th>
-            % endfor
-        </thead>
-        <tbody>
-            <tr>
-                <td>raw</td>
-                % for datum in entry['data'][0]:
-                <td>${datum}</td>
-                % endfor
-            </tr>
-            <tr>
-                <td>synth</td>
-                % for datum in entry['data'][1]:
-                <td>${datum}</td>
-                % endfor
-            </tr>
-        </tbody>
-    </table>
-    </div>
-    <div style="display:table; margin: 0 auto;">${entry['path']}</div>
-</div>
-% endfor
-
-</section>
-
-<section>
-<h3 align="center">Pair-wise Correlation</h3>
-% for idx, entry in zip(['Raw Dataset', 'Synthesized Dataset'], corrs):
-    <span>${idx}</span>
-    <div class="wrapper">
-    <div class="table-wrapper half-wrapper">
-    <table class="table">
-    <thead>
-        <th></th>
-        % for column in entry['matrix']['columns']:
-        <th>${column}</th>
-        % endfor
-    </thead>
-    <tbody>
-    % for idx, val in enumerate(entry['matrix']['index']):
-        <tr>
-            <th>${val}</th>
-            % for datum in entry['matrix']['data'][idx]:
-            <td>${datum}</td>
-            % endfor
-        </tr>
-    % endfor
-    </tbody>
-    </table>
-    </div>
-        <div class="half-img">${entry['path']}</div>
-    </div>
-% endfor
- <ul>
-    <li style="list-style-type:none">range: [0,1] The closer the value is 1, the stronger the correlation is.</li>
-    <li>By comparing the results before and after, it can reflect whether the synthesized data has maintained the correlation among columns</li>
- </ul>
-</section>
-
-% if len(svms) > 0:
-<section>
-<h3 align="center">Misclassification Rate by SVM Classifier</h3>
-<div class="tab">
-    <%
-        svm_actives = [ ' active' if idx == 0 else '' for idx in range(len(svms))]
-    %>
-    % for active, entry in zip(svm_actives, svms):
-    <a class="tablinks ${active}" onclick="openColumn(event, '${entry['column']}')">${entry['column']}</a>
-    % endfor
-</div>
-<%
-    svm_displays = [ 'block' if idx == 0 else 'none' for idx in range(len(svms))]
-%>
-% for display, entry in zip(svm_displays, svms):
-<div class="tabcontent ${entry['column']}" style="display: ${display};">
-    % if len(entry['path']) == 1:
-    <div style="display:block; text-align: center;">${entry['path'][0]}</div>
-    % endif
-    % if len(entry['path']) == 2:
-    <div style="display:contents;float:left;">${entry['path'][0]}</div>
-    <div style="display:contents;float:right;">${entry['path'][1]}</div>
-    % endif
-</div>
-% endfor
-<ul>
-    <li>After synthesis, if the misclassification rate approximates to the rate of original data, the synthesized dataset can be used for SVM classifier modeling</li>
-</ul>
-</section>
-% endif
-</div>
-</body>
-</html>
+<!DOCTYPE html>
+<html lang="en">
+<head>
+    <meta charset="UTF-8">
+    <meta name="viewport" content="width=device-width, initial-scale=1">
+    <title>Evaluation Report</title>
+    <style>
+        * {
+            font-family: Arial, sans-serif;
+        }
+        html {
+            background: white;
+        }
+        .container {
+            margin: auto;
+            width: 1280px;
+            max-width: 1280px;
+            background: #80808029;
+        }
+        .content {
+            padding: 0 10px 20px 10px;
+        }
+        section {
+            padding: 10px 0;
+        }
+        h2 {
+            background: black;
+            color: white;
+            margin: 0;
+            height: 48px;
+            line-height: 2;
+            width: 1280px;
+        }
+        table {
+            width: 100%;
+            max-width: 100%;
+            background-color: #fff;
+            border-collapse: collapse;
+        }
+        table th, td {
+            text-align: center;
+            padding: 5px;
+            vertical-align: top;
+            border: 1px solid #ddd;
+            font-weight: normal;
+        }
+        table {
+            border: none;
+        }
+    
+        table tbody tr td:not(:first-child), ul>li{
+            font-size: 0.9em;
+        }
+        .content ul {
+            padding: 20px;
+        }
+        div.half-img {
+            float: right;
+            width: 45%;
+        }
+        div.wrapper {
+            height: auto;
+            overflow: auto;
+            padding: 5px 0;
+        }
+        div.table-wrapper {
+            overflow: auto;
+            float: left;
+        }
+        div.half-wrapper {
+            width: 54%;
+        }
+        div.full-wrapper {
+            width: 100%;
+            margin-bottom: 8px;
+        }
+
+        .tab {
+            background-color: #f1f1f1;
+            overflow-x: auto;
+        }
+        .tab > a {
+            background-color: inherit;
+            float: left;
+            border: none;
+            outline: none;
+            cursor: pointer;
+            padding: 14px 16px;
+            transition: 0.3s;
+            border-top: 4px solid #f1f1f1;
+            font-size: 16px;
+            border-right: 1px solid #E0E0E0;
+        }
+        .tab > a:hover {
+            background-color: #ddd;
+            border-top: 4px solid #ddd;
+            cursor: pointer;
+        }
+        .tab > a.active {
+            background-color: white;
+            border-top: 4px solid #38bbe8;
+        }
+
+        .dropdown {
+            float: left;
+            overflow: hidden;
+        }
+        .dropdown > .more {
+            font-size: 16px;
+            border: none;
+            outline: none;
+            padding: 14px 16px;
+            font-family: inherit;
+            margin: 0;
+            display: block;
+            border-top: 4px solid #f1f1f1;
+        }
+        .dropdown-content {
+            display: none;
+            position: absolute;
+            background-color: #f9f9f9;
+            z-index: 1;
+            margin-top: 2px;
+        }
+        .dropdown-content > a {
+            float: none;
+            color: black;
+            padding: 12px 16px;
+            text-decoration: none;
+            display: block;
+            text-align: left;
+            border-top: none;
+            border-left: 4px solid #f9f9f9;
+        }
+        .dropdown > .more:hover,
+        .dropdown-content > a:hover {
+            background-color: #ddd;
+            cursor: pointer;
+        }
+        .dropdown > .more:hover {
+            border-top: 4px solid #ddd;
+        }
+        .dropdown-content > a.active {
+            background-color: white;
+            border-left: 4px solid #38bbe8;
+        }
+        .dropdown:hover .dropdown-content {
+            display: block;
+        }
+
+        .tabcontent {
+            display: none;
+            padding: 8px 4px 8px 4px;
+            border-top: none;
+            background: white;
+        }
+
+        div::-webkit-scrollbar {
+            width: 10px;
+            height: 10px;
+            background-color: #F5F5F5;
+        }
+        div::-webkit-scrollbar-thumb {
+            background-color: darkgrey;
+            outline: 1px solid slategrey;
+        }
+    </style>
+    <script>
+    function openColumn(evt, column) {
+        var i, tabcontent, tablinks;
+        section = evt.target.parentNode.parentNode;
+        if (section.tagName != 'SECTION' && section.className == 'dropdown') {
+            section = section.parentNode.parentNode;
+        }
+
+        tabcontent = section.getElementsByClassName("tabcontent");
+        for (i = 0; i < tabcontent.length; i++) {
+            tabcontent[i].style.display = "none";
+        }
+        tablinks = section.getElementsByClassName("tablinks");
+        for (i = 0; i < tablinks.length; i++) {
+            tablinks[i].className = tablinks[i].className.replace(" active", "");
+        }
+        section.querySelectorAll('.tabContent,.' + column)[0].style.display = "block";
+        evt.currentTarget.className += " active";
+    };
+
+    const adapt = (tab) => {
+        width = tab.offsetWidth;
+        items = Array.from(tab.children);
+        wholeWidth = items.reduce((acc, cur) => {
+                                return cur.offsetWidth + acc;
+                            }, 0);
+        if (wholeWidth > width) {
+            tab.insertAdjacentHTML('beforeend',
+                `<div class="dropdown">
+                <a type="button" class="more">
+                    <span>More &darr;</span>
+                </a>
+                <div class="dropdown-content"></div>
+                </div>`);
+            moreWidth = tab.querySelector('.more').offsetWidth;
+            for (i = 0, partWidth = moreWidth; i < items.length; i++) {
+                if (partWidth < width) {
+                    partWidth += items[i].offsetWidth;
+                } else {
+                    last = items[i - 1];
+                    dropDown = tab.querySelector('.dropdown');
+                    last.after(dropDown);
+                    dropDownList = dropDown.querySelector('.dropdown-content');
+                    for (j = i - 1; j < items.length; j++) {
+                        dropDownList.appendChild(items[j]);
+                    }
+                    break;
+                }
+            }
+        }
+    };
+
+    const load = () => {
+        tabs = document.querySelectorAll('.tab');
+        tabs.forEach((tab) => adapt(tab));
+    };
+    window.addEventListener('resize', load);
+    window.addEventListener('load', load);
+    </script>
+</head>
+<body class="container">
+<h2 align="center">${title}</h2>
+
+<div class="content">
+<section>
+<h3 align="center">Basic Information</h3>
+% for basic in basics:
+<div class="table-wrapper full-wrapper">
+<table class="table">
+    <thead>
+        <th></th>
+        % for column in basic['columns']:
+        <th>${column}</th>
+        % endfor
+    </thead>
+    <tbody>
+    % for idx, val in enumerate(basic['index']):
+        <tr>
+            <td>${val}</td>
+            % for datum in basic['data'][idx]:
+            <td>${datum}</td>
+            % endfor
+        </tr>
+    % endfor
+    </tbody>
+</table>
+</div>
+<ul>
+    <li style="list-style-type:none">  range: [0,1] The smaller the value is, the closer the synthesized data is to the raw data.</li>
+    <li>err: relative error, a measure of the discrepancy between raw data and synthesized data.</li>
+    <li>jsd: Jensen-Shannon divergence, a measure of the similarity between the probability distribution of raw and synthesized data.</li>
+</ul>
+% endfor
+</section>
+
+<section>
+<h3 align="center">Attribute Distribution</h3>
+<div class="tab">
+    <%
+        actives = [ ' active' if idx == 0 else '' for idx in range(len(dists))]
+    %>
+    % for active, entry in zip(actives, dists):
+    <a class="tablinks ${active}" onclick="openColumn(event, '${entry['name']}')">${entry['name']}</a>
+    % endfor
+</div>
+<%
+    displays = [ 'block' if idx == 0 else 'none' for idx in range(len(dists))]
+%>
+% for display, entry in zip(displays, dists):
+<div class="tabcontent ${entry['name']}" style="display: ${display};">
+    <div class="table-wrapper full-wrapper">
+    <table class="table">
+        <thead>
+            <th>(%)</th>
+            % for col in entry['columns']:
+            <th>${col}</th>
+            % endfor
+        </thead>
+        <tbody>
+            <tr>
+                <td>raw</td>
+                % for datum in entry['data'][0]:
+                <td>${datum}</td>
+                % endfor
+            </tr>
+            <tr>
+                <td>synth</td>
+                % for datum in entry['data'][1]:
+                <td>${datum}</td>
+                % endfor
+            </tr>
+        </tbody>
+    </table>
+    </div>
+    <div style="display:table; margin: 0 auto;">${entry['path']}</div>
+</div>
+% endfor
+
+</section>
+
+<section>
+<h3 align="center">Pair-wise Correlation</h3>
+% for idx, entry in zip(['Raw Dataset', 'Synthesized Dataset'], corrs):
+    <span>${idx}</span>
+    <div class="wrapper">
+    <div class="table-wrapper half-wrapper">
+    <table class="table">
+    <thead>
+        <th></th>
+        % for column in entry['matrix']['columns']:
+        <th>${column}</th>
+        % endfor
+    </thead>
+    <tbody>
+    % for idx, val in enumerate(entry['matrix']['index']):
+        <tr>
+            <th>${val}</th>
+            % for datum in entry['matrix']['data'][idx]:
+            <td>${datum}</td>
+            % endfor
+        </tr>
+    % endfor
+    </tbody>
+    </table>
+    </div>
+        <div class="half-img">${entry['path']}</div>
+    </div>
+% endfor
+ <ul>
+    <li style="list-style-type:none">range: [0,1] The closer the value is 1, the stronger the correlation is.</li>
+    <li>By comparing the results before and after, it can reflect whether the synthesized data has maintained the correlation among columns</li>
+ </ul>
+</section>
+
+% if len(svms) > 0:
+<section>
+<h3 align="center">Misclassification Rate by SVM Classifier</h3>
+<div class="tab">
+    <%
+        svm_actives = [ ' active' if idx == 0 else '' for idx in range(len(svms))]
+    %>
+    % for active, entry in zip(svm_actives, svms):
+    <a class="tablinks ${active}" onclick="openColumn(event, '${entry['column']}')">${entry['column']}</a>
+    % endfor
+</div>
+<%
+    svm_displays = [ 'block' if idx == 0 else 'none' for idx in range(len(svms))]
+%>
+% for display, entry in zip(svm_displays, svms):
+<div class="tabcontent ${entry['column']}" style="display: ${display};">
+    % if len(entry['path']) == 1:
+    <div style="display:block; text-align: center;">${entry['path'][0]}</div>
+    % endif
+    % if len(entry['path']) == 2:
+    <div style="display:contents;float:left;">${entry['path'][0]}</div>
+    <div style="display:contents;float:right;">${entry['path'][1]}</div>
+    % endif
+</div>
+% endfor
+<ul>
+    <li>After synthesis, if the misclassification rate approximates to the rate of original data, the synthesized dataset can be used for SVM classifier modeling</li>
+</ul>
+</section>
+% endif
+</div>
+</body>
+</html>
```

### Comparing `ds4ml-0.3.4/ds4ml/utils.py` & `ds4ml-0.3.5/ds4ml/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,479 +1,498 @@
-# -*- coding: utf-8 -*-
-
-"""
-Utility functions for data synthesis. Including:
-    input/output,
-    machine learning,
-    ...
-"""
-import argparse
-import csv
-import numpy as np
-import os
-import re
-import hashlib
-
-from string import ascii_lowercase
-from pandas import Series, DataFrame
-
-
-# ---------------------------------------------------------------
-# Utilities for Input/Output
-
-
-def has_header(path, encoding='utf-8', sep=','):
-    """
-    Auto-detect if csv file has header.
-    """
-    from pandas import read_csv
-
-    def _offset_stream():
-        from io import StringIO
-        if isinstance(path, StringIO):
-            path.seek(0)
-
-    _offset_stream()
-    df0 = read_csv(path, header=None, nrows=10, skipinitialspace=True,
-                   encoding=encoding, sep=sep)
-    _offset_stream()
-    df1 = read_csv(path, nrows=10, skipinitialspace=True, encoding=encoding, sep=sep)
-    # If the column is numerical, its dtype is different without/with header
-    # TODO how about categorical columns
-    _offset_stream()
-    return tuple(df0.dtypes) != tuple(df1.dtypes)
-
-
-def ends_with_json(path):
-    return re.match(r".+\.json", path, re.IGNORECASE) is not None
-
-
-def read_data_from_csv(path, na_values=None, header=None, sep=","):
-    """
-    Read data set from csv or other delimited text file. And remove empty
-    columns (all values are null).
-    """
-    from pandas import read_csv
-
-    try:
-        header = header or ('infer' if has_header(path, sep=sep) else None)
-        df = read_csv(path, skipinitialspace=True, na_values=na_values,
-                      header=header, sep=sep, float_precision='high')
-    except (UnicodeDecodeError, NameError):
-        header = header or ('infer' if has_header(path, encoding='latin1',
-                                                  sep=sep) else None)
-        df = read_csv(path, skipinitialspace=True, na_values=na_values,
-                      header=header, encoding='latin1', sep=sep,
-                      float_precision='high')
-
-    # Remove columns with empty active domain, i.e., all values are missing.
-    before_attrs = set(df.columns)
-    df.dropna(axis=1, how='all')
-    after_attrs = set(df.columns)
-    if len(before_attrs) > len(after_attrs):
-        print(
-            f'Empty columns are removed, include {before_attrs - after_attrs}.')
-    # Remove rows with all empty values
-    df.dropna(axis=0, how='all')
-    if header is None:
-        df = df.rename(lambda x: f'#{x}', axis='columns')
-    return df
-
-
-def write_csv(file, data):
-    """ write data to csv files """
-    # if data is not a list of list, make it:
-    if isinstance(data, list) and not isinstance(data[0], list):
-        data = [data]
-    with open(file, 'a') as f:
-        writer = csv.writer(f, lineterminator='\n')
-        writer.writerows(data)
-    f.close()
-
-
-def file_name(path):
-    """ Return the file name without extension from a path. """
-    return os.path.splitext(os.path.basename(path))[0]
-
-
-def str_to_list(val, separator=','):
-    """
-    Split one string to a list by separator.
-    """
-    if val is None:
-        return None
-    return val.split(separator)
-
-
-# ---------------------------------------------------------------
-# Utilities for Plotting
-
-
-def _compress_svg_data(svg: str):
-    value = re.sub(r'\n', ' ', svg)
-    value = re.sub(r' {2,}', ' ', value)
-    value = re.sub(r'<style type="text/css">.*</style>', '', value)
-    value = re.sub(r'<!--(.*?)-->', '', value)
-    value = re.sub(r'<\?xml.*\?>', '', value)
-    value = re.sub(r'<!DOCTYPE.*dtd">', '', value)
-    return value.strip()
-
-
-def _prepare_for_cjk_characters(chars):
-    """ If input string has Chinese, Japanese, and Korean characters, set
-    specific font for them. """
-    has_cjk = False
-    for c in chars:
-        if any([start <= ord(c) <= end for start, end in [
-            (4352, 4607), (11904, 42191), (43072, 43135), (44032, 55215),
-            (63744, 64255), (65072, 65103), (65381, 65500), (131072, 196607)
-        ]]):
-            has_cjk = True
-            break
-    if has_cjk:
-        import matplotlib
-        matplotlib.rcParams['font.family'] = ['Microsoft Yahei']
-
-
-def plot_confusion_matrix(matrix: DataFrame, title='',
-                          ylabel='Predicted', xlabel='Actual',
-                          otype='string', path=None, cmap='Blues',
-                          vrange=None):
-    """
-    Plot a confusion matrix to show predict and actual values.
-
-    Parameters
-    ----------
-    matrix : pandas.DataFrame
-        the matrix to plot
-
-    title : str
-        title of image
-
-    ylabel : str
-        label in y-axis of image
-
-    xlabel : str
-        label in x-axis of image
-
-    otype : str
-        output type, support 'string' (default), 'file', 'show'
-
-    path : str
-        output path for 'file' type, default is 'matrix_2_3.svg' ((2, 3) is the
-        shape of matrix).
-
-    cmap : str
-        color
-
-    vrange : 2-tuple
-        manually set range of matrix
-    """
-    import matplotlib.pyplot as plt
-    _prepare_for_cjk_characters(''.join(map(str, matrix.columns)))
-    figsize = (6.4, 4.8)
-    n_columns = matrix.columns.size
-    if n_columns > 9:
-        from math import ceil
-        width = 6.4 + ceil((n_columns - 9) / 2) * 0.8
-        height = width * figsize[1] / figsize[0]
-        figsize = (width, height)
-    fig = plt.figure(figsize=figsize)
-    ax = fig.add_subplot(111)
-    if vrange is None:
-        vrange = (matrix.values.min(), matrix.values.max())
-    exp = len(str(vrange[1])) - 1
-    if exp > 2:
-        matrix = matrix.div(10 ** exp)
-        vrange = (vrange[0] / (10 ** exp), vrange[1] / (10 ** exp))
-    im = ax.imshow(matrix.values, cmap=cmap, vmin=vrange[0], vmax=vrange[1])
-    ax.set(xticks=np.arange(matrix.shape[1]),
-           yticks=np.arange(matrix.shape[0]),
-           xticklabels=matrix.columns,
-           yticklabels=matrix.index,
-           title=title,
-           ylabel=ylabel,
-           xlabel=xlabel)
-    ax.tick_params(which='both', length=0)
-    for edge, spine in ax.spines.items():
-        spine.set_visible(False)
-
-    # Loop over data dimensions and create text annotations.
-    thresh = (vrange[0] + vrange[1]) / 2.
-    for i in range(matrix.shape[0]):
-        for j in range(matrix.shape[1]):
-            if exp > 2:
-                text = '{:.2f}'.format(matrix.iloc[i, j])
-            else:
-                text = matrix.iloc[i, j]
-            ax.text(j, i, text,
-                    ha="center", va="center",
-                    color="white" if matrix.iloc[i, j] > thresh else "black")
-    from ds4ml.metrics import error_rate
-    ax.set_title('Rate: {:.1%}'.format(error_rate(matrix)), fontsize=10)
-
-    cbar = ax.figure.colorbar(im, ax=ax, pad=0.03, aspect=30)
-    cbar.outline.set_visible(False)
-    if exp > 2:
-        cbar.ax.text(0, -0.1, f'(e+{exp})')
-    cbar.ax.tick_params(which='both', length=0)
-    fig.autofmt_xdate()
-    fig.tight_layout()
-    plt.subplots_adjust()
-    try:
-        if otype == 'string':
-            from io import StringIO
-            img = StringIO()
-            plt.savefig(img, format='svg', bbox_inches='tight')
-            return _compress_svg_data(img.getvalue())
-        elif otype == 'file':
-            if path is None:
-                path = 'matrix_{}_{}.svg'.format(matrix.shape[0],
-                                                 matrix.shape[1])
-            plt.savefig(path, bbox_inches='tight')
-            return path
-        elif otype == 'show':
-            plt.show()
-    finally:
-        plt.close()
-
-
-def plot_histogram(bins, heights, otype='string', path=None,
-                   x_label='', y_label='Frequency'):
-    """
-    Plot two bars.
-    Note: Because pyplot draws diagrams auto-scale, this function will provide
-    kinds of diagram patterns.
-    """
-    import matplotlib.pyplot as plt
-    _prepare_for_cjk_characters(''.join(map(str, bins)))
-    length = len(bins)
-    fig_width = 6.4
-    ticks = 22
-    if length < 5:
-        # make 7 bars to show the data
-        # insert 0 or '' to the center of array
-        # e.g. [3, 4] => [3, 0, 4], ['1', '2', '3'] => ['1', '', '2', '', '3'], ...
-        bins = list(map(str, bins))
-        bins = ',,'.join(bins).split(',')
-        heights = np.insert(heights, list(range(1, length)), 0, axis=1)
-        # pad 0 or '' to array in the begin and end
-        pad = (7 - len(bins)) // 2
-        bins = tuple([''] * pad + bins + [''] * pad)
-        heights = np.append(np.insert(heights, [0], [0] * pad, axis=1),
-                            np.zeros((len(heights), pad), dtype=int), axis=1)
-        length = 7
-    else:
-        # TODO: if count of bins is bigger than 33, and it is categorical, how?
-        if length >= 60:
-            bins = bins[:60]
-            heights = heights[:, :60]
-            length = 60
-        bins = tuple(map(str, bins))
-        length_ = [8, 12, 16, 20, 32, 42, 48, 60]
-        ticks_ = [22, 30, 36, 48, 76, 96, 108, 172]
-        width_ = [6.4, 9.6, 11.2, 11.2, 11.2, 14, 14, 15]
-        idx = len([i for i in length_ if length > i])
-        ticks = ticks_[idx]
-        fig_width = width_[idx]
-
-    x = np.arange(length)
-    fig = plt.figure(figsize=(fig_width, 4.8))
-    ax = fig.add_subplot(111)
-    width = length / ticks
-    diff = width / 2 + 0.01
-    ax.bar(x - diff, heights[0], width=width, color='#38bbe8')
-    ax.bar(x + diff, heights[1], width=width, color='#ffd56e')
-    ax.legend(['raw', 'synth'])
-    fig.autofmt_xdate()
-    # fig.tight_layout(pad=1.5)
-    plt.xticks(x, bins, fontsize=10)
-    plt.xlabel(x_label)
-    plt.ylabel(y_label)
-    plt.subplots_adjust()
-    try:
-        if otype == 'string':
-            from io import StringIO
-            img = StringIO()
-            plt.savefig(img, format='svg', bbox_inches='tight')
-            return _compress_svg_data(img.getvalue())
-        elif otype == 'file':
-            if path is None:
-                path = 'histogram_{}_{}.svg'.format(len(bins), len(heights))
-            plt.savefig(path, bbox_inches='tight')
-            return path
-        elif otype == 'show':
-            plt.show()
-    finally:
-        plt.close()
-
-
-def plot_heatmap(data, title='', otype='string', path=None, cmap='Blues'):
-    """
-    Plot a heatmap to show pairwise correlations (e.g. mutual information).
-
-    Parameters see <code>plot_confusion_matrix</code>
-    """
-    import matplotlib.pyplot as plt
-    _prepare_for_cjk_characters(''.join(data.columns))
-    fig = plt.figure()
-    ax = fig.add_subplot(111)
-    im = ax.imshow(data.values, cmap=cmap)
-
-    ax.set_title(title, fontsize=10)
-    ticks = np.arange(len(data.columns))
-    ax.set_xticks(ticks)
-    ax.set_xticklabels(data.columns)
-    ax.set_yticks(ticks)
-    ax.set_yticklabels(data.index)
-    ax.tick_params(which='both', length=0)
-    for edge, spine in ax.spines.items():
-        spine.set_visible(False)
-
-    # set color bar in the right
-    cbar = ax.figure.colorbar(im, ax=ax, pad=0.03, aspect=30)
-    cbar.outline.set_visible(False)
-    cbar.ax.tick_params(which='both', length=0)
-    fig.autofmt_xdate()
-    fig.tight_layout()
-    plt.subplots_adjust()
-    try:
-        if otype == 'string':
-            from io import StringIO
-            img = StringIO()
-            plt.savefig(img, format='svg', facecolor='#ebebeb',
-                        bbox_inches='tight')
-            return _compress_svg_data(img.getvalue())
-        elif otype == 'file':
-            if path is None:
-                path = 'heatmap_{}_{}.svg'.format(data.shape[0], data.shape[1])
-            plt.savefig(path, facecolor='#ebebeb', bbox_inches='tight')
-            return path
-        elif otype == 'show':
-            plt.show()
-    finally:
-        plt.close()
-
-
-# ---------------------------------------------------------------
-# Utilities for Metrics, ML
-
-def train_and_predict(x_train, y_train, x_test):
-    """
-    Predict <x, y> by SVM classifier, and compare with test data
-    """
-    from sklearn.svm import SVC
-    classifier = SVC(gamma='scale')
-    classifier.fit(x_train, y_train)
-    result = classifier.predict(x_test)
-    return result
-
-
-def mutual_information(child: Series, parents: DataFrame):
-    """
-    Mutual information of child (Series) and parents (DataFrame) distributions
-    """
-    from sklearn.metrics import mutual_info_score
-    if parents.shape[1] == 1:
-        parents = parents.iloc[:, 0]
-    else:
-        parents = parents.apply(lambda x: ' '.join(x.array), axis=1)
-    return mutual_info_score(child, parents)
-
-
-def normalize_distribution(frequencies):
-    frequencies = np.array(frequencies, dtype=float)
-    frequencies = frequencies.clip(0)
-    total = frequencies.sum()
-    if total > 0:
-        if np.isinf(total):
-            return normalize_distribution(np.isinf(frequencies))
-        else:
-            return frequencies / total
-    else:
-        return np.full_like(frequencies, 1 / frequencies.size)
-
-
-def normalize_range(start, stop, bins=20):
-    """
-    Return evenly spaced values within a given interval, and a dynamically
-    calculated step, to make number of bins close to 20. If integer interval,
-    the smallest step is 1; If float interval, the smallest step is 0.5.
-    """
-    from math import ceil, floor
-    if isinstance(start, int) and isinstance(stop, int):
-        step = ceil((stop - start) / bins)
-    else:
-        start = floor(start)
-        stop = ceil(stop)
-        step = (stop - start) / bins
-        step = ceil(step) if ceil(step) == round(step) else round(step) + 0.5
-    stop = step * (bins + 1) + start
-    return np.arange(start, stop, step)
-
-
-def is_datetime(value: str):
-    from dateutil.parser import parse
-    """
-    Detect a value is a datetime. Exclude some datetime literals (weekdays and
-    months) from method `dateutil.parser`.
-    """
-    literals = {'mon', 'monday', 'tue', 'tuesday', 'wed', 'wednesday', 'thu',
-                'thursday', 'fri', 'friday', 'sat', 'saturday', 'sun', 'sunday',
-                'jan', 'january', 'feb', 'february', 'mar', 'march', 'apr',
-                'april', 'may', 'jun', 'june', 'jul', 'july', 'aug', 'august',
-                'sep', 'sept', 'september', 'oct', 'october', 'nov', 'november',
-                'dec', 'december'}
-    try:
-        value = value.lower()
-        if value in literals:
-            return False
-        parse(value)
-        return True
-    except ValueError:
-        return False
-    except AttributeError:
-        return False
-
-
-def is_discrete_values(values: Series) -> bool:
-    unique_values = values.unique()
-    return len(unique_values) < len(values) * 0.8
-
-
-def randomize_string(length):
-    return ''.join(np.random.choice(list(ascii_lowercase), size=length))
-
-
-def pseudonymise_string(value):
-    """ pseudonymise a string by RIPEMD-160 hashes """
-    return hashlib.new('ripemd160', str(value).encode('utf-8')).hexdigest()
-
-
-# ---------------------------------------------------------------
-# Utilities for arguments parser
-
-
-class CustomFormatter(argparse.HelpFormatter):
-    def _format_action_invocation(self, action):
-        if not action.option_strings:
-            metavar, = self._metavar_formatter(action, action.dest)(1)
-            return metavar
-        else:
-            parts = []
-            # if the Optional doesn't take a value, format is:
-            #    -s, --long
-            if action.nargs == 0:
-                parts.extend(action.option_strings)
-
-            # if the Optional takes a value, format is:
-            #    -s ARGS, --long ARGS
-            # change to
-            #    -s, --long ARGS
-            else:
-                default = action.dest.upper()
-                args_string = self._format_args(action, default)
-                for option_string in action.option_strings:
-                    # parts.append('%s %s' % (option_string, args_string))
-                    parts.append('%s' % option_string)
-                parts[-1] += ' %s' % args_string
-            return ', '.join(parts)
+# -*- coding: utf-8 -*-
+
+"""
+Utility functions for data synthesis. Including:
+    input/output,
+    machine learning,
+    ...
+"""
+import argparse
+import csv
+import numpy as np
+import os
+import re
+import hashlib
+
+from string import ascii_lowercase
+from pandas import Series, DataFrame
+
+FREQ_NAME = '@-freq#@'
+
+# ---------------------------------------------------------------
+# Utilities for Input/Output
+
+
+def has_header(path, encoding='utf-8', sep=','):
+    """
+    Auto-detect if csv file has header.
+    """
+    from pandas import read_csv
+
+    def _offset_stream():
+        from io import StringIO
+        if isinstance(path, StringIO):
+            path.seek(0)
+
+    _offset_stream()
+    df0 = read_csv(path, header=None, nrows=10, skipinitialspace=True,
+                   encoding=encoding, sep=sep)
+    _offset_stream()
+    df1 = read_csv(path, nrows=10, skipinitialspace=True, encoding=encoding, sep=sep)
+    # If the column is numerical, its dtype is different without/with header
+    # TODO how about categorical columns
+    _offset_stream()
+    return tuple(df0.dtypes) != tuple(df1.dtypes)
+
+
+def ends_with_json(path):
+    return re.match(r".+\.json", path, re.IGNORECASE) is not None
+
+
+def read_data_from_csv(path, na_values=None, header=None, sep=","):
+    """
+    Read data set from csv or other delimited text file. And remove empty
+    columns (all values are null).
+    """
+    from pandas import read_csv
+
+    try:
+        header = header or ('infer' if has_header(path, sep=sep) else None)
+        df = read_csv(path, skipinitialspace=True, na_values=na_values,
+                      header=header, sep=sep, float_precision='high')
+    except (UnicodeDecodeError, NameError):
+        header = header or ('infer' if has_header(path, encoding='latin1',
+                                                  sep=sep) else None)
+        df = read_csv(path, skipinitialspace=True, na_values=na_values,
+                      header=header, encoding='latin1', sep=sep,
+                      float_precision='high')
+
+    # Remove columns with empty active domain, i.e., all values are missing.
+    before_attrs = set(df.columns)
+    df.dropna(axis=1, how='all')
+    after_attrs = set(df.columns)
+    if len(before_attrs) > len(after_attrs):
+        print(
+            f'Empty columns are removed, include {before_attrs - after_attrs}.')
+    # Remove rows with all empty values
+    df.dropna(axis=0, how='all')
+    if header is None:
+        df = df.rename(lambda x: f'#{x}', axis='columns')
+    return df
+
+
+def write_csv(file, data):
+    """ write data to csv files """
+    # if data is not a list of list, make it:
+    if isinstance(data, list) and not isinstance(data[0], list):
+        data = [data]
+    with open(file, 'a') as f:
+        writer = csv.writer(f, lineterminator='\n')
+        writer.writerows(data)
+    f.close()
+
+
+def file_name(path):
+    """ Return the file name without extension from a path. """
+    return os.path.splitext(os.path.basename(path))[0]
+
+
+def str_to_list(val, separator=','):
+    """
+    Split one string to a list by separator.
+    """
+    if val is None:
+        return None
+    return val.split(separator)
+
+
+# ---------------------------------------------------------------
+# Utilities for Plotting
+
+
+def _compress_svg_data(svg: str):
+    value = re.sub(r'\n', ' ', svg)
+    value = re.sub(r' {2,}', ' ', value)
+    value = re.sub(r'<style type="text/css">.*</style>', '', value)
+    value = re.sub(r'<!--(.*?)-->', '', value)
+    value = re.sub(r'<\?xml.*\?>', '', value)
+    value = re.sub(r'<!DOCTYPE.*dtd">', '', value)
+    return value.strip()
+
+
+def _prepare_for_cjk_characters(chars):
+    """ If input string has Chinese, Japanese, and Korean characters, set
+    specific font for them. """
+    has_cjk = False
+    for c in chars:
+        if any([start <= ord(c) <= end for start, end in [
+            (4352, 4607), (11904, 42191), (43072, 43135), (44032, 55215),
+            (63744, 64255), (65072, 65103), (65381, 65500), (131072, 196607)
+        ]]):
+            has_cjk = True
+            break
+    if has_cjk:
+        import matplotlib
+        matplotlib.rcParams['font.family'] = ['Microsoft Yahei']
+
+
+def plot_confusion_matrix(matrix: DataFrame, title='',
+                          ylabel='Predicted', xlabel='Actual',
+                          otype='string', path=None, cmap='Blues',
+                          vrange=None):
+    """
+    Plot a confusion matrix to show predict and actual values.
+
+    Parameters
+    ----------
+    matrix : pandas.DataFrame
+        the matrix to plot
+
+    title : str
+        title of image
+
+    ylabel : str
+        label in y-axis of image
+
+    xlabel : str
+        label in x-axis of image
+
+    otype : str
+        output type, support 'string' (default), 'file', 'show'
+
+    path : str
+        output path for 'file' type, default is 'matrix_2_3.svg' ((2, 3) is the
+        shape of matrix).
+
+    cmap : str
+        color
+
+    vrange : 2-tuple
+        manually set range of matrix
+    """
+    import matplotlib.pyplot as plt
+    _prepare_for_cjk_characters(''.join(map(str, matrix.columns)))
+    figsize = (6.4, 4.8)
+    n_columns = matrix.columns.size
+    if n_columns > 9:
+        from math import ceil
+        width = 6.4 + ceil((n_columns - 9) / 2) * 0.8
+        height = width * figsize[1] / figsize[0]
+        figsize = (width, height)
+    fig = plt.figure(figsize=figsize)
+    ax = fig.add_subplot(111)
+    if vrange is None:
+        vrange = (matrix.values.min(), matrix.values.max())
+    exp = len(str(vrange[1])) - 1
+    if exp > 2:
+        matrix = matrix.div(10 ** exp)
+        vrange = (vrange[0] / (10 ** exp), vrange[1] / (10 ** exp))
+    im = ax.imshow(matrix.values, cmap=cmap, vmin=vrange[0], vmax=vrange[1])
+    ax.set(xticks=np.arange(matrix.shape[1]),
+           yticks=np.arange(matrix.shape[0]),
+           xticklabels=matrix.columns,
+           yticklabels=matrix.index,
+           title=title,
+           ylabel=ylabel,
+           xlabel=xlabel)
+    ax.tick_params(which='both', length=0)
+    for edge, spine in ax.spines.items():
+        spine.set_visible(False)
+
+    # Loop over data dimensions and create text annotations.
+    thresh = (vrange[0] + vrange[1]) / 2.
+    for i in range(matrix.shape[0]):
+        for j in range(matrix.shape[1]):
+            if exp > 2:
+                text = '{:.2f}'.format(matrix.iloc[i, j])
+            else:
+                text = matrix.iloc[i, j]
+            ax.text(j, i, text,
+                    ha="center", va="center",
+                    color="white" if matrix.iloc[i, j] > thresh else "black")
+    from ds4ml.metrics import error_rate
+    ax.set_title('Rate: {:.1%}'.format(error_rate(matrix)), fontsize=10)
+
+    cbar = ax.figure.colorbar(im, ax=ax, pad=0.03, aspect=30)
+    cbar.outline.set_visible(False)
+    if exp > 2:
+        cbar.ax.text(0, -0.1, f'(e+{exp})')
+    cbar.ax.tick_params(which='both', length=0)
+    fig.autofmt_xdate()
+    fig.tight_layout()
+    plt.subplots_adjust()
+    try:
+        if otype == 'string':
+            from io import StringIO
+            img = StringIO()
+            plt.savefig(img, format='svg', bbox_inches='tight')
+            return _compress_svg_data(img.getvalue())
+        elif otype == 'file':
+            if path is None:
+                path = 'matrix_{}_{}.svg'.format(matrix.shape[0],
+                                                 matrix.shape[1])
+            plt.savefig(path, bbox_inches='tight')
+            return path
+        elif otype == 'show':
+            plt.show()
+    finally:
+        plt.close()
+
+
+def plot_histogram(bins, heights, otype='string', path=None,
+                   x_label='', y_label='Frequency'):
+    """
+    Plot two bars.
+    Note: Because pyplot draws diagrams auto-scale, this function will provide
+    kinds of diagram patterns.
+    """
+    import matplotlib.pyplot as plt
+    _prepare_for_cjk_characters(''.join(map(str, bins)))
+    length = len(bins)
+    fig_width = 6.4
+    ticks = 22
+    if length < 5:
+        # make 7 bars to show the data
+        # insert 0 or '' to the center of array
+        # e.g. [3, 4] => [3, 0, 4], ['1', '2', '3'] => ['1', '', '2', '', '3'], ...
+        bins = list(map(str, bins))
+        bins = ',,'.join(bins).split(',')
+        heights = np.insert(heights, list(range(1, length)), 0, axis=1)
+        # pad 0 or '' to array in the begin and end
+        pad = (7 - len(bins)) // 2
+        bins = tuple([''] * pad + bins + [''] * pad)
+        heights = np.append(np.insert(heights, [0], [0] * pad, axis=1),
+                            np.zeros((len(heights), pad), dtype=int), axis=1)
+        length = 7
+    else:
+        # TODO: if count of bins is bigger than 33, and it is categorical, how?
+        if length >= 60:
+            bins = bins[:60]
+            heights = heights[:, :60]
+            length = 60
+        bins = tuple(map(str, bins))
+        length_ = [8, 12, 16, 20, 32, 42, 48, 60]
+        ticks_ = [22, 30, 36, 48, 76, 96, 108, 172]
+        width_ = [6.4, 9.6, 11.2, 11.2, 11.2, 14, 14, 15]
+        idx = len([i for i in length_ if length > i])
+        ticks = ticks_[idx]
+        fig_width = width_[idx]
+
+    x = np.arange(length)
+    fig = plt.figure(figsize=(fig_width, 4.8))
+    ax = fig.add_subplot(111)
+    width = length / ticks
+    diff = width / 2 + 0.01
+    ax.bar(x - diff, heights[0], width=width, color='#38bbe8')
+    ax.bar(x + diff, heights[1], width=width, color='#ffd56e')
+    ax.legend(['raw', 'synth'])
+    fig.autofmt_xdate()
+    # fig.tight_layout(pad=1.5)
+    plt.xticks(x, bins, fontsize=10)
+    plt.xlabel(x_label)
+    plt.ylabel(y_label)
+    plt.subplots_adjust()
+    try:
+        if otype == 'string':
+            from io import StringIO
+            img = StringIO()
+            plt.savefig(img, format='svg', bbox_inches='tight')
+            return _compress_svg_data(img.getvalue())
+        elif otype == 'file':
+            if path is None:
+                path = 'histogram_{}_{}.svg'.format(len(bins), len(heights))
+            plt.savefig(path, bbox_inches='tight')
+            return path
+        elif otype == 'show':
+            plt.show()
+    finally:
+        plt.close()
+
+
+def plot_heatmap(data, title='', otype='string', path=None, cmap='Blues'):
+    """
+    Plot a heatmap to show pairwise correlations (e.g. mutual information).
+
+    Parameters see <code>plot_confusion_matrix</code>
+    """
+    import matplotlib.pyplot as plt
+    _prepare_for_cjk_characters(''.join(data.columns))
+    fig = plt.figure()
+    ax = fig.add_subplot(111)
+    im = ax.imshow(data.values, cmap=cmap)
+
+    ax.set_title(title, fontsize=10)
+    ticks = np.arange(len(data.columns))
+    ax.set_xticks(ticks)
+    ax.set_xticklabels(data.columns)
+    ax.set_yticks(ticks)
+    ax.set_yticklabels(data.index)
+    ax.tick_params(which='both', length=0)
+    for edge, spine in ax.spines.items():
+        spine.set_visible(False)
+
+    # set color bar in the right
+    cbar = ax.figure.colorbar(im, ax=ax, pad=0.03, aspect=30)
+    cbar.outline.set_visible(False)
+    cbar.ax.tick_params(which='both', length=0)
+    fig.autofmt_xdate()
+    fig.tight_layout()
+    plt.subplots_adjust()
+    try:
+        if otype == 'string':
+            from io import StringIO
+            img = StringIO()
+            plt.savefig(img, format='svg', facecolor='#ebebeb',
+                        bbox_inches='tight')
+            return _compress_svg_data(img.getvalue())
+        elif otype == 'file':
+            if path is None:
+                path = 'heatmap_{}_{}.svg'.format(data.shape[0], data.shape[1])
+            plt.savefig(path, facecolor='#ebebeb', bbox_inches='tight')
+            return path
+        elif otype == 'show':
+            plt.show()
+    finally:
+        plt.close()
+
+
+# ---------------------------------------------------------------
+# Utilities for Metrics, ML
+
+def train_and_predict(x_train, y_train, x_test):
+    """
+    Predict <x, y> by SVM classifier, and compare with test data
+    """
+    from sklearn.svm import SVC
+    classifier = SVC(gamma='scale')
+    classifier.fit(x_train, y_train)
+    result = classifier.predict(x_test)
+    return result
+
+
+def is_integer_dataframe(data: DataFrame) -> bool:
+    from pandas.api.types import is_integer_dtype
+    for _type in data.dtypes:
+        if not is_integer_dtype(_type):
+            return False
+    return True
+
+
+def mutual_information(child: Series, parents: DataFrame | Series):
+    """
+    Mutual information of child (Series) and parents (DataFrame) distributions
+    """
+    from sklearn.metrics import normalized_mutual_info_score
+    if isinstance(parents, Series):
+        return normalized_mutual_info_score(child, parents)
+
+    if parents.shape[1] == 1:
+        parents = parents.iloc[:, 0]
+    else:
+        if is_integer_dataframe(parents):
+            parents = parents.astype(str)
+            lengths = parents.applymap(len).max()
+            parents = parents.apply(
+                lambda row: int('1' + ''.join(
+                    [s.zfill(w) for s, w in zip(row, lengths)])), axis=1)
+        else:
+            parents = parents.apply(lambda x: ' '.join(x.array), axis=1)
+    return normalized_mutual_info_score(child, parents)
+
+
+def normalize_distribution(frequencies):
+    frequencies = np.array(frequencies, dtype=float)
+    frequencies = frequencies.clip(0)
+    total = frequencies.sum()
+    if total > 0:
+        if np.isinf(total):
+            return normalize_distribution(np.isinf(frequencies))
+        else:
+            return frequencies / total
+    else:
+        return np.full_like(frequencies, 1 / frequencies.size)
+
+
+def normalize_range(start, stop, bins=20):
+    """
+    Return evenly spaced values within a given interval, and a dynamically
+    calculated step, to make number of bins close to 20. If integer interval,
+    the smallest step is 1; If float interval, the smallest step is 0.5.
+    """
+    from math import ceil, floor
+    if isinstance(start, int) and isinstance(stop, int):
+        step = ceil((stop - start) / bins)
+    else:
+        start = floor(start)
+        stop = ceil(stop)
+        step = (stop - start) / bins
+        step = ceil(step) if ceil(step) == round(step) else round(step) + 0.5
+    stop = step * (bins + 1) + start
+    return np.arange(start, stop, step)
+
+
+def is_datetime(value: str):
+    from dateutil.parser import parse
+    """
+    Detect a value is a datetime. Exclude some datetime literals (weekdays and
+    months) from method `dateutil.parser`.
+    """
+    literals = {'mon', 'monday', 'tue', 'tuesday', 'wed', 'wednesday', 'thu',
+                'thursday', 'fri', 'friday', 'sat', 'saturday', 'sun', 'sunday',
+                'jan', 'january', 'feb', 'february', 'mar', 'march', 'apr',
+                'april', 'may', 'jun', 'june', 'jul', 'july', 'aug', 'august',
+                'sep', 'sept', 'september', 'oct', 'october', 'nov', 'november',
+                'dec', 'december'}
+    try:
+        value = value.lower()
+        if value in literals:
+            return False
+        parse(value)
+        return True
+    except ValueError:
+        return False
+    except AttributeError:
+        return False
+
+
+def is_discrete_values(values: Series) -> bool:
+    unique_values = values.unique()
+    return len(unique_values) < len(values) * 0.8
+
+
+def randomize_string(length):
+    return ''.join(np.random.choice(list(ascii_lowercase), size=length))
+
+
+def pseudonymise_string(value):
+    """ pseudonymise a string by RIPEMD-160 hashes """
+    return hashlib.new('ripemd160', str(value).encode('utf-8')).hexdigest()
+
+
+# ---------------------------------------------------------------
+# Utilities for arguments parser
+
+
+class CustomFormatter(argparse.HelpFormatter):
+    def _format_action_invocation(self, action):
+        if not action.option_strings:
+            metavar, = self._metavar_formatter(action, action.dest)(1)
+            return metavar
+        else:
+            parts = []
+            # if the Optional doesn't take a value, format is:
+            #    -s, --long
+            if action.nargs == 0:
+                parts.extend(action.option_strings)
+
+            # if the Optional takes a value, format is:
+            #    -s ARGS, --long ARGS
+            # change to
+            #    -s, --long ARGS
+            else:
+                default = action.dest.upper()
+                args_string = self._format_args(action, default)
+                for option_string in action.option_strings:
+                    # parts.append('%s %s' % (option_string, args_string))
+                    parts.append('%s' % option_string)
+                parts[-1] += ' %s' % args_string
+            return ', '.join(parts)
```

### Comparing `ds4ml-0.3.4/ds4ml.egg-info/PKG-INFO` & `ds4ml-0.3.5/ds4ml.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1
-Name: ds4ml
-Version: 0.3.4
-Summary: A Python library for data synthesis and evaluation
-Home-page: https://github.com/SAP/data-synthesis-for-machine-learning
-Maintainer: Yan Zhao
-Maintainer-email: yan.zhao01@sap.com
-Project-URL: Bug Tracker, https://github.com/SAP/data-synthesis-for-machine-learning/issues
-Project-URL: Documentation, https://github.com/SAP/data-synthesis-for-machine-learning
-Project-URL: Source Code, https://github.com/SAP/data-synthesis-for-machine-learning
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-The recent enforcement of data privacy protection regulations, such as GDPR,
-has made data sharing more difficult. This tool intends to facilitate data
-sharing from a customer by synthesizing a dataset based on the original dataset
-for later machine learning.
-
-There are two parts to this tool:
-
-- Data synthesizer
-  Synthesize a dataset based on the original dataset. It accepts CSV data as
-  input, and output a synthesized dataset based on Differential Privacy. The
-  algorithm in the data synthesizer reference to the paper (
-  http://dimacs.rutgers.edu/~graham/pubs/papers/privbayes-tods.pdf).
-- Data utility evaluation
-  Evaluate the data utility for the synthesized dataset. The original dataset
-  and the synthesized dataset as the input, one utility evaluation report will
-  be generated with several indicators.
+Metadata-Version: 2.1
+Name: ds4ml
+Version: 0.3.5
+Summary: A Python library for data synthesis and evaluation
+Home-page: https://github.com/SAP/data-synthesis-for-machine-learning
+Maintainer: Yan Zhao
+Maintainer-email: yan.zhao01@sap.com
+Project-URL: Bug Tracker, https://github.com/SAP/data-synthesis-for-machine-learning/issues
+Project-URL: Documentation, https://github.com/SAP/data-synthesis-for-machine-learning
+Project-URL: Source Code, https://github.com/SAP/data-synthesis-for-machine-learning
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+The recent enforcement of data privacy protection regulations, such as GDPR,
+has made data sharing more difficult. This tool intends to facilitate data
+sharing from a customer by synthesizing a dataset based on the original dataset
+for later machine learning.
+
+There are two parts to this tool:
+
+- Data synthesizer
+  Synthesize a dataset based on the original dataset. It accepts CSV data as
+  input, and output a synthesized dataset based on Differential Privacy. The
+  algorithm in the data synthesizer reference to the paper (
+  http://dimacs.rutgers.edu/~graham/pubs/papers/privbayes-tods.pdf).
+- Data utility evaluation
+  Evaluate the data utility for the synthesized dataset. The original dataset
+  and the synthesized dataset as the input, one utility evaluation report will
+  be generated with several indicators.
```

### Comparing `ds4ml-0.3.4/ds4ml.egg-info/SOURCES.txt` & `ds4ml-0.3.5/ds4ml.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 ds4ml.egg-info/dependency_links.txt
 ds4ml.egg-info/entry_points.txt
 ds4ml.egg-info/requires.txt
 ds4ml.egg-info/top_level.txt
 ds4ml/command/__init__.py
 ds4ml/command/evaluate.py
 ds4ml/command/pattern.py
-ds4ml/command/runtest.py
 ds4ml/command/synthesize.py
 ds4ml/template/report.html
 tests/test_attribute.py
 tests/test_dataset.py
 tests/test_evaluator.py
 tests/test_metrics.py
 tests/test_synthesizer.py
```

### Comparing `ds4ml-0.3.4/setup.py` & `ds4ml-0.3.5/setup.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-#!/usr/bin/env python
-
-import os
-
-from setuptools import setup
-
-pwd = os.path.abspath(os.path.dirname(__file__))
-
-INSTALL_REQUIRES = [
-    'numpy >= 1.14.3',
-    'matplotlib >= 2.2.2',
-    'mako >= 1.2.2',
-    'pandas >= 0.24.2',
-    'scikit-learn >= 0.20.2',
-    'python-dateutil >= 2.7.3'
-]
-
-LONG_DESCRIPTION = """
-The recent enforcement of data privacy protection regulations, such as GDPR,
-has made data sharing more difficult. This tool intends to facilitate data
-sharing from a customer by synthesizing a dataset based on the original dataset
-for later machine learning.
-
-There are two parts to this tool:
-
-- Data synthesizer
-  Synthesize a dataset based on the original dataset. It accepts CSV data as
-  input, and output a synthesized dataset based on Differential Privacy. The
-  algorithm in the data synthesizer reference to the paper (
-  http://dimacs.rutgers.edu/~graham/pubs/papers/privbayes-tods.pdf).
-- Data utility evaluation
-  Evaluate the data utility for the synthesized dataset. The original dataset
-  and the synthesized dataset as the input, one utility evaluation report will
-  be generated with several indicators.
-"""
-
-about = {}
-with open(os.path.join(pwd, 'ds4ml', '__version__.py'), mode='r',
-          encoding='utf-8') as f:
-    exec(f.read(), about)
-
-
-def main():
-    setup(name=about['__title__'],
-          description=about['__description__'],
-          long_description=LONG_DESCRIPTION,
-          long_description_content_type='text/markdown',
-          url=about['__url__'],
-          project_urls={
-              "Bug Tracker": about['__url__'] + "/issues",
-              "Documentation": about['__url__'],
-              "Source Code": about['__url__'],
-          },
-          version=about['__version__'],
-          packages=['ds4ml', 'ds4ml.command'],
-          package_data={
-              '': ['template/*.html']
-          },
-          entry_points={
-              'console_scripts': [
-                  'data-pattern = ds4ml.command.pattern:main',
-                  'data-synthesize = ds4ml.command.synthesize:main',
-                  'data-evaluate = ds4ml.command.evaluate:main'
-              ]
-          },
-          maintainer=about['__maintainer__'],
-          maintainer_email=about['__maintainer_email__'],
-          install_requires=INSTALL_REQUIRES,
-          platform='any')
-
-
-if __name__ == '__main__':
-    main()
+#!/usr/bin/env python
+
+import os
+
+from setuptools import setup
+
+pwd = os.path.abspath(os.path.dirname(__file__))
+
+INSTALL_REQUIRES = [
+    'numpy >= 1.14.3',
+    'matplotlib >= 2.2.2',
+    'mako >= 1.2.2',
+    'pandas >= 0.24.2',
+    'scikit-learn >= 0.20.2',
+    'python-dateutil >= 2.7.3'
+]
+
+LONG_DESCRIPTION = """
+The recent enforcement of data privacy protection regulations, such as GDPR,
+has made data sharing more difficult. This tool intends to facilitate data
+sharing from a customer by synthesizing a dataset based on the original dataset
+for later machine learning.
+
+There are two parts to this tool:
+
+- Data synthesizer
+  Synthesize a dataset based on the original dataset. It accepts CSV data as
+  input, and output a synthesized dataset based on Differential Privacy. The
+  algorithm in the data synthesizer reference to the paper (
+  http://dimacs.rutgers.edu/~graham/pubs/papers/privbayes-tods.pdf).
+- Data utility evaluation
+  Evaluate the data utility for the synthesized dataset. The original dataset
+  and the synthesized dataset as the input, one utility evaluation report will
+  be generated with several indicators.
+"""
+
+about = {}
+with open(os.path.join(pwd, 'ds4ml', '__version__.py'), mode='r',
+          encoding='utf-8') as f:
+    exec(f.read(), about)
+
+
+def main():
+    setup(name=about['__title__'],
+          description=about['__description__'],
+          long_description=LONG_DESCRIPTION,
+          long_description_content_type='text/markdown',
+          url=about['__url__'],
+          project_urls={
+              "Bug Tracker": about['__url__'] + "/issues",
+              "Documentation": about['__url__'],
+              "Source Code": about['__url__'],
+          },
+          version=about['__version__'],
+          packages=['ds4ml', 'ds4ml.command'],
+          package_data={
+              '': ['template/*.html']
+          },
+          entry_points={
+              'console_scripts': [
+                  'data-pattern = ds4ml.command.pattern:main',
+                  'data-synthesize = ds4ml.command.synthesize:main',
+                  'data-evaluate = ds4ml.command.evaluate:main'
+              ]
+          },
+          maintainer=about['__maintainer__'],
+          maintainer_email=about['__maintainer_email__'],
+          install_requires=INSTALL_REQUIRES,
+          platform='any')
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `ds4ml-0.3.4/tests/test_attribute.py` & `ds4ml-0.3.5/tests/test_attribute.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,288 +1,294 @@
-
-from numpy import random, array_equal
-from pandas import Series
-from ds4ml.attribute import Attribute
-from ds4ml.utils import randomize_string
-
-size = 30
-
-
-def isclose(a, b):
-    from math import isclose
-    return isclose(a, b, rel_tol=1e-03)
-
-
-def test_integer_attribute():
-    ints = random.randint(1, 100, size)
-    attr = Attribute(Series(ints), name='ID', categorical=False)
-    assert attr.type == 'integer'
-    assert attr.name == 'ID'
-    assert attr.min_ >= 1
-    assert attr.max_ <= 100
-    assert len(attr.bins) == 20
-    assert isclose(sum(attr.prs), 1.0)
-
-    from .testdata import adults01
-    attr = Attribute(adults01['age'], categorical=True)
-    assert attr.type == 'integer'
-    assert attr.categorical
-
-
-def test_float_attribute():
-    floats = random.uniform(1, 100, size)
-    attr = Attribute(Series(floats, name='Float'))
-    assert attr.type == 'float'
-    assert attr.min_ >= 1
-    assert attr.max_ <= 100
-    assert len(attr.bins) == 20
-    assert isclose(sum(attr.prs), 1.0)
-
-
-def test_string_attribute():
-    strings = list(map(lambda x: randomize_string(5), range(size)))
-    attr = Attribute(Series(strings, name='String'), categorical=True)
-    assert attr.type == 'string'
-    assert attr.min_ == 5
-    assert attr.categorical
-
-
-def test_set_domain_for_integer_attribute():
-    ints = random.randint(1, 100, size)
-    attr = Attribute(Series(ints, name='Integer'))
-    assert attr.min_ >= 1
-    assert attr.max_ <= 100
-    attr.domain = [-2, 120]
-    assert attr.min_ == -2
-    assert attr.max_ == 120
-
-
-def test_set_domain_for_integer_categorical_attribute():
-    ints = random.randint(1, 100, size)
-    attr = Attribute(Series(ints, name='Integer'), categorical=True)
-    assert attr.bins[0] >= 1
-    assert attr.bins[-1] <= 100
-    attr.domain = [-2, 120]
-    assert attr.bins[0] == -2
-    assert attr.bins[-1] == 120
-
-
-def test_set_domain_for_float_attribute():
-    floats = random.uniform(1, 100, size)
-    attr = Attribute(Series(floats, name='Float'))
-    assert attr.min_ >= 1
-    assert attr.max_ <= 100
-    attr.domain = [-2, 120]
-    assert attr.min_ == -2
-    assert attr.max_ == 120
-
-
-def test_set_domain_for_string_attribute():
-    strings = list(map(lambda x: randomize_string(5), range(size)))
-    attr = Attribute(Series(strings, name='String'), categorical=True)
-    bins = attr.bins
-    attr.domain = ['a', 'b', 'China', 'USA']
-    assert len(bins) + 4 == len(attr.bins)
-
-
-def test_set_domain_for_datetime_attribute():
-    dates = ['05/29/1988', '06/22/1988', '07/30/1992', '07/30/1992',
-             '11/12/2000', '01/02/2001', '01/02/2001', '12/03/2001',
-             '07/09/2002', '10/22/2002']
-    attr = Attribute(Series(dates, name='String'), categorical=True)
-    bins = attr.bins
-    attr.domain = ['07/01/1997', '12/20/1999', '01/01/2004']
-    assert len(bins) + 3 == len(attr.bins)
-
-
-def test_counts_numerical_attribute():
-    ints = random.randint(1, 100, size)
-    attr = Attribute(Series(ints, name='Integer'))
-    counts = attr.counts(normalize=False)
-    assert sum(counts) == 30
-    assert len(counts) == 20
-    counts = attr.counts(bins=[0, 10, 20, 30, 100], normalize=False)
-    assert sum(counts) == 30
-    assert len(counts) == 4
-
-    # categorical ints
-    attr = Attribute(Series([1, 10, 11, 10, 20, 15, 16, 25], name='Integer'),
-                     categorical=True)
-    counts = attr.counts(normalize=False)
-    assert sum(counts) == 8
-    assert len(counts) == 7
-    counts = attr.counts(bins=[5, 10, 15], normalize=False)
-    assert sum(counts) == 3
-    assert len(counts) == 3
-
-
-def test_decimals_float_attribute():
-    floats = map(lambda v: round(v, 2), random.uniform(1, 10, size))
-    attr = Attribute(Series(floats, name='Float'))
-    assert attr.decimals() == 2
-
-
-def test_counts_datetimes():
-    dates = ['05/29/1988', '06/22/1988', '07/30/1992', '07/30/1992',
-             '11/12/2000', '01/02/2001', '01/02/2001', '12/03/2001',
-             '07/09/2002', '10/22/2002']
-    attr = Attribute(Series(dates, name='DateTime'), categorical=True)
-    counts = attr.counts(normalize=False)
-    assert sum(counts) == len(dates)
-    assert array_equal(counts, [1, 1, 2, 1, 2, 1, 1, 1])
-
-    counts = attr.counts(bins=['12/03/2001', '10/22/2002'], normalize=False)
-    assert array_equal(counts, [1, 1])
-
-
-def test_counts_categorical_attribute():
-    ints = random.randint(1, 10, size)
-    attr = Attribute(Series(ints, name='Integer'), categorical=True)
-    assert sum(attr.counts()) == 30
-
-
-def test_choice_integers():
-    ints = random.randint(1, 100, size)
-    attr = Attribute(Series(ints, name='Integer'))
-    assert len(attr.bins) == 20
-    choices = attr.choice()
-    assert len(choices) == size
-
-
-def test_choice_floats():
-    floats = random.uniform(1, 10, size)
-    attr = Attribute(Series(floats, name='Float'))
-    assert len(attr.bins) == 20
-    choices = attr.choice()
-    assert len(choices) == size
-
-
-def test_choice_strings():
-    strings = list(map(lambda x: randomize_string(5), range(size)))
-    attr = Attribute(Series(strings, name='String'))
-    choices = attr.choice()
-    assert len(choices) == size
-
-
-def test_choice_datetimes():
-    dates = ['05/29/1988', '06/22/1988', '07/30/1992', '01/02/2001',
-             '11/12/2000', '07/09/2002', '08/30/1998', '06/03/1997',
-             '10/22/2002', '12/03/2001']
-    attr = Attribute(Series(dates, name='DateTime'))
-    choices = attr.choice()
-    assert len(choices) == len(dates)
-
-
-def test_bin_indexes_ints():
-    ints = [3, 5, 7, 8, 7, 1, 10, 30, 16, 19]
-    attr = Attribute(Series(ints), name='ID', categorical=False)
-    indexes = attr.bin_indexes()
-    assert len(indexes) == len(ints)
-
-
-def test_bin_indexes_datetimes():
-    dates = ['05/29/1988', '06/22/1988', '07/30/1992', '07/30/1992',
-             '11/12/2000', '01/02/2001', '01/02/2001', '12/03/2001',
-             '07/09/2002', '10/22/2002']
-    attr = Attribute(Series(dates, name='DateTime'))
-    indexes = attr.bin_indexes()
-    assert len(indexes) == len(dates)
-
-
-def test_pseudonymize_strings():
-    strings = Series(['Abc', 'edf', 'Abc', 'take', '中国', 'edf', 'Abc'])
-    attr = Attribute(strings, name='String')
-    pseudonyms = attr.pseudonymize()
-    assert array_equal(strings.value_counts().values,
-                       pseudonyms.value_counts().values)
-
-
-def test_pseudonymize_ints():
-    ints = Series([11, 2, 3, 4, 5, 4, 3, 2, 3, 4, 11])
-    attr = Attribute(ints, name='Integer')
-    pseudonyms = attr.pseudonymize()
-    assert array_equal(ints.value_counts().values,
-                       pseudonyms.value_counts().values)
-
-
-def test_pseudonymize_floats():
-    floats = Series([11.5, 2.6, 3.0, 4.3, 5, 4.3, 3.0, 2.6, 3.0, 4.3, 11.6])
-    attr = Attribute(floats, name='Float')
-    pseudonyms = attr.pseudonymize()
-    assert array_equal(floats.value_counts().values,
-                       pseudonyms.value_counts().values)
-
-
-def test_pseudonym_dates():
-    ints = Series(['07/15/2019', '07/24/2019', '07/23/2019', '07/22/2019',
-                   '07/21/2019', '07/22/2019', '07/23/2019', '07/24/2019',
-                   '07/23/2019', '07/22/2019', '07/15/2019'])
-    attr = Attribute(ints, name='Date')
-    pseudonyms = attr.pseudonymize()
-    assert array_equal(ints.value_counts().values,
-                       pseudonyms.value_counts().values)
-
-
-def test_random_ints():
-    ints = [3, 5, 7, 8, 7, 1, 10, 30, 16, 19]
-    attr = Attribute(ints, name='Integer')
-    randoms = attr.random()
-    assert len(randoms) == len(ints)
-
-
-def test_random_datetimes():
-    datetimes = ['07/15/2019', '07/24/2019', '07/23/2019', '07/22/2019',
-                 '07/21/2019', '07/22/2019', '07/23/2019', '07/24/2019',
-                 '07/23/2019', '07/22/2019', '07/15/2019']
-    attr = Attribute(datetimes, name='Date')
-    randoms = attr.random()
-    assert len(randoms) == len(datetimes)
-
-
-def test_random_strings():
-    strings = list(map(lambda x: randomize_string(5), range(size)))
-    attr = Attribute(Series(strings, name='String'))
-    randoms = attr.random()
-    assert len(randoms) == size
-
-
-def test_retain_ints():
-    ints = [3, 5, 7, 8, 7, 1, 10, 30, 16, 19]
-    attr = Attribute(ints, name='Integer')
-    retains = attr.retain()
-    assert len(retains) == len(ints)
-
-    retains = attr.retain(size=15)
-    assert array_equal(retains.head(len(ints)).tolist(), ints)
-
-
-def test_encode_numerical_attributes():
-    from .testdata import adults01
-    attr = Attribute(adults01['age'])
-    assert attr.bins[0] <= 19
-    assert attr.bins[-1] >= 56
-    assert len(attr.encode()) == len(attr)
-
-    from sklearn.model_selection import train_test_split
-    train, test = train_test_split(adults01['age'])
-    assert len(attr.encode(data=train)) == len(train)
-
-
-def test_encode_categorical_attributes():
-    from pandas import DataFrame
-    from .testdata import adults01
-    frame = DataFrame(adults01)
-    attr = Attribute(frame['education'], categorical=True)
-    columns = ['11th', '7th-8th', '9th', 'Assoc-acdm', 'Bachelors', 'Doctorate',
-               'HS-grad', 'Masters', 'Some-college']
-    assert array_equal(attr.bins, columns)
-    assert array_equal(attr.encode().columns, columns)
-
-
-def test_encode_datetime_attributes():
-    from pandas import DataFrame
-    from .testdata import adults01
-    frame = DataFrame(adults01)
-    attr = Attribute(frame['birth'])
-    # assert other information
-    assert len(attr.encode()) == len(attr)
-
+
+from numpy import random, array_equal
+from pandas import Series
+from ds4ml.attribute import Attribute
+from ds4ml.utils import randomize_string
+
+size = 30
+
+
+def isclose(a, b):
+    from math import isclose
+    return isclose(a, b, rel_tol=1e-03)
+
+
+def test_integer_attribute():
+    ints = random.randint(1, 100, size)
+    attr = Attribute(Series(ints), name='ID', categorical=False)
+    assert attr.type == 'integer'
+    assert attr.name == 'ID'
+    assert attr.min_ >= 1
+    assert attr.max_ <= 100
+    assert len(attr.bins) == 20
+    assert isclose(sum(attr.prs), 1.0)
+
+    from .testdata import adults01
+    attr = Attribute(adults01['age'], categorical=True)
+    assert attr.type == 'integer'
+    assert attr.categorical
+
+
+def test_float_attribute():
+    floats = random.uniform(1, 100, size)
+    attr = Attribute(Series(floats, name='Float'))
+    assert attr.type == 'float'
+    assert attr.min_ >= 1
+    assert attr.max_ <= 100
+    assert len(attr.bins) == 20
+    assert isclose(sum(attr.prs), 1.0)
+
+
+def test_string_attribute():
+    strings = list(map(lambda x: randomize_string(5), range(size)))
+    attr = Attribute(Series(strings, name='String'), categorical=True)
+    assert attr.type == 'string'
+    assert attr.min_ == 5
+    assert attr.categorical
+
+
+def test_set_domain_for_integer_attribute():
+    ints = random.randint(1, 100, size)
+    attr = Attribute(Series(ints, name='Integer'))
+    assert attr.min_ >= 1
+    assert attr.max_ <= 100
+    attr.domain = [-2, 120]
+    assert attr.min_ == -2
+    assert attr.max_ == 120
+
+
+def test_set_domain_for_integer_categorical_attribute():
+    ints = random.randint(1, 100, size)
+    attr = Attribute(Series(ints, name='Integer'), categorical=True)
+    assert attr.bins[0] >= 1
+    assert attr.bins[-1] <= 100
+    attr.domain = [-2, 120]
+    assert attr.bins[0] == -2
+    assert attr.bins[-1] == 120
+
+
+def test_set_domain_for_float_attribute():
+    floats = random.uniform(1, 100, size)
+    attr = Attribute(Series(floats, name='Float'))
+    assert attr.min_ >= 1
+    assert attr.max_ <= 100
+    attr.domain = [-2, 120]
+    assert attr.min_ == -2
+    assert attr.max_ == 120
+
+
+def test_set_domain_for_string_attribute():
+    strings = list(map(lambda x: randomize_string(5), range(size)))
+    attr = Attribute(Series(strings, name='String'), categorical=True)
+    bins = attr.bins
+    attr.domain = ['a', 'b', 'China', 'USA']
+    assert len(bins) + 4 == len(attr.bins)
+
+
+def test_set_domain_for_datetime_attribute():
+    dates = ['05/29/1988', '06/22/1988', '07/30/1992', '07/30/1992',
+             '11/12/2000', '01/02/2001', '01/02/2001', '12/03/2001',
+             '07/09/2002', '10/22/2002']
+    attr = Attribute(Series(dates, name='String'), categorical=True)
+    bins = attr.bins
+    attr.domain = ['07/01/1997', '12/20/1999', '01/01/2004']
+    assert len(bins) + 3 == len(attr.bins)
+
+
+def test_counts_numerical_attribute():
+    ints = random.randint(1, 100, size)
+    attr = Attribute(Series(ints, name='Integer'))
+    counts = attr.counts(normalize=False)
+    assert sum(counts) == 30
+    assert len(counts) == 20
+    counts = attr.counts(bins=[0, 10, 20, 30, 100], normalize=False)
+    assert sum(counts) == 30
+    assert len(counts) == 4
+
+    # categorical ints
+    attr = Attribute(Series([1, 10, 11, 10, 20, 15, 16, 25], name='Integer'),
+                     categorical=True)
+    counts = attr.counts(normalize=False)
+    assert sum(counts) == 8
+    assert len(counts) == 7
+    counts = attr.counts(bins=[5, 10, 15], normalize=False)
+    assert sum(counts) == 3
+    assert len(counts) == 3
+
+
+def test_decimals_float_attribute():
+    floats = map(lambda v: round(v, 2), random.uniform(1, 10, size))
+    attr = Attribute(Series(floats, name='Float'))
+    assert attr.decimals() == 2
+
+
+def test_counts_datetimes():
+    dates = ['05/29/1988', '06/22/1988', '07/30/1992', '07/30/1992',
+             '11/12/2000', '01/02/2001', '01/02/2001', '12/03/2001',
+             '07/09/2002', '10/22/2002']
+    attr = Attribute(Series(dates, name='DateTime'), categorical=True)
+    counts = attr.counts(normalize=False)
+    assert sum(counts) == len(dates)
+    assert array_equal(counts, [1, 1, 2, 1, 2, 1, 1, 1])
+
+    counts = attr.counts(bins=['12/03/2001', '10/22/2002'], normalize=False)
+    assert array_equal(counts, [1, 1])
+
+
+def test_counts_categorical_attribute():
+    ints = random.randint(1, 10, size)
+    attr = Attribute(Series(ints, name='Integer'), categorical=True)
+    assert sum(attr.counts()) == 30
+
+
+def test_choice_integers():
+    ints = random.randint(1, 100, size)
+    attr = Attribute(Series(ints, name='Integer'))
+    assert len(attr.bins) == 20
+    choices = attr.choice()
+    assert len(choices) == size
+
+
+def test_choice_floats():
+    floats = random.uniform(1, 10, size)
+    attr = Attribute(Series(floats, name='Float'))
+    assert len(attr.bins) == 20
+    choices = attr.choice()
+    assert len(choices) == size
+
+
+def test_choice_strings():
+    strings = list(map(lambda x: randomize_string(5), range(size)))
+    attr = Attribute(Series(strings, name='String'))
+    choices = attr.choice()
+    assert len(choices) == size
+
+
+def test_choice_datetimes():
+    dates = ['05/29/1988', '06/22/1988', '07/30/1992', '01/02/2001',
+             '11/12/2000', '07/09/2002', '08/30/1998', '06/03/1997',
+             '10/22/2002', '12/03/2001']
+    attr = Attribute(Series(dates, name='DateTime'))
+    choices = attr.choice()
+    assert len(choices) == len(dates)
+
+
+def test_bin_indexes_ints():
+    ints = [3, 5, 7, 8, 7, 1, 10, 30, 16, 19]
+    attr = Attribute(Series(ints), name='ID', categorical=False)
+    indexes = attr.bin_indexes()
+    assert len(indexes) == len(ints)
+
+
+def test_bin_indexes_datetimes():
+    dates = ['05/29/1988', '06/22/1988', '07/30/1992', '07/30/1992',
+             '11/12/2000', '01/02/2001', '01/02/2001', '12/03/2001',
+             '07/09/2002', '10/22/2002']
+    attr = Attribute(Series(dates, name='DateTime'))
+    indexes = attr.bin_indexes()
+    assert len(indexes) == len(dates)
+
+
+def test_pseudonymize_strings():
+    strings = Series(['Abc', 'edf', 'Abc', 'take', '中国', 'edf', 'Abc'])
+    attr = Attribute(strings, name='String')
+    pseudonyms = attr.pseudonymize()
+    assert array_equal(strings.value_counts().values,
+                       pseudonyms.value_counts().values)
+
+
+def test_pseudonymize_ints():
+    ints = Series([11, 2, 3, 4, 5, 4, 3, 2, 3, 4, 11])
+    attr = Attribute(ints, name='Integer')
+    pseudonyms = attr.pseudonymize()
+    assert array_equal(ints.value_counts().values,
+                       pseudonyms.value_counts().values)
+
+
+def test_pseudonymize_floats():
+    floats = Series([11.5, 2.6, 3.0, 4.3, 5, 4.3, 3.0, 2.6, 3.0, 4.3, 11.6])
+    attr = Attribute(floats, name='Float')
+    pseudonyms = attr.pseudonymize()
+    assert array_equal(floats.value_counts().values,
+                       pseudonyms.value_counts().values)
+
+
+def test_pseudonym_dates():
+    ints = Series(['07/15/2019', '07/24/2019', '07/23/2019', '07/22/2019',
+                   '07/21/2019', '07/22/2019', '07/23/2019', '07/24/2019',
+                   '07/23/2019', '07/22/2019', '07/15/2019'])
+    attr = Attribute(ints, name='Date')
+    pseudonyms = attr.pseudonymize()
+    assert array_equal(ints.value_counts().values,
+                       pseudonyms.value_counts().values)
+
+
+def test_random_ints():
+    ints = [3, 5, 7, 8, 7, 1, 10, 30, 16, 19]
+    attr = Attribute(ints, name='Integer')
+    randoms = attr.random()
+    assert len(randoms) == len(ints)
+
+
+def test_random_datetimes():
+    datetimes = ['07/15/2019', '07/24/2019', '07/23/2019', '07/22/2019',
+                 '07/21/2019', '07/22/2019', '07/23/2019', '07/24/2019',
+                 '07/23/2019', '07/22/2019', '07/15/2019']
+    attr = Attribute(datetimes, name='Date')
+    randoms = attr.random()
+    assert len(randoms) == len(datetimes)
+
+
+def test_random_strings():
+    strings = list(map(lambda x: randomize_string(5), range(size)))
+    attr = Attribute(Series(strings, name='String'))
+    randoms = attr.random()
+    assert len(randoms) == size
+
+
+def test_retain_ints():
+    ints = [3, 5, 7, 8, 7, 1, 10, 30, 16, 19]
+    attr = Attribute(ints, name='Integer')
+    retains = attr.retain()
+    assert len(retains) == len(ints)
+
+    retains = attr.retain(size=15)
+    assert array_equal(retains.head(len(ints)).tolist(), ints)
+
+
+def test_encode_numerical_attributes():
+    from .testdata import adults01
+    attr = Attribute(adults01['age'])
+    assert attr.bins[0] <= 19
+    assert attr.bins[-1] >= 56
+    assert len(attr.encode()) == len(attr)
+
+    from sklearn.model_selection import train_test_split
+    train, test = train_test_split(adults01['age'])
+    assert len(attr.encode(data=train)) == len(train)
+
+
+def test_encode_categorical_attributes():
+    from pandas import DataFrame
+    from .testdata import adults01
+    frame = DataFrame(adults01)
+    attr = Attribute(frame['education'], categorical=True)
+    columns = ['11th', '7th-8th', '9th', 'Assoc-acdm', 'Bachelors', 'Doctorate',
+               'HS-grad', 'Masters', 'Some-college']
+    assert array_equal(attr.bins, columns)
+    assert array_equal(attr.encode().columns, columns)
+
+    attr = Attribute(frame['education'].astype('category'))
+    columns = ['11th', '7th-8th', '9th', 'Assoc-acdm', 'Bachelors', 'Doctorate',
+               'HS-grad', 'Masters', 'Some-college']
+    assert array_equal(attr.bins, columns)
+    assert array_equal(attr.encode().columns, columns)
+
+
+def test_encode_datetime_attributes():
+    from pandas import DataFrame
+    from .testdata import adults01
+    frame = DataFrame(adults01)
+    attr = Attribute(frame['birth'])
+    # assert other information
+    assert len(attr.encode()) == len(attr)
+
```

### Comparing `ds4ml-0.3.4/tests/test_dataset.py` & `ds4ml-0.3.5/tests/test_dataset.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-
-from pandas import DataFrame
-from numpy import array_equal
-
-from ds4ml.dataset import DataSet
-
-from .testdata import adults01
-
-
-def test_encode():
-    from .testdata import adults01
-    from numpy import array_equal
-    dataset = DataSet(adults01)
-    frame = dataset.encode()
-    for col in ['education', 'relationship', 'salary']:
-        assert col not in frame.columns
-    for col in ['age', 'birth']:
-        assert col in frame.columns
-
-    assert 'salary_<=50K' in frame.columns
-    assert 'salary_>50K' in frame.columns
-
-    for attr, val in [('salary', '<=50K'),
-                      ('relationship', 'Wife'),
-                      ('relationship', 'Husband')]:
-        trans_col = frame[f'{attr}_{val}'].apply(lambda v: v == 1)
-        origin_col = adults01[attr] == val
-        assert array_equal(trans_col, origin_col)
-
-
-def test_encode_partly():
-    from .testdata import adults01
-    from sklearn.model_selection import train_test_split
-    dataset = DataSet(adults01)
-    train, test = train_test_split(adults01, test_size=0.2)
-    frame = dataset.encode(data=train)
-    assert 'salary_<=50K' in frame.columns
-    assert 'salary_>50K' in frame.columns
-    assert ((0 == frame['salary_<=50K']) | (frame['salary_<=50K'] == 1)).all()
-    assert ((0.0 <= frame['age']) & (frame['age'] <= 1.0)).all()
-
-
-def test_encode_empty_column():
-    from numpy import array_equal
-    data = [[1001, 'A', 'Female'],
-            [1002, 'B', 'Male'],
-            [1003, 'C', 'Male'],
-            [1004, 'D', 'Female'],
-            [1005, 'E', 'Female']]
-    ds = DataSet(data, columns=['ID', 'Name', 'Sex'])
-    x = DataFrame(data[-2:], columns=['ID', 'Name', 'Sex'])
-    x_tf = ds.encode(data=x)
-    # Name is not categorical, because it has unique values
-    assert x_tf.shape == (2, 3)
-    assert array_equal(x_tf.columns.tolist(), ['ID', 'Sex_Female', 'Sex_Male'])
-
-
-def test_svm_task():
-    from sklearn.svm import SVC
-    from sklearn.model_selection import train_test_split
-    from .testdata import adults01
-    c_df = DataFrame(adults01)
-    c_tf = DataSet(c_df).encode()
-    train, test = train_test_split(c_tf, test_size=0.2)
-
-    def make_train_x_y(df):
-        x_ = df.drop(['salary_<=50K', 'salary_>50K'], axis=1)
-        # <=50K and >50K are binary, complementary
-        _, ym_ = df['salary_<=50K'], df['salary_>50K']
-        return x_, ym_
-
-    tr_x, tr_y = make_train_x_y(train)
-    te_x, te_y = make_train_x_y(test)
-    clf = SVC(gamma='scale')
-    clf.fit(tr_x, tr_y)
-    pr_y = clf.predict(te_x)
-    from sklearn.metrics import confusion_matrix, classification_report
-    print(confusion_matrix(te_y, pr_y))
-    print(classification_report(te_y, pr_y))
-
-
-def test_synthesize():
-    dataset = DataSet(adults01)
-    df = dataset.synthesize()
-    assert df.size == dataset.size
-
-
-def test_synthesize_for_one_column():
-    dataset = DataSet(adults01[['age']])
-    df = dataset.synthesize()
-    assert df.size == adults01[['age']].size
-    assert min(df['age']) <= max(dataset['age'])
-    assert min(dataset['age']) <= max(df['age'])
-
-
-def test_to_pattern_for_one_column():
-    dataset = DataSet(adults01[['age']])
-    pattern = dataset.to_pattern()
-    assert pattern['network'] is None
-    assert 'age' in pattern['prs']
-
-
-def test_synthesize_from_pattern():
-    pattern = {'attrs':
-                   {'age': {'name': 'age', 'type': 'integer',
-                            'categorical': False, 'min': 19, 'max': 59,
-                            'decimals': None,
-                            'bins': [19.0, 21.0, 23.0, 25.0, 27.0, 29.0, 31.0,
-                                     33.0, 35.0, 37.0, 39.0, 41.0, 43.0, 45.0,
-                                     47.0, 49.0, 51.0, 53.0, 55.0, 57.0],
-                            'prs': [0.067, 0.0, 0.067, 0.033, 0.033, 0.033, 0.1,
-                                    0.033, 0.0333, 0.1333, 0.1011, 0.033, 0.0667,
-                                    0.0, 0.0, 0.1, 0.0333, 0.0667, 0.0333, 0.0333]
-                            }
-                    },
-               'config': {'pseudonyms': None},
-               'network': None,
-               'prs': {'age': [0.06049, 0.0293, 0.079, 0.0, 0.035, 0.002, 0.090,
-                               0.0581, 0.0357, 0.151, 0.084, 0.00892, 0.06809,
-                               0.0047, 0.0316, 0.1161, 0.042, 0.064, 0.04, 0.0]},
-               'records': 30}
-    df = DataSet.from_pattern(pattern).synthesize()
-    assert df.size == 30
-
-
-def test_synthesize_with_pseudonyms():
-    dataset = DataSet(adults01)
-    df = dataset.synthesize(pseudonyms=['salary'])
-    assert df.size == dataset.size
-    assert array_equal(dataset['salary'].value_counts().values,
-                       df['salary'].value_counts().values)
-
-
-def test_synthesize_with_retains():
-    dataset = DataSet(adults01)
-    df = dataset.synthesize(retains=['age'])
-    assert df.size == dataset.size
-    assert array_equal(dataset['age'], df['age'])
-
-
-def test_synthesize_for_privacy():
-    # Verify probability after synthesis by differential privacy. (This test
-    # case may fail because of limit runs.)
-    from numpy.random import randint
-    from numpy import exp
-    epsilon = 0.1
-    runs = 200
-    data = randint(65, 90, size=(199, 2))
-    set1 = DataSet(data.tolist() + [[65, 65]], columns=['ColA', 'ColB'])
-    set2 = DataSet(data.tolist() + [[65, 66]], columns=['ColA', 'ColB'])
-    counts = [0, 0]
-    for i in range(runs):
-        df1 = set1.synthesize(epsilon=epsilon)
-        df2 = set2.synthesize(epsilon=epsilon)
-        counts[0] += ((df1['ColA'] == 65) & (df1['ColB'] == 65)).sum()
-        counts[1] += ((df2['ColA'] == 65) & (df2['ColB'] == 66)).sum()
-    assert counts[0] / (runs * 200) <= exp(epsilon) * counts[1] / (runs * 200)
+
+from pandas import DataFrame
+from numpy import array_equal
+
+from ds4ml.dataset import DataSet
+
+from .testdata import adults01
+
+
+def test_encode():
+    from .testdata import adults01
+    from numpy import array_equal
+    dataset = DataSet(adults01)
+    frame = dataset.encode()
+    for col in ['education', 'relationship', 'salary']:
+        assert col not in frame.columns
+    for col in ['age', 'birth']:
+        assert col in frame.columns
+
+    assert 'salary_<=50K' in frame.columns
+    assert 'salary_>50K' in frame.columns
+
+    for attr, val in [('salary', '<=50K'),
+                      ('relationship', 'Wife'),
+                      ('relationship', 'Husband')]:
+        trans_col = frame[f'{attr}_{val}'].apply(lambda v: v == 1)
+        origin_col = adults01[attr] == val
+        assert array_equal(trans_col, origin_col)
+
+
+def test_encode_partly():
+    from .testdata import adults01
+    from sklearn.model_selection import train_test_split
+    dataset = DataSet(adults01)
+    train, test = train_test_split(adults01, test_size=0.2)
+    frame = dataset.encode(data=train)
+    assert 'salary_<=50K' in frame.columns
+    assert 'salary_>50K' in frame.columns
+    assert ((0 == frame['salary_<=50K']) | (frame['salary_<=50K'] == 1)).all()
+    assert ((0.0 <= frame['age']) & (frame['age'] <= 1.0)).all()
+
+
+def test_encode_empty_column():
+    from numpy import array_equal
+    data = [[1001, 'A', 'Female'],
+            [1002, 'B', 'Male'],
+            [1003, 'C', 'Male'],
+            [1004, 'D', 'Female'],
+            [1005, 'E', 'Female']]
+    ds = DataSet(data, columns=['ID', 'Name', 'Sex'])
+    x = DataFrame(data[-2:], columns=['ID', 'Name', 'Sex'])
+    x_tf = ds.encode(data=x)
+    # Name is not categorical, because it has unique values
+    assert x_tf.shape == (2, 3)
+    assert array_equal(x_tf.columns.tolist(), ['ID', 'Sex_Female', 'Sex_Male'])
+
+
+def test_svm_task():
+    from sklearn.svm import SVC
+    from sklearn.model_selection import train_test_split
+    from .testdata import adults01
+    c_df = DataFrame(adults01)
+    c_tf = DataSet(c_df).encode()
+    train, test = train_test_split(c_tf, test_size=0.2)
+
+    def make_train_x_y(df):
+        x_ = df.drop(['salary_<=50K', 'salary_>50K'], axis=1)
+        # <=50K and >50K are binary, complementary
+        _, ym_ = df['salary_<=50K'], df['salary_>50K']
+        return x_, ym_
+
+    tr_x, tr_y = make_train_x_y(train)
+    te_x, te_y = make_train_x_y(test)
+    clf = SVC(gamma='scale')
+    clf.fit(tr_x, tr_y)
+    pr_y = clf.predict(te_x)
+    from sklearn.metrics import confusion_matrix, classification_report
+    print(confusion_matrix(te_y, pr_y))
+    print(classification_report(te_y, pr_y))
+
+
+def test_synthesize():
+    dataset = DataSet(adults01)
+    df = dataset.synthesize()
+    assert df.size == dataset.size
+
+
+def test_synthesize_for_one_column():
+    dataset = DataSet(adults01[['age']])
+    df = dataset.synthesize()
+    assert df.size == adults01[['age']].size
+    assert min(df['age']) <= max(dataset['age'])
+    assert min(dataset['age']) <= max(df['age'])
+
+
+def test_to_pattern_for_one_column():
+    dataset = DataSet(adults01[['age']])
+    pattern = dataset.to_pattern()
+    assert pattern['network'] is None
+    assert 'age' in pattern['prs']
+
+
+def test_synthesize_from_pattern():
+    pattern = {'attrs':
+                   {'age': {'name': 'age', 'type': 'integer',
+                            'categorical': False, 'min': 19, 'max': 59,
+                            'decimals': None,
+                            'bins': [19.0, 21.0, 23.0, 25.0, 27.0, 29.0, 31.0,
+                                     33.0, 35.0, 37.0, 39.0, 41.0, 43.0, 45.0,
+                                     47.0, 49.0, 51.0, 53.0, 55.0, 57.0],
+                            'prs': [0.067, 0.0, 0.067, 0.033, 0.033, 0.033, 0.1,
+                                    0.033, 0.0333, 0.1333, 0.1011, 0.033, 0.0667,
+                                    0.0, 0.0, 0.1, 0.0333, 0.0667, 0.0333, 0.0333]
+                            }
+                    },
+               'config': {'pseudonyms': None},
+               'network': None,
+               'prs': {'age': [0.06049, 0.0293, 0.079, 0.0, 0.035, 0.002, 0.090,
+                               0.0581, 0.0357, 0.151, 0.084, 0.00892, 0.06809,
+                               0.0047, 0.0316, 0.1161, 0.042, 0.064, 0.04, 0.0]},
+               'records': 30}
+    df = DataSet.from_pattern(pattern).synthesize()
+    assert df.size == 30
+
+
+def test_synthesize_with_pseudonyms():
+    dataset = DataSet(adults01)
+    df = dataset.synthesize(pseudonyms=['salary'])
+    assert df.size == dataset.size
+    assert array_equal(dataset['salary'].value_counts().values,
+                       df['salary'].value_counts().values)
+
+
+def test_synthesize_with_retains():
+    dataset = DataSet(adults01)
+    df = dataset.synthesize(retains=['age'])
+    assert df.size == dataset.size
+    assert array_equal(dataset['age'], df['age'])
+
+
+def test_synthesize_for_privacy():
+    # Verify probability after synthesis by differential privacy. (This test
+    # case may fail because of limit runs.)
+    from numpy.random import randint
+    from numpy import exp
+    epsilon = 0.1
+    runs = 200
+    data = randint(65, 90, size=(199, 2))
+    set1 = DataSet(data.tolist() + [[65, 65]], columns=['ColA', 'ColB'])
+    set2 = DataSet(data.tolist() + [[65, 66]], columns=['ColA', 'ColB'])
+    counts = [0, 0]
+    for i in range(runs):
+        df1 = set1.synthesize(epsilon=epsilon)
+        df2 = set2.synthesize(epsilon=epsilon)
+        counts[0] += ((df1['ColA'] == 65) & (df1['ColB'] == 65)).sum()
+        counts[1] += ((df2['ColA'] == 65) & (df2['ColB'] == 66)).sum()
+    assert counts[0] / (runs * 200) <= exp(epsilon) * counts[1] / (runs * 200)
```

### Comparing `ds4ml-0.3.4/tests/test_evaluator.py` & `ds4ml-0.3.5/tests/test_evaluator.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-
-from pandas import DataFrame
-from ds4ml.evaluator import BiFrame, split_feature_class
-from ds4ml.dataset import DataSet
-from numpy import array_equal
-
-from .testdata import adults01, adults02
-
-
-def test_corr():
-    frame = BiFrame(DataFrame(adults01), DataFrame(adults02))
-    a_mi, b_mi = frame.corr()
-    from numpy import allclose, alltrue
-    assert allclose(a_mi, a_mi.T)
-    assert alltrue(a_mi >= 0.0)
-    assert alltrue(a_mi <= 1.0)
-    assert allclose(b_mi, b_mi.T)
-    assert alltrue(b_mi >= 0.0)
-    assert alltrue(b_mi <= 1.0)
-
-
-def test_dist():
-    frame = BiFrame(DataFrame(adults01), DataFrame(adults02))
-    columns = ['age', 'education', 'relationship', 'salary', 'birth']
-    for col in columns:
-        bins, counts = frame.dist(col)
-        assert len(bins) == len(counts[0])
-        assert len(bins) == len(counts[1])
-
-
-def test_describe():
-    frame = BiFrame(DataFrame(adults01), DataFrame(adults02))
-    desc = frame.describe()
-    from numpy import alltrue
-    columns = ['age', 'birth', 'education', 'relationship', 'salary']
-    # 'sex' not in adults01
-    assert array_equal(desc.columns, columns)
-    assert alltrue(desc >= 0.0)
-    assert alltrue(desc <= 1.0)
-    assert array_equal(desc.index, ['err', 'jsd'])
-
-
-def test_split_feature_class():
-    frame = DataSet(adults01[['age', 'relationship', 'salary']].head(10)).encode()
-    features1, class1 = split_feature_class('birth', frame)
-    assert features1.equals(frame)
-    assert class1 is None
-
-    features2, class2 = split_feature_class('age', frame)
-    assert features2.equals(frame)
-    assert class2 is None
-
-    features3, class3 = split_feature_class('salary', frame)
-    assert len(features3.columns) == 4
-    assert class3.name == 'salary_>50K'
-
-    features4, class4 = split_feature_class('relationship', frame)
-    assert len(features4.columns) == 3
-    assert class4.min() == 0
-    assert class4.max() == 2
-
-
-def test_classify_one_class():
-    frame = BiFrame(DataFrame(adults01), DataFrame(adults02))
-    matrix = frame.classify('salary')
-    assert len(matrix) == 2
-    assert array_equal(matrix[0].columns, ['<=50K', '>50K'])
-    assert array_equal(matrix[0].index, ['<=50K', '>50K'])
-
-
-def test_classify_multiple_classes():
-    frame = BiFrame(DataFrame(adults01), DataFrame(adults02))
-    matrix = frame.classify('education')
-    assert len(matrix) == 2
-    columns = ['11th', '7th-8th', '9th', 'Assoc-acdm', 'Assoc-voc', 'Bachelors',
-               'Doctorate', 'HS-grad', 'Masters', 'Some-college']
-    assert array_equal(matrix[0].columns, columns)
-    assert array_equal(matrix[0].index, columns)
-    assert array_equal(matrix[1].columns, columns)
-    assert array_equal(matrix[1].index, columns)
-
-
-def test_to_html():
-    frame = BiFrame(DataFrame(adults01), DataFrame(adults02))
-    report = 'a.html'
-    frame.to_html(report, labels=['education'])
-    import os.path
-    assert os.path.isfile(report)
-    if os.path.exists(report):
-        os.remove(report)
+
+from pandas import DataFrame
+from ds4ml.evaluator import BiFrame, split_feature_class
+from ds4ml.dataset import DataSet
+from numpy import array_equal
+
+from .testdata import adults01, adults02
+
+
+def test_corr():
+    frame = BiFrame(DataFrame(adults01), DataFrame(adults02))
+    a_mi, b_mi = frame.corr()
+    from numpy import allclose, alltrue
+    assert allclose(a_mi, a_mi.T)
+    assert alltrue(a_mi >= 0.0)
+    assert alltrue(a_mi <= 1.0)
+    assert allclose(b_mi, b_mi.T)
+    assert alltrue(b_mi >= 0.0)
+    assert alltrue(b_mi <= 1.0)
+
+
+def test_dist():
+    frame = BiFrame(DataFrame(adults01), DataFrame(adults02))
+    columns = ['age', 'education', 'relationship', 'salary', 'birth']
+    for col in columns:
+        bins, counts = frame.dist(col)
+        assert len(bins) == len(counts[0])
+        assert len(bins) == len(counts[1])
+
+
+def test_describe():
+    frame = BiFrame(DataFrame(adults01), DataFrame(adults02))
+    desc = frame.describe()
+    from numpy import alltrue
+    columns = ['age', 'birth', 'education', 'relationship', 'salary']
+    # 'sex' not in adults01
+    assert array_equal(desc.columns, columns)
+    assert alltrue(desc >= 0.0)
+    assert alltrue(desc <= 1.0)
+    assert array_equal(desc.index, ['err', 'jsd'])
+
+
+def test_split_feature_class():
+    frame = DataSet(adults01[['age', 'relationship', 'salary']].head(10)).encode()
+    features1, class1 = split_feature_class('birth', frame)
+    assert features1.equals(frame)
+    assert class1 is None
+
+    features2, class2 = split_feature_class('age', frame)
+    assert features2.equals(frame)
+    assert class2 is None
+
+    features3, class3 = split_feature_class('salary', frame)
+    assert len(features3.columns) == 4
+    assert class3.name == 'salary_>50K'
+
+    features4, class4 = split_feature_class('relationship', frame)
+    assert len(features4.columns) == 3
+    assert class4.min() == 0
+    assert class4.max() == 2
+
+
+def test_classify_one_class():
+    frame = BiFrame(DataFrame(adults01), DataFrame(adults02))
+    matrix = frame.classify('salary')
+    assert len(matrix) == 2
+    assert array_equal(matrix[0].columns, ['<=50K', '>50K'])
+    assert array_equal(matrix[0].index, ['<=50K', '>50K'])
+
+
+def test_classify_multiple_classes():
+    frame = BiFrame(DataFrame(adults01), DataFrame(adults02))
+    matrix = frame.classify('education')
+    assert len(matrix) == 2
+    columns = ['11th', '7th-8th', '9th', 'Assoc-acdm', 'Assoc-voc', 'Bachelors',
+               'Doctorate', 'HS-grad', 'Masters', 'Some-college']
+    assert array_equal(matrix[0].columns, columns)
+    assert array_equal(matrix[0].index, columns)
+    assert array_equal(matrix[1].columns, columns)
+    assert array_equal(matrix[1].index, columns)
+
+
+def test_to_html():
+    frame = BiFrame(DataFrame(adults01), DataFrame(adults02))
+    report = 'a.html'
+    frame.to_html(report, labels=['education'])
+    import os.path
+    assert os.path.isfile(report)
+    if os.path.exists(report):
+        os.remove(report)
```

### Comparing `ds4ml-0.3.4/tests/test_metrics.py` & `ds4ml-0.3.5/tests/test_metrics.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-
-from ds4ml.metrics import (pairwise_mutual_information,
-                           relative_error, error_rate)
-
-
-def test_pairwise_mutual_information():
-    from pandas import DataFrame
-    from .testdata import adults01
-    frame = DataFrame(adults01)
-    mi = pairwise_mutual_information(frame)
-    from numpy import allclose, alltrue
-    assert allclose(mi, mi.T)
-    assert alltrue(mi >= 0.0)
-    assert alltrue(mi <= 1.0)
-
-
-def test_error_rate():
-    from sklearn.metrics import accuracy_score
-    from numpy.random import randint
-    from numpy import isclose
-    y_true = [2, 0, 2, 2, 0, 1]
-    y_pred = [0, 0, 2, 2, 0, 2]
-    # its confusion matrix:
-    # 2 0 0
-    # 0 0 1
-    # 1 0 2
-    assert isclose(error_rate(y_true, y_pred), 0.3333)
-    for _ in range(10):
-        y_true = randint(0, 20, 100)
-        y_pred = randint(0, 20, 100)
-        assert isclose(error_rate(y_true, y_pred),
-                       1 - accuracy_score(y_true, y_pred))
-
-
-def test_relative_error():
-    from numpy import array, random
-    a = array([0, 1, 0])
-    b = array([1, 1, 0])
-    assert relative_error(a, b) == 0.3333
-
-    for _ in range(10):
-        size = random.randint(5, 100)
-        x = random.choice(20, size)
-        y = random.choice(20, size)
-        assert 0.0 <= relative_error(x, y) <= 1.0
-        x = random.rand(size)
-        y = random.rand(size)
-        assert 0.0 <= relative_error(x, y) <= 1.0
-
+
+from ds4ml.metrics import (pairwise_mutual_information,
+                           relative_error, error_rate)
+
+
+def test_pairwise_mutual_information():
+    from pandas import DataFrame
+    from .testdata import adults01
+    frame = DataFrame(adults01)
+    mi = pairwise_mutual_information(frame)
+    from numpy import allclose, alltrue
+    assert allclose(mi, mi.T)
+    assert alltrue(mi >= 0.0)
+    assert alltrue(mi <= 1.0)
+
+
+def test_error_rate():
+    from sklearn.metrics import accuracy_score
+    from numpy.random import randint
+    from numpy import isclose
+    y_true = [2, 0, 2, 2, 0, 1]
+    y_pred = [0, 0, 2, 2, 0, 2]
+    # its confusion matrix:
+    # 2 0 0
+    # 0 0 1
+    # 1 0 2
+    assert isclose(error_rate(y_true, y_pred), 0.3333)
+    for _ in range(10):
+        y_true = randint(0, 20, 100)
+        y_pred = randint(0, 20, 100)
+        assert isclose(error_rate(y_true, y_pred),
+                       1 - accuracy_score(y_true, y_pred))
+
+
+def test_relative_error():
+    from numpy import array, random
+    a = array([0, 1, 0])
+    b = array([1, 1, 0])
+    assert relative_error(a, b) == 0.3333
+
+    for _ in range(10):
+        size = random.randint(5, 100)
+        x = random.choice(20, size)
+        y = random.choice(20, size)
+        assert 0.0 <= relative_error(x, y) <= 1.0
+        x = random.rand(size)
+        y = random.rand(size)
+        assert 0.0 <= relative_error(x, y) <= 1.0
+
```

### Comparing `ds4ml-0.3.4/tests/test_synthesizer.py` & `ds4ml-0.3.5/tests/test_synthesizer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-
-from .testdata import adults01
-
-
-def test_calculate_degree():
-    from ds4ml.synthesizer import calculate_degree
-    degree = calculate_degree(8140, 6, 0.05)
-    assert 0 < degree <= 6 / 2
-
-
-def test_greedy_bayes():
-    from pandas import DataFrame
-    from ds4ml.synthesizer import greedy_bayes
-    network = greedy_bayes(DataFrame(adults01), epsilon=0.1)
-    assert network[0][0] in adults01.columns
-    assert type(network[0][1]) == list
-
-
-def test_noisy_distributions():
-    from ds4ml.synthesizer import noisy_distributions
-    from pandas import DataFrame
-    dataset = DataFrame([
-        [1, 0, 40],
-        [1, 1, 42],
-        [0, 0, 30],
-        [0, 1, 30],
-        [1, 1, 36],
-        [1, 1, 50],
-        [0, 0, 32],
-        [0, 0, 28]
-    ], columns=['salary', 'sex', 'age'])
-    columns = ['salary', 'sex']
-    epsilon = 0.05
-    noisy = noisy_distributions(dataset, columns, epsilon)
-    assert noisy.shape == (4, 3)
-    assert len(noisy[noisy['freq'] >= 0]) == 4
-
-
-def test_noisy_distributions_for_one_column():
-    from ds4ml.synthesizer import noisy_distributions
-    from pandas import DataFrame
-    dataset = DataFrame([
-        [1, 0, 40],
-        [1, 1, 42],
-        [0, 0, 30],
-        [0, 1, 30],
-        [1, 1, 36],
-        [1, 1, 50],
-        [0, 0, 32],
-        [0, 0, 28]
-    ], columns=['salary', 'sex', 'age'])
-    columns = ['sex']
-    epsilon = 0.05
-    noisy = noisy_distributions(dataset, columns, epsilon)
-    assert noisy.shape == (2, 2)
-    assert len(noisy[noisy['freq'] >= 0]) == 2
-
-    columns = ['age']
-    epsilon = 0.05
-    noisy = noisy_distributions(dataset[['age']], columns, epsilon)
-    assert noisy.shape[1] == 2
-
-
-def test_noisy_conditionals():
-    from ds4ml.synthesizer import noisy_conditionals
-    from pandas import DataFrame
-    dataset = DataFrame([
-        [1, 0, 40],
-        [1, 1, 42],
-        [0, 0, 30],
-        [0, 1, 30],
-        [1, 1, 36],
-        [1, 1, 50],
-        [0, 0, 32],
-        [0, 0, 28]
-    ], columns=['salary', 'sex', 'age'])
-    epsilon = 0.05
-    network = [('salary', ['sex']), ('age', ['sex', 'salary'])]
-    noisy = noisy_conditionals(network, dataset, epsilon)
-    assert len(noisy['sex']) == 2
-    assert (1.0 - sum(noisy['sex'])) < 1e-6
-    assert len(noisy['salary']) == 2
-    assert '[0]' in noisy['salary']
-    assert '[1]' in noisy['salary']
-    assert len(noisy['age']) == 4
-    assert '[0, 0]' in noisy['age']
-    assert '[0, 1]' in noisy['age']
-    assert '[1, 0]' in noisy['age']
-    assert '[1, 1]' in noisy['age']
+
+from .testdata import adults01
+from ds4ml.utils import FREQ_NAME
+
+def test_calculate_degree():
+    from ds4ml.synthesizer import calculate_degree
+    degree = calculate_degree(8140, 6, 0.05)
+    assert 0 < degree <= 6 / 2
+
+
+def test_greedy_bayes():
+    from pandas import DataFrame
+    from ds4ml.synthesizer import greedy_bayes
+    network = greedy_bayes(DataFrame(adults01), epsilon=0.1)
+    assert network[0][0] in adults01.columns
+    assert type(network[0][1]) == list
+
+
+def test_noisy_distributions():
+    from ds4ml.synthesizer import noisy_distributions
+    from pandas import DataFrame
+    dataset = DataFrame([
+        [1, 0, 40],
+        [1, 1, 42],
+        [0, 0, 30],
+        [0, 1, 30],
+        [1, 1, 36],
+        [1, 1, 50],
+        [0, 0, 32],
+        [0, 0, 28]
+    ], columns=['salary', 'sex', 'age'])
+    columns = ['salary', 'sex']
+    epsilon = 0.05
+    noisy = noisy_distributions(dataset, columns, epsilon)
+    assert noisy.shape == (4, 3)
+    assert len(noisy[noisy[FREQ_NAME] >= 0]) == 4
+
+
+def test_noisy_distributions_for_one_column():
+    from ds4ml.synthesizer import noisy_distributions
+    from pandas import DataFrame
+    dataset = DataFrame([
+        [1, 0, 40],
+        [1, 1, 42],
+        [0, 0, 30],
+        [0, 1, 30],
+        [1, 1, 36],
+        [1, 1, 50],
+        [0, 0, 32],
+        [0, 0, 28]
+    ], columns=['salary', 'sex', 'age'])
+    columns = ['sex']
+    epsilon = 0.05
+    noisy = noisy_distributions(dataset, columns, epsilon)
+    assert noisy.shape == (2, 2)
+    assert len(noisy[noisy[FREQ_NAME] >= 0]) == 2
+
+    columns = ['age']
+    epsilon = 0.05
+    noisy = noisy_distributions(dataset[['age']], columns, epsilon)
+    assert noisy.shape[1] == 2
+
+
+def test_noisy_conditionals():
+    from ds4ml.synthesizer import noisy_conditionals
+    from pandas import DataFrame
+    dataset = DataFrame([
+        [1, 0, 40],
+        [1, 1, 42],
+        [0, 0, 30],
+        [0, 1, 30],
+        [1, 1, 36],
+        [1, 1, 50],
+        [0, 0, 32],
+        [0, 0, 28]
+    ], columns=['salary', 'sex', 'age'])
+    epsilon = 0.05
+    network = [('salary', ['sex']), ('age', ['sex', 'salary'])]
+    noisy = noisy_conditionals(network, dataset, epsilon)
+    assert len(noisy['sex']) == 2
+    assert (1.0 - sum(noisy['sex'])) < 1e-6
+    assert len(noisy['salary']) == 2
+    assert '[0]' in noisy['salary']
+    assert '[1]' in noisy['salary']
+    assert len(noisy['age']) == 4
+    assert '[0, 0]' in noisy['age']
+    assert '[0, 1]' in noisy['age']
+    assert '[1, 0]' in noisy['age']
+    assert '[1, 1]' in noisy['age']
```

### Comparing `ds4ml-0.3.4/tests/testdata.py` & `ds4ml-0.3.5/tests/testdata.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-"""
-Test Data is from part of https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data
-"""
-from pandas import DataFrame
-
-adults01 = DataFrame([
-    [39, 'Bachelors', 'Not-in-family', '<=50K', '06/26/1980'],
-    [50, 'Bachelors', 'Husband', '<=50K', '06/18/1969'],
-    [38, 'HS-grad', 'Not-in-family', '<=50K', '06/27/1981'],
-    [53, '11th', 'Husband', '<=50K', '06/16/1966'],
-    [28, 'Bachelors', 'Wife', '<=50K', '07/05/1991'],
-    [37, 'Masters', 'Wife', '<=50K', '06/28/1982'],
-    [49, '9th', 'Not-in-family', '<=50K', '06/19/1970'],
-    [52, 'HS-grad', 'Husband', '>50K', '06/17/1967'],
-    [31, 'Masters', 'Not-in-family', '>50K', '07/02/1988'],
-    [42, 'Bachelors', 'Husband', '>50K', '06/24/1977'],
-    [37, 'Some-college', 'Husband', '>50K', '06/28/1982'],
-    [30, 'Bachelors', 'Husband', '>50K', '07/03/1989'],
-    [23, 'Bachelors', 'Own-child', '<=50K', '07/08/1996'],
-    [32, 'Bachelors', 'Not-in-family', '<=50K', '07/02/1987'],
-    [34, '7th-8th', 'Husband', '<=50K', '06/30/1985'],
-    [25, 'HS-grad', 'Own-child', '<=50K', '07/07/1994'],
-    [32, 'HS-grad', 'Unmarried', '<=50K', '07/02/1987'],
-    [38, '11th', 'Husband', '<=50K', '06/27/1981'],
-    [43, 'Masters', 'Unmarried', '>50K', '06/23/1976'],
-    [40, 'Doctorate', 'Husband', '>50K', '06/26/1979'],
-    [54, 'HS-grad', 'Unmarried', '<=50K', '06/15/1965'],
-    [35, '9th', 'Husband', '<=50K', '06/29/1984'],
-    [43, '11th', 'Husband', '<=50K', '06/23/1976'],
-    [59, 'HS-grad', 'Unmarried', '<=50K', '06/11/1960'],
-    [56, 'Bachelors', 'Husband', '>50K', '06/14/1963'],
-    [19, 'HS-grad', 'Own-child', '<=50K', '07/11/2000'],
-    [39, 'HS-grad', 'Not-in-family', '<=50K', '06/26/1980'],
-    [49, 'HS-grad', 'Husband', '<=50K', '06/19/1970'],
-    [23, 'Assoc-acdm', 'Not-in-family', '<=50K', '07/08/1996'],
-    [20, 'Some-college', 'Own-child', '<=50K', '07/11/1999']
-], columns=['age', 'education', 'relationship', 'salary', 'birth'])
-
-
-adults02 = DataFrame([
-    [19, 'HS-grad', 'Own-child', 'Male', '<=50K', '07/11/2000'],
-    [26, 'Bachelors', 'Own-child', 'Male', '<=50K', '07/06/1993'],
-    [27, 'Some-college', 'Not-in-family', 'Male', '<=50K', '07/05/1992'],
-    [41, 'Masters', 'Husband', 'Male', '<=50K', '06/25/1978'],
-    [33, 'Doctorate', 'Husband', 'Male', '<=50K', '07/01/1986'],
-    [56, 'Some-college', 'Not-in-family', 'Male', '<=50K', '06/14/1963'],
-    [43, 'Bachelors', 'Husband', 'Male', '>50K', '06/23/1976'],
-    [29, 'HS-grad', 'Wife', 'Female', '<=50K', '07/04/1990'],
-    [44, '11th', 'Husband', 'Male', '>50K', '06/23/1975'],
-    [37, 'Some-college', 'Own-child', 'Female', '<=50K', '06/28/1982'],
-    [24, 'Some-college', 'Not-in-family', 'Male', '<=50K', '07/08/1995'],
-    [38, 'HS-grad', 'Husband', 'Male', '<=50K', '06/27/1981'],
-    [35, 'Masters', 'Husband', 'Male', '>50K', '06/29/1984'],
-    [39, 'Bachelors', 'Own-child', 'Female', '<=50K', '06/26/1980'],
-    [47, 'HS-grad', 'Husband', 'Male', '>50K', '06/20/1972'],
-    [51, 'HS-grad', 'Husband', 'Male', '>50K', '06/17/1968'],
-    [38, 'HS-grad', 'Husband', 'Male', '<=50K', '06/27/1981'],
-    [44, 'Some-college', 'Unmarried', 'Female', '<=50K', '06/23/1975'],
-    [24, 'HS-grad', 'Other-relative', 'Female', '<=50K', '07/08/1995'],
-    [41, 'HS-grad', 'Unmarried', 'Female', '<=50K', '06/25/1978'],
-    [51, 'Assoc-voc', 'Unmarried', 'Female', '<=50K', '06/17/1968'],
-    [60, 'HS-grad', 'Husband', 'Male', '<=50K', '06/11/1959'],
-    [40, 'Bachelors', 'Husband', 'Male', '>50K', '06/26/1979'],
-    [27, 'Some-college', 'Wife', 'Female', '<=50K', '07/05/1992'],
-    [36, 'HS-grad', 'Husband', 'Male', '>50K', '06/29/1983'],
-    [44, 'HS-grad', 'Husband', 'Male', '<=50K', '06/23/1975'],
-    [33, 'Some-college', None, 'Female', '<=50K', '07/01/1986'],
-    [53, '7th-8th', 'Husband', 'Male', '<=50K', '06/16/1966'],
-    [43, 'HS-grad', 'Husband', 'Male', '>50K', '06/23/1976'],
-    [44, 'Assoc-acdm', 'Not-in-family', 'Male', '<=50K', '06/23/1975'],
-], columns=['age', 'education', 'relationship', 'sex', 'salary', 'birth'])
-
-adult_with_head = 'age, education, relationship, sex, salary, birth\n' \
-           '19, HS-grad, Own-child, Male, <=50K, 07/11/2000\n' \
-           '41, Masters, Husband, Male, <=50K, 06/25/1978\n' \
-           '44, HS-grad, Husband, Male, <=50K, 06/23/1975'
-
-
-adult_without_head = '19, HS-grad, Own-child, Male, <=50K, 07/11/2000\n' \
-           '41, Masters, Husband, Male, <=50K, 06/25/1978\n' \
-           '40, Masters, Husband, Female, <=50K, 06/21/1977\n' \
-           '44, HS-grad, Husband, Male, <=50K, 06/23/1975'
-
-
-adult_with_head_res = DataFrame([
-    [19, 'HS-grad', 'Own-child', 'Male', '<=50K', '07/11/2000'],
-    [41, 'Masters', 'Husband', 'Male', '<=50K', '06/25/1978'],
-    [44, 'HS-grad', 'Husband', 'Male', '<=50K', '06/23/1975']
+"""
+Test Data is from part of https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data
+"""
+from pandas import DataFrame
+
+adults01 = DataFrame([
+    [39, 'Bachelors', 'Not-in-family', '<=50K', '06/26/1980'],
+    [50, 'Bachelors', 'Husband', '<=50K', '06/18/1969'],
+    [38, 'HS-grad', 'Not-in-family', '<=50K', '06/27/1981'],
+    [53, '11th', 'Husband', '<=50K', '06/16/1966'],
+    [28, 'Bachelors', 'Wife', '<=50K', '07/05/1991'],
+    [37, 'Masters', 'Wife', '<=50K', '06/28/1982'],
+    [49, '9th', 'Not-in-family', '<=50K', '06/19/1970'],
+    [52, 'HS-grad', 'Husband', '>50K', '06/17/1967'],
+    [31, 'Masters', 'Not-in-family', '>50K', '07/02/1988'],
+    [42, 'Bachelors', 'Husband', '>50K', '06/24/1977'],
+    [37, 'Some-college', 'Husband', '>50K', '06/28/1982'],
+    [30, 'Bachelors', 'Husband', '>50K', '07/03/1989'],
+    [23, 'Bachelors', 'Own-child', '<=50K', '07/08/1996'],
+    [32, 'Bachelors', 'Not-in-family', '<=50K', '07/02/1987'],
+    [34, '7th-8th', 'Husband', '<=50K', '06/30/1985'],
+    [25, 'HS-grad', 'Own-child', '<=50K', '07/07/1994'],
+    [32, 'HS-grad', 'Unmarried', '<=50K', '07/02/1987'],
+    [38, '11th', 'Husband', '<=50K', '06/27/1981'],
+    [43, 'Masters', 'Unmarried', '>50K', '06/23/1976'],
+    [40, 'Doctorate', 'Husband', '>50K', '06/26/1979'],
+    [54, 'HS-grad', 'Unmarried', '<=50K', '06/15/1965'],
+    [35, '9th', 'Husband', '<=50K', '06/29/1984'],
+    [43, '11th', 'Husband', '<=50K', '06/23/1976'],
+    [59, 'HS-grad', 'Unmarried', '<=50K', '06/11/1960'],
+    [56, 'Bachelors', 'Husband', '>50K', '06/14/1963'],
+    [19, 'HS-grad', 'Own-child', '<=50K', '07/11/2000'],
+    [39, 'HS-grad', 'Not-in-family', '<=50K', '06/26/1980'],
+    [49, 'HS-grad', 'Husband', '<=50K', '06/19/1970'],
+    [23, 'Assoc-acdm', 'Not-in-family', '<=50K', '07/08/1996'],
+    [20, 'Some-college', 'Own-child', '<=50K', '07/11/1999']
+], columns=['age', 'education', 'relationship', 'salary', 'birth'])
+
+
+adults02 = DataFrame([
+    [19, 'HS-grad', 'Own-child', 'Male', '<=50K', '07/11/2000'],
+    [26, 'Bachelors', 'Own-child', 'Male', '<=50K', '07/06/1993'],
+    [27, 'Some-college', 'Not-in-family', 'Male', '<=50K', '07/05/1992'],
+    [41, 'Masters', 'Husband', 'Male', '<=50K', '06/25/1978'],
+    [33, 'Doctorate', 'Husband', 'Male', '<=50K', '07/01/1986'],
+    [56, 'Some-college', 'Not-in-family', 'Male', '<=50K', '06/14/1963'],
+    [43, 'Bachelors', 'Husband', 'Male', '>50K', '06/23/1976'],
+    [29, 'HS-grad', 'Wife', 'Female', '<=50K', '07/04/1990'],
+    [44, '11th', 'Husband', 'Male', '>50K', '06/23/1975'],
+    [37, 'Some-college', 'Own-child', 'Female', '<=50K', '06/28/1982'],
+    [24, 'Some-college', 'Not-in-family', 'Male', '<=50K', '07/08/1995'],
+    [38, 'HS-grad', 'Husband', 'Male', '<=50K', '06/27/1981'],
+    [35, 'Masters', 'Husband', 'Male', '>50K', '06/29/1984'],
+    [39, 'Bachelors', 'Own-child', 'Female', '<=50K', '06/26/1980'],
+    [47, 'HS-grad', 'Husband', 'Male', '>50K', '06/20/1972'],
+    [51, 'HS-grad', 'Husband', 'Male', '>50K', '06/17/1968'],
+    [38, 'HS-grad', 'Husband', 'Male', '<=50K', '06/27/1981'],
+    [44, 'Some-college', 'Unmarried', 'Female', '<=50K', '06/23/1975'],
+    [24, 'HS-grad', 'Other-relative', 'Female', '<=50K', '07/08/1995'],
+    [41, 'HS-grad', 'Unmarried', 'Female', '<=50K', '06/25/1978'],
+    [51, 'Assoc-voc', 'Unmarried', 'Female', '<=50K', '06/17/1968'],
+    [60, 'HS-grad', 'Husband', 'Male', '<=50K', '06/11/1959'],
+    [40, 'Bachelors', 'Husband', 'Male', '>50K', '06/26/1979'],
+    [27, 'Some-college', 'Wife', 'Female', '<=50K', '07/05/1992'],
+    [36, 'HS-grad', 'Husband', 'Male', '>50K', '06/29/1983'],
+    [44, 'HS-grad', 'Husband', 'Male', '<=50K', '06/23/1975'],
+    [33, 'Some-college', None, 'Female', '<=50K', '07/01/1986'],
+    [53, '7th-8th', 'Husband', 'Male', '<=50K', '06/16/1966'],
+    [43, 'HS-grad', 'Husband', 'Male', '>50K', '06/23/1976'],
+    [44, 'Assoc-acdm', 'Not-in-family', 'Male', '<=50K', '06/23/1975'],
+], columns=['age', 'education', 'relationship', 'sex', 'salary', 'birth'])
+
+adult_with_head = 'age, education, relationship, sex, salary, birth\n' \
+           '19, HS-grad, Own-child, Male, <=50K, 07/11/2000\n' \
+           '41, Masters, Husband, Male, <=50K, 06/25/1978\n' \
+           '44, HS-grad, Husband, Male, <=50K, 06/23/1975'
+
+
+adult_without_head = '19, HS-grad, Own-child, Male, <=50K, 07/11/2000\n' \
+           '41, Masters, Husband, Male, <=50K, 06/25/1978\n' \
+           '40, Masters, Husband, Female, <=50K, 06/21/1977\n' \
+           '44, HS-grad, Husband, Male, <=50K, 06/23/1975'
+
+
+adult_with_head_res = DataFrame([
+    [19, 'HS-grad', 'Own-child', 'Male', '<=50K', '07/11/2000'],
+    [41, 'Masters', 'Husband', 'Male', '<=50K', '06/25/1978'],
+    [44, 'HS-grad', 'Husband', 'Male', '<=50K', '06/23/1975']
 ], columns=['age', 'education', 'relationship', 'sex', 'salary', 'birth'])
```

