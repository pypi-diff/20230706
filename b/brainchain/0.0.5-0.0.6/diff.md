# Comparing `tmp/brainchain-0.0.5.tar.gz` & `tmp/brainchain-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainchain-0.0.5.tar", max compression
+gzip compressed data, was "brainchain-0.0.6.tar", max compression
```

## Comparing `brainchain-0.0.5.tar` & `brainchain-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.0.5/brainchain/README.md
--rw-r--r--   0        0        0      104 2023-07-06 16:47:41.411790 brainchain-0.0.5/brainchain/__init__.py
--rw-r--r--   0        0        0     4983 2023-07-05 23:39:12.540065 brainchain-0.0.5/brainchain/brainchain.py
--rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.0.5/brainchain/carnivore.py
--rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.0.5/brainchain/coredata.py
--rw-r--r--   0        0        0     1713 2023-07-06 15:10:07.036695 brainchain-0.0.5/brainchain/example.py
--rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.0.5/brainchain/factcheck.py
--rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.0.5/brainchain/requirements.txt
--rw-r--r--   0        0        0     6351 2023-07-05 20:38:03.247634 brainchain-0.0.5/brainchain/sales_intel.py
--rw-r--r--   0        0        0      530 2023-07-06 16:44:28.277736 brainchain-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 brainchain-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.0.6/brainchain/README.md
+-rw-r--r--   0        0        0      116 2023-07-06 17:41:02.950196 brainchain-0.0.6/brainchain/__init__.py
+-rw-r--r--   0        0        0     5003 2023-07-06 18:14:40.602140 brainchain-0.0.6/brainchain/brainchain.py
+-rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.0.6/brainchain/carnivore.py
+-rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.0.6/brainchain/coredata.py
+-rw-r--r--   0        0        0     1548 2023-07-06 16:58:13.696070 brainchain-0.0.6/brainchain/example.py
+-rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.0.6/brainchain/factcheck.py
+-rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.0.6/brainchain/requirements.txt
+-rw-r--r--   0        0        0       36 2023-07-06 16:49:37.176065 brainchain-0.0.6/brainchain/sales_intel/__init__.py
+-rw-r--r--   0        0        0      228 2023-07-06 16:50:45.249726 brainchain-0.0.6/brainchain/sales_intel/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4629 2023-07-06 16:50:45.250557 brainchain-0.0.6/brainchain/sales_intel/__pycache__/sales_intel.cpython-311.pyc
+-rw-r--r--   0        0        0     6334 2023-07-06 16:50:33.601761 brainchain-0.0.6/brainchain/sales_intel/sales_intel.py
+-rw-r--r--   0        0        0      531 2023-07-06 18:14:55.478527 brainchain-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 brainchain-0.0.6/PKG-INFO
```

### Comparing `brainchain-0.0.5/brainchain/README.md` & `brainchain-0.0.6/brainchain/README.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.0.5/brainchain/brainchain.py` & `brainchain-0.0.6/brainchain/brainchain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,97 +1,99 @@
 import requests
 import os
 import sys
 from urllib.parse import quote
 
-import json, os, requests
+import json
+import os
+import requests
 from urllib.parse import quote
-from sales_intel import SalesIntel
+from sales_intel.sales_intel import SalesIntel
 from factcheck import FactCheck
 
 import requests
 import os
 
