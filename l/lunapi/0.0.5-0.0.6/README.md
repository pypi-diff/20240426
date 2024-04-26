# Comparing `tmp/lunapi-0.0.5-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/lunapi-0.0.6-pp39-pypy39_pp73-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,11 @@
-Zip file size: 9868572 bytes, number of entries: 13
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-06 17:57 lunapi-0.0.5.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-06 17:57 lunapi/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-06 17:57 lunapi.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-06 17:57 lunapi-0.0.5.dist-info/licenses/
--rw-rw-r--  2.0 unx      165 b- defN 24-Feb-06 17:57 lunapi-0.0.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx     1372 b- defN 24-Feb-06 17:57 lunapi-0.0.5.dist-info/METADATA
--rw-rw-r--  2.0 unx        0 b- defN 24-Feb-06 17:57 lunapi-0.0.5.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx      734 b- defN 24-Feb-06 17:57 lunapi-0.0.5.dist-info/RECORD
--rw-rw-r--  2.0 unx    35149 b- defN 24-Feb-06 17:57 lunapi-0.0.5.dist-info/licenses/LICENSE
--rwxr-xr-x  2.0 unx 25495488 b- defN 24-Feb-06 17:57 lunapi/lunapi0.pypy39-pp73-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx     8894 b- defN 24-Feb-06 17:57 lunapi/lunapi0.cpp
--rw-r--r--  2.0 unx      353 b- defN 24-Feb-06 17:57 lunapi/__init__.py
--rw-r--r--  2.0 unx    34822 b- defN 24-Feb-06 17:57 lunapi/lunapi1.py
-13 files, 25576977 bytes uncompressed, 9866884 bytes compressed:  61.4%
+Zip file size: 6484827 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx      724 b- defN 24-Apr-26 14:23 lunapi-0.0.6.dist-info/RECORD
+-rw-rw-r--  2.0 unx      118 b- defN 24-Apr-26 14:23 lunapi-0.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-26 14:23 lunapi-0.0.6.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx     1350 b- defN 24-Apr-26 14:23 lunapi-0.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx    35149 b- defN 24-Apr-26 14:23 lunapi-0.0.6.dist-info/licenses/LICENSE
+-rw-r--r--  2.0 unx      352 b- defN 24-Apr-26 14:23 lunapi/__init__.py
+-rw-r--r--  2.0 unx    44647 b- defN 24-Apr-26 14:23 lunapi/lunapi1.py
+-rwxr-xr-x  2.0 unx 13397280 b- defN 24-Apr-26 14:23 lunapi/lunapi0.pypy39-pp73-darwin.so
+-rw-r--r--  2.0 unx     9418 b- defN 24-Apr-26 14:23 lunapi/lunapi0.cpp
+9 files, 13489038 bytes uncompressed, 6483611 bytes compressed:  51.9%
```

## zipnote {}

```diff
@@ -1,40 +1,28 @@
-Filename: lunapi-0.0.5.dist-info/
+Filename: lunapi-0.0.6.dist-info/RECORD
 Comment: 
 
-Filename: lunapi/
+Filename: lunapi-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: lunapi.libs/
+Filename: lunapi-0.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: lunapi-0.0.5.dist-info/licenses/
+Filename: lunapi-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: lunapi-0.0.5.dist-info/WHEEL
+Filename: lunapi-0.0.6.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: lunapi-0.0.5.dist-info/METADATA
-Comment: 
-
-Filename: lunapi-0.0.5.dist-info/entry_points.txt
-Comment: 
-
-Filename: lunapi-0.0.5.dist-info/RECORD
+Filename: lunapi/__init__.py
 Comment: 
 
-Filename: lunapi-0.0.5.dist-info/licenses/LICENSE
+Filename: lunapi/lunapi1.py
 Comment: 
 
-Filename: lunapi/lunapi0.pypy39-pp73-x86_64-linux-gnu.so
+Filename: lunapi/lunapi0.pypy39-pp73-darwin.so
 Comment: 
 
 Filename: lunapi/lunapi0.cpp
 Comment: 
 
-Filename: lunapi/__init__.py
-Comment: 
-
-Filename: lunapi/lunapi1.py
-Comment: 
-
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## lunapi/lunapi0.cpp

