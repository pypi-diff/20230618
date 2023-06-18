# Comparing `tmp/aqme-1.5.0.tar.gz` & `tmp/aqme-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqme-1.5.0.tar", last modified: Tue May 23 11:31:27 2023, max compression
+gzip compressed data, was "aqme-1.5.1.tar", last modified: Sun Jun 18 09:03:47 2023, max compression
```

## Comparing `aqme-1.5.0.tar` & `aqme-1.5.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 11:31:27.245301 aqme-1.5.0/
--rw-rw-rw-   0        0        0     1086 2022-09-14 16:11:15.000000 aqme-1.5.0/LICENSE
--rw-rw-rw-   0        0        0     1035 2023-05-23 11:31:27.245301 aqme-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3419 2023-03-06 16:00:20.000000 aqme-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 11:31:27.211067 aqme-1.5.0/aqme/
--rw-rw-rw-   0        0        0        0 2022-09-14 16:11:15.000000 aqme-1.5.0/aqme/__init__.py
--rw-rw-rw-   0        0        0      628 2022-09-14 16:11:15.000000 aqme-1.5.0/aqme/__main__.py
--rw-rw-rw-   0        0        0     9791 2023-05-01 11:11:50.000000 aqme-1.5.0/aqme/aqme.py
--rw-rw-rw-   0        0        0     3586 2023-05-01 11:11:41.000000 aqme-1.5.0/aqme/argument_parser.py
--rw-rw-rw-   0        0        0    24365 2023-04-30 17:05:33.000000 aqme-1.5.0/aqme/cmin.py
--rw-rw-rw-   0        0        0     1503 2022-12-10 12:38:42.000000 aqme-1.5.0/aqme/cmin_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-23 11:31:27.232044 aqme-1.5.0/aqme/csearch/
--rw-rw-rw-   0        0        0       37 2022-12-06 18:50:02.000000 aqme-1.5.0/aqme/csearch/__init__.py
--rw-rw-rw-   0        0        0    49308 2023-03-15 18:15:42.000000 aqme-1.5.0/aqme/csearch/base.py
--rw-rw-rw-   0        0        0    24815 2023-03-16 10:06:51.000000 aqme-1.5.0/aqme/csearch/crest.py
--rw-rw-rw-   0        0        0     8237 2023-01-31 07:17:56.000000 aqme-1.5.0/aqme/csearch/fullmonte.py
--rw-rw-rw-   0        0        0    15621 2023-02-05 12:34:12.000000 aqme-1.5.0/aqme/csearch/templates.py
--rw-rw-rw-   0        0        0    16736 2023-04-30 17:05:33.000000 aqme-1.5.0/aqme/csearch/utils.py
--rw-rw-rw-   0        0        0    20614 2022-12-09 18:04:27.000000 aqme-1.5.0/aqme/filter.py
--rw-rw-rw-   0        0        0    41399 2023-04-30 17:08:10.000000 aqme-1.5.0/aqme/qcorr.py
--rw-rw-rw-   0        0        0    24886 2023-03-12 08:17:09.000000 aqme-1.5.0/aqme/qcorr_utils.py
--rw-rw-rw-   0        0        0    26177 2023-05-01 14:27:23.000000 aqme-1.5.0/aqme/qdescp.py
--rw-rw-rw-   0        0        0    15665 2023-05-01 14:25:40.000000 aqme-1.5.0/aqme/qdescp_utils.py
--rw-rw-rw-   0        0        0    20608 2023-04-30 17:08:42.000000 aqme-1.5.0/aqme/qprep.py
-drwxrwxrwx   0        0        0        0 2023-05-23 11:31:27.234456 aqme-1.5.0/aqme/templates/
--rw-rw-rw-   0        0        0      354 2022-09-14 16:11:15.000000 aqme-1.5.0/aqme/templates/template-2.sdf
--rw-rw-rw-   0        0        0      448 2022-09-14 16:11:15.000000 aqme-1.5.0/aqme/templates/template-3.sdf
--rw-rw-rw-   0        0        0      640 2022-09-14 16:11:15.000000 aqme-1.5.0/aqme/templates/template-4-and-5.sdf
--rw-rw-rw-   0        0        0    27517 2023-05-01 11:04:52.000000 aqme-1.5.0/aqme/utils.py
--rw-rw-rw-   0        0        0     4486 2023-04-30 17:05:33.000000 aqme-1.5.0/aqme/vismol.py
-drwxrwxrwx   0        0        0        0 2023-05-23 11:31:27.215276 aqme-1.5.0/aqme.egg-info/
--rw-rw-rw-   0        0        0     1035 2023-05-23 11:31:26.000000 aqme-1.5.0/aqme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      746 2023-05-23 11:31:27.000000 aqme-1.5.0/aqme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 11:31:26.000000 aqme-1.5.0/aqme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-05-23 11:31:26.000000 aqme-1.5.0/aqme.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-23 11:31:26.000000 aqme-1.5.0/aqme.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      118 2023-05-23 11:31:27.245301 aqme-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1882 2023-05-23 11:26:58.000000 aqme-1.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 11:31:27.245301 aqme-1.5.0/tests/
--rw-rw-rw-   0        0        0     2948 2023-04-30 17:05:33.000000 aqme-1.5.0/tests/test_cmin.py
--rw-rw-rw-   0        0        0    28035 2023-03-06 09:24:52.000000 aqme-1.5.0/tests/test_csearch.py
--rw-rw-rw-   0        0        0    34526 2023-03-18 10:55:19.000000 aqme-1.5.0/tests/test_qcorr.py
--rw-rw-rw-   0        0        0     7360 2023-03-06 09:24:03.000000 aqme-1.5.0/tests/test_qdescp.py
--rw-rw-rw-   0        0        0    19952 2023-03-13 07:06:58.000000 aqme-1.5.0/tests/test_qprep.py
+drwxrwxrwx   0        0        0        0 2023-06-18 09:03:47.681054 aqme-1.5.1/
+-rw-rw-rw-   0        0        0     1086 2022-09-14 16:11:15.000000 aqme-1.5.1/LICENSE
+-rw-rw-rw-   0        0        0     1035 2023-06-18 09:03:47.681054 aqme-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3419 2023-06-17 19:42:28.000000 aqme-1.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 09:03:47.637537 aqme-1.5.1/aqme/
+-rw-rw-rw-   0        0        0        0 2022-09-14 16:11:15.000000 aqme-1.5.1/aqme/__init__.py
+-rw-rw-rw-   0        0        0      628 2022-09-14 16:11:15.000000 aqme-1.5.1/aqme/__main__.py
+-rw-rw-rw-   0        0        0    10222 2023-06-17 19:42:28.000000 aqme-1.5.1/aqme/aqme.py
+-rw-rw-rw-   0        0        0     3702 2023-06-17 19:42:28.000000 aqme-1.5.1/aqme/argument_parser.py
+-rw-rw-rw-   0        0        0    23871 2023-06-17 19:42:28.000000 aqme-1.5.1/aqme/cmin.py
+-rw-rw-rw-   0        0        0     1503 2023-06-17 19:42:28.000000 aqme-1.5.1/aqme/cmin_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-18 09:03:47.660690 aqme-1.5.1/aqme/csearch/
+-rw-rw-rw-   0        0        0       37 2023-06-17 19:42:28.000000 aqme-1.5.1/aqme/csearch/__init__.py
+-rw-rw-rw-   0        0        0    58613 2023-06-17 19:42:28.000000 aqme-1.5.1/aqme/csearch/base.py
+-rw-rw-rw-   0        0        0    25064 2023-06-17 19:42:28.000000 aqme-1.5.1/aqme/csearch/crest.py
+-rw-rw-rw-   0        0        0     8237 2023-06-17 19:42:28.000000 aqme-1.5.1/aqme/csearch/fullmonte.py
+-rw-rw-rw-   0        0        0    15621 2023-06-17 19:42:28.000000 aqme-1.5.1/aqme/csearch/templates.py
+-rw-rw-rw-   0        0        0    17379 2023-06-17 19:42:28.000000 aqme-1.5.1/aqme/csearch/utils.py
+-rw-rw-rw-   0        0        0    18619 2023-06-17 19:42:28.000000 aqme-1.5.1/aqme/filter.py
+-rw-rw-rw-   0        0        0    41350 2023-06-17 19:42:28.000000 aqme-1.5.1/aqme/qcorr.py
+-rw-rw-rw-   0        0        0    24886 2023-06-17 19:42:28.000000 aqme-1.5.1/aqme/qcorr_utils.py
+-rw-rw-rw-   0        0        0    31628 2023-06-17 19:42:28.000000 aqme-1.5.1/aqme/qdescp.py
+-rw-rw-rw-   0        0        0    16342 2023-06-17 19:42:28.000000 aqme-1.5.1/aqme/qdescp_utils.py
+-rw-rw-rw-   0        0        0    20608 2023-06-17 19:42:28.000000 aqme-1.5.1/aqme/qprep.py
+drwxrwxrwx   0        0        0        0 2023-06-18 09:03:47.665295 aqme-1.5.1/aqme/templates/
+-rw-rw-rw-   0        0        0      354 2022-09-14 16:11:15.000000 aqme-1.5.1/aqme/templates/template-2.sdf
+-rw-rw-rw-   0        0        0      448 2022-09-14 16:11:15.000000 aqme-1.5.1/aqme/templates/template-3.sdf
+-rw-rw-rw-   0        0        0      640 2022-09-14 16:11:15.000000 aqme-1.5.1/aqme/templates/template-4-and-5.sdf
+-rw-rw-rw-   0        0        0    27978 2023-06-18 09:03:42.000000 aqme-1.5.1/aqme/utils.py
+-rw-rw-rw-   0        0        0     4486 2023-06-17 19:42:28.000000 aqme-1.5.1/aqme/vismol.py
+drwxrwxrwx   0        0        0        0 2023-06-18 09:03:47.649196 aqme-1.5.1/aqme.egg-info/
+-rw-rw-rw-   0        0        0     1035 2023-06-18 09:03:47.000000 aqme-1.5.1/aqme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      746 2023-06-18 09:03:47.000000 aqme-1.5.1/aqme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 09:03:47.000000 aqme-1.5.1/aqme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-06-18 09:03:47.000000 aqme-1.5.1/aqme.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-18 09:03:47.000000 aqme-1.5.1/aqme.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      118 2023-06-18 09:03:47.681054 aqme-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1889 2023-06-18 09:03:30.000000 aqme-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 09:03:47.679544 aqme-1.5.1/tests/
+-rw-rw-rw-   0        0        0     2948 2023-06-17 19:42:28.000000 aqme-1.5.1/tests/test_cmin.py
+-rw-rw-rw-   0        0        0    28035 2023-06-17 19:42:28.000000 aqme-1.5.1/tests/test_csearch.py
+-rw-rw-rw-   0        0        0    35938 2023-06-17 19:42:28.000000 aqme-1.5.1/tests/test_qcorr.py
+-rw-rw-rw-   0        0        0    11792 2023-06-17 19:42:28.000000 aqme-1.5.1/tests/test_qdescp.py
+-rw-rw-rw-   0        0        0    19952 2023-06-17 19:42:28.000000 aqme-1.5.1/tests/test_qprep.py
```

### Comparing `aqme-1.5.0/LICENSE` & `aqme-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aqme-1.5.0/PKG-INFO` & `aqme-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aqme
-Version: 1.5.0
+Version: 1.5.1
 Summary: Automated Quantum Mechanical Environments
 Home-page: https://github.com/jvalegre/aqme
-Download-URL: https://github.com/jvalegre/aqme/archive/refs/tags/1.5.0.tar.gz
+Download-URL: https://github.com/jvalegre/aqme/archive/refs/tags/1.5.1.tar.gz
 Author: Shree Sowndarya S. V., Juan V. Alegre Requena
 Author-email: svss@colostate.edu, jvalegre@unizar.es
 License: MIT
 Keywords: workflows,computational chemistry,conformational sampling,cheminformatics,quantum mechanics,DFT,automated
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `aqme-1.5.0/README.md` & `aqme-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `aqme-1.5.0/aqme/__main__.py` & `aqme-1.5.1/aqme/__main__.py`

 * *Files identical despite different names*

### Comparing `aqme-1.5.0/aqme/aqme.py` & `aqme-1.5.1/aqme/aqme.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     except ModuleNotFoundError:
         print("x  RDKit is not installed! You can install the program with 'conda install -c conda-forge rdkit'")
         sys.exit()
 
     # CSEARCH
     if args.csearch:
         csearch(
+            verbose=args.verbose,
             input=args.input,
             command_line=args.command_line,
             smi=args.smi,
             name=args.name,
             w_dir_main=args.w_dir_main,
             destination=args.destination,
             charge=args.charge,
@@ -105,24 +106,30 @@
             ewin_fullmonte=args.ewin_fullmonte,
             ewin_sample_fullmonte=args.ewin_sample_fullmonte,
             nsteps_fullmonte=args.nsteps_fullmonte,
             nrot_fullmonte=args.nrot_fullmonte,
             ang_fullmonte=args.ang_fullmonte,
             crest_keywords=args.crest_keywords,
             xtb_keywords=args.xtb_keywords,
-            angle_off=args.angle_off,
+            geom=args.geom,
+            bond_thres=args.bond_thres,
+            angle_thres=args.angle_thres,
+            dihedral_thres=args.dihedral_thres,
             nprocs=args.nprocs,
             cregen=args.cregen,
             cregen_keywords=args.cregen_keywords,
             crest_force=args.crest_force,
+            crest_nrun=args.crest_nrun,
+            crest_nclust=args.crest_nclust,
         )
 
     # CMIN
     if args.cmin:
         cmin(
+            verbose=args.verbose,
             files=args.files,
             command_line=args.command_line,
             w_dir_main=args.w_dir_main,
             destination=args.destination,
             varfile=args.varfile,
             nprocs=args.nprocs,
             program=args.program,
@@ -146,14 +153,15 @@
             prefix=args.prefix,
             suffix=args.suffix,
         )
 
     # QPREP
     if args.qprep:
         qprep(
+            verbose=args.verbose,
             files=args.files,
             command_line=args.command_line,
             atom_types=args.atom_types,
             cartesians=args.cartesians,
             w_dir_main=args.w_dir_main,
             destination=args.destination,
             varfile=args.varfile,
@@ -174,14 +182,15 @@
             lowest_n = args.lowest_n,
             e_threshold_qprep= args.e_threshold_qprep,
         )
 
     # QCORR
     if args.qcorr:
         qcorr(
+            verbose=args.verbose,
             files=args.files,
             command_line=args.command_line,
             w_dir_main=args.w_dir_main,
             fullcheck=args.fullcheck,
             varfile=args.varfile,
             ifreq_cutoff=args.ifreq_cutoff,
             amplitude_ifreq=args.amplitude_ifreq,
@@ -205,29 +214,31 @@
             bs_nogen=args.bs_nogen,
             nodup_check=args.nodup_check,
         )
 
     # QDESCP
     if args.qdescp:
         qdescp(
+            verbose=args.verbose,
+            command_line=args.command_line,
             w_dir_main=args.w_dir_main,
             destination=args.destination,
             files=args.files,
             charge=args.charge,
             mult=args.mult,
             program=args.program,
             qdescp_temp=args.qdescp_temp,
             qdescp_acc=args.qdescp_acc,
             qdescp_solvent=args.qdescp_solvent,
             boltz=args.boltz,
             nmr_atoms=args.nmr_atoms,
             nmr_slope=args.nmr_slope,
             nmr_intercept=args.nmr_intercept,
             nmr_experim=args.nmr_experim,
-            qdescp_atom=args.qdescp_atom,
+            qdescp_atoms=args.qdescp_atoms,
             dbstep_r=args.dbstep_r,
             robert=args.robert,
             csv_name=args.csv_name
         )
 
 
 if __name__ == "__main__":
```

### Comparing `aqme-1.5.0/aqme/argument_parser.py` & `aqme-1.5.1/aqme/argument_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #      This file contains the argument parser         #
 #####################################################.
 
 import os
 
 var_dict = {
     "varfile": None,
+    "verbose": True,
     "input": "",
     "output_name": "output",
     "command_line": False,
     "name": None,
     "path": "",
     "output": ".sdf",
     "csearch": False,
@@ -86,33 +87,37 @@
     "s2_threshold": 10.0,
     "isom_type": None,
     "isom_inputs": os.getcwd(),
     "vdwfrac": 0.5,
     "covfrac": 1.1,
     "fullcheck": True,
     "suffix": "",
-    "geom_rules": [],
-    "angle_off": 30,
+    "geom": [],
+    "bond_thres": 0.2,
+    "angle_thres": 30,
+    "dihedral_thres": 30,
     "crest_keywords": None,
     "crest_force": 0.5,
     "prefix": "",
     "qdescp": False,
     "qdescp_temp": 300,
     "qdescp_acc": 0.2,
     "qdescp_solvent": None,
     "boltz": True,
     "nmr_atoms": [6, 1],  # [C,H]
     "nmr_slope": [-1.0537, -1.0784],  # [C,H]
     "nmr_intercept": [181.7815,31.8723],  # [C,H]
     "nmr_experim": None,
     "nodup_check": False,
-    "qdescp_atom": None,
+    "qdescp_atoms": [],
     "dbstep_r": 3.5,
     "robert": True,
-    "csv_name": None
+    "csv_name": None,
+    "crest_nrun": 1,
+    "crest_nclust": 0.4
 }
 
 
 # part for using the options in a script or jupyter notebook
 class options_add:
     pass
