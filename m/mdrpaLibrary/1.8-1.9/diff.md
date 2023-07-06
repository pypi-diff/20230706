# Comparing `tmp/mdrpaLibrary-1.8.tar.gz` & `tmp/mdrpaLibrary-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdrpaLibrary-1.8.tar", last modified: Wed Jul  5 17:47:28 2023, max compression
+gzip compressed data, was "mdrpaLibrary-1.9.tar", last modified: Thu Jul  6 11:48:53 2023, max compression
```

## Comparing `mdrpaLibrary-1.8.tar` & `mdrpaLibrary-1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 17:47:28.830843 mdrpaLibrary-1.8/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-05 17:47:28.830631 mdrpaLibrary-1.8/PKG-INFO
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 17:47:28.829249 mdrpaLibrary-1.8/mdrpaLibrary/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:55:03.000000 mdrpaLibrary-1.8/mdrpaLibrary/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3353 2023-07-05 16:14:44.000000 mdrpaLibrary-1.8/mdrpaLibrary/clickButtonModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      491 2023-07-05 17:39:47.000000 mdrpaLibrary-1.8/mdrpaLibrary/getUiModels.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3379 2023-07-05 16:14:55.000000 mdrpaLibrary-1.8/mdrpaLibrary/inputFieldModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1823 2023-07-05 17:46:36.000000 mdrpaLibrary-1.8/mdrpaLibrary/modelDrivenRpa.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3393 2023-07-05 16:14:58.000000 mdrpaLibrary-1.8/mdrpaLibrary/selectCheckboxModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3449 2023-07-05 16:15:00.000000 mdrpaLibrary-1.8/mdrpaLibrary/selectFromDropdownModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      863 2023-07-05 16:13:32.000000 mdrpaLibrary-1.8/mdrpaLibrary/sendReportModel.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 17:47:28.830346 mdrpaLibrary-1.8/mdrpaLibrary/utils/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 mdrpaLibrary-1.8/mdrpaLibrary/utils/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2484 2023-07-05 16:13:57.000000 mdrpaLibrary-1.8/mdrpaLibrary/utils/utils.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 17:47:28.829959 mdrpaLibrary-1.8/mdrpaLibrary.egg-info/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-05 17:47:28.000000 mdrpaLibrary-1.8/mdrpaLibrary.egg-info/PKG-INFO
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      489 2023-07-05 17:47:28.000000 mdrpaLibrary-1.8/mdrpaLibrary.egg-info/SOURCES.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-05 17:47:28.000000 mdrpaLibrary-1.8/mdrpaLibrary.egg-info/dependency_links.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       13 2023-07-05 17:47:28.000000 mdrpaLibrary-1.8/mdrpaLibrary.egg-info/top_level.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-05 17:47:28.830905 mdrpaLibrary-1.8/setup.cfg
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      193 2023-07-05 17:47:04.000000 mdrpaLibrary-1.8/setup.py
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 11:48:53.974649 mdrpaLibrary-1.9/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-06 11:48:53.974463 mdrpaLibrary-1.9/PKG-INFO
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 11:48:53.972991 mdrpaLibrary-1.9/mdrpaLibrary/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 11:24:56.000000 mdrpaLibrary-1.9/mdrpaLibrary/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3325 2023-07-06 11:19:01.000000 mdrpaLibrary-1.9/mdrpaLibrary/clickButtonModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      491 2023-07-05 17:39:47.000000 mdrpaLibrary-1.9/mdrpaLibrary/getUiModels.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3352 2023-07-06 11:19:23.000000 mdrpaLibrary-1.9/mdrpaLibrary/inputFieldModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1871 2023-07-06 11:47:58.000000 mdrpaLibrary-1.9/mdrpaLibrary/modelDrivenRpa.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3366 2023-07-06 11:20:06.000000 mdrpaLibrary-1.9/mdrpaLibrary/selectCheckboxModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3425 2023-07-06 11:20:26.000000 mdrpaLibrary-1.9/mdrpaLibrary/selectFromDropdownModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      863 2023-07-06 11:20:30.000000 mdrpaLibrary-1.9/mdrpaLibrary/sendReportModel.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 11:48:53.974145 mdrpaLibrary-1.9/mdrpaLibrary/utils/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 mdrpaLibrary-1.9/mdrpaLibrary/utils/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2484 2023-07-05 16:13:57.000000 mdrpaLibrary-1.9/mdrpaLibrary/utils/utils.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 11:48:53.973772 mdrpaLibrary-1.9/mdrpaLibrary.egg-info/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-06 11:48:53.000000 mdrpaLibrary-1.9/mdrpaLibrary.egg-info/PKG-INFO
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      489 2023-07-06 11:48:53.000000 mdrpaLibrary-1.9/mdrpaLibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-06 11:48:53.000000 mdrpaLibrary-1.9/mdrpaLibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       13 2023-07-06 11:48:53.000000 mdrpaLibrary-1.9/mdrpaLibrary.egg-info/top_level.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-06 11:48:53.974700 mdrpaLibrary-1.9/setup.cfg
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      193 2023-07-06 11:48:22.000000 mdrpaLibrary-1.9/setup.py
```

### Comparing `mdrpaLibrary-1.8/mdrpaLibrary/clickButtonModel.robot` & `mdrpaLibrary-1.9/mdrpaLibrary/clickButtonModel.robot`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     Set Suite Variable  ${page_name}    ${page} 
     Set Suite Variable  ${element_name}   ${ui_element}
     Set Suite Variable  ${element}  ${EMPTY}
     ${response}=  Set UI Element  ${model_name}   ${page_name}  ${element_name}   ${models}   
     Set Suite Variable  ${element}   ${response} 
     Set Suite Variable  ${current_mode}   ${element["current_mode"]} 
     Set Suite Variable  ${element_locators}     ${element["element_locators"]} 
-    @{keyword_list}=    Create List    Click Button By ID    Click Button By Path    Click Button By Label   Click Button By Image
+    @{keyword_list}=    Create List    Click Button By ID    Click Button By Path    Click Button By Label  
 
    
     ${id}=   Get ID From Attributes  ${element_locators["dom"]["attributes"]}
     Set Suite Variable  ${id}
     Set Suite Variable  ${path}   ${element_locators["dom"]["path"]}
     Set Suite Variable  ${text}   ${element_locators["dom"]["text"]}
     Set Suite Variable  ${image}  ${element_locators["surface"]["image"]}
@@ -50,26 +50,26 @@
        Run Keyword If    '${interaction_status}' == 'Fail'    ${keyword}    
     END
    
     
 Click Button By ID
     ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    id=${id}
     Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND  Click Element    id=${id}
-    ...  ELSE    Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  'id'
+    ...  ELSE    Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  id
     
 
 Click Button By Path
     ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    xpath=${path}
     Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND  Click Element    xpath=${path}
-    ...  ELSE  Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  'path'
+    ...  ELSE  Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  path
 
 Click Button By Label
     ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    xpath=//a[text()='${text}']
     Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND  Click Element   xpath=//a[text()='${text}']
-    ...  ELSE    Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  'text'
+    ...  ELSE    Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  text
 
 
 
 # The below keywords are to get a specific UI Element from the model
```

