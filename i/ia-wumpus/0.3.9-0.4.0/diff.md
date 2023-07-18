# Comparing `tmp/ia_wumpus-0.3.9.tar.gz` & `tmp/ia_wumpus-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ia_wumpus-0.3.9.tar", max compression
+gzip compressed data, was "ia_wumpus-0.4.0.tar", max compression
```

## Comparing `ia_wumpus-0.3.9.tar` & `ia_wumpus-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.3.9/LICENSE
--rw-r--r--   0        0        0     4260 2023-05-31 03:35:24.780713 ia_wumpus-0.3.9/README.md
--rw-r--r--   0        0        0      636 2023-05-29 00:49:09.138275 ia_wumpus-0.3.9/ia_wumpus/__init__.py
--rw-r--r--   0        0        0     8670 2023-06-08 03:02:20.786412 ia_wumpus-0.3.9/ia_wumpus/agente_reativo_v1.py
--rw-r--r--   0        0        0     8960 2023-05-29 00:49:09.162276 ia_wumpus-0.3.9/ia_wumpus/ambiente.py
--rw-r--r--   0        0        0     1355 2023-05-27 02:48:23.434838 ia_wumpus-0.3.9/ia_wumpus/dinamica_agente_ambiente.py
--rw-r--r--   0        0        0      513 2023-06-08 23:06:42.508627 ia_wumpus-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     4902 1970-01-01 00:00:00.000000 ia_wumpus-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4251 2023-07-17 00:04:08.021968 ia_wumpus-0.4.0/README.md
+-rw-r--r--   0        0        0      698 2023-07-17 18:55:44.260943 ia_wumpus-0.4.0/ia_wumpus/__init__.py
+-rw-r--r--   0        0        0     8672 2023-07-17 00:04:13.510295 ia_wumpus-0.4.0/ia_wumpus/agente_reativo_v1.py
+-rw-r--r--   0        0        0    11787 2023-07-18 02:56:54.145582 ia_wumpus-0.4.0/ia_wumpus/agente_reativo_v2.py
+-rw-r--r--   0        0        0     9080 2023-07-18 16:11:35.250199 ia_wumpus-0.4.0/ia_wumpus/ambiente.py
+-rw-r--r--   0        0        0     1355 2023-07-17 00:04:13.682305 ia_wumpus-0.4.0/ia_wumpus/dinamica_agente_ambiente.py
+-rw-r--r--   0        0        0      553 2023-07-18 21:21:16.823177 ia_wumpus-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4975 1970-01-01 00:00:00.000000 ia_wumpus-0.4.0/PKG-INFO
```

### Comparing `ia_wumpus-0.3.9/LICENSE` & `ia_wumpus-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.9/README.md` & `ia_wumpus-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ### [Documentação ia-wumpus](https://oseiasdfarias.github.io/IA_mundo_do_wumpus/)
 
 <br>
 
 # Versões do Projeto
 
-<img src="https://raw.githubusercontent.com/Oseiasdfarias/IA_mundo_do_wumpus/340951a7d59c7ce6e3c981455b77638781b23d52/docs/static/img/code_demo.svg" alt="Ambiente Mundo do Wumpus." style="width:900px">
+<img src="https://raw.githubusercontent.com/Oseiasdfarias/IA_mundo_do_wumpus/318cc41584c60d36a122f6ff15271d52a8fb9be7/utils/code_demo2.svg" alt="Ambiente Mundo do Wumpus." style="width:900px">
 
 <br>
 
 ## [Link Versão 00](https://github.com/Oseiasdfarias/IA_mundo_do_wumpus/tree/versao_0)
 
 **Etapa 1 - Gerador Aleatório de Ambientes do Mundo do Wumpus.**
```

### Comparing `ia_wumpus-0.3.9/ia_wumpus/__init__.py` & `ia_wumpus-0.4.0/ia_wumpus/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,10 +13,11 @@
 #            Oséias Farias
 #
 # Data: Maio - 2023
 #  ----------------------------------------------------
 
 from .ambiente import Ambiente                   # noqa: F401
 from .agente_reativo_v1 import AgenteReativoV1   # noqa: F401
+from .agente_reativo_v2 import AgenteReativoV2   # noqa: F401
 
 
 __version__ = "0.3.6"
