# Comparing `tmp/aug_sfutils-0.8.9.tar.gz` & `tmp/aug_sfutils-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aug_sfutils-0.8.9.tar", last modified: Wed Sep 20 08:27:51 2023, max compression
+gzip compressed data, was "aug_sfutils-0.9.1.tar", last modified: Fri Apr 26 08:26:50 2024, max compression
```

## Comparing `aug_sfutils-0.8.9.tar` & `aug_sfutils-0.9.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 git      (13229) t3tok     (2400)        0 2023-09-20 08:27:51.000000 aug_sfutils-0.8.9/
--rwxr-xr-x   0 git      (13229) t3tok     (2400)     1080 2023-09-11 11:10:50.000000 aug_sfutils-0.8.9/LICENSE
--rw-r--r--   0 git      (13229) t3tok     (2400)      549 2023-09-20 08:27:51.000000 aug_sfutils-0.8.9/PKG-INFO
--rwxr-xr-x   0 git      (13229) t3tok     (2400)       99 2023-09-11 11:10:50.000000 aug_sfutils-0.8.9/README.md
-drwxr-xr-x   0 git      (13229) t3tok     (2400)        0 2023-09-20 08:27:51.000000 aug_sfutils-0.8.9/aug_sfutils/
--rwxr-xr-x   0 git      (13229) t3tok     (2400)     1265 2023-09-20 08:22:54.000000 aug_sfutils-0.8.9/aug_sfutils/__init__.py
--rw-r--r--   0 git      (13229) t3tok     (2400)      125 2023-09-20 08:22:54.000000 aug_sfutils-0.8.9/aug_sfutils/config.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)     5386 2023-09-20 08:22:54.000000 aug_sfutils-0.8.9/aug_sfutils/contour.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)     1834 2023-09-20 08:22:54.000000 aug_sfutils-0.8.9/aug_sfutils/getlastshot.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)     8235 2023-09-20 08:22:54.000000 aug_sfutils-0.8.9/aug_sfutils/journal.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)     1586 2023-09-20 08:22:54.000000 aug_sfutils-0.8.9/aug_sfutils/libddc.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)     3892 2023-09-20 08:22:54.000000 aug_sfutils-0.8.9/aug_sfutils/manage_ed.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)    27752 2023-09-20 08:22:54.000000 aug_sfutils-0.8.9/aug_sfutils/mapeq.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)      242 2023-09-20 08:22:54.000000 aug_sfutils-0.8.9/aug_sfutils/parse_kwargs.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)    17819 2023-09-20 08:22:54.000000 aug_sfutils-0.8.9/aug_sfutils/sf2equ.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)     7063 2023-09-20 08:22:54.000000 aug_sfutils-0.8.9/aug_sfutils/sfh.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)     4034 2023-09-20 08:22:54.000000 aug_sfutils-0.8.9/aug_sfutils/sfhmod.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)     7191 2023-09-20 08:22:54.000000 aug_sfutils-0.8.9/aug_sfutils/sfmap.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)      720 2023-09-20 08:22:54.000000 aug_sfutils-0.8.9/aug_sfutils/sfobj.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)    14613 2023-09-20 08:22:54.000000 aug_sfutils-0.8.9/aug_sfutils/sfread.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)    27549 2023-09-20 08:22:54.000000 aug_sfutils-0.8.9/aug_sfutils/shotfile.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)      831 2023-09-20 08:22:54.000000 aug_sfutils-0.8.9/aug_sfutils/str_byt.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)     1329 2023-09-20 08:22:54.000000 aug_sfutils-0.8.9/aug_sfutils/time_no_elm.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)     6161 2023-09-20 08:22:54.000000 aug_sfutils-0.8.9/aug_sfutils/time_slice.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)    18708 2023-09-20 08:22:54.000000 aug_sfutils-0.8.9/aug_sfutils/ww.py
-drwxr-xr-x   0 git      (13229) t3tok     (2400)        0 2023-09-20 08:27:51.000000 aug_sfutils-0.8.9/aug_sfutils.egg-info/
--rw-r--r--   0 git      (13229) t3tok     (2400)      549 2023-09-20 08:27:50.000000 aug_sfutils-0.8.9/aug_sfutils.egg-info/PKG-INFO
--rw-r--r--   0 git      (13229) t3tok     (2400)      723 2023-09-20 08:27:50.000000 aug_sfutils-0.8.9/aug_sfutils.egg-info/SOURCES.txt
--rw-r--r--   0 git      (13229) t3tok     (2400)        1 2023-09-20 08:27:50.000000 aug_sfutils-0.8.9/aug_sfutils.egg-info/dependency_links.txt
--rw-r--r--   0 git      (13229) t3tok     (2400)       12 2023-09-20 08:27:50.000000 aug_sfutils-0.8.9/aug_sfutils.egg-info/top_level.txt
--rwxr-xr-x   0 git      (13229) t3tok     (2400)      104 2023-09-11 11:10:50.000000 aug_sfutils-0.8.9/pyproject.toml
--rwxr-xr-x   0 git      (13229) t3tok     (2400)      590 2023-09-20 08:27:51.000000 aug_sfutils-0.8.9/setup.cfg
-drwxr-xr-x   0 git      (13229) t3tok     (2400)        0 2023-09-20 08:27:51.000000 aug_sfutils-0.8.9/tests/
--rwxr-xr-x   0 git      (13229) t3tok     (2400)      205 2023-09-11 11:10:52.000000 aug_sfutils-0.8.9/tests/test_dds.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)      579 2023-09-11 11:10:52.000000 aug_sfutils-0.8.9/tests/test_rhotheta.py
+drwx--x---   0 git      (13229) nobody   (65534)        0 2024-04-26 08:26:50.439885 aug_sfutils-0.9.1/
+-rwx------   0 git      (13229) nobody   (65534)     1080 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/LICENSE
+-rwxr--r--   0 git      (13229) nobody   (65534)      549 2024-04-26 08:26:50.436896 aug_sfutils-0.9.1/PKG-INFO
+-rwx------   0 git      (13229) nobody   (65534)       99 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/README.md
+drwx--x---   0 git      (13229) nobody   (65534)        0 2024-04-26 08:26:50.378215 aug_sfutils-0.9.1/aug_sfutils/
+-rwx------   0 git      (13229) nobody   (65534)     1270 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/__init__.py
+-rwx------   0 git      (13229) nobody   (65534)      125 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/config.py
+-rwx------   0 git      (13229) nobody   (65534)     6658 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/contour.py
+-rwx------   0 git      (13229) nobody   (65534)    29146 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/equilibrium.py
+-rwx------   0 git      (13229) nobody   (65534)     1834 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/getlastshot.py
+-rwx------   0 git      (13229) nobody   (65534)     9080 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/journal.py
+-rwx------   0 git      (13229) nobody   (65534)     1612 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/libddc.py
+-rwx------   0 git      (13229) nobody   (65534)     3892 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/manage_ed.py
+-rwx------   0 git      (13229) nobody   (65534)    28018 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/mapeq.py
+-rwx------   0 git      (13229) nobody   (65534)      242 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/parse_kwargs.py
+-rwx------   0 git      (13229) nobody   (65534)     3340 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/read_imas.py
+-rwx------   0 git      (13229) nobody   (65534)     7318 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/sfh.py
+-rwx------   0 git      (13229) nobody   (65534)     4049 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/sfhmod.py
+-rwx------   0 git      (13229) nobody   (65534)     7191 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/sfmap.py
+-rwx------   0 git      (13229) nobody   (65534)      720 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/sfobj.py
+-rwx------   0 git      (13229) nobody   (65534)    15139 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/sfread.py
+-rwx------   0 git      (13229) nobody   (65534)    28008 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/shotfile.py
+-rwx------   0 git      (13229) nobody   (65534)      831 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/str_byt.py
+-rwx------   0 git      (13229) nobody   (65534)     1329 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/time_no_elm.py
+-rwx------   0 git      (13229) nobody   (65534)     6161 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/time_slice.py
+-rwx------   0 git      (13229) nobody   (65534)    18981 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/aug_sfutils/ww.py
+drwx--x---   0 git      (13229) nobody   (65534)        0 2024-04-26 08:26:50.429574 aug_sfutils-0.9.1/aug_sfutils.egg-info/
+-rwxr--r--   0 git      (13229) nobody   (65534)      549 2024-04-26 08:26:50.000000 aug_sfutils-0.9.1/aug_sfutils.egg-info/PKG-INFO
+-rwx------   0 git      (13229) nobody   (65534)      755 2024-04-26 08:26:50.000000 aug_sfutils-0.9.1/aug_sfutils.egg-info/SOURCES.txt
+-rwx------   0 git      (13229) nobody   (65534)        1 2024-04-26 08:26:50.000000 aug_sfutils-0.9.1/aug_sfutils.egg-info/dependency_links.txt
+-rwx------   0 git      (13229) nobody   (65534)       12 2024-04-26 08:26:50.000000 aug_sfutils-0.9.1/aug_sfutils.egg-info/top_level.txt
+-rwx------   0 git      (13229) nobody   (65534)      104 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/pyproject.toml
+-rwx------   0 git      (13229) nobody   (65534)      590 2024-04-26 08:26:50.445558 aug_sfutils-0.9.1/setup.cfg
+drwx--x---   0 git      (13229) nobody   (65534)        0 2024-04-26 08:26:50.421031 aug_sfutils-0.9.1/tests/
+-rwx------   0 git      (13229) nobody   (65534)      205 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/tests/test_dds.py
+-rwx------   0 git      (13229) nobody   (65534)      579 2024-04-26 08:19:20.000000 aug_sfutils-0.9.1/tests/test_rhotheta.py
```

### Comparing `aug_sfutils-0.8.9/LICENSE` & `aug_sfutils-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aug_sfutils-0.8.9/PKG-INFO` & `aug_sfutils-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aug_sfutils
-Version: 0.8.9
+Version: 0.9.1
 Summary: A utility to read AUG shotfiles
 Home-page: https://gitlab.mpcdf.mpg.de/git/aug_sfutils
 Author: Giovanni Tardini
 Author-email: giovanni.tardini@ipp.mpg.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aug_sfutils-0.8.9/aug_sfutils/__init__.py` & `aug_sfutils-0.9.1/aug_sfutils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 """Shotfile reading with pure python
 
 https://www.aug.ipp.mpg.de/aug/manuals/aug_sfutils
 
 """
 __author__  = 'Giovanni Tardini (Tel. 1898)'