### Comparing `mdrpaLibrary-1.8/mdrpaLibrary/inputFieldModel.robot` & `mdrpaLibrary-1.9/mdrpaLibrary/inputFieldModel.robot`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Set Suite Variable  ${element_name}  ${ui_element} 
     Set Suite Variable  ${models}    ${model} 
     Set Suite Variable  ${element}  ${EMPTY}
     ${response}=  Set UI Element  ${model_name}   ${page_name}  ${element_name}   ${model}   
     Set Suite Variable  ${element}   ${response} 
     Set Suite Variable  ${current_mode}   ${element["current_mode"]} 
     Set Suite Variable  ${element_locators}     ${element["element_locators"]} 
-    @{keyword_list}=    Create List     Input Field By ID    Input Field By Path    Input Field By Label   Input Field By Image
+    @{keyword_list}=    Create List     Input Field By ID    Input Field By Path    Input Field By Label  
 
     ${id}=   Get ID From Attributes  ${element_locators["dom"]["attributes"]}
     Set Suite Variable  ${id}
     Set Suite Variable  ${path}   ${element_locators["dom"]["path"]}
     Set Suite Variable  ${text}   ${element_locators["dom"]["text"]}
     Set Suite Variable  ${image}  ${element_locators["surface"]["image"]}
     Set Suite Variable  ${value}
@@ -47,26 +47,26 @@
     FOR    ${keyword}    IN    @{keyword_list}
        Run Keyword If    '${interaction_status}' == 'Fail'    ${keyword}    
     END
 
 Input Field By ID
     ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    id=${id}
     Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND    Input Text  id=${id}    ${value}     
-    ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  'id'
+    ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  id
     
 
 Input Field By Path
     ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    xpath=${path}
     Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND   Input Text  xpath=${path}    ${value}      
-    ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  'path'
+    ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  path
 
 Input Field By Label
     ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    xpath=//a[text()='${text}']
     Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND   Input Text   xpath=//a[text()='${text}']  ${value} 
