# Comparing `tmp/gtki_module_exex-0.0.5-py3-none-any.whl.zip` & `tmp/gtki_module_exex-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6291 bytes, number of entries: 11
+Zip file size: 6715 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-09 04:59 gtki_module_exex/__init__.py
--rw-rw-rw-  2.0 fat     6335 b- defN 23-Jun-16 14:54 gtki_module_exex/main.py
+-rw-rw-rw-  2.0 fat    11494 b- defN 23-Jul-06 11:35 gtki_module_exex/main.py
 -rw-rw-rw-  2.0 fat     1431 b- defN 23-Jun-15 14:51 gtki_module_exex/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-09 05:22 gtki_module_exex/tests/__init__.py
--rw-rw-rw-  2.0 fat     2319 b- defN 23-Jun-16 14:37 gtki_module_exex/tests/main_tests.py
+-rw-rw-rw-  2.0 fat     2251 b- defN 23-Jul-06 07:30 gtki_module_exex/tests/main_tests.py
 -rw-rw-rw-  2.0 fat     1007 b- defN 22-Jun-09 05:55 gtki_module_exex/tests/mixins_tests.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-16 14:54 gtki_module_exex-0.0.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      279 b- defN 23-Jun-16 14:54 gtki_module_exex-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-16 14:54 gtki_module_exex-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-16 14:54 gtki_module_exex-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      952 b- defN 23-Jun-16 14:54 gtki_module_exex-0.0.5.dist-info/RECORD
-11 files, 13523 bytes uncompressed, 4653 bytes compressed:  65.6%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-06 11:43 gtki_module_exex-0.0.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      279 b- defN 23-Jul-06 11:43 gtki_module_exex-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-06 11:43 gtki_module_exex-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-06 11:43 gtki_module_exex-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      953 b- defN 23-Jul-06 11:43 gtki_module_exex-0.0.6.dist-info/RECORD
+11 files, 18615 bytes uncompressed, 5077 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: gtki_module_exex/tests/main_tests.py
 Comment: 
 
 Filename: gtki_module_exex/tests/mixins_tests.py
 Comment: 
 
-Filename: gtki_module_exex-0.0.5.dist-info/LICENSE
+Filename: gtki_module_exex-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: gtki_module_exex-0.0.5.dist-info/METADATA
+Filename: gtki_module_exex-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: gtki_module_exex-0.0.5.dist-info/WHEEL
+Filename: gtki_module_exex-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: gtki_module_exex-0.0.5.dist-info/top_level.txt
+Filename: gtki_module_exex-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: gtki_module_exex-0.0.5.dist-info/RECORD
+Filename: gtki_module_exex-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gtki_module_exex/main.py

