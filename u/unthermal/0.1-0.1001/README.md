# Comparing `tmp/unthermal-0.1.tar.gz` & `tmp/unthermal-0.1001.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unthermal-0.1.tar", last modified: Fri May 31 17:59:42 2024, max compression
+gzip compressed data, was "unthermal-0.1001.tar", last modified: Sat Jun  1 14:17:20 2024, max compression
```

## Comparing `unthermal-0.1.tar` & `unthermal-0.1001.tar`

### file list

```diff
@@ -1,29 +1,18 @@
-drwxr-xr-x   0 leonardo  (1000) leonardo  (1000)        0 2024-05-31 17:59:42.105609 unthermal-0.1/
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)     1072 2024-05-31 16:03:53.000000 unthermal-0.1/LICENSE.txt
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)       42 2024-05-31 15:51:11.000000 unthermal-0.1/MANIFEST.in
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)     2728 2024-05-31 17:59:42.105609 unthermal-0.1/PKG-INFO
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)     2259 2024-05-31 13:19:16.000000 unthermal-0.1/README.md
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)      710 2024-05-31 17:59:19.000000 unthermal-0.1/pyproject.toml
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)       38 2024-05-31 17:59:42.105609 unthermal-0.1/setup.cfg
-drwxr-xr-x   0 leonardo  (1000) leonardo  (1000)        0 2024-05-31 17:59:42.102275 unthermal-0.1/unthermal/
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)      226 2024-05-31 14:54:15.000000 unthermal-0.1/unthermal/__init__.py
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)    17426 2024-05-31 14:53:30.000000 unthermal-0.1/unthermal/controlsys.py
-drwxr-xr-x   0 leonardo  (1000) leonardo  (1000)        0 2024-05-31 17:59:42.105609 unthermal-0.1/unthermal/experiment_files/
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)       34 2024-05-22 00:50:57.000000 unthermal-0.1/unthermal/experiment_files/DCmotor_fo_model_pbrs50.csv
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)       53 2024-05-22 00:50:57.000000 unthermal-0.1/unthermal/experiment_files/DCmotor_so_model_pbrs.csv
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)     6230 2024-05-23 13:55:05.000000 unthermal-0.1/unthermal/experiment_files/DCmotor_step_closed_exp.csv
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)       34 2024-05-23 15:07:24.000000 unthermal-0.1/unthermal/experiment_files/Thermal_fo_model_pbrs.csv
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)       53 2024-05-23 15:07:24.000000 unthermal-0.1/unthermal/experiment_files/Thermal_fotd_model_pbrs.csv
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)    82724 2024-05-22 11:22:57.000000 unthermal-0.1/unthermal/experiment_files/Thermal_prbs_open_exp.csv
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)    15218 2024-05-27 22:57:08.000000 unthermal-0.1/unthermal/experiment_files/Thermal_profile_closed_exp.csv
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)      338 2024-05-20 15:26:12.000000 unthermal-0.1/unthermal/experiment_files/Thermal_static_gain_model.csv
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)      672 2024-05-20 16:37:18.000000 unthermal-0.1/unthermal/experiment_files/Thermal_static_gain_response.csv
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)    12214 2024-05-24 21:23:31.000000 unthermal-0.1/unthermal/experiment_files/Thermal_step_closed_exp.csv
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)    22513 2024-05-31 14:53:30.000000 unthermal-0.1/unthermal/identsys.py
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)     3450 2024-05-31 16:08:19.000000 unthermal-0.1/unthermal/thermalsys.py
-drwxr-xr-x   0 leonardo  (1000) leonardo  (1000)        0 2024-05-31 17:59:42.105609 unthermal-0.1/unthermal.egg-info/
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)     2728 2024-05-31 17:59:42.000000 unthermal-0.1/unthermal.egg-info/PKG-INFO
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)      858 2024-05-31 17:59:42.000000 unthermal-0.1/unthermal.egg-info/SOURCES.txt
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)        1 2024-05-31 17:59:42.000000 unthermal-0.1/unthermal.egg-info/dependency_links.txt
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)       49 2024-05-31 17:59:42.000000 unthermal-0.1/unthermal.egg-info/requires.txt
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)       32 2024-05-31 17:59:42.000000 unthermal-0.1/unthermal.egg-info/top_level.txt
+drwxr-xr-x   0 leonardo  (1000) leonardo  (1000)        0 2024-06-01 14:17:20.275942 unthermal-0.1001/
+-rw-r--r--   0 leonardo  (1000) leonardo  (1000)     1072 2024-05-31 16:03:53.000000 unthermal-0.1001/LICENSE
+-rw-r--r--   0 leonardo  (1000) leonardo  (1000)       42 2024-05-31 15:51:11.000000 unthermal-0.1001/MANIFEST.in
+-rw-r--r--   0 leonardo  (1000) leonardo  (1000)     2748 2024-06-01 14:17:20.275942 unthermal-0.1001/PKG-INFO
+-rw-r--r--   0 leonardo  (1000) leonardo  (1000)     2259 2024-05-31 13:19:16.000000 unthermal-0.1001/README.md
+-rw-r--r--   0 leonardo  (1000) leonardo  (1000)      734 2024-06-01 14:17:07.000000 unthermal-0.1001/pyproject.toml
+-rw-r--r--   0 leonardo  (1000) leonardo  (1000)       38 2024-06-01 14:17:20.275942 unthermal-0.1001/setup.cfg
+drwxr-xr-x   0 leonardo  (1000) leonardo  (1000)        0 2024-06-01 14:17:20.275942 unthermal-0.1001/unthermal/
+-rw-r--r--   0 leonardo  (1000) leonardo  (1000)      226 2024-05-31 14:54:15.000000 unthermal-0.1001/unthermal/__init__.py
+-rw-r--r--   0 leonardo  (1000) leonardo  (1000)    17556 2024-06-01 13:59:21.000000 unthermal-0.1001/unthermal/controlsys.py
+-rw-r--r--   0 leonardo  (1000) leonardo  (1000)    22748 2024-06-01 14:15:29.000000 unthermal-0.1001/unthermal/identsys.py
+-rw-r--r--   0 leonardo  (1000) leonardo  (1000)     3553 2024-06-01 13:57:43.000000 unthermal-0.1001/unthermal/thermalsys.py
+drwxr-xr-x   0 leonardo  (1000) leonardo  (1000)        0 2024-06-01 14:17:20.275942 unthermal-0.1001/unthermal.egg-info/
+-rw-r--r--   0 leonardo  (1000) leonardo  (1000)     2748 2024-06-01 14:17:20.000000 unthermal-0.1001/unthermal.egg-info/PKG-INFO
+-rw-r--r--   0 leonardo  (1000) leonardo  (1000)      300 2024-06-01 14:17:20.000000 unthermal-0.1001/unthermal.egg-info/SOURCES.txt
+-rw-r--r--   0 leonardo  (1000) leonardo  (1000)        1 2024-06-01 14:17:20.000000 unthermal-0.1001/unthermal.egg-info/dependency_links.txt
+-rw-r--r--   0 leonardo  (1000) leonardo  (1000)       49 2024-06-01 14:17:20.000000 unthermal-0.1001/unthermal.egg-info/requires.txt
+-rw-r--r--   0 leonardo  (1000) leonardo  (1000)       32 2024-06-01 14:17:20.000000 unthermal-0.1001/unthermal.egg-info/top_level.txt
```

### Comparing `unthermal-0.1/LICENSE.txt` & `unthermal-0.1001/LICENSE`

 * *Files identical despite different names*

### Comparing `unthermal-0.1/PKG-INFO` & `unthermal-0.1001/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: unthermal
-Version: 0.1
-Summary: unthermal is a package for interacting with a real thermal plant trought IoT
+Version: 0.1001
+Summary: unthermal is a package designed for interacting with a physical thermal plant via IoT technology.
 Author-email: Leonardo Bermeo <lbermeoc@unal.edu.co>
 Project-URL: Homepage, https://github.com/nebisman/UNThermal.git
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
 Requires-Dist: iottalk-paho-mqtt
 Requires-Dist: control
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scipy
```

### Comparing `unthermal-0.1/README.md` & `unthermal-0.1001/README.md`

 * *Files identical despite different names*

### Comparing `unthermal-0.1/pyproject.toml` & `unthermal-0.1001/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "unthermal"
 authors = [{name = "Leonardo Bermeo", email = "lbermeoc@unal.edu.co"}]
