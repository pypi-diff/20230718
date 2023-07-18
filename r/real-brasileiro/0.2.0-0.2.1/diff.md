# Comparing `tmp/real_brasileiro-0.2.0.tar.gz` & `tmp/real-brasileiro-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "real_brasileiro-0.2.0.tar", last modified: Sat Oct 15 00:43:54 2022, max compression
+gzip compressed data, was "real-brasileiro-0.2.1.tar", last modified: Tue Jul 18 03:46:00 2023, max compression
```

## Comparing `real_brasileiro-0.2.0.tar` & `real-brasileiro-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,11 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2022-10-15 00:43:54.560620 real_brasileiro-0.2.0/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2064 2022-10-15 00:36:37.000000 real_brasileiro-0.2.0/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1304 2022-10-15 00:43:54.560620 real_brasileiro-0.2.0/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      892 2022-10-15 00:36:48.000000 real_brasileiro-0.2.0/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2022-10-15 00:43:54.560620 real_brasileiro-0.2.0/real_br/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       30 2022-10-15 00:36:45.000000 real_brasileiro-0.2.0/real_br/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4478 2022-10-15 00:36:12.000000 real_brasileiro-0.2.0/real_br/real_br.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2022-10-15 00:43:54.560620 real_brasileiro-0.2.0/real_brasileiro.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1304 2022-10-15 00:43:54.000000 real_brasileiro-0.2.0/real_brasileiro.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      221 2022-10-15 00:43:54.000000 real_brasileiro-0.2.0/real_brasileiro.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2022-10-15 00:43:54.000000 real_brasileiro-0.2.0/real_brasileiro.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2022-10-15 00:43:54.000000 real_brasileiro-0.2.0/real_brasileiro.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2022-10-15 00:43:54.560620 real_brasileiro-0.2.0/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      605 2022-10-15 00:40:40.000000 real_brasileiro-0.2.0/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-18 03:46:00.523476 real-brasileiro-0.2.1/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1073 2023-07-18 03:36:07.000000 real-brasileiro-0.2.1/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1270 2023-07-18 03:46:00.523476 real-brasileiro-0.2.1/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      966 2023-07-18 03:42:42.000000 real-brasileiro-0.2.1/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-18 03:46:00.523476 real-brasileiro-0.2.1/real_brasileiro.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1270 2023-07-18 03:46:00.000000 real-brasileiro-0.2.1/real_brasileiro.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      182 2023-07-18 03:46:00.000000 real-brasileiro-0.2.1/real_brasileiro.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-07-18 03:46:00.000000 real-brasileiro-0.2.1/real_brasileiro.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-07-18 03:46:00.000000 real-brasileiro-0.2.1/real_brasileiro.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-07-18 03:46:00.523476 real-brasileiro-0.2.1/setup.cfg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      377 2023-07-18 03:45:16.000000 real-brasileiro-0.2.1/setup.py
```

### Comparing `real_brasileiro-0.2.0/PKG-INFO` & `real-brasileiro-0.2.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,73 @@
 Metadata-Version: 2.1
-Name: real_brasileiro
-Version: 0.2.0
-Summary: Classe para formatar valores para o formato de Real Brasileiro
-Home-page: UNKNOWN
-Author: Daniel Mendonca
-Author-email: heromon.9010@gmai.com
-License: MIT License
-Keywords: Dinheiro,dinheiro brasileiro,reias,Dinheiro em reais,Real_brasileiro,Real brasileiro,R$
+Name: real-brasileiro
+Version: 0.2.1
+Summary: UNKNOWN
+Home-page: https://github.com/MikalROn/Real_br
+Author: Daniel Coêlho
+Author-email: heromon.9010@gmail.com
+License: UNKNOWN
 Platform: UNKNOWN
+Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Real brasileiro
 
 > Status do projeto: Em desenvolvimento
 
 este projeto tem como objetivo me ajudar na formatação, sanitização e apresentação dos valores com os quais eu diariamente trabalho.
+## Download
 
-## Entradas
+```shell
+$pip install real-brasileiro
 ```
+
+## Entradas
+```python
 from real_br import Real
 
 print(Real(10.10),
     Real(10),
     Real('R$ 100,55'))
 
 ```
 > Nos testes você consegue conferir melhor em quais formatos a classe aceita os valores.
 
 
 ## Criando objeto
 
