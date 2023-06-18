# Comparing `tmp/qsonic-0.6.2.tar.gz` & `tmp/qsonic-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsonic-0.6.2.tar", last modified: Tue May 23 15:21:02 2023, max compression
+gzip compressed data, was "qsonic-0.7.1.tar", last modified: Sun Jun 18 01:03:31 2023, max compression
```

## Comparing `qsonic-0.6.2.tar` & `qsonic-0.7.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:21:02.929183 qsonic-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-23 15:20:44.000000 qsonic-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-23 15:21:02.929183 qsonic-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-23 15:20:44.000000 qsonic-0.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:21:02.925182 qsonic-0.6.2/py/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:21:02.929183 qsonic-0.6.2/py/qsonic/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/mathtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/mpi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    49929 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/picca_continuum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:21:02.929183 qsonic-0.6.2/py/qsonic/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/scripts/qsonic_calib.py
--rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/scripts/qsonic_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    25509 2023-05-23 15:20:44.000000 qsonic-0.6.2/py/qsonic/spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:21:02.929183 qsonic-0.6.2/py/qsonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-23 15:21:02.000000 qsonic-0.6.2/py/qsonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-23 15:21:02.000000 qsonic-0.6.2/py/qsonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:21:02.000000 qsonic-0.6.2/py/qsonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-23 15:21:02.000000 qsonic-0.6.2/py/qsonic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-23 15:21:02.000000 qsonic-0.6.2/py/qsonic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 15:21:02.000000 qsonic-0.6.2/py/qsonic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-23 15:20:44.000000 qsonic-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-23 15:20:44.000000 qsonic-0.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-23 15:21:02.929183 qsonic-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 15:20:44.000000 qsonic-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:21:02.929183 qsonic-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-23 15:20:44.000000 qsonic-0.6.2/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-23 15:20:44.000000 qsonic-0.6.2/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-23 15:20:44.000000 qsonic-0.6.2/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-23 15:20:44.000000 qsonic-0.6.2/tests/test_mathtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-23 15:20:44.000000 qsonic-0.6.2/tests/test_mpi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-05-23 15:20:44.000000 qsonic-0.6.2/tests/test_picca_continuum.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 15:20:44.000000 qsonic-0.6.2/tests/test_qsonic_calib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-23 15:20:44.000000 qsonic-0.6.2/tests/test_spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:03:31.121441 qsonic-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-18 01:03:12.000000 qsonic-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-18 01:03:31.121441 qsonic-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-18 01:03:12.000000 qsonic-0.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:03:31.117441 qsonic-0.7.1/py/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:03:31.121441 qsonic-0.7.1/py/qsonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18264 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/mathtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/mpi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52012 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/picca_continuum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:03:31.121441 qsonic-0.7.1/py/qsonic/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/scripts/qsonic_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/scripts/qsonic_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30001 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:03:31.121441 qsonic-0.7.1/py/qsonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-18 01:03:31.000000 qsonic-0.7.1/py/qsonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-18 01:03:31.000000 qsonic-0.7.1/py/qsonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:03:31.000000 qsonic-0.7.1/py/qsonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-18 01:03:31.000000 qsonic-0.7.1/py/qsonic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-18 01:03:31.000000 qsonic-0.7.1/py/qsonic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-18 01:03:31.000000 qsonic-0.7.1/py/qsonic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-18 01:03:12.000000 qsonic-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-18 01:03:12.000000 qsonic-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-18 01:03:31.121441 qsonic-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 01:03:12.000000 qsonic-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:03:31.121441 qsonic-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-18 01:03:12.000000 qsonic-0.7.1/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-18 01:03:12.000000 qsonic-0.7.1/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-18 01:03:12.000000 qsonic-0.7.1/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-18 01:03:12.000000 qsonic-0.7.1/tests/test_mathtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-18 01:03:12.000000 qsonic-0.7.1/tests/test_mpi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-06-18 01:03:12.000000 qsonic-0.7.1/tests/test_picca_continuum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-18 01:03:12.000000 qsonic-0.7.1/tests/test_qsonic_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-18 01:03:12.000000 qsonic-0.7.1/tests/test_spectrum.py
```

### Comparing `qsonic-0.6.2/LICENSE` & `qsonic-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.2/PKG-INFO` & `qsonic-0.7.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsonic
-Version: 0.6.2
+Version: 0.7.1
 Summary: Quasar continuum fitter for DESI
 Author: Naim Goksel Karacayli
 Author-email: ngokselk@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/p-slash/qsonic/issues
 Project-URL: Documentation, http://qsonic.readthedocs.io/
 Project-URL: Source, https://github.com/p-slash/qsonic
@@ -33,17 +33,17 @@
 
 **QSOnic** is an MPI-parallelized, highly optimized quasar continuum fitting package for DESI built on the same algorithm as `picca <https://github.com/igmhub/picca>`_, but *faster*. It also provides an efficient API to read DESI quasar spectra.
 
 The key differences
 -------------------
 - Coadding of spectrograph arms is optional and performed after continuum fitting.
 - Continuum is multiplied by a fiducial mean flux when provided.
-- You can pass fiducial var_lss (column ``VAR``) and mean flux (column ``MEANFLUX``) for observed wavelength ``LAMBDA`` in ``STATS`` extention of a FITS file. Wavelength should be linearly and equally spaced. This is the same format as rawio output from picca.
+- You can pass fiducial var_lss (column **VAR_LSS**) and mean flux (column **MEANFLUX**) for observed wavelength **LAMBDA** in **STATS** extention of a FITS file. Wavelength should be linearly and equally spaced. This is the same format as rawio output from picca, except **VAR** column in picca is the variance on flux not deltas. We break away from that convention by explicitly requiring variance on deltas in a new column.
 - If no fiducial is passed, we fit only for var_lss (no eta fitting by default). Eta fitting can be enabled, but is not recommended for Lya forest.
 - Internal weights for continuum fitting and coadding are based on smoothed ``IVAR``, and output ``WEIGHT`` is based on this smoothed ivar. This smoothing can be turned off.
 - Chi2 information as well as best fits are saved in continuum_chi2_catalog.fits. Chi2 is calculated using smooth ivar and var_lss, and does not subtract sum of ln(weights).
 
 Similarities
 ------------
-+ Delta files are the same. `CONT` column is mean flux times continuum even when fiducial mean flux is passed.
++ Delta files are the same. ``CONT`` column is mean flux times continuum even when fiducial mean flux is passed.
 + ``MEANSNR`` in header file and chi2 catalog is average of flux times square root of positive ivar values. Header values are per arm, but catalog values are the average over all arms.
 + Eta fitting does not rescale ``IVAR`` output. Pipeline noise will be modified with explicit calibration option.
```

### Comparing `qsonic-0.6.2/README.rst` & `qsonic-0.7.1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 
 **QSOnic** is an MPI-parallelized, highly optimized quasar continuum fitting package for DESI built on the same algorithm as `picca <https://github.com/igmhub/picca>`_, but *faster*. It also provides an efficient API to read DESI quasar spectra.
 
 The key differences
 -------------------
 - Coadding of spectrograph arms is optional and performed after continuum fitting.
 - Continuum is multiplied by a fiducial mean flux when provided.
-- You can pass fiducial var_lss (column ``VAR``) and mean flux (column ``MEANFLUX``) for observed wavelength ``LAMBDA`` in ``STATS`` extention of a FITS file. Wavelength should be linearly and equally spaced. This is the same format as rawio output from picca.
+- You can pass fiducial var_lss (column **VAR_LSS**) and mean flux (column **MEANFLUX**) for observed wavelength **LAMBDA** in **STATS** extention of a FITS file. Wavelength should be linearly and equally spaced. This is the same format as rawio output from picca, except **VAR** column in picca is the variance on flux not deltas. We break away from that convention by explicitly requiring variance on deltas in a new column.
 - If no fiducial is passed, we fit only for var_lss (no eta fitting by default). Eta fitting can be enabled, but is not recommended for Lya forest.
 - Internal weights for continuum fitting and coadding are based on smoothed ``IVAR``, and output ``WEIGHT`` is based on this smoothed ivar. This smoothing can be turned off.
 - Chi2 information as well as best fits are saved in continuum_chi2_catalog.fits. Chi2 is calculated using smooth ivar and var_lss, and does not subtract sum of ln(weights).
 
 Similarities
 ------------
-+ Delta files are the same. `CONT` column is mean flux times continuum even when fiducial mean flux is passed.
++ Delta files are the same. ``CONT`` column is mean flux times continuum even when fiducial mean flux is passed.
 + ``MEANSNR`` in header file and chi2 catalog is average of flux times square root of positive ivar values. Header values are per arm, but catalog values are the average over all arms.
 + Eta fitting does not rescale ``IVAR`` output. Pipeline noise will be modified with explicit calibration option.
```

### Comparing `qsonic-0.6.2/py/qsonic/calibration.py` & `qsonic-0.7.1/py/qsonic/calibration.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.2/py/qsonic/catalog.py` & `qsonic-0.7.1/py/qsonic/catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from healpy import ang2pix
 import numpy as np
 from numpy.lib.recfunctions import rename_fields, append_fields
 
 from qsonic.mpi_utils import logging_mpi, balance_load, mpi_fnc_bcast
 
 _accepted_extnames = set(['QSO_CAT', 'ZCATALOG', 'METADATA'])