-__version__ = '0.8.9'
-__date__    = '20.09.2023'
+__version__ = '0.9.1'
+__date__    = '12.01.2024'
 
 import os, sys, logging, traceback
 
 fmt = logging.Formatter('%(asctime)s | %(name)s | %(levelname)s: %(message)s', '%H:%M:%S')
 
 logger = logging.getLogger('aug_sfutils')
 
@@ -38,15 +38,15 @@
 try:
     from .journal import *
 except:
     traceback.print_exc()
     logger.warning('journal not loaded')
 
 from .sfread import *
-from .sf2equ import *
+from .equilibrium import *
 from .libddc import ddcshotnr, previousshot
 from .mapeq import *
 from .contour import *
 try:
     from .getlastshot import getlastshot
 except:
     traceback.print_exc()
```

### Comparing `aug_sfutils-0.8.9/aug_sfutils/contour.py` & `aug_sfutils-0.9.1/aug_sfutils/contour.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 import numpy as np
 from aug_sfutils import SFREAD, str_byt
 
+class ROT_MATRIX:
+
+
+    def __init__(self, alpha, x_in, y_in, x_cen=0, y_cen=0):
+
+        x_in2  = x_in - x_cen
+        y_in2  = y_in - y_cen
+        x_out2 = x_in2*np.cos(alpha) - y_in2*np.sin(alpha)
+        y_out2 = x_in2*np.sin(alpha) + y_in2*np.cos(alpha)
+        self.x = x_out2 + x_cen
+        self.y = y_out2 + y_cen
+
 Rlim_xml = np.array([ \
     0.2887, 1.1357, 1.1383, 1.1408, 1.1431, 1.1450, 1.2466, 1.2500, 1.2588, 1.2664, \
     1.2729, 1.2783, 1.2854, 1.2878, 1.2872, 1.2829, 1.2360, 1.2340, 1.2437, 1.2440, \
     1.2440, 1.2799, 1.2799, 1.2804, 1.3225, 1.3256, 1.4590, 1.4629, 1.5541, 1.5553, \
     1.5553, 1.5675, 1.5793, 1.5794, 1.6140, 1.6352, 1.6361, 1.6431, 1.6581, 1.6737, \
     1.7021, 1.7075, 1.7155, 1.7274, 1.7389, 1.7521, 1.9944], dtype=np.float32)
 