```

### Comparing `ia_wumpus-0.3.9/ia_wumpus/agente_reativo_v1.py` & `ia_wumpus-0.4.0/ia_wumpus/agente_reativo_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         self.get_opcoes_mov()
         if self.__sentir_fedor() and self.bala:
             self.bala = False
             pos_tiro = self.sortear_pos(self.__list_opc_mov_ag)
             pos_wumpus = self.amb.get_pos_objetos()["wumpus"]
             for i in pos_wumpus:
                 if i == pos_tiro:
-                    console.print("[INFO] Tiro e matou o Wumpos!",
+                    console.print("[INFO] Atirou e matou o Wumpos!",
                                   style="green")
                     return
             console.print("[DANG] Errou o tiro!",
                           style="danger")
 
     def verificar_vitorio(self) -> bool:
         if self.pegou_ouro:
```

### Comparing `ia_wumpus-0.3.9/ia_wumpus/ambiente.py` & `ia_wumpus-0.4.0/ia_wumpus/ambiente.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,27 +45,30 @@
                  t_pausa: float = 0.0) -> None:
         self.clear()
         self.t_pausa = t_pausa
         if dimensao_ambiente < 3:
             self.dimensao_ambiente = 3
         else:
             self.dimensao_ambiente = dimensao_ambiente
+
         self.pocos = self.dimensao_ambiente
+
         self.wumpus = wumpus
         self.ouro = ouro
         self.dimensoes = (self.dimensao_ambiente,
                           self.dimensao_ambiente)
 
         self.__mundo = np.zeros(self.dimensoes, dtype=int)
         self.__mundo[:] = 0
 
         # Percepções dos Objetos no Ambiente.
         self.__pos_percepcoes: dict = {"brisa":  [],
                                        "fedor":  [],
-                                       "brilho": []}
+                                       "brilho": [],
+                                       "ouro": []}
         # Posições dos Objetos no Ambiente.
         self.__pos_objetos: dict = {"pocos":  [],
                                     "wumpus": [],
                                     "ouro":   [],
                                     "agente": []}
 
         # Posicionando o Agente no ambiente.
@@ -168,14 +171,15 @@
 
     def __add_pos_ouro(self) -> None:
         """Posicionando o(s) Ouro(s) no Ambiente."""
         for i in range(self.ouro):
             pos_ouro = self.__add_pos_obj_map(3)
             self.__salvar_pos_objetos(objeto="ouro", pos_objeto=pos_ouro)
             self.__pos_percepcoes["brilho"].append((pos_ouro[1], pos_ouro[0]))
+            self.__add_percepcoes_obj(objeto="ouro", pos=pos_ouro)
 
     def __add_pos_agente(self) -> None:
         """Posicionando o(s) Agente(s) no Ambiente."""
         self.__mundo[(0, 0)] = 4
         self.__salvar_pos_objetos(objeto="agente", pos_objeto=(0, 0))
 
     @staticmethod
```

### Comparing `ia_wumpus-0.3.9/ia_wumpus/dinamica_agente_ambiente.py` & `ia_wumpus-0.4.0/ia_wumpus/dinamica_agente_ambiente.py`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.9/PKG-INFO` & `ia_wumpus-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: ia-wumpus
-Version: 0.3.9
+Version: 0.4.0
 Summary: Projeto O Mundo do Wumpus - Anbiente para estudo da disciplina de Inteligencia Computacional.
 Author: Oseiasdfarias
 Author-email: oseias.dfarias@gmail.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: numpy (>=1.24.3)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Description-Content-Type: text/markdown
 
 # Mundo do Wumpus - Intelegência Computacional
 
 Ambiente para estudo de modelos de Apredizagem de Máquina da disciplina de Inteligência Computacional.
 
@@ -25,15 +27,15 @@
 
 ### [Documentação ia-wumpus](https://oseiasdfarias.github.io/IA_mundo_do_wumpus/)
 
 <br>
 
 # Versões do Projeto
 
-<img src="https://raw.githubusercontent.com/Oseiasdfarias/IA_mundo_do_wumpus/340951a7d59c7ce6e3c981455b77638781b23d52/docs/static/img/code_demo.svg" alt="Ambiente Mundo do Wumpus." style="width:900px">
+<img src="https://raw.githubusercontent.com/Oseiasdfarias/IA_mundo_do_wumpus/318cc41584c60d36a122f6ff15271d52a8fb9be7/utils/code_demo2.svg" alt="Ambiente Mundo do Wumpus." style="width:900px">
 
 <br>
 
 ## [Link Versão 00](https://github.com/Oseiasdfarias/IA_mundo_do_wumpus/tree/versao_0)
 
 **Etapa 1 - Gerador Aleatório de Ambientes do Mundo do Wumpus.**
```

