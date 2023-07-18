# Comparing `tmp/rpa_cooperativa-1.0.63.tar.gz` & `tmp/rpa_cooperativa-1.0.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.63.tar", last modified: Thu Jul 13 17:08:14 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.64.tar", last modified: Tue Jul 18 13:24:54 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.63.tar` & `rpa_cooperativa-1.0.64.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 17:08:14.671725 rpa_cooperativa-1.0.63/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.63/LICENSE
--rw-rw-rw-   0        0        0     6969 2023-07-13 17:08:14.668413 rpa_cooperativa-1.0.63/PKG-INFO
--rw-rw-rw-   0        0        0     5824 2023-07-13 15:55:54.000000 rpa_cooperativa-1.0.63/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 17:08:14.445498 rpa_cooperativa-1.0.63/rpa_coop/
--rw-rw-rw-   0        0        0      585 2023-05-22 15:25:02.000000 rpa_cooperativa-1.0.63/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 17:08:14.626747 rpa_cooperativa-1.0.63/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.63/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.63/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.63/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.63/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.63/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.63/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.63/rpa_coop/img/siac_branco.PNG
--rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.63/rpa_coop/img/siat_amarelo.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.63/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.63/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.63/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0    91196 2023-07-13 17:04:43.000000 rpa_cooperativa-1.0.63/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-07-13 17:08:14.663415 rpa_cooperativa-1.0.63/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     6969 2023-07-13 17:08:13.000000 rpa_cooperativa-1.0.63/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-07-13 17:08:13.000000 rpa_cooperativa-1.0.63/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 17:08:13.000000 rpa_cooperativa-1.0.63/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-13 17:08:13.000000 rpa_cooperativa-1.0.63/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      581 2023-07-13 17:08:13.000000 rpa_cooperativa-1.0.63/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-13 17:08:13.000000 rpa_cooperativa-1.0.63/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 17:08:14.672725 rpa_cooperativa-1.0.63/setup.cfg
--rw-rw-rw-   0        0        0     2350 2023-07-13 16:50:58.000000 rpa_cooperativa-1.0.63/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:24:54.063764 rpa_cooperativa-1.0.64/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.64/LICENSE
+-rw-rw-rw-   0        0        0     6969 2023-07-18 13:24:54.060636 rpa_cooperativa-1.0.64/PKG-INFO
+-rw-rw-rw-   0        0        0     5824 2023-07-13 15:55:54.000000 rpa_cooperativa-1.0.64/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 13:24:53.876124 rpa_cooperativa-1.0.64/rpa_coop/
+-rw-rw-rw-   0        0        0      585 2023-05-22 15:25:02.000000 rpa_cooperativa-1.0.64/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:24:53.968459 rpa_cooperativa-1.0.64/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.64/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.64/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.64/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.64/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.64/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.64/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.64/rpa_coop/img/siac_branco.PNG
+-rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.64/rpa_coop/img/siat_amarelo.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.64/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.64/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.64/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0   101525 2023-07-18 13:22:44.000000 rpa_cooperativa-1.0.64/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:24:54.053000 rpa_cooperativa-1.0.64/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6969 2023-07-18 13:24:53.000000 rpa_cooperativa-1.0.64/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-07-18 13:24:53.000000 rpa_cooperativa-1.0.64/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 13:24:53.000000 rpa_cooperativa-1.0.64/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 13:24:53.000000 rpa_cooperativa-1.0.64/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      581 2023-07-18 13:24:53.000000 rpa_cooperativa-1.0.64/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-18 13:24:53.000000 rpa_cooperativa-1.0.64/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 13:24:54.064764 rpa_cooperativa-1.0.64/setup.cfg
+-rw-rw-rw-   0        0        0     2350 2023-07-18 12:25:45.000000 rpa_cooperativa-1.0.64/setup.py
```

### Comparing `rpa_cooperativa-1.0.63/LICENSE` & `rpa_cooperativa-1.0.64/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.63/PKG-INFO` & `rpa_cooperativa-1.0.64/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa_cooperativa
-Version: 1.0.63
+Version: 1.0.64
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.63/README.md` & `rpa_cooperativa-1.0.64/README.md`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.63/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.64/rpa_coop/__init__.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.63/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.64/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.63/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.64/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.63/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.64/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.63/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.64/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.63/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.64/rpa_coop/rpa_coop.py`

 * *Files 6% similar despite different names*

