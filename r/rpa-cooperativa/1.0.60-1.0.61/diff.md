# Comparing `tmp/rpa_cooperativa-1.0.60.tar.gz` & `tmp/rpa_cooperativa-1.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.60.tar", last modified: Mon Jul  3 13:04:13 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.61.tar", last modified: Thu Jul  6 12:12:37 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.60.tar` & `rpa_cooperativa-1.0.61.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 13:04:13.671739 rpa_cooperativa-1.0.60/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.60/LICENSE
--rw-rw-rw-   0        0        0     6875 2023-07-03 13:04:13.663749 rpa_cooperativa-1.0.60/PKG-INFO
--rw-rw-rw-   0        0        0     5730 2023-05-19 18:58:05.000000 rpa_cooperativa-1.0.60/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 13:04:13.394221 rpa_cooperativa-1.0.60/rpa_coop/
--rw-rw-rw-   0        0        0      585 2023-05-22 15:25:02.000000 rpa_cooperativa-1.0.60/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 13:04:13.604206 rpa_cooperativa-1.0.60/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.60/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.60/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.60/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.60/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.60/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.60/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.60/rpa_coop/img/siac_branco.PNG
--rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.60/rpa_coop/img/siat_amarelo.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.60/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.60/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.60/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0    88164 2023-06-23 12:22:08.000000 rpa_cooperativa-1.0.60/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-07-03 13:04:13.653069 rpa_cooperativa-1.0.60/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     6875 2023-07-03 13:04:12.000000 rpa_cooperativa-1.0.60/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-07-03 13:04:12.000000 rpa_cooperativa-1.0.60/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 13:04:12.000000 rpa_cooperativa-1.0.60/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-03 13:04:12.000000 rpa_cooperativa-1.0.60/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      581 2023-07-03 13:04:12.000000 rpa_cooperativa-1.0.60/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-03 13:04:12.000000 rpa_cooperativa-1.0.60/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 13:04:13.674347 rpa_cooperativa-1.0.60/setup.cfg
--rw-rw-rw-   0        0        0     2350 2023-07-03 12:40:46.000000 rpa_cooperativa-1.0.60/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:12:37.029126 rpa_cooperativa-1.0.61/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.61/LICENSE
+-rw-rw-rw-   0        0        0     6875 2023-07-06 12:12:37.022172 rpa_cooperativa-1.0.61/PKG-INFO
+-rw-rw-rw-   0        0        0     5730 2023-05-19 18:58:05.000000 rpa_cooperativa-1.0.61/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 12:12:36.753613 rpa_cooperativa-1.0.61/rpa_coop/
+-rw-rw-rw-   0        0        0      585 2023-05-22 15:25:02.000000 rpa_cooperativa-1.0.61/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:12:36.964964 rpa_cooperativa-1.0.61/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.61/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.61/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.61/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.61/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.61/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.61/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.61/rpa_coop/img/siac_branco.PNG
+-rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.61/rpa_coop/img/siat_amarelo.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.61/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.61/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.61/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0    88529 2023-07-06 12:10:26.000000 rpa_cooperativa-1.0.61/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:12:37.017001 rpa_cooperativa-1.0.61/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6875 2023-07-06 12:12:35.000000 rpa_cooperativa-1.0.61/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-07-06 12:12:35.000000 rpa_cooperativa-1.0.61/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 12:12:35.000000 rpa_cooperativa-1.0.61/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-06 12:12:35.000000 rpa_cooperativa-1.0.61/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      581 2023-07-06 12:12:35.000000 rpa_cooperativa-1.0.61/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 12:12:35.000000 rpa_cooperativa-1.0.61/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 12:12:37.030126 rpa_cooperativa-1.0.61/setup.cfg
+-rw-rw-rw-   0        0        0     2350 2023-07-06 11:58:56.000000 rpa_cooperativa-1.0.61/setup.py
```

### Comparing `rpa_cooperativa-1.0.60/LICENSE` & `rpa_cooperativa-1.0.61/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.60/PKG-INFO` & `rpa_cooperativa-1.0.61/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa_cooperativa
-Version: 1.0.60
+Version: 1.0.61
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.60/README.md` & `rpa_cooperativa-1.0.61/README.md`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.60/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.61/rpa_coop/__init__.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.60/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.61/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.60/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.61/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.60/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.61/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.60/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.61/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.60/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.61/rpa_coop/rpa_coop.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,19 @@
         self.pw_bd_grafana = str(urllib.parse.quote_plus(gerador_pwd('grafana', 'senha')))
         
         self.ip_sistema_senhas = str(gerador_pwd('sistema_senhas', 'ip_host'))
         self.user_sistema_senhas = str(gerador_pwd('sistema_senhas', 'usuario'))
         self.database_sistema_senhas = str(gerador_pwd('sistema_senhas', 'db_name'))
         self.pw_bd_sistema_senhas = str(urllib.parse.quote_plus(gerador_pwd('sistema_senhas', 'senha')))
         
+        self.ip_db_sapiens = str(gerador_pwd('pw_bd_sapiens', 'ip_host'))
+        self.db_sapiens = str(gerador_pwd('pw_bd_sapiens', 'db_name'))
+        self.pw_db_sapiens = str(gerador_pwd('pw_bd_sapiens', 'senha'))
+        self.user_db_sapiens = str(gerador_pwd('pw_bd_sapiens', 'usuario'))
+        
         self.ip_denodo = str(gerador_pwd('denodo_web', 'ip_host'))
         self.user_denodo = str(gerador_pwd('denodo_web', 'usuario'))
         self.pw_denodo = str(urllib.parse.quote_plus(gerador_pwd('denodo_web', 'senha')))
         
         self.token_api_denodo = str(gerador_pwd('token_api_denodo', 'senha'))
         self.url_api_denodo = str(gerador_pwd('token_api_denodo', 'ip_host'))
 
@@ -162,15 +167,16 @@
         elif (db == 'ldw') or (db == 'seguros') or (db == 'cooperativa') or (db == 'auditoria_7000'):
             conexao = create_engine(f'denodo://{self.user_denodo}:{self.pw_denodo}@{self.ip_denodo}:9996/{db}')
         elif (db == 'grafana'):
             conexao = create_engine(f'mysql+mysqlconnector://{self.user_grafana}:{self.pw_bd_grafana}@{self.ip_grafana}/{db}')
         elif (db == 'sistema_senhas'):
             banco = self.database_sistema_senhas
             conexao = create_engine(f'mysql+mysqlconnector://{self.user_sistema_senhas}:{self.pw_bd_sistema_senhas}@{self.ip_sistema_senhas}:3307/{banco}')
-            # conexao = mysql.connect(host=self.ip_sistema_senhas, port=3307, database=banco, user=self.user_sistema_senhas, password=self.pw_bd_sistema_senhas)
+        elif (db == 'sapiens') or (db == 'sap') or (db == 'fiori'):
+            conexao = create_engine(f"mssql+pymssql://{self.user_db_sapiens}:{self.pw_db_sapiens}@{self.ip_db_sapiens}")
         else:
             conexao = create_engine(f'mysql+{library_sql}://{user_db}:{password_db}@{ip_ou_host_db}:{porta}/{db}')
         return conexao
             
                          
     def criar_conexao(self, db:str, user_db='user_opcional', password_db='senha_opcional', ip_ou_host_db='ip_host_opcional', porta='3306', library_sql='mysqlconnector'):
         '''
@@ -188,15 +194,16 @@
         elif (db == 'ldw') or (db == 'seguros') or (db == 'cooperativa') or (db == 'auditoria_7000'):
             conexao = create_engine(f'denodo://{self.user_denodo}:{self.pw_denodo}@{self.ip_denodo}:9996/{db}')
         elif (db == 'grafana'):
             conexao = create_engine(f'mysql+mysqlconnector://{self.user_grafana}:{self.pw_bd_grafana}@{self.ip_grafana}/{db}')
         elif (db == 'sistema_senhas'):
             banco = self.database_sistema_senhas
             conexao = create_engine(f'mysql+mysqlconnector://{self.user_sistema_senhas}:{self.pw_bd_sistema_senhas}@{self.ip_sistema_senhas}:3307/{banco}')
-            # conexao = mysql.connect(host=self.ip_sistema_senhas, port=3307, database=banco, user=self.user_sistema_senhas, password=self.pw_bd_sistema_senhas)
+        elif (db == 'sapiens') or (db == 'sap') or (db == 'fiori'):
+            conexao = create_engine(f"mssql+pymssql://{self.user_db_sapiens}:{self.pw_db_sapiens}@{self.ip_db_sapiens}")
         else:
             conexao = create_engine(f'mysql+{library_sql}://{user_db}:{password_db}@{ip_ou_host_db}:{porta}/{db}')
         return conexao
             
         
     def api_consulta_denodo(self, database:str, tabela:str, colunas:str, filtro_where="opcional"):
         '''
```

### Comparing `rpa_cooperativa-1.0.60/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.61/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-cooperativa
-Version: 1.0.60
+Version: 1.0.61
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.60/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.61/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.60/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.61/rpa_cooperativa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.60/setup.py` & `rpa_cooperativa-1.0.61/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.60",
+    version="1.0.61",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
```

