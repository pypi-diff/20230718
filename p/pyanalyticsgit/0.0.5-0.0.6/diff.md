# Comparing `tmp/pyanalyticsgit-0.0.5.tar.gz` & `tmp/pyanalyticsgit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyanalyticsgit-0.0.5.tar", last modified: Fri Jul 14 02:11:38 2023, max compression
+gzip compressed data, was "pyanalyticsgit-0.0.6.tar", last modified: Mon Jul 17 23:41:13 2023, max compression
```

## Comparing `pyanalyticsgit-0.0.5.tar` & `pyanalyticsgit-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-14 02:11:38.462043 pyanalyticsgit-0.0.5/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1064 2023-07-13 15:04:24.000000 pyanalyticsgit-0.0.5/LICENSE
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     6941 2023-07-14 02:11:38.462043 pyanalyticsgit-0.0.5/PKG-INFO
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     6391 2023-07-13 15:15:11.000000 pyanalyticsgit-0.0.5/README.md
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-14 02:11:38.454043 pyanalyticsgit-0.0.5/pyanalyticsgit/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       19 2023-07-13 15:04:24.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/__init__.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      314 2023-07-14 02:10:50.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/monitoramento.py
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-14 02:11:38.458043 pyanalyticsgit-0.0.5/pyanalyticsgit/repo/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        0 2023-07-13 15:04:24.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/repo/__init__.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4922 2023-07-13 15:15:11.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/repo/automatizar.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4886 2023-07-14 01:56:02.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/repo/commit.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4414 2023-07-14 00:22:32.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/repo/connect.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4423 2023-07-14 01:56:04.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/repo/issue.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3263 2023-07-14 01:56:06.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/repo/milestone.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3615 2023-07-14 02:05:10.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/repo/relatorio.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1361 2023-07-13 15:15:11.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/test_linux.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1363 2023-07-13 15:15:11.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/test_macos.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1063 2023-07-13 15:15:11.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/test_windows.py
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-14 02:11:38.454043 pyanalyticsgit-0.0.5/pyanalyticsgit.egg-info/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     6941 2023-07-14 02:11:38.000000 pyanalyticsgit-0.0.5/pyanalyticsgit.egg-info/PKG-INFO
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      586 2023-07-14 02:11:38.000000 pyanalyticsgit-0.0.5/pyanalyticsgit.egg-info/SOURCES.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        1 2023-07-14 02:11:38.000000 pyanalyticsgit-0.0.5/pyanalyticsgit.egg-info/dependency_links.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       92 2023-07-14 02:11:38.000000 pyanalyticsgit-0.0.5/pyanalyticsgit.egg-info/requires.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       35 2023-07-14 02:11:38.000000 pyanalyticsgit-0.0.5/pyanalyticsgit.egg-info/top_level.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       38 2023-07-14 02:11:38.462043 pyanalyticsgit-0.0.5/setup.cfg
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      963 2023-07-14 02:08:49.000000 pyanalyticsgit-0.0.5/setup.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-17 23:41:13.391965 pyanalyticsgit-0.0.6/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1064 2023-07-13 15:04:24.000000 pyanalyticsgit-0.0.6/LICENSE
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     6631 2023-07-17 23:41:13.387965 pyanalyticsgit-0.0.6/PKG-INFO
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     6081 2023-07-17 23:36:01.000000 pyanalyticsgit-0.0.6/README.md
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-17 23:41:13.387965 pyanalyticsgit-0.0.6/pyanalyticsgit/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       19 2023-07-13 15:04:24.000000 pyanalyticsgit-0.0.6/pyanalyticsgit/__init__.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      314 2023-07-17 23:33:23.000000 pyanalyticsgit-0.0.6/pyanalyticsgit/monitoramento.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-17 23:41:13.387965 pyanalyticsgit-0.0.6/pyanalyticsgit/repo/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        0 2023-07-13 15:04:24.000000 pyanalyticsgit-0.0.6/pyanalyticsgit/repo/__init__.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4922 2023-07-17 23:04:06.000000 pyanalyticsgit-0.0.6/pyanalyticsgit/repo/automatizar.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     5322 2023-07-17 23:05:06.000000 pyanalyticsgit-0.0.6/pyanalyticsgit/repo/commit.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4680 2023-07-17 23:37:48.000000 pyanalyticsgit-0.0.6/pyanalyticsgit/repo/connect.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4444 2023-07-17 23:05:22.000000 pyanalyticsgit-0.0.6/pyanalyticsgit/repo/issue.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     5468 2023-07-17 23:05:33.000000 pyanalyticsgit-0.0.6/pyanalyticsgit/repo/milestone.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3980 2023-07-17 23:05:43.000000 pyanalyticsgit-0.0.6/pyanalyticsgit/repo/relatorio.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1361 2023-07-17 23:04:06.000000 pyanalyticsgit-0.0.6/pyanalyticsgit/test_linux.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1363 2023-07-17 23:04:06.000000 pyanalyticsgit-0.0.6/pyanalyticsgit/test_macos.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1063 2023-07-17 23:04:06.000000 pyanalyticsgit-0.0.6/pyanalyticsgit/test_windows.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-17 23:41:13.387965 pyanalyticsgit-0.0.6/pyanalyticsgit.egg-info/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     6631 2023-07-17 23:41:13.000000 pyanalyticsgit-0.0.6/pyanalyticsgit.egg-info/PKG-INFO
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      586 2023-07-17 23:41:13.000000 pyanalyticsgit-0.0.6/pyanalyticsgit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        1 2023-07-17 23:41:13.000000 pyanalyticsgit-0.0.6/pyanalyticsgit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       92 2023-07-17 23:41:13.000000 pyanalyticsgit-0.0.6/pyanalyticsgit.egg-info/requires.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       35 2023-07-17 23:41:13.000000 pyanalyticsgit-0.0.6/pyanalyticsgit.egg-info/top_level.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       38 2023-07-17 23:41:13.391965 pyanalyticsgit-0.0.6/setup.cfg
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      963 2023-07-17 23:40:35.000000 pyanalyticsgit-0.0.6/setup.py
```

### Comparing `pyanalyticsgit-0.0.5/LICENSE` & `pyanalyticsgit-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.5/PKG-INFO` & `pyanalyticsgit-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,146 +1,137 @@
 Metadata-Version: 2.1
 Name: pyanalyticsgit
