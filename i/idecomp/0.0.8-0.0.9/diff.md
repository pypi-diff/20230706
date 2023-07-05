# Comparing `tmp/idecomp-0.0.8.tar.gz` & `tmp/idecomp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idecomp-0.0.8.tar", last modified: Tue May 18 00:44:30 2021, max compression
+gzip compressed data, was "idecomp-0.0.9.tar", last modified: Wed Aug 11 21:09:12 2021, max compression
```

## Comparing `idecomp-0.0.8.tar` & `idecomp-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 00:44:30.238346 idecomp-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-05-18 00:43:39.000000 idecomp-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2842 2021-05-18 00:44:30.238346 idecomp-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2052 2021-05-18 00:43:39.000000 idecomp-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 00:44:30.238346 idecomp-0.0.8/idecomp/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2021-05-18 00:43:39.000000 idecomp-0.0.8/idecomp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 00:44:30.238346 idecomp-0.0.8/idecomp/_utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-18 00:43:39.000000 idecomp-0.0.8/idecomp/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      143 2021-05-18 00:43:39.000000 idecomp-0.0.8/idecomp/_utils/escrita.py
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2021-05-18 00:43:39.000000 idecomp-0.0.8/idecomp/_utils/leitura.py
--rw-r--r--   0 runner    (1001) docker     (121)      205 2021-05-18 00:43:39.000000 idecomp-0.0.8/idecomp/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 00:44:30.238346 idecomp-0.0.8/idecomp/decomp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-18 00:43:39.000000 idecomp-0.0.8/idecomp/decomp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 00:44:30.238346 idecomp-0.0.8/idecomp/decomp/modelos/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-18 00:43:39.000000 idecomp-0.0.8/idecomp/decomp/modelos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24807 2021-05-18 00:43:39.000000 idecomp-0.0.8/idecomp/decomp/modelos/relato.py
--rw-r--r--   0 runner    (1001) docker     (121)    17783 2021-05-18 00:43:39.000000 idecomp-0.0.8/idecomp/decomp/relato.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 00:44:30.238346 idecomp-0.0.8/idecomp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2842 2021-05-18 00:44:30.000000 idecomp-0.0.8/idecomp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      417 2021-05-18 00:44:30.000000 idecomp-0.0.8/idecomp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-18 00:44:30.000000 idecomp-0.0.8/idecomp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-05-18 00:44:30.000000 idecomp-0.0.8/idecomp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-05-18 00:44:30.000000 idecomp-0.0.8/idecomp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-18 00:44:30.238346 idecomp-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      938 2021-05-18 00:43:39.000000 idecomp-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 21:09:12.447537 idecomp-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-08-11 21:05:46.000000 idecomp-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2597 2021-08-11 21:09:12.447537 idecomp-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2052 2021-08-11 21:05:46.000000 idecomp-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 21:09:12.443537 idecomp-0.0.9/idecomp/
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2021-08-11 21:05:46.000000 idecomp-0.0.9/idecomp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 21:09:12.447537 idecomp-0.0.9/idecomp/_utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-11 21:05:46.000000 idecomp-0.0.9/idecomp/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1295 2021-08-11 21:05:46.000000 idecomp-0.0.9/idecomp/_utils/arquivo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2088 2021-08-11 21:05:46.000000 idecomp-0.0.9/idecomp/_utils/bloco.py
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2021-08-11 21:05:46.000000 idecomp-0.0.9/idecomp/_utils/dadosarquivo.py
+-rw-r--r--   0 runner    (1001) docker     (121)      574 2021-08-11 21:05:46.000000 idecomp-0.0.9/idecomp/_utils/dadosdadger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1507 2021-08-11 21:05:46.000000 idecomp-0.0.9/idecomp/_utils/escrita.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6617 2021-08-11 21:05:46.000000 idecomp-0.0.9/idecomp/_utils/leitura.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2490 2021-08-11 21:05:46.000000 idecomp-0.0.9/idecomp/_utils/registrodadger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4448 2021-08-11 21:05:46.000000 idecomp-0.0.9/idecomp/_utils/registros.py
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2021-08-11 21:05:46.000000 idecomp-0.0.9/idecomp/_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      732 2021-08-11 21:05:46.000000 idecomp-0.0.9/idecomp/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 21:09:12.447537 idecomp-0.0.9/idecomp/decomp/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-11 21:05:46.000000 idecomp-0.0.9/idecomp/decomp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12424 2021-08-11 21:05:46.000000 idecomp-0.0.9/idecomp/decomp/dadger.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 21:09:12.447537 idecomp-0.0.9/idecomp/decomp/modelos/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-11 21:05:46.000000 idecomp-0.0.9/idecomp/decomp/modelos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    80556 2021-08-11 21:05:46.000000 idecomp-0.0.9/idecomp/decomp/modelos/dadger.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18239 2021-08-11 21:05:46.000000 idecomp-0.0.9/idecomp/decomp/modelos/relato.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4732 2021-08-11 21:05:46.000000 idecomp-0.0.9/idecomp/decomp/relato.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 21:09:12.447537 idecomp-0.0.9/idecomp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2597 2021-08-11 21:09:12.000000 idecomp-0.0.9/idecomp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      671 2021-08-11 21:09:12.000000 idecomp-0.0.9/idecomp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-11 21:09:12.000000 idecomp-0.0.9/idecomp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-08-11 21:09:12.000000 idecomp-0.0.9/idecomp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-08-11 21:09:12.000000 idecomp-0.0.9/idecomp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-11 21:09:12.447537 idecomp-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      938 2021-08-11 21:05:46.000000 idecomp-0.0.9/setup.py
```

### Comparing `idecomp-0.0.8/LICENSE` & `idecomp-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `idecomp-0.0.8/PKG-INFO` & `idecomp-0.0.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,32 @@
-Metadata-Version: 2.1
-Name: idecomp
-Version: 0.0.8
-Summary: Interface para arquivos do DECOMP
-Home-page: https://github.com/rjmalves/idecomp
-Author: Rogerio Alves
-Author-email: rogerioalves.ee@gmail.com
-License: UNKNOWN
-Description: # idecomp
-        
-        [![tests](https://github.com/rjmalves/idecomp/actions/workflows/main.yml/badge.svg)](https://github.com/rjmalves/idecomp/actions/workflows/main.yml)  
-        [![codecov](https://codecov.io/gh/rjmalves/idecomp/branch/main/graph/badge.svg?token=ZSJBGO81JP)](https://codecov.io/gh/rjmalves/idecomp)
-        
-        O *idecomp* é um pacote Python para manipulação dos arquivos
-        de entrada e saída do programa [DECOMP](http://www.cepel.br/pt_br/produtos/decomp-modelo-de-planejamento-da-operacao-de-sistemas-hidrotermicos-interligados-de-curto-prazo.htm),
-        desenvolvido pelo [CEPEL](http://www.cepel.br/) e utilizado para os estudos de planejamento e operação do Sistema Interligado Nacional (SIN).
-        
-        O idecomp oferece:
-        
-        - Meios para leitura dos arquivos de entrada e saída do DECOMP
-        - Armazenamento e processamento de dados otimizados com o uso de [NumPy](https://numpy.org/)
-        - Dados estruturados em modelos com o uso do paradigma de orientação a objetos (OOP)
-        - Utilidades de escritas dos arquivos de entrada do DECOMP para elaboração automatizada de estudos
-        
-        Com *idecomp* é possível ler os arquivos de texto, característicos do DECOMP, e salvar as informações em [pickle](https://docs.python.org/3/library/pickle.html>), 
-        para poupar processamento futuro e reduzir o tempo de execução.
-        
-        ## Instalação
-        
-        O idecomp é compatível com versões de Python >= 3.5. A única dependência formal é o módulo NumPy, que deve sempre ser mantido na versão mais atualizada para a distribuição de Python instalada.
-        
-        Em posse de uma instalação local de Python, é recomendado que se use um ambiente virtual para instalação de módulos de terceiros, sendo que o idecomp não é uma exceção. Para mais detalhes sobre o uso de ambientes virtuais, recomenda-se a leitura do recurso oficial de Python para ambientes virtuais: [venv](https://docs.python.org/3/library/venv.html).
-        
-        ```
-        python -m pip install idecomp
-        ```
-        
-        ## Documentação
-        
-        Guias, tutoriais e as referências podem ser encontrados no site oficial do pacote: https://rjmalves.github.io/idecomp
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 2 - Pre-Alpha
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
+# idecomp
+
+[![tests](https://github.com/rjmalves/idecomp/actions/workflows/main.yml/badge.svg)](https://github.com/rjmalves/idecomp/actions/workflows/main.yml)  
+[![codecov](https://codecov.io/gh/rjmalves/idecomp/branch/main/graph/badge.svg?token=ZSJBGO81JP)](https://codecov.io/gh/rjmalves/idecomp)
+
+O *idecomp* é um pacote Python para manipulação dos arquivos
+de entrada e saída do programa [DECOMP](http://www.cepel.br/pt_br/produtos/decomp-modelo-de-planejamento-da-operacao-de-sistemas-hidrotermicos-interligados-de-curto-prazo.htm),
+desenvolvido pelo [CEPEL](http://www.cepel.br/) e utilizado para os estudos de planejamento e operação do Sistema Interligado Nacional (SIN).
+
+O idecomp oferece:
+
+- Meios para leitura dos arquivos de entrada e saída do DECOMP
+- Armazenamento e processamento de dados otimizados com o uso de [NumPy](https://numpy.org/)
+- Dados estruturados em modelos com o uso do paradigma de orientação a objetos (OOP)
+- Utilidades de escritas dos arquivos de entrada do DECOMP para elaboração automatizada de estudos
+
+Com *idecomp* é possível ler os arquivos de texto, característicos do DECOMP, e salvar as informações em [pickle](https://docs.python.org/3/library/pickle.html>), 
+para poupar processamento futuro e reduzir o tempo de execução.
+
+## Instalação
+
+O idecomp é compatível com versões de Python >= 3.5. A única dependência formal é o módulo NumPy, que deve sempre ser mantido na versão mais atualizada para a distribuição de Python instalada.
+
+Em posse de uma instalação local de Python, é recomendado que se use um ambiente virtual para instalação de módulos de terceiros, sendo que o idecomp não é uma exceção. Para mais detalhes sobre o uso de ambientes virtuais, recomenda-se a leitura do recurso oficial de Python para ambientes virtuais: [venv](https://docs.python.org/3/library/venv.html).
+
+```
+python -m pip install idecomp
+```
+
+## Documentação
+
+Guias, tutoriais e as referências podem ser encontrados no site oficial do pacote: https://rjmalves.github.io/idecomp
```

