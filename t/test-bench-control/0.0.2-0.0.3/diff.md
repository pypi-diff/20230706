# Comparing `tmp/test_bench_control-0.0.2.tar.gz` & `tmp/test_bench_control-0.0.3.tar.gz`

## Comparing `test_bench_control-0.0.2.tar` & `test_bench_control-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 test_bench_control-0.0.2/src/test_bench_control/__init__.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 test_bench_control-0.0.2/src/test_bench_control/camera.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 test_bench_control-0.0.2/src/test_bench_control/motor.py
--rw-r--r--   0        0        0   163760 2020-02-02 00:00:00.000000 test_bench_control-0.0.2/src/test_bench_control/pipipi.jpg.filepart
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 test_bench_control-0.0.2/LICENSE
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 test_bench_control-0.0.2/README.md
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 test_bench_control-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 test_bench_control-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 test_bench_control-0.0.3/src/test_bench_control/__init__.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 test_bench_control-0.0.3/src/test_bench_control/camera.py
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 test_bench_control-0.0.3/src/test_bench_control/motor.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 test_bench_control-0.0.3/LICENSE
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 test_bench_control-0.0.3/README.md
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 test_bench_control-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 test_bench_control-0.0.3/PKG-INFO
```

### Comparing `test_bench_control-0.0.2/src/test_bench_control/motor.py` & `test_bench_control-0.0.3/src/test_bench_control/motor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import RPi.GPIO as GPIO
 import time
-#import sys
 import numpy as np
 
 GPIO.setmode(GPIO.BOARD)
 
-# Raspberry Pi Pin-Belegung fur TB6600 Treiber
+# Raspberry Pi Pin Assignment for TB6600 Driver
 DIR = 33
 PUL = 35
 ENA = 37
 
 DIR_Left = GPIO.HIGH
 DIR_Right = GPIO.LOW
 
@@ -17,59 +16,67 @@
 ENA_Released = GPIO.HIGH
 
 GPIO.setwarnings(False)
 GPIO.setup(DIR, GPIO.OUT)
 GPIO.setup(PUL, GPIO.OUT)
 GPIO.setup(ENA, GPIO.OUT)
 
-def rotate(degree,slope=0.5,rpm_max=200): #degree: rotation of plate in degree, slope: how fast motor starts [0,1] 0=slow, 1=fast, max_rpm: max rpm of motor
+def rotate(degree,slope=0.5,rpm_max=100):
+    
+    ###########################################################################################
+    #  Pre:     degree  (float) - rotation of plate in degrees D=[-inf,inf] 
+    #           slope   (float) - how fast motor starts D=[0,1], with 0 = slowest, 1 = fastest
+    #           rpm_max (float) - max rpm of motor, NOT the plate! D=[50,300]
+    #  Post:    no return value
+    #  Example: rotate(degree=-8.6,slope=0.2,rpm_max=200)
+    ###########################################################################################
+
     if degree==0:
         exit()
     if degree<0:
         GPIO.output(DIR, DIR_Left)
     if degree>0:
         GPIO.output(DIR, DIR_Right)
         
-    if rpm_max > 1000:
-        rpm_max = 1000
-    if rpm_max < 100:
-        rpm_max = 100
+    if rpm_max > 300:
+        rpm_max = 300
+    if rpm_max < 50:
+        rpm_max = 50
     if slope > 1:
         slope = 1
     if slope < 0:
         slope = 0
         
-    # Motor aktivieren und halten
+    # activate motor and hold torque
     GPIO.output(ENA, ENA_Locked)
 
-    #1 motor turn equals 400 steps. With i = 1:15, 1 table turn is 15*400 = 6000 steps
+    # 1 motor turn equals 400 steps. With i = 1:15, 1 table turn is 15*400 = 6000 steps
     steps=int(abs(degree)*6000/360)
     RPM_of_step = np.zeros(steps)
     slope = 0.8*slope + 0.2 #min slope is 0.2, max slope is 1.0
-    rpm_min = 100 #might adapt in future
+    rpm_min = 50 #might adapt in future
     steps_until_max_rpm = int((rpm_max-rpm_min)/slope)
     
+    # if degree is so small: ramp up and ramp down
     if steps<=2*steps_until_max_rpm:
-        #slope up and down
+        #ramp up and down
         for i in range(0,int(steps/2)):
             RPM_of_step[i]=rpm_min+i*slope
             RPM_of_step[steps-i-1]=rpm_min+i*slope
     else:
-        
-        #slope up, stay up and then and down
+        #ramp up, stay up and then and down
         for i in range(0,steps_until_max_rpm):
             RPM_of_step[i]=rpm_min+i*slope
             RPM_of_step[steps-i-1]=rpm_min+i*slope
         for i in range(steps_until_max_rpm,(steps-steps_until_max_rpm)):
             RPM_of_step[i]=rpm_max
     
     for i in range(0,len(RPM_of_step)):
         currentfrequency=0.3/(RPM_of_step[i])
-        # Puls modulieren
+        # modulate pulse
         GPIO.output(PUL, GPIO.HIGH)
         time.sleep(currentfrequency/2)#(0.0001875)
-
         GPIO.output(PUL, GPIO.LOW)
         time.sleep(currentfrequency/2)
 
-    # Motor freigeben
+    # release motor
     GPIO.output(ENA, ENA_Released)
```

### Comparing `test_bench_control-0.0.2/LICENSE` & `test_bench_control-0.0.3/LICENSE`

 * *Files identical despite different names*