-Version: 0.0.5
+Version: 0.0.6
 Summary: Biblioteca PyAnalyticsGit para gerar relatórios Git.
 Home-page: UNKNOWN
 Author: Gabriel Barbosa, Jefferson Sena, Mateus Levy, Pedro Henrique, Rodrigo Fonseca, Tiago Albuquerque
 Author-email: gabrielb.alencarr@gmail.com, jeffersonsena12144@gmail.com, mateuslevy06@gmail.com, pedrolulhenrique@gmail.com, Rodrigofonseca399@gmail.com, tiago28973@gmail.com 
 License: MIT License
 Keywords: pyAnalyticsGit
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
-<img src="https://user-images.githubusercontent.com/98030427/236968066-315be92b-eabe-4d76-a5d7-bbaaa8df1e2d.png" width="78px" />
+<img src="https://user-images.githubusercontent.com/98030427/236968066-315be92b-eabe-4d76-a5d7-bbaaa8df1e2d.png" width="100px" />
 </div>
 
 
 
 
 # 📝 Descrição
-O PyAnalyticsGit é um projeto em Python criado por estudantes de Engenharia de Software que tem como funcionalidades, a biblioteca do PyAnalyticsGit possibilita que o usuário consiga gerar relatórios automatizados com base em dados de repositórios do GitHub, tais quais, histórico de commits, nome do commit, branch, tamanho do log, etc...
+O PyAnalyticsGit é um projeto em Python criado por estudantes de Engenharia de Software da Universidade de Brasília - UnB. A biblioteca possibilita que o usuário consiga gerar relatórios automatizados a partir de um commit e com base nos dados do repositórios no GitHub como histórico de commits, nome do commit, branch, milestones e entre outros, gerar um relatório em markdown com gráficos e tabelas.
 
-A biblioteca do PyAnalyticsGit deve ser capaz de analisar o desempenho de um projeto oferecendo no relatório parâmetros como taxa de commit por branch, taxa de commit por tempo, horario recorrente de commit, entre outros.
+A biblioteca do PyAnalyticsGit deve ser capaz de analisar o desempenho de um projeto oferecendo no relatório parâmetros como taxa de commit por branch, fluxo de desenvolvimento por sprint, commits por usuário, entre outros.
 
-Com essa ferramenta, é possível obter uma ampla variedade de dados e análises de projetos e repositórios do Git, incluindo gráficos e estatísticas. A biblioteca funciona recebendo os dados de saída dos comandos do Git e realizando a análise e tratamento dos dados de forma eficiente e precisa. Com essa solução, os usuários podem otimizar seus processos e aprimorar a gestão dos seus projetos do Git.
+Com essa ferramenta, é possível obter uma ampla variedade de dados e análises de projetos e repositórios do Git, incluindo gráficos e estatísticas. A biblioteca funciona recebendo os dados da API do GitHub e realizando a análise e tratamento dos dados de forma eficiente. Com essa solução, os usuários podem otimizar seus processos e aprimorar a gestão dos seus projetos do Git.
 
 ## :dart: Objetivo
 ### Qual é o propósito do PyAnalyticsGit?
 
 O PyAnalyticsGit tem como objetivo geral fornecer  uma forma automatizada, eficiente e acessível de gerar relatórios com informações de projetos, progressos e as métricas com dados de repositórios no Github, afim de acompanhar e ter o controle do andamento daquele projeto. Desta forma, os principais objetivos que do PyAnalyticsGit é:
 
 * Extrair informações relevantes de commits, issues e milestones do GitHub.
 * Gerar relatórios em formato Markdown para facilitar a leitura e compartilhamento.
 * Incluir gráficos e tabelas para apresentar visualmente as informações extraídas.
 * Facilitar o acompanhamento do desenvolvimento do projeto e a tomada de decisões.
 
 ##
 
 ## Fluxo de Instalação e Funcionamento
-***OBS: Os comandos estão configurados em Linux, mas deverá estar para Linux,
-MacOs e Windows***
 
 
 ### Instalação/Introdução
- Breve Descrição da API e da Biblioteca (Funcionamento e Visão de Produto
-Resumido). Inicialmente, é recomendável a utilização de um ambiente virtual, que pode ser
+ Inicialmente, é recomendável a utilização de um ambiente virtual, que pode ser
 criado através do venv:
 
 Digite em seu terminal:
 ```
 python3 -m venv myenv
 ```
-Pronto, Assim sera criado um ambiente virtual chamado "myenv"
+Pronto, assim sera criado um ambiente virtual chamado "myenv"
 
 Para ativar o ambiente:
 ```
 source myenv/bin/activate
 ```