@@ -143,7 +155,47 @@
             jvert = len(s1) - 1
 # Interpolate R, z
         ds_ratio = (slen - s_vert[jvert])/ds_vert[jvert]
         Rout[js] = Rlim_aug[jvert] + ds_ratio*(Rlim_aug[jvert+1] - Rlim_aug[jvert])
         Zout[js] = Zlim_aug[jvert] + ds_ratio*(Zlim_aug[jvert+1] - Zlim_aug[jvert])
 
     return np.squeeze(Rout), np.squeeze(Zout)
+
+
+def getgc_tor(rotate=True):
+
+    '''Reading structure components in horizontal cut'''
+
+    f_geom = '/shares/departments/AUG/users/git/diaggeom.data/tor.data'
+    f = open(f_geom, 'r')
+
+    xtor_struct = {}
+    ytor_struct = {}
+    jstr = 0
+    xtor_struct[jstr] = []
+    ytor_struct[jstr] = []
+    for line in f.readlines():
+        if (line.strip() != ''):
+            xval, yval = line.split()
+            xtor_struct[jstr].append(float(xval))
+            ytor_struct[jstr].append(float(yval))
+        else:
+            jstr += 1
+            xtor_struct[jstr] = []
+            ytor_struct[jstr] = []
+    f.close()
+    nstr = jstr
+
+# Rotate
+
+    if rotate:
+        gamma = -3*np.pi/8. # 3 sectors out of 16
+    else:
+        gamma = 0.
+
+    tor_str = {}
+    for jstr in range(nstr):
+        x_in = np.array(xtor_struct[jstr])
+        y_in = np.array(ytor_struct[jstr])
+        tor_str[jstr] = ROT_MATRIX(gamma, x_in, y_in)
+
+    return tor_str
```

### Comparing `aug_sfutils-0.8.9/aug_sfutils/getlastshot.py` & `aug_sfutils-0.9.1/aug_sfutils/getlastshot.py`

 * *Files identical despite different names*

### Comparing `aug_sfutils-0.8.9/aug_sfutils/journal.py` & `aug_sfutils-0.9.1/aug_sfutils/journal.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A class for reading and manipulating the 'augjournal' from MariaDB"""
 
-import logging, datetime, dateutil, traceback
+import logging, datetime, time, dateutil, traceback
 import pandas as pd
 from sqlalchemy import create_engine
 
 logger = logging.getLogger('journal')
 fmt = logging.Formatter('%(asctime)s | %(name)s | %(levelname)s: %(message)s', '%H:%M:%S')
 if len(logger.handlers) == 0:
     hnd = logging.StreamHandler()
@@ -240,14 +240,38 @@
             Int >0 if day=date is/was an experimental day, 0 otherwise
         """
 
         df = self.searchSession(date=date, onlyUseful=False)
         return len(df)
 
 
