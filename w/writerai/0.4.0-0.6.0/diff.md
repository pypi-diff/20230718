# Comparing `tmp/writerai-0.4.0.tar.gz` & `tmp/writerai-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "writerai-0.4.0.tar", last modified: Mon Apr 17 12:53:39 2023, max compression
+gzip compressed data, was "writerai-0.6.0.tar", last modified: Wed Jun 28 20:43:22 2023, max compression
```

## Comparing `writerai-0.4.0.tar` & `writerai-0.6.0.tar`

### file list

```diff
@@ -1,129 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:53:39.080897 writerai-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-17 12:53:39.080897 writerai-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-17 12:53:29.000000 writerai-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 12:53:39.080897 writerai-0.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-04-17 12:53:29.000000 writerai-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:53:39.068897 writerai-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:53:39.072897 writerai-0.4.0/src/writer/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2710 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/ai_content_detector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2221 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/billing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4602 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/completions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4476 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/content.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4074 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/cowrite.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2434 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/download_the_customized_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6434 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6919 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/modelcustomization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:53:39.072897 writerai-0.4.0/src/writer/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:53:39.072897 writerai-0.4.0/src/writer/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2547 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1453 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/addterms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1424 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/contentcheck.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1598 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/contentcorrect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1459 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/createcompletion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1521 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/createmodelcustomization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1642 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/createmodelcustomizationcompletion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1155 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/deletefile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/deletemodelcustomization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1527 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/deletesnippets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1521 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/deleteterms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1381 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/detectcontent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1349 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/fetchcustomizedmodelfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2669 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/findsnippets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3087 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/findterms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/generate_content.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1178 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/getfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1400 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/getmodelcustomization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      941 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/getsubscriptiondetails.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1099 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/listfiles.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1277 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/listmodelcustomizations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1131 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/listmodels.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1593 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/listpages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1398 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/listtemplates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2131 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/listusers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1089 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/pagedetails.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1614 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/updatesnippets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1619 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/updateterms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/uploadfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:53:39.080897 writerai-0.4.0/src/writer/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4173 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1033 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/approvedtermextension.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      722 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/approvedtermextensioncreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      821 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/completiongenerationchoice.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1135 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/completiongenerationchoicelogprobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2288 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/completionrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      669 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/completionresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      437 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/contentdetectorrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/contentdetectorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2524 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/contentissue.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/contentrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2638 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/contentsettings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      437 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/correctionresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2076 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/createcustomizationrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1008 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/createtermsrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      890 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/createtermsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/customizationsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      433 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/deleteresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2033 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/draft.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      695 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/failmessage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/failresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1681 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/fulllinkedterm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4416 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/fulltermwithuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      765 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/generatetemplaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/generationmodelinforesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/generationmodelsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      454 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/hyperparameters.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2034 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/input.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      713 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/linkedtermcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/magicrequestinput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1638 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3026 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/modelcustomization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1249 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/modelfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      597 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/modelfilesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2186 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/pagepublicapiresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2370 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/pagewithsectionresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      975 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/paginatedresult_fulltermwithuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/paginatedresult_pagepublicapiresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      970 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/paginatedresult_snippetwithuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      985 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/paginatedresult_userpublicresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      685 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/pagination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      609 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/processedcontent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      652 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/sectioninfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      929 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/simpleuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/snippettagv2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1202 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/snippetupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2215 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/snippetwithuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2057 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/subscriptionpublicresponseapi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1926 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/templatedetailsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3209 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/termcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1104 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/termexample.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      675 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/termexamplecreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      807 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/terminologyuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1344 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/termmistake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/termmistakecreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/termtagcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      791 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/termtagresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3139 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/termupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1008 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/updatetermsrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      550 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/uploadmodelfilerequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      929 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/usage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      542 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/usageitem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2557 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/userpublicresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2259 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models_.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7161 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5524 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/snippet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3613 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/styleguide.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7285 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/terminology.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2288 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:53:39.080897 writerai-0.4.0/src/writer/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:53:39.080897 writerai-0.4.0/src/writerai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-17 12:53:38.000000 writerai-0.4.0/src/writerai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-17 12:53:38.000000 writerai-0.4.0/src/writerai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 12:53:38.000000 writerai-0.4.0/src/writerai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-17 12:53:38.000000 writerai-0.4.0/src/writerai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 12:53:38.000000 writerai-0.4.0/src/writerai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:43:22.529208 writerai-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-06-28 20:43:22.529208 writerai-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-28 20:43:09.000000 writerai-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 20:43:22.529208 writerai-0.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1154 2023-06-28 20:43:09.000000 writerai-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:43:22.517208 writerai-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:43:22.517208 writerai-0.6.0/src/writer/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2767 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/ai_content_detector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2049 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/billing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5360 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/completions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5209 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/content.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/cowrite.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4204 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/document.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2533 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/download_the_customized_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8114 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8864 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/modelcustomization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:43:22.517208 writerai-0.6.0/src/writer/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:43:22.521208 writerai-0.6.0/src/writer/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2824 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1431 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/addterms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1402 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/contentcheck.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1574 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/contentcorrect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1437 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/createcompletion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1499 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/createmodelcustomization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1618 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/createmodelcustomizationcompletion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1215 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/deletefile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1433 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/deletemodelcustomization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1503 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/deletesnippets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1497 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/deleteterms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1361 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/detectcontent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1327 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/fetchcustomizedmodelfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2619 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/findsnippets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3019 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/findterms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1398 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/generate_content.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1309 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/getdocumentdetails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1158 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/getfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/getmodelcustomization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      927 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/getsubscriptiondetails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1081 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/listfiles.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/listmodelcustomizations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1113 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/listmodels.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1563 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/listpages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2333 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/listteamdocuments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1376 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/listtemplates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2089 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/listusers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/pagedetails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1590 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/updatesnippets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1595 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/updateterms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1281 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/operations/uploadfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:43:22.529208 writerai-0.6.0/src/writer/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4247 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1021 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/approvedtermextension.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      714 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/approvedtermextensioncreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2280 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/briefdocument.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      938 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/briefdocuments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      815 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/completiongenerationchoice.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/completiongenerationchoicelogprobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2264 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/completionrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/completionresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      433 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/contentdetectorrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      683 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/contentdetectorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2502 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/contentissue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/contentrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2604 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/contentsettings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      433 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/correctionresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2056 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/createcustomizationrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/createtermsrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      884 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/createtermsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/customizationsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      429 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/deleteresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2385 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/document.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2009 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/draft.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      687 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/failmessage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      855 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/failresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1657 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/fulllinkedterm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4362 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/fulltermwithuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      759 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/generatetemplaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      803 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/generationmodelinforesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      669 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/generationmodelsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      450 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/hyperparameters.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2004 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/input.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      707 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/linkedtermcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      632 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/magicrequestinput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1612 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2996 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/modelcustomization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1235 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/modelfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      593 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/modelfilesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/pagepublicapiresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2340 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/pagewithsectionresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      967 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/paginatedresult_fulltermwithuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      992 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/paginatedresult_pagepublicapiresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/paginatedresult_snippetwithuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      977 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/paginatedresult_userpublicresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      679 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/pagination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      605 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/processedcontent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/sectioninfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      329 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      919 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/simpleuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      419 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/snippettagv2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1190 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/snippetupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2195 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/snippetwithuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2025 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/subscriptionpublicresponseapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/templatedetailsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3167 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/termcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1084 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/termexample.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      661 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/termexamplecreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      799 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/terminologyuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1322 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/termmistake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/termmistakecreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      420 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/termtagcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/termtagresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3097 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/termupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/updatetermsrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      540 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/uploadmodelfilerequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      919 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/usage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/usageitem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2525 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models/shared/userpublicresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2234 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/models_.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4461 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      892 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/sdkconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6739 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/snippet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4139 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/styleguide.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9118 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/terminology.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2133 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:43:22.529208 writerai-0.6.0/src/writer/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-06-28 20:43:09.000000 writerai-0.6.0/src/writer/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:43:22.529208 writerai-0.6.0/src/writerai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-06-28 20:43:22.000000 writerai-0.6.0/src/writerai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-06-28 20:43:22.000000 writerai-0.6.0/src/writerai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 20:43:22.000000 writerai-0.6.0/src/writerai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-28 20:43:22.000000 writerai-0.6.0/src/writerai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-28 20:43:22.000000 writerai-0.6.0/src/writerai.egg-info/top_level.txt
```

### Comparing `writerai-0.4.0/src/writer/ai_content_detector.py` & `writerai-0.6.0/src/writer/ai_content_detector.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,42 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-import requests as requests_http
-from . import utils
-from typing import Any, Optional
+from .sdkconfiguration import SDKConfiguration
+from typing import Optional
+from writer import utils
 from writer.models import operations, shared
 
 class AIContentDetector:
     r"""Methods related to AI Content Detector"""
-    _client: requests_http.Session
-    _security_client: requests_http.Session
-    _server_url: str
-    _language: str
-    _sdk_version: str
-    _gen_version: str
-    _globals: dict[str, dict[str, dict[str, Any]]]
+    sdk_configuration: SDKConfiguration
 
-    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str, gbls: dict[str, dict[str, dict[str, Any]]]) -> None:
-        self._client = client
-        self._security_client = security_client
-        self._server_url = server_url
-        self._language = language
-        self._sdk_version = sdk_version
-        self._gen_version = gen_version
-        self._globals = gbls
+    def __init__(self, sdk_config: SDKConfiguration) -> None:
+        self.sdk_configuration = sdk_config
         
-    def detect(self, request: operations.DetectContentRequest) -> operations.DetectContentResponse:
+    
+    def detect(self, content_detector_request: shared.ContentDetectorRequest, organization_id: Optional[int] = None) -> operations.DetectContentResponse:
         r"""Content detector api"""
-        base_url = self._server_url
+        request = operations.DetectContentRequest(
+            content_detector_request=content_detector_request,
+            organization_id=organization_id,
+        )
         
-        url = utils.generate_url(operations.DetectContentRequest, base_url, '/content/organization/{organizationId}/detect', request, self._globals)
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
+        url = utils.generate_url(operations.DetectContentRequest, base_url, '/content/organization/{organizationId}/detect', request, self.sdk_configuration.globals)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "content_detector_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.DetectContentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
```

### Comparing `writerai-0.4.0/src/writer/completions.py` & `writerai-0.6.0/src/writer/completions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-import requests as requests_http
-from . import utils
-from typing import Any, Optional
+from .sdkconfiguration import SDKConfiguration
+from typing import Optional
+from writer import utils
 from writer.models import operations, shared
 
 class Completions:
     r"""Methods related to Completions"""
-    _client: requests_http.Session
-    _security_client: requests_http.Session
-    _server_url: str
-    _language: str
-    _sdk_version: str
-    _gen_version: str
-    _globals: dict[str, dict[str, dict[str, Any]]]
-
-    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str, gbls: dict[str, dict[str, dict[str, Any]]]) -> None:
-        self._client = client
-        self._security_client = security_client
-        self._server_url = server_url
-        self._language = language
-        self._sdk_version = sdk_version
-        self._gen_version = gen_version
-        self._globals = gbls
+    sdk_configuration: SDKConfiguration
+
+    def __init__(self, sdk_config: SDKConfiguration) -> None:
+        self.sdk_configuration = sdk_config
         
-    def create(self, request: operations.CreateCompletionRequest) -> operations.CreateCompletionResponse:
+    
+    def create(self, completion_request: shared.CompletionRequest, model_id: str, organization_id: Optional[int] = None) -> operations.CreateCompletionResponse:
         r"""Create completion for LLM model"""
-        base_url = self._server_url
+        request = operations.CreateCompletionRequest(
+            completion_request=completion_request,
+            model_id=model_id,
+            organization_id=organization_id,
+        )
         
-        url = utils.generate_url(operations.CreateCompletionRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/completions', request, self._globals)
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
+        url = utils.generate_url(operations.CreateCompletionRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/completions', request, self.sdk_configuration.globals)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "completion_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateCompletionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -55,28 +51,37 @@
             
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
-    def create_model_customization_completion(self, request: operations.CreateModelCustomizationCompletionRequest) -> operations.CreateModelCustomizationCompletionResponse:
+    
+    def create_model_customization_completion(self, completion_request: shared.CompletionRequest, customization_id: str, model_id: str, organization_id: Optional[int] = None) -> operations.CreateModelCustomizationCompletionResponse:
         r"""Create completion for LLM customization model"""
-        base_url = self._server_url
+        request = operations.CreateModelCustomizationCompletionRequest(
+            completion_request=completion_request,
+            customization_id=customization_id,
+            model_id=model_id,
+            organization_id=organization_id,
+        )
         
-        url = utils.generate_url(operations.CreateModelCustomizationCompletionRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/customization/{customizationId}/completions', request, self._globals)
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
+        url = utils.generate_url(operations.CreateModelCustomizationCompletionRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/customization/{customizationId}/completions', request, self.sdk_configuration.globals)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "completion_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateModelCustomizationCompletionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
```

### Comparing `writerai-0.4.0/src/writer/content.py` & `writerai-0.6.0/src/writer/content.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-import requests as requests_http
-from . import utils
-from typing import Any, Optional
+from .sdkconfiguration import SDKConfiguration
+from typing import Optional
+from writer import utils
 from writer.models import operations, shared
 
 class Content:
     r"""Methods related to Content"""
-    _client: requests_http.Session
-    _security_client: requests_http.Session
-    _server_url: str
-    _language: str
-    _sdk_version: str
-    _gen_version: str
-    _globals: dict[str, dict[str, dict[str, Any]]]
-
-    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str, gbls: dict[str, dict[str, dict[str, Any]]]) -> None:
-        self._client = client
-        self._security_client = security_client
-        self._server_url = server_url
-        self._language = language
-        self._sdk_version = sdk_version
-        self._gen_version = gen_version
-        self._globals = gbls
+    sdk_configuration: SDKConfiguration
+
+    def __init__(self, sdk_config: SDKConfiguration) -> None:
+        self.sdk_configuration = sdk_config
         
-    def check(self, request: operations.ContentCheckRequest) -> operations.ContentCheckResponse:
+    
+    def check(self, content_request: shared.ContentRequest, team_id: int, organization_id: Optional[int] = None) -> operations.ContentCheckResponse:
         r"""Check your content against your preset styleguide."""
-        base_url = self._server_url
+        request = operations.ContentCheckRequest(
+            content_request=content_request,
+            team_id=team_id,
+            organization_id=organization_id,
+        )
         
-        url = utils.generate_url(operations.ContentCheckRequest, base_url, '/content/organization/{organizationId}/team/{teamId}/check', request, self._globals)
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
+        url = utils.generate_url(operations.ContentCheckRequest, base_url, '/content/organization/{organizationId}/team/{teamId}/check', request, self.sdk_configuration.globals)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "content_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ContentCheckResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -55,28 +51,37 @@
             
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
-    def correct(self, request: operations.ContentCorrectRequest) -> operations.ContentCorrectResponse:
+    
+    def correct(self, content_request: shared.ContentRequest, team_id: int, x_request_id: Optional[str] = None, organization_id: Optional[int] = None) -> operations.ContentCorrectResponse:
         r"""Apply the style guide suggestions directly to your content."""
-        base_url = self._server_url
+        request = operations.ContentCorrectRequest(
+            content_request=content_request,
+            team_id=team_id,
+            x_request_id=x_request_id,
+            organization_id=organization_id,
+        )
         
-        url = utils.generate_url(operations.ContentCorrectRequest, base_url, '/content/organization/{organizationId}/team/{teamId}/correct', request, self._globals)
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
+        url = utils.generate_url(operations.ContentCorrectRequest, base_url, '/content/organization/{organizationId}/team/{teamId}/correct', request, self.sdk_configuration.globals)
         headers = utils.get_headers(request)
         req_content_type, data, form = utils.serialize_request_body(request, "content_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ContentCorrectResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
```

### Comparing `writerai-0.4.0/src/writer/cowrite.py` & `writerai-0.6.0/src/writer/document.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,88 +1,83 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-import requests as requests_http
-from . import utils
-from typing import Any, Optional
+from .sdkconfiguration import SDKConfiguration
+from typing import Optional
+from writer import utils
 from writer.models import operations, shared
 
-class CoWrite:
-    r"""Methods related to CoWrite"""
-    _client: requests_http.Session
-    _security_client: requests_http.Session
-    _server_url: str
-    _language: str
-    _sdk_version: str
-    _gen_version: str
-    _globals: dict[str, dict[str, dict[str, Any]]]
-
-    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str, gbls: dict[str, dict[str, dict[str, Any]]]) -> None:
-        self._client = client
-        self._security_client = security_client
-        self._server_url = server_url
-        self._language = language
-        self._sdk_version = sdk_version
-        self._gen_version = gen_version
-        self._globals = gbls
-        
-    def generate_content(self, request: operations.GenerateContentRequest) -> operations.GenerateContentResponse:
-        r"""Generate content using predefined templates"""
-        base_url = self._server_url
+class Document:
+    r"""Methods related to document"""
+    sdk_configuration: SDKConfiguration
+
+    def __init__(self, sdk_config: SDKConfiguration) -> None:
+        self.sdk_configuration = sdk_config
+        
+    
+    def get(self, document_id: int, team_id: int, organization_id: Optional[int] = None) -> operations.GetDocumentDetailsResponse:
+        r"""Get document details"""
+        request = operations.GetDocumentDetailsRequest(
+            document_id=document_id,
+            team_id=team_id,
+            organization_id=organization_id,
+        )
         
-        url = utils.generate_url(operations.GenerateContentRequest, base_url, '/cowrite/organization/{organizationId}/team/{teamId}/generate', request, self._globals)
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
+        url = utils.generate_url(operations.GetDocumentDetailsRequest, base_url, '/organization/{organizationId}/team/{teamId}/document/{documentId}', request, self.sdk_configuration.globals)
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "generate_template_request", 'json')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        if data is None and form is None:
-            raise Exception('request body is required')
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
-        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GenerateContentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetDocumentDetailsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Draft])
-                res.draft = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Document])
+                res.document = out
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
-    def list_templates(self, request: operations.ListTemplatesRequest) -> operations.ListTemplatesResponse:
-        r"""Get a list of your existing CoWrite templates"""
-        base_url = self._server_url
-        
-        url = utils.generate_url(operations.ListTemplatesRequest, base_url, '/cowrite/organization/{organizationId}/team/{teamId}/template/{templateId}', request, self._globals)
+    
+    def list(self, request: operations.ListTeamDocumentsRequest) -> operations.ListTeamDocumentsResponse:
+        r"""List team documents"""
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
+        url = utils.generate_url(operations.ListTeamDocumentsRequest, base_url, '/organization/{organizationId}/team/{teamId}/document', request, self.sdk_configuration.globals)
+        headers = {}
+        query_params = utils.get_query_params(operations.ListTeamDocumentsRequest, request, self.sdk_configuration.globals)
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
-        http_res = client.request('GET', url)
+        http_res = client.request('GET', url, params=query_params, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListTemplatesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListTeamDocumentsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.TemplateDetailsResponse])
-                res.template_details_response = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.BriefDocuments])
+                res.brief_documents = out
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
```

### Comparing `writerai-0.4.0/src/writer/files.py` & `writerai-0.6.0/src/writer/files.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,76 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-import requests as requests_http
-from . import utils
-from typing import Any, Optional
+from .sdkconfiguration import SDKConfiguration
+from typing import Optional
+from writer import utils
 from writer.models import operations, shared
 
 class Files:
     r"""Methods related to Files"""