```diff
@@ -1,12 +1,14 @@
 import datetime
 from wsqluse import wsqluse
-from gtki_module_exex.mixins import XlsCreator, TemplateCreator, DataFiller, IshbDailyReportTemplate
+from gtki_module_exex.mixins import XlsCreator, TemplateCreator, DataFiller, \
+    IshbDailyReportTemplate
 from ar_qdk.main import ARQDK
 
+
 class CreateExcel(XlsCreator, TemplateCreator, DataFiller):
     def __init__(self, file_name, data_list, column_names=None):
         if column_names:
             self.column_names = column_names
         self.data_list = data_list
         self.file_name = file_name
         self.workbook = self.create_workbook()
@@ -47,96 +49,200 @@
     def __init__(self, file_name, ar_ip, ar_port,
                  column_names=None):
         self.file_name = file_name
         self.ar_qdk = ARQDK(ip=ar_ip, port=ar_port)
         self.ar_qdk.make_connection()
         self.workbook = self.create_workbook()
         self.worksheet = self.create_worksheet()
-        #super().__init__(file_name, acts_list, column_names)
-        self.column_names = ["Категория", "Клиент", "Перевозчик", "Количество \nрейсов",
-                    "Общий вес,\nтонн", "Выручка, руб.", "Ошибки"]
+        # super().__init__(file_name, acts_list, column_names)
+        self.column_names = ["Категория", "Клиент", "Перевозчик",
+                             "Количество \nрейсов",
+                             "Общий вес,\nтонн", "Выручка, руб.", "Ошибки"]
         self.header_format = self.workbook.add_format({'bold': True,
-                                                  'align': 'center',
-                                                  'valign': 'center',
-                                                  'font_size': 11})
+                                                       'align': 'center',
+                                                       'valign': 'center',
+                                                       'font_size': 11})
         self.header_format.set_font_size(11)
         self.header_format.set_center_across()
+        self.amount_format = self.header_format = self.workbook.add_format(
+            {'bold': True,
+             'font_size': 11})
 
     def create_day_header(self, day=None):
         merge_format = self.workbook.add_format({'align': 'center'})
         merge_format.set_font_size(14)
         self.worksheet.merge_range('A1:G1', day, merge_format)
 
     def operate_trash_cat(self, trash_cat, day, start_row):
-        #records = self.get_records(trash_cat, day)
-        records = self.ar_qdk.execute_method("get_daily_report",
+        records = self.ar_qdk.execute_method("get_daily_report_by_trash_cat",
                                              trash_cat=trash_cat,
                                              day=day,
                                              get_response=True)
         if records['status']:
             records = records['info']
         if not records:
             return
-        self.worksheet.write(start_row, 0, trash_cat, self.header_format)
+        trash_cat_row = start_row + 1
+        self.worksheet.write(trash_cat_row, 0, trash_cat, self.amount_format)
+        record_row = trash_cat_row
         for rec in records:
-            self.set_record(rec['client_name'], rec['carrier_name'], rec['amount'], rec['tonnage'], start_row)
-            start_row += 1
-        amount, tonnage = self.get_amount(records)
-        return self.set_amount(amount, tonnage, start_row+1)
-
+            self.set_record(rec['client_name'], rec['carrier_name'],
+                            rec['amount'], rec['tonnage'], record_row)
+            record_row += 1
+        return self.set_amount(start_row, record_row)
 
     def get_amount(self, records):
         amount = 0
         tonnage = 0
         for rec in records:
             amount += rec['amount']
             tonnage += rec['tonnage']
         return amount, tonnage
 
-
     def set_record(self, client, carrier, amount, tonnage, start_row):
-        self.worksheet.write(start_row, 1, client)
-        self.worksheet.write(start_row, 2, carrier)
-        self.worksheet.write(start_row, 3, amount)
-        self.worksheet.write(start_row, 4, tonnage)
+        record_format = self.workbook.add_format()
+        self.worksheet.write(start_row, 1, client, record_format)
+        self.worksheet.write(start_row, 2, carrier, record_format)
+        self.worksheet.write(start_row, 3, amount, record_format)
+        self.worksheet.write(start_row, 4, tonnage, record_format)
         return
 
-    @wsqluse.getTableDictStripper
-    def get_records(self, trash_cat, day):
-        return self.sql_shell.get_table_dict(
-            "select c.name as client_name, cr.name as carrier_name, "
-            "sum(r.cargo) as tonnage, count(r.id) as amount "
-            "from records r left join clients c on (r.client_id=c.id) "
-            "left join clients cr on (r.carrier=cr.id) "
-            f"where r.trash_cat=(select id from trash_cats where name='{trash_cat}') "
-            f"and time_in::date='{day}' group by (c.name, cr.name);"
-        )
-
-    def set_amount(self, amount, tonnage, row=2):
-        self.worksheet.write(row, 0, "ИТОГО", self.header_format)
-        self.worksheet.write(row, 3, amount, self.header_format)
-        self.worksheet.write(row, 4, tonnage, self.header_format)
-        return row
-
-    def set_trash_cat(self, cat_name, row):
-        self.worksheet.write(row, 0, cat_name, self.header_format)
+    def set_amount(self, start_record_row, end_record_row, alias="ИТОГО:"):
+        amount_format = self.header_format = self.workbook.add_format(
+            {'bold': True,
+             'font_size': 12})
+        self.worksheet.write(end_record_row + 1, 0, alias,
+                             self.header_format)
+        self.worksheet.write_formula(end_record_row + 1, 3,
+                                     f"=SUM(D{start_record_row + 2}:D{end_record_row})",
+                                     amount_format)
+        self.worksheet.write_formula(end_record_row + 1, 4,
+                                     f"=SUM(E{start_record_row + 2}:E{end_record_row})",
+                                     amount_format)
+        return end_record_row
+
+    def set_final_amount(self, end_record_row, rows, alias="ВСЕГО:"):
+        final_format = self.workbook.add_format(
+            {'bold': True,
+             'font_size': 14})
+        self.worksheet.write(end_record_row + 1, 0, alias,
+                             final_format)
+        amount_func = f"=SUM({'+'.join([f'D{row}' for row in rows])})"
+        tonnage_func = f"=SUM({'+'.join([f'E{row}' for row in rows])})"
+        self.worksheet.write_formula(end_record_row + 1, 3,
+                                     amount_func,
+                                     final_format)
+        self.worksheet.write_formula(end_record_row + 1, 4,
+                                     tonnage_func,
+                                     final_format)
+        return end_record_row
 
     def create_document(self, day=None):
+        amounts = []
         if not day:
             day = datetime.datetime.now()
         self.create_day_header(day.strftime("%#d/%m/%Y"))
         self.set_column_width()
         start_row = self.set_column_names()
-        start_row += 1
+        new_row = start_row
         for tc in ["ТКО", "ПО", "Хвосты", "Прочее"]:
-            start_row = self.operate_trash_cat(tc, day.strftime("%Y.%m.%d"), start_row=start_row)
-            if start_row:
-                start_row += 2
+            new_row = self.operate_trash_cat(tc, day.strftime("%Y.%m.%d"),
+                                             start_row=new_row)
+            amounts.append(new_row+2)
+            new_row += 1
+        row = self.add_hyundai(day, new_row)
+        amounts.append(row+2)
+        row = self.add_phys(day, row+2)
+        amounts.append(row+2)
+        row = self.add_recyclables(day, row+2)
+        amounts.append(row+2)
+        row = self.set_amount(start_record_row=start_row,
+                              end_record_row=row+2, alias="ВСЕГО")
+        row = self.set_final_amount(row, amounts)
+        self.set_borders(row+1)
+        self.add_user_info(row)
         self.workbook.close()
 
+    def add_user_info(self, row):
+        row += 3
+        current_user_info = self.ar_qdk.execute_method("get_current_user_info",
+                                                       get_response=True)
+        if not current_user_info['status']:
+            return
+        username = current_user_info['info'][0]['username']
+        self.worksheet.write(row, 0, "Сдал:")
+        self.worksheet.write(row, 1, username)
+        self.worksheet.write(row, 3, "Подпись:")
+        return row
+        #self.worksheet.write(trash_cat_row, 0, "Физ.лицо", self.amount_format)
+
+    def add_hyundai(self, day, start_row):
+        records = self.ar_qdk.execute_method("get_daily_report_by_car_number",
+                                             car_number='Н370УЕ102',
+                                             day=day,
+                                             get_response=True)
+        if records['status']:
+            records = records['info']
+        if not records:
+            return
+        trash_cat_row = start_row + 1
+        self.worksheet.write(trash_cat_row, 0, "ХУНДАЙ", self.amount_format)
+        record_row = trash_cat_row
+        for rec in records:
+            self.set_record(rec['client_name'], rec['carrier_name'],
+                            rec['amount'], rec['tonnage'], record_row)
+            record_row += 1
+        return self.set_amount(start_row, record_row)
+
+    def add_phys(self, day, start_row):
+        records = self.ar_qdk.execute_method("get_daily_report_by_client",
+                                             client='Физлицо',
+                                             day=day,
+                                             get_response=True)
+        if records['status']:
+            records = records['info']
+        if not records:
+            return
+        trash_cat_row = start_row + 1
+        self.worksheet.write(trash_cat_row, 0, "Физ.лицо", self.amount_format)
+        record_row = trash_cat_row
+        for rec in records:
+            self.set_record(rec['client_name'], rec['carrier_name'],
+                            rec['amount'], rec['tonnage'], record_row)
+            record_row += 1
+        return self.set_amount(start_row, record_row)
+
+    def add_recyclables(self, day, start_row):
+        records = self.ar_qdk.execute_method("get_daily_report_by_client",
+                                             client='ИПБутыринИ.А.',
+                                             day=day,
+                                             get_response=True)
+        if records['status']:
+            records = records['info']
+        if not records:
+            return
+        trash_cat_row = start_row + 1
+        self.worksheet.write(trash_cat_row, 0, "Вторсырье", self.amount_format)
+        record_row = trash_cat_row
+        for rec in records:
+            self.set_record(rec['client_name'], rec['carrier_name'],
+                            rec['amount'], rec['tonnage'], record_row)
+            record_row += 1
+        return self.set_amount(start_row, record_row)
+
+    def set_borders(self, last_row):
+        border_format = self.workbook.add_format()
+        border_format.set_border()
+        self.worksheet.conditional_format(f'A2:G{last_row + 1}',
+                                          {'type': 'no_blanks',
+                                           'format': border_format})
+        self.worksheet.conditional_format(f'A2:G{last_row + 1}',
+                                          {'type': 'blanks',
+                                           'format': border_format})
+
     def set_column_names(self):
         col_num = 0
         self.worksheet.set_row_pixels(1, 42)
         for col_name in self.column_names:
             self.worksheet.write(1, col_num, col_name, self.header_format)
             col_num += 1
         return 1
```