+    def wait4nextShot(self, hour_end=19, time_sleep=60):
+        '''Waits for a new JOU shotfile to be created, then it returns the new shot number'''
+
+        refShot = self.getLastShot() # for reference
+        logger.debug('Initial shot %d', refShot)
+        while True:
+            logger.info('Waiting for the next shot')
+            logger.info('Ctrl+C to exit')
+            loctime = time.localtime(time.time())
+            hour = loctime[3]
+            if hour >= hour_end: # Quit at 7 p.m. or custom time
+                break
+            try:
+                newShot = JOU.getLastShot()
+                if newShot > refShot:
+                    return newShot
+            except:
+                logger.error('Problems reading last shot number')
+                continue
+            time.sleep(time_sleep)
+
+        return None
+
+
 if __name__ == '__main__':
 
     jou = JOURNAL()
 
     shot = 38384
 
     entry_d = jou.getShotEntries(shot)
```

### Comparing `aug_sfutils-0.8.9/aug_sfutils/libddc.py` & `aug_sfutils-0.9.1/aug_sfutils/libddc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from aug_sfutils import config
 
 
 def ddcshotnr(diag, shot=99999, exp='AUGD'):
     """Py-ddcshotnr
-    Gets next shotnumber of specified diagnostic from
+    Gets closest shotnumber of specified diagnostic from
     specified experiment smaller than the provided shotnumber
 
     Input:
         diag        str  Diagnostic
         shot(opt)   int  Shot number (default: 99999)
         exp(opt)    str  Exp (default: 'AUGD')
     Error codes:
@@ -22,15 +22,16 @@
     # AUGD shotfiles follow a particular path-specification
     basepath = os.path.join(config.sfBasepath, exp.lower(), diag.upper())
 
     # go backwards starting with directory of given shot
     for nshot1000 in range(int(shot//1000), -1, -1):
         sub_dir = '%s/%d' %(basepath, nshot1000)
         if os.path.isdir(sub_dir):
-            for nshot in range(shot, nshot1000*1000, -1):
+            shot_beg = min(shot, (nshot1000+1)*1000-1)
+            for nshot in range(shot_beg, nshot1000*1000-1, -1):
                 sfpath = '%s/%d' %(sub_dir, nshot)
                 if os.path.isfile(sfpath):
                     return nshot
                 for ed in range(1, 100):
                     sfpath = '%s/%d.%d' %(sub_dir, nshot, ed)
                     if os.path.isfile(sfpath):
                         return nshot
@@ -38,11 +39,7 @@
     return -1
 
 
 def previousshot(diag, shot=99999, exp='AUGD'):
     """Alias of ddcshotnr
     """
     return ddcshotnr(diag, shot=shot, exp=exp)
-
-
-if __name__ == "__main__":
-    pass
```

### Comparing `aug_sfutils-0.8.9/aug_sfutils/manage_ed.py` & `aug_sfutils-0.9.1/aug_sfutils/manage_ed.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os, struct, logging, traceback
 import numpy as np
 from aug_sfutils import config
 
 logger = logging.getLogger('aug_sfutils.manage_ed')
-logger.level = logging.INFO
-#logger.level = logging.DEBUG
+#logger.level = logging.INFO
+logger.level = logging.DEBUG
 
 
 def sf_path(nshot, diag, exp='AUGD', ed=0):
     """Path finder for shotfiles
 
     Input:
         nshot    int  Shotnumber
```

### Comparing `aug_sfutils-0.8.9/aug_sfutils/mapeq.py` & `aug_sfutils-0.9.1/aug_sfutils/mapeq.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Equilibrium utilities library
 """
 
 import sys, time, logging, datetime
 import numpy as np
 from scipy.ndimage import map_coordinates
 from scipy.interpolate import UnivariateSpline, interp1d, InterpolatedUnivariateSpline, RectBivariateSpline, LinearNDInterpolator
-from aug_sfutils.sf2equ import sigma
+from aug_sfutils.equilibrium import sigma
 
 logger = logging.getLogger('aug_sfutils.mapeq')
 #logger.setLevel(logging.INFO)
 
 
 def get_nearest_index(tim_eq, tarr):
     """Find nearest time index for a given time.
@@ -675,23 +675,26 @@
         #solve some issues very close to the core
         rho_line[:,:,0] = 0
 
     for i, ii in enumerate(unique_idx):
         jt = index_idx[ii]
         for k in range(ntheta):
             rho_lin = rho_line[i, k]