+
 class Brainchain:
     def __init__(self, env: str = "prod", api_key: str = os.environ["BRAINCHAIN_API_KEY"], service_url="https://brainchain--agent.modal.run/", salesintel_api_key=os.environ["SALESINTEL_API_KEY"]):
         self.api_key = api_key
         self.env = env
         self.fact_check_instance = FactCheck(environment=env)
         self.sales_intel_client = SalesIntel(salesintel_api_key)
         self.search
         self.environments = ["prod", "dev"]
         self.services = {
             "agent": {
-                "prod" : "https://brainchain--agent.modal.run/",
-                "dev" : "https://brainchain--agent-dev.modal.run/"
+                "prod": "https://brainchain--agent.modal.run/",
+                "dev": "https://brainchain--agent-dev.modal.run/"
             },
             "prompting": {
                 "prod": "https://brainchain--prompting.modal.run/",
                 "dev": "https://brainchain--prompting-dev.modal.run/"
             },
             "pdf_title": {
                 "prod": "https://brainchain--pdf-title.modal.run/",
                 "dev": "https://brainchain--pdf-title-dev.modal.run/"
             },
             "pdf_authors": {
                 "prod": "https://brainchain--pdf-authors.modal.run/",
                 "dev": "https://brainchain--pdf-authors-dev.modal.run/"
             },
-            "search" : {}
+            "search": {}
         }
 
     def fact_check(self, statement):
         return self.fact_check_instance.fact_check(statement)
 
     def search(self, query):
         endpoint = self.services["search"]
 
     def prompt(self, q, history=[], top_p=0.0, system="You are a multi-disciplinary research assistant who formulates, validates, and figures out correct answers. Your insights are ferocious and undeniable. You expand and digest new concepts and relate them to what you already know.", model="gpt-3.5-turbo-16k", presence_penalty=0.0, frequency_penalty=0.0, n=1):
         endpoint = self.services["prompting"][self.env]
         headers = {"Authorization": f"Bearer {self.api_key}"}
-        params = {"user_prompt": q, "history": history, "system_prompt": system, "model": model, "presence_penalty": float(presence_penalty), "frequency_penalty": float(frequency_penalty), "top_p": float(top_p)}
+        params = {"user_prompt": q, "history": history, "system_prompt": system, "model": model, "presence_penalty": float(
+            presence_penalty), "frequency_penalty": float(frequency_penalty), "top_p": float(top_p)}
         response = requests.get(endpoint, headers=headers, params=params)
 
         if response.status_code == 200:
             return response.json()
         else:
             response.raise_for_status()
 
     # Only use text_first_page - MUCH faster! url_link provided for testing across link types
     def obtain_title(self, text_first_page: str = None, url_link: str = None):
         endpoint = self.services["pdf_title"][self.env]
         params = {}
 
         if text_first_page:
             params["document_text"] = text_first_page
-    
+
         if url_link:
             params["url_link"] = url_link
 
         headers = {"Authorization": f"Bearer {self.api_key}"}
         response = requests.post(endpoint, headers=headers, params=params)
         return json.loads(response.content)
 
     # Only use text_first_page - MUCH faster! url_link provided for testing across link types
     def obtain_authors(self, text_first_page: str = None, url_link: str = None):
         endpoint = self.services["pdf_authors"][self.env]
         params = {}
 
         if text_first_page:
             params["document_text"] = text_first_page
-    
+
         if url_link:
             params["url_link"] = url_link
 
         headers = {"Authorization": f"Bearer {self.api_key}"}
         response = requests.post(endpoint, headers=headers, params=params)
         return json.loads(response.content)
 
-
-
     def summon(self, prompt, agent_type="PAE", model="gpt-4-0613", max_tokens=1024, temperature=0.3, top_p=0.3, top_k=0.0, presence_penalty=1.0, frequency_penalty=1.0):
         endpoint = self.services["agent"][self.env]
         headers = {"Authorization": f"Bearer {self.api_key}"}
         params = {
             "prompt": prompt,
             "env": self.env,
             "agent_type": agent_type,
@@ -105,20 +107,19 @@
         }
         response = requests.get(endpoint, headers=headers, params=params)
 
         if response.status_code == 200:
             return response.json()
         else:
             response.raise_for_status()
-    
+
     def get_company(self, **kwargs):
         return self.sales_intel_client.get_company(**kwargs)
 
     def get_people(self, **kwargs):
         return self.sales_intel_client.get_people(**kwargs)
 
     def get_technologies(self, **kwargs):
         return self.sales_intel_client.get_technologies(**kwargs)
 
     def get_news(self, **kwargs):
         return self.sales_intel_client.get_news(**kwargs)