```

### Comparing `aqme-1.5.0/aqme/cmin.py` & `aqme-1.5.1/aqme/cmin.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,17 +97,17 @@
 from rdkit.Chem.PropertyMol import PropertyMol
 from progress.bar import IncrementalBar
 from rdkit.Geometry import Point3D
 import pandas as pd
 import time
 from aqme.utils import (
     load_variables,
-    substituted_mol,
     mol_from_sdf_or_mol_or_mol2,
-    add_prefix_suffix
+    add_prefix_suffix,
+    check_xtb
 )
 from aqme.filter import ewin_filter, pre_E_filter, RMSD_and_E_filter
 from aqme.cmin_utils import creation_of_dup_csv_cmin
 from aqme.csearch.crest import xtb_opt_main
 from aqme.csearch.utils import prepare_com_files
 
 hartree_to_kcal = 627.509
@@ -136,14 +136,18 @@
             if self.args.program.lower() not in ["xtb", "ani"]:
                 cmin_program = False
         if not cmin_program:
             self.args.log.write('\nx  Program not supported for CMIN refinement! Specify: program="xtb" (or "ani")')
             self.args.log.finalize()
             sys.exit()
 
+        # check if xTB is installed
+        if self.args.program.lower() == "xtb":
+            _ = check_xtb(self)
+
         # retrieves the different files to run in CMIN
         if len(self.args.files) == 0:
             self.args.log.write('\nx  No files were found! Make sure you use quotation marks if you are using * (i.e. --files "*.sdf")')
             self.args.log.finalize()
             sys.exit()
 
         # create the dataframe to store the data
@@ -215,15 +219,16 @@
             frames = [self.final_dup_data, total_data]
             self.final_dup_data = pd.concat(frames, ignore_index=True, sort=True)
             bar.next()
         bar.finish()
         
         # store all the information into a CSV file
         cmin_csv_file = self.args.w_dir_main.joinpath("CMIN-Data.csv")
-        self.final_dup_data.to_csv(cmin_csv_file, index=False)
+        if self.args.verbose:
+            self.final_dup_data.to_csv(cmin_csv_file, index=False)
 
         elapsed_time = round(time.time() - start_time_overall, 2)
         self.args.log.write(f"\nTime CMIN: {elapsed_time} seconds\n")
         self.args.log.finalize()
 
         # delete extra temporary files created when using XYZ, GJF, COM and PDB files
         if file_format.lower() in ['.xyz', '.gjf', '.com', '.pdb']:
@@ -310,29 +315,29 @@
                     mol, energy, cmin_valid = self.ani_optimize(mol,charge,mult)
                 # xTB calculations use the xTB program directly
                 elif self.args.program.lower() == "xtb":
                     # for contrained optimizations
                     complex_ts = False
                     if len(self.args.constraints_atoms) >= 1 or len(self.args.constraints_dist) >= 1 or len(self.args.constraints_angle) >= 1 or len(self.args.constraints_dihedral) >= 1:
                         complex_ts = True
-                    # name_init = str(open(file, "r").readlines()[0].strip())
                     name_init = mol.GetProp('_Name')
-                    # print(name_init)
                     mol, energy, cmin_valid = xtb_opt_main(
                         f'{self.name}_conf_{i}',
                         dup_data,
                         dup_data_idx,
                         self,
                         charge,
                         mult,
+                        None,
                         self.args.constraints_atoms,
                         self.args.constraints_dist,
                         self.args.constraints_angle,
                         self.args.constraints_dihedral,
                         'xtb',
+                        self.args.geom,
                         complex_ts=complex_ts,
                         mol=mol,
                         name_init=name_init
                     )
                 if cmin_valid:
                     pmol = PropertyMol(mol)
                     outmols.append(pmol)
@@ -418,18 +423,18 @@
         ]
         for file in temp_files:
             if os.path.exists(file):
                 os.remove(file)
 
         return dup_data
 
-    # xTB AND ANI MAIN OPTIMIZATION PROCESS
+    # ANI MAIN OPTIMIZATION PROCESS
     def ani_optimize(self, mol, charge, mult):
 
-        # Attempts ANI/xTB imports and exits if the programs are not installed
+        # Attempts ANI imports and exits if the programs are not installed
         try:
             import torch
             import warnings
             warnings.filterwarnings('ignore')
 
         except ModuleNotFoundError:
             self.args.log.write("x  Torch-related modules are not installed! You can install these modules with 'pip install torch torchvision torchani'")
@@ -506,35 +511,22 @@
 
     # generate the CMIN optimization model
     def get_cmin_model(self):
         """
         Function to generate the optimization model for CMIN (using xTB or ANI methods)
         """
 
-        if self.args.program.lower() == "ani":
-            try:
-                import torchani
-            except (ImportError,ModuleNotFoundError):
-                self.args.log.write("x  Torchani is not installed! You can install the program with 'pip install torchani'")
-                self.args.log.finalize()
-                sys.exit()
-
-            model = getattr(torchani.models,self.args.ani_method)()
+        try:
+            import torchani
+        except (ImportError,ModuleNotFoundError):
+            self.args.log.write("x  Torchani is not installed! You can install the program with 'pip install torchani'")
+            self.args.log.finalize()
+            sys.exit()
 
-        elif self.args.program.lower() == "xtb":
-            try:
-                subprocess.run(
-                    ["xtb", "-h"], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
-                )
-            except FileNotFoundError:
-                self.args.log.write("x  xTB is not installed (CREST cannot be used)! You can install the program with 'conda install -c conda-forge xtb'")
-                self.args.log.finalize()
-                sys.exit()
-    
-            model = None
+        model = getattr(torchani.models,self.args.ani_method)()
 
         return model
 
     # write SDF files for xTB and ANI
     def write_confs(self, conformers, selectedcids, log):
         if len(conformers) > 0:
             write_confs = 0
```

### Comparing `aqme-1.5.0/aqme/cmin_utils.py` & `aqme-1.5.1/aqme/cmin_utils.py`

 * *Files identical despite different names*

### Comparing `aqme-1.5.0/aqme/csearch/base.py` & `aqme-1.5.1/aqme/csearch/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -82,14 +82,24 @@
       (in g/mol). If 0 is set, this filter is off
    max_torsions : int, default=0
       Discard systems with more than this many torsions (relevant to avoid 
       molecules with many rotatable bonds). If 0 is set, this filter is off
    seed : int, default=62609
       Random seed used during RDKit embedding (in the 
       Chem.rdDistGeom.EmbedMultipleConfs() RDKit function)
+   geom : list, default=[]
+      Geometry rule to pass for the systems. Format: [SMARTS,VALUE]. Geometry rules
+      might be atoms, bonds, angles and dihedral. For example, a rule to keep only
+      molecules with C-Pd-C atoms at 180 degrees: ['[C][Pd][C]',180]
+   bond_thres : float, default=0.2
+      Threshold used to discard bonds in the geom option (+-0.2 A) 
+   angle_thres : float, default=30
+      Threshold used to discard angles in the geom option (+-30 degrees) 
+   dihedral_thres : float, default=30
+      Threshold used to discard dihedral angles in the geom option (+-30 degrees) 
 
 Only organometallic molecules
 .............................
 
    auto_metal_atoms : bool, default=True
      Automatically detect metal atoms for the RDKit conformer generation. Charge 
      and mult should be specified as well since the automatic charge and mult 
@@ -125,15 +135,15 @@
       Number of dihedrals to rotate simultaneously (picked at random) during 
       each step of the Fullmonte sampling
    ang_fullmonte : float, default=30
       Available angle interval to use in the Fullmonte sampling. For example, if
       the angle is 120.0, the program chooses randomly between 120 and 240 
       degrees (picked at random) during each step of the sampling
 
-Crest only
+CREST only
 ++++++++++
 
    nprocs : int, default=2
       Number of processors used in CREST optimizations
    constraints_atoms : list, default=[]
       Specify constrained atoms as [AT1,AT2,AT3]. An example of multiple constraints with
       atoms 1, 2 and 5 frozen: [1,2,5]
@@ -157,14 +167,16 @@
    cregen : bool, default=False
       If True, perform a CREGEN analysis after CREST (filtering options below)
    cregen_keywords : str, default=None
       Additional keywords for CREGEN (i.e. cregen_keywords='--ethr 0.02')
    xtb_keywords : str, default=None
       Define additional keywords to use in the xTB pre-optimization that are not 
       included in -c, --uhf, -P and --input. For example: '--alpb ch2cl2 --gfn 1' 
+    crest_nrun : int, default=1
+      Specify as number of runs if multiple starting points from RDKit starting points is required.
 """
 #####################################################.
 #          This file stores the CSEARCH class       #
 #             used in conformer generation          #
 #####################################################.
 
 import math
@@ -175,43 +187,51 @@
 import subprocess
 import glob
 from pathlib import Path
 import pandas as pd
 import concurrent.futures as futures
 import multiprocessing as mp
 from progress.bar import IncrementalBar
+import numpy as np
 
 from rdkit.Chem import AllChem as Chem
 from rdkit.Chem import Descriptors as Descriptors
 from rdkit.Chem import rdmolfiles
 from rdkit.Chem import rdMolTransforms, PropertyMol, rdDistGeom, Lipinski
 
-from aqme.filter import filters, ewin_filter, pre_E_filter, RMSD_and_E_filter
+from aqme.filter import (
+    filters, ewin_filter,
+    pre_E_filter,
+    RMSD_and_E_filter,
+    geom_filter
+    )
 from aqme.csearch.utils import (
     prepare_direct_smi,
     prepare_smiles_files,
     prepare_csv_files,
     prepare_cdx_files,
     prepare_com_files,
     prepare_sdf_files,
     prepare_pdb_files,
     creation_of_dup_csv_csearch,
     minimize_rdkit_energy,
     com_2_xyz,
     check_constraints,
     smi_to_mol,
-    getDihedralMatches
-)
+    getDihedralMatches,
+    cluster_conformers
+    )
 from aqme.csearch.templates import template_embed, check_metal_neigh
 from aqme.csearch.fullmonte import generating_conformations_fullmonte, realign_mol
 from aqme.utils import (
     substituted_mol,
     load_variables,
     set_metal_atomic_number,
     check_xtb,
+    check_crest,
     get_files
     )
 from aqme.csearch.crest import xtb_opt_main
 
 
 class csearch:
     """
@@ -238,14 +258,15 @@
             sys.exit()
 
         if str(self.args.auto_metal_atoms) == "False":
             self.args.auto_metal_atoms = False
 
         if self.args.program.lower() == "crest":
             _ = check_xtb(self)
+            _ = check_crest(self)
 
         if self.args.smi is None and self.args.input == "":
             self.args.log.write("\nx  Program requires either a SMILES or an input file to proceed! Please look up acceptable file formats. Specify: smi='CCC' (or input='filename.csv')")
             self.args.log.finalize()
             sys.exit()
         elif self.args.smi is not None and self.args.input != "":
             self.args.log.write("\nx  Program requires either a SMILES or an input file to proceed, don't use both!")
@@ -288,22 +309,28 @@
             # store all the information into a CSV file
             csearch_file_no_path = (
                 os.path.basename(csearch_file).split(".")[0]
             )
             self.csearch_csv_file = self.args.w_dir_main.joinpath(
                 f"CSEARCH-Data-{csearch_file_no_path}.csv"
             )
-            self.final_dup_data.to_csv(self.csearch_csv_file, index=False)
+            if self.args.verbose:
+                self.final_dup_data.to_csv(self.csearch_csv_file, index=False)
 
-            elapsed_time = round(time.time() - start_time_overall, 2)
-            self.args.log.write(f"\nTime CSEARCH: {elapsed_time} seconds\n")
-            self.args.log.finalize()
+            # removes systems that did not generate any conformers
+            for sdf_file in glob.glob(f'{self.args.w_dir_main}/CSEARCH/*.sdf'):
+                if os.path.getsize(sdf_file) == 0:
+                    os.remove(sdf_file)
+
+        elapsed_time = round(time.time() - start_time_overall, 2)
+        self.args.log.write(f"\nTime CSEARCH: {elapsed_time} seconds\n")
+        self.args.log.finalize()
 
-            # this is added to avoid path problems in jupyter notebooks
-            os.chdir(self.args.initial_dir)
+        # this is added to avoid path problems in jupyter notebooks
+        os.chdir(self.args.initial_dir)
 
     def load_jobs(self, csearch_file):
         """
         Load information of the different molecules for conformer generation
         """
 
         SUPPORTED_INPUTS = [
@@ -342,15 +369,20 @@
         Extension2inputgen[".sdf"] = prepare_sdf_files
         Extension2inputgen[".mol"] = prepare_sdf_files
         Extension2inputgen[".mol2"] = prepare_sdf_files
         Extension2inputgen[".pdb"] = prepare_pdb_files
 
         # Prepare the jobs
         prepare_function = Extension2inputgen[file_format]
-        job_inputs = prepare_function(self.args, csearch_file)
+        try:
+            job_inputs = prepare_function(self.args, csearch_file)
+        except FileNotFoundError:
+            self.args.log.write(f'\nx  File {os.path.basename(csearch_file)} was not found! In the "input" option, make sure that 1) the PATH to the files is correct and 2) the PATH doesn\'t start with "/".')
+            self.args.log.finalize()
+            sys.exit()     
 
         return job_inputs
 
     def run_csearch(self, job_inputs):
         # create the dataframe to store the data
         self.final_dup_data = creation_of_dup_csv_csearch(self.args.program.lower())
 
@@ -369,25 +401,29 @@
                     name_,
                     charge_,
                     mult_,
                     constraints_atoms_,
                     constraints_dist_,
                     constraints_angle_,
                     constraints_dihedral_,
+                    complex_type_,
+                    geom_
                 ) = job_input
                 job = executor.submit(
                     self.compute_confs(
                         smi_,
                         name_,
                         charge_,
                         mult_,
                         constraints_atoms_,
                         constraints_dist_,
                         constraints_angle_,
                         constraints_dihedral_,
+                        complex_type_,
+                        geom_
                     )
                 )
                 jobs.append(job)
 
                 bar.next()
 
             bar.finish()
@@ -398,14 +434,16 @@
         name,
         charge,
         mult,
         constraints_atoms,
         constraints_dist,
         constraints_angle,
         constraints_dihedral,
+        complex_type,
+        geom
     ):
         """
         Function to start conformer generation
         """
 
         self.args.log.write(f"\n   ----- {name} -----")
 
@@ -436,16 +474,18 @@
                 return
 
         else:
             # for 3D input formats, the smi variable represents the mol object
             mol = smi
             if mol is None:
                 self.args.log.write(f"\nx  Failed to convert the provided input to an RDkit Mol object! Please check the starting structure.")
-                self.args.log.finalize()
-                sys.exit()
+                if self.args.input.split(".")[1] not in ["csv","cdx","txt","yaml","yml","rtf"]:
+                    self.args.log.finalize()
+                    sys.exit()
+                return
                 
             # check if the optimization is constrained
             complex_ts = check_constraints(self)
 
         if self.args.destination is None:
             self.csearch_folder = Path(self.args.initial_dir).joinpath(
                 f"CSEARCH"
@@ -454,14 +494,15 @@
             if self.args.initial_dir.as_posix() in f"{self.args.destination}":
                 self.csearch_folder = Path(self.args.destination)
             else:
                 self.csearch_folder = Path(self.args.initial_dir).joinpath(self.args.destination)
 
         self.csearch_folder.mkdir(exist_ok=True, parents=True)
 
+        # for 3D input types
         if self.args.program.lower() in ["crest"] and self.args.smi is None:
             if self.args.input.split(".")[1] in ["pdb", "mol2", "mol", "sdf"]:
                 command_pdb = [
                     "obabel",
                     f'-i{self.args.input.split(".")[1]}',
                     f'{name}.{self.args.input.split(".")[1]}',
                     "-oxyz",
@@ -495,33 +536,35 @@
             # get pre-determined geometries for metal complexes
             accepted_complex_types = [
                 "squareplanar",
                 "squarepyramidal",
                 "linear",
                 "trigonalplanar",
             ]
-            if self.args.complex_type != '' and self.args.complex_type not in accepted_complex_types:
-                self.args.log.write(f"x  The metal template specified in complex_type ({self.args.complex_type}) is not valid! Options: squareplanar, squarepyramidal, linear and trigonalplanar")
-                self.args.log.finalize()
-                sys.exit()
+            if complex_type != '' and complex_type not in accepted_complex_types:
+                self.args.log.write(f"x  The metal template specified in complex_type ({complex_type}) is not valid! Options: squareplanar, squarepyramidal, linear and trigonalplanar")
+                if self.args.input.split(".")[1] not in ["csv","cdx","txt","yaml","yml","rtf"]:
+                    self.args.log.finalize()
+                    sys.exit()
+                return
 
-            if self.args.complex_type in accepted_complex_types:
+            if complex_type in accepted_complex_types:
                 count_metals = 0
                 valid_template = True
                 # check if the specified metal is included in the system
                 for metal_idx_ind in self.args.metal_idx:
                     if metal_idx_ind is not None:
                         # calculate number of expected neighbours
-                        valid_template = check_metal_neigh(mol, self.args.complex_type, metal_idx_ind, self.args.log, valid_template)
+                        valid_template = check_metal_neigh(mol, complex_type, metal_idx_ind, self.args.log, valid_template)
                         count_metals += 1
 
                 if count_metals == 1 and valid_template:
                     template_opt = True
                     template_kwargs = dict()
-                    template_kwargs["complex_type"] = self.args.complex_type
+                    template_kwargs["complex_type"] = complex_type
                     template_kwargs["metal_idx"] = self.args.metal_idx
                     template_kwargs["maxsteps"] = self.args.opt_steps_rdkit
                     template_kwargs["heavyonly"] = self.args.heavyonly
                     template_kwargs["maxmatches"] = self.args.max_matches_rmsd
                     template_kwargs["mol"] = mol
                     template_kwargs["name"] = name
                     items = template_embed(self, **template_kwargs)
@@ -535,35 +578,39 @@
                             constraints_atoms,
                             constraints_dist,
                             constraints_angle,
                             constraints_dihedral,
                             complex_ts,
                             charge,
                             mult,
+                            smi,
+                            geom,
                             coord_map,
                             alg_map,
-                            template,
+                            template
                         )
                         frames = [total_data, data]
                         total_data = pd.concat(frames, sort=True)
 
                 elif count_metals > 1 or count_metals == 0:
-                    self.args.log.write(f"\nx  The template specified {self.args.complex_type} is not used for systems with more than 1 metal or for organic molecueles.")
+                    self.args.log.write(f"\nx  The template specified {complex_type} is not used for systems with more than 1 metal or for organic molecueles.")
 
         if not template_opt:
             total_data = self.conformer_generation(
                 mol,
                 name,
                 constraints_atoms,
                 constraints_dist,
                 constraints_angle,
                 constraints_dihedral,
                 complex_ts,
                 charge,
                 mult,
+                smi,
+                geom
             )
 
         # Updates the dataframe with infromation about conformer generation
         frames = [self.final_dup_data, total_data]
         self.final_dup_data = pd.concat(frames, ignore_index=True, sort=True)
 
     # automatic detection of metal atoms   
@@ -573,90 +620,129 @@
                             'Tc', 'Ru', 'Rh', 'Pd', 'Ag', 'Cd', 'Hf', 'Ta', 'W', 'Re', 'Os', 'Ir', 'Pt', 'Au',
                             'Hg', 'Rf', 'Db', 'Sg', 'Bh', 'Hs', 'Mt', 'Ds', 'Rg', 'Cn', 'Nh', 'Fl', 'Mc', 'Lv', 'Ts', 'Og']
         for atom in mol.GetAtoms():
             if atom.GetSymbol() in transition_metals:
                 self.args.metal_atoms.append(atom.GetSymbol())
         if len(self.args.metal_atoms) > 0:
             self.args.log.write(f"\no  AQME recognized the following metal atoms: {self.args.metal_atoms}")
