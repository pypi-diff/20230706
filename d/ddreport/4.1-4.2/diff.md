# Comparing `tmp/ddreport-4.1.tar.gz` & `tmp/ddreport-4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddreport-4.1.tar", last modified: Thu Jun  8 08:38:22 2023, max compression
+gzip compressed data, was "ddreport-4.2.tar", last modified: Thu Jul  6 06:48:46 2023, max compression
```

## Comparing `ddreport-4.1.tar` & `ddreport-4.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 08:38:22.878338 ddreport-4.1/
--rw-rw-rw-   0        0        0       27 2022-11-03 01:34:06.000000 ddreport-4.1/MANIFEST.in
--rw-rw-rw-   0        0        0      437 2023-06-08 08:38:22.878338 ddreport-4.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-08 08:38:22.811053 ddreport-4.1/ddreport/
--rw-rw-rw-   0        0        0        0 2022-11-02 07:43:40.000000 ddreport-4.1/ddreport/__init__.py
--rw-rw-rw-   0        0        0     8128 2023-06-08 08:30:41.000000 ddreport-4.1/ddreport/api.py
--rw-rw-rw-   0        0        0     2554 2023-04-27 06:51:09.000000 ddreport-4.1/ddreport/db.py
--rw-rw-rw-   0        0        0      389 2023-04-22 12:51:35.000000 ddreport-4.1/ddreport/exceptd.py
--rw-rw-rw-   0        0        0     4039 2023-06-08 08:05:35.000000 ddreport-4.1/ddreport/func.py
--rw-rw-rw-   0        0        0     2016 2023-05-04 09:10:09.000000 ddreport-4.1/ddreport/handle.py
--rw-rw-rw-   0        0        0     1175 2023-03-08 10:44:46.000000 ddreport-4.1/ddreport/orm.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:38:22.875345 ddreport-4.1/ddreport/template/
--rw-rw-rw-   0        0        0    20482 2023-04-28 01:19:06.000000 ddreport-4.1/ddreport/template/index.html
--rw-rw-rw-   0        0        0    11672 2023-06-08 08:03:55.000000 ddreport-4.1/ddreport/testReport.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:38:22.839039 ddreport-4.1/ddreport.egg-info/
--rw-rw-rw-   0        0        0      437 2023-06-08 08:38:22.000000 ddreport-4.1/ddreport.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-06-08 08:38:22.000000 ddreport-4.1/ddreport.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 08:38:22.000000 ddreport-4.1/ddreport.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-08 08:38:22.000000 ddreport-4.1/ddreport.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-06-08 08:38:22.000000 ddreport-4.1/ddreport.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-08 08:38:22.000000 ddreport-4.1/ddreport.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 08:38:22.878338 ddreport-4.1/setup.cfg
--rw-rw-rw-   0        0        0     1562 2023-06-08 08:37:51.000000 ddreport-4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:48:46.959392 ddreport-4.2/
+-rw-rw-rw-   0        0        0       27 2022-11-03 01:34:06.000000 ddreport-4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      450 2023-07-06 06:48:46.958387 ddreport-4.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-06 06:48:46.927670 ddreport-4.2/ddreport/
+-rw-rw-rw-   0        0        0        0 2023-06-08 08:39:13.000000 ddreport-4.2/ddreport/__init__.py
+-rw-rw-rw-   0        0        0     8917 2023-07-06 02:19:40.000000 ddreport-4.2/ddreport/api.py
+-rw-rw-rw-   0        0        0     2747 2023-06-14 08:29:51.000000 ddreport-4.2/ddreport/db.py
+-rw-rw-rw-   0        0        0      389 2023-06-08 08:39:13.000000 ddreport-4.2/ddreport/exceptd.py
+-rw-rw-rw-   0        0        0     4039 2023-06-08 08:39:13.000000 ddreport-4.2/ddreport/func.py
+-rw-rw-rw-   0        0        0     2016 2023-06-08 08:39:13.000000 ddreport-4.2/ddreport/handle.py
+-rw-rw-rw-   0        0        0     1175 2023-06-08 08:39:13.000000 ddreport-4.2/ddreport/orm.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:48:46.957469 ddreport-4.2/ddreport/template/
+-rw-rw-rw-   0        0        0    20794 2023-07-06 06:48:26.000000 ddreport-4.2/ddreport/template/index.html
+-rw-rw-rw-   0        0        0    11627 2023-06-20 03:30:45.000000 ddreport-4.2/ddreport/testReport.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:48:46.954720 ddreport-4.2/ddreport.egg-info/
+-rw-rw-rw-   0        0        0      450 2023-07-06 06:48:46.000000 ddreport-4.2/ddreport.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-07-06 06:48:46.000000 ddreport-4.2/ddreport.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 06:48:46.000000 ddreport-4.2/ddreport.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-06 06:48:46.000000 ddreport-4.2/ddreport.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-07-06 06:48:46.000000 ddreport-4.2/ddreport.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 06:48:46.000000 ddreport-4.2/ddreport.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 06:48:46.959392 ddreport-4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1575 2023-07-06 06:44:20.000000 ddreport-4.2/setup.py
```

### Comparing `ddreport-4.1/ddreport/api.py` & `ddreport-4.2/ddreport/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,15 +108,15 @@
                 E.msg_dict = dict(ass_item=assert_item, row=n + 1)
                 ExceptInfo(Q, E).raised()
             if assert_item.get("type").upper() == 'TEXT':
                 if assert_item.get("value") not in r.text:
                     E.typed = 21                                                                        # TEXT匹配失败
                     E.msg_dict = dict(ass_item=assert_item, row=n + 1, expect_value=assert_item.get("value"))
                     ExceptInfo(Q, E).raised()