-            (tmp, ) = np.where(np.diff(rho_lin) > 0)
-            imax = tmp[-1] + 1
+            (tmp, ) = np.where(np.diff(rho_lin) <= 0) # UniSpline needs monotonic+ x array
+            if len(tmp) > 0:
+                imax = tmp[0] + 1
+            else:
+                imax = len(rho_lin)
+
             rspl = InterpolatedUnivariateSpline(rho_lin[:imax], \
-                   line_r[i, k, :imax], k=2) 
-            
+                   line_r[i, k, :imax], k=2)
             R[jt, k] = rspl(rho[jt].flatten()).reshape(rho[jt].shape)
 
-            zspl = InterpolatedUnivariateSpline( \
-                   rho_line[i, k, :imax], line_z[i, k, :imax], k=2)
+            zspl = InterpolatedUnivariateSpline(rho_lin[:imax], \
+                   line_z[i, k, :imax], k=2)
             z[jt, k] = zspl(rho[jt].flatten()).reshape(rho[jt].shape)
 
     return R, z
 
 
 def mag_theta_star(eqm, t_in, n_rho=400, n_theta=200, rz_grid=False ):
     
@@ -812,15 +815,15 @@
     return np.squeeze(rho_surf)
 
 
 def to_geqdsk(equ, t_in=0., cocos_out=1):
     """
     Parameters
     ----------
-    eqm: instance of aug_sfutils.sf2equ.EQU
+    eqm: instance of aug_sfutils.equilibrium.EQU
     t_in : float
         Time in seconds.
 
     Returns
     -------
     dict :
         Dictionary containing CLISTE results in OMFIT geqdsk format.
@@ -860,28 +863,33 @@
     geq['RLEFT']   = equ.Rmesh[0]
     geq['RDIM']    = equ.Rmesh[-1] - equ.Rmesh[0]
     geq['ZDIM']    = equ.Zmesh[-1] - equ.Zmesh[0]
     geq['RMAXIS']  = equ.Rmag[jt]
     geq['ZMAXIS']  = equ.Zmag[jt]
     geq['SIMAG']   = psi_in[0]
     geq['SIBRY']   = psi_in[-1]
-    geq['CURRENT'] = equ.ip[jt]
+    if hasattr(equ, 'ip'):
+        geq['CURRENT'] = equ.ip[jt]
+    else:
+        geq['CURRENT'] = equ.ipipsi[jt]
     geq['BCENTR']  = equ.B0[jt]
     geq['RCENTR']  = equ.R0  ##[jt]   # TODO this seems to be time-independent?
     geq['ZMID']    = 0.5*(equ.Zmesh[-1] + equ.Zmesh[0])
     geq['PSIRZ'] = equ.pfm[:, :, jt]
 
     # Interpolate onto an equidistant Psi-grid
     psi_grid = np.linspace(psi_in[0], psi_in[-1], len(equ.Rmesh))
 
 # np.interp fails if "psi_in" is non-monotonic or not ascending
     q  = interp1d(psi_in, equ.q[jt]    , kind='linear', fill_value='extrapolate')
     p  = interp1d(psi_in, equ.pres[jt] , kind='linear', fill_value='extrapolate')
     dp = interp1d(psi_in, equ.dpres[jt], kind='linear', fill_value='extrapolate')
     f  = interp1d(psi_in, 2.e-7*equ.jpol[jt], kind='linear', fill_value='extrapolate')
+    if equ.ffp is None:
+        equ.ffp = 4.e-14 * equ.jpol * equ.djpol
     df = interp1d(psi_in, -2*np.pi*equ.ffp[jt], kind='linear', fill_value='extrapolate')
     geq['QPSI']   = q(psi_grid)
     geq['PRES']   = p(psi_grid)
     geq['PPRIME'] = dp(psi_grid)
     geq['FPOL']   = f(psi_grid)
     geq['FFPRIM'] = df(psi_grid)
```

### Comparing `aug_sfutils-0.8.9/aug_sfutils/sfh.py` & `aug_sfutils-0.9.1/aug_sfutils/sfh.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,14 +65,23 @@
 
         if qual:
             err = libsfh.sfhmdqualindex(self.c_sfid, c_obj, c_nx, c_ny, c_nz)
         else:
             err = libsfh.sfhmdindex24(self.c_sfid, c_obj, c_nx, c_ny, c_nz)
         libsfh.sfherror(err, 'mdindex24')
 
+    def Mdformat(self, obj, fmt):
+
+        bobj  = str_byt.to_byt(obj)
+        c_obj = ct.c_char_p(bobj)
+        c_format = ct.c_uint16(fmt)
+
+        err = libsfh.sfhmdformat(self.c_sfid, c_obj, c_format)
+        libsfh.sfherror(err, 'mdformat')
+        
     def Modtim(self, obj, nt):
         """Modifes the size of the time dimension of an object
         """
 
         bobj  = str_byt.to_byt(obj)
         c_obj = ct.c_char_p(bobj)
         c_nt  = ct.c_uint32(nt)
```

### Comparing `aug_sfutils-0.8.9/aug_sfutils/sfhmod.py` & `aug_sfutils-0.9.1/aug_sfutils/sfhmod.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             logger.error('modtim accepts only TB, AB, Sig, SigName')
         elif SFOlbl in ('TimeBase', 'AreaBase'):
             sfo.n_steps = nt
         elif SFOlbl == 'Signal':
             sfo.index[-1] = nt
         elif SFOlbl == 'SignalGroup':
             tdim = None
-            for robj in sfo.relobjects:
+            for jrel, robj in enumerate(sfo.relobjects):
                 if robj.SFOtypeLabel == 'TimeBase':
                     tdim = jrel
                     break
             if tdim is not None:
                 sfo.index[3-tdim] = nt
 
 
@@ -68,15 +68,15 @@
             index.append(1)
         sfo.index = index[::-1]
 
 
     def modareasize(self, abase, size_x=None, size_y=None, size_z=None):
         '''Changes the sizes of an AreaBase'''
 
-        sfobj = self.sffull[abase]
+        sfo = self.sffull[abase]
         if sfo.SFOtypeLabel != 'AreaBase':
             logger.error('modareasize needs an AreaBase')
             return
 
         if size_x is not None:
             sfo.size_x = size_x
         if size_y is not None:
```

### Comparing `aug_sfutils-0.8.9/aug_sfutils/sfmap.py` & `aug_sfutils-0.9.1/aug_sfutils/sfmap.py`

 * *Files identical despite different names*

### Comparing `aug_sfutils-0.8.9/aug_sfutils/sfobj.py` & `aug_sfutils-0.9.1/aug_sfutils/sfobj.py`

 * *Files identical despite different names*

### Comparing `aug_sfutils-0.8.9/aug_sfutils/sfread.py` & `aug_sfutils-0.9.1/aug_sfutils/sfread.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,16 @@
             else:
                 self.shot = nshot
                 self.diag = diag.upper()
                 self.exp  = exp  # unused herein, but useful docu
 
         logger.debug('Shotfile path: %s', self.sfpath)
         if os.path.isfile(self.sfpath):
-            self.time = datetime.datetime.fromtimestamp(os.path.getctime(self.sfpath))
+            self.timePath = datetime.datetime.fromtimestamp(os.path.getctime(self.sfpath))
+            self.time = datetime.datetime.fromtimestamp(os.path.getmtime(self.sfpath))
         else:
             logger.error('Shotfile %s not found' %self.sfpath)
             return
 
         logger.info('Fetching SF %s', self.sfpath)
         self.sf = SF(self.sfpath)
         self.status = (self.sf is not None)
@@ -277,15 +278,15 @@
 
     def raw2calib(self, sfo):
         """
         Calibrates an uncalibrated Signal or SignalGroup
         """
 # Calibrated signals and signal groups
         if sfo.SFOtypeLabel not in ('SignalGroup', 'Signal'):
-            logging.error('Calibration failed for %s: no Sig, no SGR', sfo.objectname)
+            logging.error('Calibration failed for %s: no Sig, no SGR', sfo.objectName)
             return sfo
 
         pscal = self.lincalib(sfo)
         if pscal is None:
             if sfo.phys_unit == 'counts':
                 for robj in sfo.relobjects:
                     if robj.SFOtypeLabel == 'TimeBase':
@@ -306,18 +307,22 @@
             shift = np.atleast_1d(pscal[shif])
             if sfo.SFOtypeLabel == 'Signal' or len(multi) == 1:
                 sfo *= multi[0] # MXR
                 sfo += shift[0]
             else:
                 n_pars = sfo.shape[1]
                 if n_pars != len(multi):
-                    logger.warning('Inconsitent sizes in calibration PSet %s', obj)
+                    logger.warning('Inconsitent sizes in calibration PSet %s', sfo.objectName)
                 if n_pars <= len(multi):
-                    sfo *= multi[: n_pars] # BLB
-                    sfo += shift[: n_pars]
+                    if sfo.ndim == 3:
+                        sfo *= multi[np.newaxis, : n_pars, np.newaxis]
+                        sfo += shift[np.newaxis, : n_pars, np.newaxis]
+                    else:
+                        sfo *= multi[: n_pars] # BLB
+                        sfo += shift[: n_pars]
                 else:
                     sfo *= multi[0]
                     sfo += shift[0]
 
         return sfo
 
 
@@ -351,15 +356,22 @@
         return self.sf[obj].data
 
 
     def getlist_by_type(self, SFOlbl='Signal'):
         """
         Returns a list of names of all SF-objects of a given type (Signal, TimeBase)
         """
-        return [lbl for lbl, sfo in self.sf.items() if sfo.SFOtypeLabel == SFOlbl]
+        objlist = []
+        if isinstance(SFOlbl, int):
+            SFOlbl = sfmap.olbl[SFOlbl]
+        for lbl, sfo in self.sf.items():
+            if hasattr(sfo, 'SFOtypeLabel'):
+                if sfo.SFOtypeLabel == SFOlbl:
+                    objlist.append(lbl)
+        return objlist
 
 
     def getobjectName(self, jobj):
         """
         Returns the object name for an inpur object ID
         """
```

### Comparing `aug_sfutils-0.8.9/aug_sfutils/shotfile.py` & `aug_sfutils-0.9.1/aug_sfutils/shotfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,52 +118,63 @@
             self.sfh2byte() # converts to bytes string (Shotfile content)
 
 
     def read_sfh(self, psets=True):
         """Reads a full shotfile header, including the data of ParamSets, Devices, Lists"""
 
         self.SFobjects = []
-        self.addressMultiplier   = 1
+        self.addressMultiplier = 1
 
-        n_max = 1000
+        n_max = 10000
         n_obj = n_max
-        self.objId2objName = []
+        self.objNames = []
+        self.objects  = []
+        self.parsets  = []
         for j in range(n_max):
             sfo = SF_OBJECT(jobj=j, sfname=self.shotfilePath)
             if hasattr(sfo, 'objectType'):
                 sfo.objid = j
                 onam = sfo.objectName
-                if sfo.SFOtypeLabel == 'Diagnostic':
-                    if n_obj == n_max: # There might be several diags objects in a SFH
-                        self.shotNumber = sfo.shot
-                        self.diagName   = str_byt.to_str(sfo.diag.strip())
-                        n_obj = sfo.num_objs
-                self.objId2objName.append(onam)
-                self.SFobjects.append(sfo)
-                if sfo.SFOtypeLabel == 'ADDRLEN':
-                    self.addressMultiplier = sfmap.addrsizes[sfo.addrlen]
-                self.__dict__[onam] = sfo
-            if j >= n_obj - 1:
-                break
+                if onam:
+                    typ = sfo.SFOtypeLabel
+                    if typ == 'Diagnostic':
+                        if n_obj == n_max: # There might be several diags objects in a SFH
+                            self.shotNumber = sfo.shot
+                            self.diagName   = str_byt.to_str(sfo.diag.strip())
+                            n_obj = sfo.num_objs
+                    elif typ in ('SignalGroup', 'Signal', 'TimeBase', 'AreaBase'):
+                        self.objects.append(onam)
+                    elif typ in ('ParamSet', 'Device'):
+                        self.parsets.append(onam)
+                    elif typ == 'ADDRLEN':
+                        self.addressMultiplier = sfmap.addrsizes[sfo.addrlen]
+                    self.objNames.append(onam)
+                    self.SFobjects.append(sfo)
+                    self.__dict__[onam] = sfo
+                if j >= n_obj - 1:
+                    break
 
 
     def set_attributes(self):
         """Sets useful context info for the entire shotfile, plus data for Lists, ParmSets, Devices"""
 
         for sfo in self.SFobjects:
             sfo.address *= self.addressMultiplier
-            sfo.relations  = [self.objId2objName[jid] for jid in sfo.rel if jid != 65535]
-            sfo.relobjects = [self.SFobjects[jid]     for jid in sfo.rel if jid != 65535]
+            sfo.relations  = [self.objNames[jid]  for jid in sfo.rel if jid != 65535]
+            sfo.relobjects = [self.SFobjects[jid] for jid in sfo.rel if jid != 65535]
             if hasattr(sfo, 'dataFormat'):
                 if sfo.dataFormat in sfmap.dtf['SFfmt'].values:
                     sfo.dataType = sfmap.typeMap('SFfmt', 'descr', sfo.dataFormat)
 
             if sfo.SFOtypeLabel == 'List':
-                sfo.getList()
-                sfo.data = [self.objId2objName[jid] for jid in sfo.data]
+                try:
+                    sfo.getList()
+                    sfo.data = [self.objNames[jid] for jid in sfo.data]
+                except:
+                    logger.error('List %s not read properly', sfo.objectName)
             elif sfo.SFOtypeLabel in ('Device', 'ParamSet'):
                 sfo.getParamSet()
             elif sfo.SFOtypeLabel in ('Signal', 'SignalGroup'):
                 for jrel, robj in enumerate(sfo.relobjects):
 # check where the related timebase is
                     if robj.SFOtypeLabel == 'TimeBase':
                         shape_arr = sfo.index[::-1][:sfo.num_dims]
@@ -514,16 +525,16 @@
                 self.ppg_time()
             else:   # ADC_intern, e.g. DCN:T-ADC-SL
                 self.data = (np.arange(self.n_steps, dtype=np.float32) - self.n_pre)/self.s_rate
         else:
             type_len = sfmap.typeLength(dfmt)
             bytlen = np.prod(shape_arr) * type_len
             if dfmt in sfmap.fmt2len.keys(): # char variable
-                data2 = np.chararray(shape_arr, itemsize=type_len, buffer=getChunk(self.sfname, self.address, bytlen), order='F')
-                self.data = np.array([str_byt.to_str(val) for val in data2.ravel()]).reshape(data2.shape) # <1ms for SSQ
+                raw = getChunk(self.sfname, self.address, bytlen)
+                self.data = np.array([str_byt.to_str(raw[i:i+type_len], strip=False) for i in range(0, len(raw), type_len)]).reshape(shape_arr[::-1]).T
             else: # numerical variable
                 sfmt = sfmap.typeMap('SFfmt', 'struc', dfmt)
                 addr = self.address
 # Read data only in the time range of interest
                 if self.SFOtypeLabel in ('Signal', 'TimeBase', 'AreaBase') or self.time_last():
                     addr += type_len*nbeg*np.prod(shape_arr[:-1])
                     if nend is None:
```

### Comparing `aug_sfutils-0.8.9/aug_sfutils/str_byt.py` & `aug_sfutils-0.9.1/aug_sfutils/str_byt.py`

 * *Files identical despite different names*

### Comparing `aug_sfutils-0.8.9/aug_sfutils/time_no_elm.py` & `aug_sfutils-0.9.1/aug_sfutils/time_no_elm.py`

 * *Files identical despite different names*

### Comparing `aug_sfutils-0.8.9/aug_sfutils/time_slice.py` & `aug_sfutils-0.9.1/aug_sfutils/time_slice.py`

 * *Files identical despite different names*

### Comparing `aug_sfutils-0.8.9/aug_sfutils/ww.py` & `aug_sfutils-0.9.1/aug_sfutils/ww.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 logger = logging.getLogger('aug_sfutils.ww')
 #logger.setLevel(logging.INFO)
 #logger.setLevel(logging.DEBUG)
 
 wwlib = os.path.join(config.sfLib, 'libddww8.so')
 libddww = ct.cdll.LoadLibrary(wwlib)
 
-LOGICAL = sfmap.typeMap('descr', 'SFfmt', 'LOGICAL')
+LOGICAL = sfmap.typeMap('descr', 'SFtyp', 'LOGICAL')
 
 
 def getError(error):
 
     """ Check if an error/warning occured
     """
 
@@ -47,14 +47,21 @@
     """
 
     def Open(self, exp, diag, nshot, edition=-1, mode='new'):
         """Equivalent of wwopen
         Prepares output shotfile.
         """
         self.Close()
