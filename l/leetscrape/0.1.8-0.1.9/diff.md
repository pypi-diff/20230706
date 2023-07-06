# Comparing `tmp/leetscrape-0.1.8.tar.gz` & `tmp/leetscrape-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leetscrape-0.1.8.tar", max compression
+gzip compressed data, was "leetscrape-0.1.9.tar", max compression
```

## Comparing `leetscrape-0.1.8.tar` & `leetscrape-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1802 2023-01-19 06:50:11.199911 leetscrape-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5921 2023-01-18 22:54:41.492479 leetscrape-0.1.8/README.md
--rw-r--r--   0        0        0       23 2023-01-19 06:50:23.685761 leetscrape-0.1.8/src/leetscrape/__init__.py
--rw-r--r--   0        0        0     4195 2023-01-18 03:01:14.961902 leetscrape-0.1.8/src/leetscrape/_constants.py
--rw-r--r--   0        0        0     6068 2023-01-18 23:46:55.961974 leetscrape-0.1.8/src/leetscrape/ExtractSolutions.py
--rw-r--r--   0        0        0     9311 2023-01-19 06:48:37.301315 leetscrape-0.1.8/src/leetscrape/GenerateCodeStub.py
--rw-r--r--   0        0        0     4410 2023-01-18 07:05:06.616741 leetscrape-0.1.8/src/leetscrape/GetQuestionInfo.py
--rw-r--r--   0        0        0     7760 2023-01-17 08:00:23.737716 leetscrape-0.1.8/src/leetscrape/GetQuestionsList.py
--rw-r--r--   0        0        0     1680 2023-01-18 22:45:02.559734 leetscrape-0.1.8/src/leetscrape/scripts.py
--rw-r--r--   0        0        0     2944 2023-01-18 22:46:45.225927 leetscrape-0.1.8/src/leetscrape/utils.py
--rw-r--r--   0        0        0     7587 1970-01-01 00:00:00.000000 leetscrape-0.1.8/setup.py
--rw-r--r--   0        0        0     7238 1970-01-01 00:00:00.000000 leetscrape-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1802 2023-01-19 07:36:38.433323 leetscrape-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5921 2023-01-18 22:54:41.492479 leetscrape-0.1.9/README.md
+-rw-r--r--   0        0        0       23 2023-01-19 07:36:59.496818 leetscrape-0.1.9/src/leetscrape/__init__.py
+-rw-r--r--   0        0        0     4195 2023-01-18 03:01:14.961902 leetscrape-0.1.9/src/leetscrape/_constants.py
+-rw-r--r--   0        0        0     6068 2023-01-18 23:46:55.961974 leetscrape-0.1.9/src/leetscrape/ExtractSolutions.py
+-rw-r--r--   0        0        0     9787 2023-01-19 07:34:48.497361 leetscrape-0.1.9/src/leetscrape/GenerateCodeStub.py
+-rw-r--r--   0        0        0     4410 2023-01-18 07:05:06.616741 leetscrape-0.1.9/src/leetscrape/GetQuestionInfo.py
+-rw-r--r--   0        0        0     7760 2023-01-17 08:00:23.737716 leetscrape-0.1.9/src/leetscrape/GetQuestionsList.py
+-rw-r--r--   0        0        0     1680 2023-01-18 22:45:02.559734 leetscrape-0.1.9/src/leetscrape/scripts.py
+-rw-r--r--   0        0        0     2944 2023-01-18 22:46:45.225927 leetscrape-0.1.9/src/leetscrape/utils.py
+-rw-r--r--   0        0        0     7587 1970-01-01 00:00:00.000000 leetscrape-0.1.9/setup.py
+-rw-r--r--   0        0        0     7238 1970-01-01 00:00:00.000000 leetscrape-0.1.9/PKG-INFO
```

### Comparing `leetscrape-0.1.8/pyproject.toml` & `leetscrape-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "leetscrape"
-version = "0.1.8"
+version = "0.1.9"
 description = "Introducing LeetScrape - a powerful and efficient Python package designed to scrape problem statements and their topic and company tags, difficulty, test cases, hints, and code stubs from LeetCode.com. Easily download and save LeetCode problems to your local machine, making it convenient for offline practice and studying. It is perfect for anyone preparing for coding interviews. With the LeetScrape, you can boost your coding skills and improve your chances of landing your dream job."
 authors = ["Nikhil Ravi <nr337@cornell.edu>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/nikhil-ravi/LeetScrape"
 documentation = "https://leetscrape.chowkabhara.com/"
```

### Comparing `leetscrape-0.1.8/README.md` & `leetscrape-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `leetscrape-0.1.8/src/leetscrape/_constants.py` & `leetscrape-0.1.9/src/leetscrape/_constants.py`

 * *Files identical despite different names*

### Comparing `leetscrape-0.1.8/src/leetscrape/ExtractSolutions.py` & `leetscrape-0.1.9/src/leetscrape/ExtractSolutions.py`

 * *Files identical despite different names*

### Comparing `leetscrape-0.1.8/src/leetscrape/GenerateCodeStub.py` & `leetscrape-0.1.9/src/leetscrape/GenerateCodeStub.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 import pandas as pd
 from .utils import camel_case
 import ast
 import marko
 import re
 
 
-def parse_args(args: str) -> dict[str, str]:
+def parse_args(args: str) -> dict:
     """A method to parse the arguments of a python method given in string format.
 
     Args:
         args (str): The arguments of a method in string format.
 
     Returns:
-        dict[str, str]: A dictionary of argument value pairs.
+        dict: A dictionary of argument value pairs.
     """
     args = "f({})".format(args)
     tree = ast.parse(args)
     funccall = tree.body[0].value  # type: ignore
     args = {arg.arg: ast.literal_eval(arg.value) for arg in funccall.keywords}  # type: ignore
     return args  # type: ignore
 
@@ -164,20 +164,33 @@
         parameters = []
         for test in code_blocks:
             if "Input" in test:
                 for line in test.split("\n"):
                     if line.startswith("Input:"):
                         inp = line.split("Input:")[1]
                 parameter_dict = parse_args(inp)  # type: ignore
-                parameter_dict["output"] = re.search("Output: (.*)\n", test).group(1)  # type: ignore
+                parameter_dict["output"] = re.search("Output: (.*)\n", test)
+                if parameter_dict["output"] is not None:
+                    parameter_dict["output"] = parse_args(
+                        parameter_dict["output"]
+                        .group(0)
+                        .replace("Output: ", "Output= ")
+                        .replace("\n", "")
+                    )["Output"]
                 parameters.append(parameter_dict)
+        print(parameters)
         output_string = ", ".join(list(parameters[0].keys()))
         input_string = ", ".join(
             [
-                f"({str(list(parameter.values())).strip('[]')})"
+                ", ".join(
+                    [
+                        "'{}'".format(x) if isinstance(x, str) else str(x)
+                        for x in parameter.values()
+                    ]
+                )
                 for parameter in parameters
             ]
         )
         return input_string, output_string
 
     def create_test_file(self, code_text: str) -> str:
         """Generates the test file for the given question.
```

### Comparing `leetscrape-0.1.8/src/leetscrape/GetQuestionInfo.py` & `leetscrape-0.1.9/src/leetscrape/GetQuestionInfo.py`

 * *Files identical despite different names*

### Comparing `leetscrape-0.1.8/src/leetscrape/GetQuestionsList.py` & `leetscrape-0.1.9/src/leetscrape/GetQuestionsList.py`

 * *Files identical despite different names*

### Comparing `leetscrape-0.1.8/src/leetscrape/scripts.py` & `leetscrape-0.1.9/src/leetscrape/scripts.py`

 * *Files identical despite different names*

### Comparing `leetscrape-0.1.8/src/leetscrape/utils.py` & `leetscrape-0.1.9/src/leetscrape/utils.py`

 * *Files identical despite different names*

### Comparing `leetscrape-0.1.8/setup.py` & `leetscrape-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 entry_points = \
 {'console_scripts': ['leetscrape = leetscrape.scripts:leetscrape_question',
                      'leetupload_solution = '
                      'leetscrape.scripts:leetupload_solution']}
 
 setup_kwargs = {
     'name': 'leetscrape',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Introducing LeetScrape - a powerful and efficient Python package designed to scrape problem statements and their topic and company tags, difficulty, test cases, hints, and code stubs from LeetCode.com. Easily download and save LeetCode problems to your local machine, making it convenient for offline practice and studying. It is perfect for anyone preparing for coding interviews. With the LeetScrape, you can boost your coding skills and improve your chances of landing your dream job.',
     'long_description': '# LeetScrape\n\n[![Python application](https://github.com/nikhil-ravi/LeetcodeScraper/actions/workflows/python-app.yml/badge.svg)](https://github.com/nikhil-ravi/LeetcodeScraper/actions/workflows/python-app.yml) [![deploy-docs](https://github.com/nikhil-ravi/LeetScrape/actions/workflows/deploy-docs.yml/badge.svg)](https://leetscrape.chowkabhara.com) [![PYPI](https://img.shields.io/pypi/v/leetscrape)](https://pypi.org/project/leetscrape/)\n\nIntroducing the LeetScrape - a powerful and efficient Python package designed to scrape problem statements and basic test cases from LeetCode.com. With this package, you can easily download and save LeetCode problems to your local machine, making it convenient for offline practice and studying. It is perfect for software engineers and students preparing for coding interviews. The package is lightweight, easy to use and can be integrated with other tools and IDEs. With the LeetScrape, you can boost your coding skills and improve your chances of landing your dream job.\n\nUse this package to get the list of Leetcode questions, their topic and company tags, difficulty, question body (including test cases, constraints, hints), and code stubs in any of the available programming languages.\n\nDetailed documentation available [here](https://leetscrape.chowkabhara.com/).\n\n## Installation\n\nStart by installing the package from pip or conda:\n```bash\npip install leetscrape\n# or using conda:\nconda install leetscrape\n# or using poetry:\npoetry add leetscrape\n```\n\n\n## Usage\n\n### Command Line\nRun the `leetscrape` command to get a code stub and a pytest test file for a given Leetcode question:\n```bash\n$ leetscrape --titleSlug two-sum --qid 1\n```\nAt least one of the two arguments is required.\n- `titleSlug` is the slug of the leetcode question that is in the url of the question, and\n- `qid` is the number associated with the question.\n\n### Other classes\n\nImport the relevant classes from the package:\n\n```python\nfrom leetscrape.GetQuestionsList import GetQuestionsList\nfrom leetscrape.GetQuestionInfo import GetQuestionInfo\nfrom leetscrape.utils import combine_list_and_info, get_all_questions_body\n```\n\n### Scrape the list of problems\nGet the list of questions, companies, topic tags, categories using the [`GetQuestionsList`](/GetQuestionsList/#getquestionslist) class:\n\n```python\nls = GetQuestionsList()\nls.scrape() # Scrape the list of questions\nls.to_csv(directory_path="../data/") # Save the scraped tables to a directory\n```\n\n### Get Question statement and other information\nQuery individual question\'s information such as the body, test cases, constraints, hints, code stubs, and company tags using the [`GetQuestionInfo`](/GetQuestionsList/#getquestionslist) class:\n\n```python\n# This table can be generated using the previous commnd\nquestions_info = pd.read_csv("../data/questions.csv")\n\n# Scrape question body\nquestions_body_list = get_all_questions_body(\n    questions_info["titleSlug"].tolist(),\n    questions_info["paidOnly"].tolist(),\n    save_to="../data/questionBody.pickle",\n)\n\n# Save to a pandas dataframe\nquestions_body = pd.DataFrame(\n    questions_body_list\n).drop(columns=["titleSlug"])\nquestions_body["QID"] = questions_body["QID"].astype(int)\n```\n\n> **Note**\n> The above code stub is time consuming (10+ minutes) since there are 2500+ questions.\n\nCreate a new dataframe with all the questions and their metadata and body information.\n\n```python\nquestions = combine_list_and_info(\n    info_df = questions_body, list_df=ls.questions, save_to="../data/all.json"\n)\n```\n\n### Upload scraped data to a Database\nCreate a PostgreSQL database using the [SQL](https://github.com/nikhil-ravi/LeetScrape/blob/dcabdd8bd11b03aac0b725c0adc4881b9be9a48f/example/sql/create.sql) dump and insert data using `sqlalchemy`.\n\n```python\nfrom sqlalchemy import create_engine\nfrom sqlalchemy.orm import sessionmaker\n\nengine = create_engine("<database_connection_string>", echo=True)\nquestions.to_sql(con=engine, name="questions", if_exists="append", index=False)\n# Repeat the same for tables ls.topicTags, ls.categories,\n# ls.companies, # ls.questionTopics, and ls.questionCategory\n```\n\nUse the [`queried_questions_list`](https://github.com/nikhil-ravi/LeetScrape/blob/dcabdd8bd11b03aac0b725c0adc4881b9be9a48f/example/sql/create.sql#L228-L240) PostgreSQL function (defined in the SQL dump) to query for questions containy query terms:\n\n```sql\nselect * from queried_questions_list(\'<query term>\');\n```\n\nUse the [`all_questions_list`](https://github.com/nikhil-ravi/LeetScrape/blob/dcabdd8bd11b03aac0b725c0adc4881b9be9a48f/example/sql/create.sql#L243-L253) PostgreSQL function (defined in the SQL dump) to query for all the questions in the database:\n\n```sql\nselect * from all_questions_list();\n```\n\nUse the [`get_similar_questions`](https://github.com/nikhil-ravi/LeetScrape/blob/dcabdd8bd11b03aac0b725c0adc4881b9be9a48f/example/sql/create.sql#L255-L270) PostgreSQL function (defined in the SQL dump) to query for all questions similar to a given question:\n\n```sql\nselect * from get_similar_questions(<QuestionID>);\n```\n\n\n### Extract solutions from a `.py` file\n\nYou may want to extract solutions from a `.py` files to upload them to a database. You can do so using the [`ExtractSolutions`](/src/leetscrape/ExtractSolutions.py) class.\n```python\nfrom leetscrape.ExtractSolutions import extract\n# Returns a dict of the form {QuestionID: solutions}\nsolutions = extract(filename=<path_to_python_script>)\n```\n\nUse the [`upload_solutions`](/utils/#leetscrape.utils.upload_solutions) method to upload the extracted solution code stubs from your python script to the PosgreSQL database.\n\n```python\nfrom leetscrape.ExtractSolutions import upload_solutions\nupload_solutions(engine=<sqlalchemy_engine>, row_id = <row_id_in_table>, solutions: <solutions_dict>)\n```\n',
     'author': 'Nikhil Ravi',
     'author_email': 'nr337@cornell.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/nikhil-ravi/LeetScrape',
```

### Comparing `leetscrape-0.1.8/PKG-INFO` & `leetscrape-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leetscrape
-Version: 0.1.8
+Version: 0.1.9
 Summary: Introducing LeetScrape - a powerful and efficient Python package designed to scrape problem statements and their topic and company tags, difficulty, test cases, hints, and code stubs from LeetCode.com. Easily download and save LeetCode problems to your local machine, making it convenient for offline practice and studying. It is perfect for anyone preparing for coding interviews. With the LeetScrape, you can boost your coding skills and improve your chances of landing your dream job.
 Home-page: https://github.com/nikhil-ravi/LeetScrape
 License: MIT
 Author: Nikhil Ravi
 Author-email: nr337@cornell.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