-            elif assert_item.get("type").upper() in ['JSON', 'JSON_BOOL', 'JSON_LEN']:
+            elif assert_item.get("type").upper() in ['JSON', 'JSON_BOOL', 'JSON_IN', 'JSON_CONTAIN', 'JSON_LEN']:
                 if is_json is False:
                     E.typed = 14                                                                        # 响应类型不是json
                     E.msg_dict = dict(ass_item=assert_item, row=n + 1)
                     ExceptInfo(Q, E).raised()
                 results = jsonpath(r.json(), assert_item.get('exp')) or []
                 result = results[0] if len(results) == 1 else results
                 if assert_item.get("type").upper() == "JSON":
@@ -125,14 +125,24 @@
                         E.msg_dict = dict(ass_item=assert_item, row=n + 1, expect_value=assert_item.get("value"), actual_value=result)
                         ExceptInfo(Q, E).raised()
                 elif assert_item.get("type").upper() == "JSON_BOOL":
                     if bool(result) != assert_item.get("value"):
                         E.typed = 22                                                                    # JSON匹配失败
                         E.msg_dict = dict(ass_item=assert_item, row=n + 1, expect_value=assert_item.get("value"), actual_value=result)
                         ExceptInfo(Q, E).raised()
+                elif assert_item.get("type").upper() == "JSON_IN":
+                    if result not in assert_item.get("value"):
+                        E.typed = 22  # JSON匹配失败
+                        E.msg_dict = dict(ass_item=assert_item, row=n + 1, expect_value=assert_item.get("value"), actual_value=result)
+                        ExceptInfo(Q, E).raised()  
+                elif assert_item.get("type").upper() == "JSON_CONTAIN":
+                    if assert_item.get("value") not in result:
+                        E.typed = 22  # JSON匹配失败
+                        E.msg_dict = dict(ass_item=assert_item, row=n + 1, expect_value=assert_item.get("value"), actual_value=result)
+                        ExceptInfo(Q, E).raised() 
                 else:
                     try:
                         length = len(result)
                     except Exception:
                         length = None
                     if length != assert_item.get("value"):
                         E.typed = 22                                                                    # JSON匹配失败
```

### Comparing `ddreport-4.1/ddreport/db.py` & `ddreport-4.2/ddreport/db.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 import pymysql
 from sshtunnel import SSHTunnelForwarder
 
 
 
 class PytestMysql:
-    def __init__(self, db, db_ssh=None):
-        self.__SSH = False
-        if db_ssh:
+    def __init__(self, db_config):
+        if db_config and db_config.get('ssh'):
             self.__SSH = True