## gtki_module_exex/tests/main_tests.py

```diff
@@ -33,15 +33,14 @@
         amount_info = 'Итого 5000 (3 взвешивания)'
         inst = main.CreateExcelActs('main_acts.xls', self.data_list,
                                     amount_info)
         inst.create_document()
 
 
     def tests_creat_daily_report(self):
-        sql_shell = Wsqluse("gdb", "qodex", "0kra1na&73", "127.0.0.1")
-        inst = main.CreateExcelDailyReport('ishb_daily.xls',
+        inst = main.CreateExcelDailyReport('ishb_daily_new.xls',
                                            ar_port=52250,
                                            ar_ip="localhost")
         inst.create_document()
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `gtki_module_exex-0.0.5.dist-info/LICENSE` & `gtki_module_exex-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gtki_module_exex-0.0.5.dist-info/RECORD` & `gtki_module_exex-0.0.6.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 gtki_module_exex/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gtki_module_exex/main.py,sha256=86MUeoKOCisSxCFEhGkIIiWypuiMaTBcvnx8K5QEDso,6335
+gtki_module_exex/main.py,sha256=Ykpx6r0B4jKJAGqYxx8W7Xncseu0r3Zv8sNt6RIaAO0,11494
 gtki_module_exex/mixins.py,sha256=nKYRHMoFYSva364Q2WyH30SefjAxi5xGXekgLmRAyXk,1431
 gtki_module_exex/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gtki_module_exex/tests/main_tests.py,sha256=B4FlY1vXuCg6D0tasIimMedKGDXJeclVrz8xNslv48M,2319