-Agora que o ambiente virtual está devidamente criado, Verifique se o ambiente foi inicializado corretamente (verifique que se o nome
-do ambiente, nesse caso “myenv” está no início do caminho em seu terminal.
 
 ### Instalação da biblioteca
 Vamos começar a instalar a biblioteca com o seguinte comando:
 - Instale o sistema de gerenciamento de bibliotecas python “pip”
 - Execute o comando em seu terminal:
 ```
 pip install pyanalyticsgit
 ```
 - Para verificar se a instalação ocorreu com sucesso execute em seu
 terminal:
 ```
 pip show pyanalyticsgit
 ```
 ### Automação
-Apos a configurado e instalado agora o usuario configura a automação. 
+Após configurado e instalado a biblioteca o usuario poderá configurar a automação. 
 
-O usuário deve executar o arquivo a partir de diretório que contenha .git (de um
-diretório que é repositório)
+O usuário deve executar o arquivo a partir do diretório do Repositório no terminal (o diretório deve possuir o arquivo .git para a correta configuração).
 
 Para verificar se seu diretório é um repositório verifique se tem o arquivo
-“.git”
-- execute no terminal o comando: ls -a (pois o .git é uma pasta oculta) —
-(verificar como é no windows)
+“.git” execute no terminal o comando: ls -a (pois o .git é uma pasta oculta).
 
 Verificado isso deve importar a classe Automatiza:
 ```
-from analyticsgit.automatiza import Automatiza
+from pyanalyticsgit.repo.automatiza import Automatiza
 ```
 Após importar deve chamar o método automatiza():
 ```
 Automatizar.automatiza()
 ```
 Este método verifica qual o SO utilizado e
 cria o arquivo post-commit para automatizar
 
 
 Ao executar o repositório estará automatizado e a cada commit será gerado um
-relatório.
+relatório em markdown.
 Após executar o método de automação não é necessário executar novamente.
 O usuário deve apagar o método caso for gerar um relatório Estático.
 
 ### Relatório Automatizado
 
-A cada evento de commit o git chama o método de monitoramento que executa
+A cada evento de commit o git chama o scripty de monitoramento que executa
 a criação do relatório.
-- Obs: Toda essa parte é automatizada o usuário so precisa executar os
-métodos de cima e configurar o .env
 
 O relatório gerado estará em um arquivo docs/relatorio.md
 
 - .env:
   - Deve ser criado um arquivo .env no ambiente de utilização da biblioteca e
 definir os valores de ‘user_name’(usuário ou repositório que contém o
-repositório que se quer o relatório) e ‘repo_name’ (repositório desejado)
+repositório que será gerado o relatório) e ‘repo_name’ (repositório desejado)
   - Exemplo no repostirório https://github.com/fga-eps-mds/2023.1-PyAnalyticsGit.git :
 
 - O arquivo ‘.env’ deve estar assim para o exemplo acima:
   ```
   user_name = "fga-eps-mds"
   repo_name = "2023.1-PyAnalyticsGit"
   ```
 ### Relatório Estático
 Gera relatórios de repositórios a partir da função “gerar_relatório” recebendo
 como parâmetros os valores de usuários e/ou repositórios existentes do github:
 
-- Exemplo: https://github.com/fga-eps-mds/2023.1-PyAnalyticsGit.git
-- Utilize o método:
+Para criar o relatório deverá ser importado a classe Relatorio:
 ```
-gerar_relatorio(’fga-eps-mds’,’2023.1-PyAnalyticsGit’)
+from pyanalyticsgit.repo.relatorio import Relatorio
 ```
-- Lembre-se de mudar os parâmetros para o repositório em interesse.
+Ao importar o usuário cria uma instância da classe Relatorio e chama o método:
 
-Caso os parâmetros não sejam fornecidos, o relatório usará os valores das
-variáveis de ambiente contidas em .env.
+- Exemplo: https://github.com/fga-eps-mds/2023.1-PyAnalyticsGit.git
 ```
-gerar_relatorio()
+Relatorio().gerar_relatorio(’fga-eps-mds’,’2023.1-PyAnalyticsGit’)
 ```
 