-description = "unthermal is a package for interacting with a real thermal plant trought IoT"
-version = "0.1"
+description = "unthermal is a package designed for interacting with a physical thermal plant via IoT technology."
+version = "0.1001"
 readme = "README.md"
 
 requires-python = ">=3.7"
 dependencies = [
     "iottalk-paho-mqtt",
     "control",
     "numpy",
```

### Comparing `unthermal-0.1/unthermal/controlsys.py` & `unthermal-0.1001/unthermal/controlsys.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from queue import Queue
 from math import ceil
 import json
 import numpy as np
 import matplotlib.pyplot as plt
 from pathlib import Path
 from scipy.signal import cont2discrete
-from .thermalsys import PATH, ThermalSystemIoT
+from .thermalsys import ThermalSystemIoT, PATH_DATA, PATH_DEFAULT
 
 def float2hex(value):
     val_binary = struct.pack('>f', value)
     return val_binary.hex()
 
 
 def long2hex(value):
@@ -78,19 +78,19 @@
     system.publish(topic_pub, message)
     system.disconnect()
     rcode = True
     print("succesfull change of PID parameters")
     return rcode
 
 
-def step_closed(system, r0=0 , r1=100, t0=0 ,  t1=1, filepath = PATH + "Thermal_step_closed_exp.csv"):
+def step_closed(system, r0=0 , r1=100, t0=0 ,  t1=1):
     def step_message(system, userdata, message):
         q.put(message)
 
-    Path(PATH).mkdir(exist_ok=True)
+
 
     low_val = r0
     high_val = r1
     low_time = t0
     high_time = t1
     topic_pub = system.codes["USER_SYS_STEP_CLOSED"]
     topic_sub = system.codes["SYS_USER_SIGNALS_CLOSED"]
@@ -189,22 +189,22 @@
             ay.legend([line_r, line_y], [f'$r(t):$ {r_curr:0.2f}', f'$y(t):$ {y_curr: 0.3f}$~^oC$'], fontsize=16, loc="upper left")
             au.legend([line_u], [f'$u(t):$ {u_curr: 0.1f}'], fontsize=16)
             exp.append([t_curr, r_curr, y_curr, u_curr])
             plt.draw()
             plt.pause(sampling_time)
 
 
-    plt.show()
-    np.savetxt(filepath, exp, delimiter=",", fmt="%0.8f", comments="", header='t,r,y,u')
+    np.savetxt(PATH_DEFAULT + "Thermal_step_closed_exp.csv",  exp, delimiter=",", fmt="%0.8f", comments="", header='t,r,y,u')
+    np.savetxt(PATH_DATA + "Thermal_step_closed_exp.csv",  exp, delimiter=",", fmt="%0.8f", comments="", header='t,r,y,u')
     system.disconnect()
-    print("Step response completed")
+    plt.show()
     return t, r, y, u
 
 
-def stairs_closed(system, stairs=[40, 50, 60], duration=100, filepath = "stair_closed_exp.csv"):
+def stairs_closed(system, stairs=[40, 50, 60], duration=100):
     def usersignal_message(system, userdata, message):
         q.put(message)
 
     # accessing fields of system IoT
     sampling_time = system.codes["THERMAL_SAMPLING_TIME"]
     topic_pub = system.codes["USER_SYS_STAIRS_CLOSED"]
     topic_sub = system.codes["SYS_USER_SIGNALS_CLOSED"]
@@ -254,16 +254,18 @@
             u.append(u_curr)
             line_r.set_data(t, r)
             line_y.set_data(t, y)
             exp.append([t_curr, r_curr, y_curr, u_curr])
             plt.draw()
             plt.pause(0.1)
             npc += 1
-    npy.savetxt(filepath, exp, delimiter=",",
-                fmt="%0.8f", comments="", header='t,r,y,u')
+
+
+    npy.savetxt(PATH_DEFAULT + "Thermal_stairs_closed_exp.csv", exp, delimiter=",", fmt="%0.8f", comments="", header='t,r,y,u')
+    npy.savetxt(PATH_DATA + "Thermal_stairs_closed_exp.csv", exp, delimiter=",", fmt="%0.8f", comments="", header='t,r,y,u')
     system.disconnect()
     plt.show()
     return t, y, r, u
 
 
 
 def set_controller(system, controller):
@@ -385,15 +387,15 @@
 
     system.connect()
     system.publish(topic_pub, message)
     system.disconnect()
     return
 
 
-def profile_closed(system, timevalues = [0, 50, 100 , 150], refvalues = [40, 50, 60, 70], filepath=PATH+"Thermal_profile_closed_exp.csv"):
+def profile_closed(system, timevalues = [0, 50, 100 , 150], refvalues = [40, 50, 60, 70]):
     def profile_message(system, userdata, message):
         # This is the callback for receiving messages from the plant
         q.put(message)
 
     # reading the configuration parameters from the code's field in the plant
 
     topic_pub = system.codes["USER_SYS_PROFILE_CLOSED"]
@@ -519,20 +521,22 @@
             exp.append([t_curr, r_curr, y_curr, u_curr])
             plt.draw()
             plt.pause(sampling_time)
     ay.legend([line_r, line_y], ['$r(t)$ (reference)', '$y_R(t)$ (real output)'], fontsize=16,
               loc="upper left")
     au.legend([line_u], ['$u(t)$ (control signal)'], fontsize=14)
 
-    PATH1 = r'/home/leonardo/sharefolder/ProyectoSabatico/Reporte/figures/'
-    plt.savefig(PATH1 + "Thermal_profile_response.svg", bbox_inches='tight')
+
+
+    np.savetxt(PATH_DEFAULT + "Thermal_profile_closed_exp.csv", exp, delimiter=",", fmt="%0.8f",
+               comments="", header='t,r,y,u')
+    np.savetxt(PATH_DATA + "Thermal_profile_closed_exp.csv", exp, delimiter=",", fmt="%0.8f",
+               comments="", header='t,r,y,u')
     plt.show()
-    np.savetxt(filepath, exp, delimiter=",", fmt="%0.8f", comments="", header='t,r,y,u')
     system.disconnect()
-    print("Step response completed")
     return t, r, y, u
```

### Comparing `unthermal-0.1/unthermal/identsys.py` & `unthermal-0.1001/unthermal/identsys.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,34 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.integrate import odeint
 from scipy.optimize import minimize
 from scipy.interpolate import interp1d
 from scipy.stats import linregress
 import control as ct
-from .thermalsys import ThermalSystemIoT, PATH
+from .thermalsys import ThermalSystemIoT, PATH_DATA, PATH_DEFAULT
 from .controlsys import  long2hex, float2hex, hex2long, set_pid, hex2float
 import json
 from math import ceil
 from queue import Queue
 from pathlib import Path
 import csv
+from pathlib import Path
+
 
 import matplotlib
 matplotlib.use("TkAgg", force=True)
 
 
-def read_csv_file3(filepath=PATH + 'DCmotor_prbs_open_exp.csv'):
-    with open(filepath , newline='') as file:
+
+
+
+
+def read_csv_file3():
+    with open(PATH_DATA + 'Thermal_prbs_open_exp.csv', newline='') as file:
         reader = csv.reader(file)
         # Iterate over each row in the CSV file
         num_line = 0
         t = []
         u = []
         y = []
         for row in reader:
@@ -124,28 +130,31 @@
     ax.set_yticks([0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100])
     ax.grid(color='#1a1a1a40', linestyle='--', linewidth=0.25)
     line_exp, = ax.plot(uee, yee, color="#00aa00", linewidth=1, marker=r"$\circ$",markeredgewidth=0.1)
     ax.set_xlim(0, 100)
     ax.set_ylim(0, 100)
     exp = []
     y_test = np.arange(30,100, step)
-    Path(PATH).mkdir(exist_ok=True)
+
 
     for yi in y_test:
         u, y = step_closed_staticgain(system, r0=0, r1=yi, t0=0, t1=60)
         yf = np.mean(y[-15:])
         uf = np.mean(u[-15:])
         exp.append([uf, yf])
         yee.append(yf)
         uee.append(uf)
         line_exp.set_data(uee, yee)
         plt.draw()
         plt.pause(0.1)
-        np.savetxt(PATH + "Thermal_static_gain_response.csv", exp, delimiter=",", fmt="%0.8f", comments="",
-                   header='u,t')
+
+    np.savetxt(PATH_DEFAULT + "Thermal_static_gain_response.csv", exp, delimiter=",", fmt="%0.8f", comments="",
+               header='u,t')
+    np.savetxt(PATH_DATA + "Thermal_static_gain_response.csv", exp, delimiter=",", fmt="%0.8f", comments="",
+               header='u,t')
 
     res = linregress(uee, yee, alternative='greater')
     m = res.slope
     b = res.intercept
     ymod = m * np.array(uee) + b
     line_mod, = ax.plot(uee, ymod, color="#0088aaff", linewidth=1.5)
     stringmodel = r"Model:  $T_{ee}= m\,u_{ee} + b=$" + f"{m:0.2f}" + r"$\,u_{ee}+$" + f"{b:0.2f}"
@@ -154,15 +163,15 @@
                header='m,b')
     plt.show()
     system.disconnect()
     return
 
 
 
