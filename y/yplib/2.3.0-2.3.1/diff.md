# Comparing `tmp/yplib-2.3.0.tar.gz` & `tmp/yplib-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.3.0.tar", last modified: Thu Jul  6 08:19:19 2023, max compression
+gzip compressed data, was "dist\yplib-2.3.1.tar", last modified: Thu Jul  6 08:50:01 2023, max compression
```

## Comparing `yplib-2.3.0.tar` & `yplib-2.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 08:19:19.883493 yplib-2.3.0/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.3.0/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-06 08:19:19.883493 yplib-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 08:19:19.884174 yplib-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-06 08:19:00.000000 yplib-2.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:19:19.880391 yplib-2.3.0/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.3.0/yplib/__init__.py
--rw-rw-rw-   0        0        0    12428 2023-07-04 00:52:40.000000 yplib-2.3.0/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.3.0/yplib/chart_html.py
--rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.3.0/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.3.0/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.3.0/yplib/http_util.py
--rw-rw-rw-   0        0        0    32812 2023-07-06 08:18:01.000000 yplib-2.3.0/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.3.0/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.3.0/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.3.0/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.3.0/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:19:19.882772 yplib-2.3.0/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-06 08:19:19.000000 yplib-2.3.0/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-06 08:19:19.000000 yplib-2.3.0/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 08:19:19.000000 yplib-2.3.0/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 08:19:19.000000 yplib-2.3.0/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 08:50:01.930331 yplib-2.3.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.3.1/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-06 08:50:01.929465 yplib-2.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 08:50:01.930331 yplib-2.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-06 08:49:53.000000 yplib-2.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:50:01.925604 yplib-2.3.1/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.3.1/yplib/__init__.py
+-rw-rw-rw-   0        0        0    12428 2023-07-04 00:52:40.000000 yplib-2.3.1/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.3.1/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.3.1/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.3.1/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.3.1/yplib/http_util.py
+-rw-rw-rw-   0        0        0    33596 2023-07-06 08:49:32.000000 yplib-2.3.1/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.3.1/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.3.1/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.3.1/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.3.1/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:50:01.928963 yplib-2.3.1/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-06 08:50:01.000000 yplib-2.3.1/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-06 08:50:01.000000 yplib-2.3.1/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 08:50:01.000000 yplib-2.3.1/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-06 08:50:01.000000 yplib-2.3.1/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.3.0/LICENSE` & `yplib-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.3.0/setup.py` & `yplib-2.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.3.0",
+  version="2.3.1",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.3.0/yplib/__init__.py` & `yplib-2.3.1/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.0/yplib/chart.py` & `yplib-2.3.1/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.0/yplib/chart_html.py` & `yplib-2.3.1/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.0/yplib/db.py` & `yplib-2.3.1/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.0/yplib/file.py` & `yplib-2.3.1/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.0/yplib/http_util.py` & `yplib-2.3.1/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.0/yplib/index.py` & `yplib-2.3.1/yplib/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,14 @@
 from datetime import timedelta
 
 import xlrd
 import xlwt
 
 
 # 记录日志, 如果是对象会转化为 json