+gtki_module_exex/tests/main_tests.py,sha256=ZTo-ylgaHZCNeMuVtoktNdEzwioc9r6XU7EWCgpVfGw,2251
 gtki_module_exex/tests/mixins_tests.py,sha256=8oogAhtkQgyhB3sUEsIvQpvA1a7YrRPc76bDHKsxodI,1007
-gtki_module_exex-0.0.5.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-gtki_module_exex-0.0.5.dist-info/METADATA,sha256=Mn9Jwml3C3WMNSrRR2Oba26V4P0WR9ArfUvRpEA1-u0,279
-gtki_module_exex-0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gtki_module_exex-0.0.5.dist-info/top_level.txt,sha256=5fDck53WZ0oTnmcblVZKn9XwbA-Uqijh0L93F1ml9Bc,17
-gtki_module_exex-0.0.5.dist-info/RECORD,,
+gtki_module_exex-0.0.6.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+gtki_module_exex-0.0.6.dist-info/METADATA,sha256=obLkj4LRBS6sQoDDsQo0Hrcvk1emEp-sozPg5_Hrt1U,279
+gtki_module_exex-0.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gtki_module_exex-0.0.6.dist-info/top_level.txt,sha256=5fDck53WZ0oTnmcblVZKn9XwbA-Uqijh0L93F1ml9Bc,17
+gtki_module_exex-0.0.6.dist-info/RECORD,,
```

