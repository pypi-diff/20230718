# Comparing `tmp/recipe_scrapers-9.2.5.tar.gz` & `tmp/recipe_scrapers-9.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recipe_scrapers-9.2.5.tar", last modified: Sat Oct  3 01:56:24 2020, max compression
+gzip compressed data, was "dist/recipe_scrapers-9.2.6.tar", last modified: Sat Oct  3 22:44:38 2020, max compression
```

## Comparing `recipe_scrapers-9.2.5.tar` & `recipe_scrapers-9.2.6.tar`

### file list

```diff
@@ -1,115 +1,116 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-03 01:56:24.000000 recipe_scrapers-9.2.5/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       86 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    11831 2020-10-03 01:56:24.000000 recipe_scrapers-9.2.5/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     9545 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-03 01:56:24.000000 recipe_scrapers-9.2.5/recipe_scrapers/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9026 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/__version__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4116 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/_abstract.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2178 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/_decorators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2125 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/_exception_handling.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5278 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/_schemaorg.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2451 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      528 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/acouplecooks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      585 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/allrecipes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      597 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/ambitiouskitchen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      538 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/archanaskitchen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      587 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/averiecooks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1729 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/bbcfood.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      653 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/bbcgoodfood.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2514 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/bettycrocker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      444 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/bonappetit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      595 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/bowlofdelicious.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1317 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/budgetbytes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      580 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/chefkoch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      974 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/closetcooking.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1234 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/cookieandkate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      579 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/cookpad.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1511 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/cookstr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3967 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/copykat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1108 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/countryliving.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      586 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/cybercook.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1779 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/delish.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      608 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/eatsmarter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2280 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/epicurious.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      595 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/fifteenspatulas.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1615 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/finedininglovers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1391 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/fitmencook.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      914 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/food.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1239 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/foodnetwork.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1076 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/foodrepublic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1372 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/geniuskitchen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1637 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/giallozafferano.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      591 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/gimmesomeoven.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4315 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/gonnawantseconds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1989 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/gousto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2427 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/greatbritishchefs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      597 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/halfbakedharvest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      585 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/hassenchef.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      979 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/heinzbrasil.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2151 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/hellofresh.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      589 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/hostthetoast.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1016 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/hundredandonecookbooks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1403 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/ig.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      899 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/inspiralized.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/jamieoliver.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1673 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/justbento.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1088 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/kennymcgovern.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      517 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/kochbar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      597 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/lecremedelacrumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      587 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/livelytable.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      591 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/lovingitvegan.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      581 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/marmiton.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2500 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/matprat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1407 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/mindmegette.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      595 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/minimalistbaker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      576 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/misya.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1329 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/momswithcrockpots.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1317 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/motherthyme.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1242 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/mybakingaddiction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      583 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/myrecipes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1309 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/nihhealthyeating.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      605 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/nourishedbynutrition.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1290 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/nutritionbynathalie.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      587 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/nytimes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      585 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/ohsheglows.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1062 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/panelinha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1055 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/paninihappy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1006 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/przepisy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      585 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/purelypope.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1144 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/realsimple.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1126 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/seriouseats.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1319 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/simplyquinoa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1156 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/simplyrecipes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      587 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/skinnytaste.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3359 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/southernliving.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      625 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/spendwithpennies.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1303 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/steamykitchen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      587 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/tasteofhome.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1073 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/tastesoflizzyt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      574 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/tasty.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1228 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/tastykitchen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1799 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/thehappyfoodie.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1037 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/thekitchn.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      543 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/thenutritiouskitchen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1053 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/thepioneerwoman.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      720 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/thespruceeats.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1266 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/thevintagemixer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      591 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/thewoksoflife.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3275 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/tineno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      898 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/tudogostoso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1333 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/twopeasandtheirpod.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2116 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/vegolosi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      591 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/watchwhatueat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      956 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/whatsgabycooking.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1219 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/wikicookbook.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1469 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/recipe_scrapers/yummly.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-03 01:56:24.000000 recipe_scrapers-9.2.5/recipe_scrapers.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11831 2020-10-03 01:56:24.000000 recipe_scrapers-9.2.5/recipe_scrapers.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3424 2020-10-03 01:56:24.000000 recipe_scrapers-9.2.5/recipe_scrapers.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-03 01:56:24.000000 recipe_scrapers-9.2.5/recipe_scrapers.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       93 2020-10-03 01:56:24.000000 recipe_scrapers-9.2.5/recipe_scrapers.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2020-10-03 01:56:24.000000 recipe_scrapers-9.2.5/recipe_scrapers.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-10-03 01:56:24.000000 recipe_scrapers-9.2.5/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1337 2020-10-03 01:54:34.000000 recipe_scrapers-9.2.5/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-03 22:44:38.000000 recipe_scrapers-9.2.6/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       86 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11902 2020-10-03 22:44:38.000000 recipe_scrapers-9.2.6/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-03 22:44:38.000000 recipe_scrapers-9.2.6/recipe_scrapers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1303 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/steamykitchen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3978 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/_abstract.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      914 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/food.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      585 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/ohsheglows.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1637 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/giallozafferano.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      591 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/thewoksoflife.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2116 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/vegolosi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      606 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/eatsmarter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2500 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/matprat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1108 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/countryliving.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5846 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/_schemaorg.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      898 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/tudogostoso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      595 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/minimalistbaker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1239 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/foodnetwork.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      956 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/whatsgabycooking.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      576 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/misya.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      586 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/cybercook.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2427 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/greatbritishchefs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      597 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/halfbakedharvest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      587 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/livelytable.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1469 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/yummly.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1391 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/fitmencook.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1372 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/geniuskitchen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3275 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/tineno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1309 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/nihhealthyeating.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1144 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/realsimple.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      517 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/kochbar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1062 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/panelinha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1317 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/budgetbytes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1403 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/ig.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/__version__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      653 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/bbcgoodfood.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      585 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/purelypope.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      579 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/cookpad.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      444 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/bonappetit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      538 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/archanaskitchen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      605 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/nourishedbynutrition.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3967 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/copykat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      581 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/marmiton.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1053 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/thepioneerwoman.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1156 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/simplyrecipes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2211 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/hellofresh.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      595 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/fifteenspatulas.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1615 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/finedininglovers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      585 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/allrecipes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1989 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/gousto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1088 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/kennymcgovern.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1219 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/wikicookbook.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      899 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/inspiralized.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1016 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/hundredandonecookbooks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      532 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/eatwhattonight.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1073 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/tastesoflizzyt.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1799 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/thehappyfoodie.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      979 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/heinzbrasil.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1006 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/przepisy.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      543 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/thenutritiouskitchen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1126 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/seriouseats.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1266 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/thevintagemixer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      591 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/lovingitvegan.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2125 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/_exception_handling.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      597 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/ambitiouskitchen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1319 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/simplyquinoa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      587 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/tasteofhome.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4315 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/gonnawantseconds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3359 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/southernliving.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      528 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/acouplecooks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1511 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/cookstr.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      587 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/averiecooks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      625 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/spendwithpennies.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      587 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/skinnytaste.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/bbcfood.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      574 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/tasty.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1329 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/momswithcrockpots.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      591 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/watchwhatueat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1779 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/delish.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      591 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/gimmesomeoven.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1055 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/paninihappy.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      597 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/lecremedelacrumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1037 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/thekitchn.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9112 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1333 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/twopeasandtheirpod.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1290 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/nutritionbynathalie.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/jamieoliver.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      583 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/myrecipes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1947 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/epicurious.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1317 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/motherthyme.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1242 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/mybakingaddiction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2451 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1234 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/cookieandkate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2514 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/bettycrocker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      595 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/bowlofdelicious.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1401 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/mindmegette.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1228 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/tastykitchen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      585 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/hassenchef.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      720 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/thespruceeats.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2178 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/_decorators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1673 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/justbento.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      589 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/hostthetoast.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1076 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/foodrepublic.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      580 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/chefkoch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      974 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/closetcooking.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      587 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/recipe_scrapers/nytimes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-10-03 22:44:38.000000 recipe_scrapers-9.2.6/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9608 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-03 22:44:38.000000 recipe_scrapers-9.2.6/recipe_scrapers.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11902 2020-10-03 22:44:38.000000 recipe_scrapers-9.2.6/recipe_scrapers.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-03 22:44:38.000000 recipe_scrapers-9.2.6/recipe_scrapers.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2020-10-03 22:44:38.000000 recipe_scrapers-9.2.6/recipe_scrapers.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3458 2020-10-03 22:44:38.000000 recipe_scrapers-9.2.6/recipe_scrapers.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       93 2020-10-03 22:44:38.000000 recipe_scrapers-9.2.6/recipe_scrapers.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1337 2020-10-03 22:42:42.000000 recipe_scrapers-9.2.6/setup.py
```

### Comparing `recipe_scrapers-9.2.5/LICENSE` & `recipe_scrapers-9.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/PKG-INFO` & `recipe_scrapers-9.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: recipe_scrapers
-Version: 9.2.5
+Version: 9.2.6
 Summary: Python package, scraping recipes from all over the internet
 Home-page: https://github.com/hhursev/recipe-scrapers/
 Author: Hristo Harsev
 Author-email: r+pypi@hharsev.com
 License: UNKNOWN
 Description: .. image:: https://img.shields.io/pypi/v/recipe-scrapers.svg?
             :target: https://pypi.org/project/recipe-scrapers/