-            ssh_address_or_host, ssh_username = (db_ssh["host"], db_ssh['port']), db_ssh['user']
-            remote_bind_address = (db['host'], db['port'])
+            db_ssh = db_config.get('ssh')
+            ssh_address_or_host = (db_ssh["host"], db_ssh['port'])
+            ssh_username = db_ssh['user']
+            remote_bind_address = (db_config['host'], db_config['port'])
             ssh_db_config = {"ssh_address_or_host": ssh_address_or_host, "ssh_username": ssh_username, "remote_bind_address": remote_bind_address}
             if db_ssh.get('password'):
                 ssh_db_config['ssh_password'] = db_ssh.get('password')
             else:
                 ssh_db_config['ssh_pkey'] = db_ssh.get('pkey') or None
             self.__server = SSHTunnelForwarder(**ssh_db_config)
-        self.__condb(db)
+            del db_config['ssh']
+        else:
+            self.__SSH = False
+        self.__dbConnect(db_config)
 
-    def __condb(self, db):
+    def __dbConnect(self, db_config):
         try:
-            data = {**db, **{'charset': 'utf8', 'cursorclass': pymysql.cursors.DictCursor, 'autocommit': True}}
+            data = {'charset': 'utf8', 'cursorclass': pymysql.cursors.DictCursor, 'autocommit': True}
+            data.update(db_config)
             if self.__SSH is True:
                 self.__server.start()
                 data['host'], data['port'] = "127.0.0.1", self.__server.local_bind_port  # 重新赋值
             self.__conn = pymysql.connect(**data)
             self.__conn.ping(reconnect=True)
             self.__cursor = self.__conn.cursor()
         except Exception:
```

### Comparing `ddreport-4.1/ddreport/func.py` & `ddreport-4.2/ddreport/func.py`

 * *Files identical despite different names*

### Comparing `ddreport-4.1/ddreport/handle.py` & `ddreport-4.2/ddreport/handle.py`

 * *Files identical despite different names*

### Comparing `ddreport-4.1/ddreport/orm.py` & `ddreport-4.2/ddreport/orm.py`

 * *Files identical despite different names*

### Comparing `ddreport-4.1/ddreport/template/index.html` & `ddreport-4.2/ddreport/template/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -44,22 +44,22 @@
 
     .row-expand {
         background-color: #f5f5f5;
         padding: 10px;
     }
 
     .block {
-  padding: 30px 0;
-  text-align: center;
-  border-right: solid 1px var(--el-border-color);
-  display: inline-block;
-  width: 49%;
-  box-sizing: border-box;
-  vertical-align: top;
-}
+        padding: 30px 0;
+        text-align: center;
+        border-right: solid 1px #E9EBF0;
+        display: inline-block;
+        width: 49%;
+        box-sizing: border-box;
+        vertical-align: top;
+    }
 
 
 </style>
 <body>
 <div id="app">
     <el-scrollbar height="100vh">
         <el-backtop target="#app  .el-scrollbar__wrap"></el-backtop>
@@ -126,15 +126,16 @@
                 <br/>
                 <!-- table详情 ---------------->
                 <el-card>
                     <template #header>
                         <el-row class="card-header">
                             <el-col :span="20">
                                 <span>所属分类:</span>
-                                <el-select v-model="filterData.model_v" clearable @change="f_selectChange" placeholder="全部" style="width: 400px">
+                                <el-select v-model="filterData.model_v" clearable @change="f_selectChange"
+                                           placeholder="全部" style="width: 400px">
                                     <el-option v-for="item in filterData.model_options" :key="item" :label="item"
                                                :value="item"></el-option>
                                 </el-select>
                                 <span>结果:</span>
                                 <el-select v-model="filterData.status_v" clearable @change="f_selectChange"
                                            placeholder="全部">
                                     <el-option label="成功" value="passed"></el-option>
@@ -169,19 +170,22 @@
                                             <el-tab-pane label="跳过说明" v-if="scope.row.skipped">
                                                 <pre v-html="scope.row.skipped"></pre>
                                             </el-tab-pane>
                                             <el-tab-pane v-if="scope.row.msg_dict">
                                                 <template #label>
                                                     <span style="background-color: #f6c3c6; padding: 2px 5px; border-radius: 3px">失败详情</span>
                                                 </template>