-    _client: requests_http.Session
-    _security_client: requests_http.Session
-    _server_url: str
-    _language: str
-    _sdk_version: str
-    _gen_version: str
-    _globals: dict[str, dict[str, dict[str, Any]]]
-
-    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str, gbls: dict[str, dict[str, dict[str, Any]]]) -> None:
-        self._client = client
-        self._security_client = security_client
-        self._server_url = server_url
-        self._language = language
-        self._sdk_version = sdk_version
-        self._gen_version = gen_version
-        self._globals = gbls
+    sdk_configuration: SDKConfiguration
+
+    def __init__(self, sdk_config: SDKConfiguration) -> None:
+        self.sdk_configuration = sdk_config
         
-    def delete(self, request: operations.DeleteFileRequest) -> operations.DeleteFileResponse:
+    
+    def delete(self, file_id: str, organization_id: Optional[int] = None) -> operations.DeleteFileResponse:
         r"""Delete file"""
-        base_url = self._server_url
+        request = operations.DeleteFileRequest(
+            file_id=file_id,
+            organization_id=organization_id,
+        )
         
-        url = utils.generate_url(operations.DeleteFileRequest, base_url, '/llm/organization/{organizationId}/file/{fileId}', request, self._globals)
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
+        url = utils.generate_url(operations.DeleteFileRequest, base_url, '/llm/organization/{organizationId}/file/{fileId}', request, self.sdk_configuration.globals)
+        headers = {}
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
-        http_res = client.request('DELETE', url)
+        http_res = client.request('DELETE', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.DeleteFileResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[dict[str, Any]])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.DeleteFile200ApplicationJSON])
                 res.delete_file_200_application_json_object = out
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
-    def get(self, request: operations.GetFileRequest) -> operations.GetFileResponse:
+    
+    def get(self, file_id: str, organization_id: Optional[int] = None) -> operations.GetFileResponse:
         r"""Get file"""
-        base_url = self._server_url
+        request = operations.GetFileRequest(
+            file_id=file_id,
+            organization_id=organization_id,
+        )
         
-        url = utils.generate_url(operations.GetFileRequest, base_url, '/llm/organization/{organizationId}/file/{fileId}', request, self._globals)
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
+        url = utils.generate_url(operations.GetFileRequest, base_url, '/llm/organization/{organizationId}/file/{fileId}', request, self.sdk_configuration.globals)
+        headers = {}
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
-        http_res = client.request('GET', url)
+        http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetFileResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
@@ -78,24 +82,31 @@
             
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
-    def list(self, request: operations.ListFilesRequest) -> operations.ListFilesResponse:
+    
+    def list(self, organization_id: Optional[int] = None) -> operations.ListFilesResponse:
         r"""List files"""
-        base_url = self._server_url
+        request = operations.ListFilesRequest(
+            organization_id=organization_id,
+        )
         
-        url = utils.generate_url(operations.ListFilesRequest, base_url, '/llm/organization/{organizationId}/file', request, self._globals)
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
+        url = utils.generate_url(operations.ListFilesRequest, base_url, '/llm/organization/{organizationId}/file', request, self.sdk_configuration.globals)
+        headers = {}
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
-        http_res = client.request('GET', url)
+        http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListFilesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
@@ -107,28 +118,35 @@
             
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
-    def upload(self, request: operations.UploadFileRequest) -> operations.UploadFileResponse:
+    
+    def upload(self, upload_model_file_request: shared.UploadModelFileRequest, organization_id: Optional[int] = None) -> operations.UploadFileResponse:
         r"""Upload file"""
-        base_url = self._server_url
+        request = operations.UploadFileRequest(
+            upload_model_file_request=upload_model_file_request,
+            organization_id=organization_id,
+        )
         
-        url = utils.generate_url(operations.UploadFileRequest, base_url, '/llm/organization/{organizationId}/file', request, self._globals)
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
+        url = utils.generate_url(operations.UploadFileRequest, base_url, '/llm/organization/{organizationId}/file', request, self.sdk_configuration.globals)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "upload_model_file_request", 'multipart')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.UploadFileResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
```

### Comparing `writerai-0.4.0/src/writer/modelcustomization.py` & `writerai-0.6.0/src/writer/snippet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,146 +1,127 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-import requests as requests_http
-from . import utils
-from typing import Any, Optional
+from .sdkconfiguration import SDKConfiguration
+from typing import Optional
+from writer import utils
 from writer.models import operations, shared
 
-class ModelCustomization:
-    r"""Methods related to Model Customization"""
-    _client: requests_http.Session
-    _security_client: requests_http.Session
-    _server_url: str
-    _language: str
-    _sdk_version: str
-    _gen_version: str
-    _globals: dict[str, dict[str, dict[str, Any]]]
-
-    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str, gbls: dict[str, dict[str, dict[str, Any]]]) -> None:
-        self._client = client
-        self._security_client = security_client
-        self._server_url = server_url
-        self._language = language
-        self._sdk_version = sdk_version
-        self._gen_version = gen_version
-        self._globals = gbls
-        
-    def create(self, request: operations.CreateModelCustomizationRequest) -> operations.CreateModelCustomizationResponse:
-        r"""Create model customization"""
-        base_url = self._server_url
+class Snippet:
+    r"""Methods related to Snippets"""
+    sdk_configuration: SDKConfiguration
+
+    def __init__(self, sdk_config: SDKConfiguration) -> None:
+        self.sdk_configuration = sdk_config
+        
+    
+    def delete(self, team_id: int, x_request_id: Optional[str] = None, ids: Optional[list[str]] = None, organization_id: Optional[int] = None) -> operations.DeleteSnippetsResponse:
+        r"""Delete snippets"""
+        request = operations.DeleteSnippetsRequest(
+            team_id=team_id,
+            x_request_id=x_request_id,
+            ids=ids,
+            organization_id=organization_id,
+        )
+        
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        
+        url = utils.generate_url(operations.DeleteSnippetsRequest, base_url, '/snippet/organization/{organizationId}/team/{teamId}', request, self.sdk_configuration.globals)
+        headers = utils.get_headers(request)
+        query_params = utils.get_query_params(operations.DeleteSnippetsRequest, request, self.sdk_configuration.globals)
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        url = utils.generate_url(operations.CreateModelCustomizationRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/customization', request, self._globals)
+        client = self.sdk_configuration.security_client
         
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "create_customization_request", 'json')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        if data is None and form is None:
-            raise Exception('request body is required')
-        
-        client = self._security_client
-        
-        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        http_res = client.request('DELETE', url, params=query_params, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.CreateModelCustomizationResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.DeleteSnippetsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.ModelCustomization])
-                res.model_customization = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.DeleteResponse])
+                res.delete_response = out
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
-    def delete(self, request: operations.DeleteModelCustomizationRequest) -> operations.DeleteModelCustomizationResponse:
-        r"""Delete Model customization"""
-        base_url = self._server_url
-        
-        url = utils.generate_url(operations.DeleteModelCustomizationRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/customization/{customizationId}', request, self._globals)
-        
-        
-        client = self._security_client
-        
-        http_res = client.request('DELETE', url)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.DeleteModelCustomizationResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            res.headers = http_res.headers
-            
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[dict[str, Any]])
-                res.delete_model_customization_200_application_json_object = out
-        elif http_res.status_code in [400, 401, 403, 404, 500]:
-            res.headers = http_res.headers
-            
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
-                res.fail_response = out
-
-        return res
-
-    def get(self, request: operations.GetModelCustomizationRequest) -> operations.GetModelCustomizationResponse:
-        r"""Get model customization"""
-        base_url = self._server_url
-        
-        url = utils.generate_url(operations.GetModelCustomizationRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/customization/{customizationId}', request, self._globals)
+    
+    def find(self, request: operations.FindSnippetsRequest) -> operations.FindSnippetsResponse:
+        r"""Find snippets"""
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
+        url = utils.generate_url(operations.FindSnippetsRequest, base_url, '/snippet/organization/{organizationId}/team/{teamId}', request, self.sdk_configuration.globals)
+        headers = {}
+        query_params = utils.get_query_params(operations.FindSnippetsRequest, request, self.sdk_configuration.globals)
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
-        http_res = client.request('GET', url)
+        http_res = client.request('GET', url, params=query_params, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetModelCustomizationResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.FindSnippetsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.ModelCustomization])
-                res.model_customization = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PaginatedResultSnippetWithUser])
+                res.paginated_result_snippet_with_user = out
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
-    def list(self, request: operations.ListModelCustomizationsRequest) -> operations.ListModelCustomizationsResponse:
-        r"""List model customizations"""
-        base_url = self._server_url
-        
-        url = utils.generate_url(operations.ListModelCustomizationsRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/customization', request, self._globals)
-        
+    
+    def update(self, team_id: int, request_body: Optional[list[shared.SnippetUpdate]] = None, x_request_id: Optional[str] = None, organization_id: Optional[int] = None) -> operations.UpdateSnippetsResponse:
+        r"""Update snippets"""
+        request = operations.UpdateSnippetsRequest(
+            team_id=team_id,
+            request_body=request_body,
+            x_request_id=x_request_id,
+            organization_id=organization_id,
+        )
+        
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        
+        url = utils.generate_url(operations.UpdateSnippetsRequest, base_url, '/snippet/organization/{organizationId}/team/{teamId}', request, self.sdk_configuration.globals)
+        headers = utils.get_headers(request)
+        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
-        http_res = client.request('GET', url)
+        http_res = client.request('PUT', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListModelCustomizationsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.UpdateSnippetsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.CustomizationsResponse])
-                res.customizations_response = out
+                out = utils.unmarshal_json(http_res.text, Optional[list[shared.SnippetWithUser]])
+                res.snippet_with_users = out
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
```

### Comparing `writerai-0.4.0/src/writer/models/operations/__init__.py` & `writerai-0.6.0/src/writer/models/operations/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 from .deletesnippets import *
 from .deleteterms import *
 from .detectcontent import *
 from .fetchcustomizedmodelfile import *
 from .findsnippets import *
 from .findterms import *
 from .generate_content import *
+from .getdocumentdetails import *
 from .getfile import *
 from .getmodelcustomization import *
 from .getsubscriptiondetails import *
 from .listfiles import *
 from .listmodelcustomizations import *
 from .listmodels import *
 from .listpages import *
+from .listteamdocuments import *
 from .listtemplates import *
 from .listusers import *
 from .pagedetails import *
 from .updatesnippets import *
 from .updateterms import *
 from .uploadfile import *
 