-def prbs_open(system, op_point=50, peak_amp=4, stab_time=60, uee_time=10, divider=30, filepath = "prbs_open_exp.csv"):
+def prbs_open(system, op_point=50, peak_amp=4, stab_time=60, uee_time=10, divider=30):
     def pbrs_message(system, userdata, message):
         q.put(message)
 
     topic_pub = system.codes["USER_SYS_PRBS_OPEN"]
     topic_sub = system.codes["SYS_USER_SIGNALS_OPEN"]
     sampling_time = system.codes["THERMAL_SAMPLING_TIME"]
     peak_amp_hex = float2hex(peak_amp)
@@ -272,20 +281,20 @@
                 line_y.set_data(t, y)
                 line_u.set_data(t, u)
                 txt1.set_color("#d40055")
                 txt2.set_color("#338000")
                 txt1.set_text( f'Current Temperature: {yt_curr: 0.2f}$~^oC$')
                 txt2.set_text( f'Current Input: {ut_curr:0.2f}% ({0.02475*ut_curr:0.2f} W)')
                 exp.append([tt_curr-t0, ut_curr, yt_curr])
-                np.savetxt(filepath, exp, delimiter=",",
-                           fmt="%0.8f", comments="", header='t,u,y')
+
             plt.draw()
             plt.pause(0.1)