-                                                <el-tag style="margin: 0 0 5px 20px" type="danger" v-if="scope.row.typed">{{f_errorInfo(scope.row.typed)}}</el-tag>
+                                                <el-tag style="margin: 0 0 5px 20px" type="danger"
+                                                        v-if="scope.row.typed">{{f_errorInfo(scope.row.typed)}}
+                                                </el-tag>
                                                 <pre v-html="scope.row.msg_dict"></pre>
                                             </el-tab-pane>
                                             <el-tab-pane label="图片预览" v-if="scope.row.img">
-                                                <el-image :src="scope.row.img" fit="contain" alt="图片" @error="f_handleImageLoadError"></el-image>
+                                                <el-image :src="scope.row.img" fit="contain" alt="图片"
+                                                          @error="f_handleImageLoadError"></el-image>
                                                 <span v-if="imgErrorText" style="color: #9d300b">{{imgErrorText}}</span>
                                             </el-tab-pane>
                                             <el-tab-pane v-if="scope.row.status_code" disabled>
                                                 <template #label>
                                                     <span class="custom-tabs-label">
                                                         <el-tag :type="scope.row.status_code==200?'success':'danger'">{{scope.row.status_code}}</el-tag>
                                                     </span>
@@ -208,21 +212,23 @@
                         </el-table-column>
                     </el-table>
                 </el-card>
             </el-col>
         </el-row>
         <!-- 展开/折叠/top按钮 -->
         <div style="right: 40px; position: absolute; width:40px;">
-            <el-affix position="bottom" :offset="150" >
+            <el-affix position="bottom" :offset="150">
                 <el-row>
                     <el-col style="margin-bottom: 20px;">
-                        <el-button type="primary" plain circle size="large" @click="f_toggleRowExpansion(true)">+</el-button>
+                        <el-button type="primary" plain circle size="large" @click="f_toggleRowExpansion(true)">+
+                        </el-button>
                     </el-col>
                     <el-col>
-                        <el-button type="primary" plain circle size="large" @click="f_toggleRowExpansion(false)">-</el-button>
+                        <el-button type="primary" plain circle size="large" @click="f_toggleRowExpansion(false)">-
+                        </el-button>
                     </el-col>
                 </el-row>
             </el-affix>
         </div>
         <el-backtop target="#app .el-scrollbar__wrap"></el-backtop>
     </el-scrollbar>
 </div>
@@ -244,34 +250,34 @@
                     if (filterData.model_options.indexOf(el['model']) === -1) {
                         filterData.model_options.push(el['model'])
                     }
                 })
                 f_selectChange()
             }
 