-__all__ = ["AddTermsRequest","AddTermsResponse","ContentCheckRequest","ContentCheckResponse","ContentCorrectRequest","ContentCorrectResponse","CreateCompletionRequest","CreateCompletionResponse","CreateModelCustomizationCompletionRequest","CreateModelCustomizationCompletionResponse","CreateModelCustomizationRequest","CreateModelCustomizationResponse","DeleteFileRequest","DeleteFileResponse","DeleteModelCustomizationRequest","DeleteModelCustomizationResponse","DeleteSnippetsRequest","DeleteSnippetsResponse","DeleteTermsRequest","DeleteTermsResponse","DetectContentRequest","DetectContentResponse","FetchCustomizedModelFileRequest","FetchCustomizedModelFileResponse","FindSnippetsRequest","FindSnippetsResponse","FindSnippetsSortFieldEnum","FindSnippetsSortOrderEnum","FindTermsPartOfSpeechEnum","FindTermsRequest","FindTermsResponse","FindTermsSortFieldEnum","FindTermsSortOrderEnum","FindTermsTypeEnum","GenerateContentRequest","GenerateContentResponse","GetFileRequest","GetFileResponse","GetModelCustomizationRequest","GetModelCustomizationResponse","GetSubscriptionDetailsResponse","ListFilesRequest","ListFilesResponse","ListModelCustomizationsRequest","ListModelCustomizationsResponse","ListModelsRequest","ListModelsResponse","ListPagesRequest","ListPagesResponse","ListPagesStatusEnum","ListTemplatesRequest","ListTemplatesResponse","ListUsersRequest","ListUsersResponse","ListUsersSortFieldEnum","ListUsersSortOrderEnum","PageDetailsRequest","PageDetailsResponse","UpdateSnippetsRequest","UpdateSnippetsResponse","UpdateTermsRequest","UpdateTermsResponse","UploadFileRequest","UploadFileResponse"]
+__all__ = ["AddTermsRequest","AddTermsResponse","ContentCheckRequest","ContentCheckResponse","ContentCorrectRequest","ContentCorrectResponse","CreateCompletionRequest","CreateCompletionResponse","CreateModelCustomizationCompletionRequest","CreateModelCustomizationCompletionResponse","CreateModelCustomizationRequest","CreateModelCustomizationResponse","DeleteFile200ApplicationJSON","DeleteFileRequest","DeleteFileResponse","DeleteModelCustomization200ApplicationJSON","DeleteModelCustomizationRequest","DeleteModelCustomizationResponse","DeleteSnippetsRequest","DeleteSnippetsResponse","DeleteTermsRequest","DeleteTermsResponse","DetectContentRequest","DetectContentResponse","FetchCustomizedModelFileRequest","FetchCustomizedModelFileResponse","FindSnippetsRequest","FindSnippetsResponse","FindSnippetsSortField","FindSnippetsSortOrder","FindTermsPartOfSpeech","FindTermsRequest","FindTermsResponse","FindTermsSortField","FindTermsSortOrder","FindTermsType","GenerateContentRequest","GenerateContentResponse","GetDocumentDetailsRequest","GetDocumentDetailsResponse","GetFileRequest","GetFileResponse","GetModelCustomizationRequest","GetModelCustomizationResponse","GetSubscriptionDetailsResponse","ListFilesRequest","ListFilesResponse","ListModelCustomizationsRequest","ListModelCustomizationsResponse","ListModelsRequest","ListModelsResponse","ListPagesRequest","ListPagesResponse","ListPagesStatus","ListTeamDocumentsRequest","ListTeamDocumentsResponse","ListTeamDocumentsSortField","ListTeamDocumentsSortOrder","ListTemplatesRequest","ListTemplatesResponse","ListUsersRequest","ListUsersResponse","ListUsersSortField","ListUsersSortOrder","PageDetailsRequest","PageDetailsResponse","UpdateSnippetsRequest","UpdateSnippetsResponse","UpdateTermsRequest","UpdateTermsResponse","UploadFileRequest","UploadFileResponse"]
```

### Comparing `writerai-0.4.0/src/writer/models/operations/addterms.py` & `writerai-0.6.0/src/writer/models/operations/addterms.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,26 +5,29 @@
 import requests as requests_http
 from ..shared import createtermsrequest as shared_createtermsrequest
 from ..shared import createtermsresponse as shared_createtermsresponse
 from ..shared import failresponse as shared_failresponse
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class AddTermsRequest:
+    create_terms_request: shared_createtermsrequest.CreateTermsRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
-    create_terms_request: shared_createtermsrequest.CreateTermsRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})  
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
-    
+
+
+
 
 @dataclasses.dataclass
 class AddTermsResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
-    create_terms_response: Optional[shared_createtermsresponse.CreateTermsResponse] = dataclasses.field(default=None)  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
+    create_terms_response: Optional[shared_createtermsresponse.CreateTermsResponse] = dataclasses.field(default=None)
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/contentcheck.py` & `writerai-0.6.0/src/writer/models/operations/contentcheck.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,26 +5,29 @@
 import requests as requests_http
 from ..shared import contentrequest as shared_contentrequest
 from ..shared import failresponse as shared_failresponse
 from ..shared import processedcontent as shared_processedcontent
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class ContentCheckRequest:
+    content_request: shared_contentrequest.ContentRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
-    content_request: shared_contentrequest.ContentRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})  
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
-    
+
+
+
 
 @dataclasses.dataclass
 class ContentCheckResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    processed_content: Optional[shared_processedcontent.ProcessedContent] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    processed_content: Optional[shared_processedcontent.ProcessedContent] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/contentcorrect.py` & `writerai-0.6.0/src/writer/models/operations/contentcorrect.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,27 +5,30 @@
 import requests as requests_http
 from ..shared import contentrequest as shared_contentrequest
 from ..shared import correctionresponse as shared_correctionresponse
 from ..shared import failresponse as shared_failresponse
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class ContentCorrectRequest:
+    content_request: shared_contentrequest.ContentRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})
     
-    content_request: shared_contentrequest.ContentRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})  
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
-    x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})  
-    
+
+
+
 
 @dataclasses.dataclass
 class ContentCorrectResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
-    correction_response: Optional[shared_correctionresponse.CorrectionResponse] = dataclasses.field(default=None)  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
+    correction_response: Optional[shared_correctionresponse.CorrectionResponse] = dataclasses.field(default=None)
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/createcompletion.py` & `writerai-0.6.0/src/writer/models/operations/createcompletion.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,26 +5,29 @@
 import requests as requests_http
 from ..shared import completionrequest as shared_completionrequest
 from ..shared import completionresponse as shared_completionresponse
 from ..shared import failresponse as shared_failresponse
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class CreateCompletionRequest:
+    completion_request: shared_completionrequest.CompletionRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
+    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
-    completion_request: shared_completionrequest.CompletionRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})  
-    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})  
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
-    
+
+
+
 
 @dataclasses.dataclass
 class CreateCompletionResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
-    completion_response: Optional[shared_completionresponse.CompletionResponse] = dataclasses.field(default=None)  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
+    completion_response: Optional[shared_completionresponse.CompletionResponse] = dataclasses.field(default=None)
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/createmodelcustomization.py` & `writerai-0.6.0/src/writer/models/operations/createmodelcustomization.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,29 @@
 import requests as requests_http
 from ..shared import createcustomizationrequest as shared_createcustomizationrequest
 from ..shared import failresponse as shared_failresponse
 from ..shared import modelcustomization as shared_modelcustomization
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class CreateModelCustomizationRequest:
+    create_customization_request: shared_createcustomizationrequest.CreateCustomizationRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
+    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
-    create_customization_request: shared_createcustomizationrequest.CreateCustomizationRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})  
-    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})  
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
-    
+
+
+
 
 @dataclasses.dataclass
 class CreateModelCustomizationResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    model_customization: Optional[shared_modelcustomization.ModelCustomization] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    model_customization: Optional[shared_modelcustomization.ModelCustomization] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/createmodelcustomizationcompletion.py` & `writerai-0.6.0/src/writer/models/operations/createmodelcustomizationcompletion.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,30 @@
 import requests as requests_http
 from ..shared import completionrequest as shared_completionrequest
 from ..shared import completionresponse as shared_completionresponse
 from ..shared import failresponse as shared_failresponse
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class CreateModelCustomizationCompletionRequest:
+    completion_request: shared_completionrequest.CompletionRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
+    customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})
+    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
-    completion_request: shared_completionrequest.CompletionRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})  
-    customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})  
-    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})  
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
-    
+
+
+
 
 @dataclasses.dataclass
 class CreateModelCustomizationCompletionResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
-    completion_response: Optional[shared_completionresponse.CompletionResponse] = dataclasses.field(default=None)  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
+    completion_response: Optional[shared_completionresponse.CompletionResponse] = dataclasses.field(default=None)
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/deletefile.py` & `writerai-0.6.0/src/writer/models/operations/deletemodelcustomization.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
-from typing import Any, Optional
+from typing import Optional
+
 
 
 @dataclasses.dataclass
-class DeleteFileRequest:
-    
-    file_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'fileId', 'style': 'simple', 'explode': False }})  
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
+class DeleteModelCustomizationRequest:
+    customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})
+    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
 
+
+
+
 @dataclasses.dataclass
-class DeleteFileResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
-    delete_file_200_application_json_object: Optional[dict[str, Any]] = dataclasses.field(default=None)  
+class DeleteModelCustomization200ApplicationJSON:
+    pass
+
+
+
+@dataclasses.dataclass
+class DeleteModelCustomizationResponse:
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
+    delete_model_customization_200_application_json_object: Optional[DeleteModelCustomization200ApplicationJSON] = dataclasses.field(default=None)
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/deletemodelcustomization.py` & `writerai-0.6.0/src/writer/models/operations/getdocumentdetails.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import document as shared_document
 from ..shared import failresponse as shared_failresponse
-from typing import Any, Optional
+from typing import Optional
+
 
 
 @dataclasses.dataclass
-class DeleteModelCustomizationRequest:
-    
-    customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})  
-    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})  
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
+class GetDocumentDetailsRequest:
+    document_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'documentId', 'style': 'simple', 'explode': False }})
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
 
+
+
+
 @dataclasses.dataclass
-class DeleteModelCustomizationResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
-    delete_model_customization_200_application_json_object: Optional[dict[str, Any]] = dataclasses.field(default=None)  
+class GetDocumentDetailsResponse:
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
+    document: Optional[shared_document.Document] = dataclasses.field(default=None)
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/deletesnippets.py` & `writerai-0.6.0/src/writer/models/operations/getfile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import deleteresponse as shared_deleteresponse
 from ..shared import failresponse as shared_failresponse
+from ..shared import modelfile as shared_modelfile
 from typing import Optional
 
 
+
 @dataclasses.dataclass
-class DeleteSnippetsRequest:
-    
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
-    ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})  
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
-    x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})  
+class GetFileRequest:
+    file_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'fileId', 'style': 'simple', 'explode': False }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
 
+
+
+
 @dataclasses.dataclass
-class DeleteSnippetsResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
-    delete_response: Optional[shared_deleteresponse.DeleteResponse] = dataclasses.field(default=None)  
+class GetFileResponse:
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    model_file: Optional[shared_modelfile.ModelFile] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/deleteterms.py` & `writerai-0.6.0/src/writer/models/operations/deleteterms.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,27 +4,30 @@
 import dataclasses
 import requests as requests_http
 from ..shared import deleteresponse as shared_deleteresponse
 from ..shared import failresponse as shared_failresponse
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class DeleteTermsRequest:
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
+    ids: Optional[list[int]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})
     
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
-    ids: Optional[list[int]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})  
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
-    x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})  
-    
+
+
+
 
 @dataclasses.dataclass
 class DeleteTermsResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
-    delete_response: Optional[shared_deleteresponse.DeleteResponse] = dataclasses.field(default=None)  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
+    delete_response: Optional[shared_deleteresponse.DeleteResponse] = dataclasses.field(default=None)
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/detectcontent.py` & `writerai-0.6.0/src/writer/models/operations/detectcontent.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 import requests as requests_http
 from ..shared import contentdetectorrequest as shared_contentdetectorrequest
 from ..shared import contentdetectorresponse as shared_contentdetectorresponse
 from ..shared import failresponse as shared_failresponse
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class DetectContentRequest:
+    content_detector_request: shared_contentdetectorrequest.ContentDetectorRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
-    content_detector_request: shared_contentdetectorrequest.ContentDetectorRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})  
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
-    
+
+
+
 
 @dataclasses.dataclass
 class DetectContentResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
-    content_detector_responses: Optional[list[shared_contentdetectorresponse.ContentDetectorResponse]] = dataclasses.field(default=None)  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
+    content_detector_responses: Optional[list[shared_contentdetectorresponse.ContentDetectorResponse]] = dataclasses.field(default=None)
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/fetchcustomizedmodelfile.py` & `writerai-0.6.0/src/writer/models/operations/fetchcustomizedmodelfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,26 +3,29 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class FetchCustomizedModelFileRequest:
+    customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})
+    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
-    customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})  
-    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})  
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
-    
+
+
+
 
 @dataclasses.dataclass
 class FetchCustomizedModelFileResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    fetch_customized_model_file_200_application_octet_stream_binary_string: Optional[bytes] = dataclasses.field(default=None)  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    fetch_customized_model_file_200_application_octet_stream_binary_string: Optional[bytes] = dataclasses.field(default=None)
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/findsnippets.py` & `writerai-0.6.0/src/writer/models/operations/findsnippets.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,42 +4,45 @@
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
 from ..shared import paginatedresult_snippetwithuser as shared_paginatedresult_snippetwithuser
 from enum import Enum
 from typing import Optional
 
-class FindSnippetsSortFieldEnum(str, Enum):
+class FindSnippetsSortField(str, Enum):
     SHORTCUT = 'shortcut'
     CREATION_TIME = 'creationTime'
     MODIFICATION_TIME = 'modificationTime'
 
-class FindSnippetsSortOrderEnum(str, Enum):
+class FindSnippetsSortOrder(str, Enum):
     ASC = 'asc'
     DESC = 'desc'
 
 
+
 @dataclasses.dataclass
 class FindSnippetsRequest:
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
+    limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    search: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'search', 'style': 'form', 'explode': True }})
+    shortcuts: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'shortcuts', 'style': 'form', 'explode': True }})
+    sort_field: Optional[FindSnippetsSortField] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortField', 'style': 'form', 'explode': True }})
+    sort_order: Optional[FindSnippetsSortOrder] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortOrder', 'style': 'form', 'explode': True }})
+    tags: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'tags', 'style': 'form', 'explode': True }})
     
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
-    limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})  
-    offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})  
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
-    search: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'search', 'style': 'form', 'explode': True }})  
-    shortcuts: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'shortcuts', 'style': 'form', 'explode': True }})  
-    sort_field: Optional[FindSnippetsSortFieldEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortField', 'style': 'form', 'explode': True }})  
-    sort_order: Optional[FindSnippetsSortOrderEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortOrder', 'style': 'form', 'explode': True }})  
-    tags: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'tags', 'style': 'form', 'explode': True }})  
-    
+
+
+
 
 @dataclasses.dataclass
 class FindSnippetsResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    paginated_result_snippet_with_user: Optional[shared_paginatedresult_snippetwithuser.PaginatedResultSnippetWithUser] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    paginated_result_snippet_with_user: Optional[shared_paginatedresult_snippetwithuser.PaginatedResultSnippetWithUser] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/findterms.py` & `writerai-0.6.0/src/writer/models/operations/findterms.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,55 +4,58 @@
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
 from ..shared import paginatedresult_fulltermwithuser as shared_paginatedresult_fulltermwithuser
 from enum import Enum
 from typing import Optional
 
-class FindTermsPartOfSpeechEnum(str, Enum):
+class FindTermsPartOfSpeech(str, Enum):
     NOUN = 'noun'
     VERB = 'verb'
     ADVERB = 'adverb'
     ADJECTIVE = 'adjective'
 
-class FindTermsSortFieldEnum(str, Enum):
+class FindTermsSortField(str, Enum):
     TERM = 'term'
     CREATION_TIME = 'creationTime'
     MODIFICATION_TIME = 'modificationTime'
     TYPE = 'type'
 
-class FindTermsSortOrderEnum(str, Enum):
+class FindTermsSortOrder(str, Enum):
     ASC = 'asc'
     DESC = 'desc'
 
-class FindTermsTypeEnum(str, Enum):
+class FindTermsType(str, Enum):
     APPROVED = 'approved'
     BANNED = 'banned'
     PENDING = 'pending'
 
 
+
 @dataclasses.dataclass
 class FindTermsRequest:
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
+    limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    part_of_speech: Optional[FindTermsPartOfSpeech] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'partOfSpeech', 'style': 'form', 'explode': True }})
+    sort_field: Optional[FindTermsSortField] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortField', 'style': 'form', 'explode': True }})
+    sort_order: Optional[FindTermsSortOrder] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortOrder', 'style': 'form', 'explode': True }})
+    tags: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'tags', 'style': 'form', 'explode': True }})
+    term: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'term', 'style': 'form', 'explode': True }})
+    type: Optional[FindTermsType] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'type', 'style': 'form', 'explode': True }})
     
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
-    limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})  
-    offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})  
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
-    part_of_speech: Optional[FindTermsPartOfSpeechEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'partOfSpeech', 'style': 'form', 'explode': True }})  
-    sort_field: Optional[FindTermsSortFieldEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortField', 'style': 'form', 'explode': True }})  
-    sort_order: Optional[FindTermsSortOrderEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortOrder', 'style': 'form', 'explode': True }})  
-    tags: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'tags', 'style': 'form', 'explode': True }})  
-    term: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'term', 'style': 'form', 'explode': True }})  
-    type: Optional[FindTermsTypeEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'type', 'style': 'form', 'explode': True }})  
-    
+
+
+
 
 @dataclasses.dataclass
 class FindTermsResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    paginated_result_full_term_with_user: Optional[shared_paginatedresult_fulltermwithuser.PaginatedResultFullTermWithUser] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    paginated_result_full_term_with_user: Optional[shared_paginatedresult_fulltermwithuser.PaginatedResultFullTermWithUser] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/generate_content.py` & `writerai-0.6.0/src/writer/models/operations/updatesnippets.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import draft as shared_draft
 from ..shared import failresponse as shared_failresponse