### Comparing `idecomp-0.0.8/README.md` & `idecomp-0.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: idecomp
+Version: 0.0.9
+Summary: Interface para arquivos do DECOMP
+Home-page: https://github.com/rjmalves/idecomp
+Author: Rogerio Alves
+Author-email: rogerioalves.ee@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 2 - Pre-Alpha
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # idecomp
 
 [![tests](https://github.com/rjmalves/idecomp/actions/workflows/main.yml/badge.svg)](https://github.com/rjmalves/idecomp/actions/workflows/main.yml)  
 [![codecov](https://codecov.io/gh/rjmalves/idecomp/branch/main/graph/badge.svg?token=ZSJBGO81JP)](https://codecov.io/gh/rjmalves/idecomp)
 
 O *idecomp* é um pacote Python para manipulação dos arquivos
 de entrada e saída do programa [DECOMP](http://www.cepel.br/pt_br/produtos/decomp-modelo-de-planejamento-da-operacao-de-sistemas-hidrotermicos-interligados-de-curto-prazo.htm),
@@ -26,7 +43,9 @@
 ```
 python -m pip install idecomp
 ```
 
 ## Documentação
 
 Guias, tutoriais e as referências podem ser encontrados no site oficial do pacote: https://rjmalves.github.io/idecomp
+
+
```

### Comparing `idecomp-0.0.8/idecomp.egg-info/PKG-INFO` & `idecomp-0.0.9/idecomp.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 Metadata-Version: 2.1
 Name: idecomp
-Version: 0.0.8
+Version: 0.0.9
 Summary: Interface para arquivos do DECOMP
 Home-page: https://github.com/rjmalves/idecomp
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 License: UNKNOWN
-Description: # idecomp
-        
-        [![tests](https://github.com/rjmalves/idecomp/actions/workflows/main.yml/badge.svg)](https://github.com/rjmalves/idecomp/actions/workflows/main.yml)  
-        [![codecov](https://codecov.io/gh/rjmalves/idecomp/branch/main/graph/badge.svg?token=ZSJBGO81JP)](https://codecov.io/gh/rjmalves/idecomp)
-        
-        O *idecomp* é um pacote Python para manipulação dos arquivos
-        de entrada e saída do programa [DECOMP](http://www.cepel.br/pt_br/produtos/decomp-modelo-de-planejamento-da-operacao-de-sistemas-hidrotermicos-interligados-de-curto-prazo.htm),
-        desenvolvido pelo [CEPEL](http://www.cepel.br/) e utilizado para os estudos de planejamento e operação do Sistema Interligado Nacional (SIN).
-        
-        O idecomp oferece:
-        
-        - Meios para leitura dos arquivos de entrada e saída do DECOMP
-        - Armazenamento e processamento de dados otimizados com o uso de [NumPy](https://numpy.org/)
-        - Dados estruturados em modelos com o uso do paradigma de orientação a objetos (OOP)
-        - Utilidades de escritas dos arquivos de entrada do DECOMP para elaboração automatizada de estudos
-        
-        Com *idecomp* é possível ler os arquivos de texto, característicos do DECOMP, e salvar as informações em [pickle](https://docs.python.org/3/library/pickle.html>), 
-        para poupar processamento futuro e reduzir o tempo de execução.
-        
-        ## Instalação
-        
-        O idecomp é compatível com versões de Python >= 3.5. A única dependência formal é o módulo NumPy, que deve sempre ser mantido na versão mais atualizada para a distribuição de Python instalada.
-        
-        Em posse de uma instalação local de Python, é recomendado que se use um ambiente virtual para instalação de módulos de terceiros, sendo que o idecomp não é uma exceção. Para mais detalhes sobre o uso de ambientes virtuais, recomenda-se a leitura do recurso oficial de Python para ambientes virtuais: [venv](https://docs.python.org/3/library/venv.html).
-        
-        ```
-        python -m pip install idecomp
-        ```
-        
-        ## Documentação
-        
-        Guias, tutoriais e as referências podem ser encontrados no site oficial do pacote: https://rjmalves.github.io/idecomp
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# idecomp
+
+[![tests](https://github.com/rjmalves/idecomp/actions/workflows/main.yml/badge.svg)](https://github.com/rjmalves/idecomp/actions/workflows/main.yml)  
+[![codecov](https://codecov.io/gh/rjmalves/idecomp/branch/main/graph/badge.svg?token=ZSJBGO81JP)](https://codecov.io/gh/rjmalves/idecomp)
+
+O *idecomp* é um pacote Python para manipulação dos arquivos
+de entrada e saída do programa [DECOMP](http://www.cepel.br/pt_br/produtos/decomp-modelo-de-planejamento-da-operacao-de-sistemas-hidrotermicos-interligados-de-curto-prazo.htm),
+desenvolvido pelo [CEPEL](http://www.cepel.br/) e utilizado para os estudos de planejamento e operação do Sistema Interligado Nacional (SIN).
+
+O idecomp oferece:
+
+- Meios para leitura dos arquivos de entrada e saída do DECOMP
+- Armazenamento e processamento de dados otimizados com o uso de [NumPy](https://numpy.org/)
+- Dados estruturados em modelos com o uso do paradigma de orientação a objetos (OOP)
+- Utilidades de escritas dos arquivos de entrada do DECOMP para elaboração automatizada de estudos
+
+Com *idecomp* é possível ler os arquivos de texto, característicos do DECOMP, e salvar as informações em [pickle](https://docs.python.org/3/library/pickle.html>), 
+para poupar processamento futuro e reduzir o tempo de execução.
+
+## Instalação
+
+O idecomp é compatível com versões de Python >= 3.5. A única dependência formal é o módulo NumPy, que deve sempre ser mantido na versão mais atualizada para a distribuição de Python instalada.
+
+Em posse de uma instalação local de Python, é recomendado que se use um ambiente virtual para instalação de módulos de terceiros, sendo que o idecomp não é uma exceção. Para mais detalhes sobre o uso de ambientes virtuais, recomenda-se a leitura do recurso oficial de Python para ambientes virtuais: [venv](https://docs.python.org/3/library/venv.html).
+
+```
+python -m pip install idecomp
+```
+
+## Documentação
+
+Guias, tutoriais e as referências podem ser encontrados no site oficial do pacote: https://rjmalves.github.io/idecomp
+
+
```

### Comparing `idecomp-0.0.8/setup.py` & `idecomp-0.0.9/setup.py`

 * *Files identical despite different names*