-def to_print(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
-             a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
-    return to_log(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20, time_prefix=False)
-
-
-# 将 log 数据, 写入到文件
-def to_print_file(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
-                  a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
-    lo = to_print(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20)
-    to_txt([lo], datetime.today().strftime('%Y-%m-%d'), 'print', True, '.txt')
-
-
-# 记录日志, 如果是对象会转化为 json
 def to_log(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
            a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20='', time_prefix=True):
     l = [a1, a2, a3, a4, a5, a6, a7, a8, a9, a10,
          a11, a12, a13, a14, a15, a16, a17, a18, a19, a20]
     d = ''
     for one in l:
         if can_use_json(one):
@@ -41,14 +28,27 @@
                 d += ' '
             d += o
     lo = datetime.today().strftime('%Y-%m-%d %H:%M:%S') + ' ' + d if time_prefix else d
     print(lo)
     return lo
 
 
+# 记录日志, 如果是对象会转化为 json
+def to_print(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
+             a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
+    return to_log(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20, time_prefix=False)
+
+
+# 将 log 数据, 写入到文件
+def to_print_file(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
+                  a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
+    lo = to_print(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20)
+    to_txt([lo], datetime.today().strftime('%Y-%m-%d'), 'print', True, '.txt')
+
+
 # 将 log 数据, 写入到文件
 def to_log_file(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
                 a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20='', time_prefix=True):
     lo = to_log(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20, time_prefix=time_prefix)
     to_txt([lo], datetime.today().strftime('%Y-%m-%d'), 'log', True, '.log')
 
 
@@ -119,82 +119,89 @@
 def can_use_json(data):
     if isinstance(data, dict) or isinstance(data, list) or isinstance(data, tuple) or isinstance(data, set):
         return True
     return False
 
 
 # 检查文件夹是否存在,不存在,就创建新的
+# 支持多级目录 , 例如: C:\Users\yangpu\Desktop\study\a\b\c\d\e\f
 def check_file(file_name):
     if file_name is None or file_name == '':
         return
     for sep in ['\\', '/']:
         f_n = file_name.split(sep)
         for i in range(1, len(f_n) + 1):
             # C:\Users\yangpu\Desktop\study\p.t
             p_n = sep.join(f_n[0:i])
             if not os.path.exists(p_n):
                 os.mkdir(p_n)
 
 
 # 获得文件名称
+# 按照  name_天小时分钟_秒毫秒随机数 的规则来生成
 def get_file_name(file_name, suffix='.txt'):
     [day, hour, minute, second, ss] = datetime.today().strftime('%d_%H_%M_%S_%f').split('_')
     return str(file_name) \
         + '_' + day + hour + minute \
         + '_' + second + ss[0] + random_int_str(1) \
         + suffix
 
 
-# 获得文件名称
+# 文件是否存在
 def file_is_empty(file_name=None):
     return file_name is None or file_name == '' or not os.path.exists(file_name)
 
 
+# md5 算法
 def do_md5(data='do_md5'):
     return hashlib.md5(data.encode(encoding='UTF-8')).hexdigest()
 
 
+# sha256 算法
 def do_sha256(data='do_sha256'):
     h = hashlib.sha256()
     h.update(data.encode('utf-8'))
     return h.hexdigest()
 
 
+# uuid 类型的随机数, 默认 32 位长度
 def random_uuid(length=32):
     r = uuid.uuid4().hex
     while len(r) < length:
         r += uuid.uuid4().hex
     return r[0:length]
 
 
 # 获得随机数
-# length ：随机数长度
-# start_str ：随机数开始的字符的位置,从 1 开始
-# 包含 : start_str
-# end_str ：随机数结束的字符的位置
-# 不包含 : end_str
+# length    ：随机数长度
+# start_str ：随机数开始的字符的位置,从 1 开始, 包含start_str
+# end_str   : 随机数结束的字符的位置, 不包含end_str
+# 默认的随机数是 : 数字+字母大小写
 def random_str(length=64, start_str=1, end_str=62):
     c_s = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789-_'
     r = ''
     start_str = max(1, start_str)
     end_str = min(len(c_s), end_str)
     while len(r) < length:
         r += c_s[random.Random().randint(start_str, end_str) - 1]
     return r
 
 
+# 字母的随机数, 默认小写
 def random_letter(length=10, is_upper=False):
     r = random_str(length=length, end_str=26)
     return r.upper() if is_upper else r
 
 
+# 数字的随机数, 返回 int
 def random_int(length=10):
     return int(random_int_str(length=length))
 
 
+# 数字的随机数, 返回 str
 def random_int_str(length=10):
     return random_str(length=length, start_str=53, end_str=62)
 
 
 # 去掉 str 中的 非数字字符, 然后, 再转化为 int
 def to_int(s):
     if isinstance(s, int):
@@ -213,14 +220,15 @@
         return s
     if s is None or s == '':
         return 0.0
     s = ''.join(filter(lambda ch: ch in '0123456789.', str(s)))
     return 0.0 if s == '' else float(s)
 
 
+# 将字符串 s 转化成 datetime
 def to_datetime(s=None, r_str=False):
     if s is None or s == '':
         return str(datetime.today()) if r_str else datetime.today()
     s = str(s)
     r = None
     m_s = {
         "^\\d{4}$": "%Y",
@@ -242,36 +250,53 @@
         time_str = time.strftime("%Y-%m-%d %H:%M:%S", time_arr)
         r = datetime.strptime(time_str, "%Y-%m-%d %H:%M:%S")
     if r is None:
         r = datetime.today()
     return str(r) if r_str else r
 
 
+# 将字符串 s 转化成 datetime, 然后再次转化成 str
+def to_datetime_str(s=None):
+    return to_datetime(s, r_str=True)
+
+
 # 时间加几天
 def to_datetime_add(s=None, days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0):
     return to_datetime(s) + timedelta(days=days, seconds=seconds, microseconds=microseconds,
                                       milliseconds=milliseconds, minutes=minutes, hours=hours,
                                       weeks=weeks)
 
 
+# 将字符串 s 转化成 date 例如: 2021-02-03
 def to_date(s=None):
     return str(to_datetime(s))[0:10]
 
 
+# 时间加几天
 def to_date_add(s=None, days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0):
     return str(to_datetime_add(s=s, days=days, seconds=seconds, microseconds=microseconds,
                                milliseconds=milliseconds, minutes=minutes, hours=hours, weeks=weeks))[0:10]
 
 
 # 将 list 中的数据以 json 或者基本类型的形式写入到文件中
-# data_list : 数组数据, 也可以不是数组
-# file_name : 文件名 , 当文件名是 C:\Users\yangpu\Desktop\study\abc\d\e\f\a.txt 这种类型的时候, 可以直接创建文件夹,
-# fixed_name : 是否固定文件名
-# file_path : 文件路径
-def to_txt(data_list, file_name='txt', file_path='txt', fixed_name=False, suffix='.txt'):
+# data_list   : 数组数据, 也可以不是数组
+# file_name   : 文件名 , 默认 txt
+#               当文件名是 C:\Users\yangpu\Desktop\study\abc\d\e\f\a.txt 这种类型的时候, 可以直接创建文件夹,
+#                   会赋值 file_path=C:\Users\yangpu\Desktop\study\abc\d\e\f,
+#                         file_name=a.txt,
+#                         fixed_name=True
+#               当文件名是 abc 的时候, 按照正常值,计算
+# file_path   : 文件路径
+# fixed_name  : 是否固定文件名
+# suffix      : 文件后缀, 默认 .txt
+def to_txt(data_list,
+           file_name='txt',
+           file_path='txt',
+           fixed_name=False,
+           suffix='.txt'):
     file_name = str(file_name)
     for sep in ['\\', '/']:
         f_n = file_name.split(sep)
         if len(f_n) > 1:
             file_name = f_n[-1]
             file_path = sep.join(f_n[0:-1])
             if '.' in file_name:
@@ -304,25 +329,26 @@
 
 
 # 将 list 中的数据写入到固定的文件中,自己设置文件后缀
 def to_txt_data(data_list, file_name='data'):
     return to_txt(data_list, file_name, 'data', True)
 
 
+# 转化成字符串
 def to_str(data):
     if can_use_json(data):
         s = json.dumps(data)
     else:
         s = str(data)
     return s
 
 
 # 根据json的key排序,用于签名
 # 按照 key 排序, 按照 key=value 然后再 & 连接, 如果数据中有 list, 使用 , 连接 list 中的数据, 然后拼接成 str 返回
-# sep : 分隔符 , 默认 &
+# sep       : 分隔符 , 默认 &
 # join      : 连接符 , 默认 =
 # join_list : list 数据 连接符 , 默认 ,
 def sort_by_json_key(data_obj, sep='&', join='=', join_list=','):
     if isinstance(data_obj, list) or isinstance(data_obj, tuple) or isinstance(data_obj, set):
         return join_list.join(list(map(lambda x: f'{x}', data_obj)))
     if not isinstance(data_obj, dict):
         return str(data_obj)
@@ -334,47 +360,31 @@
             s = sort_by_json_key(data_obj=value_one, sep=sep, join=join, join_list=join_list)
         else:
             s = str(value_one)
         r_l.append(f'{one[0]}{join}{s}')
     return sep.join(r_l)
 
 
-# data = {}
-# data['merchantId'] = "merchantId"
-# data['currency'] = "IDR"
-# data['accType'] = "payout"
-# data['version'] = "1.0"
-# data['b'] = {
-#     'a': 1,
-#     'c': 'c',
-#     'b': 'po',
-# }
-# b = [2, 3, 8, 4, "yp"]
-# data['c'] = b
-# sign = sort_by_json_key(data)
-# print(sign)
-
-
 # 当读取 txt 之类的文件的时候
 # 将 txt 文件读取到 list 中, 每一行自动过滤掉行前行后的特殊字符
-# sep : 是否对每一行进行分割,如果存在这个字段,就分割
-# sep_all : 将文件转化成一个字符串,然后对这个字符串,再次总体分割
-# start_index : 从这个地方开始读取,从1开始标号 , 包含这一行
-# start_line :  从这个地方开始读取,从第一行开始找到这个字符串开始标记 , 包含这一行
-# end_index :   读取到这个地方结束,从1开始标号 , 不包含这一行
-# end_line :    读取到这个地方结束,从第一行开始找到这个字符串开始标记 , 不包含这一行
-# count :       读取指定的行数
+# sep             : 是否对每一行进行分割,如果存在这个字段,就分割
+# sep_all         : 将文件转化成一个字符串,然后对这个字符串,再次总体分割
+# start_index     : 从这个地方开始读取,从1开始标号 , 包含这一行
+# start_line      : 从这个地方开始读取,从第一行开始找到这个字符串开始标记 , 包含这一行
+# end_index       : 读取到这个地方结束,从1开始标号 , 不包含这一行
+# end_line        : 读取到这个地方结束,从第一行开始找到这个字符串开始标记 , 不包含这一行
+# count           : 读取指定的行数
 ################################################
 # 当读取 excel 之类的文件的时候
 # 将 excel 文件读取到 list 中, 可以指定 sheet, 也可以指定列 column_index(列) ,自动过滤掉每个单元格前后的特殊字符
-# sheet : 从 1 开始编号,
-# column_index : 从 1 开始编号, 指定列
-# column_index : 如果是指定值, 这个时候返回的是一个 list, 没有嵌套 list
-# column_index : 如果是 '1,2,3,4'   [1,2,3,4], 返回的是一个嵌套 list[list]
-# column_date : 指定日期格式的列,规则与 column_index 一样
+# sheet           : 从 1 开始编号,
+# column_index    : 从 1 开始编号, 指定列
+# column_index    : 如果是指定值, 这个时候返回的是一个 list, 没有嵌套 list
+# column_index    : 如果是 '1,2,3,4'   [1,2,3,4], 返回的是一个嵌套 list[list]
+# column_date     : 指定日期格式的列,规则与 column_index 一样
 # column_datetime : 指定日期格式的列,规则与 column_index 一样
 # 返回的数据一定是一个 list
 def to_list(file_name='a.txt',
             sep=None,
             sep_line=None,
             sep_line_contain=None,
             sep_line_prefix=None,
@@ -407,18 +417,18 @@
                             end_index=end_index,
                             end_line=end_line,
                             count=count)
 
 
 # 当读取 excel 之类的文件的时候
 # 将 excel 文件读取到 list 中, 可以指定 sheet, 也可以指定列 column_index(列) ,自动过滤掉每个单元格前后的特殊字符
-# sheet_index  : 从 1 开始编号,
-# column_index : 从 1 开始编号, 指定列, 如果是指定值是一个, 这个时候返回的是一个 list, 没有嵌套 list
-#                如果是 '1,2,3,4'   [1,2,3,4], 返回的是一个嵌套 list[list]
-# column_date :  指定日期格式的列,规则与 column_index 一样
+# sheet_index     : 从 1 开始编号,
+# column_index    : 从 1 开始编号, 指定列, 如果是指定值是一个, 这个时候返回的是一个 list, 没有嵌套 list
+#                    如果是 '1,2,3,4'   [1,2,3,4], 返回的是一个嵌套 list[list]
+# column_date     : 指定日期格式的列,规则与 column_index 一样
 # column_datetime : 指定日期格式的列,规则与 column_index 一样
 def to_list_from_excel(file_name='a.xls',
                        sheet_index=1,
                        column_index=None,
                        column_date=None,
                        column_datetime=None):
     if file_is_empty(file_name):
```

### Comparing `yplib-2.3.0/yplib/mail.py` & `yplib-2.3.1/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.0/yplib/mail_html.py` & `yplib-2.3.1/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.3.0/yplib/markdown.py` & `yplib-2.3.1/yplib/markdown.py`

 * *Files identical despite different names*