-from ..shared import generatetemplaterequest as shared_generatetemplaterequest
+from ..shared import snippetupdate as shared_snippetupdate
+from ..shared import snippetwithuser as shared_snippetwithuser
 from typing import Optional
 
 
+
 @dataclasses.dataclass
-class GenerateContentRequest:
-    
-    generate_template_request: shared_generatetemplaterequest.GenerateTemplateRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})  
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
+class UpdateSnippetsRequest:
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    request_body: Optional[list[shared_snippetupdate.SnippetUpdate]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})
     
 
+
+
+
 @dataclasses.dataclass
-class GenerateContentResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
-    draft: Optional[shared_draft.Draft] = dataclasses.field(default=None)  
+class UpdateSnippetsResponse:
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    snippet_with_users: Optional[list[shared_snippetwithuser.SnippetWithUser]] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/getfile.py` & `writerai-0.6.0/src/writer/models/operations/listmodelcustomizations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import customizationsresponse as shared_customizationsresponse
 from ..shared import failresponse as shared_failresponse
-from ..shared import modelfile as shared_modelfile
 from typing import Optional
 
 
+
 @dataclasses.dataclass
-class GetFileRequest:
-    
-    file_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'fileId', 'style': 'simple', 'explode': False }})  
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
+class ListModelCustomizationsRequest:
+    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
 
+
+
+
 @dataclasses.dataclass
-class GetFileResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+class ListModelCustomizationsResponse:
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
+    customizations_response: Optional[shared_customizationsresponse.CustomizationsResponse] = dataclasses.field(default=None)
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    model_file: Optional[shared_modelfile.ModelFile] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/getmodelcustomization.py` & `writerai-0.6.0/src/writer/models/operations/getmodelcustomization.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
 from ..shared import modelcustomization as shared_modelcustomization
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class GetModelCustomizationRequest:
+    customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})
+    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
-    customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})  
-    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})  
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
-    
+
+
+
 
 @dataclasses.dataclass
 class GetModelCustomizationResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    model_customization: Optional[shared_modelcustomization.ModelCustomization] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    model_customization: Optional[shared_modelcustomization.ModelCustomization] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/getsubscriptiondetails.py` & `writerai-0.6.0/src/writer/models/operations/getsubscriptiondetails.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
 from ..shared import subscriptionpublicresponseapi as shared_subscriptionpublicresponseapi
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class GetSubscriptionDetailsResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    subscription_public_response_api: Optional[shared_subscriptionpublicresponseapi.SubscriptionPublicResponseAPI] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    subscription_public_response_api: Optional[shared_subscriptionpublicresponseapi.SubscriptionPublicResponseAPI] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/listfiles.py` & `writerai-0.6.0/src/writer/models/operations/listtemplates.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
-from ..shared import modelfilesresponse as shared_modelfilesresponse
+from ..shared import templatedetailsresponse as shared_templatedetailsresponse
 from typing import Optional
 
 
+
 @dataclasses.dataclass
-class ListFilesRequest:
-    
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
+class ListTemplatesRequest:
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
+    template_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'templateId', 'style': 'simple', 'explode': False }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
 
+
+
+
 @dataclasses.dataclass
-class ListFilesResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+class ListTemplatesResponse:
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    model_files_response: Optional[shared_modelfilesresponse.ModelFilesResponse] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    template_details_response: Optional[shared_templatedetailsresponse.TemplateDetailsResponse] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/listmodelcustomizations.py` & `writerai-0.6.0/src/writer/models/operations/generate_content.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import customizationsresponse as shared_customizationsresponse
+from ..shared import draft as shared_draft
 from ..shared import failresponse as shared_failresponse
+from ..shared import generatetemplaterequest as shared_generatetemplaterequest
 from typing import Optional
 
 
+
 @dataclasses.dataclass
-class ListModelCustomizationsRequest:
-    
-    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})  
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
+class GenerateContentRequest:
+    generate_template_request: shared_generatetemplaterequest.GenerateTemplateRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
 
+
+
+
 @dataclasses.dataclass
-class ListModelCustomizationsResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
-    customizations_response: Optional[shared_customizationsresponse.CustomizationsResponse] = dataclasses.field(default=None)  
+class GenerateContentResponse:
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
+    draft: Optional[shared_draft.Draft] = dataclasses.field(default=None)
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/listmodels.py` & `writerai-0.6.0/src/writer/models/operations/listmodels.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
 from ..shared import generationmodelsresponse as shared_generationmodelsresponse
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class ListModelsRequest:
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
     
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
-    
+
+
+
 
 @dataclasses.dataclass
 class ListModelsResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    generation_models_response: Optional[shared_generationmodelsresponse.GenerationModelsResponse] = dataclasses.field(default=None)  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    generation_models_response: Optional[shared_generationmodelsresponse.GenerationModelsResponse] = dataclasses.field(default=None)
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/listpages.py` & `writerai-0.6.0/src/writer/models/operations/listpages.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,34 @@
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
 from ..shared import paginatedresult_pagepublicapiresponse as shared_paginatedresult_pagepublicapiresponse
 from enum import Enum
 from typing import Optional
 
-class ListPagesStatusEnum(str, Enum):
+class ListPagesStatus(str, Enum):
     LIVE = 'live'
     OFFLINE = 'offline'
 
 
+
 @dataclasses.dataclass
 class ListPagesRequest:
+    limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
+    status: Optional[ListPagesStatus] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'status', 'style': 'form', 'explode': True }})
     
-    limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})  
-    offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})  
-    status: Optional[ListPagesStatusEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'status', 'style': 'form', 'explode': True }})  
-    
+
+
+
 
 @dataclasses.dataclass
 class ListPagesResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    paginated_result_page_public_api_response: Optional[shared_paginatedresult_pagepublicapiresponse.PaginatedResultPagePublicAPIResponse] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    paginated_result_page_public_api_response: Optional[shared_paginatedresult_pagepublicapiresponse.PaginatedResultPagePublicAPIResponse] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/listtemplates.py` & `writerai-0.6.0/src/writer/models/shared/paginatedresult_snippetwithuser.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import failresponse as shared_failresponse
-from ..shared import templatedetailsresponse as shared_templatedetailsresponse
+from ..shared import pagination as shared_pagination
+from ..shared import snippetwithuser as shared_snippetwithuser
+from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
+from writer import utils
 
 
-@dataclasses.dataclass
-class ListTemplatesRequest:
-    
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
-    template_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'templateId', 'style': 'simple', 'explode': False }})  
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
-    
+@dataclass_json(undefined=Undefined.EXCLUDE)
 
 @dataclasses.dataclass
-class ListTemplatesResponse:
+class PaginatedResultSnippetWithUser:
+    pagination: shared_pagination.Pagination = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination') }})
+    total_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalCount') }})
+    result: Optional[list[shared_snippetwithuser.SnippetWithUser]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('result'), 'exclude': lambda f: f is None }})
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
-    fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    template_details_response: Optional[shared_templatedetailsresponse.TemplateDetailsResponse] = dataclasses.field(default=None)  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/listusers.py` & `writerai-0.6.0/src/writer/models/operations/listusers.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,42 +4,45 @@
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
 from ..shared import paginatedresult_userpublicresponse as shared_paginatedresult_userpublicresponse
 from enum import Enum
 from typing import Optional
 
-class ListUsersSortFieldEnum(str, Enum):
+class ListUsersSortField(str, Enum):
     ID = 'id'
     NAME = 'name'
     CREATION_TIME = 'creationTime'
     DELETED = 'deleted'
     MODIFICATION_TIME = 'modificationTime'
     EMAIL = 'email'
     LAST_SEEN = 'lastSeen'
 
-class ListUsersSortOrderEnum(str, Enum):
+class ListUsersSortOrder(str, Enum):
     ASC = 'asc'
     DESC = 'desc'
 
 
+
 @dataclasses.dataclass
 class ListUsersRequest:
+    limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
+    search: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'search', 'style': 'form', 'explode': True }})
+    sort_field: Optional[ListUsersSortField] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortField', 'style': 'form', 'explode': True }})
+    sort_order: Optional[ListUsersSortOrder] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortOrder', 'style': 'form', 'explode': True }})
     
-    limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})  
-    offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})  
-    search: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'search', 'style': 'form', 'explode': True }})  
-    sort_field: Optional[ListUsersSortFieldEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortField', 'style': 'form', 'explode': True }})  
-    sort_order: Optional[ListUsersSortOrderEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortOrder', 'style': 'form', 'explode': True }})  
-    
+
+
+
 
 @dataclasses.dataclass
 class ListUsersResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    paginated_result_user_public_response: Optional[shared_paginatedresult_userpublicresponse.PaginatedResultUserPublicResponse] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    paginated_result_user_public_response: Optional[shared_paginatedresult_userpublicresponse.PaginatedResultUserPublicResponse] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/pagedetails.py` & `writerai-0.6.0/src/writer/models/operations/pagedetails.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
 from ..shared import pagewithsectionresponse as shared_pagewithsectionresponse
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class PageDetailsRequest:
+    page_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'pageId', 'style': 'simple', 'explode': False }})
     
-    page_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'pageId', 'style': 'simple', 'explode': False }})  
-    
+
+
+
 
 @dataclasses.dataclass
 class PageDetailsResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    page_with_section_response: Optional[shared_pagewithsectionresponse.PageWithSectionResponse] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    page_with_section_response: Optional[shared_pagewithsectionresponse.PageWithSectionResponse] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/operations/updateterms.py` & `writerai-0.6.0/src/writer/models/operations/updateterms.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,30 @@
 import requests as requests_http
 from ..shared import createtermsresponse as shared_createtermsresponse
 from ..shared import failresponse as shared_failresponse
 from ..shared import updatetermsrequest as shared_updatetermsrequest
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class UpdateTermsRequest:
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
+    update_terms_request: shared_updatetermsrequest.UpdateTermsRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})
     
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
-    update_terms_request: shared_updatetermsrequest.UpdateTermsRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})  
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
-    x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})  
-    
+
+
+
 
 @dataclasses.dataclass
 class UpdateTermsResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
-    create_terms_response: Optional[shared_createtermsresponse.CreateTermsResponse] = dataclasses.field(default=None)  
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
+    create_terms_response: Optional[shared_createtermsresponse.CreateTermsResponse] = dataclasses.field(default=None)
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    r"""Bad Request"""  
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
-    
+    r"""Bad Request"""
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/__init__.py` & `writerai-0.6.0/src/writer/models/shared/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from .approvedtermextension import *
 from .approvedtermextensioncreate import *
+from .briefdocument import *
+from .briefdocuments import *
 from .completiongenerationchoice import *
 from .completiongenerationchoicelogprobs import *
 from .completionrequest import *
 from .completionresponse import *
 from .contentdetectorrequest import *
 from .contentdetectorresponse import *
 from .contentissue import *
@@ -13,14 +15,15 @@
 from .contentsettings import *
 from .correctionresponse import *
 from .createcustomizationrequest import *
 from .createtermsrequest import *
 from .createtermsresponse import *
 from .customizationsresponse import *
 from .deleteresponse import *
+from .document import *
 from .draft import *
 from .failmessage import *
 from .failresponse import *
 from .fulllinkedterm import *
 from .fulltermwithuser import *
 from .generatetemplaterequest import *
 from .generationmodelinforesponse import *
@@ -60,8 +63,8 @@
 from .termupdate import *
 from .updatetermsrequest import *
 from .uploadmodelfilerequest import *
 from .usage import *
 from .usageitem import *
 from .userpublicresponse import *
 
-__all__ = ["ApprovedTermExtension","ApprovedTermExtensionCreate","CompletionGenerationChoice","CompletionGenerationChoiceLogprobs","CompletionRequest","CompletionResponse","ContentDetectorRequest","ContentDetectorResponse","ContentDetectorResponseLabelEnum","ContentIssue","ContentIssueServiceEnum","ContentRequest","ContentSettings","CorrectionResponse","CreateCustomizationRequest","CreateTermsRequest","CreateTermsRequestFailHandlingEnum","CreateTermsResponse","CustomizationsResponse","DeleteResponse","Draft","FailMessage","FailResponse","FullLinkedTerm","FullLinkedTermPosEnum","FullTermWithUser","FullTermWithUserPosEnum","FullTermWithUserTypeEnum","GenerateTemplateRequest","GenerationModelInfoResponse","GenerationModelInfoResponseTypeEnum","GenerationModelsResponse","HyperParameters","Input","InputTypeEnum","LinkedTermCreate","MagicRequestInput","MetaData","MetaDataTierEnum","ModelCustomization","ModelFile","ModelFilesResponse","PagePublicAPIResponse","PagePublicAPIResponseStatusEnum","PageWithSectionResponse","PageWithSectionResponseStatusEnum","PaginatedResultFullTermWithUser","PaginatedResultPagePublicAPIResponse","PaginatedResultSnippetWithUser","PaginatedResultUserPublicResponse","Pagination","ProcessedContent","SectionInfo","Security","SimpleUser","SnippetTagV2","SnippetUpdate","SnippetWithUser","SubscriptionPublicResponseAPI","SubscriptionPublicResponseAPIProductNameEnum","SubscriptionPublicResponseAPIStatusEnum","TemplateDetailsResponse","TermCreate","TermCreatePosEnum","TermCreateTypeEnum","TermExample","TermExampleCreate","TermExampleCreateTypeEnum","TermExampleTypeEnum","TermMistake","TermMistakeCreate","TermMistakeCreatePosEnum","TermMistakePosEnum","TermTagCreate","TermTagResponse","TermUpdate","TermUpdatePosEnum","TermUpdateTypeEnum","TerminologyUser","UpdateTermsRequest","UpdateTermsRequestFailHandlingEnum","UploadModelFileRequest","UploadModelFileRequestFile","Usage","UsageItem","UserPublicResponse","UserPublicResponseAccountStatusEnum"]
+__all__ = ["ApprovedTermExtension","ApprovedTermExtensionCreate","BriefDocument","BriefDocumentAccess","BriefDocuments","CompletionGenerationChoice","CompletionGenerationChoiceLogprobs","CompletionRequest","CompletionResponse","ContentDetectorRequest","ContentDetectorResponse","ContentDetectorResponseLabel","ContentIssue","ContentIssueService","ContentRequest","ContentSettings","CorrectionResponse","CreateCustomizationRequest","CreateTermsRequest","CreateTermsRequestFailHandling","CreateTermsResponse","CustomizationsResponse","DeleteResponse","Document","DocumentAccess","Draft","FailMessage","FailResponse","FullLinkedTerm","FullLinkedTermPos","FullTermWithUser","FullTermWithUserPos","FullTermWithUserType","GenerateTemplateRequest","GenerationModelInfoResponse","GenerationModelInfoResponseType","GenerationModelsResponse","HyperParameters","Input","InputType","LinkedTermCreate","MagicRequestInput","MetaData","MetaDataTier","ModelCustomization","ModelFile","ModelFilesResponse","PagePublicAPIResponse","PagePublicAPIResponseStatus","PageWithSectionResponse","PageWithSectionResponseStatus","PaginatedResultFullTermWithUser","PaginatedResultPagePublicAPIResponse","PaginatedResultSnippetWithUser","PaginatedResultUserPublicResponse","Pagination","ProcessedContent","SectionInfo","Security","SimpleUser","SnippetTagV2","SnippetUpdate","SnippetWithUser","SubscriptionPublicResponseAPI","SubscriptionPublicResponseAPIProductName","SubscriptionPublicResponseAPIStatus","TemplateDetailsResponse","TermCreate","TermCreatePos","TermCreateType","TermExample","TermExampleCreate","TermExampleCreateType","TermExampleType","TermMistake","TermMistakeCreate","TermMistakeCreatePos","TermMistakePos","TermTagCreate","TermTagResponse","TermUpdate","TermUpdatePos","TermUpdateType","TerminologyUser","UpdateTermsRequest","UpdateTermsRequestFailHandling","UploadModelFileRequest","UploadModelFileRequestFile","Usage","UsageItem","UserPublicResponse","UserPublicResponseAccountStatus"]
```

### Comparing `writerai-0.4.0/src/writer/models/shared/approvedtermextension.py` & `writerai-0.6.0/src/writer/models/shared/approvedtermextensioncreate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class ApprovedTermExtension:
+class ApprovedTermExtensionCreate:
+    capitalize: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('capitalize') }})
+    fix_case: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fixCase') }})
+    fix_common_mistakes: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fixCommonMistakes') }})
     