```diff
@@ -197,14 +197,20 @@
         
         self.ip_denodo = str(gerador_pwd('denodo_web', 'ip_host'))
         self.user_denodo = str(gerador_pwd('denodo_web', 'usuario'))
         self.pw_denodo = str(urllib.parse.quote_plus(gerador_pwd('denodo_web', 'senha')))
         
         self.token_api_denodo = str(gerador_pwd('token_api_denodo', 'senha'))
         self.url_api_denodo = str(gerador_pwd('token_api_denodo', 'ip_host'))
+        
+        self.user_plat_atend = str(gerador_pwd('contacorrente', 'usuario'))
+        self.senha_plat_atend = str(urllib.parse.quote_plus(gerador_pwd('contacorrente', 'senha')))
+        self.name_plat_atend = str(gerador_pwd('contacorrente', 'db_name'))
+        self.ip_plat_atend = str(gerador_pwd('contacorrente', 'ip_host'))
+        self.porta_plat_atend = str(gerador_pwd('contacorrente', 'porta'))
 
         
     def criar_engine(self, db:str, user_db='user_opcional', password_db='senha_opcional', ip_ou_host_db='ip_host_opcional', porta='3306', library_sql='mysqlconnector'):
         '''
         retorna conexao com db, db='parametro_obrigatorio' \n
         schema planinng: db = ('planning', 'fluid', 'cronos', 'controles_internos') \n
         schema sistema_senhas: db = 'sistema_senhas' \n
@@ -221,14 +227,17 @@
         elif (db == 'grafana'):
             conexao = create_engine(f'mysql+mysqlconnector://{self.user_grafana}:{self.pw_bd_grafana}@{self.ip_grafana}/{db}')
         elif (db == 'sistema_senhas'):
             banco = self.database_sistema_senhas
             conexao = create_engine(f'mysql+mysqlconnector://{self.user_sistema_senhas}:{self.pw_bd_sistema_senhas}@{self.ip_sistema_senhas}:3307/{banco}')
         elif (db == 'sapiens') or (db == 'sap') or (db == 'fiori'):
             conexao = create_engine(f"mssql+pymssql://{self.user_db_sapiens}:{self.pw_db_sapiens}@{self.ip_db_sapiens}")
+        elif (db == 'contacorrente'):
+            # plataforma de atendimento
+            conexao = create_engine(f'mysql+mysqlconnector://{self.user_plat_atend}:{self.senha_plat_atend}@{self.ip_plat_atend}/{self.name_plat_atend}', pool_recycle=3600)
         else:
             conexao = create_engine(f'mysql+{library_sql}://{user_db}:{password_db}@{ip_ou_host_db}:{porta}/{db}')
         return conexao
             
                          
     def criar_conexao(self, db:str, user_db='user_opcional', password_db='senha_opcional', ip_ou_host_db='ip_host_opcional', porta='3306', library_sql='mysqlconnector'):
         '''
@@ -248,14 +257,17 @@
         elif (db == 'grafana'):
             conexao = create_engine(f'mysql+mysqlconnector://{self.user_grafana}:{self.pw_bd_grafana}@{self.ip_grafana}/{db}')
         elif (db == 'sistema_senhas'):
             banco = self.database_sistema_senhas
             conexao = create_engine(f'mysql+mysqlconnector://{self.user_sistema_senhas}:{self.pw_bd_sistema_senhas}@{self.ip_sistema_senhas}:3307/{banco}')
         elif (db == 'sapiens') or (db == 'sap') or (db == 'fiori'):
             conexao = create_engine(f"mssql+pymssql://{self.user_db_sapiens}:{self.pw_db_sapiens}@{self.ip_db_sapiens}")
+        elif (db == 'contacorrente'):
+            # plataforma de atendimento
+            conexao = create_engine(f'mysql+mysqlconnector://{self.user_plat_atend}:{self.senha_plat_atend}@{self.ip_plat_atend}/{self.name_plat_atend}', pool_recycle=3600)
         else:
             conexao = create_engine(f'mysql+{library_sql}://{user_db}:{password_db}@{ip_ou_host_db}:{porta}/{db}')
         return conexao
             
         
     def api_consulta_denodo(self, database:str, tabela:str, colunas:str, filtro_where="opcional"):
         '''
@@ -1632,15 +1644,15 @@
             df = self.dados.consultar_banco_dados(self.conexao, f"SELECT * FROM rpa_fila WHERE status_rpa='{tipo_status}'")
         df = df[['cod_rpa', 'executar_na_vm', 'status_rpa']]
         print(df)
         print()
         return df
     
                           
-class Escrever_por_extenso:  
+class Escrever_por_extenso_old:  
             
     def __init__(self):
         self.url_api_escreve_por_extenso = str(gerador_pwd('por_extenso', 'senha'))
    
     
     def numero_por_extenso(self, valor:str):
         '''
@@ -1702,15 +1714,183 @@
             if 'VALOR NÃO SUPORTADO' in str(texto_e): texto_e = 'ZERO'
             res = requests.post(url, data={"Valor": f'{valor_d}', "Monetario": "Não"})
             texto_d =  res.json()['Valor'].upper()
             if 'VALOR NÃO SUPORTADO' in str(texto_d): texto_d = 'ZERO'
         taxa_extenso = texto_e + ' virgula ' + texto_d + ' por cento'    
         return taxa_extenso.upper()
         
-                     
+   
+class Escrever_por_extenso:  
+            
+    def __init__(self):
+        self.unidades = ['', 'um', 'dois', 'três', 'quatro', 'cinco', 'seis', 'sete', 'oito', 'nove']
+        self.especiais = ['dez', 'onze', 'doze', 'treze', 'catorze', 'quinze', 'dezesseis', 'dezessete', 'dezoito', 'dezenove']
+        self.dezenas = ['', '', 'vinte', 'trinta', 'quarenta', 'cinquenta', 'sessenta', 'setenta', 'oitenta', 'noventa']
+        self.centenas = ['', 'cento', 'duzentos', 'trezentos', 'quatrocentos', 'quinhentos', 'seiscentos', 'setecentos', 'oitocentos', 'novecentos']
+   
+    
+    def calc_3digitos(self, num: str):
+        C = ''   
+        num = int(num)             
+        num = str(num)
+        if int(len(num)) == 3:
+            if int(num[-3]) == 1 and int(num[-2:]) == 0: C = 'cem'
+            elif int(num[-3]) >= 1 and int(num[-2:]) == 0: C = self.centenas[int(num[-3])] 
+            elif int(num[-3]) >= 1 and int(num[-2]) == 0 and int(num[-1]) > 0: C = self.centenas[int(num[-3])] + ' e ' + self.unidades[int(num[-1])]
+            elif int(num[-3]) >= 1 and int(num[-2]) == 1 and int(num[-1]) >= 0: C = self.centenas[int(num[-3])] + ' e ' +  self.especiais[int(num[-1])]
+            elif int(num[-3]) >= 1 and int(num[-2]) > 0 and int(num[-1]) == 0: C = self.centenas[int(num[-3])] + ' e ' +  self.dezenas[int(num[-2])]
+            elif int(num[-3]) >= 1 and int(num[-2]) > 0 and int(num[-1]) > 0: C = self.centenas[int(num[-3])] + ' e ' +  self.dezenas[int(num[-2])] + ' e ' + self.unidades[int(num[-1])]  
+        elif int(len(num)) == 2:
+            if int(num[-2]) == 1: C = self.especiais[int(num[-1])]
+            elif int(num[-2]) > 1 and int(num[-1]) == 0: C = self.dezenas[int(num[-2])]
+            elif int(num[-2]) > 1 and int(num[-1]) > 0: C = self.dezenas[int(num[-2])] + ' e ' + self.unidades[int(num[-1])]   
+        else:
+            C = 'um' if int(num) == 1 else self.unidades[int(num)]
+        return C 
+
+
+    def taxa_por_extenso(self, taxa: float | str, nome_separador: str = 'virgula') -> str:
+        '''taxa_texto = taxa_por_extenso(128.09)\n
+            cento e vinte e oito virgula zero nove por cento
+        ''' 
+        if isinstance(taxa, float):
+            taxa = str(taxa).replace('.', ',')
+            if taxa[-2] == ',': taxa = taxa + '0'
+        else:
+            taxa = str(taxa).replace('.', ',').replace(' ', '')
+            if taxa[-2] == ',': taxa = taxa + '0'
+            
+        if ',' in taxa:
+            valor_aux = taxa.split(',')
+            valor_dir = valor_aux[0]
+            valor_esq = valor_aux[1]
+        else:
+            valor_dir = taxa
+            valor_esq = '0'
+    
+        if int(valor_dir) > 999: return 'erro, valor maximo 999,99 por cento'    
+        if int(valor_dir) > 0:
+            valor_dir_extenso = ''   
+            valor_dir_extenso = self.calc_3digitos(valor_dir)
+        else:
+            valor_dir_extenso = 'zero'
+            
+        if int(valor_esq) > 0:
+            valor_esq_extenso = ''
+            valor_esq_extenso = self.calc_3digitos(valor_esq)
+            if valor_esq[-2] == '0': valor_esq_extenso = 'zero ' + valor_esq_extenso
+            return valor_dir_extenso + ' ' + nome_separador + ' ' + valor_esq_extenso + ' por cento'
+        else:
+            return valor_dir_extenso + ' por cento'
+            
+                    
+    def numero_por_extenso(self, numero: float | str, monetario: bool = True, moeda_unit: str ='real', moeda_plural: str ='reais', nome_separador: str = 'virgula') -> str:
+        '''valor_texto = numero_por_extenso(100306000000.01)\n
+        cem bilhões e trezentos e seis milhões de reais e um centavo
+        '''
+        C , num , centavos, cents = '0', str(numero), '', ''
+        
+        def calc_centavos(cents: str):
+            if int(cents[-2]) == 0 and int(cents[-1]) > 0: D = self.unidades[int(cents[-1])]
+            elif int(cents[-2]) == 1 and int(cents[-1]) >= 0: D = self.especiais[int(cents[-1])]
+            elif int(cents[-2]) > 1 and int(cents[-1]) == 0: D = self.dezenas[int(cents[-2])] 
+            else: D = self.dezenas[int(cents[-2])] + ' e ' + self.unidades[int(cents[-1])]    
+            return D
+        
+        num = num.replace('.','').replace(',','.') if '.' in num and ',' in num else num.replace(',', '.')
+        if num == '0' or num == '0.0' or num == '0.00': return 'zero'
+        num_aux = num.split('.') if '.' in num else ''
+        num = str(num_aux[0]) if num_aux != '' else num
+        cents = str(num_aux[1]) if num_aux != '' else ''
+        cents = cents + '0' if int(len(cents)) < 2 else cents[:2]
+                
+        if cents != '' and cents != '0' and cents != '00':
+            centavos = calc_centavos(cents)
+            if monetario:
+                centavos = ' e ' + centavos + ' centavo' if cents == '01' else ' e ' + centavos + ' centavos'
+            else:
+                if cents[-2] == '0':
+                    centavos = ' ' + nome_separador + ' zero ' + centavos 
+                else:
+                    centavos = ' ' + nome_separador + ' ' + centavos 
+                
+        if not monetario:
+            moeda_unit = ''
+            moeda_plural = ''
+
+        # Começa a montar as strings de numero para texto  
+        if len(num) > 12:
+            print('valor numerico muito grande, nao suportado, max 999 bilhoes')
+            return 'valor numerico muito grande, nao suportado, max 999 bilhoes'
+        elif len(num) > 9:
+            C = self.calc_3digitos(num[-3:])
+            M = self.calc_3digitos(num[-6:-3])
+            ML = self.calc_3digitos(num[-9:-6])  
+            BL = self.calc_3digitos(num[:-9])     
+
+            if int(num[-6:-3]) > 0 and int(num[-3:]) == 0: texto_m = ' mil'
+            elif int(num[-6:-3]) > 0 and int(num[-3:]) > 0: texto_m = ' mil e '
+            else: texto_m = ''
+                
+            if int(num[-6:-3]) == 0 and int(num[-9:-6]) == 1 and int(num[-3:]) >= 1: texto_ml = ' milhão e '
+            elif int(num[-6:-3]) == 0 and int(num[-9:-6]) == 1: texto_ml = ' milhão de'
+            elif int(num[-6:-3]) > 0 and int(num[-9:-6]) == 1: texto_ml = ' milhão e '
+            elif int(num[-6:-3]) == 0 and int(num[-9:-6]) > 1: texto_ml = ' milhões de'
+            elif int(num[-6:-3]) > 0 and int(num[-9:-6]) > 1: texto_ml = ' milhões e '
+            else: texto_ml = ''
+            
+            if int(num) == 1000000000: texto_bl = ' bilhão de'
+            elif int(num) > 1000000000 and int(num[-9:]) > 0 and int(num) < 2000000000: texto_bl = ' bilhão e '
+            elif int(num) > 1000000000 and int(num[-9:]) == 0: texto_bl = ' bilhões de'
+            elif int(num) > 2000000000 and int(num[-9:]) > 0: texto_bl = ' bilhões e '
+            else: texto_bl = ''
+            
+            if not monetario:
+                texto_ml = texto_ml.replace(' milhão de', ' milhão')
+                texto_ml = texto_ml.replace(' milhões de', ' milhões')
+                texto_bl = texto_bl.replace(' bilhão de', ' bilhão')
+                texto_bl = texto_bl.replace(' bilhões de', ' bilhões')
+
+            r = BL + texto_bl + ML + texto_ml + M + texto_m + C + ' ' + moeda_plural + centavos if cents != '' else ML + texto_ml + M + texto_m + C + ' ' + moeda_plural
+            return r.replace('  ', ' ') 
+        elif len(num) > 6:
+            C = self.calc_3digitos(num[-3:])
+            M = self.calc_3digitos(num[-6:-3])
+            ML = self.calc_3digitos(num[:-6])       
+
+            if int(num[-6:-3]) > 0 and int(num[-3:]) == 0: texto_m = ' mil'
+            elif int(num[-6:-3]) > 0 and int(num[-3:]) > 0: texto_m = ' mil e '
+            else: texto_m = ''
+                        
+            if int(num) == 1000000: texto_ml = ' milhão de'
+            elif int(num) > 1000000 and int(num[-6:]) > 0 and int(num) < 2000000: texto_ml = ' milhão e '
+            elif int(num) > 1000000 and int(num[-6:]) == 0: texto_ml = ' milhões de'
+            elif int(num) > 2000000 and int(num[-6:]) > 0: texto_ml = ' milhões e '
+            else: texto_ml = ''
+            
+            if not monetario:
+                texto_ml = texto_ml.replace(' milhão de', ' milhão')
+                texto_ml = texto_ml.replace(' milhões de', ' milhões')
+                
+            r = ML + texto_ml + M + texto_m + C + ' ' + moeda_plural + centavos if cents != '' else ML + texto_ml + M + texto_m + C + ' ' + moeda_plural
+            return r.replace('  ', ' ')  
+        elif len(num) > 3:
+            C = self.calc_3digitos(num[-3:])
+            M = self.calc_3digitos(num[:-3])
+            if cents != '': r = M + ' mil ' + moeda_plural if str(num)[-3:] == '000' else M + ' mil e ' + C + ' ' + moeda_plural + centavos
+            else: r = M + ' mil ' + moeda_plural if str(num)[-3:] == '000' else M + ' mil e ' + C + ' ' + moeda_plural
+            return r.replace('  ', ' ')  
+        elif len(num) <= 3:
+            C = self.calc_3digitos(num)
+            if cents != '' and C == '': r = centavos[2:] 
+            elif cents != '': r = C + ' ' + moeda_unit if int(num) == 1 else C + ' ' + moeda_plural + centavos
+            else: r = C + ' ' + moeda_unit if int(num) == 1 else C + ' ' + moeda_plural
+            return r.replace('  ', ' ') 
+        
+                            
 class Gerador_de_codigo:
     
     def __init__(self):
         pass
     
     
     def comentar_linha(self, path:str, search:str):
```

### Comparing `rpa_cooperativa-1.0.63/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.64/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-cooperativa
-Version: 1.0.63
+Version: 1.0.64
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.63/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.64/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.63/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.64/rpa_cooperativa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.63/setup.py` & `rpa_cooperativa-1.0.64/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.63",
+    version="1.0.64",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
```