-
```

### Comparing `brainchain-0.0.5/brainchain/carnivore.py` & `brainchain-0.0.6/brainchain/carnivore.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.0.5/brainchain/coredata.py` & `brainchain-0.0.6/brainchain/coredata.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.0.5/brainchain/example.py` & `brainchain-0.0.6/brainchain/example.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,28 +8,23 @@
 from modal import web_endpoint
 import os
 
 image = (
     Image.debian_slim(python_version="3.11")
     .apt_install(["python3-dev", "gcc", "git"])
     .apt_install("libmagic-dev")
-    .pip_install(["bs4", "redis", "numpy", "flask", "typing", "requests", "modal", "psycopg2-binary", "sqlalchemy", "promptlayer", "openai"])
-    .pip_install_private_repos(
-        "github.com/Brainchain-ai/brainchain.py",
-        git_user="arthur-brainchain",
-        secrets=[modal.Secret.from_name("brainchain-prompt-eng")],
-    )
+    .pip_install(["brainchain", "bs4", "redis", "numpy", "flask", "typing", "requests", "modal", "psycopg2-binary", "sqlalchemy", "promptlayer", "openai"])
 )
 
 app = FastAPI()
-stub = Stub("brainchain-citadel", image=image)
+stub = Stub("arthur-example-client-usage", image=image)
 
 
 @stub.function(secret=Secret.from_name("brainchain-prompt-eng"))
-@web_endpoint(method="POST", label="spawn-working")
+@web_endpoint(method="POST", label="spawn-working-2min")
 async def summon_agent(request: Request):
     # Get JSON data from the request
     data = await request.json()
 
     # Extract the 'prompt' field from the JSON data
     prompt = data.get('prompt')
     # Create an instance of the Brainchain client
```

### Comparing `brainchain-0.0.5/brainchain/factcheck.py` & `brainchain-0.0.6/brainchain/factcheck.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.0.5/brainchain/requirements.txt` & `brainchain-0.0.6/brainchain/requirements.txt`

 * *Files identical despite different names*

### Comparing `brainchain-0.0.5/brainchain/sales_intel.py` & `brainchain-0.0.6/brainchain/sales_intel/sales_intel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import requests
 import os
 
+
 class SalesIntel:
     def __init__(self, api_key):
         self.api_key = api_key or os.environ['SALESINTEL_API_KEY']
         self.base_url = "https://api.salesintel.io"
 