-    capitalize: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('capitalize') }})  
-    fix_case: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fixCase') }})  
-    fix_common_mistakes: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fixCommonMistakes') }})  
-    term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termId') }})  
-    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/approvedtermextensioncreate.py` & `writerai-0.6.0/src/writer/models/shared/magicrequestinput.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
+from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class ApprovedTermExtensionCreate:
+class MagicRequestInput:
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    value: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value'), 'exclude': lambda f: f is None }})
     
-    capitalize: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('capitalize') }})  
-    fix_case: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fixCase') }})  
-    fix_common_mistakes: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fixCommonMistakes') }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/completiongenerationchoice.py` & `writerai-0.6.0/src/writer/models/shared/pagination.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import completiongenerationchoicelogprobs as shared_completiongenerationchoicelogprobs
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class CompletionGenerationChoice:
+class Pagination:
+    limit: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('limit'), 'exclude': lambda f: f is None }})
+    offset: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('offset'), 'exclude': lambda f: f is None }})
     
-    text: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('text') }})  
-    logprobs: Optional[shared_completiongenerationchoicelogprobs.CompletionGenerationChoiceLogprobs] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logprobs'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/completiongenerationchoicelogprobs.py` & `writerai-0.6.0/src/writer/models/shared/completiongenerationchoicelogprobs.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class CompletionGenerationChoiceLogprobs:
+    text_offset: Optional[list[int]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('textOffset'), 'exclude': lambda f: f is None }})
+    token_logprobs: Optional[list[float]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tokenLogprobs'), 'exclude': lambda f: f is None }})
+    tokens: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tokens'), 'exclude': lambda f: f is None }})
+    top_logprobs: Optional[list[dict[str, str]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('topLogprobs'), 'exclude': lambda f: f is None }})
     
-    text_offset: Optional[list[int]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('textOffset'), 'exclude': lambda f: f is None }})  
-    token_logprobs: Optional[list[float]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tokenLogprobs'), 'exclude': lambda f: f is None }})  
-    tokens: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tokens'), 'exclude': lambda f: f is None }})  
-    top_logprobs: Optional[list[dict[str, str]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('topLogprobs'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/completionrequest.py` & `writerai-0.6.0/src/writer/models/shared/createcustomizationrequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ..shared import hyperparameters as shared_hyperparameters
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class CompletionRequest:
+class CreateCustomizationRequest:
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    training_dataset_file_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trainingDatasetFileId') }})
+    additional_hyper_parameters: Optional[shared_hyperparameters.HyperParameters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additionalHyperParameters'), 'exclude': lambda f: f is None }})
+    batch_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('batchSize'), 'exclude': lambda f: f is None }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    epochs: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('epochs'), 'exclude': lambda f: f is None }})
+    learning_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('learningRate'), 'exclude': lambda f: f is None }})
+    prompt_template: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptTemplate'), 'exclude': lambda f: f is None }})
+    validation_dataset_file_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validationDatasetFileId'), 'exclude': lambda f: f is None }})
     
-    prompt: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prompt') }})  
-    best_of: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bestOf'), 'exclude': lambda f: f is None }})  
-    frequency_penalty: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('frequencyPenalty'), 'exclude': lambda f: f is None }})  
-    logprobs: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logprobs'), 'exclude': lambda f: f is None }})  
-    max_tokens: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maxTokens'), 'exclude': lambda f: f is None }})  
-    min_tokens: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minTokens'), 'exclude': lambda f: f is None }})  
-    n: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('n'), 'exclude': lambda f: f is None }})  
-    presence_penalty: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('presencePenalty'), 'exclude': lambda f: f is None }})  
-    stop: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stop'), 'exclude': lambda f: f is None }})  
-    temperature: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('temperature'), 'exclude': lambda f: f is None }})  
-    top_p: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('topP'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/completionresponse.py` & `writerai-0.6.0/src/writer/models/shared/completionresponse.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,12 +5,13 @@
 from ..shared import completiongenerationchoice as shared_completiongenerationchoice
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class CompletionResponse:
+    choices: Optional[list[shared_completiongenerationchoice.CompletionGenerationChoice]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('choices'), 'exclude': lambda f: f is None }})
     
-    choices: Optional[list[shared_completiongenerationchoice.CompletionGenerationChoice]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('choices'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/contentdetectorresponse.py` & `writerai-0.6.0/src/writer/models/shared/paginatedresult_userpublicresponse.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ..shared import pagination as shared_pagination
+from ..shared import userpublicresponse as shared_userpublicresponse
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
+from typing import Optional
 from writer import utils
 
-class ContentDetectorResponseLabelEnum(str, Enum):
-    FAKE = 'fake'
-    REAL = 'real'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class ContentDetectorResponse:
+class PaginatedResultUserPublicResponse:
+    pagination: shared_pagination.Pagination = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination') }})
+    total_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalCount') }})
+    result: Optional[list[shared_userpublicresponse.UserPublicResponse]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('result'), 'exclude': lambda f: f is None }})
     
-    label: ContentDetectorResponseLabelEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label') }})  
-    score: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('score') }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/contentissue.py` & `writerai-0.6.0/src/writer/models/shared/contentissue.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Any, Optional
 from writer import utils
 
-class ContentIssueServiceEnum(str, Enum):
+class ContentIssueService(str, Enum):
     COMMON_MISTAKES = 'common-mistakes'
     BANNED_WORDS = 'banned-words'
     DICTIONARY = 'dictionary'
     GEC = 'gec'
     INFINITIVE = 'infinitive'
     SPELLING = 'spelling'
     WRITING_STYLE = 'writing-style'
@@ -44,17 +44,18 @@
     FORMATTING = 'formatting'
     TWITTER = 'twitter'
     GEC_DARK = 'gec-dark'
     GEC_GPT3 = 'gec-gpt3'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class ContentIssue:
+    from_: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('from') }})
+    service: ContentIssueService = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service') }})
+    until: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('until') }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    meta: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('meta'), 'exclude': lambda f: f is None }})
+    suggestions: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('suggestions'), 'exclude': lambda f: f is None }})
     
-    from_: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('from') }})  
-    service: ContentIssueServiceEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service') }})  
-    until: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('until') }})  
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})  
-    meta: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('meta'), 'exclude': lambda f: f is None }})  
-    suggestions: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('suggestions'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/contentrequest.py` & `writerai-0.6.0/src/writer/models/shared/contentrequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,13 +4,14 @@
 import dataclasses
 from ..shared import contentsettings as shared_contentsettings
 from dataclasses_json import Undefined, dataclass_json
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class ContentRequest:
+    content: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content') }})
+    settings: shared_contentsettings.ContentSettings = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('settings') }})
     
-    content: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content') }})  
-    settings: shared_contentsettings.ContentSettings = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('settings') }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/contentsettings.py` & `writerai-0.6.0/src/writer/models/shared/contentsettings.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class ContentSettings:
+    age_and_family_status: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ageAndFamilyStatus') }})
+    confidence: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('confidence') }})
+    content_safeguards: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contentSafeguards') }})
+    disability: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('disability') }})
+    gender_identity_sensitivity: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('genderIdentitySensitivity') }})
+    gender_inclusive_nouns: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('genderInclusiveNouns') }})
+    gender_inclusive_pronouns: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('genderInclusivePronouns') }})
+    grammar: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grammar') }})
+    healthy_communication: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('healthyCommunication') }})
+    passive_voice: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('passiveVoice') }})
+    race_ethnicity_nationality_sensitivity: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('raceEthnicityNationalitySensitivity') }})
+    sexual_orientation_sensitivity: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sexualOrientationSensitivity') }})
+    spelling: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('spelling') }})
+    substance_use_sensitivity: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('substanceUseSensitivity') }})
+    unclear_reference: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unclearReference') }})
+    wordiness: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('wordiness') }})
     
-    age_and_family_status: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ageAndFamilyStatus') }})  
-    confidence: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('confidence') }})  
-    content_safeguards: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contentSafeguards') }})  
-    disability: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('disability') }})  
-    gender_identity_sensitivity: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('genderIdentitySensitivity') }})  
-    gender_inclusive_nouns: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('genderInclusiveNouns') }})  
-    gender_inclusive_pronouns: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('genderInclusivePronouns') }})  
-    grammar: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grammar') }})  
-    healthy_communication: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('healthyCommunication') }})  
-    passive_voice: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('passiveVoice') }})  
-    race_ethnicity_nationality_sensitivity: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('raceEthnicityNationalitySensitivity') }})  
-    sexual_orientation_sensitivity: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sexualOrientationSensitivity') }})  
-    spelling: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('spelling') }})  
-    substance_use_sensitivity: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('substanceUseSensitivity') }})  
-    unclear_reference: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unclearReference') }})  
-    wordiness: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('wordiness') }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/createcustomizationrequest.py` & `writerai-0.6.0/src/writer/models/shared/termcreate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,44 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import hyperparameters as shared_hyperparameters
+from ..shared import approvedtermextensioncreate as shared_approvedtermextensioncreate
+from ..shared import linkedtermcreate as shared_linkedtermcreate
+from ..shared import termexamplecreate as shared_termexamplecreate
+from ..shared import termmistakecreate as shared_termmistakecreate
+from ..shared import termtagcreate as shared_termtagcreate
 from dataclasses_json import Undefined, dataclass_json
+from enum import Enum
 from typing import Optional
 from writer import utils
 
+class TermCreatePos(str, Enum):
+    NOUN = 'noun'
+    VERB = 'verb'
+    ADVERB = 'adverb'
+    ADJECTIVE = 'adjective'
+
+class TermCreateType(str, Enum):
+    APPROVED = 'approved'
+    BANNED = 'banned'
+    PENDING = 'pending'
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class CreateCustomizationRequest:
+class TermCreate:
+    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})
+    term: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('term') }})
+    type: TermCreateType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    approved_term_extension: Optional[shared_approvedtermextensioncreate.ApprovedTermExtensionCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('approvedTermExtension'), 'exclude': lambda f: f is None }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    examples: Optional[list[shared_termexamplecreate.TermExampleCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('examples'), 'exclude': lambda f: f is None }})
+    highlight: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('highlight'), 'exclude': lambda f: f is None }})
+    linked_terms: Optional[list[shared_linkedtermcreate.LinkedTermCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkedTerms'), 'exclude': lambda f: f is None }})
+    mistakes: Optional[list[shared_termmistakecreate.TermMistakeCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mistakes'), 'exclude': lambda f: f is None }})
+    pos: Optional[TermCreatePos] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})
+    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
+    tags: Optional[list[shared_termtagcreate.TermTagCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tags'), 'exclude': lambda f: f is None }})
     
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
-    training_dataset_file_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trainingDatasetFileId') }})  
-    additional_hyper_parameters: Optional[shared_hyperparameters.HyperParameters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additionalHyperParameters'), 'exclude': lambda f: f is None }})  
-    batch_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('batchSize'), 'exclude': lambda f: f is None }})  
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})  
-    epochs: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('epochs'), 'exclude': lambda f: f is None }})  
-    learning_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('learningRate'), 'exclude': lambda f: f is None }})  
-    prompt_template: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptTemplate'), 'exclude': lambda f: f is None }})  
-    validation_dataset_file_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validationDatasetFileId'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/createtermsrequest.py` & `writerai-0.6.0/src/writer/models/shared/createtermsrequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 import dataclasses
 from ..shared import termcreate as shared_termcreate
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from writer import utils
 
-class CreateTermsRequestFailHandlingEnum(str, Enum):
+class CreateTermsRequestFailHandling(str, Enum):
     ACCUMULATE = 'accumulate'
     VALIDATE = 'validate'
     SKIP = 'skip'
     VALIDATE_ONLY = 'validateOnly'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class CreateTermsRequest:
+    fail_handling: Optional[CreateTermsRequestFailHandling] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('failHandling'), 'exclude': lambda f: f is None }})
+    models: Optional[list[shared_termcreate.TermCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('models'), 'exclude': lambda f: f is None }})
     
-    fail_handling: Optional[CreateTermsRequestFailHandlingEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('failHandling'), 'exclude': lambda f: f is None }})  
-    models: Optional[list[shared_termcreate.TermCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('models'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/createtermsresponse.py` & `writerai-0.6.0/src/writer/models/shared/createtermsresponse.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,13 +6,14 @@
 from ..shared import fulltermwithuser as shared_fulltermwithuser
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class CreateTermsResponse:
+    fails: Optional[list[shared_failmessage.FailMessage]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fails'), 'exclude': lambda f: f is None }})
+    models: Optional[list[shared_fulltermwithuser.FullTermWithUser]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('models'), 'exclude': lambda f: f is None }})
     
-    fails: Optional[list[shared_failmessage.FailMessage]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fails'), 'exclude': lambda f: f is None }})  
-    models: Optional[list[shared_fulltermwithuser.FullTermWithUser]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('models'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/customizationsresponse.py` & `writerai-0.6.0/src/writer/models/shared/customizationsresponse.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,12 +5,13 @@
 from ..shared import modelcustomization as shared_modelcustomization
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class CustomizationsResponse:
+    customizations: Optional[list[shared_modelcustomization.ModelCustomization]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customizations'), 'exclude': lambda f: f is None }})
     
-    customizations: Optional[list[shared_modelcustomization.ModelCustomization]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customizations'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/draft.py` & `writerai-0.6.0/src/writer/models/shared/draft.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 from datetime import datetime
 from marshmallow import fields
 from typing import Any, Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class Draft:
+    body: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body') }})
+    created_user_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdUserId') }})
+    creation_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    deleted: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deleted') }})
+    document_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('documentId') }})
+    inputs: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inputs') }})
+    organization_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('organizationId') }})
+    team_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('teamId') }})
+    template_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('templateId') }})
+    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title'), 'exclude': lambda f: f is None }})
     
-    body: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body') }})  
-    created_user_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdUserId') }})  
-    creation_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
-    deleted: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deleted') }})  
-    document_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('documentId') }})  
-    inputs: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inputs') }})  
-    organization_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('organizationId') }})  
-    team_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('teamId') }})  
-    template_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('templateId') }})  
-    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})  
-    title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/failmessage.py` & `writerai-0.6.0/src/writer/models/shared/sectioninfo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Any
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class FailMessage:
+class SectionInfo:
+    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    title: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title') }})
+    url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url') }})
     
-    description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})  
-    extras: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('extras') }})  
-    key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key') }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/failresponse.py` & `writerai-0.6.0/src/writer/models/shared/terminologyuser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import failmessage as shared_failmessage
 from dataclasses_json import Undefined, dataclass_json
-from typing import Any, Optional
+from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class FailResponse:
-    r"""Bad Request"""
+class TerminologyUser:
+    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    full_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fullName'), 'exclude': lambda f: f is None }})
     
-    extras: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('extras') }})  
-    tpe: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tpe') }})  
-    errors: Optional[list[shared_failmessage.FailMessage]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errors'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/fulllinkedterm.py` & `writerai-0.6.0/src/writer/models/shared/fulllinkedterm.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 import dataclasses
 from ..shared import approvedtermextension as shared_approvedtermextension
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from writer import utils
 
-class FullLinkedTermPosEnum(str, Enum):
+class FullLinkedTermPos(str, Enum):
     NOUN = 'noun'
     VERB = 'verb'
     ADVERB = 'adverb'
     ADJECTIVE = 'adjective'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class FullLinkedTerm:
+    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})
+    linked_term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkedTermId') }})
+    term: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('term') }})
+    term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termId') }})
+    approved_term_extension: Optional[shared_approvedtermextension.ApprovedTermExtension] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('approvedTermExtension'), 'exclude': lambda f: f is None }})
+    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    pos: Optional[FullLinkedTermPos] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})
     