-    # PATH1 = r'/home/leonardo/sharefolder/ProyectoSabatico/Reporte/figures/'
-    # plt.savefig(PATH1 + "Thermal_pbrs.svg", format="svg", bbox_inches="tight")
+
+    np.savetxt(PATH_DEFAULT + "prbs_open_exp.csv", exp, delimiter=",", fmt="%0.8f", comments="", header='t,u,y')
+    np.savetxt(PATH_DATA + "prbs_open_exp.csv", exp, delimiter=",", fmt="%0.8f", comments="", header='t,u,y')
     system.disconnect()
     plt.show()
     return tt, ut, yt
 
 
 
 def get_models_prbs(system, yop = 50, peak_amp= 4, usefile = True):
@@ -336,21 +345,19 @@
         return norm(ysim - ym)
 
 
     if  (yop >= 100):
          raise ValueError(f"The maximum temperature for this system is 100 degrees celsius")
 
     if usefile:
-        t,u,y = read_csv_file3(filepath = PATH + 'Thermal_prbs_open_exp.csv')
+        t, u, y = read_csv_file3()
     else:
-        t, u, y =  prbs_open(system, op_point=yop, peak_amp= peak_amp, stab_time=60, uee_time=10, divider=30, filepath = PATH + "Thermal_prbs_open_exp.csv")
-
+        t, u, y = prbs_open(system, op_point=yop, peak_amp=peak_amp, stab_time=60, uee_time=10, divider=30)
 
     m = 1.2341015052212259