@@ -76,14 +76,15 @@
         - `https://cookstr.com/ <https://cookstr.com>`_
         - `https://copykat.com/ <https://copykat.com>`_
         - `https://countryliving.com/ <https://countryliving.com>`_
         - `https://cybercook.com.br/ <https://cybercook.com.br/>`_
         - `https://delish.com/ <https://delish.com>`_
         - `https://eatsmarter.com/ <https://eatsmarter.com/>`_
         - `https://eatsmarter.de/ <https://eatsmarter.de/>`_
+        - `https://eatwhattonight.com/ <https://eatwhattonight.com/>`_
         - `https://epicurious.com/ <https://epicurious.com>`_
         - `https://fifteenspatulas.com/ <https://www.fifteenspatulas.com/>`_
         - `https://finedininglovers.com/ <https://www.finedininglovers.com>`_
         - `https://fitmencook.com/ <https://www.fitmencook.com>`_
         - `https://food.com/ <https://www.food.com>`_
         - `https://foodnetwork.com/ <https://www.foodnetwork.com>`_
         - `https://foodrepublic.com/ <https://foodrepublic.com>`_
```

### Comparing `recipe_scrapers-9.2.5/README.rst` & `recipe_scrapers-9.2.6/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 - `https://cookstr.com/ <https://cookstr.com>`_
 - `https://copykat.com/ <https://copykat.com>`_
 - `https://countryliving.com/ <https://countryliving.com>`_
 - `https://cybercook.com.br/ <https://cybercook.com.br/>`_
 - `https://delish.com/ <https://delish.com>`_
 - `https://eatsmarter.com/ <https://eatsmarter.com/>`_
 - `https://eatsmarter.de/ <https://eatsmarter.de/>`_