-    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})  
-    linked_term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkedTermId') }})  
-    term: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('term') }})  
-    term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termId') }})  
-    approved_term_extension: Optional[shared_approvedtermextension.ApprovedTermExtension] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('approvedTermExtension'), 'exclude': lambda f: f is None }})  
-    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})  
-    pos: Optional[FullLinkedTermPosEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/fulltermwithuser.py` & `writerai-0.6.0/src/writer/models/shared/fulltermwithuser.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,42 +12,43 @@
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
 from typing import Optional
 from writer import utils
 
-class FullTermWithUserPosEnum(str, Enum):
+class FullTermWithUserPos(str, Enum):
     NOUN = 'noun'
     VERB = 'verb'
     ADVERB = 'adverb'
     ADJECTIVE = 'adjective'
 
-class FullTermWithUserTypeEnum(str, Enum):
+class FullTermWithUserType(str, Enum):
     APPROVED = 'approved'
     BANNED = 'banned'
     PENDING = 'pending'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class FullTermWithUser:
+    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})
+    created_user: shared_terminologyuser.TerminologyUser = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdUser') }})
+    creation_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    highlight: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('highlight') }})
+    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    modification_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modificationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    modified_user: shared_terminologyuser.TerminologyUser = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedUser') }})
+    term: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('term') }})
+    term_bank_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termBankId') }})
+    type: FullTermWithUserType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    approved_term_extension: Optional[shared_approvedtermextension.ApprovedTermExtension] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('approvedTermExtension'), 'exclude': lambda f: f is None }})
+    backlinked_terms: Optional[list[shared_fulllinkedterm.FullLinkedTerm]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('backlinkedTerms'), 'exclude': lambda f: f is None }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    examples: Optional[list[shared_termexample.TermExample]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('examples'), 'exclude': lambda f: f is None }})
+    linked_terms: Optional[list[shared_fulllinkedterm.FullLinkedTerm]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkedTerms'), 'exclude': lambda f: f is None }})
+    mistakes: Optional[list[shared_termmistake.TermMistake]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mistakes'), 'exclude': lambda f: f is None }})
+    pos: Optional[FullTermWithUserPos] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})
+    tags: Optional[list[shared_termtagresponse.TermTagResponse]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tags'), 'exclude': lambda f: f is None }})
     
-    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})  
-    created_user: shared_terminologyuser.TerminologyUser = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdUser') }})  
-    creation_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
-    highlight: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('highlight') }})  
-    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
-    modification_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modificationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
-    modified_user: shared_terminologyuser.TerminologyUser = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedUser') }})  
-    term: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('term') }})  
-    term_bank_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termBankId') }})  
-    type: FullTermWithUserTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})  
-    approved_term_extension: Optional[shared_approvedtermextension.ApprovedTermExtension] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('approvedTermExtension'), 'exclude': lambda f: f is None }})  
-    backlinked_terms: Optional[list[shared_fulllinkedterm.FullLinkedTerm]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('backlinkedTerms'), 'exclude': lambda f: f is None }})  
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})  
-    examples: Optional[list[shared_termexample.TermExample]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('examples'), 'exclude': lambda f: f is None }})  
-    linked_terms: Optional[list[shared_fulllinkedterm.FullLinkedTerm]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkedTerms'), 'exclude': lambda f: f is None }})  
-    mistakes: Optional[list[shared_termmistake.TermMistake]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mistakes'), 'exclude': lambda f: f is None }})  
-    pos: Optional[FullTermWithUserPosEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})  
-    tags: Optional[list[shared_termtagresponse.TermTagResponse]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tags'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/generatetemplaterequest.py` & `writerai-0.6.0/src/writer/models/shared/generatetemplaterequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,13 +5,14 @@
 from ..shared import magicrequestinput as shared_magicrequestinput
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class GenerateTemplateRequest:
+    template_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('templateId') }})
+    inputs: Optional[list[shared_magicrequestinput.MagicRequestInput]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inputs'), 'exclude': lambda f: f is None }})
     
-    template_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('templateId') }})  
-    inputs: Optional[list[shared_magicrequestinput.MagicRequestInput]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inputs'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/generationmodelinforesponse.py` & `writerai-0.6.0/src/writer/models/shared/usageitem.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
 from writer import utils
 
-class GenerationModelInfoResponseTypeEnum(str, Enum):
-    GPT = 'GPT'
-    INSTRUCT = 'Instruct'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class GenerationModelInfoResponse:
+class UsageItem:
+    limit: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('limit') }})
+    value: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value') }})
     
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
-    type: GenerationModelInfoResponseTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/generationmodelsresponse.py` & `writerai-0.6.0/src/writer/models/shared/generationmodelsresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,12 +5,13 @@
 from ..shared import generationmodelinforesponse as shared_generationmodelinforesponse
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class GenerationModelsResponse:
+    data: Optional[list[shared_generationmodelinforesponse.GenerationModelInfoResponse]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
     
-    data: Optional[list[shared_generationmodelinforesponse.GenerationModelInfoResponse]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/input.py` & `writerai-0.6.0/src/writer/models/shared/input.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from writer import utils
 
-class InputTypeEnum(str, Enum):
+class InputType(str, Enum):
     TEXTBOX = 'textbox'
     TEXTAREA = 'textarea'
     DROPDOWN = 'dropdown'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class Input:
+    dynamic: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dynamic') }})
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    required: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required') }})
+    type: InputType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    help: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('help'), 'exclude': lambda f: f is None }})
+    max_fields: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maxFields'), 'exclude': lambda f: f is None }})
+    min_fields: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minFields'), 'exclude': lambda f: f is None }})
+    options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('options'), 'exclude': lambda f: f is None }})
+    subtitle: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtitle'), 'exclude': lambda f: f is None }})
+    unit_copy: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unitCopy'), 'exclude': lambda f: f is None }})
     
-    dynamic: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dynamic') }})  
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
-    required: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required') }})  
-    type: InputTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})  
-    help: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('help'), 'exclude': lambda f: f is None }})  
-    max_fields: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maxFields'), 'exclude': lambda f: f is None }})  
-    min_fields: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minFields'), 'exclude': lambda f: f is None }})  
-    options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('options'), 'exclude': lambda f: f is None }})  
-    subtitle: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtitle'), 'exclude': lambda f: f is None }})  
-    unit_copy: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unitCopy'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/linkedtermcreate.py` & `writerai-0.6.0/src/writer/models/shared/linkedtermcreate.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,13 +4,14 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class LinkedTermCreate:
+    linked_term_id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkedTermId'), 'exclude': lambda f: f is None }})
+    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
     
-    linked_term_id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkedTermId'), 'exclude': lambda f: f is None }})  
-    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/magicrequestinput.py` & `writerai-0.6.0/src/writer/models/shared/failmessage.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class MagicRequestInput:
+class FailMessage:
+    description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})
+    extras: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('extras') }})
+    key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key') }})
     
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
-    value: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/metadata.py` & `writerai-0.6.0/src/writer/models/shared/document.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+import dateutil.parser
+from ..shared import simpleuser as shared_simpleuser
 from dataclasses_json import Undefined, dataclass_json
+from datetime import datetime
 from enum import Enum
+from marshmallow import fields
 from typing import Optional
 from writer import utils
 
-class MetaDataTierEnum(str, Enum):
-    ENTERPRISE_1 = 'enterprise-1'
-    ENTERPRISE_2 = 'enterprise-2'
-    ENTERPRISE_3 = 'enterprise-3'
-    ENTERPRISE_4 = 'enterprise-4'
+class DocumentAccess(str, Enum):
+    PRIVATE = 'private'
+    PUBLIC = 'public'
+    SHARED = 'shared'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class MetaData:
+class Document:
+    access: DocumentAccess = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access') }})
+    content: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content') }})
+    creation_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    modification_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modificationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    organization_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('organizationId') }})
+    score: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('score') }})
+    team_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('teamId') }})
+    title: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title') }})
+    created_user: Optional[shared_simpleuser.SimpleUser] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdUser'), 'exclude': lambda f: f is None }})
+    modified_user: Optional[shared_simpleuser.SimpleUser] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedUser'), 'exclude': lambda f: f is None }})
     
-    portal: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('portal') }})  
-    reporting: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reporting') }})  
-    snippets_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('snippetsCount') }})  
-    sso_access: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssoAccess') }})  
-    styleguide: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('styleguide') }})  
-    team_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('teamCount') }})  
-    terms_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termsCount') }})  
-    tier: Optional[MetaDataTierEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tier'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/modelcustomization.py` & `writerai-0.6.0/src/writer/models/shared/modelcustomization.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,25 +8,26 @@
 from datetime import datetime
 from marshmallow import fields
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class ModelCustomization:
+    base_model_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('baseModelId') }})
+    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    status: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
+    training_dataset_file_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trainingDatasetFileId') }})
+    updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    additional_hyper_parameters: Optional[shared_hyperparameters.HyperParameters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additionalHyperParameters'), 'exclude': lambda f: f is None }})
+    batch_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('batchSize'), 'exclude': lambda f: f is None }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    epochs: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('epochs'), 'exclude': lambda f: f is None }})
+    learning_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('learningRate'), 'exclude': lambda f: f is None }})
+    prompt_template: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptTemplate'), 'exclude': lambda f: f is None }})
+    validation_dataset_file_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validationDatasetFileId'), 'exclude': lambda f: f is None }})
     
-    base_model_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('baseModelId') }})  
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
-    status: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})  
-    training_dataset_file_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trainingDatasetFileId') }})  
-    updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
-    additional_hyper_parameters: Optional[shared_hyperparameters.HyperParameters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additionalHyperParameters'), 'exclude': lambda f: f is None }})  
-    batch_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('batchSize'), 'exclude': lambda f: f is None }})  
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})  
-    epochs: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('epochs'), 'exclude': lambda f: f is None }})  
-    learning_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('learningRate'), 'exclude': lambda f: f is None }})  
-    prompt_template: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptTemplate'), 'exclude': lambda f: f is None }})  
-    validation_dataset_file_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validationDatasetFileId'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/modelfile.py` & `writerai-0.6.0/src/writer/models/shared/modelfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class ModelFile:
+    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    format: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    number_of_samples: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('numberOfSamples') }})
+    size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size') }})
     
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
-    format: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format') }})  
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
-    number_of_samples: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('numberOfSamples') }})  
-    size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size') }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/modelfilesresponse.py` & `writerai-0.6.0/src/writer/models/shared/modelfilesresponse.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,12 +5,13 @@
 from ..shared import modelfile as shared_modelfile
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class ModelFilesResponse:
+    files: Optional[list[shared_modelfile.ModelFile]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('files'), 'exclude': lambda f: f is None }})
     
-    files: Optional[list[shared_modelfile.ModelFile]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('files'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/pagepublicapiresponse.py` & `writerai-0.6.0/src/writer/models/shared/pagepublicapiresponse.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
 from typing import Optional
 from writer import utils
 
-class PagePublicAPIResponseStatusEnum(str, Enum):
+class PagePublicAPIResponseStatus(str, Enum):
     LIVE = 'live'
     OFFLINE = 'offline'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class PagePublicAPIResponse:
+    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    order: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('order') }})
+    status: PagePublicAPIResponseStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
+    title: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title') }})
+    updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url') }})
+    section: Optional[shared_sectioninfo.SectionInfo] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('section'), 'exclude': lambda f: f is None }})
+    updated_by: Optional[shared_simpleuser.SimpleUser] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedBy'), 'exclude': lambda f: f is None }})
     
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
-    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
-    order: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('order') }})  
-    status: PagePublicAPIResponseStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})  
-    title: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title') }})  
-    updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
-    url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url') }})  
-    section: Optional[shared_sectioninfo.SectionInfo] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('section'), 'exclude': lambda f: f is None }})  
-    updated_by: Optional[shared_simpleuser.SimpleUser] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedBy'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/pagewithsectionresponse.py` & `writerai-0.6.0/src/writer/models/shared/pagewithsectionresponse.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
 from typing import Optional
 from writer import utils
 
-class PageWithSectionResponseStatusEnum(str, Enum):
+class PageWithSectionResponseStatus(str, Enum):
     LIVE = 'live'
     OFFLINE = 'offline'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class PageWithSectionResponse:
+    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    order: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('order') }})
+    status: PageWithSectionResponseStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
+    title: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title') }})
+    updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url') }})
+    content: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
+    section: Optional[shared_sectioninfo.SectionInfo] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('section'), 'exclude': lambda f: f is None }})
+    updated_by: Optional[shared_simpleuser.SimpleUser] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedBy'), 'exclude': lambda f: f is None }})
     
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
-    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
-    order: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('order') }})  
-    status: PageWithSectionResponseStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})  
-    title: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title') }})  
-    updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
-    url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url') }})  
-    content: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})  
-    section: Optional[shared_sectioninfo.SectionInfo] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('section'), 'exclude': lambda f: f is None }})  
-    updated_by: Optional[shared_simpleuser.SimpleUser] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedBy'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/paginatedresult_fulltermwithuser.py` & `writerai-0.6.0/src/writer/models/shared/paginatedresult_fulltermwithuser.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from ..shared import pagination as shared_pagination
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class PaginatedResultFullTermWithUser:
+    pagination: shared_pagination.Pagination = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination') }})
+    total_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalCount') }})
+    result: Optional[list[shared_fulltermwithuser.FullTermWithUser]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('result'), 'exclude': lambda f: f is None }})
     
-    pagination: shared_pagination.Pagination = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination') }})  
-    total_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalCount') }})  
-    result: Optional[list[shared_fulltermwithuser.FullTermWithUser]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('result'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/paginatedresult_pagepublicapiresponse.py` & `writerai-0.6.0/src/writer/models/shared/paginatedresult_pagepublicapiresponse.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from ..shared import pagination as shared_pagination
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class PaginatedResultPagePublicAPIResponse:
+    pagination: shared_pagination.Pagination = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination') }})
+    total_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalCount') }})
+    result: Optional[list[shared_pagepublicapiresponse.PagePublicAPIResponse]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('result'), 'exclude': lambda f: f is None }})
     
-    pagination: shared_pagination.Pagination = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination') }})  
-    total_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalCount') }})  
-    result: Optional[list[shared_pagepublicapiresponse.PagePublicAPIResponse]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('result'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/paginatedresult_snippetwithuser.py` & `writerai-0.6.0/src/writer/models/shared/generationmodelinforesponse.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import pagination as shared_pagination
-from ..shared import snippetwithuser as shared_snippetwithuser
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from enum import Enum
 from writer import utils
 
+class GenerationModelInfoResponseType(str, Enum):
+    GPT = 'GPT'
+    INSTRUCT = 'Instruct'
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class PaginatedResultSnippetWithUser:
+class GenerationModelInfoResponse:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    type: GenerationModelInfoResponseType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
     
-    pagination: shared_pagination.Pagination = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination') }})  
-    total_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalCount') }})  
-    result: Optional[list[shared_snippetwithuser.SnippetWithUser]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('result'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/paginatedresult_userpublicresponse.py` & `writerai-0.6.0/src/writer/models/shared/briefdocuments.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ..shared import briefdocument as shared_briefdocument
 from ..shared import pagination as shared_pagination
-from ..shared import userpublicresponse as shared_userpublicresponse
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class PaginatedResultUserPublicResponse:
+class BriefDocuments:
+    pagination: shared_pagination.Pagination = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination') }})
+    total_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalCount') }})
+    result: Optional[list[shared_briefdocument.BriefDocument]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('result'), 'exclude': lambda f: f is None }})
     
-    pagination: shared_pagination.Pagination = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination') }})  
-    total_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalCount') }})  
-    result: Optional[list[shared_userpublicresponse.UserPublicResponse]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('result'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/pagination.py` & `writerai-0.6.0/src/writer/models/shared/termmistakecreate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
+from enum import Enum
 from typing import Optional
 from writer import utils
 
+class TermMistakeCreatePos(str, Enum):
+    NOUN = 'noun'
+    VERB = 'verb'
+    ADVERB = 'adverb'
+    ADJECTIVE = 'adjective'
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class Pagination:
+class TermMistakeCreate:
+    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})
+    mistake: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mistake') }})
+    pos: Optional[TermMistakeCreatePos] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})
+    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
     