-    def get_company(self, company_domain=None, company_industries=None, company_location_states=None, 
-                    company_location_zipcodes=None, company_location_zipcodes_distance=None, 
-                    company_max_revenue=None, company_max_size=None, company_min_revenue=None, 
-                    company_min_size=None, company_naics_codes=None, company_name=None, 
-                    company_sic_codes=None, email=None, first_name=None, is_ev_contact=None, 
+    def get_company(self, company_domain=None, company_industries=None, company_location_states=None,
+                    company_location_zipcodes=None, company_location_zipcodes_distance=None,
+                    company_max_revenue=None, company_max_size=None, company_min_revenue=None,
+                    company_min_size=None, company_naics_codes=None, company_name=None,
+                    company_sic_codes=None, email=None, first_name=None, is_ev_contact=None,
                     is_international=None):
         url = f"{self.base_url}/service/company"
         params = {
             "company_domain": company_domain,
             "company_industries": company_industries,
             "company_location_states": company_location_states,
             "company_location_zipcodes": company_location_zipcodes,
@@ -31,16 +32,16 @@
             "is_ev_contact": is_ev_contact,
             "is_international": is_international
         }
         headers = {"X-CB-ApiKey": f"{self.api_key}"}
         response = requests.get(url, headers=headers, params=params)
         return response.json()
 
-    def get_people(self, first_name=None, last_name=None, location_country_codes=None, page=1, page_size=50, 
-                   sort_by=None, sort_direction=None, tech_category=None, tech_product=None, 
+    def get_people(self, first_name=None, last_name=None, location_country_codes=None, page=1, page_size=50,
+                   sort_by=None, sort_direction=None, tech_category=None, tech_product=None,
                    tech_subcategory=None, tech_vendor=None, verified=None):
         url = f"{self.base_url}/service/people"
         params = {
             "first_name": first_name,
             "last_name": last_name,
             "location_country_codes": location_country_codes,
             "page": page,
@@ -53,23 +54,23 @@
             "tech_vendor": tech_vendor,
             "verified": verified
         }
         headers = {"X-CB-ApiKey": f"{self.api_key}"}
         response = requests.get(url, headers=headers, params=params)
         return response.json()
 
-    def get_technologies(self, company_domain=None, company_industries=None, company_location_states=None, 
-                         company_location_zipcodes=None, company_location_zipcodes_distance=None, 
-                         company_max_revenue=None, company_max_size=None, company_min_revenue=None, 
-                         company_min_size=None, company_naics_codes=None, company_name=None, 
-                         company_sic_codes=None, email=None, first_name=None, is_ev_contact=None, 
-                         is_international=None, job_departments=None, job_levels=None, 
-                         job_sub_departments=None, job_title=None, last_name=None, 
-                         location_country_codes=None, page=1, page_size=50, sort_by=None, 
-                         sort_direction=None, tech_category=None, tech_product=None, 
+    def get_technologies(self, company_domain=None, company_industries=None, company_location_states=None,
+                         company_location_zipcodes=None, company_location_zipcodes_distance=None,
+                         company_max_revenue=None, company_max_size=None, company_min_revenue=None,
+                         company_min_size=None, company_naics_codes=None, company_name=None,
+                         company_sic_codes=None, email=None, first_name=None, is_ev_contact=None,
+                         is_international=None, job_departments=None, job_levels=None,
+                         job_sub_departments=None, job_title=None, last_name=None,
+                         location_country_codes=None, page=1, page_size=50, sort_by=None,
+                         sort_direction=None, tech_category=None, tech_product=None,
                          tech_subcategory=None, tech_vendor=None, verified=None):
         url = f"{self.base_url}/service/technologies"
         params = {
             "company_domain": company_domain,
             "company_industries": company_industries,
             "company_location_states": company_location_states,
             "company_location_zipcodes": company_location_zipcodes,
@@ -101,16 +102,16 @@
             "tech_vendor": tech_vendor,
             "verified": verified
         }
         headers = {"X-CB-ApiKey": f"{self.api_key}"}
         response = requests.get(url, headers=headers, params=params)
         return response.json()
 
-    def get_news(self, last_name=None, location_country_codes=None, page=1, page_size=50, 
-                 sort_by=None, sort_direction=None, tech_category=None, tech_product=None, 
+    def get_news(self, last_name=None, location_country_codes=None, page=1, page_size=50,
+                 sort_by=None, sort_direction=None, tech_category=None, tech_product=None,
                  tech_subcategory=None, tech_vendor=None, verified=None):
         url = f"{self.base_url}/service/news"
         params = {
             "last_name": last_name,
             "location_country_codes": location_country_codes,
             "page": page,
             "page_size": page_size,
```

### Comparing `brainchain-0.0.5/pyproject.toml` & `brainchain-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brainchain"
-version = "0.0.5"
+version = "0.0.6"
 description = "Brainchain API client"
 authors = ["Arthur M. Collé <arthur@brainchain.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = "2.31.0"
 promptlayer = "0.1.90"
@@ -18,8 +18,8 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.source]]
 name = "private"
 url = "https://pypi.org/simple"
-secondary = true
+secondary = true
```

### Comparing `brainchain-0.0.5/PKG-INFO` & `brainchain-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainchain
-Version: 0.0.5
+Version: 0.0.6
 Summary: Brainchain API client
 Author: Arthur M. Collé
 Author-email: arthur@brainchain.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