+- `https://eatwhattonight.com/ <https://eatwhattonight.com/>`_
 - `https://epicurious.com/ <https://epicurious.com>`_
 - `https://fifteenspatulas.com/ <https://www.fifteenspatulas.com/>`_
 - `https://finedininglovers.com/ <https://www.finedininglovers.com>`_
 - `https://fitmencook.com/ <https://www.fitmencook.com>`_
 - `https://food.com/ <https://www.food.com>`_
 - `https://foodnetwork.com/ <https://www.foodnetwork.com>`_
 - `https://foodrepublic.com/ <https://foodrepublic.com>`_
```

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/__init__.py` & `recipe_scrapers-9.2.6/recipe_scrapers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from .cookpad import CookPad
 from .cookstr import Cookstr
 from .copykat import CopyKat
 from .countryliving import CountryLiving
 from .cybercook import Cybercook
 from .delish import Delish
 from .eatsmarter import Eatsmarter
+from .eatwhattonight import EatWhatTonight
 from .epicurious import Epicurious
 from .fifteenspatulas import FifteenSpatulas
 from .finedininglovers import FineDiningLovers
 from .fitmencook import FitMenCook
 from .food import Food
 from .foodnetwork import FoodNetwork
 from .foodrepublic import FoodRepublic
@@ -117,14 +118,15 @@
     Cookstr.host(): Cookstr,
     CopyKat.host(): CopyKat,
     CountryLiving.host(): CountryLiving,
     Cybercook.host(): Cybercook,
     Delish.host(): Delish,
     Eatsmarter.host(): Eatsmarter,
     Eatsmarter.host(domain="de"): Eatsmarter,
+    EatWhatTonight.host(): EatWhatTonight,
     Epicurious.host(): Epicurious,
     FifteenSpatulas.host(): FifteenSpatulas,
     FineDiningLovers.host(): FineDiningLovers,
     FitMenCook.host(): FitMenCook,
     Food.host(): Food,
     FoodNetwork.host(): FoodNetwork,
     FoodRepublic.host(): FoodRepublic,
```

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/_abstract.py` & `recipe_scrapers-9.2.6/recipe_scrapers/_abstract.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,18 +21,14 @@
             page_data = requests.get(url, headers=HEADERS).content
 
         self.exception_handling = exception_handling
         self.meta_http_equiv = meta_http_equiv
         self.soup = BeautifulSoup(page_data, "html.parser")
         self.schema = SchemaOrg(page_data, host=self.host())
         self.url = url
-        # if self.schema.data:
-        #     print("Class: %s has schema." % (
-        #         self.__class__.__name__
-        #     ))
 
     def url(self):
         return self.url
 
     @classmethod
     def host(cls):
         """ get the hostdef of the url, so we can use the correct scraper """
```

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/_decorators.py` & `recipe_scrapers-9.2.6/recipe_scrapers/_decorators.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/_exception_handling.py` & `recipe_scrapers-9.2.6/recipe_scrapers/_exception_handling.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/_schemaorg.py` & `recipe_scrapers-9.2.6/recipe_scrapers/_schemaorg.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,16 +109,25 @@
         ]
 
     def _extract_howto_instructions_text(self, schema_item):
         instructions_gist = []
         if type(schema_item) is str:
             instructions_gist.append(schema_item)
         elif schema_item.get("@type") == "HowToStep":
+            if schema_item.get("name", False):
+                # some sites have duplicated name and text properties (1:1)
+                # others have name same as text but truncated to X chars.
+                # ignore name in these cases and add the name value only if it's different from the text
+                if not schema_item.get("text").startswith(
+                    schema_item.get("name").rstrip(".")
+                ):
+                    instructions_gist.append(schema_item.get("name"))
             instructions_gist.append(schema_item.get("text"))
         elif schema_item.get("@type") == "HowToSection":
+            instructions_gist.append(schema_item.get("name"))
             for item in schema_item.get("itemListElement"):
                 instructions_gist += self._extract_howto_instructions_text(item)
         return instructions_gist
 
     def instructions(self):
         instructions = self.data.get("recipeInstructions") or ""
```

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/_utils.py` & `recipe_scrapers-9.2.6/recipe_scrapers/_utils.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/acouplecooks.py` & `recipe_scrapers-9.2.6/recipe_scrapers/acouplecooks.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/allrecipes.py` & `recipe_scrapers-9.2.6/recipe_scrapers/allrecipes.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/ambitiouskitchen.py` & `recipe_scrapers-9.2.6/recipe_scrapers/ambitiouskitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/archanaskitchen.py` & `recipe_scrapers-9.2.6/recipe_scrapers/archanaskitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/averiecooks.py` & `recipe_scrapers-9.2.6/recipe_scrapers/averiecooks.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/bbcfood.py` & `recipe_scrapers-9.2.6/recipe_scrapers/bbcfood.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from ._abstract import AbstractScraper
 from ._utils import get_minutes, normalize_string, get_yields
 
 
 class BBCFood(AbstractScraper):
     @classmethod
     def host(self, domain="com"):