-    limit: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('limit'), 'exclude': lambda f: f is None }})  
-    offset: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('offset'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/processedcontent.py` & `writerai-0.6.0/src/writer/models/shared/processedcontent.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,12 +5,13 @@
 from ..shared import contentissue as shared_contentissue
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class ProcessedContent:
+    issues: Optional[list[shared_contentissue.ContentIssue]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('issues'), 'exclude': lambda f: f is None }})
     
-    issues: Optional[list[shared_contentissue.ContentIssue]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('issues'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/sectioninfo.py` & `writerai-0.6.0/src/writer/models/shared/termexamplecreate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
+from enum import Enum
 from writer import utils
 
+class TermExampleCreateType(str, Enum):
+    GOOD = 'good'
+    BAD = 'bad'
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class SectionInfo:
+class TermExampleCreate:
+    example: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('example') }})
+    type: TermExampleCreateType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
     
-    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
-    title: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title') }})  
-    url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url') }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/simpleuser.py` & `writerai-0.6.0/src/writer/models/shared/simpleuser.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class SimpleUser:
+    first_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName') }})
+    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
     
-    first_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName') }})  
-    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})  
-    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/snippetupdate.py` & `writerai-0.6.0/src/writer/models/shared/snippetupdate.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from ..shared import snippettagv2 as shared_snippettagv2
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class SnippetUpdate:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    snippet: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('snippet') }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    shortcut: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shortcut'), 'exclude': lambda f: f is None }})
+    tags: Optional[list[shared_snippettagv2.SnippetTagV2]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tags'), 'exclude': lambda f: f is None }})
     
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
-    snippet: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('snippet') }})  
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})  
-    shortcut: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shortcut'), 'exclude': lambda f: f is None }})  
-    tags: Optional[list[shared_snippettagv2.SnippetTagV2]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tags'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/snippetwithuser.py` & `writerai-0.6.0/src/writer/models/shared/snippetwithuser.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 from datetime import datetime
 from marshmallow import fields
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class SnippetWithUser:
+    created_user: shared_terminologyuser.TerminologyUser = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdUser') }})
+    creation_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    modification_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modificationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    modified_user: shared_terminologyuser.TerminologyUser = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedUser') }})
+    snippet: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('snippet') }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    shortcut: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shortcut'), 'exclude': lambda f: f is None }})
+    tags: Optional[list[shared_snippettagv2.SnippetTagV2]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tags'), 'exclude': lambda f: f is None }})
     
-    created_user: shared_terminologyuser.TerminologyUser = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdUser') }})  
-    creation_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
-    modification_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modificationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
-    modified_user: shared_terminologyuser.TerminologyUser = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedUser') }})  
-    snippet: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('snippet') }})  
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})  
-    shortcut: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shortcut'), 'exclude': lambda f: f is None }})  
-    tags: Optional[list[shared_snippettagv2.SnippetTagV2]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tags'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/subscriptionpublicresponseapi.py` & `writerai-0.6.0/src/writer/models/shared/subscriptionpublicresponseapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,36 +7,37 @@
 from ..shared import usage as shared_usage
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
 from writer import utils
 
-class SubscriptionPublicResponseAPIProductNameEnum(str, Enum):
+class SubscriptionPublicResponseAPIProductName(str, Enum):
     FREE = 'free'
     PRO = 'pro'
     TEAM = 'team'
     ENTERPRISE = 'enterprise'
     LEGACY = 'legacy'
 
-class SubscriptionPublicResponseAPIStatusEnum(str, Enum):
+class SubscriptionPublicResponseAPIStatus(str, Enum):
     TRIALING = 'trialing'
     ACTIVE = 'active'
     PAST_DUE = 'past_due'
     INCOMPLETE = 'incomplete'
     INCOMPLETE_EXPIRED = 'incomplete_expired'
     UNPAID = 'unpaid'
     CANCELED = 'canceled'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class SubscriptionPublicResponseAPI:
+    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    meta: shared_metadata.MetaData = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('meta') }})
+    product_name: SubscriptionPublicResponseAPIProductName = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('productName') }})
+    seats: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('seats') }})
+    status: SubscriptionPublicResponseAPIStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
+    subscription_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subscriptionId') }})
+    usage: shared_usage.Usage = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('usage') }})
     
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
-    meta: shared_metadata.MetaData = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('meta') }})  
-    product_name: SubscriptionPublicResponseAPIProductNameEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('productName') }})  
-    seats: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('seats') }})  
-    status: SubscriptionPublicResponseAPIStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})  
-    subscription_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subscriptionId') }})  
-    usage: shared_usage.Usage = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('usage') }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/templatedetailsresponse.py` & `writerai-0.6.0/src/writer/models/shared/templatedetailsresponse.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 from datetime import datetime
 from marshmallow import fields
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class TemplateDetailsResponse:
+    category_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('categoryId') }})
+    creation_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    modification_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modificationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    guide_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('guideUrl'), 'exclude': lambda f: f is None }})
+    inputs: Optional[list[shared_input.Input]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inputs'), 'exclude': lambda f: f is None }})
     
-    category_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('categoryId') }})  
-    creation_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
-    modification_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modificationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})  
-    guide_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('guideUrl'), 'exclude': lambda f: f is None }})  
-    inputs: Optional[list[shared_input.Input]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inputs'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/termcreate.py` & `writerai-0.6.0/src/writer/models/shared/termupdate.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,36 +8,37 @@
 from ..shared import termmistakecreate as shared_termmistakecreate
 from ..shared import termtagcreate as shared_termtagcreate
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from writer import utils
 
-class TermCreatePosEnum(str, Enum):
+class TermUpdatePos(str, Enum):
     NOUN = 'noun'
     VERB = 'verb'
     ADVERB = 'adverb'
     ADJECTIVE = 'adjective'
 
-class TermCreateTypeEnum(str, Enum):
+class TermUpdateType(str, Enum):
     APPROVED = 'approved'
     BANNED = 'banned'
     PENDING = 'pending'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class TermCreate:
+class TermUpdate:
+    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})
+    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    term: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('term') }})
+    type: TermUpdateType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    approved_term_extension: Optional[shared_approvedtermextensioncreate.ApprovedTermExtensionCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('approvedTermExtension'), 'exclude': lambda f: f is None }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    examples: Optional[list[shared_termexamplecreate.TermExampleCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('examples'), 'exclude': lambda f: f is None }})
+    highlight: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('highlight'), 'exclude': lambda f: f is None }})
+    linked_terms: Optional[list[shared_linkedtermcreate.LinkedTermCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkedTerms'), 'exclude': lambda f: f is None }})
+    mistakes: Optional[list[shared_termmistakecreate.TermMistakeCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mistakes'), 'exclude': lambda f: f is None }})
+    pos: Optional[TermUpdatePos] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})
+    tags: Optional[list[shared_termtagcreate.TermTagCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tags'), 'exclude': lambda f: f is None }})
     
-    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})  
-    term: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('term') }})  
-    type: TermCreateTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})  
-    approved_term_extension: Optional[shared_approvedtermextensioncreate.ApprovedTermExtensionCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('approvedTermExtension'), 'exclude': lambda f: f is None }})  
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})  
-    examples: Optional[list[shared_termexamplecreate.TermExampleCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('examples'), 'exclude': lambda f: f is None }})  
-    highlight: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('highlight'), 'exclude': lambda f: f is None }})  
-    linked_terms: Optional[list[shared_linkedtermcreate.LinkedTermCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkedTerms'), 'exclude': lambda f: f is None }})  
-    mistakes: Optional[list[shared_termmistakecreate.TermMistakeCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mistakes'), 'exclude': lambda f: f is None }})  
-    pos: Optional[TermCreatePosEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})  
-    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})  
-    tags: Optional[list[shared_termtagcreate.TermTagCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tags'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/termexample.py` & `writerai-0.6.0/src/writer/models/shared/termexample.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from writer import utils
 
-class TermExampleTypeEnum(str, Enum):
+class TermExampleType(str, Enum):
     GOOD = 'good'
     BAD = 'bad'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class TermExample:
+    example: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('example') }})
+    term_bank_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termBankId') }})
+    term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termId') }})
+    type: TermExampleType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     
-    example: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('example') }})  
-    term_bank_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termBankId') }})  
-    term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termId') }})  
-    type: TermExampleTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})  
-    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/termexamplecreate.py` & `writerai-0.6.0/src/writer/models/shared/approvedtermextension.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
+from typing import Optional
 from writer import utils
 
-class TermExampleCreateTypeEnum(str, Enum):
-    GOOD = 'good'
-    BAD = 'bad'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class TermExampleCreate:
+class ApprovedTermExtension:
+    capitalize: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('capitalize') }})
+    fix_case: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fixCase') }})
+    fix_common_mistakes: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fixCommonMistakes') }})
+    term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termId') }})
+    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     
-    example: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('example') }})  
-    type: TermExampleCreateTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/terminologyuser.py` & `writerai-0.6.0/src/writer/models/shared/contentdetectorresponse.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from enum import Enum
 from writer import utils
 
+class ContentDetectorResponseLabel(str, Enum):
+    FAKE = 'fake'
+    REAL = 'real'
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class TerminologyUser:
+class ContentDetectorResponse:
+    label: ContentDetectorResponseLabel = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label') }})
+    score: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('score') }})
     
-    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})  
-    full_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fullName'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/termmistake.py` & `writerai-0.6.0/src/writer/models/shared/termmistake.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from writer import utils
 
-class TermMistakePosEnum(str, Enum):
+class TermMistakePos(str, Enum):
     NOUN = 'noun'
     VERB = 'verb'
     ADVERB = 'adverb'
     ADJECTIVE = 'adjective'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class TermMistake:
+    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})
+    mistake: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mistake') }})
+    term_bank_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termBankId') }})
+    term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termId') }})
+    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    pos: Optional[TermMistakePos] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})
     
-    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})  
-    mistake: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mistake') }})  
-    term_bank_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termBankId') }})  
-    term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termId') }})  
-    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})  
-    pos: Optional[TermMistakePosEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/termtagresponse.py` & `writerai-0.6.0/src/writer/models/shared/failresponse.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ..shared import failmessage as shared_failmessage
 from dataclasses_json import Undefined, dataclass_json
+from typing import Any, Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class TermTagResponse:
+class FailResponse:
+    r"""Bad Request"""
+    extras: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('extras') }})
+    tpe: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tpe') }})
+    errors: Optional[list[shared_failmessage.FailMessage]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errors'), 'exclude': lambda f: f is None }})
     
-    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
-    parent_tag_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentTagId') }})  
-    tag: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag') }})  
-    term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termId') }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/termupdate.py` & `writerai-0.6.0/src/writer/models/shared/userpublicresponse.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,34 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import approvedtermextensioncreate as shared_approvedtermextensioncreate
-from ..shared import linkedtermcreate as shared_linkedtermcreate
-from ..shared import termexamplecreate as shared_termexamplecreate
-from ..shared import termmistakecreate as shared_termmistakecreate
-from ..shared import termtagcreate as shared_termtagcreate
+import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
+from datetime import datetime
 from enum import Enum
+from marshmallow import fields
 from typing import Optional
 from writer import utils
 
-class TermUpdatePosEnum(str, Enum):
-    NOUN = 'noun'
-    VERB = 'verb'
-    ADVERB = 'adverb'
-    ADJECTIVE = 'adjective'
-
-class TermUpdateTypeEnum(str, Enum):
-    APPROVED = 'approved'
-    BANNED = 'banned'
-    PENDING = 'pending'
+class UserPublicResponseAccountStatus(str, Enum):
+    INVITED = 'invited'
+    SIGNED_UP = 'signed_up'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class TermUpdate:
+class UserPublicResponse:
+    account_status: UserPublicResponseAccountStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountStatus') }})
+    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    first_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName') }})
+    full_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fullName') }})
+    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    avatar: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('avatar'), 'exclude': lambda f: f is None }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    invited_by: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invitedBy'), 'exclude': lambda f: f is None }})
+    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
+    last_seen_online: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastSeenOnline'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    timezone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timezone'), 'exclude': lambda f: f is None }})
     
-    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})  
-    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
-    term: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('term') }})  
-    type: TermUpdateTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})  
-    approved_term_extension: Optional[shared_approvedtermextensioncreate.ApprovedTermExtensionCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('approvedTermExtension'), 'exclude': lambda f: f is None }})  
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})  
-    examples: Optional[list[shared_termexamplecreate.TermExampleCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('examples'), 'exclude': lambda f: f is None }})  
-    highlight: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('highlight'), 'exclude': lambda f: f is None }})  
-    linked_terms: Optional[list[shared_linkedtermcreate.LinkedTermCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkedTerms'), 'exclude': lambda f: f is None }})  
-    mistakes: Optional[list[shared_termmistakecreate.TermMistakeCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mistakes'), 'exclude': lambda f: f is None }})  
-    pos: Optional[TermUpdatePosEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})  
-    tags: Optional[list[shared_termtagcreate.TermTagCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tags'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/updatetermsrequest.py` & `writerai-0.6.0/src/writer/models/shared/updatetermsrequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 import dataclasses
 from ..shared import termupdate as shared_termupdate
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from writer import utils
 
-class UpdateTermsRequestFailHandlingEnum(str, Enum):
+class UpdateTermsRequestFailHandling(str, Enum):
     ACCUMULATE = 'accumulate'
     VALIDATE = 'validate'
     SKIP = 'skip'
     VALIDATE_ONLY = 'validateOnly'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class UpdateTermsRequest:
+    fail_handling: Optional[UpdateTermsRequestFailHandling] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('failHandling'), 'exclude': lambda f: f is None }})
+    models: Optional[list[shared_termupdate.TermUpdate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('models'), 'exclude': lambda f: f is None }})
     
-    fail_handling: Optional[UpdateTermsRequestFailHandlingEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('failHandling'), 'exclude': lambda f: f is None }})  
-    models: Optional[list[shared_termupdate.TermUpdate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('models'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/uploadmodelfilerequest.py` & `writerai-0.6.0/src/writer/models/shared/uploadmodelfilerequest.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 
 
+
 @dataclasses.dataclass
 class UploadModelFileRequestFile:
+    content: bytes = dataclasses.field(metadata={'multipart_form': { 'content': True }})
+    file: str = dataclasses.field(metadata={'multipart_form': { 'field_name': 'file' }})
     
-    content: bytes = dataclasses.field(metadata={'multipart_form': { 'content': True }})  
-    file: str = dataclasses.field(metadata={'multipart_form': { 'field_name': 'file' }})  
-    
+
+
+
 
 @dataclasses.dataclass
 class UploadModelFileRequest:
+    file: UploadModelFileRequestFile = dataclasses.field(metadata={'multipart_form': { 'file': True }})
     
-    file: UploadModelFileRequestFile = dataclasses.field(metadata={'multipart_form': { 'file': True }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/usage.py` & `writerai-0.6.0/src/writer/models/shared/usage.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import dataclasses
 from ..shared import usageitem as shared_usageitem
 from dataclasses_json import Undefined, dataclass_json
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class Usage:
+    co_write_words: shared_usageitem.UsageItem = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('coWriteWords') }})
+    team: shared_usageitem.UsageItem = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('team') }})
+    user: shared_usageitem.UsageItem = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('user') }})
+    words: shared_usageitem.UsageItem = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('words') }})
     
-    co_write_words: shared_usageitem.UsageItem = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('coWriteWords') }})  
-    team: shared_usageitem.UsageItem = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('team') }})  
-    user: shared_usageitem.UsageItem = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('user') }})  
-    words: shared_usageitem.UsageItem = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('words') }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/usageitem.py` & `writerai-0.6.0/src/writer/models/shared/termtagresponse.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,13 +3,16 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class UsageItem:
+class TermTagResponse:
+    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    parent_tag_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentTagId') }})
+    tag: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag') }})
+    term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termId') }})
     