-"""set: Accepted extentions for quasar catalog."""
+"""set: Accepted extensions for quasar catalog."""
 _required_columns = [
     set(['TARGETID']), set(['Z']), set(['TARGET_RA', 'RA']),
     set(['TARGET_DEC', 'DEC'])
 ]
 """list(set): Required columns for all cases."""
 _required_data_columns = [
     set(['SURVEY']),
```

### Comparing `qsonic-0.6.2/py/qsonic/io.py` & `qsonic-0.7.1/py/qsonic/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,25 +49,26 @@
         help="Arms to read.")
 
     outgroup = parser.add_argument_group('Output options')
     outgroup.add_argument(
         "--outdir", '-o',
         help="Output directory to save deltas.")
     outgroup.add_argument(
-        "--coadd-arms", action="store_true",
-        help="Coadds arms when saving.")
+        "--coadd-arms", default="before",
+        choices=["before", "after", "disable"],
+        help="Coadds arms before or after continuum fitting or not at all.")
     outgroup.add_argument(
         "--save-by-hpx", action="store_true",
         help="Save by healpix. If not, saves by MPI rank.")
     return parser
 
 
 def read_spectra_onehealpix(
         catalog_hpx, input_dir, arms_to_keep, mock_analysis, skip_resomat,
-        program="dark"
+        read_true_continuum, program="dark"
 ):
     """ Returns a list of Spectrum objects for a given catalog of a single
     healpix.
 
     Arguments
     ---------
     catalog_hpx: :external+numpy:py:class:`ndarray <numpy.ndarray>`
@@ -77,14 +78,16 @@
         Input directory
     arms_to_keep: list(str)
         Must only contain B, R and Z
     mock_analysis: bool
         Reads for mock data if true.
     skip_resomat: bool
         If true, do not read resomat.
+    read_true_continuum: bool
+        If true, reads the true continuum for mock analysis.
     program: str, default: "dark"
         Always use dark program.
 
     Returns
     ---------
     spectra_list: list(Spectrum)
 
@@ -93,15 +96,16 @@
     RuntimeWarning
         If number of quasars in the healpix file does not match the catalog.
     """
     spectra_list = []
 
     if mock_analysis:
         data, idx_cat = read_onehealpix_file_mock(
-            catalog_hpx, input_dir, arms_to_keep, skip_resomat
+            catalog_hpx, input_dir, arms_to_keep, skip_resomat,
+            read_true_continuum
         )
 
         if idx_cat.size != catalog_hpx.size:
             catalog_hpx = catalog_hpx[idx_cat]
 
         spectra_list.extend(
             qsonic.spectrum.generate_spectra_list_from_data(
@@ -287,14 +291,62 @@
 # def _read_imagehdu_2(imhdu, quasar_indices):
 #     ndims = imhdu.get_info()['ndims']
 #     if ndims == 2:
 #         return np.vstack([imhdu[int(idx), :] for idx in quasar_indices])
 #     return np.vstack([imhdu[int(idx), :, :] for idx in quasar_indices])
 
 
+def _read_true_continuum(targetids, fspec):
+    """Read true continuum as dictionary from file.
+
+    Arguments
+    ---------
+    targetids: :external+numpy:py:class:`ndarray <numpy.ndarray>`
+        Target IDs.
+    fspec: str
+        Filename to open.
+
+    Returns
+    ---------
+    cont_data: dict( :external+numpy:py:class:`ndarray <numpy.ndarray>` )
+        This has keys for w1, w2, dwave and data, where data is ndarray and
+        others are floats.
+
+    Raises
+    ---------
+    RuntimeError
+        If number of quasars in TRUE_CONT does not match the input.
+    """
+    with fitsio.FITS(fspec) as fitsfile:
+        hdr = fitsfile['TRUE_CONT'].read_header()
+        true_continua = fitsfile['TRUE_CONT'].read()
+    w1 = hdr['WMIN']
+    w2 = hdr['WMAX']
+    dw = hdr['DWAVE']
+
+    common_targetids, idx_fbr, _ = np.intersect1d(
+        true_continua['TARGETID'], targetids,
+        assume_unique=True, return_indices=True
+    )
+
+    if (common_targetids.size != targetids.size):
+        raise RuntimeError(
+            f"Error reading true continua from {fspec}. "
+            "Number of quasars in TRUE_CONT does not match the catalog "
+            f"catalog:{targetids.size} vs "
+            f"healpix:{common_targetids.size}!")
+
+    cont_data = {
+        'w1': w1, 'w2': w2, 'dwave': dw,
+        'data': true_continua['TRUE_CONT'][idx_fbr, :].astype("f8")
+    }
+
+    return cont_data
+
+
 def _read_onehealpix_file(
         targetids_by_survey, fspec, arms_to_keep, skip_resomat
 ):
     """ Common function to read a single fits file.
 
     Arguments
     ---------
@@ -462,28 +514,33 @@
     data, idx_cat = _read_onehealpix_file(
         cat_by_survey['TARGETID'], fspec, arms_to_keep, skip_resomat)
 
     return data, idx_cat
 
 
 def read_onehealpix_file_mock(
-        catalog_hpx, input_dir, arms_to_keep, skip_resomat, nside=16
+        catalog_hpx, input_dir, arms_to_keep, skip_resomat,
+        read_true_continuum, nside=16
 ):
     """ Read a single FITS file for mocks.
 
     Arguments
     ---------
     catalog_hpx: :external+numpy:py:class:`ndarray <numpy.ndarray>`
         Catalog for a single healpix. Ordered by TARGETID.
     input_dir: str
         Input directory.
     arms_to_keep: list(str)
         Must only contain B, R and Z.
     skip_resomat: bool
         If true, do not read resomat.
+    read_true_continuum: bool
+        If true, reads the true continuum for mock analysis.
+    nside: int, default: 16
+        NSIDE for healpix.
 
     Returns
     ---------
     data: dict
         Only quasar spectra are read into keywords wave, flux etc. Resolution
         is read if present.
     idx_cat: :external+numpy:py:class:`ndarray <numpy.ndarray>`
@@ -495,22 +552,24 @@
         If number of quasars in the healpix file does not match the catalog.
     """
     pixnum = catalog_hpx['HPXPIXEL'][0]
     fspec = f"{input_dir}/{pixnum//100}/{pixnum}/spectra-{nside}-{pixnum}.fits"
     data, idx_cat = _read_onehealpix_file(
         catalog_hpx['TARGETID'], fspec, arms_to_keep, skip_resomat)
 
+    fspec = f"{input_dir}/{pixnum//100}/{pixnum}/truth-{nside}-{pixnum}.fits"
+    if read_true_continuum:
+        data['cont'] = _read_true_continuum(catalog_hpx['TARGETID'], fspec)
+
     if skip_resomat:
         return data, idx_cat
 
-    fspec = f"{input_dir}/{pixnum//100}/{pixnum}/truth-{nside}-{pixnum}.fits"
-    fitsfile = fitsio.FITS(fspec)
-    for arm in arms_to_keep:
-        data['reso'][arm] = np.array(fitsfile[f'{arm}_RESOLUTION'].read())
-    fitsfile.close()
+    with fitsio.FITS(fspec) as fitsfile:
+        for arm in arms_to_keep:
+            data['reso'][arm] = np.array(fitsfile[f'{arm}_RESOLUTION'].read())
 
     return data, idx_cat
 
 
 def _float_range(f1, f2):
     # Define the function with default arguments
     def float_range_checker(arg):
```

### Comparing `qsonic-0.6.2/py/qsonic/masks.py` & `qsonic-0.7.1/py/qsonic/masks.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.2/py/qsonic/mathtools.py` & `qsonic-0.7.1/py/qsonic/mathtools.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.2/py/qsonic/mpi_utils.py` & `qsonic-0.7.1/py/qsonic/mpi_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,33 +3,44 @@
 
 import fitsio
 import numpy as np
 
 from qsonic import QsonicException
 
 
-def mpi_parse(parser, comm, mpi_rank, options=None):
+def _logic_true(args):
+    return True
+
+
+def mpi_parse(
+        parser, comm, mpi_rank, options=None, args_logic_fnc=_logic_true
+):
     """ Parse arguments on the master node, then broadcast.
 
     Arguments
     ---------
     parser: argparse.ArgumentParser
         Parser to be used.
     comm: MPI.COMM_WORLD
         MPI comm object for bcast
     mpi_rank: int
         Rank of the MPI process.
     options: None or list, default: None
         Options to parse. None parses ``sys.argv``
+    args_logic_fnc: Callable[[args], bool], default: True
+        Logic function to check for args.
     """
     if mpi_rank == 0:
         try:
             args = parser.parse_args(options)
         except SystemExit:
             args = -1
+
+        if not args_logic_fnc(args):
+            args = -1
     else:
         args = -1
 
     args = comm.bcast(args)
     if args == -1:
         exit(0)
 
@@ -183,15 +194,15 @@
 
     def write(self, data, names=None, extname=None, header=None):
         """ Write to FITS file.
 
         Arguments
         ---------
         data: list(:external+numpy:py:class:`ndarray <numpy.ndarray>`)
-            Data to write to extention.
+            Data to write to extension.
         names: list(str)or None, default: None
             Column names for data.
         extname: str or None, default: None
             Extention name.
         header: dict or None, default: None
             Header dictionary to save.
         """
```

### Comparing `qsonic-0.6.2/py/qsonic/picca_continuum.py` & `qsonic-0.7.1/py/qsonic/picca_continuum.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,20 +37,20 @@
     if parser is None:
         parser = argparse.ArgumentParser(
             formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 
     cont_group = parser.add_argument_group('Continuum fitting options')
 
     cont_group.add_argument(
-        "--rfdwave", type=float, default=0.8,
-        help="Rest-frame wave steps. Complies with forest limits")
-    cont_group.add_argument(
-        "--no-iterations", type=int, default=10,
+        "--num-iterations", type=int, default=10,
         help="Number of iterations for continuum fitting.")
     cont_group.add_argument(
+        "--true-continuum", action="store_true",
+        help="True continuum analysis deltas if mock analysis")
+    cont_group.add_argument(
         "--fiducial-meanflux", help="Fiducial mean flux FITS file.")
     cont_group.add_argument(
         "--fiducial-varlss", help="Fiducial var_lss FITS file.")
     cont_group.add_argument(
         "--cont-order", type=int, default=1,
         help="Order of continuum fitting polynomial.")
     cont_group.add_argument(
@@ -59,14 +59,17 @@
     cont_group.add_argument(
         "--var-use-cov", action="store_true",
         help="Use covariance in varlss-eta fitting.")
     cont_group.add_argument(
         "--normalize-stacked-flux", action="store_true",
         help="NOT IMPLEMENTED: Force stacked flux to be one at the end.")
     cont_group.add_argument(
+        "--rfdwave", type=float, default=0.8,
+        help="Rest-frame wave steps. Complies with forest limits")
+    cont_group.add_argument(
         "--minimizer", default="iminuit", choices=["iminuit", "l_bfgs_b"],
         help="Minimizer to fit the continuum.")
 
     return parser
 
 
 class PiccaContinuumFitter():
@@ -111,46 +114,49 @@
     varlss_fitter: VarLSSFitter or None
         None if fiducials are set for var_lss.
     varlss_interp: FastLinear1DInterp or FastCubic1DInterp
         Cubic spline for var_lss if fitting. Linear if from file.
     eta_interp: FastCubic1DInterp
         Interpolator for eta. Returns one if fiducial var_lss is set.
     niterations: int
-        Number of iterations from `args.no_iterations`.
+        Number of iterations from ``args.num_iterations``.
     cont_order: int
-        Order of continuum polynomial from `args.cont_order`.
+        Order of continuum polynomial from ``args.cont_order``.
     outdir: str or None
         Directory to save catalogs. If None or empty, does not save.
     fit_eta: bool
         True if fitting eta and fiducial var_lss is not set.
     """
 
     def _get_fiducial_interp(self, fname, col2read):
         """ Return an interpolator for mean flux or var_lss.
 
-        FITS file must have a 'STATS' extention, which must have 'LAMBDA',
-        'MEANFLUX' and 'VAR' columns. This is the same format as raw_io output
-        from picca. 'LAMBDA' must be linearly and equally spaced.
-        This function sets up ``col2read`` as FastLinear1DInterp object.
+        FITS file must have a **STATS** extention, which must have **LAMBDA**,
+        **MEANFLUX** and **VAR_LSS** columns. This is the same format as rawio
+        output from picca, except **VAR** column in picca is the variance of
+        flux not deltas. We break away from that convention by explicitly
+        requiring variance on deltas in a new column. **LAMBDA** must be
+        linearly and equally spaced. This function sets up ``col2read`` as
+        FastLinear1DInterp object.
 
         Arguments
         ---------
         fname: str
             Filename of the FITS file.
         col2read: str
-            Should be 'MEANFLUX' or 'VAR'.
+            Should be **MEANFLUX** or **VAR_LSS**.
 
         Returns
         -------
         FastLinear1DInterp
 
         Raises
         ------
         QsonicException
-            If 'LAMBDA' is not equally spaced or ``col2read`` is not in the
+            If **LAMBDA** is not equally spaced or ``col2read`` is not in the
             file.
         """
         def _read(fname, col2read):
             with fitsio.FITS(fname) as fts:
                 data = fts['STATS'].read()
 
             waves = data['LAMBDA']
@@ -207,30 +213,30 @@
 
         self.flux_stacker = FluxStacker(
             args.wave1, args.wave2, 8., comm=self.comm)
 
         if args.fiducial_varlss:
             self.varlss_fitter = None
             self.varlss_interp = self._get_fiducial_interp(
-                args.fiducial_varlss, 'VAR')
+                args.fiducial_varlss, 'VAR_LSS')
         else:
             self.varlss_fitter = VarLSSFitter(
                 args.wave1, args.wave2, use_cov=args.var_use_cov,
                 comm=self.comm)
             self.varlss_interp = FastCubic1DInterp(
                 self.varlss_fitter.waveobs[0], self.varlss_fitter.dwobs,
                 0.1 * np.ones(self.varlss_fitter.nwbins),
                 ep=np.zeros(self.varlss_fitter.nwbins))
 
         self.eta_interp = FastCubic1DInterp(
             self.varlss_interp.xp0, self.varlss_interp.dxp,
             np.ones_like(self.varlss_interp.fp),
             ep=np.zeros_like(self.varlss_interp.fp))
 
-        self.niterations = args.no_iterations
+        self.niterations = args.num_iterations
         self.cont_order = args.cont_order
         self.outdir = args.outdir
         self.fit_eta = args.var_fit_eta
 
     def _continuum_costfn(self, x, wave, flux, ivar_sm, z_qso):
         """ Cost function to minimize for each quasar.
 
@@ -413,36 +419,36 @@
         Raises
         ------
         QsonicException
             If there are no valid fits.
         RuntimeWarning
             If more than 20% spectra have invalid fits.
         """
-        no_valid_fits = 0
-        no_invalid_fits = 0
+        num_valid_fits = 0
+        num_invalid_fits = 0
 
         # For each forest fit continuum
         for spec in spectra_list:
             self.fit_continuum(spec)
 
             if not spec.cont_params['valid']:
-                no_invalid_fits += 1
+                num_invalid_fits += 1
             else:
-                no_valid_fits += 1
+                num_valid_fits += 1
 
-        no_valid_fits = self.comm.allreduce(no_valid_fits)
-        no_invalid_fits = self.comm.allreduce(no_invalid_fits)
-        logging_mpi(f"Number of valid fits: {no_valid_fits}", self.mpi_rank)
-        logging_mpi(f"Number of invalid fits: {no_invalid_fits}",
+        num_valid_fits = self.comm.allreduce(num_valid_fits)
+        num_invalid_fits = self.comm.allreduce(num_invalid_fits)
+        logging_mpi(f"Number of valid fits: {num_valid_fits}", self.mpi_rank)
+        logging_mpi(f"Number of invalid fits: {num_invalid_fits}",
                     self.mpi_rank)
 
-        if no_valid_fits == 0:
+        if num_valid_fits == 0:
             raise QsonicException("Crucial error: No valid continuum fits!")
 
-        invalid_ratio = no_invalid_fits / (no_valid_fits + no_invalid_fits)
+        invalid_ratio = num_invalid_fits / (num_valid_fits + num_invalid_fits)
         if invalid_ratio > 0.2:
             warn_mpi("More than 20% spectra have invalid fits.", self.mpi_rank)
 
     def _project_normalize_meancont(self, new_meancont):
         """ Project out higher order Legendre polynomials from the new mean
         continuum since these are degenerate with the free fitting parameters.
         Returns a normalized mean continuum. Integrals are calculated using
@@ -635,40 +641,37 @@
         """Main function to fit continua and iterate.
 
         Consists of three major steps: initializing, fitting, updating global
         variables. The initialization sets ``cont_params`` variable of every
         Spectrum object. Continuum polynomial order is carried by setting
         ``cont_params[x]``. At each iteration:
 
-        1. Global variables (mean continuum, var_lss) are saved to file
-           (attributes.fits) file. This ensures the order of what is used in
+        1. Global variables (mean continuum, var_lss) are saved to
+           ``attributes.fits`` file. This ensures the order of what is used in
            each iteration.
         2. All spectra are fit.
         3. Mean continuum is updated by stacking, smoothing and removing
            degenarate modes. Check for convergence if update is small.
         4. If fitting for var_lss, fit and update by calculating variance
            statistics.
 
-        At the end of requested iterations or convergence, a chi2 catalog is
-        created that includes information regarding chi2, mean_snr, targetid,
-        etc.
-
         Arguments
         ---------
         spectra_list: list(Spectrum)
             Spectrum objects to fit.
         """
         has_converged = False
 
         for spec in spectra_list:
             spec.cont_params['method'] = 'picca'
             spec.cont_params['x'] = np.append(
                 spec.cont_params['x'][0], np.zeros(self.cont_order))
             spec.cont_params['xcov'] = np.eye(self.cont_order + 1)
-            spec.cont_params['dof'] = spec.get_real_size()
+            spec.cont_params['dof'] = \
+                spec.get_real_size() - self.cont_order - 1
 
         fname = f"{self.outdir}/attributes.fits" if self.outdir else ""
         fattr = MPISaver(fname, self.mpi_rank)
 
         for it in range(self.niterations):
             is_last_it = it == self.niterations - 1
             logging_mpi(
@@ -688,18 +691,67 @@
                 logging_mpi("Iteration has converged.", self.mpi_rank)
                 break
 
         if not has_converged:
             warn_mpi("Iteration has NOT converged.", self.mpi_rank)
 
         self.save(fattr)
-        self.varlss_fitter.write(fattr)
+        if self.varlss_fitter:
+            self.varlss_fitter.write(fattr)
         fattr.close()
         logging_mpi("All continua are fit.", self.mpi_rank)
 
+    def true_continuum(self, spectra_list):
+        """True continuum reduction. Uses fiducials for mean flux and varlss
+        interpolation. Continuum is interpolated using a cubic spline.
+
+        .. warning::
+
+            This function would work even if you did not pass any fiducial.
+
+        Arguments
+        ---------
+        spectra_list: list(Spectrum)
+            Spectrum objects.
+        """
+        self.cont_order = 0
+
+        for spec in spectra_list:
+            spec.cont_params['method'] = 'true'
+            spec.cont_params['valid'] = True
+            spec.cont_params['x'] = np.zeros(1)
+            spec.cont_params['xcov'] = np.eye(1)
+            spec.cont_params['dof'] = spec.get_real_size()
+            spec.cont_params['cont'] = {}
+
+            w1 = spec.cont_params['true_data_w1']
+            dwave = spec.cont_params['true_data_dwave']
+            tcont = spec.cont_params['true_data']
+
+            tcont_interp = FastCubic1DInterp(w1, dwave, tcont)
+
+            for arm, wave_arm in spec.forestwave.items():
+                cont_est = tcont_interp(wave_arm)
+                cont_est *= self.meanflux_interp(wave_arm)
+                spec.cont_params['cont'][arm] = cont_est
+
+            spec.set_forest_weight(self.varlss_interp)
+            spec.calc_continuum_chi2()
+
+        self.update_mean_cont(spectra_list, False)
+        self.update_var_lss_eta(spectra_list, False)
+        fname = f"{self.outdir}/attributes.fits" if self.outdir else ""
+        fattr = MPISaver(fname, self.mpi_rank)
+        self.save(fattr)
+        if self.varlss_fitter:
+            self.varlss_fitter.write(fattr)
+        fattr.close()
+
+        logging_mpi("True continuum applied.", self.mpi_rank)
+
     def save(self, fattr, suff=''):
         """Save mean continuum and var_lss (if fitting) to a fits file.
 
         Arguments
         ---------
         fattr: MPISaver
             File handler to save only on master node.
@@ -723,16 +775,17 @@
             [self.varlss_fitter.waveobs,
              self.varlss_interp.fp, self.varlss_interp.ep,
              self.eta_interp.fp, self.eta_interp.ep],
             names=['lambda', 'var_lss', 'e_var_lss', 'eta', 'e_eta'],
             extname=f'VAR_FUNC{suff}')
 
     def save_contchi2_catalog(self, spectra_list):
-        """Save chi2 catalog if ``self.outdir`` is set. All values are gathered
-        and saved on the master node.
+        """Save the chi2 catalog that includes information regarding chi2,
+        mean_snr, targetid, etc. if ``self.outdir`` is set. All values are
+        gathered to and saved on the master node.
 
         Arguments
         ---------
         spectra_list: list(Spectrum)
             Spectrum objects to fit.
         """
         if not self.outdir:
@@ -811,16 +864,16 @@
 
         ...
         varfitter = VarLSSFitter(
             wave1, wave2, nwbins,
             var1, var2, nvarbins,
             nsubsamples=100, comm=comm)
         # Change static minimum numbers for valid statistics
-        VarLSSFitter.min_no_pix = min_no_pix
-        VarLSSFitter.min_no_qso = min_no_qso
+        VarLSSFitter.min_num_pix = min_num_pix
+        VarLSSFitter.min_num_qso = min_num_qso
 
         for delta in deltas_list:
             varfitter.add(delta.wave, delta.delta, delta.ivar)
 
         logging_mpi("Fitting variance for VarLSS and eta", mpi_rank)
         fit_results = np.ones((nwbins, 2))
         fit_results[:, 0] = 0.1
@@ -868,17 +921,17 @@
         Subsampler object that stores mean_delta in axis=0, var_delta in axis=1
         , var2_delta in axis=2, mean bin variance in axis=3.
     comm: MPI.COMM_WORLD or None, default: None
         MPI comm object to allreduce if enabled.
     mpi_rank: int
         Rank of the MPI process if ``comm!=None``. Zero otherwise.
     """
-    min_no_pix = 500
+    min_num_pix = 500
     """int: Minimum number of pixels a bin must have to be valid."""
-    min_no_qso = 50
+    min_num_qso = 50
     """int: Minimum number of quasars a bin must have to be valid."""
 
     @staticmethod
     def variance_function(var_pipe, var_lss, eta=1):
         """Variance model to be fit.
 
         .. math::
@@ -1109,16 +1162,16 @@
         self._allreduce()
         self._calc_subsampler_stats()
 
         nfails = 0
         fit_results = np.zeros_like(initial_guess)
         std_results = np.zeros_like(initial_guess)
 
-        w_gtr_min = ((self.num_pixels > VarLSSFitter.min_no_pix)
-                     & (self.num_qso > VarLSSFitter.min_no_qso))
+        w_gtr_min = ((self.num_pixels > VarLSSFitter.min_num_pix)
+                     & (self.num_qso > VarLSSFitter.min_num_qso))
 
         if self.use_cov:
             err_base = self.cov_var_delta
         else:
             err_base = self.e_var_delta
 
         for iwave in range(self.nwbins):
@@ -1175,28 +1228,28 @@
         # Smooth new estimates
         if smooth:
             fit_results = self._smooth_fit_results(fit_results, std_results)
 
         return fit_results, std_results
 
     def write(self, mpi_saver, min_snr=0, max_snr=100):
-        """ Write variance statistics to FITS file in 'VAR_STATS' extention.
+        """ Write variance statistics to FITS file in 'VAR_STATS' extension.
 
         Arguments
         ---------
         mpi_saver: MPISaver
             MPI FITS file handler.
         min_snr: float, default: 0
             Minimum SNR in this sample to be written into header.
         max_snr: float, default: 100
             Maximum SNR in this sample to be written into header.
         """
         hdr_dict = {
-            'MINNPIX': VarLSSFitter.min_no_pix,
-            'MINNQSO': VarLSSFitter.min_no_qso,
+            'MINNPIX': VarLSSFitter.min_num_pix,
+            'MINNQSO': VarLSSFitter.min_num_qso,
             'MINSNR': min_snr,
             'MAXSNR': max_snr,
             'WAVE1': self.waveobs[0],
             'WAVE2': self.waveobs[-1],
             'NWBINS': self.nwbins,
             'IVAR1': self.ivar_edges[0],
             'IVAR2': self.ivar_edges[-1],
```

### Comparing `qsonic-0.6.2/py/qsonic/scripts/qsonic_calib.py` & `qsonic-0.7.1/py/qsonic/scripts/qsonic_calib.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 
     return deltas_list
 
 
 def mpi_stack_fluxes(args, comm, deltas_list):
     dwave = deltas_list[0].header['DELTA_LAMBDA']
     nwaveobs = int((args.wave2 - args.wave1) / dwave) + 1
-    waveobs = np.arange(nwaveobs) * dwave + args.wave1
+    waveobs = np.linspace(args.wave1, args.wave2, nwaveobs)
     stacked_flux = np.zeros(nwaveobs)
     weights = np.zeros(nwaveobs)
 
     for delta in deltas_list:
         flux = 1 + delta.delta
         idx = np.round((delta.wave - args.wave1) / dwave).astype(int)
         w = (idx >= 0) & (idx < nwaveobs)
```

### Comparing `qsonic-0.6.2/py/qsonic/scripts/qsonic_fit.py` & `qsonic-0.7.1/py/qsonic/scripts/qsonic_fit.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,27 +40,55 @@
     analysis_group.add_argument(
         "--smoothing-scale", default=16., type=float,
         help="Smoothing scale for pipeline noise in A.")
     analysis_group.add_argument(
         "--min-rsnr", type=float, default=0.,
         help="Minium SNR <F/sigma> above Lya.")
     analysis_group.add_argument(
-        "--skip", type=qsonic.io._float_range(0, 1), default=0.,
+        "--skip", type=qsonic.io._float_range(0, 1), default=0.2,
         help="Skip short spectra lower than given ratio.")
-    analysis_group.add_argument(
-        "--keep-nonforest-pixels", action="store_true",
-        help="Keeps non forest wavelengths. Memory intensive!")
 
     parser = qsonic.spectrum.add_wave_region_parser(parser)
     parser = qsonic.masks.add_mask_parser(parser)
     parser = add_picca_continuum_parser(parser)
 
     return parser
 
 
+def args_logic_fnc_qsonic_fit(args):
+    args_pass = True
+
+    args.arms = list(set(args.arms))
+
+    if args.true_continuum:
+        if not args.mock_analysis:
+            logging.error(
+                "True continuum is only applicable to mock analysis.")
+            args_pass = False
+
+        if not args.fiducial_meanflux:
+            logging.error(
+                "True continuum analysis requires fiducial mean flux.")
+            args_pass = False
+
+        if not args.fiducial_varlss:
+            logging.error("True continuum analysis requires fiducial var_lss.")
+            args_pass = False
+
+    if args.wave2 <= args.wave1:
+        logging.error("wave2 must be greater than wave1.")
+        args_pass = False
+
+    if args.forest_w2 <= args.forest_w1:
+        logging.error("forest_w2 must be greater than forest_w1.")
+        args_pass = False
+
+    return args_pass
+
+
 def mpi_read_spectra_local_queue(local_queue, args, comm, mpi_rank):
     """ Read local spectra for the MPI rank. Set forest and observed wavelength
     range.
 
     Arguments
     ---------
     local_queue: list(:external+numpy:py:class:`ndarray <numpy.ndarray>`)
@@ -84,22 +112,22 @@
     # skip_resomat = args.skip_resomat or not args.mock_analysis
     skip_resomat = args.skip_resomat
 
     spectra_list = []
     # Each process reads its own list
     for cat in local_queue:
         local_specs = qsonic.io.read_spectra_onehealpix(
-            cat, args.input_dir, args.arms, args.mock_analysis, skip_resomat)
+            cat, args.input_dir, args.arms, args.mock_analysis, skip_resomat,
+            args.true_continuum)
 
         for spec in local_specs:
             spec.set_forest_region(
                 args.wave1, args.wave2, args.forest_w1, args.forest_w2)
 
-            if not args.keep_nonforest_pixels:
-                spec.remove_nonforest_pixels()
+            spec.remove_nonforest_pixels()
 
         spectra_list.extend(
             [spec for spec in local_specs if spec.rsnr > args.min_rsnr])
 
         # if args.skip_resomat:
         #     continue
 
@@ -108,14 +136,19 @@
         # nspec = w.sum()
 
         # # Read resolution matrix hopefully faster
         # spectra_list[-nspec:] = \
         #     qsonic.io.read_resolution_matrices_onehealpix_data(
         #         cat[w], args.input_dir, spectra_list[-nspec:])
 
+    if args.coadd_arms == "before":
+        logging_mpi("Coadding arms.", mpi_rank)
+        for spec in spectra_list:
+            spec.coadd_arms_forest()
+
     nspec_all = comm.reduce(len(spectra_list))
     etime = (time.time() - start_time) / 60  # min
     logging_mpi(
         f"All {nspec_all} spectra are read in {etime:.1f} mins.", mpi_rank)
 
     return spectra_list
 
@@ -228,16 +261,57 @@
     dforest_wave = lya2 - lya1
     spectra_list = [spec for spec in spectra_list
                     if spec.is_long(dforest_wave, skip_ratio)]
 
     return spectra_list
 
 
+def mpi_continuum_fitting(spectra_list, args, comm, mpi_rank):
+    # Initialize continuum fitter & global functions
+    logging_mpi("Initializing continuum fitter.", mpi_rank)
+    start_time = time.time()
+    qcfit = PiccaContinuumFitter(args)
+
+    if not args.true_continuum:
+        # Fit continua
+        # Stack all spectra in each process
+        # Broadcast and recalculate global functions
+        # Iterate
+        logging_mpi("Fitting continuum.", mpi_rank)
+        qcfit.iterate(spectra_list)
+    else:
+        logging_mpi("True continuum.", mpi_rank)
+        qcfit.true_continuum(spectra_list)
+
+    if args.coadd_arms == "after":
+        logging_mpi("Coadding arms.", mpi_rank)
+        for spec in qsonic.spectrum.valid_spectra(spectra_list):
+            spec.coadd_arms_forest(qcfit.varlss_interp, qcfit.eta_interp)
+            spec.calc_continuum_chi2()
+
+    qcfit.save_contchi2_catalog(spectra_list)
+
+    # Keep only valid spectra
+    spectra_list = list(qsonic.spectrum.valid_spectra(spectra_list))
+
+    # Final cleaning. Especially important if not coadding arms.
+    for spec in spectra_list:
+        spec.drop_short_arms(args.forest_w1, args.forest_w2, args.skip)
+
+    etime = (time.time() - start_time) / 60  # min
+    logging_mpi(f"Continuum fitting and tweaking took {etime:.1f} mins.",
+                mpi_rank)
+
+    return spectra_list
+
+
 def mpi_run_all(comm, mpi_rank, mpi_size):
-    args = mpi_parse(get_parser(), comm, mpi_rank)
+    args = mpi_parse(get_parser(), comm, mpi_rank,
+                     args_logic_fnc=args_logic_fnc_qsonic_fit)
+
     if mpi_rank == 0 and args.outdir:
         os_makedirs(args.outdir, exist_ok=True)
 
     tol = (args.forest_w2 - args.forest_w1) * args.skip
     zmin_qso = args.wave1 / (args.forest_w2 - tol) - 1
     zmax_qso = args.wave2 / (args.forest_w1 + tol) - 1
 
@@ -266,47 +340,18 @@
     # remove from sample if no pixels is small
     spectra_list = remove_short_spectra(
         spectra_list, args.forest_w1, args.forest_w2, args.skip, mpi_rank)
 
     # Create smoothed ivar as intermediate variable
     if args.smoothing_scale > 0:
         for spec in spectra_list:
-            spec.set_smooth_ivar(args.smoothing_scale)
+            spec.set_smooth_forestivar(args.smoothing_scale)
 
     # Continuum fitting
-    # -------------------
-    # Initialize continuum fitter & global functions
-    logging_mpi("Initializing continuum fitter.", mpi_rank)
-    start_time = time.time()
-    qcfit = PiccaContinuumFitter(args)
-    logging_mpi("Fitting continuum.", mpi_rank)
-
-    # Fit continua
-    # Stack all spectra in each process
-    # Broadcast and recalculate global functions
-    # Iterate
-    qcfit.iterate(spectra_list)
-
-    if args.coadd_arms:
-        logging_mpi("Coadding arms.", mpi_rank)
-        for spec in qsonic.spectrum.valid_spectra(spectra_list):
-            spec.coadd_arms_forest(qcfit.varlss_interp, qcfit.eta_interp)
-
-    qcfit.save_contchi2_catalog(spectra_list)
-
-    # Keep only valid spectra
-    spectra_list = list(qsonic.spectrum.valid_spectra(spectra_list))
-
-    # Final cleaning. Especially important if not coadding arms.
-    for spec in spectra_list:
-        spec.drop_short_arms(args.forest_w1, args.forest_w2, args.skip)
-
-    etime = (time.time() - start_time) / 60  # min
-    logging_mpi(f"Continuum fitting and tweaking took {etime:.1f} mins.",
-                mpi_rank)
+    spectra_list = mpi_continuum_fitting(spectra_list, args, comm, mpi_rank)
 
     # Save deltas
     logging_mpi("Saving deltas.", mpi_rank)
     qsonic.io.save_deltas(
         spectra_list, args.outdir,
         save_by_hpx=args.save_by_hpx, mpi_rank=mpi_rank)
```

### Comparing `qsonic-0.6.2/py/qsonic/spectrum.py` & `qsonic-0.7.1/py/qsonic/spectrum.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,32 +27,27 @@
     wave_group.add_argument(
         "--wave1", type=float, default=3600.,
         help="First observed wavelength edge.")
     wave_group.add_argument(
         "--wave2", type=float, default=6000.,
         help="Last observed wavelength edge.")
     wave_group.add_argument(
-        "--forest-w1", type=float, default=1040.,
+        "--forest-w1", type=float, default=1050.,
         help="First forest wavelength edge.")
     wave_group.add_argument(
-        "--forest-w2", type=float, default=1200.,
+        "--forest-w2", type=float, default=1180.,
         help="Last forest wavelength edge.")
 
     return parser
 
 
 def generate_spectra_list_from_data(cat_by_survey, data):
     spectra_list = []
     for idx, catrow in enumerate(cat_by_survey):
-        spectra_list.append(
-            Spectrum(
-                catrow, data['wave'], data['flux'],
-                data['ivar'], data['mask'], data['reso'], idx
-            )
-        )
+        spectra_list.append(Spectrum.from_dictionary(catrow, data, idx))
 
     return spectra_list
 
 
 def valid_spectra(spectra_list):
     """Generator for continuum valid spectra."""
     return (spec for spec in spectra_list if spec.cont_params['valid'])
@@ -78,28 +73,31 @@
     idx: int
         Index to access in flux, ivar, mask and reso that corresponds to the
         quasar in `catrow`.
 
     Attributes
     ----------
     rsnr: float
-        Average SNR above Lya. Calculated in set_forest_region.
+        Average SNR above Lya. Calculated in :meth:`set_forest_region`.
     mean_snr: dict(float)
         Mean signal-to-noise ratio in the forest.
     _f1, _f2: dict(int)
-        Forest indices. Set up using `set_forest_region` method. Then use
+        Forest indices. Set up using :meth:`set_forest_region` method. Then use
         property functions to access forest wave, flux, ivar instead.
     cont_params: dict
         Continuum parameters. Initial estimates are constructed.
     """
     WAVE_LYA_A = 1215.67
     """float: Lya wavelength in A."""
     _wave = None
     """dict(:external+numpy:py:class:`ndarray <numpy.ndarray>`): Common
     wavelength grid for **all** Spectra."""
+    _coadd_wave = None
+    """dict(:external+numpy:py:class:`ndarray <numpy.ndarray>`): Common
+    **coadded** wavelength grid for **all** Spectra."""
     _dwave = None
     """float: Wavelength spacing."""
     _blinding = None
     """str or None: Blinding. Must be set for certain data."""
     _fits_colnames = ['LAMBDA', 'DELTA', 'IVAR', 'WEIGHT', 'CONT']
     """list(str): Column names to save in delta files."""
 
@@ -119,14 +117,26 @@
             Spectrum._dwave = wave_arm[1] - wave_arm[0]
         elif check_consistency:
             for arm, wave_arm in Spectrum._wave.items():
                 assert (arm in wave.keys())
                 assert (np.allclose(Spectrum._wave[arm], wave_arm))
 
     @staticmethod
+    def _set_coadd_wave():
+        if Spectrum._coadd_wave:
+            return
+
+        min_wave = np.min([wave[0] for wave in Spectrum._wave.values()])
+        max_wave = np.max([wave[-1] for wave in Spectrum._wave.values()])
+
+        nwaves = int((max_wave - min_wave) / Spectrum._dwave + 0.1) + 1
+        coadd_wave = np.linspace(min_wave, max_wave, nwaves)
+        Spectrum._coadd_wave = {'brz': coadd_wave}
+
+    @staticmethod
     def set_blinding(catalog, args):
         """Set the blinding strategy.
 
         'LASNIGHT' column, args.mock_analysis, args.forest_w1 decide the
         blinding strategy. Mock, side band and SV analyses are not blinded.
 
         Arguments
@@ -156,18 +166,45 @@
             Spectrum._fits_colnames.append('RESOMAT')
 
     @staticmethod
     def blinding_not_set():
         """bool: ``True`` if blinding is not set."""
         return Spectrum._blinding is None
 
+    @classmethod
+    def from_dictionary(cls, catrow, data, idx):
+        """Create a Spectrum from dictionary. See :class:`Spectrum` for
+        argument details.
+
+        If ``cont`` key is present in ``data``, :attr:`cont_params` dictionary
+        gains the following::
+
+            cont_params['true_data_w1'] (float): First wavelength
+            cont_params['true_data_dwave'] (float): Wavelength spacing
+            cont_params['true_data'] (ndarray): True continuum
+
+        Returns
+        -------
+        Spectrum
+        """
+        spec = cls(catrow, data['wave'], data['flux'], data['ivar'],
+                   data['mask'], data['reso'], idx)
+
+        if "cont" in data.keys():
+            spec.cont_params['true_data_w1'] = data['cont']['w1']
+            spec.cont_params['true_data_dwave'] = data['cont']['dwave']
+            spec.cont_params['true_data'] = data['cont']['data'][idx]
+
+        return spec
+
     def __init__(self, catrow, wave, flux, ivar, mask, reso, idx):
         self.catrow = catrow
         Spectrum._set_wave(wave)
 
+        self._current_wave = Spectrum._wave
         self.flux = {}
         self.ivar = {}
         self.reso = {}
 
         self.rsnr = None
         self.mean_snr = None
         self._f1 = {}
@@ -178,24 +215,23 @@
         self._forestivar_sm = {}
         self._forestreso = {}
         self._forestweight = {}
 
         self._smoothing_scale = 0
 
         for arm, wave_arm in self.wave.items():
-            self._f1[arm], self._f2[arm] = 0, wave_arm.size
             self.flux[arm] = flux[arm][idx]
             self.ivar[arm] = ivar[arm][idx]
             w = (mask[arm][idx] != 0) | np.isnan(self.flux[arm])\
                 | np.isnan(self.ivar[arm])
             self.flux[arm][w] = 0
             self.ivar[arm][w] = 0
 
             if not reso:
-                pass
+                continue
             elif reso[arm].ndim == 2:
                 self.reso[arm] = reso[arm].copy()
             else:
                 self.reso[arm] = reso[arm][idx]
 
         self.cont_params = {}
         self.cont_params['method'] = ''
@@ -304,91 +340,111 @@
             self._forestivar_sm.pop(arm, None)
             self._forestweight.pop(arm, None)
             self.cont_params['cont'].pop(arm, None)
 
     def remove_nonforest_pixels(self):
         """ Remove non-forest pixels from storage.
 
-        This equates `flux` to `forestflux` etc, but `wave` is not modified,
+        This sets :attr:`flux`, :attr:`ivar` and :attr:`reso` to empty
+        dictionary, but :attr:`wave` is not modified,
         since it is a static variable. Good practive is to loop using, e.g.,
-        `for arm, wave_arm in self.forestwave.items():`.
+        ``for arm, wave_arm in self.forestwave.items():``.
         """
-        self.flux = self.forestflux
-        self.ivar = self.forestivar
-        self.reso = self.forestreso
-
-        # Is this needed?
-        self._forestflux = self.flux
-        self._forestivar = self.ivar
-        self._forestreso = self.reso
+        self._current_wave = {}
+        self.flux = {}
+        self.ivar = {}
+        self.reso = {}
 
     def get_real_size(self):
-        """int: Sum of number of pixels with `forestivar > 0` for all arms."""
+        """
+        Returns
+        -------
+        int: Sum of number of pixels with ``forestivar > 0`` for all arms.
+        """
         size = 0
         for ivar_arm in self.forestivar.values():
             size += np.sum(ivar_arm > 0)
 
         return size
 
     def is_long(self, dforest_wave, skip_ratio):
+        """Determine if spectrum is long enough to be accepted.
+
+        The condition is :meth:`get_real_size` > ``skip_ratio * npixels``,
+        where ``npixels`` :math:`=(1 + z_\\mathrm{qso}) \\times` ``dforest_wave``
+        :math:`/ \\mathrm{d}\\lambda` and :math:`\\mathrm{d}\\lambda` is
+        wavelength spacing in the observed frame in A. 
+
+        Arguments
+        ---------
+        dforest_wave: float
+            Length of the forest in the rest-frame in A.
+        skip_ratio: float
+            Minimum ratio that needs to be present and unmasked to keep the
+            spectrum.
+
+        Returns
+        -------
+        bool
+        """
         npixels = (1 + self.z_qso) * dforest_wave / self.dwave
         return self.get_real_size() > skip_ratio * npixels
 
-    def set_smooth_ivar(self, smoothing_size=16.):
+    def set_smooth_forestivar(self, smoothing_size=16.):
         """ Set :attr:`forestivar_sm` to smoothed inverse variance. Before this
         call :attr:`forestivar_sm` points to :attr:`forestivar`. If
         ``smoothing_size <= 0``, smoothing is undone such that ivar_sm
-        points to ivar.
-
+        points to ivar. Also, :attr:`forestweight` points to this.
 
         ``smoothing_size`` is saved to a private :attr:`_smoothing_scale`
         variable for future use.
 
         Arguments
         ---------
         smoothing_size: float, default: 16
             Gaussian smoothing spread in A.
         """
-        self._forestivar_sm = {}
         if smoothing_size <= 0:
             self._smoothing_scale = 0
             self._forestivar_sm = self._forestivar
-            return
+        else:
+            self._smoothing_scale = smoothing_size
+            sigma_pix = smoothing_size / self.dwave
+            self._forestivar_sm = {
+                arm: get_smooth_ivar(ivar_arm, sigma_pix)
+                for arm, ivar_arm in self.forestivar.items()
+            }
 
-        self._smoothing_scale = smoothing_size
-        sigma_pix = smoothing_size / self.dwave
-        for arm, ivar_arm in self.forestivar.items():
-            self._forestivar_sm[arm] = get_smooth_ivar(ivar_arm, sigma_pix)
+        self._forestweight = self._forestivar_sm
 
     def set_forest_weight(
-            self,
-            varlss_interp=_zero_function,
-            eta_interp=_one_function
+            self, varlss_interp=_zero_function, eta_interp=_one_function
     ):
         """ Sets :attr:`forestweight` for a given var_lss and eta correction.
         Always uses :attr:`forestivar_sm`, which is not actually smoothed if
-        :meth:`set_smooth_ivar` is not called.
+        :meth:`set_smooth_forestivar` is not called.
 
         .. math::
 
             w = i / (\\eta + i \\sigma^2_\\mathrm{LSS} C^2),
 
         where i is IVAR and C is the continuum.
 
         Arguments
         ---------
         varlss_interp: Callable[[ndarray], ndarray], default: 0
             LSS variance interpolator.
         eta_interp: Callable[[ndarray], ndarray], default: 1
             eta interpolator.
         """
-        self._forestweight = {}
         if not self.cont_params['valid'] or not self.cont_params['cont']:
+            self._forestweight = self._forestivar_sm
             return
 
+        self._forestweight = {}
         for arm, wave_arm in self.forestwave.items():
             cont_est = self.cont_params['cont'][arm]
             var_lss = varlss_interp(wave_arm) * cont_est**2
             eta = eta_interp(wave_arm)
             ivar_arm = self.forestivar_sm[arm]
             self._forestweight[arm] = ivar_arm / (eta + ivar_arm * var_lss)
 
@@ -411,66 +467,104 @@
             flux = self.forestflux[arm]
             chi2 += np.dot(weight, (flux - cont_est)**2)
 
         self.cont_params['chi2'] = chi2
 
         return chi2
 
-    def _coadd_arms_reso(self, nwaves, idxes):
-        """Coadd resolution matrix"""
-        max_ndia = np.max([reso.shape[0] for reso in self.forestreso.values()])
-        coadd_reso = np.zeros((max_ndia, nwaves))
-        creso_norm = np.zeros(nwaves)
-
-        for arm, reso_arm in self.forestreso.items():
-            weight = self.forestweight[arm].copy()
-            weight[weight == 0] = 1e-8
-
-            reso_arm = self.forestreso[arm]
-            ddia = max_ndia - reso_arm.shape[0]
-            # Assumption ddia cannot be odd
-            ddia = ddia // 2
-            if ddia > 0:
-                reso_arm = np.pad(reso_arm, ((ddia, ddia), (0, 0)))
+    def simple_coadd(self):
+        """Coadding without continuum and var_lss terms on the full spectrum.
+        Weights, forests etc. will not be set. Replaces :attr:`wave`,
+        :attr:`flux`, :attr:`ivar` and :attr:`reso` attributes with
+        dictionaries that has a single arm ``brz`` as key to access the coadded
+        data.
+
+        We first set the static coadded wavelength grid if it is not set.
+        Then we add each arm using :attr:`ivar` (not smoothed). If :attr:`reso`
+        is set, we coadd the resolution matrix using the same inverse variance
+        weights. If these weights are zero for both arms, resolution matrix
+        coadding reverts to equal weights. Final private assignments are done
+        at the end to keep using arm by arm values of :attr:`ivar`.
+        """
+        Spectrum._set_coadd_wave()
 
-            coadd_reso[:, idxes[arm]] += weight * reso_arm
-            creso_norm[idxes[arm]] += weight
+        min_wave = Spectrum._coadd_wave['brz'][0]
+        nwaves = Spectrum._coadd_wave['brz'].size
 
-        coadd_reso /= creso_norm
-        self._forestreso = {'brz': coadd_reso}
+        coadd_flux = np.zeros(nwaves)
+        coadd_ivar = np.zeros(nwaves)
+        coadd_norm = np.zeros(nwaves)
+
+        idxes = {}
+        for arm, wave_arm in self.wave.items():
+            idx = ((wave_arm - min_wave) / self.dwave + 0.1).astype(int)
+            idxes[arm] = idx
+
+            weight = self.ivar[arm]
+
+            var = np.zeros_like(weight)
+            w = self.ivar[arm] > 0
+            var[w] = 1 / self.ivar[arm][w]
+
+            coadd_flux[idx] += weight * self.flux[arm]
+            coadd_ivar[idx] += weight**2 * var
+            coadd_norm[idx] += weight
+
+        w = coadd_norm > 0
+        coadd_flux[w] /= coadd_norm[w]
+        coadd_ivar[w] = coadd_norm[w]**2 / coadd_ivar[w]
+
+        if self.reso:
+            max_ndia = np.max([reso.shape[0] for reso in self.reso.values()])
+            coadd_reso = np.zeros((max_ndia, nwaves))
+            coadd_norm *= 0
+
+            for arm, reso_arm in self.reso.items():
+                weight = self.ivar[arm].copy()
+                weight[weight == 0] = 1e-8
+
+                ddia = max_ndia - reso_arm.shape[0]
+                # Assumption ddia cannot be odd
+                ddia = ddia // 2
+                if ddia > 0:
+                    reso_arm = np.pad(reso_arm, ((ddia, ddia), (0, 0)))
+
+                coadd_reso[:, idxes[arm]] += weight * reso_arm
+                coadd_norm[idxes[arm]] += weight
+
+            coadd_reso /= coadd_norm
+            self.reso = {'brz': coadd_reso}
+
+        self._current_wave = Spectrum._coadd_wave
+        self.flux = {'brz': coadd_flux}
+        self.ivar = {'brz': coadd_ivar}
 
     def coadd_arms_forest(
-            self,
-            varlss_interp=_zero_function,
-            eta_interp=_one_function
+            self, varlss_interp=_zero_function, eta_interp=_one_function
     ):
         """ Coadds different arms using :attr:`forestweight`. Interpolators are
         needed to reset :attr:`forestweight`.
 
         Replaces ``forest`` variables and ``cont_params['cont']`` with a
         dictionary that has a single arm ``brz`` as key to access coadded data.
 
         Arguments
         ---------
         varlss_interp: Callable[[ndarray], ndarray], default: 0
             LSS variance interpolator or function.
         eta_interp: Callable[[ndarray], ndarray], default: 1
             eta interpolator or function.
         """
-        if not self.cont_params['valid'] or not self.cont_params['cont']:
-            raise QsonicException("Continuum needed for coadding.")
-
         min_wave = np.min([wave[0] for wave in self.forestwave.values()])
         max_wave = np.max([wave[-1] for wave in self.forestwave.values()])
 
         nwaves = int((max_wave - min_wave) / self.dwave + 0.1) + 1
-        coadd_wave = np.arange(nwaves) * self.dwave + min_wave
+        coadd_wave = np.linspace(min_wave, max_wave, nwaves)
         coadd_flux = np.zeros(nwaves)
         coadd_ivar = np.zeros(nwaves)
-        coadd_cont = np.empty(nwaves)
         coadd_norm = np.zeros(nwaves)
 
         idxes = {}
         for arm, wave_arm in self.forestwave.items():
             idx = ((wave_arm - min_wave) / self.dwave + 0.1).astype(int)
             idxes[arm] = idx
 
@@ -480,39 +574,63 @@
             w = self.forestivar[arm] > 0
             var[w] = 1 / self.forestivar[arm][w]
 
             coadd_flux[idx] += weight * self.forestflux[arm]
             coadd_ivar[idx] += weight**2 * var
             coadd_norm[idx] += weight
 
-            # continuum needs not weighting
-            coadd_cont[idx] = self.cont_params['cont'][arm]
-
         w = coadd_norm > 0
         coadd_flux[w] /= coadd_norm[w]
         coadd_ivar[w] = coadd_norm[w]**2 / coadd_ivar[w]
 
         self._forestwave = {'brz': coadd_wave}
         self._forestflux = {'brz': coadd_flux}
         self._forestivar = {'brz': coadd_ivar}
-        self.cont_params['cont'] = {'brz': coadd_cont}
+
+        if self.cont_params['cont']:
+            coadd_cont = np.empty(nwaves)
+
+            for arm, idx in idxes.items():
+                # continuum needs not weighting
+                coadd_cont[idx] = self.cont_params['cont'][arm]
+
+            self.cont_params['cont'] = {'brz': coadd_cont}
+
         if self.forestreso:
-            self._coadd_arms_reso(nwaves, idxes)
+            max_ndia = np.max(
+                [reso.shape[0] for reso in self.forestreso.values()])
+            coadd_reso = np.zeros((max_ndia, nwaves))
+            coadd_norm *= 0
+
+            for arm, reso_arm in self.forestreso.items():
+                weight = self.forestweight[arm].copy()
+                weight[weight == 0] = 1e-8
+
+                ddia = max_ndia - reso_arm.shape[0]
+                # Assumption ddia cannot be odd
+                ddia = ddia // 2
+                if ddia > 0:
+                    reso_arm = np.pad(reso_arm, ((ddia, ddia), (0, 0)))
 
-        self.set_smooth_ivar(self._smoothing_scale)
-        self._forestweight = {}
+                coadd_reso[:, idxes[arm]] += weight * reso_arm
+                coadd_norm[idxes[arm]] += weight
+
+            coadd_reso /= coadd_norm
+            self._forestreso = {'brz': coadd_reso}
+
+        self.set_smooth_forestivar(self._smoothing_scale)
         self.set_forest_weight(varlss_interp, eta_interp)
 
         mean_snr = np.dot(
             np.sqrt(coadd_ivar), coadd_flux) / np.sum(coadd_ivar > 0)
         self.mean_snr = {'brz': mean_snr}
 
     def mean_resolution(self, arm, weight=None):
         """ Returns the weighted mean Gaussian sigma of the spectrograph
-        resolution.
+        resolution in the forest.
 
         Arguments
         ---------
         arm: str
             Arm.
         weight: None or ndarray, default: None
             Weights. If ``None``, :attr:`forestweight` is used.
@@ -544,15 +662,15 @@
         rms_in_pixel = np.abs(off_idx).dot(new_ratios) / np.sqrt(2.) / norm
         return rms_in_pixel * 3e5 * self.dwave / lambda_eff
 
     def write(self, fts_file):
         """Writes each arm to FITS file separately.
 
         Writes 'LAMBDA', 'DELTA', 'IVAR', 'WEIGHT', 'CONT' columns and
-        'RESOMAT' column if resolution matrix is present to extention name
+        'RESOMAT' column if resolution matrix is present to extension name
         ``targetid-arm``. FITS file must be initialized before.
         Each arm has its own `MEANSNR`.
 
         Arguments
         ---------
         fts_file: FITS file
             The file handler, not filename.
@@ -616,15 +734,15 @@
         """float: Declination"""
         return self.catrow['DEC']
 
     @property
     def wave(self):
         """dict(:external+numpy:py:class:`ndarray <numpy.ndarray>`): Original
         wavelength grid in A."""
-        return Spectrum._wave
+        return self._current_wave
 
     @property
     def dwave(self):
         """float: Wavelength step size in A."""
         return Spectrum._dwave
 
     @property
@@ -647,15 +765,15 @@
 
     @property
     def forestivar_sm(self):
         """dict(:external+numpy:py:class:`ndarray <numpy.ndarray>`): Forest
         smoothed inverse variance field.
 
         Initially equal to :attr:`.forestivar`. Smoothed if
-        :meth:`.set_smooth_ivar` is called."""
+        :meth:`.set_smooth_forestivar` is called."""
         return self._forestivar_sm
 
     @property
     def forestweight(self):
         """dict(:external+numpy:py:class:`ndarray <numpy.ndarray>`): Forest
         weight field. Initially equal to :attr:`.forestivar`."""
         return self._forestweight
```

### Comparing `qsonic-0.6.2/py/qsonic.egg-info/PKG-INFO` & `qsonic-0.7.1/py/qsonic.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsonic
-Version: 0.6.2
+Version: 0.7.1
 Summary: Quasar continuum fitter for DESI
 Author: Naim Goksel Karacayli
 Author-email: ngokselk@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/p-slash/qsonic/issues
 Project-URL: Documentation, http://qsonic.readthedocs.io/
 Project-URL: Source, https://github.com/p-slash/qsonic
@@ -33,17 +33,17 @@
 
 **QSOnic** is an MPI-parallelized, highly optimized quasar continuum fitting package for DESI built on the same algorithm as `picca <https://github.com/igmhub/picca>`_, but *faster*. It also provides an efficient API to read DESI quasar spectra.
 
 The key differences
 -------------------
 - Coadding of spectrograph arms is optional and performed after continuum fitting.
 - Continuum is multiplied by a fiducial mean flux when provided.
-- You can pass fiducial var_lss (column ``VAR``) and mean flux (column ``MEANFLUX``) for observed wavelength ``LAMBDA`` in ``STATS`` extention of a FITS file. Wavelength should be linearly and equally spaced. This is the same format as rawio output from picca.
+- You can pass fiducial var_lss (column **VAR_LSS**) and mean flux (column **MEANFLUX**) for observed wavelength **LAMBDA** in **STATS** extention of a FITS file. Wavelength should be linearly and equally spaced. This is the same format as rawio output from picca, except **VAR** column in picca is the variance on flux not deltas. We break away from that convention by explicitly requiring variance on deltas in a new column.
 - If no fiducial is passed, we fit only for var_lss (no eta fitting by default). Eta fitting can be enabled, but is not recommended for Lya forest.
 - Internal weights for continuum fitting and coadding are based on smoothed ``IVAR``, and output ``WEIGHT`` is based on this smoothed ivar. This smoothing can be turned off.
 - Chi2 information as well as best fits are saved in continuum_chi2_catalog.fits. Chi2 is calculated using smooth ivar and var_lss, and does not subtract sum of ln(weights).
 
 Similarities
 ------------
-+ Delta files are the same. `CONT` column is mean flux times continuum even when fiducial mean flux is passed.
++ Delta files are the same. ``CONT`` column is mean flux times continuum even when fiducial mean flux is passed.
 + ``MEANSNR`` in header file and chi2 catalog is average of flux times square root of positive ivar values. Header values are per arm, but catalog values are the average over all arms.
 + Eta fitting does not rescale ``IVAR`` output. Pipeline noise will be modified with explicit calibration option.
```

### Comparing `qsonic-0.6.2/py/qsonic.egg-info/SOURCES.txt` & `qsonic-0.7.1/py/qsonic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.2/setup.cfg` & `qsonic-0.7.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.6.2
+current_version = 0.7.1
 commit = True
 tag = True
 
 [bumpversion:file:py/qsonic/__init__.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
```

### Comparing `qsonic-0.6.2/tests/test_catalog.py` & `qsonic-0.7.1/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.2/tests/test_io.py` & `qsonic-0.7.1/tests/test_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         with pytest.raises(Exception, match=expected_msg):
             qsonic.io.save_deltas([], "outdir", None)
 
     def test_read_spectra_onehealpix(self, my_setup_fits):
         cat_by_survey, input_dir, xarms, data = my_setup_fits
 
         slist = qsonic.io.read_spectra_onehealpix(
-            cat_by_survey, input_dir, xarms, False, True)
+            cat_by_survey, input_dir, xarms, False, True, False)
 
         assert (len(slist) == cat_by_survey.size)
         for jj, spec in enumerate(slist):
             for arm in xarms:
                 npt.assert_allclose(spec.wave[arm], data['wave'][arm])
                 npt.assert_allclose(spec.flux[arm], data['flux'][arm][jj])
                 npt.assert_allclose(spec.ivar[arm], data['ivar'][arm][jj])
@@ -74,15 +74,15 @@
         # Test extra targetid in catalog
         ens_ = 3
         cat_by_survey2 = np.concatenate((cat_by_survey, cat_by_survey[-ens_:]))
         cat_by_survey2[-ens_:]['TARGETID'] += 20
         npt.assert_array_equal(cat_by_survey, cat_by_survey2[:-ens_])
         with pytest.warns(RuntimeWarning):
             slist = qsonic.io.read_spectra_onehealpix(
-                cat_by_survey2, input_dir, xarms, False, True)
+                cat_by_survey2, input_dir, xarms, False, True, False)
 
         assert (len(slist) == cat_by_survey.size)
         for jj, spec in enumerate(slist):
             for arm in xarms:
                 npt.assert_allclose(spec.wave[arm], data['wave'][arm])
                 npt.assert_allclose(spec.flux[arm], data['flux'][arm][jj])
                 npt.assert_allclose(spec.ivar[arm], data['ivar'][arm][jj])
```

### Comparing `qsonic-0.6.2/tests/test_masks.py` & `qsonic-0.7.1/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.2/tests/test_mathtools.py` & `qsonic-0.7.1/tests/test_mathtools.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.2/tests/test_mpi_utils.py` & `qsonic-0.7.1/tests/test_mpi_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 import pytest
 from unittest import TestCase
 
 import numpy as np
 import numpy.testing as npt
 
 from qsonic import QsonicException
-from qsonic.io import add_io_parser
 import qsonic.mpi_utils
-import qsonic.spectrum
 
 
 class TestMPIUtils(TestCase):
     @pytest.mark.mpi(min_size=2)
     def test_mpi_parse(self):
         from mpi4py import MPI
+        from qsonic.io import add_io_parser
         comm = MPI.COMM_WORLD
         assert comm.size > 0
 
         mpi_rank = comm.Get_rank()
         parser = argparse.ArgumentParser()
         add_io_parser(parser)
 
@@ -28,14 +27,35 @@
         assert (args.catalog == "incat")
         assert (args.outdir == "outdir")
 
         with pytest.raises(SystemExit):
             options = "--catalog incat -o outdir".split(' ')
             qsonic.mpi_utils.mpi_parse(parser, comm, mpi_rank, options)
 
+        # Test logic functions
+        from qsonic.scripts.qsonic_fit import (
+            get_parser, args_logic_fnc_qsonic_fit)
+
+        parser = get_parser()
+
+        options = ("--input-dir indir --catalog incat -o outdir "
+                   "--mock-analysis --true-continuum "
+                   "--fiducial-meanflux mflux "
+                   "--fiducial-varlss varlss").split(' ')
+        args = qsonic.mpi_utils.mpi_parse(parser, comm, mpi_rank, options,
+                                          args_logic_fnc_qsonic_fit)
+        assert args.true_continuum
+        assert args.mock_analysis
+
+        with pytest.raises(SystemExit):
+            options = ("--input-dir indir --catalog incat -o outdir "
+                       "--true-continuum").split(' ')
+            qsonic.mpi_utils.mpi_parse(parser, comm, mpi_rank, options,
+                                       args_logic_fnc_qsonic_fit)
+
     def test_mpi_fnc_bcast(self):
         matrix = np.arange(20).reshape(4, 5)
         u, s, vh = np.linalg.svd(matrix)
         result = qsonic.mpi_utils.mpi_fnc_bcast(
             np.linalg.svd, None, 0, "Error", matrix)
 
         npt.assert_allclose(result[0], u)
```

### Comparing `qsonic-0.6.2/tests/test_picca_continuum.py` & `qsonic-0.7.1/tests/test_picca_continuum.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 
 @pytest.fixture
 def get_fiducials(tmp_path):
     fname = tmp_path / "fiducials.fits"
     nsize = 100
     data = np.empty(
         nsize,
-        dtype=[('LAMBDA', 'f8'), ('MEANFLUX', 'f8'), ('VAR', 'f8')]
+        dtype=[('LAMBDA', 'f8'), ('MEANFLUX', 'f8'), ('VAR_LSS', 'f8')]
     )
     data['LAMBDA'] = np.linspace(3600, 6000, nsize)
     data['MEANFLUX'] = 2 * np.ones(nsize)
-    data['VAR'] = 3 * np.ones(nsize)
+    data['VAR_LSS'] = 3 * np.ones(nsize)
 
     with fitsio.FITS(fname, 'rw', clobber=True) as fts:
         fts.write(data, extname='STATS')
 
     return fname
```

### Comparing `qsonic-0.6.2/tests/test_qsonic_calib.py` & `qsonic-0.7.1/tests/test_qsonic_calib.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.6.2/tests/test_spectrum.py` & `qsonic-0.7.1/tests/test_spectrum.py`

 * *Files 10% similar despite different names*

```diff
@@ -136,15 +136,54 @@
         }
         spec.set_forest_weight(varlss_interp)
         spec.coadd_arms_forest(varlss_interp)
 
         assert ('brz' in spec.forestflux.keys())
         npt.assert_almost_equal(spec.forestflux['brz'], 2.1)
         npt.assert_almost_equal(spec.cont_params['cont']['brz'], 1.)
