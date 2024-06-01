# Comparing `tmp/PACMAN-charge-0.2.1.tar.gz` & `tmp/PACMAN-charge-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PACMAN-charge-0.2.1.tar", last modified: Sun May 12 12:13:38 2024, max compression
+gzip compressed data, was "PACMAN-charge-1.1.0.tar", last modified: Sat Jun  1 07:12:16 2024, max compression
```

## Comparing `PACMAN-charge-0.2.1.tar` & `PACMAN-charge-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 12:13:38.933105 PACMAN-charge-0.2.1/
--rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMAN-charge-0.2.1/LICENSE
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 12:13:38.817096 PACMAN-charge-0.2.1/PACMANCharge/
--rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-29 12:12:36.000000 PACMAN-charge-0.2.1/PACMANCharge/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMAN-charge-0.2.1/PACMANCharge/atom_init.json
--rwxrwxrwx   0 root         (0) root         (0)    25766 2024-05-07 08:18:34.000000 PACMAN-charge-0.2.1/PACMANCharge/pmcharge.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 12:13:38.888097 PACMAN-charge-0.2.1/PACMAN_charge.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3191 2024-05-12 12:13:38.000000 PACMAN-charge-0.2.1/PACMAN_charge.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      318 2024-05-12 12:13:38.000000 PACMAN-charge-0.2.1/PACMAN_charge.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-12 12:13:38.000000 PACMAN-charge-0.2.1/PACMAN_charge.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      121 2024-05-12 12:13:38.000000 PACMAN-charge-0.2.1/PACMAN_charge.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2024-05-12 12:13:38.000000 PACMAN-charge-0.2.1/PACMAN_charge.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     3191 2024-05-12 12:13:38.931105 PACMAN-charge-0.2.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2801 2024-05-12 12:13:19.000000 PACMAN-charge-0.2.1/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-12 12:13:38.934105 PACMAN-charge-0.2.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      986 2024-05-12 12:12:57.000000 PACMAN-charge-0.2.1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 12:13:38.916105 PACMAN-charge-0.2.1/test/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMAN-charge-0.2.1/test/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      134 2024-05-06 03:24:19.000000 PACMAN-charge-0.2.1/test/test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 07:12:16.631754 PACMAN-charge-1.1.0/
+-rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMAN-charge-1.1.0/LICENSE
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 07:12:16.511594 PACMAN-charge-1.1.0/PACMANCharge/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-29 12:12:36.000000 PACMAN-charge-1.1.0/PACMANCharge/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMAN-charge-1.1.0/PACMANCharge/atom_init.json
+-rwxrwxrwx   0 root         (0) root         (0)    26194 2024-06-01 07:03:13.000000 PACMAN-charge-1.1.0/PACMANCharge/pmcharge.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 07:12:16.581598 PACMAN-charge-1.1.0/PACMAN_charge.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3700 2024-06-01 07:12:16.000000 PACMAN-charge-1.1.0/PACMAN_charge.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      318 2024-06-01 07:12:16.000000 PACMAN-charge-1.1.0/PACMAN_charge.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-06-01 07:12:16.000000 PACMAN-charge-1.1.0/PACMAN_charge.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      121 2024-06-01 07:12:16.000000 PACMAN-charge-1.1.0/PACMAN_charge.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-06-01 07:12:16.000000 PACMAN-charge-1.1.0/PACMAN_charge.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     3700 2024-06-01 07:12:16.625239 PACMAN-charge-1.1.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3041 2024-06-01 07:10:31.000000 PACMAN-charge-1.1.0/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-06-01 07:12:16.632753 PACMAN-charge-1.1.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1002 2024-06-01 07:04:31.000000 PACMAN-charge-1.1.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 07:12:16.610780 PACMAN-charge-1.1.0/test/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMAN-charge-1.1.0/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      134 2024-05-06 03:24:19.000000 PACMAN-charge-1.1.0/test/test.py
```

### Comparing `PACMAN-charge-0.2.1/LICENSE` & `PACMAN-charge-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.2.1/PACMANCharge/atom_init.json` & `PACMAN-charge-1.1.0/PACMANCharge/atom_init.json`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.2.1/PACMANCharge/pmcharge.py` & `PACMAN-charge-1.1.0/PACMANCharge/pmcharge.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 package_directory = os.path.abspath(__file__).replace("pmcharge.py","")
 files_to_download = {
                     'cm5.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_cm5/cm5.pth',
                     'cm5.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_cm5/normalizer-cm5.pkl',
                     'bader.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_bader/bader.pth',
                     'bader.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_bader/normalizer-bader.pkl',
                     'ddec.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_ddec/ddec.pth',
-                    'ddec.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_ddec/normalizer-ddec.pkl'
+                    'ddec.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_ddec/normalizer-ddec.pkl',
+                    'repeat.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_repeat/repeat.pth',
+                    'repeat.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_repeat/normalizer-repeat.pkl'
                     }
 
 for file_name, url in files_to_download.items():
     file_path = os.path.join(package_directory, file_name)
     if not os.path.exists(file_path):
         response = requests.get(url)
         if response.status_code == 200:
@@ -205,16 +207,16 @@
                 cc = c - sum_chg/len(chg)
                 charges.append(round(cc, dia))
         else:
             for c in chg:
                 charges.append(round(c, dia))
     with open(name + ".cif", 'r') as file:
         lines = file.readlines()
-    lines[0] = "# generated by PACMAN-" +charge_type+" charge (https://github.com/sxm13/PACMAN/)\n"
-    lines[1] = "data_structure\n"
+    lines[0] = "# " + charge_type + " charges by PACMAN v1.1 (https://github.com/mtap-research/PACMAN-charge/)\n"
+    lines[1] = "data_"+name.split("/")[-1]+"_pacman\n"
     for i, line in enumerate(lines):
         if '_atom_site_occupancy' in line:
             lines.insert(i + 1, " _atom_site_charge\n")
             break
     charge_index = 0
     for j in range(i + 2, len(lines)):
         if charge_index < len(charges):
@@ -486,25 +488,28 @@
         N,_ = atom_fea.shape
         for conv_func in self.convs:
             nbr_fea,atom_fea,global_fea = conv_func(atom_fea,nbr_fea,nbr_fea_idx1,nbr_fea_idx2,num_nbrs,crystal_atom_idx)          
         global_fea = global_fea / atom_nums
         z = self.phi_u(global_fea)
         return z
 
-def predict(cif_file,charge_type="DDEC6",digits=6,atom_type=False,neutral=False):
+def predict(cif_file,charge_type="DDEC6",digits=6,atom_type=True,neutral=True):
    
     if charge_type == "DDEC6":
         charge_model_name = package_directory + 'ddec.pth'
         nor_name = package_directory + 'ddec.pkl'
     elif charge_type == "Bader":
         charge_model_name = package_directory + 'bader.pth'
         nor_name = package_directory + 'bader.pkl'
     elif charge_type == "CM5":
         charge_model_name = package_directory + 'cm5.pth'
         nor_name = package_directory + 'cm5.pkl'
+    elif charge_type == "REPEAT":
+        charge_model_name = package_directory + 'repeat.pth'
+        nor_name = package_directory + 'repeat.pkl'
     
     try:
         with open(nor_name, 'rb') as f:
             charge_nor = pickle.load(f)
         f.close()
     except FileNotFoundError:
         print(f"Please use correct charge")
```