```diff
@@ -70,14 +70,16 @@
     .def( "nobs" , &lunapi_t::nobs )
     .def( "clear" , &lunapi_t::clear )
 
     .def( "silence", &lunapi_t::silence )
     .def( "is_silenced" , &lunapi_t::is_silenced )
 
     .def( "flush" , &lunapi_t::flush )
+
+    .def( "reset" , &lunapi_t::reset )
     
     .def("opt",py::overload_cast<const std::string &,const std::string &>(&lunapi_t::var),
 		"Set an option value" )
 
     .def("get_opt",py::overload_cast<const std::string &>(&lunapi_t::var,py::const_ ),
 	 "Show an option value" )
     .def("get_opts",py::overload_cast<const std::vector<std::string> &>(&lunapi_t::vars,py::const_),
@@ -163,29 +165,41 @@
     .def( "attach_annot",&lunapi_inst_t::attach_annot,
 	  "Attach an annotation file to the current EDF" ,
 	  "annotfile"_a )
 
     
     .def( "refresh", &lunapi_inst_t::refresh,
 	  "Reattach the current EDF")
-    .def( "drop", &lunapi_inst_t::refresh,
+    .def( "drop", &lunapi_inst_t::drop,
 	  "Drop the current EDF" )
     
     .def( "channels", &lunapi_inst_t::channels,
 	  "Return a list of channel labels" )
     .def( "chs", &lunapi_inst_t::channels,
 	  "Return a list of channel labels" )
+    .def( "has_channels", &lunapi_inst_t::has_channels,
+	  "Return boolean for whether channels exist (with aliasing)" )
+    .def( "has", &lunapi_inst_t::has_channels,
+	  "Return boolean for whether channels exist (with aliasing)" )
+
 
+    
     .def( "annots", &lunapi_inst_t::annots,
 	  "Return a list of all annotations class labels" )
     .def( "fetch_annots", &lunapi_inst_t::fetch_annots,
 	  "Return a list of intervals for selected annotations" )
     .def( "fetch_full_annots", &lunapi_inst_t::fetch_full_annots,
 	  "Return a list of intervals and meta-data for selected annotations" )
 
+    .def( "has_annots" , &lunapi_inst_t::has_annots,
+	  "Return boolean for whether annotations exist (with aliasing)" )
+
+    .def( "has_staging" , &lunapi_inst_t::has_staging,
+	  "Return boolean for whether valid staging annotations exist" )
+    
     .def( "stat" , &lunapi_inst_t::status,
 	  "Return a dict of key details on the current EDF" )
 
     .def( "e2i" , &lunapi_inst_t::epochs2intervals ,
 	  "Convert epoch numbers to interval tuples" ,
 	  "e"_a )
     .def( "s2i" , &lunapi_inst_t::seconds2intervals ,
```

## lunapi/__init__.py

```diff
@@ -6,9 +6,8 @@
 (lunapi_t) functions
 
 __lunapi1__ is a a higher-level wrapper around lunapi0-level
     functions; most users will want to use lunapi1 functions
 
 """
 
-
 from lunapi.lunapi1 import *
```

## lunapi/lunapi1.py