-```
+```python
 from real_br import Real
 
 valor = 10
 real = Real(valor)
 print(real)
 
 ```
 
 > você também pode obter o equivalente em centavos usando
 
-```
+```python
 from real_br import Real
 
 valor = 10
 real = Real(valor)
 print(real.centavos)
 
 ```
 > A classe retorna float, str e int (int é retornado em centavos)
 
-```
+```python
 from real_br import Real
 
 valor = 10
 real = Real(valor)
 print(float(real),  int(real), str(real))
 
 ```
 # A classe possui 100% de cobertura de testes
-````commandline
+````shell
 pytest -cov
 ````
 
+
```

### Comparing `real_brasileiro-0.2.0/README.md` & `real-brasileiro-0.2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,58 @@
 # Real brasileiro
 
 > Status do projeto: Em desenvolvimento
 
 este projeto tem como objetivo me ajudar na formatação, sanitização e apresentação dos valores com os quais eu diariamente trabalho.
+## Download
 
-## Entradas
+```shell
+$pip install real-brasileiro
 ```
+
+## Entradas
+```python
 from real_br import Real
 
 print(Real(10.10),
     Real(10),
     Real('R$ 100,55'))
 
 ```
 > Nos testes você consegue conferir melhor em quais formatos a classe aceita os valores.
 
 
 ## Criando objeto
 
-```
+```python
 from real_br import Real
 
 valor = 10
 real = Real(valor)
 print(real)
 
 ```
 
 > você também pode obter o equivalente em centavos usando
 
-```
+```python
 from real_br import Real
 
 valor = 10
 real = Real(valor)
 print(real.centavos)
 
 ```
 > A classe retorna float, str e int (int é retornado em centavos)
 
-```
+```python
 from real_br import Real
 
 valor = 10
 real = Real(valor)
 print(float(real),  int(real), str(real))
 
 ```
 # A classe possui 100% de cobertura de testes
-````commandline
+````shell
 pytest -cov
-````
+````
```

### Comparing `real_brasileiro-0.2.0/real_brasileiro.egg-info/PKG-INFO` & `real-brasileiro-0.2.1/real_brasileiro.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,73 @@
 Metadata-Version: 2.1
 Name: real-brasileiro
-Version: 0.2.0
-Summary: Classe para formatar valores para o formato de Real Brasileiro
-Home-page: UNKNOWN
-Author: Daniel Mendonca
-Author-email: heromon.9010@gmai.com
-License: MIT License
-Keywords: Dinheiro,dinheiro brasileiro,reias,Dinheiro em reais,Real_brasileiro,Real brasileiro,R$
+Version: 0.2.1
+Summary: UNKNOWN
+Home-page: https://github.com/MikalROn/Real_br
+Author: Daniel Coêlho
+Author-email: heromon.9010@gmail.com
+License: UNKNOWN
 Platform: UNKNOWN
+Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Real brasileiro
 
 > Status do projeto: Em desenvolvimento
 
 este projeto tem como objetivo me ajudar na formatação, sanitização e apresentação dos valores com os quais eu diariamente trabalho.
+## Download
 
-## Entradas
+```shell
+$pip install real-brasileiro
 ```
+
+## Entradas
+```python
 from real_br import Real
 
 print(Real(10.10),
     Real(10),
     Real('R$ 100,55'))
 
 ```
 > Nos testes você consegue conferir melhor em quais formatos a classe aceita os valores.
 
 
 ## Criando objeto
 
-```
+```python
 from real_br import Real
 
 valor = 10
 real = Real(valor)
 print(real)
 
 ```
 
 > você também pode obter o equivalente em centavos usando
 
-```
+```python
 from real_br import Real
 
 valor = 10
 real = Real(valor)
 print(real.centavos)
 
 ```
 > A classe retorna float, str e int (int é retornado em centavos)
 
-```
+```python
 from real_br import Real
 
 valor = 10
 real = Real(valor)
 print(float(real),  int(real), str(real))
 
 ```
 # A classe possui 100% de cobertura de testes
-````commandline
+````shell
 pytest -cov
 ````
 
+
```