-    ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  'text'
+    ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  text
```

### Comparing `mdrpaLibrary-1.8/mdrpaLibrary/modelDrivenRpa.py` & `mdrpaLibrary-1.9/mdrpaLibrary/modelDrivenRpa.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
             'selectFromDropdownModel.robot',
             'getUiModels.robot',
             'sendReportModel.robot'
         ]  
 
     def import_resource_file(self, resource_file):
         file_path = os.path.join(self.resource_dir, resource_file)
+        file_path = os.path.normpath(file_path)
         self.builtin.import_resource(file_path)
 
 
 
     @keyword
     def click_button_model(self, *args):
         self.import_resource_file(self.resource_files[0])
```

### Comparing `mdrpaLibrary-1.8/mdrpaLibrary/selectCheckboxModel.robot` & `mdrpaLibrary-1.9/mdrpaLibrary/selectCheckboxModel.robot`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     Set Suite Variable  ${element_name}    ${ui_element} 
     Set Suite Variable  ${models}    ${model} 
     Set Suite Variable  ${element}  ${EMPTY}
     ${response}=  Set UI Element  ${model_name}   ${page_name}  ${element_name}   ${model}   
     Set Suite Variable  ${element}   ${response} 
     Set Suite Variable  ${current_mode}   ${element["current_mode"]} 
     Set Suite Variable  ${element_locators}     ${element["element_locators"]} 
-    @{keyword_list}=    Create List     Select Checkbox By ID     Select Checkbox By Path     Select Checkbox By Label    Select Checkbox By Image
+    @{keyword_list}=    Create List     Select Checkbox By ID     Select Checkbox By Path     Select Checkbox By Label    
 
     ${id}=   Get ID From Attributes  ${element_locators["dom"]["attributes"]}
     Set Suite Variable  ${id}
     Set Suite Variable  ${path}   ${element_locators["dom"]["path"]}
     Set Suite Variable  ${text}   ${element_locators["dom"]["text"]}
     Set Suite Variable  ${image}  ${element_locators["surface"]["image"]}
     Set Suite Variable  ${value}
@@ -49,26 +49,26 @@
     END
 
 
 
 Select Checkbox By ID
     ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    id=${id}
     Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND    Select Checkbox  id=${id}    
-    ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  'id'
+    ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}   id
     
 
 Select Checkbox By Path
     ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    xpath=${path}
     Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND   Select Checkbox  xpath=${path}       
-    ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  'path'
+    ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}   path
 
 Select Checkbox By Label
     ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    xpath=//a[text()='${text}']
     Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND   Select Checkbox   xpath=//a[text()='${text}']  
-    ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  'text'
+    ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}   text
```

### Comparing `mdrpaLibrary-1.8/mdrpaLibrary/selectFromDropdownModel.robot` & `mdrpaLibrary-1.9/mdrpaLibrary/selectFromDropdownModel.robot`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Set Suite Variable  ${element_name}   ${ui_element}
     Set Suite Variable  ${models}    ${model} 
     Set Suite Variable  ${element}  ${EMPTY}
     ${response}=  Set UI Element  ${model_name}   ${page_name}  ${element_name}   ${model} 
     Set Suite Variable  ${element}   ${response} 
     Set Suite Variable  ${current_mode}   ${element["current_mode"]} 
     Set Suite Variable  ${element_locators}     ${element["element_locators"]} 
-    @{keyword_list}=    Create List     Select Value By ID     Select Value By Path     Select Value By Label    Select Value By Image
+    @{keyword_list}=    Create List     Select Value By ID     Select Value By Path     Select Value By Label    
 
     ${id}=   Get ID From Attributes  ${element_locators["dom"]["attributes"]}
     Set Suite Variable  ${id}
     Set Suite Variable  ${path}   ${element_locators["dom"]["path"]}
     Set Suite Variable  ${text}   ${element_locators["dom"]["text"]}
     Set Suite Variable  ${image}  ${element_locators["surface"]["image"]}
     Set Suite Variable  ${value}
@@ -48,26 +48,26 @@
     END
 
 
 
 Select Value By ID
     ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    id=${id}
     Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable  ${interaction_status}  Pass  AND    Select From List by Value  id=${id}    ${value}     
-    ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  'id'
+    ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}   id
     
 
 Select Value By Path
     ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    xpath=${path}
     Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND   Select From List by Value  xpath=${path}    ${value}      
-    ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  'path'
+    ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}   path
 
 Select Value By Label
     ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    xpath=//a[text()='${text}']
     Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND   Select From List by Value   xpath=//a[text()='${text}']  ${value} 
-    ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  'text'
+    ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}   text
```

### Comparing `mdrpaLibrary-1.8/mdrpaLibrary/sendReportModel.robot` & `mdrpaLibrary-1.9/mdrpaLibrary/sendReportModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-1.8/mdrpaLibrary/utils/utils.robot` & `mdrpaLibrary-1.9/mdrpaLibrary/utils/utils.robot`

 * *Files identical despite different names*