### Comparing `PACMAN-charge-0.2.1/PACMAN_charge.egg-info/PKG-INFO` & `PACMAN-charge-1.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,47 @@
-Metadata-Version: 2.1
-Name: PACMAN-charge
-Version: 0.2.1
-Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
-Home-page: https://github.com/sxm13/PACMAN
-Author: Guobin Zhao
-Author-email: sxmzhaogb@gmai.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<h1 align="center">PACMAN</h1>
-
-<h4 align="center">
-
-</h4>              
-
-A **P**artial **A**tomic **C**harge Predicter for Porous **Ma**terials based on Graph Convolutional Neural **N**etwork (**PACMAN**)   
-
-[![Requires Python 3.9](https://img.shields.io/badge/Python-3.9-blue.svg?logo=python&logoColor=white)](https://python.org/downloads) [![Zenodo](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.10822403-blue)](https://doi.org/10.5281/zenodo.10822403)  [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/sxm13/PACMAN/LICENSE.txt) [![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sxmzhaogb@gmail.com) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)]() [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)]()          
-
-
-# Usage
-
-```sh      
-from PACMANCharge import pmcharge
-pmcharge.predict(cif_file="./test/Cu-BTC.cif",charge_type="DDEC6",digits=6,atom_type=False,neutral=False)
-```
-
-* cif_file: cif file (without partial atomic charges) **[cif path]**                                                            
-* charge-type (default: DDE6): DDEC6, Bader or CM5                                        
-* digits (default: 6): number of decimal places to print for partial atomic charges. ML models were trained on a 6-digit dataset.                                                                     
-* atom-type (default: False): keep the same partial atomic charge for the same atom types (based on the similarity of partial atomic charges up to 2 decimal places).                                                         
-* neutral (default: False): keep the net charge is zero. We use "mean" method to neuralize the system where the excess charges are equally distributed across all atoms.                                                                            
-
-# Website & Zenodo
-PACMAN-APP[link](https://gcn-charge-predicter-mtap.streamlit.app/)       
-DOWNLOAD full code and dataset[link](https://zenodo.org/records/10822403) But we will not update new vesion in Zenodo.            
-
-# Reference
-If you use PACMAN Charge, please cite this paper:
-```
-@article{,
-    title={PACMAN: A Robust Partial Atomic Charge Predicter for Nanoporous Materials using Crystal Graph Convolution Network},
-    author={Zhao, Guobin and Chung, Yongchul},
-    year={2024},
-}
-```
-
-# Bugs
-
-If you encounter any problem during using ***PACMAN***, please email ```sxmzhaogb@gmail.com```.                 
-
- 
-**Group:**   [Molecular Thermodynamics & Advance Processes Laboratory](https://sites.google.com/view/mtap-lab/home?authuser=0)                                
+<h1 align="center">PACMAN</h1>
+
+<h4 align="center">
+
+</h4>              
+
+A **P**artial **A**tomic **C**harge Predicter for Porous **Ma**terials based on Graph Convolutional Neural **N**etwork (**PACMAN**)   
+
+[![Requires Python 3.9](https://img.shields.io/badge/Python-3.9-blue.svg?logo=python&logoColor=white)](https://python.org/downloads) [![Zenodo](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.10822403-blue)](https://doi.org/10.5281/zenodo.10822403)  [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/mtap-research/PACMAN-charge/LICENSE) [![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sxmzhaogb@gmail.com) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)]() [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)]()          
+
+
+# Usage
+
+```sh      
+from PACMANCharge import pmcharge
+pmcharge.predict(cif_file="./test/Cu-BTC.cif",charge_type="DDEC6",digits=6,atom_type=False,neutral=False)
+```
+
+* cif_file: cif file (without partial atomic charges) **[cif path]**                                                            
+* charge-type (default: DDE6): DDEC6, Bader, CM5 or REPEAT                                         
+* digits (default: 6): number of decimal places to print for partial atomic charges. ML models were trained on a 6-digit dataset.                                                                     
+* atom-type (default: True): keep the same partial atomic charge for the same atom types (based on the similarity of partial atomic charges up to 2 decimal places).                                                         
+* neutral (default: True): keep the net charge is zero. We use "mean" method to neuralize the system where the excess charges are equally distributed across all atoms.                                                                            
+
+# Website & Zenodo
+PACMAN-APP[link](https://pacman-charge-mtap.streamlit.app/)       
+github repository[link](https://github.com/mtap-research/PACMAN-charge)                                                                          
+DOWNLOAD full code and dataset[link](https://zenodo.org/records/10822403) But we will not update new vesion in Zenodo.            
+
+# Reference
+If you use PACMAN Charge, please cite this paper:
+```
+@article{,
+    title={PACMAN: A Robust Partial Atomic Charge Predicter for Nanoporous Materials based on Crystal Graph Convolution Network},
+    author={Zhao, Guobin and Chung, Yongchul},
+    journal={Journal of Chemical Theory and Computation},
+    year={2024},
+    DOI={10.1021/acs.jctc.4c00434}
+}
+```
+
+# Bugs
+
+If you encounter any problem during using ***PACMAN***, please email ```sxmzhaogb@gmail.com```.                 
+
+ 
+**Group:**   [Molecular Thermodynamics & Advance Processes Laboratory](https://sites.google.com/view/mtap-lab)
```

### Comparing `PACMAN-charge-0.2.1/PKG-INFO` & `PACMAN-charge-1.1.0/PACMAN_charge.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,69 @@
 Metadata-Version: 2.1
 Name: PACMAN-charge
-Version: 0.2.1
+Version: 1.1.0
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
-Home-page: https://github.com/sxm13/PACMAN
+Home-page: https://github.com/mtap-research/PACMAN-charge/
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: numpy>=1.13.3
+Requires-Dist: pymatgen>=2018.6.11
+Requires-Dist: ase>=3.19
+Requires-Dist: tqdm>=4.15
+Requires-Dist: pandas>=0.20.3
+Requires-Dist: scikit-learn>=0.19.1
+Requires-Dist: joblib>=0.13.2
+Requires-Dist: torch
 
 <h1 align="center">PACMAN</h1>
 
 <h4 align="center">
 
 </h4>              
 
 A **P**artial **A**tomic **C**harge Predicter for Porous **Ma**terials based on Graph Convolutional Neural **N**etwork (**PACMAN**)   
 
-[![Requires Python 3.9](https://img.shields.io/badge/Python-3.9-blue.svg?logo=python&logoColor=white)](https://python.org/downloads) [![Zenodo](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.10822403-blue)](https://doi.org/10.5281/zenodo.10822403)  [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/sxm13/PACMAN/LICENSE.txt) [![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sxmzhaogb@gmail.com) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)]() [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)]()          
+[![Requires Python 3.9](https://img.shields.io/badge/Python-3.9-blue.svg?logo=python&logoColor=white)](https://python.org/downloads) [![Zenodo](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.10822403-blue)](https://doi.org/10.5281/zenodo.10822403)  [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/mtap-research/PACMAN-charge/LICENSE) [![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sxmzhaogb@gmail.com) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)]() [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)]()          
 
 
 # Usage
 
 ```sh      
 from PACMANCharge import pmcharge
 pmcharge.predict(cif_file="./test/Cu-BTC.cif",charge_type="DDEC6",digits=6,atom_type=False,neutral=False)
 ```
 
 * cif_file: cif file (without partial atomic charges) **[cif path]**                                                            
-* charge-type (default: DDE6): DDEC6, Bader or CM5                                        
+* charge-type (default: DDE6): DDEC6, Bader, CM5 or REPEAT                                         
 * digits (default: 6): number of decimal places to print for partial atomic charges. ML models were trained on a 6-digit dataset.                                                                     
-* atom-type (default: False): keep the same partial atomic charge for the same atom types (based on the similarity of partial atomic charges up to 2 decimal places).                                                         
-* neutral (default: False): keep the net charge is zero. We use "mean" method to neuralize the system where the excess charges are equally distributed across all atoms.                                                                            
+* atom-type (default: True): keep the same partial atomic charge for the same atom types (based on the similarity of partial atomic charges up to 2 decimal places).                                                         
+* neutral (default: True): keep the net charge is zero. We use "mean" method to neuralize the system where the excess charges are equally distributed across all atoms.                                                                            
 
 # Website & Zenodo
-PACMAN-APP[link](https://gcn-charge-predicter-mtap.streamlit.app/)       
+PACMAN-APP[link](https://pacman-charge-mtap.streamlit.app/)       
+github repository[link](https://github.com/mtap-research/PACMAN-charge)                                                                          
 DOWNLOAD full code and dataset[link](https://zenodo.org/records/10822403) But we will not update new vesion in Zenodo.            
 
 # Reference
 If you use PACMAN Charge, please cite this paper:
 ```
 @article{,
-    title={PACMAN: A Robust Partial Atomic Charge Predicter for Nanoporous Materials using Crystal Graph Convolution Network},
+    title={PACMAN: A Robust Partial Atomic Charge Predicter for Nanoporous Materials based on Crystal Graph Convolution Network},
     author={Zhao, Guobin and Chung, Yongchul},
+    journal={Journal of Chemical Theory and Computation},
     year={2024},
+    DOI={10.1021/acs.jctc.4c00434}
 }
 ```
 
 # Bugs
 
 If you encounter any problem during using ***PACMAN***, please email ```sxmzhaogb@gmail.com```.                 
 
  
-**Group:**   [Molecular Thermodynamics & Advance Processes Laboratory](https://sites.google.com/view/mtap-lab/home?authuser=0)                                
+**Group:**   [Molecular Thermodynamics & Advance Processes Laboratory](https://sites.google.com/view/mtap-lab)
```

### Comparing `PACMAN-charge-0.2.1/setup.py` & `PACMAN-charge-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import requests
 from setuptools import setup, find_packages
 
 setup(
     name="PACMAN-charge",
-    version="0.2.1",
+    version="1.1.0",
     packages=find_packages(),
     description="Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)",
     author="Guobin Zhao",
     author_email="sxmzhaogb@gmai.com",
-    url="https://github.com/sxm13/PACMAN",
+    url="https://github.com/mtap-research/PACMAN-charge/",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     include_package_data=True,
     package_data={
         'PACMANCharge': ['*.json']
     },
     license="MIT",
```