-    limit: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('limit') }})  
-    value: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value') }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models/shared/userpublicresponse.py` & `writerai-0.6.0/src/writer/models/shared/completionrequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from enum import Enum
-from marshmallow import fields
 from typing import Optional
 from writer import utils
 
-class UserPublicResponseAccountStatusEnum(str, Enum):
-    INVITED = 'invited'
-    SIGNED_UP = 'signed_up'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class UserPublicResponse:
+class CompletionRequest:
+    prompt: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prompt') }})
+    best_of: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bestOf'), 'exclude': lambda f: f is None }})
+    frequency_penalty: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('frequencyPenalty'), 'exclude': lambda f: f is None }})
+    logprobs: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logprobs'), 'exclude': lambda f: f is None }})
+    max_tokens: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maxTokens'), 'exclude': lambda f: f is None }})
+    min_tokens: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minTokens'), 'exclude': lambda f: f is None }})
+    n: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('n'), 'exclude': lambda f: f is None }})
+    presence_penalty: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('presencePenalty'), 'exclude': lambda f: f is None }})
+    stop: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stop'), 'exclude': lambda f: f is None }})
+    temperature: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('temperature'), 'exclude': lambda f: f is None }})
+    top_p: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('topP'), 'exclude': lambda f: f is None }})
     
-    account_status: UserPublicResponseAccountStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountStatus') }})  
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
-    first_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName') }})  
-    full_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fullName') }})  
-    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
-    avatar: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('avatar'), 'exclude': lambda f: f is None }})  
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})  
-    invited_by: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invitedBy'), 'exclude': lambda f: f is None }})  
-    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})  
-    last_seen_online: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastSeenOnline'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})  
-    timezone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timezone'), 'exclude': lambda f: f is None }})  
-    
+
```

### Comparing `writerai-0.4.0/src/writer/models_.py` & `writerai-0.6.0/src/writer/models_.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-import requests as requests_http
-from . import utils
-from typing import Any, Optional
+from .sdkconfiguration import SDKConfiguration
+from typing import Optional
+from writer import utils
 from writer.models import operations, shared
 
 class Models:
     r"""Methods related to Model"""
-    _client: requests_http.Session
-    _security_client: requests_http.Session
-    _server_url: str
-    _language: str
-    _sdk_version: str
-    _gen_version: str
-    _globals: dict[str, dict[str, dict[str, Any]]]
+    sdk_configuration: SDKConfiguration
 
-    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str, gbls: dict[str, dict[str, dict[str, Any]]]) -> None:
-        self._client = client
-        self._security_client = security_client
-        self._server_url = server_url
-        self._language = language
-        self._sdk_version = sdk_version
-        self._gen_version = gen_version
-        self._globals = gbls
+    def __init__(self, sdk_config: SDKConfiguration) -> None:
+        self.sdk_configuration = sdk_config
         
-    def list(self, request: operations.ListModelsRequest) -> operations.ListModelsResponse:
+    
+    def list(self, organization_id: Optional[int] = None) -> operations.ListModelsResponse:
         r"""List available LLM models"""
-        base_url = self._server_url
+        request = operations.ListModelsRequest(
+            organization_id=organization_id,
+        )
         
-        url = utils.generate_url(operations.ListModelsRequest, base_url, '/llm/organization/{organizationId}/model', request, self._globals)
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
+        url = utils.generate_url(operations.ListModelsRequest, base_url, '/llm/organization/{organizationId}/model', request, self.sdk_configuration.globals)
+        headers = {}
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
-        http_res = client.request('GET', url)
+        http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListModelsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
```

### Comparing `writerai-0.4.0/src/writer/utils/retries.py` & `writerai-0.6.0/src/writer/utils/retries.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 
 
 class RetryConfig:
     strategy: str
     backoff: BackoffStrategy
     retry_connection_errors: bool
 
-    def __init__(self, strategy: str, retry_connection_errors: bool):
+    def __init__(self, strategy: str, backoff: BackoffStrategy, retry_connection_errors: bool):
         self.strategy = strategy
+        self.backoff = backoff
         self.retry_connection_errors = retry_connection_errors
 
 
 class Retries:
     config: RetryConfig
     status_codes: list[str]
```

### Comparing `writerai-0.4.0/src/writer/utils/utils.py` & `writerai-0.6.0/src/writer/utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             raise Exception('not supported')
     elif scheme_type == "openIdConnect":
         client.client.headers[header_name] = value
     elif scheme_type == 'oauth2':
         client.client.headers[header_name] = value
     elif scheme_type == 'http':
         if sub_type == 'bearer':
-            client.client.headers[header_name] = value
+            client.client.headers[header_name] = value.lower().startswith('bearer ') and value or f'Bearer {value}'
         else:
             raise Exception('not supported')
     else:
         raise Exception('not supported')
 
 
 def _parse_basic_auth_scheme(client: SecurityClient, scheme: dataclass):
@@ -137,15 +137,16 @@
         if field_name == 'password':
             password = value
 
     data = f'{username}:{password}'.encode()
     client.client.headers['Authorization'] = f'Basic {base64.b64encode(data).decode()}'
 
 
-def generate_url(clazz: type, server_url: str, path: str, path_params: dataclass, gbls: dict[str, dict[str, dict[str, Any]]] = None) -> str:
+def generate_url(clazz: type, server_url: str, path: str, path_params: dataclass,
+                 gbls: dict[str, dict[str, dict[str, Any]]] = None) -> str:
     path_param_fields: Tuple[Field, ...] = fields(clazz)
     for field in path_param_fields:
         request_metadata = field.metadata.get('request')
         if request_metadata is not None:
             continue
 
         param_metadata = field.metadata.get('path_param')
@@ -229,15 +230,16 @@
     for key, value in params.items():
         url_with_params = url_with_params.replace(
             '{' + key + '}', value)
 
     return url_with_params
 
 
-def get_query_params(clazz: type, query_params: dataclass, gbls: dict[str, dict[str, dict[str, Any]]] = None) -> dict[str, list[str]]:
+def get_query_params(clazz: type, query_params: dataclass, gbls: dict[str, dict[str, dict[str, Any]]] = None) -> dict[
+    str, list[str]]:
     params: dict[str, list[str]] = {}
 
     param_fields: Tuple[Field, ...] = fields(clazz)
     for field in param_fields:
         request_metadata = field.metadata.get('request')
         if request_metadata is not None:
             continue
@@ -263,16 +265,19 @@
                     params[key] = [value]
         else:
             style = metadata.get('style', 'form')
             if style == 'deepObject':
                 params = params | _get_deep_object_query_params(
                     metadata, f_name, value)
             elif style == 'form':
-                params = params | _get_form_query_params(
-                    metadata, f_name, value)
+                params = params | _get_delimited_query_params(
+                    metadata, f_name, value, ",")
+            elif style == 'pipeDelimited':
+                params = params | _get_delimited_query_params(
+                    metadata, f_name, value, "|")
             else:
                 raise Exception('not yet implemented')
     return params
 
 
 def get_headers(headers_params: dataclass) -> dict[str, str]:
     if headers_params is None:
@@ -323,20 +328,23 @@
                 continue
 
             if isinstance(obj_val, list):
                 for val in obj_val:
                     if val is None:
                         continue
 
-                    if params.get(f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
-                        params[f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
+                    if params.get(
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
+                        params[
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
                         ]
 
                     params[
-                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(_val_to_string(val))
+                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(
+                        _val_to_string(val))
             else:
                 params[
                     f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
                     _val_to_string(obj_val)]
     elif isinstance(obj, dict):
         for key, value in obj.items():
             if value is None:
@@ -364,48 +372,52 @@
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _get_form_query_params(metadata: dict, field_name: str, obj: any) -> dict[str, list[str]]:
-    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name)
+def _get_delimited_query_params(metadata: dict, field_name: str, obj: any, delimiter: str) -> dict[
+    str, list[str]]:
+    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name, delimiter)
 
 
 SERIALIZATION_METHOD_TO_CONTENT_TYPE = {
-    'json':      'application/json',
-    'form':      'application/x-www-form-urlencoded',
+    'json': 'application/json',
+    'form': 'application/x-www-form-urlencoded',
     'multipart': 'multipart/form-data',
-    'raw':       'application/octet-stream',
-    'string':    'text/plain',
+    'raw': 'application/octet-stream',
+    'string': 'text/plain',
 }
 
 
-def serialize_request_body(request: dataclass, request_field_name: str, serialization_method: str) -> Tuple[str, any, any]:
+def serialize_request_body(request: dataclass, request_field_name: str, serialization_method: str) -> Tuple[
+    str, any, any]:
     if request is None:
         return None, None, None, None
 
     if not is_dataclass(request) or not hasattr(request, request_field_name):
-        return serialize_content_type(request_field_name, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method], request)
+        return serialize_content_type(request_field_name, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
+                                      request)
 
     request_val = getattr(request, request_field_name)
 
     request_fields: Tuple[Field, ...] = fields(request)
     request_metadata = None
 
     for field in request_fields:
         if field.name == request_field_name:
             request_metadata = field.metadata.get('request')
             break
 
     if request_metadata is None:
         raise Exception('invalid request type')
 
-    return serialize_content_type(request_field_name, request_metadata.get('media_type', 'application/octet-stream'), request_val)
+    return serialize_content_type(request_field_name, request_metadata.get('media_type', 'application/octet-stream'),
+                                  request_val)
 
 
 def serialize_content_type(field_name: str, media_type: str, request: dataclass) -> Tuple[str, any, list[list[any]]]:
     if re.match(r'(application|text)\/.*?\+*json.*', media_type) is not None:
         return media_type, marshal_json(request), None
     if re.match(r'multipart\/.*', media_type) is not None:
         return serialize_multipart_form(media_type, request)
@@ -470,15 +482,15 @@
                         [field_name + "[]", [None, _val_to_string(value)]])
             else:
                 form.append([field_name, [None, _val_to_string(val)]])
     return media_type, None, form
 
 
 def serialize_dict(original: dict, explode: bool, field_name, existing: Optional[dict[str, list[str]]]) -> dict[
-        str, list[str]]:
+    str, list[str]]:
     if existing is None:
         existing = []
 
     if explode is True:
         for key, val in original.items():
             if key not in existing:
                 existing[key] = []
@@ -510,15 +522,15 @@
             field_name = metadata.get('field_name', field.name)
 
             if metadata.get('json'):
                 form[field_name] = [marshal_json(val)]
             else:
                 if metadata.get('style', 'form') == 'form':
                     form = form | _populate_form(
-                        field_name, metadata.get('explode', True), val, _get_form_field_name)
+                        field_name, metadata.get('explode', True), val, _get_form_field_name, ",")
                 else:
                     raise Exception(
                         f'Invalid form style for field {field.name}')
     elif isinstance(data, dict):
         for key, value in data.items():
             form[key] = [_val_to_string(value)]
     else:
@@ -532,15 +544,16 @@
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable) -> dict[str, list[str]]:
+def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable, delimiter: str) -> \
+        dict[str, list[str]]:
     params: dict[str, list[str]] = {}
 
     if obj is None:
         return params
 
     if is_dataclass(obj):
         items = []
@@ -555,31 +568,31 @@
             if val is None:
                 continue
 
             if explode:
                 params[obj_field_name] = [_val_to_string(val)]
             else:
                 items.append(
-                    f'{obj_field_name},{_val_to_string(val)}')
+                    f'{obj_field_name}{delimiter}{_val_to_string(val)}')
 
         if len(items) > 0:
-            params[field_name] = [','.join(items)]
+            params[field_name] = [delimiter.join(items)]
     elif isinstance(obj, dict):
         items = []
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
                 params[key] = _val_to_string(value)
             else:
-                items.append(f'{key},{_val_to_string(value)}')
+                items.append(f'{key}{delimiter}{_val_to_string(value)}')
 
         if len(items) > 0:
-            params[field_name] = [','.join(items)]
+            params[field_name] = [delimiter.join(items)]
     elif isinstance(obj, list):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
@@ -587,15 +600,15 @@
                 if not field_name in params:
                     params[field_name] = []
                 params[field_name].append(_val_to_string(value))
             else:
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            params[field_name] = [','.join([str(item) for item in items])]
+            params[field_name] = [delimiter.join([str(item) for item in items])]
     else:
         params[field_name] = [_val_to_string(obj)]
 
     return params
 
 
 def _serialize_header(explode: bool, obj: any) -> str:
@@ -727,15 +740,15 @@
 
 def _val_to_string(val):
     if isinstance(val, bool):
         return str(val).lower()
     if isinstance(val, datetime):
         return val.isoformat().replace('+00:00', 'Z')
     if isinstance(val, Enum):
-        return val.value
+        return str(val.value)
 
     return str(val)
 
 
 def _populate_from_globals(param_name: str, value: any, param_type: str, gbls: dict[str, dict[str, dict[str, Any]]]):
     if value is None and gbls is not None:
         if 'parameters' in gbls:
```

### Comparing `writerai-0.4.0/src/writerai.egg-info/SOURCES.txt` & `writerai-0.6.0/src/writerai.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 setup.py
 src/writer/__init__.py
 src/writer/ai_content_detector.py
 src/writer/billing.py
 src/writer/completions.py
 src/writer/content.py
 src/writer/cowrite.py
+src/writer/document.py
 src/writer/download_the_customized_model.py
 src/writer/files.py
 src/writer/modelcustomization.py
 src/writer/models_.py
 src/writer/sdk.py
+src/writer/sdkconfiguration.py
 src/writer/snippet.py
 src/writer/styleguide.py
 src/writer/terminology.py
 src/writer/user.py
 src/writer/models/__init__.py
 src/writer/models/operations/__init__.py
 src/writer/models/operations/addterms.py
@@ -28,30 +30,34 @@
 src/writer/models/operations/deletesnippets.py
 src/writer/models/operations/deleteterms.py
 src/writer/models/operations/detectcontent.py
 src/writer/models/operations/fetchcustomizedmodelfile.py
 src/writer/models/operations/findsnippets.py
 src/writer/models/operations/findterms.py
 src/writer/models/operations/generate_content.py
+src/writer/models/operations/getdocumentdetails.py
 src/writer/models/operations/getfile.py
 src/writer/models/operations/getmodelcustomization.py
 src/writer/models/operations/getsubscriptiondetails.py
 src/writer/models/operations/listfiles.py
 src/writer/models/operations/listmodelcustomizations.py
 src/writer/models/operations/listmodels.py
 src/writer/models/operations/listpages.py
+src/writer/models/operations/listteamdocuments.py
 src/writer/models/operations/listtemplates.py
 src/writer/models/operations/listusers.py
 src/writer/models/operations/pagedetails.py
 src/writer/models/operations/updatesnippets.py
 src/writer/models/operations/updateterms.py
 src/writer/models/operations/uploadfile.py
 src/writer/models/shared/__init__.py
 src/writer/models/shared/approvedtermextension.py
 src/writer/models/shared/approvedtermextensioncreate.py
+src/writer/models/shared/briefdocument.py
+src/writer/models/shared/briefdocuments.py
 src/writer/models/shared/completiongenerationchoice.py
 src/writer/models/shared/completiongenerationchoicelogprobs.py
 src/writer/models/shared/completionrequest.py
 src/writer/models/shared/completionresponse.py
 src/writer/models/shared/contentdetectorrequest.py
 src/writer/models/shared/contentdetectorresponse.py
 src/writer/models/shared/contentissue.py
@@ -59,14 +65,15 @@
 src/writer/models/shared/contentsettings.py
 src/writer/models/shared/correctionresponse.py
 src/writer/models/shared/createcustomizationrequest.py
 src/writer/models/shared/createtermsrequest.py
 src/writer/models/shared/createtermsresponse.py
 src/writer/models/shared/customizationsresponse.py
 src/writer/models/shared/deleteresponse.py
+src/writer/models/shared/document.py
 src/writer/models/shared/draft.py
 src/writer/models/shared/failmessage.py
 src/writer/models/shared/failresponse.py
 src/writer/models/shared/fulllinkedterm.py
 src/writer/models/shared/fulltermwithuser.py
 src/writer/models/shared/generatetemplaterequest.py
 src/writer/models/shared/generationmodelinforesponse.py
```