-    Tenv = y[0] - m * u[0]
     ymean = np.mean(y)
     um = np.array(u) - u[0]
     ym = np.array(y) - ymean
 
     um_interp = interp1d(t, um, fill_value = (0,0 ), bounds_error=False)
 
     """Now we obtain the initial parameters for the model
@@ -432,30 +439,35 @@
     #line_ud, = au.plot(t, um_interp(np.array(t)-20) , color="#0000ff")
     modelstr1 = r"FO Model:     $G_1(s) = \frac{%0.2f }{%0.2f\,s+1}$  ($FIT = %0.1f$" % (alpha, tau, r1) + "%)"
     modelstr2 = r"FOTD Model: $G_2(s) = \frac{%0.2f  }{%0.2f\,s+1}\,e^{-%0.2f\,s}$  ($FIT = %0.1f$"%(alpha2, tau1, tau2, r2) + "%)"
     ay.set_title("Comparison of FO and FOTD models estimated with a PRBS signal at the operation point $y_{OP}=%0.1f^oC$"%yop)
     ay.legend([line_exp, line_model1, line_model2], ['Data', modelstr1, modelstr2],
               fontsize=15, loc = 'lower left',framealpha=0.95)
     au.legend([line_u], ['PRBS Input'], fontsize=14)
-    PATH1 = r'/home/leonardo/sharefolder/ProyectoSabatico/Reporte/figures/'
-    plt.savefig(PATH1 + "Thermal_pbrs.svg", format="svg", bbox_inches="tight")
-    plt.show()
-    Path(PATH).mkdir(exist_ok=True)
+    # PATH1 = r'/home/leonardo/sharefolder/ProyectoSabatico/Reporte/figures/'
+    # plt.savefig(PATH1 + "Thermal_pbrs.svg", format="svg", bbox_inches="tight")
+
     fo_model = [[alpha, tau]]
     so_model = [[alpha2, tau1, tau2]]
-    np.savetxt(PATH + "Thermal_fo_model_pbrs.csv", fo_model, delimiter=",",
+    np.savetxt(PATH_DEFAULT + "Thermal_fo_model_pbrs.csv", fo_model, delimiter=",",
                fmt="%0.8f", comments="", header='alpha, tau')
 
-    np.savetxt(PATH + "Thermal_fotd_model_pbrs.csv", so_model, delimiter=",",
+    np.savetxt(PATH_DEFAULT + "Thermal_fotd_model_pbrs.csv", so_model, delimiter=",",
+               fmt="%0.8f", comments="", header='alpha2, tau1, tau2')
+    np.savetxt(PATH_DATA + "Thermal_fo_model_pbrs.csv", fo_model, delimiter=",",
+               fmt="%0.8f", comments="", header='alpha, tau')
+
+    np.savetxt(PATH_DATA + "Thermal_fotd_model_pbrs.csv", so_model, delimiter=",",
                fmt="%0.8f", comments="", header='alpha2, tau1, tau2')
 
     system.disconnect()
+    plt.show()
     return #G1, G2
 
-def step_open(system, op_point=50, amplitude=5, high_time=200, stab_time=150, uee_time=20, filepath = "step_open_exp.csv"):
+def step_open(system, op_point=50, amplitude=5, high_time=200, stab_time=150, uee_time=20):
     def step_message(system, userdata, message):
         q.put(message)
 
     topic_pub = system.codes["USER_SYS_STEP_OPEN"]
     topic_sub = system.codes["SYS_USER_SIGNALS_OPEN"]
     sampling_time = system.codes["THERMAL_SAMPLING_TIME"]
     amp_hex = float2hex(amplitude)
@@ -564,28 +576,29 @@
                 line_y.set_data(t, y)
                 line_u.set_data(t, u)
                 txt1.set_color("#d40055")
                 txt2.set_color("#338000")
                 txt1.set_text( f'Current Temperature: {yt_curr: 0.2f}$~^oC$')
                 txt2.set_text( f'Current Input: {ut_curr:0.2f}% ({0.02475*ut_curr:0.2f} W)')
                 exp.append([tt_curr-t0, ut_curr, yt_curr])
-                np.savetxt(filepath, exp, delimiter=",",
-                           fmt="%0.8f", comments="", header='t,u,y')
+
             plt.draw()
             plt.pause(0.1)
     # PATH1 = r'/home/leonardo/sharefolder/ProyectoSabatico/Reporte/figures/'
     # plt.savefig(PATH1 + "Thermal_pbrs.svg", format="svg", bbox_inches="tight")
+    np.savetxt(PATH_DEFAULT, exp, delimiter=",",fmt="%0.8f", comments="", header='t,u,y')
+    np.savetxt(PATH_DATA, exp, delimiter=",",fmt="%0.8f", comments="", header='t,u,y')
     system.disconnect()
     plt.show()
     return tt, ut, yt
 
 
 
 def read_fo_model():
-    with open(PATH + 'Thermal_fo_model_pbrs.csv', newline='') as file:
+    with open(PATH_DATA + 'Thermal_fo_model_pbrs.csv', newline='') as file:
         reader = csv.reader(file)
         # Iterate over each row in the CSV file
         num_line = 0
         for row in reader:
             if num_line != 0:
                alpha = float(row[0])
                tau = float(row[1])
```

### Comparing `unthermal-0.1/unthermal/thermalsys.py` & `unthermal-0.1001/unthermal/thermalsys.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,16 +35,17 @@
         "USER_SYS_STEP_OPEN": "/thermal/user/thermal_" + PLANT_NUMBER + "/step_open",
         "USER_SYS_SET_GENCON": "/thermal/user/thermal_" + PLANT_NUMBER + "/set_gencon",
         "USER_SYS_PROFILE_CLOSED": "/thermal/user/thermal_" + PLANT_NUMBER + "/prof_closed",
         "THERMAL_SAMPLING_TIME" : 0.8
         }
 
 
-PATH = r"./experiment_files/"
-
+PATH_DEFAULT = r"./experiment_files/"
+PATH_DATA = str(Path(__file__).parent) + r"/datafiles/"
+Path(PATH_DEFAULT).mkdir(exist_ok=True)
 class ThermalSystemIoT:
 
     def __init__(self, broker_address = BROKER, port= PORT, user=USER, password=PASSWORD,  client_id="", clean_session=True):
         self.client = mqtt.Client()
         self.broker_address = broker_address
         self.port = port
         self.client.on_connect = self.on_connect
```

### Comparing `unthermal-0.1/unthermal.egg-info/PKG-INFO` & `unthermal-0.1001/unthermal.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: unthermal
-Version: 0.1
-Summary: unthermal is a package for interacting with a real thermal plant trought IoT
+Version: 0.1001
+Summary: unthermal is a package designed for interacting with a physical thermal plant via IoT technology.
 Author-email: Leonardo Bermeo <lbermeoc@unal.edu.co>
 Project-URL: Homepage, https://github.com/nebisman/UNThermal.git
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
 Requires-Dist: iottalk-paho-mqtt
 Requires-Dist: control
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scipy
```