-        return "bbc.{}".format(domain)
+        return f"bbc.{domain}"
 
     def title(self):
         return normalize_string(self.soup.find("h1").get_text())
 
     def total_time(self):
         return sum(
             [
```

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/bbcgoodfood.py` & `recipe_scrapers-9.2.6/recipe_scrapers/bbcgoodfood.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/bettycrocker.py` & `recipe_scrapers-9.2.6/recipe_scrapers/bettycrocker.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/bowlofdelicious.py` & `recipe_scrapers-9.2.6/recipe_scrapers/bowlofdelicious.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/budgetbytes.py` & `recipe_scrapers-9.2.6/recipe_scrapers/budgetbytes.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/chefkoch.py` & `recipe_scrapers-9.2.6/recipe_scrapers/chefkoch.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/closetcooking.py` & `recipe_scrapers-9.2.6/recipe_scrapers/closetcooking.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/cookieandkate.py` & `recipe_scrapers-9.2.6/recipe_scrapers/cookieandkate.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/cookpad.py` & `recipe_scrapers-9.2.6/recipe_scrapers/cookpad.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/cookstr.py` & `recipe_scrapers-9.2.6/recipe_scrapers/cookstr.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/copykat.py` & `recipe_scrapers-9.2.6/recipe_scrapers/copykat.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/countryliving.py` & `recipe_scrapers-9.2.6/recipe_scrapers/countryliving.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/cybercook.py` & `recipe_scrapers-9.2.6/recipe_scrapers/cybercook.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/delish.py` & `recipe_scrapers-9.2.6/recipe_scrapers/delish.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/eatsmarter.py` & `recipe_scrapers-9.2.6/recipe_scrapers/eatsmarter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ._abstract import AbstractScraper
 
 
 class Eatsmarter(AbstractScraper):
     @classmethod
     def host(self, domain="com"):
-        return "eatsmarter.%s" % domain
+        return f"eatsmarter.{domain}"
 
     def title(self):
         return self.schema.title()
 
     def total_time(self):
         return self.schema.total_time()
```

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/epicurious.py` & `recipe_scrapers-9.2.6/recipe_scrapers/greatbritishchefs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,76 @@
+# GreatBritishChefs.com scraper
+# Written by G.D. Wallters
+# Freely released the code to recipe_scraper group
+# 6 February, 2020
+# =======================================================
 from ._abstract import AbstractScraper
-from ._utils import normalize_string, get_yields
+from ._utils import get_minutes, normalize_string
 
 
-class Epicurious(AbstractScraper):
+class GreatBritishChefs(AbstractScraper):
     @classmethod
     def host(cls):
-        return "epicurious.com"
+        return "greatbritishchefs.com"
 
     def title(self):
-        return self.soup.find("h1", {"itemprop": "name"}).get_text()
+        return normalize_string(self.soup.find("h1").get_text())
 
     def total_time(self):
-        return 0
+        total_time = 0
+        tt1 = self.soup.find("span", {"class": "RecipeAttributes__Time"})
+        if tt1:
+            tt = tt1.find("span", {"class": "header-attribute-text"}).get_text()
+            tt3 = normalize_string(tt)
+            tt2 = get_minutes(tt3)
+            if tt3 and (tt2 == 0):
+                total_time = tt3
+            else:
+                total_time = tt2
+        return total_time
 
     def yields(self):
-        return get_yields(self.soup.find("dd", {"itemprop": "recipeYield"}))
+        recipe_yield = self.soup.find("span", {"class": "RecipeAttributes__Serves"})
+        if recipe_yield:
+            yields = normalize_string(
+                recipe_yield.find("span", {"class": "header-attribute-text"}).get_text()
+            )
+            return yields
 
     def image(self):
-        image = self.soup.find("img", {"class": "photo", "srcset": True})
-        return image["srcset"] if image else None
+        image = self.soup.find("img", {"id": "head-media"}, "src")
+        if image:
+            src = image.get("src", None)
+            if "http:" in src:
+                return src
+            else:
+                src = "http:" + src
+        return src if image else None
 
     def ingredients(self):
-        ingredients = self.soup.findAll("li", {"itemprop": "ingredients"})
-
-        return [normalize_string(ingredient.get_text()) for ingredient in ingredients]
+        ingredientsOuter = self.soup.find(
+            "ul", {"class": "IngredientsList__ListContainer"}
+        )
+        ingGroup = []
+        ingredparts = ingredientsOuter.findAll("li")
+        for i in ingredparts:
+            x = normalize_string(i.get_text())
+            ingGroup.append(x)
+        return ingGroup
 
     def instructions(self):
-        instructions = self.soup.findAll("li", {"class": "preparation-step"})
+        instructions = self.soup.find("div", {"class": "Method__List MethodList"})
 
-        return "\n".join(
-            [normalize_string(instruction.get_text()) for instruction in instructions]
-        )
+        ins = instructions.findAll("div", {"class": "MethodList__StepText"})
+
+        return "\n".join([normalize_string(inst.text) for inst in ins])
 
     def ratings(self):
-        rating = self.soup.find("span", {"class": "rating"})
-        rating = rating.get_text().split("/")[0] if rating is not None else None
-        rating = float(rating) if rating is not None else None
-        return rating
-
-    def reviews(self):
-        import re
-
-        fork_rating_re = re.compile(r"/(\d)_forks.png")
-
-        reviews = self.soup.findAll("", {"class": "most-recent"})
-        ratings = [rev.find("img", {"class": "fork-rating"}) for rev in reviews]
-        temp = []
-        for rating in ratings:
-            if "src" in rating.attrs:
-                txt = rating.attrs["src"]
-            else:
-                txt = ""
-            rating = fork_rating_re.search(txt)
-            rating = rating.group(1) if rating is not None else "0"
-            rating = int(rating) if rating != "0" else None
-            temp.append(rating)
-        ratings = temp
-        review_texts = [rev.find("div", {"class": "review-text"}) for rev in reviews]
-        reviews = [
-            rev.get_text().strip("/ flag if inappropriate") for rev in review_texts
-        ]
-        result = [
-            {"review_text": review_text, "rating": rating_score}
-            for review_text, rating_score in zip(reviews, ratings)
-        ]
-        return result
+        # This site does not support ratings at this time
+        r1 = 0
+        return r1
+
+    def description(self):
+        d = normalize_string(
+            self.soup.find("div", {"class": "RecipeAbstract__Abstract"}).text
+        )
+        return d if d else None
```

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/fifteenspatulas.py` & `recipe_scrapers-9.2.6/recipe_scrapers/fifteenspatulas.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/finedininglovers.py` & `recipe_scrapers-9.2.6/recipe_scrapers/finedininglovers.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/fitmencook.py` & `recipe_scrapers-9.2.6/recipe_scrapers/fitmencook.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/food.py` & `recipe_scrapers-9.2.6/recipe_scrapers/food.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/foodnetwork.py` & `recipe_scrapers-9.2.6/recipe_scrapers/foodnetwork.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/foodrepublic.py` & `recipe_scrapers-9.2.6/recipe_scrapers/foodrepublic.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/geniuskitchen.py` & `recipe_scrapers-9.2.6/recipe_scrapers/geniuskitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/giallozafferano.py` & `recipe_scrapers-9.2.6/recipe_scrapers/giallozafferano.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/gimmesomeoven.py` & `recipe_scrapers-9.2.6/recipe_scrapers/gimmesomeoven.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/gonnawantseconds.py` & `recipe_scrapers-9.2.6/recipe_scrapers/gonnawantseconds.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/gousto.py` & `recipe_scrapers-9.2.6/recipe_scrapers/gousto.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/greatbritishchefs.py` & `recipe_scrapers-9.2.6/recipe_scrapers/twopeasandtheirpod.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,41 @@
-# GreatBritishChefs.com scraper
-# Written by G.D. Wallters
-# Freely released the code to recipe_scraper group
-# 6 February, 2020
-# =======================================================
 from ._abstract import AbstractScraper
-from ._utils import get_minutes, normalize_string
+from ._utils import get_minutes, normalize_string, get_yields
 
 
-class GreatBritishChefs(AbstractScraper):
+class TwoPeasAndTheirPod(AbstractScraper):
     @classmethod
     def host(cls):
-        return "greatbritishchefs.com"
+        return "twopeasandtheirpod.com"
 
     def title(self):
-        return normalize_string(self.soup.find("h1").get_text())
+        return self.soup.find("h2", {"class": "wprm-recipe-name"}).get_text()
 
     def total_time(self):
-        total_time = 0
-        tt1 = self.soup.find("span", {"class": "RecipeAttributes__Time"})
-        if tt1:
-            tt = tt1.find("span", {"class": "header-attribute-text"}).get_text()
-            tt3 = normalize_string(tt)
-            tt2 = get_minutes(tt3)
-            if tt3 and (tt2 == 0):
-                total_time = tt3
-            else:
-                total_time = tt2
-        return total_time
+        minutes = self.soup.select_one(".wprm-recipe-total_time").get_text()
+        unit = self.soup.select_one(".wprm-recipe-total_time-unit").get_text()
 
-    def yields(self):
-        recipe_yield = self.soup.find("span", {"class": "RecipeAttributes__Serves"})
-        if recipe_yield:
-            yields = normalize_string(
-                recipe_yield.find("span", {"class": "header-attribute-text"}).get_text()
-            )
-            return yields
+        return get_minutes("{} {}".format(minutes, unit))
 
-    def image(self):
-        image = self.soup.find("img", {"id": "head-media"}, "src")
-        if image:
-            src = image.get("src", None)
-            if "http:" in src:
-                return src
-            else:
-                src = "http:" + src
-        return src if image else None
+    def yields(self):
+        return get_yields(
+            self.soup.select_one(
+                "div.wprm-recipe-details-container dl:nth-of-type(5) dd"
+            ).get_text()
+        )
 
     def ingredients(self):
-        ingredientsOuter = self.soup.find(
-            "ul", {"class": "IngredientsList__ListContainer"}
-        )
-        ingGroup = []
-        ingredparts = ingredientsOuter.findAll("li")
-        for i in ingredparts:
-            x = normalize_string(i.get_text())
-            ingGroup.append(x)
-        return ingGroup
+        ingredients = self.soup.findAll("li", {"class": "wprm-recipe-ingredient"})
 
-    def instructions(self):
-        instructions = self.soup.find("div", {"class": "Method__List MethodList"})
+        return [normalize_string(ingredient.get_text()) for ingredient in ingredients]
 
-        ins = instructions.findAll("div", {"class": "MethodList__StepText"})
+    def instructions(self):
+        instructions = self.soup.select(".wprm-recipe-instruction-text")
 
-        return "\n".join([normalize_string(inst.text) for inst in ins])
+        return "\n".join(
+            [normalize_string(instruction.get_text()) for instruction in instructions]
+        )
 
-    def ratings(self):
-        # This site does not support ratings at this time
-        r1 = 0
-        return r1
+    def image(self):
+        image = self.soup.find("div", {"class": "wprm-recipe-image"}).find("img")
 
-    def description(self):
-        d = normalize_string(
-            self.soup.find("div", {"class": "RecipeAbstract__Abstract"}).text
-        )
-        return d if d else None
+        return image["src"] if image else None
```

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/halfbakedharvest.py` & `recipe_scrapers-9.2.6/recipe_scrapers/halfbakedharvest.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/hassenchef.py` & `recipe_scrapers-9.2.6/recipe_scrapers/hassenchef.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/heinzbrasil.py` & `recipe_scrapers-9.2.6/recipe_scrapers/heinzbrasil.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/hellofresh.py` & `recipe_scrapers-9.2.6/recipe_scrapers/hellofresh.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ._abstract import AbstractScraper
 from ._utils import get_minutes, normalize_string, get_yields
 
 
 class HelloFresh(AbstractScraper):
     @classmethod
     def host(self, domain="com"):
-        return "hellofresh.%s" % domain
+        return f"hellofresh.{domain}"
 
     def title(self):
         return self.soup.find("h1").get_text()
 
     def total_time(self):
         return get_minutes(
             self.soup.find(
@@ -21,15 +21,17 @@
         )
 
     def yields(self):
         return get_yields(
             self.soup.find(
                 "span",
                 {"data-translation-id": "recipe-detail.recipe-detail.serving-amount"},
-            ).parent.parent.find_all("button")[0]
+            )
+            .parent.parent.find("div", {"variant": "secondary"})
+            .contents[0]
         )
 
     def ingredients(self):
         ingredients_container = self.soup.find(
             "div", {"data-test-id": "recipeDetailFragment.ingredients"}
         )
 
@@ -37,15 +39,15 @@
 
         return [
             " ".join(
                 [
                     normalize_string(ingredient_first_part.get_text()),
                     normalize_string(ingredient_second_part.get_text()),
                 ]
-            )
+            ).strip()
             for ingredient_first_part, ingredient_second_part in zip(
                 ingredients[0::2], ingredients[1::2]
             )
         ]
 
     def instructions(self):
         instructions_regex = re.compile(r"recipeDetailFragment.instructions.step-(\d)")
```

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/hostthetoast.py` & `recipe_scrapers-9.2.6/recipe_scrapers/hostthetoast.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/hundredandonecookbooks.py` & `recipe_scrapers-9.2.6/recipe_scrapers/hundredandonecookbooks.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/ig.py` & `recipe_scrapers-9.2.6/recipe_scrapers/ig.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/inspiralized.py` & `recipe_scrapers-9.2.6/recipe_scrapers/inspiralized.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/jamieoliver.py` & `recipe_scrapers-9.2.6/recipe_scrapers/jamieoliver.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/justbento.py` & `recipe_scrapers-9.2.6/recipe_scrapers/justbento.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/kennymcgovern.py` & `recipe_scrapers-9.2.6/recipe_scrapers/kennymcgovern.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/kochbar.py` & `recipe_scrapers-9.2.6/recipe_scrapers/kochbar.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/lecremedelacrumb.py` & `recipe_scrapers-9.2.6/recipe_scrapers/lecremedelacrumb.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/livelytable.py` & `recipe_scrapers-9.2.6/recipe_scrapers/livelytable.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/lovingitvegan.py` & `recipe_scrapers-9.2.6/recipe_scrapers/lovingitvegan.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/marmiton.py` & `recipe_scrapers-9.2.6/recipe_scrapers/marmiton.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/matprat.py` & `recipe_scrapers-9.2.6/recipe_scrapers/matprat.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/mindmegette.py` & `recipe_scrapers-9.2.6/recipe_scrapers/mindmegette.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     def image(self):
         image_relative_url = self.soup.find("img", {"itemprop": "photo", "src": True})[
             "src"
         ]
 
         if image_relative_url is not None:
-            image_relative_url = "http://%s%s" % (self.host(), image_relative_url)
+            image_relative_url = f"http://{self.host()}{image_relative_url}"
 
         return image_relative_url
 
     def ingredients(self):
         ingredients_html = self.soup.findAll("li", {"itemprop": "ingredient"})
 
         return [
```

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/minimalistbaker.py` & `recipe_scrapers-9.2.6/recipe_scrapers/minimalistbaker.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/misya.py` & `recipe_scrapers-9.2.6/recipe_scrapers/misya.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/momswithcrockpots.py` & `recipe_scrapers-9.2.6/recipe_scrapers/momswithcrockpots.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/motherthyme.py` & `recipe_scrapers-9.2.6/recipe_scrapers/motherthyme.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/mybakingaddiction.py` & `recipe_scrapers-9.2.6/recipe_scrapers/mybakingaddiction.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/myrecipes.py` & `recipe_scrapers-9.2.6/recipe_scrapers/myrecipes.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/nihhealthyeating.py` & `recipe_scrapers-9.2.6/recipe_scrapers/nihhealthyeating.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/nourishedbynutrition.py` & `recipe_scrapers-9.2.6/recipe_scrapers/nourishedbynutrition.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/nutritionbynathalie.py` & `recipe_scrapers-9.2.6/recipe_scrapers/nutritionbynathalie.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/nytimes.py` & `recipe_scrapers-9.2.6/recipe_scrapers/nytimes.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/ohsheglows.py` & `recipe_scrapers-9.2.6/recipe_scrapers/ohsheglows.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/panelinha.py` & `recipe_scrapers-9.2.6/recipe_scrapers/panelinha.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/paninihappy.py` & `recipe_scrapers-9.2.6/recipe_scrapers/paninihappy.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/przepisy.py` & `recipe_scrapers-9.2.6/recipe_scrapers/przepisy.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/purelypope.py` & `recipe_scrapers-9.2.6/recipe_scrapers/purelypope.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/realsimple.py` & `recipe_scrapers-9.2.6/recipe_scrapers/realsimple.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/seriouseats.py` & `recipe_scrapers-9.2.6/recipe_scrapers/seriouseats.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/simplyquinoa.py` & `recipe_scrapers-9.2.6/recipe_scrapers/simplyquinoa.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/simplyrecipes.py` & `recipe_scrapers-9.2.6/recipe_scrapers/simplyrecipes.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/skinnytaste.py` & `recipe_scrapers-9.2.6/recipe_scrapers/skinnytaste.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/southernliving.py` & `recipe_scrapers-9.2.6/recipe_scrapers/southernliving.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/spendwithpennies.py` & `recipe_scrapers-9.2.6/recipe_scrapers/spendwithpennies.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/steamykitchen.py` & `recipe_scrapers-9.2.6/recipe_scrapers/steamykitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/tasteofhome.py` & `recipe_scrapers-9.2.6/recipe_scrapers/tasteofhome.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/tastesoflizzyt.py` & `recipe_scrapers-9.2.6/recipe_scrapers/tastesoflizzyt.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/tasty.py` & `recipe_scrapers-9.2.6/recipe_scrapers/tasty.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/tastykitchen.py` & `recipe_scrapers-9.2.6/recipe_scrapers/tastykitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/thehappyfoodie.py` & `recipe_scrapers-9.2.6/recipe_scrapers/thehappyfoodie.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/thekitchn.py` & `recipe_scrapers-9.2.6/recipe_scrapers/thekitchn.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/thenutritiouskitchen.py` & `recipe_scrapers-9.2.6/recipe_scrapers/thenutritiouskitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/thepioneerwoman.py` & `recipe_scrapers-9.2.6/recipe_scrapers/thepioneerwoman.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/thespruceeats.py` & `recipe_scrapers-9.2.6/recipe_scrapers/thespruceeats.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/thevintagemixer.py` & `recipe_scrapers-9.2.6/recipe_scrapers/thevintagemixer.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/thewoksoflife.py` & `recipe_scrapers-9.2.6/recipe_scrapers/thewoksoflife.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/tineno.py` & `recipe_scrapers-9.2.6/recipe_scrapers/tineno.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/tudogostoso.py` & `recipe_scrapers-9.2.6/recipe_scrapers/tudogostoso.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/twopeasandtheirpod.py` & `recipe_scrapers-9.2.6/recipe_scrapers/vegolosi.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,67 @@
 from ._abstract import AbstractScraper
 from ._utils import get_minutes, normalize_string, get_yields
 
 
-class TwoPeasAndTheirPod(AbstractScraper):
+class Vegolosi(AbstractScraper):
     @classmethod
     def host(cls):
-        return "twopeasandtheirpod.com"
+        return "vegolosi.it"
 
     def title(self):
-        return self.soup.find("h2", {"class": "wprm-recipe-name"}).get_text()
+        return self.soup.find("h1").get_text().strip()
+
+    def preparation_time(self):
+        possible_time_info_elements = self.soup.findAll(
+            "span", {"class": "tasty-recipes-prep-time"}
+        )
+
+        return sum([get_minutes(element) for element in possible_time_info_elements])
+
+    def cooking_time(self):
+        possible_time_info_elements = self.soup.findAll(
+            "span", {"class": "tasty-recipes-cook-time"}
+        )
+
+        return sum([get_minutes(element) for element in possible_time_info_elements])
 
     def total_time(self):
-        minutes = self.soup.select_one(".wprm-recipe-total_time").get_text()
-        unit = self.soup.select_one(".wprm-recipe-total_time-unit").get_text()
+        possible_time_info_elements = self.soup.findAll(
+            "span", {"class": "tasty-recipes-total-time"}
+        )
 
-        return get_minutes("{} {}".format(minutes, unit))
+        return sum([get_minutes(element) for element in possible_time_info_elements])
 
     def yields(self):
-        return get_yields(
-            self.soup.select_one(
-                "div.wprm-recipe-details-container dl:nth-of-type(5) dd"
-            ).get_text()
+        possible_yields_info_elements = self.soup.findAll(
+            "span", {"class": "tasty-recipes-yield"}
         )
+        for element in possible_yields_info_elements:
+            if "persone" in element.get_text():
+                return get_yields(element)
+        return ""
 
     def ingredients(self):
-        ingredients = self.soup.findAll("li", {"class": "wprm-recipe-ingredient"})
+        ingredients = self.soup.select(".tasty-recipe-ingredients > ul > li")
+
+        if not ingredients:
+            ingredients = self.soup.findAll("li", {"class": "ingredient"})
 
         return [normalize_string(ingredient.get_text()) for ingredient in ingredients]
 
     def instructions(self):
-        instructions = self.soup.select(".wprm-recipe-instruction-text")
+
+        instructions = self.soup.findAll("div", {"class": "tasty-recipe-instructions"})
 
         return "\n".join(
             [normalize_string(instruction.get_text()) for instruction in instructions]
         )
 
-    def image(self):
-        image = self.soup.find("div", {"class": "wprm-recipe-image"}).find("img")
-
-        return image["src"] if image else None
+    def ratings(self):
+        return round(
+            float(
+                self.soup.find("div", {"class": "tasty-recipe-rating rating_panel"})
+                .get("data-content-rate")
+                .replace(",", ".")
+            ),
+            2,
+        )
```

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/vegolosi.py` & `recipe_scrapers-9.2.6/recipe_scrapers/epicurious.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,59 @@
 from ._abstract import AbstractScraper
-from ._utils import get_minutes, normalize_string, get_yields
+from ._utils import normalize_string, get_yields
 
 
-class Vegolosi(AbstractScraper):
+class Epicurious(AbstractScraper):
     @classmethod
     def host(cls):
-        return "vegolosi.it"
+        return "epicurious.com"
 
     def title(self):
-        return self.soup.find("h1").get_text().strip()
-
-    def preparation_time(self):
-        possible_time_info_elements = self.soup.findAll(
-            "span", {"class": "tasty-recipes-prep-time"}
-        )
-
-        return sum([get_minutes(element) for element in possible_time_info_elements])
-
-    def cooking_time(self):
-        possible_time_info_elements = self.soup.findAll(
-            "span", {"class": "tasty-recipes-cook-time"}
-        )
-
-        return sum([get_minutes(element) for element in possible_time_info_elements])
+        return normalize_string(self.soup.find("h1", {"itemprop": "name"}).get_text())
 
     def total_time(self):
-        possible_time_info_elements = self.soup.findAll(
-            "span", {"class": "tasty-recipes-total-time"}
-        )
-
-        return sum([get_minutes(element) for element in possible_time_info_elements])
+        return 0
 
     def yields(self):
-        possible_yields_info_elements = self.soup.findAll(
-            "span", {"class": "tasty-recipes-yield"}
-        )
-        for element in possible_yields_info_elements:
-            if "persone" in element.get_text():
-                return get_yields(element)
-        return ""
+        return get_yields(self.soup.find("dd", {"itemprop": "recipeYield"}))
 
-    def ingredients(self):
-        ingredients = self.soup.select(".tasty-recipe-ingredients > ul > li")
+    def image(self):
+        image = self.soup.find("img", {"class": "photo", "srcset": True})
+        return image["srcset"] if image else None
 
-        if not ingredients:
-            ingredients = self.soup.findAll("li", {"class": "ingredient"})
+    def ingredients(self):
+        ingredients = self.soup.findAll("li", {"itemprop": "ingredients"})
 
         return [normalize_string(ingredient.get_text()) for ingredient in ingredients]
 
     def instructions(self):
-
-        instructions = self.soup.findAll("div", {"class": "tasty-recipe-instructions"})
+        instructions = self.soup.findAll("li", {"class": "preparation-step"})
 
         return "\n".join(
             [normalize_string(instruction.get_text()) for instruction in instructions]
         )
 
     def ratings(self):
-        return round(
-            float(
-                self.soup.find("div", {"class": "tasty-recipe-rating rating_panel"})
-                .get("data-content-rate")
-                .replace(",", ".")
-            ),
-            2,
-        )
+        rating = self.soup.find("span", {"class": "rating"})
+        rating = rating.get_text().split("/")[0] if rating is not None else None
+        rating = float(rating) if rating is not None else None
+        return rating
+
+    def reviews(self):
+        result = []
+        reviews = self.soup.find("div", {"class": "reviews"})
+        if len(reviews.find_all("li")):
+            for li in reviews.find_all("li"):
+                rating = li.find("img", {"class": "fork-rating"})
+                try:
+                    rating_value = int(rating.get("src").split("_forks.png")[0][-1])
+                except Exception:
+                    rating_value = 0
+
+                result.append(
+                    {
+                        "review_text": normalize_string(li.find("p").get_text()),
+                        "rating": rating_value,
+                    }
+                )
+
+        return result
```

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/watchwhatueat.py` & `recipe_scrapers-9.2.6/recipe_scrapers/watchwhatueat.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/whatsgabycooking.py` & `recipe_scrapers-9.2.6/recipe_scrapers/whatsgabycooking.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/wikicookbook.py` & `recipe_scrapers-9.2.6/recipe_scrapers/wikicookbook.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers/yummly.py` & `recipe_scrapers-9.2.6/recipe_scrapers/yummly.py`

 * *Files identical despite different names*

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers.egg-info/PKG-INFO` & `recipe_scrapers-9.2.6/recipe_scrapers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: recipe-scrapers
-Version: 9.2.5
+Version: 9.2.6
 Summary: Python package, scraping recipes from all over the internet
 Home-page: https://github.com/hhursev/recipe-scrapers/
 Author: Hristo Harsev
 Author-email: r+pypi@hharsev.com
 License: UNKNOWN
 Description: .. image:: https://img.shields.io/pypi/v/recipe-scrapers.svg?
             :target: https://pypi.org/project/recipe-scrapers/
@@ -76,14 +76,15 @@
         - `https://cookstr.com/ <https://cookstr.com>`_
         - `https://copykat.com/ <https://copykat.com>`_
         - `https://countryliving.com/ <https://countryliving.com>`_
         - `https://cybercook.com.br/ <https://cybercook.com.br/>`_
         - `https://delish.com/ <https://delish.com>`_
         - `https://eatsmarter.com/ <https://eatsmarter.com/>`_
         - `https://eatsmarter.de/ <https://eatsmarter.de/>`_
+        - `https://eatwhattonight.com/ <https://eatwhattonight.com/>`_
         - `https://epicurious.com/ <https://epicurious.com>`_
         - `https://fifteenspatulas.com/ <https://www.fifteenspatulas.com/>`_
         - `https://finedininglovers.com/ <https://www.finedininglovers.com>`_
         - `https://fitmencook.com/ <https://www.fitmencook.com>`_
         - `https://food.com/ <https://www.food.com>`_
         - `https://foodnetwork.com/ <https://www.foodnetwork.com>`_
         - `https://foodrepublic.com/ <https://foodrepublic.com>`_
```

### Comparing `recipe_scrapers-9.2.5/recipe_scrapers.egg-info/SOURCES.txt` & `recipe_scrapers-9.2.6/recipe_scrapers.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 recipe_scrapers/cookpad.py
 recipe_scrapers/cookstr.py
 recipe_scrapers/copykat.py
 recipe_scrapers/countryliving.py
 recipe_scrapers/cybercook.py
 recipe_scrapers/delish.py
 recipe_scrapers/eatsmarter.py
+recipe_scrapers/eatwhattonight.py
 recipe_scrapers/epicurious.py
 recipe_scrapers/fifteenspatulas.py
 recipe_scrapers/finedininglovers.py
 recipe_scrapers/fitmencook.py
 recipe_scrapers/food.py
 recipe_scrapers/foodnetwork.py
 recipe_scrapers/foodrepublic.py
```

### Comparing `recipe_scrapers-9.2.5/setup.py` & `recipe_scrapers-9.2.6/setup.py`

 * *Files identical despite different names*