+Caso os parâmetros não sejam fornecidos, o relatório buscará os valores das
+variáveis de ambiente contidas em .env.
+
 ##
 # 🤝 Colaboradores
 
 | [<img src="https://github.com/gabrie1barbosa.png" width=80><br><sub>Gabriel Barbosa</sub>](https://github.com/gabrie1barbosa) |  [<img src="https://github.com/JeffersonSenaa.png" width=80><br><sub>Jefferson Sena</sub>](https://github.com/JeffersonSenaa) | [<img src="https://github.com/mateus9levy.png" width=80><br><sub>Mateus Levy</sub>](https://github.com/mateus9levy) |  [<img src="https://github.com/PedroHhenriq.png" width=80><br><sub>Pedro Henrique</sub>](https://github.com/PedroHhenriq) |  [<img src="https://github.com/rodfon3301.png" width=80><br><sub>Rodrigo Fonseca</sub>](https://github.com/rodfon3301) |   [<img src="https://github.com/Tiago1604.png" width=80><br><sub>Tiago Albuquerque</sub>](https://github.com/Tiago1604) |
 | :---: | :---: | :---: |  :---: | :---: | :---: | 
 
 ##
```

### Comparing `pyanalyticsgit-0.0.5/README.md` & `pyanalyticsgit-0.0.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,133 +1,124 @@
 <div align="center">
-<img src="https://user-images.githubusercontent.com/98030427/236968066-315be92b-eabe-4d76-a5d7-bbaaa8df1e2d.png" width="78px" />
+<img src="https://user-images.githubusercontent.com/98030427/236968066-315be92b-eabe-4d76-a5d7-bbaaa8df1e2d.png" width="100px" />
 </div>
 
 
 
 
 # 📝 Descrição
-O PyAnalyticsGit é um projeto em Python criado por estudantes de Engenharia de Software que tem como funcionalidades, a biblioteca do PyAnalyticsGit possibilita que o usuário consiga gerar relatórios automatizados com base em dados de repositórios do GitHub, tais quais, histórico de commits, nome do commit, branch, tamanho do log, etc...
+O PyAnalyticsGit é um projeto em Python criado por estudantes de Engenharia de Software da Universidade de Brasília - UnB. A biblioteca possibilita que o usuário consiga gerar relatórios automatizados a partir de um commit e com base nos dados do repositórios no GitHub como histórico de commits, nome do commit, branch, milestones e entre outros, gerar um relatório em markdown com gráficos e tabelas.
 
-A biblioteca do PyAnalyticsGit deve ser capaz de analisar o desempenho de um projeto oferecendo no relatório parâmetros como taxa de commit por branch, taxa de commit por tempo, horario recorrente de commit, entre outros.
+A biblioteca do PyAnalyticsGit deve ser capaz de analisar o desempenho de um projeto oferecendo no relatório parâmetros como taxa de commit por branch, fluxo de desenvolvimento por sprint, commits por usuário, entre outros.
 
-Com essa ferramenta, é possível obter uma ampla variedade de dados e análises de projetos e repositórios do Git, incluindo gráficos e estatísticas. A biblioteca funciona recebendo os dados de saída dos comandos do Git e realizando a análise e tratamento dos dados de forma eficiente e precisa. Com essa solução, os usuários podem otimizar seus processos e aprimorar a gestão dos seus projetos do Git.
+Com essa ferramenta, é possível obter uma ampla variedade de dados e análises de projetos e repositórios do Git, incluindo gráficos e estatísticas. A biblioteca funciona recebendo os dados da API do GitHub e realizando a análise e tratamento dos dados de forma eficiente. Com essa solução, os usuários podem otimizar seus processos e aprimorar a gestão dos seus projetos do Git.
 
 ## :dart: Objetivo
 ### Qual é o propósito do PyAnalyticsGit?
 
 O PyAnalyticsGit tem como objetivo geral fornecer  uma forma automatizada, eficiente e acessível de gerar relatórios com informações de projetos, progressos e as métricas com dados de repositórios no Github, afim de acompanhar e ter o controle do andamento daquele projeto. Desta forma, os principais objetivos que do PyAnalyticsGit é:
 
 * Extrair informações relevantes de commits, issues e milestones do GitHub.
 * Gerar relatórios em formato Markdown para facilitar a leitura e compartilhamento.
 * Incluir gráficos e tabelas para apresentar visualmente as informações extraídas.
 * Facilitar o acompanhamento do desenvolvimento do projeto e a tomada de decisões.
 
 ##
 
 ## Fluxo de Instalação e Funcionamento
-***OBS: Os comandos estão configurados em Linux, mas deverá estar para Linux,
-MacOs e Windows***
 
 
 ### Instalação/Introdução
- Breve Descrição da API e da Biblioteca (Funcionamento e Visão de Produto
-Resumido). Inicialmente, é recomendável a utilização de um ambiente virtual, que pode ser
+ Inicialmente, é recomendável a utilização de um ambiente virtual, que pode ser
 criado através do venv:
 
 Digite em seu terminal:
 ```
 python3 -m venv myenv
 ```
-Pronto, Assim sera criado um ambiente virtual chamado "myenv"
+Pronto, assim sera criado um ambiente virtual chamado "myenv"
 
 Para ativar o ambiente:
 ```
 source myenv/bin/activate
 ```
-Agora que o ambiente virtual está devidamente criado, Verifique se o ambiente foi inicializado corretamente (verifique que se o nome
-do ambiente, nesse caso “myenv” está no início do caminho em seu terminal.
 
 ### Instalação da biblioteca
 Vamos começar a instalar a biblioteca com o seguinte comando:
 - Instale o sistema de gerenciamento de bibliotecas python “pip”
 - Execute o comando em seu terminal:
 ```
 pip install pyanalyticsgit
 ```
 - Para verificar se a instalação ocorreu com sucesso execute em seu
 terminal:
 ```
 pip show pyanalyticsgit
 ```
 ### Automação
-Apos a configurado e instalado agora o usuario configura a automação. 
+Após configurado e instalado a biblioteca o usuario poderá configurar a automação. 
 
-O usuário deve executar o arquivo a partir de diretório que contenha .git (de um
-diretório que é repositório)
+O usuário deve executar o arquivo a partir do diretório do Repositório no terminal (o diretório deve possuir o arquivo .git para a correta configuração).
 
 Para verificar se seu diretório é um repositório verifique se tem o arquivo
-“.git”
-- execute no terminal o comando: ls -a (pois o .git é uma pasta oculta) —
-(verificar como é no windows)
+“.git” execute no terminal o comando: ls -a (pois o .git é uma pasta oculta).
 
 Verificado isso deve importar a classe Automatiza:
 ```
-from analyticsgit.automatiza import Automatiza
+from pyanalyticsgit.repo.automatiza import Automatiza
 ```
 Após importar deve chamar o método automatiza():
 ```
 Automatizar.automatiza()
 ```
 Este método verifica qual o SO utilizado e
 cria o arquivo post-commit para automatizar
 
 
 Ao executar o repositório estará automatizado e a cada commit será gerado um
-relatório.
+relatório em markdown.
 Após executar o método de automação não é necessário executar novamente.
 O usuário deve apagar o método caso for gerar um relatório Estático.
 
 ### Relatório Automatizado
 
-A cada evento de commit o git chama o método de monitoramento que executa
+A cada evento de commit o git chama o scripty de monitoramento que executa
 a criação do relatório.
-- Obs: Toda essa parte é automatizada o usuário so precisa executar os
-métodos de cima e configurar o .env
 
 O relatório gerado estará em um arquivo docs/relatorio.md
 
 - .env:
   - Deve ser criado um arquivo .env no ambiente de utilização da biblioteca e
 definir os valores de ‘user_name’(usuário ou repositório que contém o
-repositório que se quer o relatório) e ‘repo_name’ (repositório desejado)
+repositório que será gerado o relatório) e ‘repo_name’ (repositório desejado)
   - Exemplo no repostirório https://github.com/fga-eps-mds/2023.1-PyAnalyticsGit.git :
 
 - O arquivo ‘.env’ deve estar assim para o exemplo acima:
   ```
   user_name = "fga-eps-mds"
   repo_name = "2023.1-PyAnalyticsGit"
   ```
 ### Relatório Estático
 Gera relatórios de repositórios a partir da função “gerar_relatório” recebendo
 como parâmetros os valores de usuários e/ou repositórios existentes do github:
 
-- Exemplo: https://github.com/fga-eps-mds/2023.1-PyAnalyticsGit.git
-- Utilize o método:
+Para criar o relatório deverá ser importado a classe Relatorio:
 ```
-gerar_relatorio(’fga-eps-mds’,’2023.1-PyAnalyticsGit’)
+from pyanalyticsgit.repo.relatorio import Relatorio
 ```
-- Lembre-se de mudar os parâmetros para o repositório em interesse.
+Ao importar o usuário cria uma instância da classe Relatorio e chama o método:
 
-Caso os parâmetros não sejam fornecidos, o relatório usará os valores das
-variáveis de ambiente contidas em .env.
+- Exemplo: https://github.com/fga-eps-mds/2023.1-PyAnalyticsGit.git
 ```
-gerar_relatorio()
+Relatorio().gerar_relatorio(’fga-eps-mds’,’2023.1-PyAnalyticsGit’)
 ```
 
+Caso os parâmetros não sejam fornecidos, o relatório buscará os valores das
+variáveis de ambiente contidas em .env.
+
 ##
 # 🤝 Colaboradores
 
 | [<img src="https://github.com/gabrie1barbosa.png" width=80><br><sub>Gabriel Barbosa</sub>](https://github.com/gabrie1barbosa) |  [<img src="https://github.com/JeffersonSenaa.png" width=80><br><sub>Jefferson Sena</sub>](https://github.com/JeffersonSenaa) | [<img src="https://github.com/mateus9levy.png" width=80><br><sub>Mateus Levy</sub>](https://github.com/mateus9levy) |  [<img src="https://github.com/PedroHhenriq.png" width=80><br><sub>Pedro Henrique</sub>](https://github.com/PedroHhenriq) |  [<img src="https://github.com/rodfon3301.png" width=80><br><sub>Rodrigo Fonseca</sub>](https://github.com/rodfon3301) |   [<img src="https://github.com/Tiago1604.png" width=80><br><sub>Tiago Albuquerque</sub>](https://github.com/Tiago1604) |
 | :---: | :---: | :---: |  :---: | :---: | :---: | 
 
 ##
```

### Comparing `pyanalyticsgit-0.0.5/pyanalyticsgit/repo/automatizar.py` & `pyanalyticsgit-0.0.6/pyanalyticsgit/repo/automatizar.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.5/pyanalyticsgit/repo/commit.py` & `pyanalyticsgit-0.0.6/pyanalyticsgit/repo/commit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from collections import defaultdict
 import matplotlib.pyplot as plt
 from wordcloud import STOPWORDS, WordCloud
 import os
 from .connect import  Connect, api_name, api_user
 
 # diretorio_raiz = os.path.abspath(os.path.dirname(__file__))
 diretorio_raiz = os.getcwd()
@@ -37,78 +36,91 @@
 
         stopwords = set(STOPWORDS)
         stopwords.update(self.palavras_ignoradas) 
 
         wordcloud = WordCloud(width=800, height=400, background_color='white', stopwords=stopwords,
                               colormap='viridis', max_words=300).generate(texto)
 
-        plt.figure(figsize=(10, 5))
+        plt.figure(figsize=(14, 8))
         plt.imshow(wordcloud, interpolation='bilinear') 
         plt.axis('off')
         plt.title('Nuvem de palavras com nomes dos Commits')
 
         if os.path.exists(os.path.join(caminho_pasta,grafico_nuvem)):
             os.remove(os.path.join(caminho_pasta,grafico_nuvem))
 
         plt.savefig(os.path.join(caminho_pasta,grafico_nuvem))
         plt.close()    
 
     def criar_grafico_commit(self):
         """Método que cria um gráfico de barras com os nomes dos autores e a quantidade de commits"""
-        commit_authors = defaultdict(int)
+        authors = {}
         for commit in self.commits:
-            author = commit["commit"]["author"]["name"]
-            commit_authors[author] += 1
+            author_name = commit['commit']['author']['name']
+            author_login = commit['author']['login'] if commit['author'] is not None else ""
 
-        authors = list(commit_authors.keys())
-        commit_numbers = list(commit_authors.values())
+            # Usa o nome do autor como chave para agrupar os commits
+            key = author_name.lower()
+            if key not in authors:
+                authors[key] = {
+                    'name': author_name,
+                    'login': author_login,
+                    'count': 1
+                }
+            else:
+                authors[key]['count'] += 1
+
+        nicknames = [author['login'] for author in authors.values()]
+        commit_counts = [author['count'] for author in authors.values()]
 
-        plt.bar(authors, commit_numbers, color='darkred')
+        plt.figure(figsize=(8, 9))
+        plt.bar(nicknames, commit_counts, color='darkred')
         plt.xlabel('Autores')
         plt.ylabel('Número de Commits', color='darkred')
         plt.title('Gráfico de Commits por Autor', fontsize=16, color='black')
         plt.xticks(rotation=45)
         plt.gca().set_facecolor('black')
         if os.path.exists(os.path.join(caminho_pasta,grafico)):
             os.remove(os.path.join(caminho_pasta,grafico))
 
         plt.savefig(os.path.join(caminho_pasta,grafico))
         plt.close()
 
     def criar_tabela_commit(self, relatorio_file):
         """Método que cria uma tabela com os nomes dos autores e a quantidade de commits por autor"""
-        commit_count = {}
-        commit_datas = {}
+        authors = {}
         for commit in self.commits:
-            author = commit["commit"]["author"]["name"]
-            if author in commit_count:
-                commit_count[author] += 1
-                commit_datas[author].append(commit["commit"]["author"]["date"])
+            author_name = commit['commit']['author']['name']
+            author_login = commit['author']['login'] if commit['author'] is not None else ""
+
+            if author_login not in authors:
+                authors[author_login] = {
+                    'name': author_login,
+                    'commits': [],
+                    'count': 1
+                }
             else:
-                commit_count[author] = 1
-                commit_datas[author] = [commit["commit"]["author"]["date"]]    
+                authors[author_login]['count'] += 1
+
+            authors[author_login]['commits'].append(commit)
 
         with open(relatorio_file, "a+", encoding="utf-8") as file:
-            file.write("# Tabela - Quantidade de Commits por Membro\n\n")
-            file.write("| Membro | Quantidade de Commits |\n")
+            file.write("# Tabela - Quantidade de Commits por Autor\n\n")
+            file.write("| Autor | Quantidade de Commits |\n")
             file.write("| --- | ---: |\n")
-            for author, count in commit_count.items():
-                file.write(f"| {author} | {count} |\n")
+            for author_login, data in authors.items():
+                file.write(f"| {data['name']} | {data['count']} |\n")
             file.write("\n")
 
         with open(relatorio_file, "a+", encoding="utf-8") as file:
-            file.write("# Tabela de Commits por Autor\n\n")
-
-            for author in commit_count.keys():
-                file.write(f"## {author}\n\n")
+            for author_login, data in authors.items():
+                file.write("# Tabela de Commits por Autor\n\n")
+                file.write(f"## {data['name']}\n\n")
                 file.write("| Commit | Data |\n")
                 file.write("| --- | --- |\n")
-        
-                author_commits = [commit for commit in self.commits if commit["commit"]["author"]["name"] == author]
-        
-                for commit in author_commits:
+
+                for commit in data['commits']:
                     commit_message = commit["commit"]["message"]
                     commit_date = commit["commit"]["author"]["date"].split("T")[0]
                     commit_resume = " ".join(commit_message.split()[:7]) + "..." if len(commit_message.split()) > 7 else commit_message
                     file.write(f"| {commit_resume} | {commit_date} |\n")
-                file.write("\n")
-            file.write("\n")
+                file.write("\n")
```

### Comparing `pyanalyticsgit-0.0.5/pyanalyticsgit/repo/connect.py` & `pyanalyticsgit-0.0.6/pyanalyticsgit/repo/connect.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,15 +43,16 @@
                     page += 1
             
             elif response.status_code == 403:
                 print(f'StatusCode: {response.status_code}')
                 print(f'Falha ao obter os detalhes do repositório {repo}. Foram feitas muitas requisições.')
                 timestamp = response.headers['X-RateLimit-Reset']
                 tempo_fora = datetime.datetime.fromtimestamp(int(timestamp))
-                print(f'Você poderá voltar a fazer requisições em: {tempo_fora}')
+                tempo_fora_formatado = tempo_fora.strftime("%d-%m-%Y %H:%M:%S")
+                print(f'Você poderá voltar a fazer requisições em: {tempo_fora_formatado}')
                 sys.exit()
     
             else:
                 print(f'Falha ao obter os detalhes do repositório {repo}.')
                 print(f'StatusCode: {response.status_code}')
                 sys.exit()
 
@@ -77,15 +78,16 @@
                     page += 1
                
             elif response.status_code == 403:
                 print(f'StatusCode: {response.status_code}')
                 print(f'Falha ao obter os detalhes do repositório {repo}. Foram feitas muitas requisições.')
                 timestamp = response.headers['X-RateLimit-Reset']
                 tempo_fora = datetime.datetime.fromtimestamp(int(timestamp))
-                print(f'Você poderá voltar a fazer requisições em: {tempo_fora}')
+                tempo_fora_formatado = tempo_fora.strftime("%d-%m-%Y %H:%M:%S")
+                print(f'Você poderá voltar a fazer requisições em: {tempo_fora_formatado}')
                 sys.exit()
 
             else:
                 print(f'Falha ao obter os detalhes do repositório {repo}.')
                 print(f'StatusCode: {response.status_code}')
                 sys.exit()
 
@@ -101,14 +103,15 @@
             return self.milestones
         
         elif response.status_code == 403:
             print(f'StatusCode: {response.status_code}')
             print(f'Falha ao obter os detalhes do repositório {repo}. Foram feitas muitas requisições.')
             timestamp = response.headers['X-RateLimit-Reset']
             tempo_fora = datetime.datetime.fromtimestamp(int(timestamp))
-            print(f'Você poderá voltar a fazer requisições em: {tempo_fora}')
+            tempo_fora_formatado = tempo_fora.strftime("%d-%m-%Y %H:%M:%S")
+            print(f'Você poderá voltar a fazer requisições em: {tempo_fora_formatado}')
             sys.exit()
 
         else:
             print(f'Falha ao obter os detalhes do repositório {repo}.\n')
             print(f'StatusCode: {response.status_code}')
             sys.exit()
```

### Comparing `pyanalyticsgit-0.0.5/pyanalyticsgit/repo/issue.py` & `pyanalyticsgit-0.0.6/pyanalyticsgit/repo/issue.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,17 +33,17 @@
                 label_count[label["name"]] += 1
 
         labels = list(label_count.keys())
         counts = list(label_count.values())
         percentages = [(count / total_issues) * 100 for count in counts]
         sorted_labels, sorted_percentages = zip(*sorted(zip(labels, percentages), key=lambda x: x[1], reverse=True))
 
-        fig, ax = plt.subplots() 
+        fig, ax = plt.subplots(figsize=(14, 8)) 
         ax.pie(sorted_percentages, labels=sorted_labels, shadow=True, autopct='%1.1f%%', startangle=90)
-        ax.legend(loc='center right', bbox_to_anchor=(1.0, 0.5), fontsize='medium', title='Tags')
+        ax.legend(loc='upper left', fontsize='medium', title='Tags')
         ax.set_title('Grafico de Issues por Tags')
         ax.axis('equal')
         if os.path.exists(os.path.join(caminho_pasta,grafico_pizza)):
             os.remove(os.path.join(caminho_pasta,grafico_pizza))   
 
         plt.savefig(os.path.join(caminho_pasta,grafico_pizza))
         plt.close()
@@ -54,14 +54,15 @@
         for issue in self.issues:
             author = issue["user"]["login"]
             issue_authors[author] += 1
 
         authors = list(issue_authors.keys())
         issue_numbers = list(issue_authors.values())
 
+        plt.figure(figsize=(8, 9))
         plt.bar(authors, issue_numbers, color='steelblue')
         plt.xlabel('Autores')
         plt.ylabel('Número de Issues', color='steelblue')
         plt.title('Gráfico de Issues por Autor', fontsize=16, color='black')
         plt.xticks(rotation=45)
         plt.gca().set_facecolor('black')
         if os.path.exists(os.path.join(caminho_pasta,grafico_issue)):
```

### Comparing `pyanalyticsgit-0.0.5/pyanalyticsgit/repo/relatorio.py` & `pyanalyticsgit-0.0.6/pyanalyticsgit/repo/relatorio.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,8 +82,15 @@
             arq.write("# Milestones\n\n")
             arq.write("## Gráfico de Milestones\n\n")
             arq.write("<div align='center'>\n\n")
             arq.write("![Gráfico de Milestones](grafico_milestone.png)\n\n")
             arq.write("</div>\n\n")
 
         grafico_tabela_milestone.criar_tabela_milestone(self.caminho_arquivo)
-    
+
+        grafico_tabela_milestone.criar_grafico_miles_tag()
+
+        with open(self.caminho_arquivo, 'a+', encoding="utf-8") as arq:
+            arq.write("## Gráfico de Tags por Milestones\n\n")
+            arq.write("<div align='center'>\n\n")
+            arq.write("![Gráfico de Tags por Milestones](grafico_miles_tag.png)\n\n")
+            arq.write("</div>\n\n")
```

### Comparing `pyanalyticsgit-0.0.5/pyanalyticsgit/test_linux.py` & `pyanalyticsgit-0.0.6/pyanalyticsgit/test_linux.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.5/pyanalyticsgit/test_macos.py` & `pyanalyticsgit-0.0.6/pyanalyticsgit/test_macos.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.5/pyanalyticsgit/test_windows.py` & `pyanalyticsgit-0.0.6/pyanalyticsgit/test_windows.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.5/pyanalyticsgit.egg-info/PKG-INFO` & `pyanalyticsgit-0.0.6/pyanalyticsgit.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,146 +1,137 @@
 Metadata-Version: 2.1
 Name: pyanalyticsgit
-Version: 0.0.5
+Version: 0.0.6
 Summary: Biblioteca PyAnalyticsGit para gerar relatórios Git.
 Home-page: UNKNOWN
 Author: Gabriel Barbosa, Jefferson Sena, Mateus Levy, Pedro Henrique, Rodrigo Fonseca, Tiago Albuquerque
 Author-email: gabrielb.alencarr@gmail.com, jeffersonsena12144@gmail.com, mateuslevy06@gmail.com, pedrolulhenrique@gmail.com, Rodrigofonseca399@gmail.com, tiago28973@gmail.com 
 License: MIT License
 Keywords: pyAnalyticsGit
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
-<img src="https://user-images.githubusercontent.com/98030427/236968066-315be92b-eabe-4d76-a5d7-bbaaa8df1e2d.png" width="78px" />
+<img src="https://user-images.githubusercontent.com/98030427/236968066-315be92b-eabe-4d76-a5d7-bbaaa8df1e2d.png" width="100px" />
 </div>
 
 
 
 
 # 📝 Descrição
-O PyAnalyticsGit é um projeto em Python criado por estudantes de Engenharia de Software que tem como funcionalidades, a biblioteca do PyAnalyticsGit possibilita que o usuário consiga gerar relatórios automatizados com base em dados de repositórios do GitHub, tais quais, histórico de commits, nome do commit, branch, tamanho do log, etc...
+O PyAnalyticsGit é um projeto em Python criado por estudantes de Engenharia de Software da Universidade de Brasília - UnB. A biblioteca possibilita que o usuário consiga gerar relatórios automatizados a partir de um commit e com base nos dados do repositórios no GitHub como histórico de commits, nome do commit, branch, milestones e entre outros, gerar um relatório em markdown com gráficos e tabelas.
 
-A biblioteca do PyAnalyticsGit deve ser capaz de analisar o desempenho de um projeto oferecendo no relatório parâmetros como taxa de commit por branch, taxa de commit por tempo, horario recorrente de commit, entre outros.
+A biblioteca do PyAnalyticsGit deve ser capaz de analisar o desempenho de um projeto oferecendo no relatório parâmetros como taxa de commit por branch, fluxo de desenvolvimento por sprint, commits por usuário, entre outros.
 
-Com essa ferramenta, é possível obter uma ampla variedade de dados e análises de projetos e repositórios do Git, incluindo gráficos e estatísticas. A biblioteca funciona recebendo os dados de saída dos comandos do Git e realizando a análise e tratamento dos dados de forma eficiente e precisa. Com essa solução, os usuários podem otimizar seus processos e aprimorar a gestão dos seus projetos do Git.
+Com essa ferramenta, é possível obter uma ampla variedade de dados e análises de projetos e repositórios do Git, incluindo gráficos e estatísticas. A biblioteca funciona recebendo os dados da API do GitHub e realizando a análise e tratamento dos dados de forma eficiente. Com essa solução, os usuários podem otimizar seus processos e aprimorar a gestão dos seus projetos do Git.
 
 ## :dart: Objetivo
 ### Qual é o propósito do PyAnalyticsGit?
 
 O PyAnalyticsGit tem como objetivo geral fornecer  uma forma automatizada, eficiente e acessível de gerar relatórios com informações de projetos, progressos e as métricas com dados de repositórios no Github, afim de acompanhar e ter o controle do andamento daquele projeto. Desta forma, os principais objetivos que do PyAnalyticsGit é:
 
 * Extrair informações relevantes de commits, issues e milestones do GitHub.
 * Gerar relatórios em formato Markdown para facilitar a leitura e compartilhamento.
 * Incluir gráficos e tabelas para apresentar visualmente as informações extraídas.
 * Facilitar o acompanhamento do desenvolvimento do projeto e a tomada de decisões.
 
 ##
 
 ## Fluxo de Instalação e Funcionamento
-***OBS: Os comandos estão configurados em Linux, mas deverá estar para Linux,
-MacOs e Windows***
 
 
 ### Instalação/Introdução
- Breve Descrição da API e da Biblioteca (Funcionamento e Visão de Produto
-Resumido). Inicialmente, é recomendável a utilização de um ambiente virtual, que pode ser
+ Inicialmente, é recomendável a utilização de um ambiente virtual, que pode ser
 criado através do venv:
 
 Digite em seu terminal:
 ```
 python3 -m venv myenv
 ```
-Pronto, Assim sera criado um ambiente virtual chamado "myenv"
+Pronto, assim sera criado um ambiente virtual chamado "myenv"
 
 Para ativar o ambiente:
 ```
 source myenv/bin/activate
 ```
-Agora que o ambiente virtual está devidamente criado, Verifique se o ambiente foi inicializado corretamente (verifique que se o nome
-do ambiente, nesse caso “myenv” está no início do caminho em seu terminal.
 
 ### Instalação da biblioteca
 Vamos começar a instalar a biblioteca com o seguinte comando:
 - Instale o sistema de gerenciamento de bibliotecas python “pip”
 - Execute o comando em seu terminal:
 ```
 pip install pyanalyticsgit
 ```
 - Para verificar se a instalação ocorreu com sucesso execute em seu
 terminal:
 ```
 pip show pyanalyticsgit
 ```
 ### Automação
-Apos a configurado e instalado agora o usuario configura a automação. 
+Após configurado e instalado a biblioteca o usuario poderá configurar a automação. 
 
-O usuário deve executar o arquivo a partir de diretório que contenha .git (de um
-diretório que é repositório)
+O usuário deve executar o arquivo a partir do diretório do Repositório no terminal (o diretório deve possuir o arquivo .git para a correta configuração).
 
 Para verificar se seu diretório é um repositório verifique se tem o arquivo
-“.git”
-- execute no terminal o comando: ls -a (pois o .git é uma pasta oculta) —
-(verificar como é no windows)
+“.git” execute no terminal o comando: ls -a (pois o .git é uma pasta oculta).
 
 Verificado isso deve importar a classe Automatiza:
 ```
-from analyticsgit.automatiza import Automatiza
+from pyanalyticsgit.repo.automatiza import Automatiza
 ```
 Após importar deve chamar o método automatiza():
 ```
 Automatizar.automatiza()
 ```
 Este método verifica qual o SO utilizado e
 cria o arquivo post-commit para automatizar
 
 
 Ao executar o repositório estará automatizado e a cada commit será gerado um
-relatório.
+relatório em markdown.
 Após executar o método de automação não é necessário executar novamente.
 O usuário deve apagar o método caso for gerar um relatório Estático.
 
 ### Relatório Automatizado
 
-A cada evento de commit o git chama o método de monitoramento que executa
+A cada evento de commit o git chama o scripty de monitoramento que executa
 a criação do relatório.
-- Obs: Toda essa parte é automatizada o usuário so precisa executar os
-métodos de cima e configurar o .env
 
 O relatório gerado estará em um arquivo docs/relatorio.md
 
 - .env:
   - Deve ser criado um arquivo .env no ambiente de utilização da biblioteca e
 definir os valores de ‘user_name’(usuário ou repositório que contém o
-repositório que se quer o relatório) e ‘repo_name’ (repositório desejado)
+repositório que será gerado o relatório) e ‘repo_name’ (repositório desejado)
   - Exemplo no repostirório https://github.com/fga-eps-mds/2023.1-PyAnalyticsGit.git :
 
 - O arquivo ‘.env’ deve estar assim para o exemplo acima:
   ```
   user_name = "fga-eps-mds"
   repo_name = "2023.1-PyAnalyticsGit"
   ```
 ### Relatório Estático
 Gera relatórios de repositórios a partir da função “gerar_relatório” recebendo
 como parâmetros os valores de usuários e/ou repositórios existentes do github:
 
-- Exemplo: https://github.com/fga-eps-mds/2023.1-PyAnalyticsGit.git
-- Utilize o método:
+Para criar o relatório deverá ser importado a classe Relatorio:
 ```
-gerar_relatorio(’fga-eps-mds’,’2023.1-PyAnalyticsGit’)
+from pyanalyticsgit.repo.relatorio import Relatorio
 ```
-- Lembre-se de mudar os parâmetros para o repositório em interesse.
+Ao importar o usuário cria uma instância da classe Relatorio e chama o método:
 
-Caso os parâmetros não sejam fornecidos, o relatório usará os valores das
-variáveis de ambiente contidas em .env.
+- Exemplo: https://github.com/fga-eps-mds/2023.1-PyAnalyticsGit.git
 ```
-gerar_relatorio()
+Relatorio().gerar_relatorio(’fga-eps-mds’,’2023.1-PyAnalyticsGit’)
 ```
 
+Caso os parâmetros não sejam fornecidos, o relatório buscará os valores das
+variáveis de ambiente contidas em .env.
+
 ##
 # 🤝 Colaboradores
 
 | [<img src="https://github.com/gabrie1barbosa.png" width=80><br><sub>Gabriel Barbosa</sub>](https://github.com/gabrie1barbosa) |  [<img src="https://github.com/JeffersonSenaa.png" width=80><br><sub>Jefferson Sena</sub>](https://github.com/JeffersonSenaa) | [<img src="https://github.com/mateus9levy.png" width=80><br><sub>Mateus Levy</sub>](https://github.com/mateus9levy) |  [<img src="https://github.com/PedroHhenriq.png" width=80><br><sub>Pedro Henrique</sub>](https://github.com/PedroHhenriq) |  [<img src="https://github.com/rodfon3301.png" width=80><br><sub>Rodrigo Fonseca</sub>](https://github.com/rodfon3301) |   [<img src="https://github.com/Tiago1604.png" width=80><br><sub>Tiago Albuquerque</sub>](https://github.com/Tiago1604) |
 | :---: | :---: | :---: |  :---: | :---: | :---: | 
 
 ##
```

### Comparing `pyanalyticsgit-0.0.5/pyanalyticsgit.egg-info/SOURCES.txt` & `pyanalyticsgit-0.0.6/pyanalyticsgit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.5/setup.py` & `pyanalyticsgit-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from setuptools.dist import Distribution
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='pyanalyticsgit',
-    version='0.0.5',
+    version='0.0.6',
     license='MIT License',
     author='Gabriel Barbosa, Jefferson Sena, Mateus Levy, Pedro Henrique, Rodrigo Fonseca, Tiago Albuquerque',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='gabrielb.alencarr@gmail.com, jeffersonsena12144@gmail.com, mateuslevy06@gmail.com, pedrolulhenrique@gmail.com, Rodrigofonseca399@gmail.com, tiago28973@gmail.com ',
     keywords='pyAnalyticsGit',
     description=u'Biblioteca PyAnalyticsGit para gerar relatórios Git.',
```

