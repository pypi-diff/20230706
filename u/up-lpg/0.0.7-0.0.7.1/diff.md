# Comparing `tmp/up_lpg-0.0.7-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/up_lpg-0.0.7.1-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1190477 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       36 b- defN 23-May-30 14:40 up_lpg/__init__.py
--rw-rw-rw-  2.0 fat    10795 b- defN 23-May-30 14:40 up_lpg/lpg_planner.py
--rw-rw-rw-  2.0 fat  3881596 b- defN 23-May-30 14:40 up_lpg/winlpg.exe
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-30 14:47 up_lpg-0.0.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      334 b- defN 23-May-30 14:47 up_lpg-0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-May-30 14:47 up_lpg-0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-May-30 14:47 up_lpg-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      610 b- defN 23-May-30 14:47 up_lpg-0.0.7.dist-info/RECORD
-8 files, 3905043 bytes uncompressed, 1189427 bytes compressed:  69.5%
+Zip file size: 1190518 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       36 b- defN 23-Jul-06 13:00 up_lpg/__init__.py
+-rw-rw-rw-  2.0 fat    10927 b- defN 23-Jul-06 13:00 up_lpg/lpg_planner.py
+-rw-rw-rw-  2.0 fat  3881596 b- defN 23-Jul-06 13:00 up_lpg/winlpg.exe
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jul-06 13:10 up_lpg-0.0.7.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      336 b- defN 23-Jul-06 13:10 up_lpg-0.0.7.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-Jul-06 13:10 up_lpg-0.0.7.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-06 13:10 up_lpg-0.0.7.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      620 b- defN 23-Jul-06 13:10 up_lpg-0.0.7.1.dist-info/RECORD
+8 files, 3905187 bytes uncompressed, 1189448 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: up_lpg/lpg_planner.py
 Comment: 
 
 Filename: up_lpg/winlpg.exe
 Comment: 
 
-Filename: up_lpg-0.0.7.dist-info/LICENSE
+Filename: up_lpg-0.0.7.1.dist-info/LICENSE
 Comment: 
 
-Filename: up_lpg-0.0.7.dist-info/METADATA
+Filename: up_lpg-0.0.7.1.dist-info/METADATA
 Comment: 
 
-Filename: up_lpg-0.0.7.dist-info/WHEEL
+Filename: up_lpg-0.0.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: up_lpg-0.0.7.dist-info/top_level.txt
+Filename: up_lpg-0.0.7.1.dist-info/top_level.txt
 Comment: 
 
-Filename: up_lpg-0.0.7.dist-info/RECORD
+Filename: up_lpg-0.0.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## up_lpg/lpg_planner.py

```diff
@@ -240,12 +240,15 @@
             self._options.extend(['-input_plan', plan_to_repair_filename])
             return self.solve(problem)
 
     def plan_to_file(self, plan: Plan, out: IO[str]):
         with open(out, "w") as f:
             for i, act in enumerate(plan.actions):
                 parameters = str(act.actual_parameters).replace('(','').replace(')','').replace(',','')
-                f.write(f'{i}:   ({act.action.name} {parameters})  [1]\n')
+                if parameters == '':
+                    f.write(f'{i}:   ({act.action.name})  [1]\n')
+                else:
+                    f.write(f'{i}:   ({act.action.name} {parameters})  [1]\n')
 
     @staticmethod
     def supports_plan(plan_kind: "up.plans.PlanKind") -> bool:
         return plan_kind == PlanKind.SEQUENTIAL_PLAN
```

## Comparing `up_lpg-0.0.7.dist-info/LICENSE` & `up_lpg-0.0.7.1.dist-info/LICENSE`

 * *Files identical despite different names*