-            const f_errorInfo = (typed) =>{
-                if(typed == 10){
+            const f_errorInfo = (typed) => {
+                if (typed == 10) {
                     msg = "响应异常"
-                }else if (typed == 11){
+                } else if (typed == 11) {
                     msg = "断言类型错误"
-                }else if (typed == 12){
+                } else if (typed == 12) {
                     msg = "断言元素类型错误"
-                }else if (typed == 13){
+                } else if (typed == 13) {
                     msg = "断言元素key错误"
-                }else if (typed == 14){
+                } else if (typed == 14) {
                     msg = "响应内容不是json"
-                }else if (typed == 15){
+                } else if (typed == 15) {
                     msg = "断言type字段值错误"
-                }else if (typed == 20){
+                } else if (typed == 20) {
                     msg = "状态码错误"
-                }else if (typed == 21){
+                } else if (typed == 21) {
                     msg = "text匹配失败"
-                }else if (typed == 22){
+                } else if (typed == 22) {
                     msg = "json匹配失败"
-                }else {
+                } else {
                     msg = null
                 }
                 return msg
             }
 
 
             // 下拉框过滤
```

#### html2text {}

```diff
@@ -36,11 +36,11 @@
 label> å¤±è´¥è¯¦æ  {{f_errorInfo(scope.row.typed)}}
 
 src="scope.row.img" fit="contain" alt="å¾ç" @error="f_handleImageLoadError">
 {{imgErrorText}}
 label>
 type="scope.row.status_code==200?'success':'danger'">{{scope.row.status_code}}
 default="scope"> æå éè¯¯ å¤±è´¥ è·³è¿
-offset="150" >
+offset="150">
 click="f_toggleRowExpansion(true)">+
 click="f_toggleRowExpansion(false)">-
```

### Comparing `ddreport-4.1/ddreport/testReport.py` & `ddreport-4.2/ddreport/testReport.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #############################################
-# File Name: setup.py
+# File Name: ddreport
 # Author: duanliangcong
 # Mail: 137562703@qq.com
 # Created Time:  2022-11-02 15:00:00
 #############################################
 from _pytest.python import Function
 from _pytest.runner import runtestprotocol
 from jsonpath import jsonpath
+from collections.abc import Iterable
 from ddreport.api import CustomQuery
 from ddreport.db import PytestMysql
 from ddreport.func import PytestFunctions
-from collections.abc import Iterable
 from ddreport.handle import Process
 import requests
 import pytest
 import time
 import json
 import os, sys
 import re
@@ -171,15 +171,15 @@
     group.addoption(
         "--env_name",
         action="store",
         default=None,
         help="环境名称",
     ),
     group.addoption(
-        "--receive_dict",
+        "--receive",
         action="store",
         default=None,
         help="接收一个字典类型的参数",
     ),
     group.addoption(
         "--api_success",
         action="store",
@@ -201,22 +201,23 @@
         if success_show.upper() == "TRUE" or int(success_show) == 1:
             dict_data['show_success'] = True
         else:
             dict_data['show_success'] = False
     except Exception:
         dict_data['show_success'] = False
     # 记录命令传过来的参数
-    receive_dict = session.config.getoption("--receive_dict")
+    receive_dict = session.config.getoption("--receive")
     if receive_dict:
         try:
             receive_dict = json.loads(receive_dict)
         except Exception:
-            receive_dict = ast.literal_eval(receive_dict)
-        except Exception:
-            receive_dict = {}
+            try:
+                receive_dict = ast.literal_eval(receive_dict)
+            except Exception:
+                receive_dict = {}
         for k, v in receive_dict.items():
             GG.set(k, v)
 
 
 def pytest_sessionfinish(session, exitstatus):
     def set_default(obj):
         if isinstance(obj, (list, dict)):
@@ -245,15 +246,15 @@
 def pytest_runtest_makereport(item, call):
     outcome = yield
     report = outcome.get_result()
     call.duration = '%.2f' % call.duration          # 科学计数转普通格式
     if report.when == 'call':
         # 过滤不需要的funcargs
         dd_paramet.clear()
-        params_keys = [om.args[0] for om in item.own_markers]
+        params_keys = [om.args[0] for om in item.own_markers if om.args]
         for k in item.fixturenames:
             if k in ["_session_faker", "request"]:
                 continue
             elif k.startswith("dd__"):
                 continue
             elif params_keys and k in params_keys:
                 continue
@@ -278,29 +279,27 @@
 @pytest.fixture(scope='session')
 def ddreport(request):
     # 环境获取
     env_path = request.config.getoption("--env_path")
     env_name = request.config.getoption("--env_name")
     get_env = getEnvData(env_path, env_name)
     host = get_env.get('host') or ''
-    db = get_env.get('db') or None
-    db_ssh = get_env.get('db_ssh') or None
-    return MyFixture(host, db, db_ssh)
+    mysql = get_env.get('mysql')
+    return MyFixture(host, mysql)
 
 
 class MyFixture:
-    def __init__(self, host, _db, _db_ssh):
+    def __init__(self, host, mysql):
+        self.GVALUE = GG
         self.API = CustomQuery(GG, host)
         self.FC = PytestFunctions()
-        if _db:
+        self.MYSQL = None
+        if mysql:
             from ddreport.db import PytestMysql
-            self.DB = PytestMysql(_db, _db_ssh)
-        else:
-            self.DB = None
-        self.GVALUE = GG
+            self.MYSQL = PytestMysql(mysql)
         super().__init__()
 
 
 def pytest_generate_tests(metafunc):
     fixturenames = metafunc.definition.fixturenames
     dd_parames = [i for i in fixturenames if i.startswith("dd__")]
     if dd_parames:
```