-            if charge is None or mult is None:
-                self.args.log.write(f"\nx  The automated charge and multiplicity calculation might not be precise for metal complexes! You should use the charge and mult options (or the charge and mult columns in CSV inputs).")
+            if charge is None:
+                self.args.log.write(f"\nx  The automated charge calculation might not be precise for metal complexes! You should use the charge option (or the charge column in CSV inputs).")
+            if mult is None:
+                self.args.log.write(f"\nx  The automated multiplicity calculation might not be precise for metal complexes! You should use the mult option (or the mult column in CSV inputs).")
 
     def conformer_generation(
         self,
         mol,
         name,
         constraints_atoms,
         constraints_dist,
         constraints_angle,
         constraints_dihedral,
         complex_ts,
         charge,
         mult,
+        smi,
+        geom,
         coord_Map=None,
         alg_Map=None,
         mol_template=None,
     ):
         """
         Function to load mol objects and create 3D conformers
 
         """
 
         dup_data = creation_of_dup_csv_csearch(self.args.program.lower())
 
         dup_data_idx = 0
-        start_time = time.time()
         status = None
 
         # Set charge and multiplicity
         # user can overwrite charge and mult with the corresponding arguments
         if charge is None:
             charge = Chem.GetFormalCharge(mol)
         if mult is None:
             mult = Descriptors.NumRadicalElectrons(mol) + 1
 
-        dup_data.at[dup_data_idx, "Real charge"] = charge
-        dup_data.at[dup_data_idx, "Mult"] = mult
-
         # inputs that go through CREST containing 3D coordinates don't require a previous RDKit conformer sampling
         if (
             self.args.program.lower() in ["crest"]
             and self.args.smi is None
             and self.args.input.split(".")[1] in ["pdb","mol2","mol","sdf","gjf","com","xyz"]
         ):
 
             valid_structure = True
-            status = xtb_opt_main(
-                f"{name}_{self.args.program.lower()}",
-                dup_data,
-                dup_data_idx,
-                self,
-                charge,
-                mult,
-                constraints_atoms,
-                constraints_dist,
-                constraints_angle,
-                constraints_dihedral,
-                'crest',
-                mol=mol
-            )
+            if self.args.crest_nrun == 1:
+                start_time = time.time()
+                dup_data.at[dup_data_idx, "Real charge"] = charge
+                dup_data.at[dup_data_idx, "Mult"] = mult
+                dup_data.at[dup_data_idx, "Molecule"] = name
+                status = xtb_opt_main(
+                    f"{name}_{self.args.program.lower()}",
+                    dup_data,
+                    dup_data_idx,
+                    self,
+                    charge,
+                    mult,
+                    smi,
+                    constraints_atoms,
+                    constraints_dist,
+                    constraints_angle,
+                    constraints_dihedral,
+                    'crest',
+                    geom,
+                    mol=mol, 
+                )
+                n_seconds = round(time.time() - start_time, 2)
+                dup_data.at[dup_data_idx, "CSEARCH time (seconds)"] = n_seconds
+            else:
+                for pt in range(1, int(self.args.crest_nrun)+1):
+                    start_time = time.time()
+                    dup_data.at[dup_data_idx, "Real charge"] = charge
+                    dup_data.at[dup_data_idx, "Mult"] = mult
+                    dup_data.at[dup_data_idx, "Molecule"] = name + "_run_{0}".format(pt)
+                    shutil.copy(f"{name}_{self.args.program.lower()}.xyz", f"{name}_run_{pt}_{self.args.program.lower()}.xyz")
+                    status = xtb_opt_main(
+                        f"{name}_run_{pt}_{self.args.program.lower()}",
+                        dup_data,
+                        dup_data_idx,
+                        self,
+                        charge,
+                        mult,
+                        smi,
+                        constraints_atoms,
+                        constraints_dist,
+                        constraints_angle,
+                        constraints_dihedral,
+                        'crest',
+                        geom,
+                        mol=mol, 
+                    )
+                    n_seconds = round(time.time() - start_time, 2)
+                    dup_data.at[dup_data_idx, "CSEARCH time (seconds)"] = n_seconds
+                    dup_data_idx +=1
 
         else:
+            start_time = time.time()
             name = name.replace("/", "\\").split("\\")[-1].split(".")[0]
             self.csearch_file = self.csearch_folder.joinpath(
                 name + "_" + self.args.program.lower() + self.args.output
             )
-            sdwriter_init = Chem.SDWriter(str(self.csearch_file))
+            if self.args.crest_nrun != 1 and self.args.program.lower() =='crest':
+                sdwriter_init = None
+            else:
+                sdwriter_init = Chem.SDWriter(str(self.csearch_file))
 
             valid_structure = filters(
                 mol, self.args.log, self.args.max_mol_wt
             )
             if valid_structure:
                 try:
                     # the conformational search for RDKit
-                    status = self.summ_search(
+                    status, dup_data = self.summ_search(
                         mol,
                         name,
                         sdwriter_init,
                         dup_data,
                         dup_data_idx,
                         charge,
                         mult,
@@ -664,25 +750,38 @@
                         constraints_dist,
                         constraints_angle,
                         constraints_dihedral,
                         complex_ts,
                         coord_Map,
                         alg_Map,
                         mol_template,
+                        smi,
+                        geom
                     )
                 except (KeyboardInterrupt, SystemExit):
                     raise
 
         if status == -1 or not valid_structure:
             error_message = "\nx  ERROR: The structure is not valid or no conformers were obtained from this SMILES string"
             self.args.log.write(error_message)
 
-        n_seconds = round(time.time() - start_time, 2)
-        dup_data.at[dup_data_idx, "CSEARCH time (seconds)"] = n_seconds
-
+        #combining all the sdfs from more than one run
+        if self.args.crest_nrun != 1:
+            sdwriter_rd = Chem.SDWriter(str(self.csearch_file))
+            file_runs = glob.glob(str(self.csearch_folder)+'/'+ name +'_run_*'+ self.args.program.lower() +'.sdf')
+            allenergy, allmols = [], []
+            for file in file_runs:
+                mols = Chem.SDMolSupplier(file, removeHs=False)
+                for mol in mols:
+                    allmols.append(mol)
+                    allenergy.append(float(mol.GetProp('Energy')))
+            
+            allmols_sorted = [mol for _, mol in sorted(zip(allenergy, allmols), key=lambda pair: pair[0])]
+            for mol in allmols_sorted:
+                sdwriter_rd.write(mol)
         return dup_data
 
     def summ_search(
         self,
         mol,
         name,
         sdwriter,
@@ -693,21 +792,25 @@
         constraints_atoms,
         constraints_dist,
         constraints_angle,
         constraints_dihedral,
         complex_ts,
         coord_Map,
         alg_Map,
-        mol_template
+        mol_template,
+        smi,
+        geom
     ):
 
         """
         Embeds, optimizes and filters RDKit conformers
         """
 
+        start_time = time.time()
+
         # writes sdf for the first RDKit conformer generation
         if not complex_ts:
             if self.args.program.lower() in ['rdkit']:
                 self.args.log.write(f"\no  Starting RDKit conformer sampling")
             elif self.args.program.lower() in ['summ','fullmonte']:
                 self.args.log.write(f"\no  Starting RDKit-{self.args.program} conformer sampling")
             elif self.args.program.lower() in ['crest'] and self.args.input.split(".")[1] not in ["pdb","mol2","mol","sdf","gjf","com","xyz"]:
@@ -719,80 +822,143 @@
                 dup_data,
                 dup_data_idx,
                 sdwriter,
                 charge,
                 mult,
                 coord_Map,
                 alg_Map,
-                mol_template
+                mol_template,
+                smi,
+                geom
             )
+            if self.args.program.lower() in ['rdkit','fullmonte'] :
+                n_seconds = round(time.time() - start_time, 2)
+                dup_data.at[dup_data_idx, "CSEARCH time (seconds)"] = n_seconds
+
             # this avoids memory issues when using Windows
             try:
-                sdwriter.close()
+                if self.args.crest_nrun != 1 and self.args.program.lower() =='crest':
+                    pass
+                else:
+                    sdwriter.close()
             except RuntimeError:
                 pass
             # reads the initial SDF files from RDKit and uses dihedral scan if selected
             if status not in [-1, 0]:
                 # getting the energy and mols after rotations
                 if self.args.program.lower() == "summ" and len(rotmatches) != 0:
                     status = self.dihedral_filter_and_sdf(
                         name, dup_data, dup_data_idx, coord_Map, alg_Map, mol_template, ff
                     )
+                    n_seconds = round(time.time() - start_time, 2)
+                    dup_data.at[dup_data_idx, "CSEARCH time (seconds)"] = n_seconds
 
         if self.args.program.lower() in ['crest']:
             stop_xtb_opt = False
             if not complex_ts:
                 # mol_crest is the RDKit-optimized mol object
                 if mol_crest is not None:
-                    rdmolfiles.MolToXYZFile(mol_crest, name + "_crest.xyz")
+                    if self.args.crest_nrun == 1:
+                        dup_data.at[dup_data_idx, "Molecule"] = name
+                        rdmolfiles.MolToXYZFile(mol_crest[0], name + "_crest.xyz")
+                    else:
+                        # clustering to get the best mol objects
+                        cluster_centroird_mols, centroids = cluster_conformers(mol_crest, self.args.heavyonly, self.args.max_matches_rmsd, self.args.crest_nclust)
+                        num_start_points = min(int(self.args.crest_nrun), len(cluster_centroird_mols))
+                        for pt in range(1, num_start_points+1):
+                            dup_data.at[dup_data_idx, "Molecule"] = name + "_run_{0}".format(pt)
+                            rdmolfiles.MolToXYZFile(cluster_centroird_mols[pt-1], name + "_run_{0}_crest.xyz".format(pt), confId=centroids[pt-1])
+                            
                 else:
                     stop_xtb_opt = True
                     status = -1
             else:
                 # mol is the raw mol object (no optimization with RDKit to avoid problems when using
                 # noncovalent complexes and TSs)
                 if mol is not None:
-                    rdmolfiles.MolToXYZFile(mol, name + "_crest.xyz")
+                    if self.args.crest_nrun == 1:
+                        dup_data.at[dup_data_idx, "Molecule"] = name
+                        rdmolfiles.MolToXYZFile(mol, name + "_crest.xyz")
+                    else:
+                        num_start_points = min(int(self.args.crest_nrun), len(mol_crest))
+                        for pt in range(1, num_start_points+1):
+                            dup_data.at[pt-1, "Molecule"] = name + "_run_{0}".format(pt)
+                            rdmolfiles.MolToXYZFile(mol, name + "_run_{0}_crest.xyz".format(pt))
                 else:
                     stop_xtb_opt = True
                     status = -1
             if not stop_xtb_opt:
-                status = xtb_opt_main(
+                start_time = time.time()
+                dup_data.at[dup_data_idx, "Molecule"] = name
+                if self.args.crest_nrun == 1:
+                    status = xtb_opt_main(
                         f"{name}_{self.args.program.lower()}",
                         dup_data,
                         dup_data_idx,
                         self,
                         charge,
                         mult,
+                        smi,
                         constraints_atoms,
                         constraints_dist,
                         constraints_angle,
                         constraints_dihedral,
                         'crest',
+                        geom,
                         complex_ts=complex_ts,
-                        mol=mol # this is necessary for CREST calculations with constraints
-                    )
+                        mol=mol, # this is necessary for CREST calculations with constraints 
+                        )
+                    n_seconds = round(time.time() - start_time, 2)
+                    dup_data.at[dup_data_idx, "CSEARCH time (seconds)"] = n_seconds
+                else:
+                    num_start_points = min(int(self.args.crest_nrun), len(mol_crest))
+                    dup_data = pd.DataFrame(np.repeat(dup_data.values, num_start_points, axis=0), columns=dup_data.columns)
+                    for pt in range(1, num_start_points+1):
+                        start_time = time.time()
+                        dup_data.at[pt-1, "Molecule"] = f"{name}_run_{pt}"
+                        status = xtb_opt_main(
+                            f"{name}_run_{pt}_{self.args.program.lower()}",
+                            dup_data,
+                            pt-1,
+                            self,
+                            charge,
+                            mult,
+                            smi,
+                            constraints_atoms,
+                            constraints_dist,
+                            constraints_angle,
+                            constraints_dihedral,
+                            'crest',
+                            geom,
+                            complex_ts=complex_ts,
+                            mol=mol, # this is necessary for CREST calculations with constraints
+                            
+                        )
+                        n_seconds = round(time.time() - start_time, 2)
+                        dup_data.at[pt-1, "CSEARCH time (seconds)"] = n_seconds
 
-        return status
+        return status, dup_data
 
     def dihedral_filter_and_sdf(
         self, name, dup_data, dup_data_idx, coord_Map, alg_Map, mol_template, ff
     ):
         """
         Filtering after dihedral scan to sdf
         """
 
         rotated_energy = []
 
         # apply filters
         rdmols = Chem.SDMolSupplier(str(self.csearch_file), removeHs=False) 
         if rdmols is None:
             self.args.log.write("\nCould not open " + name + self.args.output)
-            self.args.log.finalize()
-            sys.exit()
+            if self.args.input.split(".")[1] not in ["csv","cdx","txt","yaml","yml","rtf"]:
+                self.args.log.finalize()
+                sys.exit()
+            return
 
         for i, rd_mol_i in enumerate(rdmols):
             if coord_Map is None and alg_Map is None and mol_template is None:
                 energy = minimize_rdkit_energy(
                     rd_mol_i, -1, self.args.log, ff, self.args.opt_steps_rdkit
                 )
             else:
@@ -989,25 +1155,25 @@
         cids = rdDistGeom.EmbedMultipleConfs(mol, initial_confs, **embed_kwargs)
 
         if len(cids) <= 1 and initial_confs != 1:
             self.args.log.write(f"\nx  Normal RDKit embeding process failed, trying to generate conformers with random coordinates (with {str(initial_confs)} possibilities)")
             embed_kwargs["useRandomCoords"] = True
             embed_kwargs["boxSizeMult"] = 10.0
             embed_kwargs["numZeroFail"] = 1000
-            embed_kwargs["numThreads"] = 1
+            embed_kwargs["numThreads"] = 0
             cids = rdDistGeom.EmbedMultipleConfs(mol, initial_confs, **embed_kwargs)
 
         if is_sdf_mol_or_mol2:
             # preserving AssignStereochemistryFrom3D
             for cid in cids:
                 Chem.AssignAtomChiralTagsFromStructure(mol, confId=cid)
 
         return cids
 
-    def min_and_E_calc(self, mol, cids, coord_Map, alg_Map, mol_template, ff):
+    def min_and_E_calc(self, mol, cids, coord_Map, alg_Map, mol_template, ff, geom):
         """
         Minimization and E calculation with RDKit after embeding
         """
 
         cenergy, outmols = [], []
 
         for _, conf in enumerate(cids):
@@ -1020,17 +1186,24 @@
                     mol,
                     conf,
                     coord_Map,
                     alg_Map,
                     mol_template,
                     self.args.opt_steps_rdkit,
                 )
-            cenergy.append(energy)
-            pmol = PropertyMol.PropertyMol(mol)
-            outmols.append(pmol)
+
+            # removes geometries that do not pass the filters (geom option)
+            mol_geom = Chem.Mol(mol)
+            if len(self.args.metal_atoms) >= 1:
+                set_metal_atomic_number(mol_geom, self.args.metal_idx, self.args.metal_sym)
+            passing_geom = geom_filter(self,mol_geom,geom)
+            if passing_geom:
+                cenergy.append(energy)
+                pmol = PropertyMol.PropertyMol(mol)
+                outmols.append(pmol)
 
         return outmols, cenergy
 
     def min_after_embed(
         self,
         mol,
         cids,
@@ -1042,33 +1215,38 @@
         update_to_rdkit,
         coord_Map,
         alg_Map,
         mol_template,
         charge,
         mult,
         ff,
+        smi,
+        geom
     ):
         """
         Minimizes, gets the energy and filters RDKit conformers after embeding
         """
 
         # gets optimized mol objects and energies