+        if exp.lower() != 'augd':
+            outDir = '%s/%s/%s' %(config.sfBasepath, exp.lower(), diag.upper())
+            edDir  = '%s/edcntl_dir' %outDir
+            if not os.path.isdir(outDir):
+                os.mkdir(outDir)
+            if not os.path.isdir(edDir):
+                os.mkdir(edDir)
         if nshot > 0:
             date = datetime.date.strftime(datetime.datetime.today(),'%y.%m.%d;%H:%M:%S')
 
             exp  = str_byt.to_byt(exp)
             diag = str_byt.to_byt(diag)
             mode = str_byt.to_byt(mode)
             date = str_byt.to_byt(date)
@@ -419,16 +426,15 @@
                     buffer = ctyp(datanp)
                 else:
                     buffer = ctyp.from_buffer(datanp)
                 _buffer = ct.byref(buffer)
                 result = libddww.wwparm_(_error, self._diaref, pset, par, _type, _lbuf, \
                                          _buffer, _stride, lset, lpar)
             if getError( error ):
-                raise Exception('ww: Error Writing Parameters into %s -> %s' %(set_name.decode('utf-8'), par_name.decode('utf-8') ) )
-
+                raise Exception('ww: Error Writing Parameters into %s -> %s' %(set_name, par_name) )
             else:
                 logger.info('   PN %s', par_name.decode('utf8'))
 
 
 def write_sf(nshot, data_d, sfhdir, diag, exp='AUGD'):
     """Function for writing a full shotfile from a data dict
```

### Comparing `aug_sfutils-0.8.9/aug_sfutils.egg-info/PKG-INFO` & `aug_sfutils-0.9.1/aug_sfutils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aug-sfutils
-Version: 0.8.9
+Name: aug_sfutils
+Version: 0.9.1
 Summary: A utility to read AUG shotfiles
 Home-page: https://gitlab.mpcdf.mpg.de/git/aug_sfutils
 Author: Giovanni Tardini
 Author-email: giovanni.tardini@ipp.mpg.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aug_sfutils-0.8.9/aug_sfutils.egg-info/SOURCES.txt` & `aug_sfutils-0.9.1/aug_sfutils.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 ./aug_sfutils/__init__.py
 ./aug_sfutils/config.py
 ./aug_sfutils/contour.py
+./aug_sfutils/equilibrium.py
 ./aug_sfutils/getlastshot.py
 ./aug_sfutils/journal.py
 ./aug_sfutils/libddc.py
 ./aug_sfutils/manage_ed.py
 ./aug_sfutils/mapeq.py
 ./aug_sfutils/parse_kwargs.py
-./aug_sfutils/sf2equ.py
+./aug_sfutils/read_imas.py
 ./aug_sfutils/sfh.py
 ./aug_sfutils/sfhmod.py
 ./aug_sfutils/sfmap.py
 ./aug_sfutils/sfobj.py
 ./aug_sfutils/sfread.py
 ./aug_sfutils/shotfile.py
 ./aug_sfutils/str_byt.py
```

### Comparing `aug_sfutils-0.8.9/setup.cfg` & `aug_sfutils-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `aug_sfutils-0.8.9/tests/test_rhotheta.py` & `aug_sfutils-0.9.1/tests/test_rhotheta.py`

 * *Files identical despite different names*