-        w = (spec.forestwave['brz'] < data['wave']['R'][0])\
-            | (spec.forestwave['brz'] > data['wave']['B'][-1])
-        npt.assert_almost_equal(spec.forestivar['brz'][w], 1)
-        npt.assert_almost_equal(spec.forestivar['brz'][~w], 2)
+
+        wbonly = int(
+            (data['wave']['R'][0] - spec.forestwave['brz'][0]) / spec.dwave
+            + 0.1)
+        npt.assert_almost_equal(spec.forestivar['brz'][:wbonly], 1)
+
+        wronly = int(
+            (data['wave']['B'][-1] - spec.forestwave['brz'][0]) / spec.dwave
+            + 0.1) + 1
+        npt.assert_almost_equal(spec.forestivar['brz'][wronly:], 1)
+
+        npt.assert_almost_equal(spec.forestivar['brz'][wbonly:wronly], 2)
+
+    def test_simple_coadd(self, setup_data):
+        cat_by_survey, _, data = setup_data(1)
+        spectra_list = qsonic.spectrum.generate_spectra_list_from_data(
+            cat_by_survey, data)
+
+        spec = spectra_list[0]
+        spec.simple_coadd()
+
+        assert (len(spec.wave.keys()) == 1)
+        assert ('brz' in spec.wave.keys())
+        assert ('brz' in spec.flux.keys())
+        npt.assert_equal(spec.wave['brz'].size, spec.flux['brz'].size)
+        npt.assert_equal(spec.wave['brz'].size, spec.ivar['brz'].size)
+        npt.assert_almost_equal(
+            spec.wave['brz'][[0, -1]],
+            [data['wave']['B'][0], data['wave']['R'][-1]])
+
+        npt.assert_almost_equal(spec.flux['brz'], 2.1)
+
+        wbonly = int(
+            (data['wave']['R'][0] - spec.wave['brz'][0]) / spec.dwave + 0.1
+        )
+        npt.assert_almost_equal(spec.ivar['brz'][:wbonly], 1)
+
+        wronly = int(
+            (data['wave']['B'][-1] - spec.wave['brz'][0]) / spec.dwave + 0.1
+        ) + 1
+        npt.assert_almost_equal(spec.ivar['brz'][wronly:], 1)
+
+        npt.assert_almost_equal(spec.ivar['brz'][wbonly:wronly], 2)
 
 
 if __name__ == '__main__':
     pytest.main()
```