+        if geom != []:
+            self.args.log.write(f"o  Applying geometry filters ({geom})")
         outmols, cenergy = self.min_and_E_calc(
-            mol, cids, coord_Map, alg_Map, mol_template, ff
+            mol, cids, coord_Map, alg_Map, mol_template, ff, geom
         )
 
         # writing charges and multiplicity after RDKit
         dup_data.at[dup_data_idx, "Mult"] = mult
         dup_data.at[dup_data_idx, "Real charge"] = charge
 
         for i, cid in enumerate(cids):
             outmols[cid].SetProp("_Name", name + " " + str(i + 1))
             outmols[cid].SetProp("Energy", str(cenergy[cid]))
             outmols[cid].SetProp("Real charge", str(charge))
             outmols[cid].SetProp("Mult", str(mult))
+            outmols[cid].SetProp("SMILES", str(smi))
 
         # sorts the energies
         cids = list(range(len(outmols)))
         sorted_all_cids = sorted(cids, key=lambda cid: cenergy[cid])
 
         self.args.log.write("\no  Applying filters to initial conformers")
 
@@ -1135,14 +1313,15 @@
                         sdwriter,
                         outmols[conf].GetProp("_Name"),
                         update_to_rdkit,
                         coord_Map,
                         alg_Map,
                         mol_template,
                     )
+                    outmols = [mol]
                     break
 
             status = 1
 
         if self.args.program.lower() == "summ":
             dup_data.at[dup_data_idx, "summ-conformers"] = total
 
@@ -1160,28 +1339,30 @@
                 alg_Map,
                 mol_template,
                 ff,
             )
             # removes the rdkit file
             os.remove(name + "_" + "rdkit" + self.args.output)
 
-        return status, mol
+        return status, outmols
 
     def rdkit_to_sdf(
         self,
         mol,
         name,
         dup_data,
         dup_data_idx,
         sdwriter,
         charge,
         mult,
         coord_Map,
         alg_Map,
-        mol_template
+        mol_template,
+        smi,
+        geom
     ):
 
         """
         Conversion from RDKit to SDF
         """
 
         try:
@@ -1199,15 +1380,14 @@
             # and initial_confs can be low to speed up the process
             initial_confs = self.args.auto_sample
         elif self.args.sample == "auto":
             initial_confs = int(self.auto_sampling(mol))
         else:
             initial_confs = int(self.args.sample)
 
-        dup_data.at[dup_data_idx, "Molecule"] = name
         update_to_rdkit = False
 
         rotmatches = getDihedralMatches(mol, self.args.heavyonly)
 
         if len(rotmatches) > self.args.max_torsions and self.args.max_torsions > 0:
             self.args.log.write(f"\nx  Too many torsions ({len(rotmatches)}). Skipping {name + self.args.output}")
         elif self.args.program.lower() == "summ" and len(rotmatches) == 0:
@@ -1227,30 +1407,35 @@
         # identify the atoms and decide Force Field
         for atom in mol.GetAtoms():
             if atom.GetAtomicNum() > 36 and self.args.ff == "MMFF":  # up to Kr for MMFF, if not the code will use UFF
                 self.args.log.write(f"\nx  {self.args.ff} is not compatible with the molecule, changing to UFF")
                 ff = "UFF"
 
         try:
-            status,mol_crest = self.min_after_embed(
+            status, mol_crest = self.min_after_embed(
                 mol,
                 cids,
                 name,
                 rotmatches,
                 dup_data,
                 dup_data_idx,
                 sdwriter,
                 update_to_rdkit,
                 coord_Map,
                 alg_Map,
                 mol_template,
                 charge,
                 mult,
                 ff,
+                smi,
+                geom
             )
         except IndexError:
             status = -1
             mol_crest = None
 
-        sdwriter.close()
+        if self.args.crest_nrun != 1 and self.args.program.lower() =='crest':
+            pass
+        else:
+            sdwriter.close()
 
         return status, rotmatches, ff, mol_crest
```

### Comparing `aqme-1.5.0/aqme/csearch/crest.py` & `aqme-1.5.1/aqme/csearch/crest.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from rdkit.Chem import rdmolfiles
 from rdkit import Geometry
 import subprocess
 import rdkit
 from pathlib import Path
 import shutil
 from aqme.utils import read_file, run_command
+from aqme.filter import geom_filter
 from rdkit.Chem import rdMolTransforms
 
 
 def atompairs(mol, atom1, atom2, constraints):
     active = []
     for x in constraints:
         active.append(x[:2])
@@ -66,22 +67,25 @@
 def xtb_opt_main(
     name,
     dup_data,
     dup_data_idx,
     self,
     charge,
     mult,
+    smi,
     constraints_atoms,
     constraints_dist,
     constraints_angle,
     constraints_dihedral,
     method_opt,
+    geom,
     complex_ts=False,
     mol=None,
-    name_init=None
+    name_init=None,
+
 ):
 
     """
     Run xTB using subprocess to perform CREST/CREGEN conformer sampling
     """
 
     name_no_path = name.replace("/", "\\").split("\\")[-1].split(".")[0]
@@ -109,15 +113,15 @@
         xyzin = f"{dat_dir}/{name_no_path}_xtb.xyz"
     dat_dir.mkdir(exist_ok=True, parents=True)
     shutil.move(f"{name}.xyz", xyzin)
 
     os.environ["OMP_STACKSIZE"] = self.args.stacksize
     # to run xTB/CREST with more than 1 processor
     os.environ["OMP_NUM_THREADS"] = str(self.args.nprocs)
-    cmin_valid = True
+    opt_valid = True
 
     os.chdir(dat_dir)
     
     # for systems that were created from 1D and 2D inputs (i.e. SMILES), this part includes two xTB
     # constrained optimizations to avoid geometry problems in noncovalent complexes and transition states
 
     # xTB optimization with all bonds frozen
@@ -234,31 +238,31 @@
             if self.args.xtb_keywords is not None:
                 for keyword in self.args.xtb_keywords.split():
                     command.append(keyword)
 
             run_command(command, f"{xyzin.split('.')[0]}_xtb1.out")
             os.rename(str(dat_dir) + "/xtbopt.xyz", xyzoutxtb1)
         except FileNotFoundError:
-            self.args.log.write(f"\nx   There was an error during the xTB pre-optimization. This error is related to parallelization of xTB jobs and is normally observed when using metal complexes in some operative systems/OpenMP versions. AQME is switching to using one processor (nprocs=1).\n")
+            self.args.log.write(f"\nx  There was an error during the xTB pre-optimization. This error is related to parallelization of xTB jobs and is normally observed when using metal complexes in some operative systems/OpenMP versions. AQME is switching to using one processor (nprocs=1).\n")
             self.args.nprocs = 1
             try:
                 if self.args.xtb_keywords is None:
                     comm_xtb = f"export OMP_STACKSIZE={self.args.stacksize} && export OMP_NUM_THREADS={self.args.nprocs},1 \
                     && xtb {xyzin} --opt -c {charge} --uhf {int(mult) - 1} >> {xyzin.split('.')[0]}_xtb1.out"
                 else:
                     comm_xtb = f"export OMP_STACKSIZE={self.args.stacksize} && export OMP_NUM_THREADS={self.args.nprocs},1 \
                     && xtb {xyzin} --opt -c {charge} --uhf {int(mult) - 1} {self.args.xtb_keywords} >> {xyzin.split('.')[0]}_xtb1.out"
                 subprocess.call(comm_xtb, shell=False)
                 os.rename(str(dat_dir) + "/xtbopt.xyz", xyzoutxtb1)
             except FileNotFoundError:
                 if self.args.program.lower() == "crest":
-                    self.args.log.write(f"\nx   There was another error during the xTB pre-optimization that could not be fixed. Trying CREST directly with no xTB preoptimization.\n")
+                    self.args.log.write(f"\nx  There was another error during the xTB pre-optimization that could not be fixed. Trying CREST directly with no xTB preoptimization.\n")
                 else:
-                    self.args.log.write(f"\nx   There was another error during the xTB pre-optimization that could not be fixed (this molecule will be skipped).\n")
-                cmin_valid = False
+                    self.args.log.write(f"\nx  There was another error during the xTB pre-optimization that could not be fixed (this molecule will be skipped).\n")
+                opt_valid = False
                 mol_rd = None
 
         xyzoutxtb2 = xyzoutxtb1
 
     xyzoutall = str(dat_dir) + "/" + name_no_path + "_conformers.xyz"
 
     # CREST sampling
@@ -319,18 +323,18 @@
                 shutil.copy(str(dat_dir) + "/crest_clustered.xyz", xyzoutall)
 
             elif os.path.exists(str(dat_dir) + "/crest_ensemble.xyz"):
                 shutil.copy(str(dat_dir) + "/crest_ensemble.xyz", xyzoutall)
             else:
                 shutil.copy(str(dat_dir) + "/crest_conformers.xyz", xyzoutall)
         except FileNotFoundError:
-            self.args.log.write("\nx   CREST conformer sampling failed! Please, try other options (i.e. include constrains, change the crest_keywords option, etc.)")
-            cmin_valid = False
+            self.args.log.write("\nx  CREST conformer sampling failed! Please, try other options (i.e. include constrains, change the crest_keywords option, etc.)")
+            opt_valid = False
 
-    if cmin_valid:
+    if opt_valid:
         if self.args.program.lower() == "crest":
             xyzall_2_xyz(xyzoutall, name_no_path)
             xyz_files = glob.glob(name_no_path + "_conf_*.xyz")
         if self.args.program.lower() == "xtb":
             xyz_files = [xyzoutxtb1]
         for _, file in enumerate(xyz_files):
             name_conf = file.split(".xyz")[0]
@@ -355,17 +359,24 @@
                 # convert from hartree (default in xtb) to kcal
                 energy_Eh = float(open(file, "r").readlines()[0])
                 energy_kcal = str(energy_Eh*627.5)
                 mol_rd.SetProp("_Name", name_no_path)
                 mol_rd.SetProp("Energy", energy_kcal)
                 mol_rd.SetProp("Real charge", str(charge))
                 mol_rd.SetProp("Mult", str(int(mult)))
-                sdwriter.write(mol_rd)
+                if smi is not None:
+                    mol_rd.SetProp("SMILES", str(smi))
+                mol_geom = Chem.Mol(mol_rd)
+                passing_geom = geom_filter(self,mol_geom,geom)
+                if passing_geom:
+                    sdwriter.write(mol_rd)
                 os.remove(file)
                 os.remove(f'{file.split(".")[0]}.xyz')
+        if self.args.program.lower() == "crest":
+            sdwriter.close()
     else:
         xyz_files = []
 
     # remove xTB/CREST files to avoid wrong readings of molecular information
     for file in glob.glob('*') + glob.glob('*.*') + glob.glob('.*'):
         if os.path.exists(file):
             if file.find('.out') == -1:
@@ -393,15 +404,15 @@
     os.chdir(self.args.w_dir_main)
 
     if method_opt == 'crest':
         dup_data.at[dup_data_idx, "crest-conformers"] = len(xyz_files)
         return 1
 
     if method_opt == 'xtb':
-        return mol_rd, energy_kcal, cmin_valid
+        return mol_rd, energy_kcal, opt_valid
 
 
 def create_xcontrol(
     args,
     constraints_atoms,
     constraints_dist,
     constraints_angle,
@@ -529,20 +540,14 @@
         constraints_angle = [[float(y) for y in x] for x in constraints_angle]
         constraints_angle = np.array(constraints_angle)
     if constraints_dihedral is not None:
         using_const = constraints_dihedral
         constraints_dihedral = [[float(y) for y in x] for x in constraints_dihedral]
         constraints_dihedral = np.array(constraints_dihedral)
 
-    if using_const is not None:
-        for smi_part in smi:
-            if ':' not in smi_part or '[' not in smi_part:
-                log.write(f"\nx  Constraints were specified {using_const} but atoms might not be mapped in the SMILES input!")
-                break
-
     molsH = []
     mols = []
     for m in smi:
         mols.append(Chem.MolFromSmiles(m))
         molsH.append(Chem.AddHs(Chem.MolFromSmiles(m)))
 
     for m in molsH:
@@ -583,59 +588,55 @@
 
     max_map = max(atom_map)
     for a in mol.GetAtoms():
         if a.GetSymbol() == "H":
             max_map += 1
             a.SetAtomMapNum(int(max_map))
 
-    nconstraints_atoms = []
-    if constraints_atoms is not None:
-        for _, ele in enumerate(constraints_atoms):
-            for atom in mol.GetAtoms():
-                if ele == atom.GetAtomMapNum():
-                    nconstraints_atoms.append(float(atom.GetIdx()) + 1)
-        nconstraints_atoms = np.array(nconstraints_atoms)
-
-    nconstraints_dist = []
-    if constraints_dist is not None:
-        for _, r in enumerate(constraints_dist):
-            nr = []
-            for _, ele in enumerate(r[:2]):
-                for atom in mol.GetAtoms():
-                    if ele == atom.GetAtomMapNum():
-                        nr.append(float(atom.GetIdx()) + 1)
-            nr.append(r[-1])
-            nconstraints_dist.append(nr)
-        nconstraints_dist = np.array(nconstraints_dist)
-
-    nconstraints_angle = []
-    if constraints_angle is not None:
+    adapted_atoms = []
+    adapted_dist = []
+    adapted_angle = []
+    adapted_dihedral = []
+    # assign constraints
+    if using_const is not None:
+        for smi_part in smi:
+            if ':' not in smi_part or '[' not in smi_part: # for SMILES that are not mapped
+                log.write(f"\nx  Constraints were specified {using_const} but atoms might not be mapped in the SMILES input!")
+                adapted_atoms = constraints_atoms
+                adapted_dist = constraints_dist
+                adapted_angle = constraints_angle
+                adapted_dihedral = constraints_dihedral
+                break
 
-        for _, r in enumerate(constraints_angle):
-            nr = []
-            for _, ele in enumerate(r[:3]):
-                for atom in mol.GetAtoms():
-                    if ele == atom.GetAtomMapNum():
-                        nr.append(float(atom.GetIdx()) + 1)
-            nr.append(r[-1])
-            nconstraints_angle.append(nr)
-        nconstraints_angle = np.array(nconstraints_angle)
+        if constraints_atoms is not None:
+            for _, ele in enumerate(constraints_atoms):
+                if adapted_atoms != []: # for mapped SMILES
+                    for atom in mol.GetAtoms():
+                        if ele == atom.GetAtomMapNum():
+                            adapted_atoms.append(float(atom.GetIdx()) + 1)
+                else:
+                    adapted_atoms = constraints_atoms
+            adapted_atoms = np.array(adapted_atoms)
 
-    nconstraints_dihedral = []
-    if constraints_dihedral is not None:
-        for _, r in enumerate(constraints_dihedral):
-            nr = []
-            for _, ele in enumerate(r[:4]):
-                for atom in mol.GetAtoms():
-                    if ele == atom.GetAtomMapNum():
-                        nr.append(float(atom.GetIdx()) + 1)
-            nr.append(r[-1])
-            nconstraints_dihedral.append(nr)
-        nconstraints_dihedral = np.array(nconstraints_dihedral)
+        constraints = [constraints_dist, constraints_angle, constraints_dihedral]
+        adapted_consts = [adapted_dist, adapted_angle, adapted_dihedral]
+        n_consts= [2, 3, 4]
+        for const,adapted_const,n_const in zip(constraints,adapted_consts,n_consts):
+            if adapted_const == []: # for mapped SMILES
+                for _, r in enumerate(const):
+                    nr = []
+                    for _, ele in enumerate(r[:n_const]):
+                        if const is not None:
+                            for atom in mol.GetAtoms():
+                                if ele == atom.GetAtomMapNum():
+                                    nr.append(float(atom.GetIdx()) + 1)
+                    nr.append(r[-1])
+                    adapted_const.append(nr)
+                adapted_const = np.array(adapted_const)
 
     return (
         mol,
-        nconstraints_atoms,
-        nconstraints_dist,
-        nconstraints_angle,
-        nconstraints_dihedral,
+        adapted_atoms,
+        adapted_dist,
+        adapted_angle,
+        adapted_dihedral,
     )
```

### Comparing `aqme-1.5.0/aqme/csearch/fullmonte.py` & `aqme-1.5.1/aqme/csearch/fullmonte.py`

 * *Files identical despite different names*

### Comparing `aqme-1.5.0/aqme/csearch/templates.py` & `aqme-1.5.1/aqme/csearch/templates.py`

 * *Files identical despite different names*

### Comparing `aqme-1.5.0/aqme/csearch/utils.py` & `aqme-1.5.1/aqme/csearch/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 
 import os
 import sys
 import subprocess
 import pandas as pd
 import ast
 from rdkit.Chem import AllChem as Chem
+from rdkit.ML.Cluster import Butina
 from aqme.utils import (
     get_info_input,
     mol_from_sdf_or_mol_or_mol2,
     read_xyz_charge_mult,
-    add_prefix_suffix
+    add_prefix_suffix,
+    get_conf_RMS
 )
 from aqme.csearch.crest import nci_ts_mol
 
 
 def creation_of_dup_csv_csearch(program):
     """
     Generates a pandas.DataFrame object with the appropiate columns for the
@@ -44,15 +46,15 @@
         "Molecule",
         "RDKit-Initial-samples",
         "RDKit-energy-window",
         "RDKit-initial_energy_threshold",
         "RDKit-RMSD-and-energy-duplicates",
         "RDKit-Unique-conformers",
     ]
-    end_columns_no_min = ["CSEARCH time (seconds)", "Overall charge"]
+    end_columns_no_min = ["CSEARCH time (seconds)"]
     fullmonte_columns = [
         "FullMonte-Unique-conformers",
     ]
     #'FullMonte-conformers',
     #'FullMonte-energy-window',
     #'FullMonte-initial_energy_threshold',
     #'FullMonte-RMSD-and-energy-duplicates']
@@ -76,28 +78,15 @@
         columns = crest_columns
     else:
         return None
     columns += end_columns_no_min
     return pd.DataFrame(columns=columns)
 
 
-def constraint_fix(
-    constraints_atoms, constraints_dist, constraints_angle, constraints_dihedral
-):
-    
-    # this function avoids problems when reading contraints from CSV files
-    constraints_atoms = constaint_2_list(constraints_atoms)
-    constraints_dist = constaint_2_list(constraints_dist)
-    constraints_angle = constaint_2_list(constraints_angle)
-    constraints_dihedral = constaint_2_list(constraints_dihedral)
-
-    return constraints_atoms, constraints_dist, constraints_angle, constraints_dihedral
-
-
-def constaint_2_list(contraints):
+def csv_2_list(contraints):
     try:
         if pd.isnull(contraints):
             contraints = []
     except ValueError:
         pass
     if not isinstance(contraints, list):
         contraints = ast.literal_eval(contraints)
@@ -121,14 +110,16 @@
         name,
         args.charge,
         args.mult,
         args.constraints_atoms,
         args.constraints_dist,
         args.constraints_angle,
         args.constraints_dihedral,
+        args.complex_type,
+        args.geom
     )
     job_inputs.append(obj)
 
     return job_inputs
 
 
 def prepare_smiles_files(args, csearch_file):
@@ -145,14 +136,16 @@
             name,
             args.charge,
             args.mult,
             args.constraints_atoms,
             args.constraints_dist,
             args.constraints_angle,
             args.constraints_dihedral,
+            args.complex_type,
+            args.geom
         )
         job_inputs.append(obj)
 
     return job_inputs
 
 
 def prepare_smiles_from_line(line, args):
@@ -198,62 +191,65 @@
 
     constraints_atoms = args.constraints_atoms
     constraints_dist = args.constraints_dist
     constraints_angle = args.constraints_angle
     constraints_dihedral = args.constraints_dihedral
 
     if "constraints_atoms" in csv_smiles.columns:
-        constraints_atoms = csv_smiles.loc[index, "constraints_atoms"]
+        if str(csv_smiles.loc[index, 'constraints_atoms']).lower() != 'nan':
+            constraints_atoms = csv_smiles.loc[index, "constraints_atoms"]
 
     if "constraints_dist" in csv_smiles.columns:
-        constraints_dist = csv_smiles.loc[index, "constraints_dist"]
+        if str(csv_smiles.loc[index, 'constraints_dist']).lower() != 'nan':
+            constraints_dist = csv_smiles.loc[index, "constraints_dist"]
 
     if "constraints_angle" in csv_smiles.columns:
-        constraints_angle = csv_smiles.loc[index, "constraints_angle"]
+        if str(csv_smiles.loc[index, 'constraints_angle']).lower() != 'nan':
+            constraints_angle = csv_smiles.loc[index, "constraints_angle"]
 
     if "constraints_dihedral" in csv_smiles.columns:
-        constraints_dihedral = csv_smiles.loc[index, "constraints_dihedral"]
-
-    (
-        constraints_atoms,
-        constraints_dist,
-        constraints_angle,
-        constraints_dihedral,
-    ) = constraint_fix(
-        constraints_atoms,
-        constraints_dist,
-        constraints_angle,
-        constraints_dihedral,
-    )
+        if str(csv_smiles.loc[index, 'constraints_dihedral']).lower() != 'nan':
+            constraints_dihedral = csv_smiles.loc[index, "constraints_dihedral"]
 
-    charge_found, mult_found = False, False
-    if args.charge is None or args.mult is None:
-        for csv_column in csv_smiles.columns:
-            if str(csv_smiles.loc[index, csv_column]) != 'nan':
-                if csv_column.lower() in ['charge','chrg'] and args.charge is None:
-                    charge = int(csv_smiles.loc[index, csv_column])
-                    charge_found = True
-                elif csv_column.lower() in ['mult','multiplicity'] and args.mult is None:
-                    mult = int(csv_smiles.loc[index, csv_column])
-                    mult_found = True
-
-    if not charge_found:
-        charge = args.charge
-    if not mult_found:
-        mult = args.mult
+    constraints_atoms = csv_2_list(constraints_atoms)
+    constraints_dist = csv_2_list(constraints_dist)
+    constraints_angle = csv_2_list(constraints_angle)
+    constraints_dihedral = csv_2_list(constraints_dihedral)
+
+    charge = args.charge
+    mult = args.mult
+    if "charge" in csv_smiles.columns:
+        if str(csv_smiles.loc[index, 'charge']).lower() != 'nan':
+            charge = csv_smiles.loc[index, "charge"]
+    if "mult" in csv_smiles.columns:
+        if str(csv_smiles.loc[index, 'mult']).lower() != 'nan':
+            mult = csv_smiles.loc[index, "mult"]
+
+    complex_type = args.complex_type
+    if "complex_type" in csv_smiles.columns:
+        if str(csv_smiles.loc[index, 'complex_type']).lower() != 'nan':
+            complex_type = csv_smiles.loc[index, "complex_type"]
+
+    geom = args.geom
+    if "geom" in csv_smiles.columns:
+        if str(csv_smiles.loc[index, 'geom']).lower() != 'nan':
+            geom = csv_smiles.loc[index, "geom"]
+    geom = csv_2_list(geom)
 
     obj = (
         smiles,
         name,
         charge,
         mult,
         constraints_atoms,
         constraints_dist,
         constraints_angle,
         constraints_dihedral,
+        complex_type,
+        geom
     )
 
     return obj
 
 
 def prepare_cdx_files(args, csearch_file):
     # converting to smiles from chemdraw
@@ -269,14 +265,16 @@
             name,
             args.charge,
             args.mult,
             args.constraints_atoms,
             args.constraints_dist,
             args.constraints_angle,
             args.constraints_dihedral,
+            args.complex_type,
+            args.geom
         )
         job_inputs.append(obj)
     return job_inputs
 
 
 def generate_mol_from_cdx(csearch_file):
     cmd_cdx = ["obabel", "-icdx", csearch_file, "-osmi", "-Ocdx.smi"]
@@ -329,14 +327,16 @@
         name,
         charge,
         mult,
         args.constraints_atoms,
         args.constraints_dist,
         args.constraints_angle,
         args.constraints_dihedral,
+        args.complex_type,
+        args.geom
     )
     job_inputs.append(obj)
     if os.path.basename(csearch_file).split('.')[1] in ["gjf", "com"]:
         os.remove(xyz_file)
     os.remove(sdffile)
 
     return job_inputs
@@ -375,14 +375,16 @@
             name,
             charge,
             mult,
             args.constraints_atoms,
             args.constraints_dist,
             args.constraints_angle,
             args.constraints_dihedral,
+            args.complex_type,
+            args.geom
         )
         job_inputs.append(obj)
     return job_inputs
 
 
 def xyz_2_sdf(file):
     """
@@ -542,8 +544,20 @@
     return (
         mol,
         constraints_atoms,
         constraints_dist,
         constraints_angle,
         constraints_dihedral,
         complex_ts
-    )
+    )
+
+def cluster_conformers(mols, heavy_only, max_matches_rmsd, cluster_thr):
+    dists = []
+    for i in range(len(mols)):
+        for j in range(i):
+            dists.append(get_conf_RMS(mols[i],mols[j], i, j, heavy_only, max_matches_rmsd))
+
+    clusts = Butina.ClusterData(dists, len(mols), cluster_thr, isDistData=True, reordering=True)
+    centroids = [x[0] for x in clusts]
+    cluster_mols = [mols[x] for x in centroids]
+
+    return cluster_mols, centroids
```

### Comparing `aqme-1.5.0/aqme/filter.py` & `aqme-1.5.1/aqme/filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 #####################################################.
 #        This file stores all the functions         #
 #             used for filtering                    #
 #####################################################.
 
-# from functools import partial
-# from rdkit.Chem import AllChem as Chem
-# from rdkit.Chem import rdMolTransforms, Descriptors
-from rdkit.Chem import Descriptors
+from rdkit import Chem
+from rdkit.Chem import rdMolTransforms, Descriptors
 from aqme.utils import periodic_table, get_conf_RMS
 
 # Aux functions of the geometry filter
 # def is_carbene_like(neighbours):
 #     """
 #     Takes a list of the metal neighbour atoms and returns True if they can be considered as if it were a carbene.
 
@@ -110,14 +108,16 @@
 
 #     Returns
 #     -------
 #     bool
 #             Whether it passes the angle requirements or not
 #     """
 
+#     from functools import partial
+
 #     is_lineal = partial(is_around_angle, angle=180, offset=offset)
 #     get_angle = lambda i, j: rdMolTransforms.GetAngleDeg(mol, i, metal_idx, j)
 #     passing = True
 
 #     if len(ligand_atoms) == 3:  # For complexes with 3 Ph_Py ligands:
 #         i, j, k = ligand_atoms
 #         angles = [get_angle(a[1], b[1]) for a, b in [(i, j), (i, k), (j, k)]]
@@ -129,24 +129,24 @@
 #         (i, i2), (j, j2) = ligand_atoms
 #         angle = get_angle(i2, j2)
 #         passing = is_lineal(angle)
 
 #     return passing
 
 
-# def passes_Ir_bidentate_x3_rule(mol, angle_off):
+# def passes_Ir_bidentate_x3_rule(mol, angle_thres):
 #     """
 #     Checks if a mol containing an Ir metal complex passes the bidentate x3
 #     rule or not.
 
 #     Parameters
 #     ----------
 #     mol : rdkit.Chem.Mol
 #             The molecule to be tested.
-#     angle_off : float
+#     angle_thres : float
 #             Angle in degrees that acts as tolerance around 180º
 
 #     Returns
 #     -------
 #     bool
 #             True if it has passed the rule
 #     """
@@ -213,131 +213,94 @@
 #                     else:
 #                         if not mol_i.GetAtomWithIdx(atom_j).IsInRingSize(5):
 #                             if mol.GetAtomWithIdx(atom_j).IsInRingSize(5):
 #                                 ligand_atoms.append([atom_i, atom_j])
 #                                 break
 #     # Check Angles
 #     passing = passing and passes_Ir_bidentate_x3_rule_angle_requirements(
-#         ligand_atoms, mol_conf, metal_idx, angle_off
+#         ligand_atoms, mol_conf, metal_idx, angle_thres
 #     )
 #     return passing
 
 
-# # Main API of the geometry filter
-# def geom_rules_output(mol, args, log, file, print_error_geom_rules):
-#     """
-#     returns if a mol object passes all the discarding rules or not.
+# Main API of the geometry filter
+def geom_filter(self,mol,geom):
+    """
+    Returns whether a mol object passes all the geometric rules.
 
-#     Parameters
-#     ----------
-#     mol : rdkit.Chem.Mol
-#             molecule to be tested.
-#     args : argparse.args
-#             [description]
-#     log : Logger
-#             [description]
-#     file : str
-#             Only used to write to the log
-#     print_error_geom_rules : bool
-#             Controls extra writing to the log.
+    Parameters
+    ----------
+    self : argparse.args
+            Self object with the AQME arguments used
+    mol : rdkit.Chem.Mol
+            Molecule to be tested.
+
+    Returns
+    -------
+    bool
+        If True, it means that it is in accordance with the rules
+    """
 
-#     Returns
-#     -------
-#     bool
-#             If True, it means that it is in accordance with the rules
-#     """
+    # detects if the geometry rule is for atoms, bonds, angles or dihedrals
 
-#     passing = True
-#     for rule in args.geom_rules:
-#         if rule == "Ir_bidentate_x3":
-#             passing = passes_Ir_bidentate_x3_rule(mol, args.angle_off)
-#         else:
-#             var = rule.split(",")
-#             if len(var) < 2:
-#                 log.write("x  The geom_rules parameter(s) was not correctly defined, this filter will be turned off")
-#                 return True
-#             atoms_filter = var[0].split("-")
-#             angle_rules = int(var[1])
-#             # the elements of this initial list will be replaced by the corresponding atom id numebrs
-#             atom_idx = ["ATOM1", "ATOM2", "ATOM3"]
-
-#             find_angle = 0
-#             incompatibility_found = False
-#             for atom in mol.GetAtoms():
-#                 # count matches
-#                 neigh_count_first = 0
-#                 neigh_count_second = 0
-#                 sym_0, sym_1, sym_2 = atoms_filter
-#                 # Finds the metal atom and gets the atom types and indexes of all its neighbours
-#                 if atom.GetSymbol() == sym_1:
-#                     # idx of the central atom
-#                     atom_idx[1] = atom.GetIdx()
-#                     for x in atom.GetNeighbors():
-#                         sym = x.GetSymbol()
-#                         if sym == sym_0 or sym == sym_2:
-#                             # this ensures that both neighbours are used
-#                             if sym == sym_0 and sym == sym_2:
-#                                 if neigh_count_first <= neigh_count_second:
-#                                     neigh_count_first += 1
-#                                     atom_idx[0] = x.GetIdx()
-#                                 else:
-#                                     neigh_count_second += 1
-#                                     atom_idx[2] = x.GetIdx()
-#                             elif sym == sym_0:
-#                                 neigh_count_first += 1
-#                                 atom_idx[0] = x.GetIdx()
-#                             elif sym == sym_2:
-#                                 neigh_count_second += 1
-#                                 atom_idx[2] = x.GetIdx()
-#                             # count matches
-#                             matches = neigh_count_first + neigh_count_second
-#                             if matches > 2:
-#                                 if not print_error_geom_rules:
-#                                     log.write(f"x  There are multiple options in geom_rules for {file}, this filter will be turned off")
-#                                     incompatibility_found = True
-#                                     break
-#                     if neigh_count_first == 1 and neigh_count_second == 1:
-#                         find_angle += 1
-#             if find_angle == 0 and not incompatibility_found:
-#                 if not print_error_geom_rules:
-#                     log.write(f"x  No angles matching the description from geom_rules in {file}, this filter will be turned off")
-#             elif find_angle > 1:
-#                 log.write(f"x  {file} contain more than one atom that meets the geom_rules criteria, this filter will be turned off")
-#             elif find_angle == 1:
-#                 # Retrieve the only 3D conformer generated in that mol object for rdMolTransforms
-#                 mol_conf = mol.GetConformer(0)
-#                 # Calculate the angle between the 3 elements
-#                 angle = rdMolTransforms.GetAngleDeg(
-#                     mol_conf, atom_idx[0], atom_idx[1], atom_idx[2]
-#                 )
-#                 passing = not is_around_angle(angle, angle_rules, args.angle_off)
-#             if not passing:
-#                 break
-#     return passing
+    passing = True
+    if geom != []:
+        passing = False
+        if len(geom) != 2:
+            self.args.log.write(f"x  The geom option {geom} was not correctly defined, the geometric filter will be turned off! Correct format: [SMARTS,THRESHOLD], for example [CCCO,180] for a 180 degree dihedral")
+            return passing
+        smarts = geom[0]
+        geom_val = geom[1]
+
+        # SMARTS match to detect the atoms and calculate the geometric value. Then, check if the value
+        # is within the threshold
+        matches = []
+        try:
+            matches = mol.GetSubstructMatches(Chem.MolFromSmarts(smarts))
+        except: # I tried to make this except more specific for Boost.Python.ArgumentError, but apparently it's not as simple as it looks
+            matches = mol.GetSubstructMatches(Chem.MolFromSmarts(f'[{smarts}]'))
+        if len(matches) > 0:
+            matches = list(matches[0])
+        mol_conf = mol.GetConformer(0) # Retrieve the only 3D conformer generated in that mol object for rdMolTransforms
+        smarts_content = ''.join(smarts.replace('[',']').split(']')) # this way both 'ATOM' and '[ATOM]' work
+        if smarts_content in periodic_table():
+            if len(matches) >= 1:
+                passing = True
+        elif len(matches) == 2:
+            mol_val = rdMolTransforms.GetBondLength(mol_conf, matches[0], matches[1])
+            passing = (geom_val - self.args.bond_thres) <= mol_val <= (geom_val + self.args.bond_thres)
+        elif len(matches) == 3:
+            mol_val = rdMolTransforms.GetAngleDeg(mol_conf, matches[0], matches[1], matches[2])
+            passing = (geom_val - self.args.angle_thres) <= mol_val <= (geom_val + self.args.angle_thres)
+        elif len(matches) == 4:
+            mol_val = rdMolTransforms.GetDihedralDeg(mol_conf, matches[0], matches[1], matches[2], matches[3])
+            passing = (geom_val - self.args.dihedral_thres) <= mol_val <= (geom_val + self.args.dihedral_thres)
+
+    return passing
 
 # Mol filters
 def filters(mol, log, molwt_cutoff):
     """
     Applies some basic filters (molwt, salts[currently off], weird atom symbols)
     that only require SMILES data from a compound and returns if the molecule
     passes the filters or not.
     """
 
     # Filter 1
     molwt_cutoff = float(molwt_cutoff)
     if Descriptors.MolWt(mol) >= molwt_cutoff and molwt_cutoff > 0:
-        log.write(f"x   Skipping this molecule as total molar mass > {molwt_cutoff}")
+        log.write(f"x  Skipping this molecule as total molar mass > {molwt_cutoff}")
         return False
 
     # Filter 2
     symbols = [atom.GetSymbol() for atom in mol.GetAtoms()]
 
     unknown_atoms = list(set(symbols) - set(periodic_table()))
     if unknown_atoms:
-        log.write(f" Exiting as atoms [{','.join(unknown_atoms)}] are not in the periodic table")
+        log.write(f"x  Exiting as atoms [{','.join(unknown_atoms)}] are not in the periodic table")
         return False
 
     # Passed
     return True
 
 
 def ewin_filter(
```

### Comparing `aqme-1.5.0/aqme/qcorr.py` & `aqme-1.5.1/aqme/qcorr.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             "spin_contaminated": 0,
             "duplicate_calc": 0,
             "atom_error": 0,
             "scf_error": 0,
             "no_data": 0,
             "linear_mol_wrong": 0,
             "not_specified": 0,
-            "geom_rules_qcorr": 0,
+            "geom_qcorr": 0,
             "isomerized": 0,
         }
 
         duplicate_data = {
             "File": [],
             "Energies": [],
             "Enthalpies": [],
@@ -295,31 +295,31 @@
         #         destination_data,
         #         self.args.w_dir_main,
         #         f"QCORR-run_{self.args.round_num}-stats.csv",
         #     )
 
     # include geom filters (ongoing work)
 
-    # 			if len(self.args.geom_rules) >= 1:
+    # 			if len(self.args.geom) >= 1:
     # 				passing_rules = True
     # 				valid_mol_gen = True
-    # 				self.args.log.write("  ----- geom_rules filter(s) will be applied to the output file -----\n")
+    # 				self.args.log.write("  ----- geom filter(s) will be applied to the output file -----\n")
     # 				try:
     # 					format_file = file.split('.')[1]
     # 					mol = output_to_mol(file,format_file)
-    # 					print_error_geom_rules=False
+    # 					print_error_geom=False
     # 					if ob_compat and rdkit_compat:
-    # 						passing_rules = geom_rules_output(mol,self.args,self.args.log,file,print_error_geom_rules)
+    # 						passing_rules = geom_output(mol,self.args,self.args.log,file,print_error_geom)
     # 						if not passing_rules:
-    # 							errortype = 'fail_geom_rules'
+    # 							errortype = 'fail_geom'
     # 					os.remove(file.split('.')[0]+'.mol')
     # 				except AttributeError:
     # 					valid_mol_gen = False
     # 					os.remove(file.split('.')[0]+'.mol')
-    # 					self.args.log.write("The file could not be converted into a mol object, geom_rules filter(s) will be disabled\n")
+    # 					self.args.log.write("The file could not be converted into a mol object, geom filter(s) will be disabled\n")
 
     def cclib_init(self, file, file_name):
         """
         Determine termination and error types (initial determination), create json files
         with cclib and load the data in the cclib json files
         """
 
@@ -862,17 +862,17 @@
             destination = destination_error.joinpath("error/scf_error/")
             file_terms["scf_error"] += 1
 
         elif errortype == "no_data":
             destination = destination_error.joinpath("error/no_data/")
             file_terms["no_data"] += 1
 
-        elif errortype == "fail_geom_rules":
-            destination = destination_error.joinpath("geom_rules_filter/")
-            file_terms["geom_rules_qcorr"] += 1
+        elif errortype == "fail_geom":
+            destination = destination_error.joinpath("geom_filter/")
+            file_terms["geom_qcorr"] += 1
 
         elif errortype == "isomerization":
             destination = destination_error.joinpath("isomerization/")
             file_terms["isomerized"] += 1
 
         elif errortype == "freq_no_conv":
             destination = destination_error.joinpath("freq_no_conv/")
@@ -908,16 +908,17 @@
         ana_data.at[0, "SCF error"] = file_terms["scf_error"]
         ana_data.at[0, "No data"] = file_terms["no_data"]
         ana_data.at[0, "Basis set error"] = file_terms["atom_error"]
         ana_data.at[0, "Other errors"] = file_terms["not_specified"]
         if float(self.args.s2_threshold) > 0.0:
             ana_data.at[0, "Spin contamination"] = file_terms["spin_contaminated"]
         ana_data.at[0, "Duplicates"] = file_terms["duplicate_calc"]
-        if len(self.args.geom_rules) >= 1:
-            ana_data.at[0, "geom_rules filter"] = file_terms["geom_rules_qcorr"]
+        if len(self.args.geom) >= 1:
+            ana_data.at[0, "geom filter"] = file_terms["geom_qcorr"]
         if self.args.isom_type is not None:
             ana_data.at[0, "Isomerization"] = file_terms["isomerized"]
         path_as_str = self.args.initial_dir.as_posix()
         csv_qcorr = path_as_str + f"/QCORR-run_{self.args.round_num}-stats.csv"
-        ana_data.to_csv(csv_qcorr, index=False)
+        if self.args.verbose:
+            ana_data.to_csv(csv_qcorr, index=False)
 
         return csv_qcorr
```

### Comparing `aqme-1.5.0/aqme/qcorr_utils.py` & `aqme-1.5.1/aqme/qcorr_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -613,15 +613,15 @@
                     if "*" in outlines[j]:
                         break
                     else:
                         keywords_line += outlines[j][6:]
                 cclib_data["metadata"]["keywords line"] = keywords_line[1:].rstrip("\n")
                 calc_type = "ground_state"
                 for keyword in keywords_line.split():
-                    if keyword.lower() in ["OptTS",'NEB-TS']:
+                    if keyword.lower() in ["optts",'neb-ts']:
                         calc_type = "transition_state"
                         break
                     if keyword.lower()[0:3] == 'pal':
                         cclib_data["metadata"]["processors"] = keyword[3]
                 cclib_data["metadata"]["ground or transition state"] = calc_type
             
             elif 'END OF INPUT' in line:
```

### Comparing `aqme-1.5.0/aqme/qdescp.py` & `aqme-1.5.1/aqme/qdescp.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
    w_dir_main : str, default=os.getcwd()
       Working directory
    destination : str, default=None,
       Directory to create the JSON file(s)
    program : str, default=None
       Program required to create the new descriptors. Current options: 'xtb', 'nmr'
-   qdescp_atom : str, default=None
-      Type of atom to calculate atomic properties (i.e., qdescp_atom='P' to 
-      study the properties of phosphorus atoms in monodentate phosphines)
+   qdescp_atoms : list of str, default=[]
+      Type of atom or group to calculate atomic properties. This option admits atoms 
+      (i.e., qdescp_atoms=['P']) and SMART patterns (i.e., qdescp_atoms=['C=O']) 
    robert : bool, default=True
       Creates a database ready to use in an AQME-ROBERT machine learning workflow,
       combining the input CSV with SMILES/code_name and the calculated xTB/DBSTEP descriptors
 
 xTB descriptors
 +++++++++++++++
 
@@ -112,165 +112,184 @@
 )
 
 from aqme.csearch.crest import xyzall_2_xyz
 
 
 class qdescp:
     """
-    Class containing all the functions from the QDESCP module related to xTB properties for SDF files.
+    Class containing all the functions from the QDESCP module
     """
 
     def __init__(self, **kwargs):
 
         start_time_overall = time.time()
+
         # load default and user-specified variables
         self.args = load_variables(kwargs, "qdescp")
 
         if self.args.destination is None:
             destination = self.args.initial_dir.joinpath("QDESCP")
         else:
             destination = Path(self.args.destination)
 
-        # retrieves the different files to run in QDESCP
+        # retrieve the different files to run in QDESCP
         _ = check_files(self,'qdescp')
 
         qdescp_program = True
         if self.args.program is None:
             qdescp_program = False
         if qdescp_program:
             if self.args.program.lower() not in ["xtb", "nmr"]:
                 qdescp_program = False
         if not qdescp_program:
             self.args.log.write("\nx  Program not supported for QDESCP descriptor generation! Specify: program='xtb' (or nmr)")
             self.args.log.finalize()
             sys.exit()
 
+        update_atom_props = [] # keeps track of the molecules with suitable atomic properties when using qdescp_atoms
+
+        self.args.log.write(f"\nStarting QDESCP-{self.args.program} with {len(self.args.files)} job(s)\n")
+
+        # run the main xTB workflow
         if self.args.program.lower() == "xtb":
-            mol_prop = ["total energy","HOMO-LUMO gap/eV","electronic energy","Dipole module/D",
+            mol_props = ["total energy","HOMO-LUMO gap/eV","electronic energy","Dipole module/D",
                 "Total charge","HOMO","LUMO","Fermi-level/eV","Total dispersion C6",
                 "Total dispersion C8","Total polarizability alpha","Total FOD"]
-            atom_prop = ["partial charges","mulliken charges","cm5 charges","FUKUI+","FUKUI-",
+            atom_props = ["partial charges","mulliken charges","cm5 charges","FUKUI+","FUKUI-",
                 "FUKUIrad","s proportion","p proportion","d proportion","Coordination numbers",
                 "Dispersion coefficient C6","Polarizability alpha","FOD","FOD s proportion",
                 "FOD p proportion","FOD d proportion",'DBSTEP_Vbur']
-            self.gather_files_and_run(destination,atom_prop)
+            if len(self.args.qdescp_atoms) == 0:
+                atom_props.remove('DBSTEP_Vbur')
 
-        elif self.args.program.lower() == "nmr":
-            mol_prop = None
-            atom_prop = ["NMR Chemical Shifts"]
-
-        if self.args.boltz == "False":
-            self.args.boltz = False
-        elif self.args.boltz == "True":
-            self.args.boltz = True
+            update_atom_props = self.gather_files_and_run(destination,atom_props,update_atom_props)
 
+        if len(update_atom_props) > 0:
+            atom_props = update_atom_props
+
+        # Boltzmann averaging of xTB values and DFT-NMR workflow
         qdescp_csv = "QDESCP_boltz_descriptors.csv"
+        boltz_dir = Path(f"{destination}/boltz")
+        if os.path.exists(f"{boltz_dir}"): 
+            self.args.log.write(f'\nx  A previous folder of {boltz_dir} already existed, it was removed and replaced with the results of this QDESCP run.')
+            shutil.rmtree(f"{boltz_dir}")
+        boltz_dir.mkdir(exist_ok=True, parents=True)
         if self.args.boltz:
-            self.args.log.write('\no  Running RDKit and collecting molecular properties')
-            boltz_dir = Path(f"{destination}/boltz")
-            boltz_dir.mkdir(exist_ok=True, parents=True)
             if self.args.program.lower() == "xtb":
+                self.args.log.write('\no  Running RDKit and collecting molecular properties')
                 for file in self.args.files:
                     mol = Chem.SDMolSupplier(file, removeHs=False)[0]
                     name = file.replace("/", "\\").split("\\")[-1].split(".")[0]
                     json_files = glob.glob(
                         str(destination) + "/" + name + "_conf_*.json"
                     )
-                    get_boltz_props(json_files, name, boltz_dir, "xtb", self, mol_prop, atom_prop, mol=mol)
-                self.write_csv_boltz_data(destination,qdescp_csv)
+                    _ = get_boltz_props(json_files, name, boltz_dir, "xtb", self, mol_props, atom_props, mol=mol)
+                _ = self.write_csv_boltz_data(destination,qdescp_csv)
 
             elif self.args.program.lower() == "nmr":
+                mol_props = None
+                atom_props = ["NMR Chemical Shifts"]
                 if self.args.files[0].split('.')[1].lower() not in ["json"]:
                     self.args.log.write(f"\nx  The format used ({self.args.files[0].split('.')[1].lower()}) is not compatible with QDESCP with NMR! Formats accepted: json")
                     self.args.log.finalize()
                     sys.exit()
 
-                for file in self.args.files:
-                    name = file.replace("/", "\\").split("\\")[-1].split("_conf")[0]
-                    json_files = glob.glob(
-                        str(os.path.dirname(os.path.abspath(file)))
-                        + "/"
-                        + name
-                        + "_conf_*.json"
-                    )
-                    get_boltz_props(
-                        json_files,
-                        name,
-                        boltz_dir,
-                        "nmr",
-                        self,
-                        mol_prop,
-                        atom_prop,
-                        self.args.nmr_atoms,
-                        self.args.nmr_slope,
-                        self.args.nmr_intercept,
-                        self.args.nmr_experim,
-                    )
+                name = self.args.files[0].replace("/", "\\").split("\\")[-1].split("_conf")[0]
+                json_files = glob.glob(
+                    str(os.path.dirname(os.path.abspath(self.args.files[0])))
+                    + "/"
+                    + name
+                    + "_conf_*.json"
+                )
+                get_boltz_props(
+                    json_files,
+                    name,
+                    boltz_dir,
+                    "nmr",
+                    self,
+                    mol_props,
+                    atom_props,
+                    self.args.nmr_atoms,
+                    self.args.nmr_slope,
+                    self.args.nmr_intercept,
+                    self.args.nmr_experim,
+                )
 
-        if self.args.robert == "False":
-            self.args.robert = False
-        if self.args.robert:
+        # AQME-ROBERT workflow
+        if self.args.robert and self.args.program.lower() == "xtb":
             if self.args.csv_name is None:
-                self.args.log.write(f"\n-  The input csv_name with SMILES and code_name is missing. A combined database for AQME-ROBERT workflows will not be created.")
+                self.args.log.write(f"\nx  The input csv_name with SMILES and code_name columns are missing. A combined database for AQME-ROBERT workflows will not be created.")
             elif not Path(f"{self.args.csv_name}").exists():
                 self.args.log.write(f"\nx  The input csv_name provided ({self.args.csv_name}) is not valid. A combined database for AQME-ROBERT workflows will not be created.")
             else:
                 combined_df = pd.DataFrame()
                 qdescp_df = pd.read_csv(qdescp_csv)
                 input_df = pd.read_csv(self.args.csv_name)
                 if 'code_name' not in input_df.columns:
                     self.args.log.write(f"\nx  The input csv_name provided ({self.args.csv_name}) does not contain the code_name column. A combined database for AQME-ROBERT workflows will not be created.")
                 elif 'SMILES' in input_df.columns or 'smiles' in input_df.columns or 'Smiles' in input_df.columns:
                     path_json = os.path.dirname(Path(qdescp_df['Name'][0]))
                     for i,input_name in enumerate(input_df['code_name']):
                         # match the entries of the two databases using the entry name
                         qdescp_col = input_df.loc[i].to_frame().T.reset_index(drop=True) # transposed, reset index
-                        input_col = qdescp_df.loc[(qdescp_df['Name'] == f'{path_json}/{input_name}_rdkit_boltz') | (qdescp_df['Name'] == f'{path_json}/{input_name}_boltz')]
+                        input_col = qdescp_df.loc[(qdescp_df['Name'] == f'{path_json}/{input_name}_rdkit_boltz') | (qdescp_df['Name'] == f'{path_json}/{input_name}_boltz') | (qdescp_df['Name'] == f'{path_json}/{input_name}_0_rdkit_boltz') | (qdescp_df['Name'] == f'{path_json}/{input_name}_1_rdkit_boltz') | (qdescp_df['Name'] == f'{path_json}/{input_name}_2_rdkit_boltz')]
                         input_col = input_col.drop(['Name'], axis=1).reset_index(drop=True)
                         combined_row = pd.concat([qdescp_col,input_col], axis=1)
-                        combined_df = combined_df.append(combined_row, ignore_index=True)
-                    _ = combined_df.to_csv(f'AQME-ROBERT_{self.args.csv_name}', index = None, header=True)
-                    self.args.log.write(f"o  The AQME-ROBERT_{self.args.csv_name} file containing the database ready for the AQME-ROBERT workflow was successfully created in {self.args.initial_dir}")
+                        combined_df = pd.concat([combined_df, combined_row], ignore_index=True)
+                    combined_df = combined_df.dropna(axis=0)
+                    csv_basename = os.path.basename(self.args.csv_name)
+                    csv_path = self.args.initial_dir.joinpath(f'AQME-ROBERT_{csv_basename}')
+                    _ = combined_df.to_csv(f'{csv_path}', index = None, header=True)
+                    self.args.log.write(f"o  The AQME-ROBERT_{csv_basename} file containing the database ready for the AQME-ROBERT workflow was successfully created in {self.args.initial_dir}")
                 else:
                     self.args.log.write(f"\nx  The input csv_name provided ({self.args.csv_name}) does not contain the SMILES column. A combined database for AQME-ROBERT workflows will not be created.")
 
         elapsed_time = round(time.time() - start_time_overall, 2)
         self.args.log.write(f"\nTime QDESCP: {elapsed_time} seconds\n")
         self.args.log.finalize()
 
     def write_csv_boltz_data(self, destination, qdescp_csv):
+        """
+        Concatenate the values for all calculations
+        """
+        
         boltz_json_files = glob.glob(str(destination) + "/boltz/*.json")
-        dfs = []  # an empty list to store the data frames
+        dfs = [] 
         for file in boltz_json_files:
-            data = pd.read_json(file, lines=True)  # read data frame from json file
+            data = pd.read_json(file, lines=True)
             data["Name"] = file.split(".json")[0]
-            dfs.append(data)  # append the data frame to the list
+            dfs.append(data)
+        if len(dfs) > 0:
+            temp = pd.concat(dfs, ignore_index=True) 
+            temp.to_csv(qdescp_csv, index=False)
+            self.args.log.write(f"o  The {qdescp_csv} file containing Boltzmann weighted xTB, DBSTEP and RDKit descriptors was successfully created in {self.args.initial_dir}")
+        else:
+            self.args.log.write(f"x  No CSV file containing Boltzmann weighted descriptors was created. This might happen when using the qdescp_atoms option with an atom/group that is not found in any of the calculations")
 
-        temp = pd.concat(
-            dfs, ignore_index=True
-        )  # concatenate all the data frames in the list.
-        temp.to_csv(qdescp_csv, index=False)
-        self.args.log.write(f"o  The {qdescp_csv} file containing Boltzmann weighted xTB, DBSTEP and RDKit descriptors was successfully created in {self.args.initial_dir}")
+    def gather_files_and_run(self, destination, atom_props, update_atom_props):
+        """
+        Load all the input files, execute xTB calculations, gather descriptors and clean up scratch data
+        """
 
-    def gather_files_and_run(self, destination, atom_prop):
         bar = IncrementalBar(
             "\no  Number of finished jobs from QDESCP", max=len(self.args.files)
         )
         # write input files
         if self.args.files[0].split('.')[1].lower() not in ["sdf", "xyz", "pdb"]:
             self.args.log.write(f"\nx  The format used ({self.args.files[0].split('.')[1].lower()}) is not compatible with QDESCP with xTB! Formats accepted: sdf, xyz, pdb")
             self.args.log.finalize()
             sys.exit()
 
         for file in self.args.files:
             xyz_files, xyz_charges, xyz_mults = [], [], []
-            name = file.replace("/", "\\").split("\\")[-1].split(".")[0]
+            name = os.path.basename(file).split('.')[0]
+            ext = os.path.basename(file).split(".")[1]
             self.args.log.write(f"\n\n   ----- {name} -----")
-            if file.split(".")[1].lower() in ["sdf", "xyz", "pdb"]:
-                if file.split(".")[1].lower() == "xyz":
+            if ext.lower() in ["sdf", "xyz", "pdb"]:
+                if ext.lower() == "xyz":
                     # separate the parent XYZ file into individual XYZ files
                     xyzall_2_xyz(file, name)
                     for conf_file in glob.glob(f"{name}_conf_*.xyz"):
                         if self.args.charge is None:
                             charge_xyz, _ = read_xyz_charge_mult(conf_file)
                         else:
                             charge_xyz = self.args.charge
@@ -280,45 +299,45 @@
                             mult_xyz = self.args.mult
                         xyz_files.append(
                             os.path.dirname(os.path.abspath(file)) + "/" + conf_file
                         )
                         xyz_charges.append(charge_xyz)
                         xyz_mults.append(mult_xyz)
 
-                elif file.split(".")[1].lower() == "pdb":
+                elif ext.lower() == "pdb":
                     command_pdb = [
                         "obabel",
                         "-ipdb",
                         file,
                         "-oxyz",
                         f"-O{os.path.dirname(os.path.abspath(file))}/{name}_conf_.xyz",
                         "-m",
                     ]
                     subprocess.run(
                         command_pdb,
                         stdout=subprocess.DEVNULL,
                         stderr=subprocess.DEVNULL,
                     )
 
-                elif file.split(".")[1].lower() == "sdf":
+                elif ext.lower() == "sdf":
                     command_sdf = [
                         "obabel",
                         "-isdf",
                         file,
                         "-oxyz",
                         f"-O{os.path.dirname(os.path.abspath(file))}/{name}_conf_.xyz",
                         "-m",
                     ]
                     subprocess.run(
                         command_sdf,
                         stdout=subprocess.DEVNULL,
                         stderr=subprocess.DEVNULL,
                     )
 
-            if file.split(".")[1].lower() in ["sdf", "pdb"]:
+            if ext.lower() in ["sdf", "pdb"]:
                 if self.args.charge is None:
                     _, charges, _, _ = mol_from_sdf_or_mol_or_mol2(file, "csearch", self.args)
                 else:
                     charges = [self.args.charge] * len(
                         glob.glob(
                             f"{os.path.dirname(os.path.abspath(file))}/{name}_conf_*.xyz"
                         )
@@ -338,22 +357,25 @@
                     )
                 ):
                     xyz_files.append(f)
                     xyz_charges.append(charges[count])
                     xyz_mults.append(mults[count])
 
             for xyz_file, charge, mult in zip(xyz_files, xyz_charges, xyz_mults):
-                name = os.path.basename(xyz_file.split(".")[0])
-                self.args.log.write(f"\n   Running xTB and collecting properties")
-                self.run_sp_xtb(xyz_file, charge, mult, name, destination)
-                self.collect_xtb_properties(atom_prop)
-                self.cleanup(name, destination)
+                name_xtb = os.path.basename(xyz_file.split(".")[0])
+                self.args.log.write(f"\no   Running xTB and collecting properties")
+                self.run_sp_xtb(xyz_file, charge, mult, name_xtb, destination)
+                path_name = Path(os.path.dirname(file)).joinpath(os.path.basename(file).split(".")[0])
+                update_atom_props = self.collect_xtb_properties(path_name, atom_props, update_atom_props)
+                self.cleanup(name_xtb, destination)
             bar.next()
         bar.finish()
 
+        return update_atom_props
+
     def run_sp_xtb(self, xyz_file, charge, mult, name, destination):
         """
         Runs single point xTB calculations to collect properties
         """
 
         dat_dir = destination / name
         dat_dir.mkdir(exist_ok=True, parents=True)
@@ -458,28 +480,28 @@
         if self.args.qdescp_solvent is not None:
             command4.append("--alpb")
             command4.append(f"{self.args.qdescp_solvent}")
         run_command(command4, self.xtb_fod)
 
         os.chdir(self.args.initial_dir)
 
-    def collect_xtb_properties(self,atom_prop):
+    def collect_xtb_properties(self,name_initial,atom_props,update_atom_props):
         """
         Collects all xTB properties from the files and puts them in a JSON file
         """
 
         (
-            energy,
+            _,
             total_charge,
-            homo_lumo,
+            _,
             homo,
             lumo,
             atoms,
-            numbers,
-            chrgs,
+            _,
+            _,
             dipole_module,
             Fermi_level,
             transition_dipole_moment,
             covCN,
             C6AA,
             alpha,
             homo_occ,
@@ -544,54 +566,114 @@
 
         with open(self.xtb_xyz, "r") as f:
             inputs = f.readlines()
 
         coordinates = [inputs[i].strip().split()[1:] for i in range(2, int(inputs[0].strip()) + 2)]
         json_data["coordinates"] = coordinates
 
-        
-        if self.args.qdescp_atom is not None:
-            idx_dbstep, idx_xtb = None, None
-
-            # calculate DBSTEP descriptors
-            self.args.log.write(f"\n   Running DBSTEP and collecting properties")
-
-            hit_at = 0
-            for i,line in enumerate(inputs):
-                if i > 2:
-                    if line.split()[0] == self.args.qdescp_atom:
-                        hit_at += 1
-                        idx_dbstep = i-1 # DBSTEP starts from index 1 (i.e. first atom has idx 1)
-                        idx_xtb = i-2
-
-            if hit_at > 1:
-                self.args.log.write(f'WARNING! More than one {self.args.qdescp_atom} were found, using {self.args.qdescp_atom} with index {idx_dbstep}.')
-
-            if idx_dbstep is not None:
-                # calculates buried volume to the type of atom selected
+        if len(self.args.qdescp_atoms) > 0:
+            # detect SMILES from SDF files generated by CSEARCH or create mol objects from regular SDF files
+            sdf_file = f'{name_initial}.sdf'
+            with open(sdf_file, "r") as F:
+                lines = F.readlines()
+
+            smi_exist = False
+            for i, line in enumerate(lines):
+                if ">  <SMILES>" in line:
+                    smi = lines[i + 1].split()[0]
+                    mol = Chem.AddHs(Chem.MolFromSmiles(smi))
+                    smi_exist = True
+            if not smi_exist:
+                mol = Chem.SDMolSupplier(sdf_file, removeHs=False)
+
+            # find the target atoms or groups
+            for pattern in self.args.qdescp_atoms:
+                matches = []
                 try:
-                    dbstep_obj = db.dbstep(self.xtb_xyz,atom1=idx_dbstep,r=float(self.args.dbstep_r),commandline=True,verbose=False,volume=True)  
-                    json_data['DBSTEP_Vbur'] = float(dbstep_obj.bur_vol)
-                except TypeError:
-                    self.args.log.write(f'WARNING! DBSTEP is not working correctly, DBSTEP properties will not be calculated.')
-                    json_data['DBSTEP_Vbur'] = 'NaN'
-
-                # selects xTB atom properties
-                for prop in atom_prop:
-                    if prop != 'DBSTEP_Vbur': # already set the value of the atom instead of a list of values
-                        json_data[prop] = json_data[prop][idx_xtb]
-
-            else:
-                self.args.log.write(f'WARNING! No {self.args.qdescp_atom} atoms were found, using NaN as the value.')
-                json_data['DBSTEP_Vbur'] = 'NaN'
-                for prop in atom_prop:
-                    json_data[prop] = 'NaN'
+                    matches = mol.GetSubstructMatches(Chem.MolFromSmarts(pattern))
+                except: # I tried to make this except more specific for Boost.Python.ArgumentError, but apparently it's not as simple as it looks
+                    try:
+                        matches = mol.GetSubstructMatches(Chem.MolFromSmarts(f'[{pattern}]'))
+                    except:
+                        self.args.log.write(f"x  WARNING! SMARTS pattern was not specified correctly! Make sure the qdescp_atoms option uses this format: \"[C]\" for atoms, \"[C=N]\" for bonds, and so on.")
+      
+                if len(matches) == 0:
+                    self.args.log.write(f"x  WARNING! SMARTS pattern {pattern} not found in the system, this molecule will not be used.")
+
+                elif len(matches) > 1:
+                    self.args.log.write(f"x  WARNING! More than one {pattern} atom was found in the system, this molecule will not be used.")
+
+                elif len(matches) == 1:
+                    # get atom types and sort them to keep the same atom order among different molecules
+                    atom_indices = list(matches[0])
+                    atom_types = []
+                    for atom_idx in atom_indices:
+                        atom_types.append(mol.GetAtoms()[atom_idx].GetSymbol())
+
+                    n_types = len(set(atom_types))
+                    if n_types == 1:
+                        sorted_indices = sorted(atom_indices, key=lambda idx: len(mol.GetAtoms()[idx].GetNeighbors()))
+                    elif n_types > 1:
+                        sorted_indices = sorted(atom_indices, key=lambda idx: mol.GetAtoms()[idx].GetAtomicNum())
+                    
+                    match_idx = 1
+                    match_names = []
+                    # separates atoms when functional groups are used
+                    for atom_idx in sorted_indices:
+                        idx_dbstep, idx_xtb = None, None
+                        idx_dbstep = atom_idx+1 # DBSTEP starts from index 1 (i.e. first atom has idx 1)
+                        idx_xtb = atom_idx
+                        atom_type = mol.GetAtoms()[atom_idx].GetSymbol()
+                        if len(matches[0]) == 1:
+                            match_name = f'{atom_type}'
+                        else:
+                            if n_types == 1:
+                                match_name = f'{pattern}_{atom_type}{match_idx}'
+                                match_idx += 1
+                            elif n_types > 1:
+                                match_name = f'{pattern}_{atom_type}'
+                        match_names.append(match_name)
+
+                        # calculate DBSTEP descriptors
+                        self.args.log.write(f"\no   Running DBSTEP and collecting properties")
+
+                        if idx_dbstep is not None:
+                            # calculates buried volume to the type of atom selected
+                            try:
+                                dbstep_obj = db.dbstep(self.xtb_xyz,atom1=idx_dbstep,r=float(self.args.dbstep_r),commandline=True,verbose=False,volume=True)  
+                                json_data[f'{match_name}_DBSTEP_Vbur'] = float(dbstep_obj.bur_vol)
+                                if f'{match_name}_DBSTEP_Vbur' not in update_atom_props:
+                                    update_atom_props.append(f'{match_name}_DBSTEP_Vbur')
+                            except TypeError:
+                                self.args.log.write(f'x  WARNING! DBSTEP is not working correctly, DBSTEP properties will not be calculated.')
+
+                            # selects xTB atomic properties
+                            for prop in atom_props:
+                                if prop != 'DBSTEP_Vbur': # set the value of the atom instead of a list of values
+                                    json_data[f'{match_name}_{prop}'] = json_data[prop][idx_xtb]
+                                    if f'{match_name}_{prop}' not in update_atom_props:
+                                        update_atom_props.append(f'{match_name}_{prop}')
+
+                    # adding max and min values for functional groups with the same two atoms
+                    if len(match_names) > 1 and n_types == 1:
+                        for prop in atom_props:
+                            prop_values = []
+                            for prop_name in match_names:
+                                prop_values.append(json_data[f'{prop_name}_{prop}'])
+                            json_data[f'{pattern}_max_{prop}'] = max(prop_values)
+                            if f'{pattern}_max_{prop}' not in update_atom_props:
+                                update_atom_props.append(f'{pattern}_max_{prop}')
+                            json_data[f'{pattern}_min_{prop}'] = min(prop_values)
+                            if f'{pattern}_min_{prop}' not in update_atom_props:
+                                update_atom_props.append(f'{pattern}_min_{prop}')
 
         with open(self.xtb_json, "w") as outfile:
             json.dump(json_data, outfile)
+        
+        return update_atom_props
 
     def cleanup(self, name, destination):
         final_json = str(destination) + "/" + name + ".json"
         shutil.move(self.xtb_json, final_json)
         # delete xTB files that does not contain useful data
         files = glob.glob(f"{destination}/{name}/*")
         for file in files:
```

### Comparing `aqme-1.5.0/aqme/qdescp_utils.py` & `aqme-1.5.1/aqme/qdescp_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 ######################################################.
 #        This file stores QDESCP functions           #
 ######################################################.
 
 import json
 import sys
+import os
 import numpy as np
 import pandas as pd
 import ast
 import math
 import rdkit
+from rdkit.Chem import Descriptors
 import warnings
 warnings.filterwarnings('ignore')
 
 GAS_CONSTANT = 8.3144621  # J / K / mol
 J_TO_AU = 4.184 * 627.509541 * 1000.0  # UNIT CONVERSION
 T = 298.15
 
@@ -38,79 +40,84 @@
 
 def get_boltz_props(
     json_files,
     name,
     boltz_dir,
     type,
     self,
-    mol_prop,
-    atom_prop,
+    mol_props,
+    atom_props,
     nmr_atoms=None,
     nmr_slope=None,
     nmr_intercept=None,
     nmr_experim=None,
     mol=None,
 ):
     """
     Retrieves the properties from json files and gives Boltzmann averaged properties
     """
 
-    if type == "nmr":
+    if type.lower() == "nmr":
         if nmr_experim is not None:
             try:
                 exp_data = pd.read_csv(nmr_experim)
             except:
                 self.args.log.write(f'\nx  The CSV file with experimental NMR shifts specified ({nmr_experim}) was not found!')
                 self.args.log.finalize()
                 sys.exit()
 
+    # calculate Boltzmann weights
     energy = []
     for k, json_file in enumerate(json_files):
         json_data = read_json(json_file)
-        if type == "xtb":
+        if type.lower() == "xtb":
             energy.append(json_data["total energy"])
-        elif type == "nmr":
+        elif type.lower() == "nmr":
             energy.append(json_data["optimization"]["scf"]["scf energies"][-1])
 
             json_data["properties"]["NMR"]["NMR Chemical Shifts"] = get_chemical_shifts(
                 json_data, nmr_atoms, nmr_slope, nmr_intercept
             )
             if nmr_experim is not None:
                 list_shift = json_data["properties"]["NMR"]["NMR Chemical Shifts"]
                 df = pd.DataFrame(
                     list_shift.items(),
                     columns=["atom_idx", "conf_{}".format(k + 1)],
                 )
                 df["atom_idx"] = df["atom_idx"] + 1
                 exp_data = exp_data.merge(df, on=["atom_idx"])
-        with open(json_file, "w") as outfile:
-            json.dump(json_data, outfile)
+            with open(json_file, "w") as outfile:
+                json.dump(json_data, outfile)
 
     boltz = get_boltz(energy)
 
+    # get weighted atomic properties
     avg_json_data = {}
-    for prop in atom_prop:
+    for i,prop in enumerate(atom_props):
         prop_list = []
         for json_file in json_files:
             json_data = read_json(json_file)
-            if self.args.qdescp_atom is None:
-                json_data['DBSTEP_Vbur'] = 'NaN'
-            if type == "xtb":
+            if type.lower() == "xtb":
+                # filter off molecules with no atomic properties found when using the qdescp_atoms option
+                if i == 0:
+                    for atom_prop in atom_props:
+                        if atom_prop not in json_data:
+                            return None
                 prop_list.append(json_data[prop])
-            if type == "nmr":
+            if type.lower() == "nmr":
                 prop_list.append(json_data["properties"]["NMR"][prop].values())
-        if self.args.qdescp_atom is None:
+
+        if len(self.args.qdescp_atoms) == 0:
             avg_prop = average_prop_atom(boltz, prop_list)
         else:
             avg_prop = average_prop_mol(boltz, prop_list)
-
-        if type == "nmr":
+        if type.lower() == "nmr":
             dictavgprop = {}
-            for i, key in enumerate(json_data["properties"]["NMR"][prop].keys()):
-                dictavgprop[key] = avg_prop[i]
+            for j, key in enumerate(json_data["properties"]["NMR"][prop].keys()):
+                dictavgprop[key] = avg_prop[j]
             avg_json_data[prop] = dictavgprop
 
             if nmr_experim is not None:
                 list_shift = avg_json_data[prop]
                 df = pd.DataFrame(
                     list_shift.items(),
                     columns=["atom_idx", "boltz_avg"],
@@ -118,36 +125,39 @@
                 df["atom_idx"] = df["atom_idx"].astype(int) + 1
                 exp_data = exp_data.merge(df, on=["atom_idx"])
                 exp_data["error_boltz"] = abs(
                     exp_data["experimental_ppm"] - exp_data["boltz_avg"]
                 )
                 qdescp_nmr = nmr_experim.split(".csv")[0] + "_predicted.csv"
                 exp_data.round(2).to_csv(qdescp_nmr, index=False)
-                self.args.log.write(f"o  The {qdescp_nmr} file containing Boltzmann weighted NMR shifts was successfully created in {self.args.initial_dir}")
+                self.args.log.write(f"o  The {os.path.basename(qdescp_nmr)} file containing Boltzmann weighted NMR shifts was successfully created in {self.args.initial_dir}")
 
-        elif type == "xtb":
-            if self.args.qdescp_atom is not None or avg_prop == 'NaN':
+        elif type.lower() == "xtb":
+            if len(self.args.qdescp_atoms) > 0 or avg_prop == 'NaN':
                 avg_json_data[prop] = avg_prop
             else:
-                avg_json_data[prop] = avg_prop.tolist()                
+                avg_json_data[prop] = avg_prop.tolist()
 
-    if type == "xtb":
-        for prop in mol_prop:
+    # get weighted molecular properties
+    if type.lower() == "xtb":
+        for prop in mol_props:
             prop_list = []
             for json_file in json_files:
                 json_data = read_json(json_file)
                 prop_list.append(json_data[prop])
             avg_prop = average_prop_mol(boltz, prop_list)
             avg_json_data[prop] = avg_prop
 
     final_boltz_file = str(boltz_dir) + "/" + name + "_boltz.json"
-    
+
     # calculate RDKit descriptors
     if mol is not None:
         avg_json_data = get_rdkit_properties(avg_json_data, mol)
+
+    # save descriptors
     with open(final_boltz_file, "w") as outfile:
         json.dump(avg_json_data, outfile)
 
 
 def get_chemical_shifts(json_data, nmr_atoms, nmr_slope, nmr_intercept):
     """
     Retrieves and scales NMR shifts from json files
@@ -213,27 +223,31 @@
 
 
 def get_rdkit_properties(avg_json_data, mol):
     """
     Calculates RDKit molecular descriptors
     """
 
-    avg_json_data["NHOHCount"] = rdkit.Chem.Lipinski.NHOHCount(mol)
-    avg_json_data["FractionCSP3"] = rdkit.Chem.Lipinski.FractionCSP3(mol)
-    avg_json_data["NOCount"] = rdkit.Chem.Lipinski.NOCount(mol)
-    avg_json_data["NumAliphaticRings"] = rdkit.Chem.Lipinski.NumAliphaticRings(mol)
-    avg_json_data["NumAromaticRings"] = rdkit.Chem.Lipinski.NumAromaticRings(mol)
-    avg_json_data["NumHAcceptors"] = rdkit.Chem.Lipinski.NumHAcceptors(mol)
-    avg_json_data["NumHDonors"] = rdkit.Chem.Lipinski.NumHDonors(mol)
-    avg_json_data["NumHeteroatoms"] = rdkit.Chem.Lipinski.NumHeteroatoms(mol)
-    avg_json_data["NumRotatableBonds"] = rdkit.Chem.Lipinski.NumRotatableBonds(mol)
-
-    avg_json_data["TPSA"] = rdkit.Chem.Descriptors.TPSA(mol)
-    avg_json_data["MolLogP"] = rdkit.Chem.Descriptors.MolLogP(mol)
-    # avg_json_data["NumAmideBonds"] = rdkit.Chem.Descriptors.NumAmideBonds(mol)
+    try:
+        descrs = Descriptors.CalcMolDescriptors(mol)
+        for descr in descrs:
+            if descrs[descr] != np.nan and str(descrs[descr]).lower() != 'nan':
+                avg_json_data[descr] = descrs[descr]
+    except AttributeError:
+        avg_json_data["NHOHCount"] = rdkit.Chem.Lipinski.NHOHCount(mol)
+        avg_json_data["FractionCSP3"] = rdkit.Chem.Lipinski.FractionCSP3(mol)
+        avg_json_data["NOCount"] = rdkit.Chem.Lipinski.NOCount(mol)
+        avg_json_data["NumAliphaticRings"] = rdkit.Chem.Lipinski.NumAliphaticRings(mol)
+        avg_json_data["NumAromaticRings"] = rdkit.Chem.Lipinski.NumAromaticRings(mol)
+        avg_json_data["NumHAcceptors"] = rdkit.Chem.Lipinski.NumHAcceptors(mol)
+        avg_json_data["NumHDonors"] = rdkit.Chem.Lipinski.NumHDonors(mol)
+        avg_json_data["NumHeteroatoms"] = rdkit.Chem.Lipinski.NumHeteroatoms(mol)
+        avg_json_data["NumRotatableBonds"] = rdkit.Chem.Lipinski.NumRotatableBonds(mol)
+        avg_json_data["TPSA"] = rdkit.Chem.Descriptors.TPSA(mol)
+        avg_json_data["MolLogP"] = rdkit.Chem.Descriptors.MolLogP(mol)
 
     return avg_json_data
 
 
 def read_fukui(file):
     """
     Read fukui output file created from XTB option. Return data.
```

### Comparing `aqme-1.5.0/aqme/qprep.py` & `aqme-1.5.1/aqme/qprep.py`

 * *Files identical despite different names*

### Comparing `aqme-1.5.0/aqme/templates/template-4-and-5.sdf` & `aqme-1.5.1/aqme/templates/template-4-and-5.sdf`

 * *Files identical despite different names*

### Comparing `aqme-1.5.0/aqme/utils.py` & `aqme-1.5.1/aqme/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from aqme.argument_parser import set_options, var_dict
 from rdkit import RDLogger
 
 GAS_CONSTANT = 8.3144621  # J / K / mol
 J_TO_AU = 4.184 * 627.509541 * 1000.0  # UNIT CONVERSION
 T = 298.15
 
-aqme_version = "1.5.0"
+aqme_version = "1.5.1"
 time_run = time.strftime("%Y/%m/%d %H:%M:%S", time.localtime())
 aqme_ref = f"AQME v {aqme_version}, Alegre-Requena, J. V.; Sowndarya, S.; Perez-Soto, R.; Alturaifi, T.; Paton, R. AQME: Automated Quantum Mechanical Environments for Researchers and Educators. Wiley Interdiscip. Rev. Comput. Mol. Sci. 2023, DOI: 10.1002/wcms.1663."
 
 RDLogger.DisableLog("rdApp.*")
 
 
 def run_command(command, outfile):
@@ -91,47 +91,43 @@
 # class for logging
 class Logger:
     """
     Class that wraps a file object to abstract the logging.
     """
 
     # Class Logger to writargs.input.split('.')[0] output to a file
-    def __init__(self, filein, append, suffix="dat"):
-        self.log = open(f"{filein}_{append}.{suffix}", "w")
+    def __init__(self, filein, append, suffix="dat", verbose=True):
+        if verbose:
+            self.log = open(f"{filein}_{append}.{suffix}", "w")
+        else:
+            self.log = ''
 
     def write(self, message):
         """
         Appends a newline character to the message and writes it into the file.
 
         Parameters
         ----------
         message : str
            Text to be written in the log file.
         """
-        self.log.write(f"{message}\n")
+        try:
+            self.log.write(f"{message}\n")
+        except AttributeError:
+            pass
         print(f"{message}\n")
 
-    def fatal(self, message):
-        """
-        Writes the message to the file. Closes the file and raises an error exit
-
-        Parameters
-        ----------
-        message : str
-           text to be written in the log file.
-        """
-        self.write(message)
-        self.finalize()
-        raise SystemExit(1)
-
     def finalize(self):
         """
         Closes the file
         """
-        self.log.close()
+        try:
+            self.log.close()
+        except AttributeError:
+            pass
 
 
 def move_file(destination, source, file):
     """
     Moves files from the source folder to the destination folder and creates
     the destination folders when needed.
 
@@ -276,14 +272,15 @@
     """
 
     for atom in mol.GetAtoms():
         if atom.GetIdx() in metal_idx:
             re_symbol = metal_sym[metal_idx.index(atom.GetIdx())]
             atomic_number = periodic_table().index(re_symbol)
             atom.SetAtomicNum(atomic_number)
+            atom.SetFormalCharge(0)
 
 
 def get_conf_RMS(mol1, mol2, c1, c2, heavy, max_matches_rmsd):
     """
     Takes in two rdkit.Chem.Mol objects and calculates the RMSD between them.
     (As side efect mol1 is left in the aligned state, if heavy is specified
     the side efect will not happen)
@@ -353,44 +350,57 @@
     for arg, value in opts:
         if arg.find("--") > -1:
             arg_name = arg.split("--")[1].strip()
         elif arg.find("-") > -1:
             arg_name = arg.split("-")[1].strip()
         if arg_name in bool_args:
             value = True
-        if value == "None":
+        elif value == "None":
             value = None
+        elif value == "False":
+            value = False
+        elif value == "True":
+            value = True
+
         if arg_name in ("h", "help"):
             print(f"o  AQME v {aqme_version} is installed correctly! For more information about the available options, see the documentation in https://github.com/jvalegre/aqme")
             sys.exit()
         else:
             # this "if" allows to use * to select multiple files in multiple OS
             if arg_name.lower() == 'files':
                 value = get_files(value)
                 kwargs[arg_name] = value
             else:
                 # this converts the string parameters to lists
-                if arg_name.lower() in ["files", "gen_atoms", "constraints_atoms", "constraints_dist", "constraints_angle", "constraints_dihedral", "atom_types", "cartesians", "nmr_atoms", "nmr_slope", "nmr_intercept"]:
-                    if not isinstance(value, list):
-                        try:
-                            value = ast.literal_eval(value)
-                        except (SyntaxError, ValueError):
-                            # this line fixes issues when using "[X]" or ["X"] instead of "['X']" when using lists
-                            if arg_name.lower() in ["gen_atoms"]:
-                                value = value.replace('[',']').replace(',',']').split(']')
-                                while('' in value):
-                                    value.remove('')
+                if arg_name.lower() in ["files", "gen_atoms", "constraints_atoms", "constraints_dist", "constraints_angle", "constraints_dihedral", "atom_types", "cartesians", "nmr_atoms", "nmr_slope", "nmr_intercept","qdescp_atoms","geom"]:
+                    value = format_lists(value)
                 kwargs[arg_name] = value
 
     # Second, load all the default variables as an "add_option" object
     args = load_variables(kwargs, "command")
     
     return args
 
 
+def format_lists(value):
+    '''
+    Transforms strings into a list
+    '''
+
+    if not isinstance(value, list):
+        try:
+            value = ast.literal_eval(value)
+        except (SyntaxError, ValueError):
+            # this line fixes issues when using "[X]" or ["X"] instead of "['X']" when using lists
+            value = value.replace('[',']').replace(',',']').replace("'",']').split(']')
+            while('' in value):
+                value.remove('')
+    return value
+
+
 def load_variables(kwargs, aqme_module, create_dat=True):
     """
     Load default and user-defined variables
     """
 
     # first, load default values and options manually added to the function
     self = set_options(kwargs)
@@ -429,15 +439,15 @@
                 self.isom_inputs = Path(f"{os.getcwd()}/{self.isom_inputs}")
             else:
                 self.isom_inputs = Path(self.isom_inputs)
 
         error_setup = False
 
         if not self.w_dir_main.exists():
-            txt_yaml += "\nx  The PATH specified as input in the w_dir_main option might be invalid! Using current working directory"
+            txt_yaml += "\nx  The PATH specified as input or files might be invalid!"
             error_setup = True
 
         if error_setup:
             self.w_dir_main = Path(os.getcwd())
             
         # start a log file to track the QCORR module
         if create_dat:
@@ -464,25 +474,25 @@
                 logger_1 = "VISMOL"
 
             if txt_yaml not in [
                 "",
                 f"\no  Importing AQME parameters from {self.varfile}",
                 "\nx  The specified yaml file containing parameters was not found! Make sure that the valid params file is in the folder where you are running the code.\n",
             ]:
-                self.log = Logger(self.initial_dir / logger_1, logger_2)
+                self.log = Logger(self.initial_dir / logger_1, logger_2, verbose=self.verbose)
                 self.log.write(txt_yaml)
                 error_setup = True
 
             if not error_setup:
                 if not self.command_line:
-                    self.log = Logger(self.initial_dir / logger_1, logger_2)
+                    self.log = Logger(self.initial_dir / logger_1, logger_2, verbose=self.verbose)
                 else:
                     # prevents errors when using command lines and running to remote directories
                     path_command = Path(f"{os.getcwd()}")
-                    self.log = Logger(path_command / logger_1, logger_2)
+                    self.log = Logger(path_command / logger_1, logger_2, verbose=self.verbose)
 
                 self.log.write(f"AQME v {aqme_version} {time_run} \nCitation: {aqme_ref}\n")
 
                 if self.command_line:
                     self.log.write(f"Command line used in AQME: aqme {' '.join([str(elem) for elem in sys.argv[1:]])}\n")
 
             if error_setup:
@@ -756,19 +766,30 @@
 
 def check_xtb(self):
     try:
         subprocess.run(
             ["xtb", "-h"], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
         )
     except FileNotFoundError:
-        self.args.log.write("x  xTB is not installed (CMIN-xTB cannot be used)! You can install the program with 'conda install -c conda-forge xtb'")
+        self.args.log.write("x  xTB is not installed (CSEARCH-CREST and CMIN-xTB cannot be used)! You can install the program with 'conda install -c conda-forge xtb'")
         self.args.log.finalize()
         sys.exit()
 
 
+def check_crest(self):
+    try:
+        subprocess.run(
+            ["crest", "-h"], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
+        )
+    except FileNotFoundError:
+        self.args.log.write("x  CREST is not installed (CSEARCH-CREST cannot be used)! You can install the program with 'conda install -c conda-forge crest'")
+        self.args.log.finalize()
+        sys.exit()
+ 
+
 def get_files(value):
     if not isinstance(value, list):
         value = value.replace('[',']').replace(',',']').split(']')
         while('' in value):
             value.remove('')
     new_value = []
     for val in value:
```

### Comparing `aqme-1.5.0/aqme/vismol.py` & `aqme-1.5.1/aqme/vismol.py`

 * *Files identical despite different names*

### Comparing `aqme-1.5.0/aqme.egg-info/PKG-INFO` & `aqme-1.5.1/aqme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aqme
-Version: 1.5.0
+Version: 1.5.1
 Summary: Automated Quantum Mechanical Environments
 Home-page: https://github.com/jvalegre/aqme
-Download-URL: https://github.com/jvalegre/aqme/archive/refs/tags/1.5.0.tar.gz
+Download-URL: https://github.com/jvalegre/aqme/archive/refs/tags/1.5.1.tar.gz
 Author: Shree Sowndarya S. V., Juan V. Alegre Requena
 Author-email: svss@colostate.edu, jvalegre@unizar.es
 License: MIT
 Keywords: workflows,computational chemistry,conformational sampling,cheminformatics,quantum mechanics,DFT,automated
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `aqme-1.5.0/aqme.egg-info/SOURCES.txt` & `aqme-1.5.1/aqme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aqme-1.5.0/setup.py` & `aqme-1.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-version = "1.5.0"
+version = "1.5.1"
 setup(
     name="aqme",
     packages=find_packages(exclude=["tests"]),
     package_data={"aqme": ["templates/*"]},
     version=version,
     license="MIT",
     description="Automated Quantum Mechanical Environments",
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.7",  # Specify which python versions you want to support
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     install_requires=[
         "PyYAML",
-        "pandas",
+        "pandas>=2.0.2",
         "progress",
         "ase",
         "numpy",
         "cclib",
         "matplotlib",
         "seaborn",
         "cffi",
```

### Comparing `aqme-1.5.0/tests/test_cmin.py` & `aqme-1.5.1/tests/test_cmin.py`

 * *Files identical despite different names*

### Comparing `aqme-1.5.0/tests/test_csearch.py` & `aqme-1.5.1/tests/test_csearch.py`

 * *Files identical despite different names*

### Comparing `aqme-1.5.0/tests/test_qcorr.py` & `aqme-1.5.1/tests/test_qcorr.py`

 * *Files 4% similar despite different names*

```diff
@@ -407,14 +407,28 @@
             "QCORR_6",
             "CH4_dup.log",
             "run_QCORR",
             "failed/run_1/duplicates",
             False,
         ),  # test successful termination with no w_dir_main
         (
+            "QCORR_7",
+            "orca_TS_success.out",
+            "run_QCORR",
+            "success",
+            False,
+        ),  # test QCORR with ORCA optimizations
+        (
+            "QCORR_7",
+            "orca_imag_freq.out",
+            None,
+            "failed/run_1/extra_imag_freq",
+            False,
+        ),  # test QCORR with ORCA optimizations
+        (
             None,
             None,
             None,
             None,
             True,
         ),  # reset the initial folder to start another set of tests
         # add genECP test
@@ -921,14 +935,43 @@
 
     elif init_folder == "QCORR_6":
         subprocess.run(cmd_aqme)
 
         # ensure the output file moves to the right folder
         assert path.exists(f"{w_dir_main}/{target_folder}/{file}")
 
+    elif init_folder == "QCORR_7":
+        w_dir_main = f"{path_qcorr}/QCORR_7"
+        cmd_aqme = [
+            "python",
+            "-m",
+            "aqme",
+            "--qcorr",
+            "--files",
+            f"{w_dir_main}/{file}",
+        ]
+        subprocess.run(cmd_aqme)
+
+        # ensure the output file moves to the right folder
+        assert path.exists(f"{w_dir_main}/{target_folder}/{file}")
+
+        if file == "orca_imag_freq.out":
+            assert path.exists(
+                f'{w_dir_main}/failed/run_1/fixed_QM_inputs/{file.split(".")[0]}.inp'
+            )
+
+            # ensure that QCORR applies the correct structural distortions to the errored calcs
+            outfile = open(f'{w_dir_main}/failed/run_1/fixed_QM_inputs/{file.split(".")[0]}.inp',"r",)
+            outlines = outfile.readlines()
+            outfile.close()
+
+            assert 'MaxStep 0.05' in outlines[9]
+            assert 'C  -4.32349420   1.79733020  -0.42830100' in outlines[12]
+
+
     # leave the folders as they were initially to run a different batch of tests
     elif restore_folder:
         os.chdir(path_main)
         shutil.rmtree(f"{path_main}/Example_workflows")
         filepath = Path(f"{path_main}/Example_workflows_original")
         filepath.rename(f"{path_main}/Example_workflows")
         # remove DAT and CSV files generated by QCORR
```

### Comparing `aqme-1.5.0/tests/test_qprep.py` & `aqme-1.5.1/tests/test_qprep.py`

 * *Files identical despite different names*