```diff
@@ -1,11 +1,11 @@
 """lunapi1 module provides a high-level convenience wrapper around lunapi0 module functions."""
 
 # Luna Python wrapper
-# v0.0.5, 5-Feb-2024
+# v0.0.6, 26-Apr-2024
 
 import lunapi.lunapi0 as _luna
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib import cm
 from IPython.core import display as ICD
@@ -13,15 +13,15 @@
 
 # resource set for Docker container version
 class resources:
    POPS_PATH = '/build/nsrr/common/resources/pops/'
    POPS_LIB = 's2'
    MODEL_PATH = '/build/luna-models/'
 
-lp_version = "v0.0.5"
+lp_version = "v0.0.6"
    
 # C++ singleton class (engine & sample list)
 # lunapi_t      --> luna
 
 # one observation
 # lunapi_inst_T --> inst
 
@@ -68,35 +68,51 @@
 
       """
           
       if type( args ) is not list: args = [ args ]
       return proj.eng.build_sample_list( args )
 
    
-   def sample_list(self, filename = None ):
-      """Reads a sample-list 'filenamne' and returns the number of observations
+   def sample_list(self, filename = None , path = None , df = True ):
+      """Reads a sample-list 'filenamne', optionally setting 'path' and returns the number of observations
 
       If filename is not defined, this returns the internal sample list
       as an object
 
       Parameters
       ----------
       filename : str
           optional filename of a sample-list to read
 
+      path : str
+          optional path to preprend to the sample-list when reading (sets the 'path' variable)
+
+      df : boolean
+          if returning a sample-list, return as a Pandas dataframe
+      
       Returns
       -------
       list
           a list of strings representing the sample-list (IDs, EDFs, annotations for each individual)
       """
     
       # return sample list
       if filename is None:
-         return proj.eng.get_sample_list()
-
+         sl = proj.eng.get_sample_list()
+         if df is True:
+            sl = pd.DataFrame( sl )
+            sl.columns = [ 'ID' , 'EDF', 'Annotations' ]
+            sl.index += 1 
+         return sl
+
+      # set path?
+      if path is not None:
+         print( "setting path to " , path )
+         self.var( 'path' , path )
+         
       # read sample list from file, after clearing anything present
       proj.eng.clear()
       self.n = proj.eng.read_sample_list( filename )
       print( "read",self.n,"individuals from" , filename )
 
 
    #------------------------------------------------------------------------
@@ -109,51 +125,57 @@
       int
           the number of observations in the sample-list
       """
 
       return proj.eng.nobs()
 
 
+   #------------------------------------------------------------------------
+      
+   def reset(self):
+      """ Drop Luna problem flag """
+      proj.eng.reset()
 
    #------------------------------------------------------------------------
    
    def inst( self, n ):
       """Generates a new instance"""
-      
-      return inst(proj.eng.inst( n ))
-      
 
-   #------------------------------------------------------------------------
+      # check bounds
+      if type(n) is int:
+         # use 1-based counts as inputs
+         n = n - 1
+         if n < 0 or n >= self.nobs():
+            print( "index out-of-bounds given sample list of " + str(self.nobs()) + " records" )
+            return
+            
+      # if the arg is a str that matches a sample-list
+      if type(n) is str:
+         sn = self.get_n(n)
+         if type(sn) is int: n = sn
+         
+      # return based on n (from sample-list) or string/empty (new instance)
+      return inst(proj.eng.inst( n ))
       
-#   def import_db( self, filename ):
-#      """Reads a Luna 'destrat' output database"""      
-#      proj.eng.import_db( filename )
-
-   #------------------------------------------------------------------------
-#   def import_db( self, filename , ids ):
-#      """Reads a subset of individuals from a 'destrat' output database"""
-#      
-#      proj.eng.import_db( filename , ids )
 
    #------------------------------------------------------------------------
    def clear(self):
       """Clears any existing project sample-list"""
-      
       proj.eng.clear()
 
 
    #------------------------------------------------------------------------
    def silence(self, b = True , verbose = False ):
       """Toggles the output mode on/off"""
       if verbose:
          if b: print( 'silencing console outputs' )
          else: print( 'enabling console outputs' )
       proj.eng.silence(b)
 
-   #------------------------------------------------------------------------                                                                                                                                                            
+   #------------------------------------------------------------------------
    def is_silenced(self, b = True ):
       """Reports on whether log is silenced"""
       return proj.eng.is_silenced()
       
       
    #------------------------------------------------------------------------
    def flush(self):
@@ -242,14 +264,24 @@
          return proj.eng.import_db_subset(f,s)
 
    #------------------------------------------------------------------------      
    def eval(self, cmdstr ):
       """Evaluates one or more Luna commands for all sample-list individuals"""
       r = proj.eng.eval(cmdstr)
       return tables( r )
+
+   #------------------------------------------------------------------------ 
+   def silent_eval(self, cmdstr ):
+      """Silently evaluates one or more Luna commands for all sample-list individuals"""
+      silence_mode = self.is_silenced()
+      self.silence(True,False)
+      r = proj.eng.eval(cmdstr)
+      self.silence( silence_mode , False )
+      return tables( r )
+   
    
    #------------------------------------------------------------------------   
    def commands( self ):
       """Return a list of commands in the output set (following eval()"""
       t = pd.DataFrame( proj.eng.commands() )
       t.columns = ["Command"]
       return t
@@ -290,15 +322,18 @@
 
    # --------------------------------------------------------------------------------
    def pops( self, s = None, s1 = None , s2 = None,
              path = None , lib = None ,
              do_edger = True ,
              no_filter = False ,
              do_reref = False ,
-             m = None , m1 = None , m2 = None ):
+             m = None , m1 = None , m2 = None,
+             lights_off = '.' , lights_on = '.' ,
+             ignore_obs = False, 
+             args = '' ):
       """Run the POPS stager"""
 
       if path == None: path = resources.POPS_PATH
       if lib == None: lib = resources.POPS_LIB
       
       import os
       if not os.path.isdir( path ):         
@@ -314,18 +349,20 @@
          
       # set options
       self.var( 'mpath' , path )
       self.var( 'lib' , lib )
       self.var( 'do_edger' , '1' if do_edger else '0' )
       self.var( 'do_reref' , '1' if do_reref else '0' )
       self.var( 'no_filter' , '1' if no_filter else '0' )
-
+      self.var( 'LOFF' , lights_off )
+      self.var( 'LON' , lights_on )
+      
       if s != None: self.var( 's' , s )
       else: self.clear_var( 's' )
-
+      
       if m != None: self.var( 'm' , m )
       else: self.clear_var( 'm' )
 
       if s1 != None: self.var( 's1' , s1 )
       else: self.clear_var( 's1' )
       
       if s2 != None: self.var( 's2' , s2 )
@@ -337,14 +374,22 @@
       if m2 != None: self.var( 'm2' , m2 )
       else: self.clear_var( 'm2' )
             
       # get either one- or two-channel mode Luna script from POPS folder
       twoch = s1 != None and s2 != None;
       if twoch: cmdstr = cmdfile( path + '/s2.ch2.txt' )
       else: cmdstr = cmdfile( path + '/s2.ch1.txt' )
+
+      # swap in any additional options to POPS
+      if ignore_obs is True:
+         args = args + ' ignore-obs-staging';
+         if do_edger is True:
+            cmdstr = cmdstr.replace( 'EDGER' , 'EDGER all' )
+      if args != '':
+            cmdstr = cmdstr.replace( 'POPS' , 'POPS ' + args + ' ')
       
       # run the command
       self.eval( cmdstr )
 
       # return of results
       return self.table( 'POPS' )
 
@@ -410,14 +455,21 @@
       t.columns = ["Value"]
       return t
 
    #------------------------------------------------------------------------
    def refresh( self ):
       """Refresh an attached EDF"""
       self.edf.refresh()
+      # also need to reset Luna problem flag
+      # note: current kludge: problem is proj-wide
+      #       so this will not play well w/ multiple EDFs
+      # todo: implement inst-specific prob flag
+      
+      _proj = proj(False)
+      _proj.reset();
 
    #------------------------------------------------------------------------      
    def ivar( self , key , value = None ):
       """Set or get an individual-level variable"""
       if value != None: self.edf.ivar( key , str(value) )
       else: return self.edf.get_ivar( key )
          
@@ -477,14 +529,29 @@
    def proc( self, cmdstr ):
       """Evaluate one or more Luna commands, returning results as an object"""
       # < log , tables >
       r = self.edf.proc( cmdstr )
       # extract and return result tables
       return tables( r[1] ) 
 
+   #------------------------------------------------------------------------                                                                           
+   def silent_proc( self, cmdstr ):
+      """Silently evaluate one or more Luna commands (for internal use)"""
+      
+      _proj = proj(False)
+      silence_mode = _proj.is_silenced()
+      _proj.silence(True,False)
+      
+      r = self.edf.proc( cmdstr )
+
+      _proj.silence( silence_mode , False )
+
+      # extract and return result tables
+      return tables( r[1] )
+
    #------------------------------------------------------------------------   
    def empty_result_set( self ):
       return len( self.edf.strata()  ) == 0
 
    #------------------------------------------------------------------------
    def strata( self ):
       """Return a dataframe of command/strata pairs from the output set"""
@@ -565,22 +632,100 @@
 
    # --------------------------------------------------------------------------------
    #
    # Luna function wrappers
    #
    # --------------------------------------------------------------------------------
 
+
+   # --------------------------------------------------------------------------------
+   def freeze( self , f ):
+      self.eval( 'FREEZE ' + f )
+
+   # --------------------------------------------------------------------------------
+   def thaw( self , f , remove = False ):
+      if remove:
+         self.eval( 'THAW tag=' + f + 'remove' )
+      else:
+         self.eval( 'THAW ' + f )
+
+   # --------------------------------------------------------------------------------
+   def empty_freezer( self ):
+      self.eval( 'CLEAN-FREEZER' )
+      
+   # --------------------------------------------------------------------------------
+   def mask( self , f = None ):
+      if f == None: return
+      if type(f) is not list: f = [ f ]
+      [ self.eval( 'MASK ' + _f ) for _f in f ]
+      self.eval( 'RE' )   
+
+   
+   # --------------------------------------------------------------------------------
+   def segments( self ):
+      self.eval( 'SEGMENTS' )
+      return self.table( 'SEGMENTS' , 'SEG' )
+   
+   # --------------------------------------------------------------------------------
+   def epoch( self , f = '' ):
+      self.eval( 'EPOCH ' + f )
+
+
+   # --------------------------------------------------------------------------------
+   def epochs( self ):
+      self.eval( 'EPOCH table' )                
+      df = self.table( 'EPOCH' , 'E' )
+      df = df[[ 'E', 'E1', 'LABEL', 'HMS', 'START','STOP','DUR' ]]
+      #df = df.drop(columns = ['ID','TP','MID','INTERVAL'] )
+      return df
+      
+   # --------------------------------------------------------------------------------
+   def psd( self, ch, var = 'PSD' , minf = None, maxf = None, minp = None, maxp = None , xlines = None , ylines = None ):
+      """Generates a PSD plot (from PSD or MTM)"""
+      if ch == None: return
+      if type(ch) is not list: ch = [ ch ]
+
+      if var == 'PSD':
+         self.eval( 'PSD spectrum dB sig=' + ','.join(ch) )
+         df = self.table( 'PSD' , 'CH_F' )
+      else:
+         self.eval( 'MTM tw=15 dB sig=' + ','.join(ch) )
+         df = self.table( 'MTM' , 'CH_F' )
+         
+      psd( df = df , ch = ch , var = var ,
+           minf = minf , maxf = maxf , minp = minp , maxp = maxp ,
+           xlines = xlines , ylines = ylines )
+      
+    
+   # --------------------------------------------------------------------------------
+   def spec( self, ch, var = 'PSD' , mine = None, maxe = None, minf = None, maxf = None , w = 0.025 ):
+      """Generates a PSD spectrogram (from PSD or MTM)"""
+      if ch == None: return
+      if type(ch) is not list: ch = [ ch ]
+
+      if var == 'PSD':
+         self.eval( 'PSD epoch-spectrum dB sig=' + ','.join(ch) )
+         df = self.table( 'PSD' , 'CH_E_F' )
+      else:
+         self.eval( 'MTM epoch-spectra epoch epoch-output dB tw=15 sig=' + ','.join(ch) )
+         df = self.table( 'MTM' , 'CH_E_F' )
+         
+      spec( df = df , ch = None , var = var ,
+            mine = mine , maxe = maxe , minf = minf , maxf = maxf , w = w )
    
    # --------------------------------------------------------------------------------
    def pops( self, s = None, s1 = None , s2 = None,
              path = None , lib = None ,
              do_edger = True ,
              no_filter = False ,
              do_reref = False ,
-             m = None , m1 = None , m2 = None ):
+             m = None , m1 = None , m2 = None ,
+             lights_off = '.' , lights_on = '.' ,
+             ignore_obs = False, 
+             args = '' ):
       """Run the POPS stager"""
 
       if path == None: path = resources.POPS_PATH
       if lib == None: lib = resources.POPS_LIB
       
       import os
       if not os.path.isdir( path ):         
@@ -596,25 +741,37 @@
          
       # set options
       self.ivar( 'mpath' , path )
       self.ivar( 'lib' , lib )
       self.ivar( 'do_edger' , '1' if do_edger else '0' )
       self.ivar( 'do_reref' , '1' if do_reref else '0' )
       self.ivar( 'no_filter' , '1' if no_filter else '0' )
+      self.ivar( 'LOFF' , lights_off )
+      self.ivar( 'LON' , lights_on )
+
       if s != None: self.ivar( 's' , s )
       if m != None: self.ivar( 'm' , m )
       if s1 != None: self.ivar( 's1' , s1 )
       if s2 != None: self.ivar( 's2' , s2 )
       if m1 != None: self.ivar( 'm1' , m1 )
       if m2 != None: self.ivar( 'm2' , m2 )
       
       # get either one- or two-channel mode Luna script from POPS folder
       twoch = s1 != None and s2 != None;
       if twoch: cmdstr = cmdfile( path + '/s2.ch2.txt' )
       else: cmdstr = cmdfile( path + '/s2.ch1.txt' )
+
+      # swap in any additional options to POPS
+      if ignore_obs is True:
+         args = args + ' ignore-obs-staging';
+         if do_edger is True:
+            cmdstr = cmdstr.replace( 'EDGER' , 'EDGER all' )
+      if args != '':
+         cmdstr = cmdstr.replace( 'POPS' , 'POPS ' + args + ' ')
+      
       
       # run the command
       self.proc( cmdstr )
 
       # return of results
       return self.table( 'POPS' , 'E' )
 
@@ -635,22 +792,85 @@
       self.ivar( 'th' , str(th) )
       self.eval( cmdfile( resources.MODEL_PATH + '/m1-adult-age-luna.txt' ) )
       return self.table( 'PREDICT' )
 
    # --------------------------------------------------------------------------------   
    def stages(self):
       """Return of a list of stages"""   
+      hyp = self.silent_proc( "STAGE" )
+      if type(hyp) is type(None): return
+      if 'STAGE: E' in hyp:
+         return hyp[ 'STAGE: E' ]
+      return
+
+   # --------------------------------------------------------------------------------   
+   def hypno(self):
+      """Hypnogram of sleep stages"""
+      if self.has_staging() is not True:
+         print( "no staging attached" )
+         return
+      return hypno( self.stages()[ 'STAGE' ] )
+
+   # --------------------------------------------------------------------------------
+   def has_staging(self):
+      """Returns boolean for whether staging is present"""
       _proj = proj(False)
       silence_mode = _proj.is_silenced()
       _proj.silence(True,False)
-      hyp = self.proc( "STAGE" )[ 'STAGE: E' ]
+      res = self.edf.has_staging()
       _proj.silence( silence_mode , False )
-      return hyp
+      return res
 
-   
+   # --------------------------------------------------------------------------------
+   def has_annots(self,anns):
+      """Returns boolean for which annotations are present"""
+      if anns == None: return
+      if type( anns ) is not list: anns = [ anns ]
+      return self.edf.has_annots( anns )
+
+   # --------------------------------------------------------------------------------
+   def has_annot(self,anns):
+      """Returns boolean for which annotations are present"""
+      return self.has_annots(anns)
+
+   # --------------------------------------------------------------------------------
+   def has_channels(self,ch):
+      """Return a boolean to indicate whether a given channel exists"""
+      if ch == None: return
+      if type(ch) is not list: ch = [ ch ]
+      return self.edf.has_channels( ch )
+
+   # --------------------------------------------------------------------------------
+   def has(self,ch):
+      """Return a boolean to indicate whether a given channel exists"""
+      if ch == None: return
+      if type(ch) is not list: ch = [ ch ]
+      return self.edf.has_channels( ch )
+
+   # --------------------------------------------------------------------------------                                                                  
+   def spec(self,ch,mine = None , maxe = None , minf = None, maxf = None, w = 0.025 ):
+      """PSD given channel 'ch'"""
+      if type( ch ) is not str:
+         return
+      if all( self.has( ch ) ) is not True:
+         return
+      res = self.silent_proc( "PSD epoch-spectrum dB sig="+ch )[ 'PSD: CH_E_F' ]
+      return spec( res , ch=ch, var='PSD', mine=mine,maxe=maxe,minf=minf,maxf=maxf,w=w)
+
+   # --------------------------------------------------------------------------------
+   def psd(self, ch, minf = None, maxf = None, minp = None, maxp = None , xlines = None , ylines = None ):
+      """Spectrogram plot for a given channel 'ch'"""
+      if type( ch ) is not str:
+         return
+      if all( self.has( ch ) ) is not True:
+         return
+      res = self.silent_proc( "PSD spectrum dB sig="+ch )[ 'PSD: CH_F' ]
+      return psd( res , ch, minf = minf, maxf = maxf, minp = minp, maxp = maxp , xlines = xlines , ylines = ylines )
+
+      
 # --------------------------------------------------------------------------------
 #
 # misc non-member utilities functions
 #
 # --------------------------------------------------------------------------------
 
 
@@ -849,18 +1069,48 @@
    ax.set_ylabel('Prob(stage)')
    ax.stackplot(x, y.T , colors = stgcol([ 'N1','N2','N3','R','W']) )
    ax.set(xlim=(1, ne), xticks=[ 1 , ne ] , 
           ylim=(0, 1), yticks=np.arange(0, 1))                                                                                             
    plt.show()
 
 
+
+
 # --------------------------------------------------------------------------------
-# TODO: stage duration plot
-# TODO: NREM cycle plot
-# TODO: overview of hypnogram plot
+def psd(df , ch, var = 'PSD' , minf = None, maxf = None, minp = None, maxp = None , 
+        xlines = None , ylines = None, dB = False ):
+    """Returns a PSD plot from PSD or MTM epoch table (CH_F)"""
+    if ch == None: return
+    if type( ch ) is not list: ch = [ ch ]
+    if type( xlines ) is not list and xlines != None: xlines = [ xlines ]
+    if type( ylines ) is not list and ylines != None: ylines = [ ylines ]
+    df = df[ df['CH'].isin(ch) ]
+    if len(df) == 0: return
+    f = df['F'].to_numpy(dtype=float)
+    p = df[var].to_numpy(dtype=float)
+    if dB is True: p = 10*np.log10(p)
+    cx = df['CH'].to_numpy(dtype=str)
+    if minp == None: minp = min(p)
+    if maxp == None: maxp = max(p)
+    if minf == None: minf = min(f)
+    if maxf == None: maxf = max(f)
+    incl = np.zeros(len(df), dtype=bool)
+    incl[ (f >= minf) & (f <= maxf) ] = True
+    f = f[ incl ]
+    p = p[ incl ]
+    cx = cx[ incl ] 
+    p[ p > maxp ] = maxp
+    p[ p < minp ] = minp
+    [ plt.plot(f[ cx == _ch ], p[ cx == _ch ] , label = _ch ) for _ch in ch ]
+    plt.legend()
+    plt.xlabel('Frequency (Hz)')
+    plt.ylabel('Power (dB)')
+    if xlines != None: [plt.axvline(_x, linewidth=1, color='gray') for _x in xlines ]
+    if ylines != None: [plt.axhline(_y, linewidth=1, color='gray') for _y in ylines ]
+    plt.show()
 
 
 # --------------------------------------------------------------------------------
 def spec(df , ch = None , var = 'PSD' , mine = None , maxe = None , minf = None, maxf = None, w = 0.025 ):
     """Returns a spectrogram from a PSD or MTM epoch table (CH_E_F)"""
     if ch != None: df = df.loc[ df['CH'] == ch ]
     if len(df) == 0: return
@@ -877,21 +1127,23 @@
     y = y[ incl ]
     z = z[ incl ]
     z = winsorize( z , limits=[w, w] )
 
     #include/exclude here...
     spec0( x,y,z,mine,maxe,minf,maxf)
 
+    
 # --------------------------------------------------------------------------------
 def spec0( x , y , z , mine , maxe , minf, maxf ):
    xn = max(x) - min(x) + 1
    yn = np.unique(y).size
    zi, yi, xi = np.histogram2d(y, x, bins=(yn,xn), weights=z, density=False )
-   counts, _, _ = np.histogram2d(y, x, bins=(yn,xn))
-   zi = zi / counts
+   counts, _, _ = np.histogram2d(y, x, bins=(yn,xn))   
+   with np.errstate(divide='ignore', invalid='ignore'):
+      zi = zi / counts
    zi = np.ma.masked_invalid(zi)
    fig, ax = plt.subplots()
    fig.set_figheight(2)
    fig.set_figwidth(15)
    ax.set_xlabel('Epoch')
    ax.set_ylabel('Frequency (Hz)')
    ax.set(xlim=(mine, maxe), ylim=(minf,maxf) )
```

## Comparing `lunapi-0.0.5.dist-info/METADATA` & `lunapi-0.0.6.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lunapi
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python interface to the Luna toolset for sleep signal analysis
-Keywords: Sleep EEG PSG Luna Signal processing
+Keywords: Sleep,EEG,PSG,Luna,Signal processing
 Author-Email: Shaun Purcell <smpurcell@bwh.harvard.edu>, Senthil Palanivelu <spalanivelu@mgh.harvard.edu>, Nataliia Kozhemiako <nkozhemiako@bwh.harvard.edu>
 Maintainer-Email: Senthil Palanivelu <spalanivelu@mgh.harvard.edu>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Framework :: Jupyter :: JupyterLab
@@ -22,12 +22,11 @@
 Requires-Python: >=3.8
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: IPython
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # lunapi
 
 Python bindings for C/C++ Luna library
```

## Comparing `lunapi-0.0.5.dist-info/licenses/LICENSE` & `lunapi-0.0.6.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

