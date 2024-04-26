# Comparing `tmp/sleep-utils-1.15.tar.gz` & `tmp/sleep-utils-1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleep-utils-1.15.tar", last modified: Thu Nov 24 10:48:28 2022, max compression
+gzip compressed data, was "sleep-utils-1.16.tar", last modified: Fri Apr 26 14:46:48 2024, max compression
```

## Comparing `sleep-utils-1.15.tar` & `sleep-utils-1.16.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:48:28.127502 sleep-utils-1.15/
--rw-r--r--   0 runner    (1001) docker     (122)     2111 2022-11-24 10:48:28.127502 sleep-utils-1.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1686 2022-11-24 10:47:23.000000 sleep-utils-1.15/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-24 10:48:28.127502 sleep-utils-1.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      763 2022-11-24 10:47:23.000000 sleep-utils-1.15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:48:28.127502 sleep-utils-1.15/sleep_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      441 2022-11-24 10:47:23.000000 sleep-utils-1.15/sleep_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16151 2022-11-24 10:47:23.000000 sleep-utils-1.15/sleep_utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (122)    28415 2022-11-24 10:47:23.000000 sleep-utils-1.15/sleep_utils/sigproc.py
--rw-r--r--   0 runner    (1001) docker     (122)    20933 2022-11-24 10:47:23.000000 sleep-utils-1.15/sleep_utils/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:48:28.127502 sleep-utils-1.15/sleep_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2111 2022-11-24 10:48:28.000000 sleep-utils-1.15/sleep_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      318 2022-11-24 10:48:28.000000 sleep-utils-1.15/sleep_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 10:48:28.000000 sleep-utils-1.15/sleep_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 10:48:26.000000 sleep-utils-1.15/sleep_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       43 2022-11-24 10:48:28.000000 sleep-utils-1.15/sleep_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2022-11-24 10:48:28.000000 sleep-utils-1.15/sleep_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:46:48.626163 sleep-utils-1.16/
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-26 14:46:48.626163 sleep-utils-1.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-26 14:46:18.000000 sleep-utils-1.16/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 14:46:48.626163 sleep-utils-1.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-26 14:46:18.000000 sleep-utils-1.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:46:48.626163 sleep-utils-1.16/sleep_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-26 14:46:18.000000 sleep-utils-1.16/sleep_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24935 2024-04-26 14:46:18.000000 sleep-utils-1.16/sleep_utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29136 2024-04-26 14:46:18.000000 sleep-utils-1.16/sleep_utils/sigproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21785 2024-04-26 14:46:18.000000 sleep-utils-1.16/sleep_utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-04-26 14:46:18.000000 sleep-utils-1.16/sleep_utils/usleep_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:46:48.626163 sleep-utils-1.16/sleep_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-26 14:46:48.000000 sleep-utils-1.16/sleep_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-26 14:46:48.000000 sleep-utils-1.16/sleep_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:46:48.000000 sleep-utils-1.16/sleep_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:46:47.000000 sleep-utils-1.16/sleep_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-26 14:46:48.000000 sleep-utils-1.16/sleep_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 14:46:48.000000 sleep-utils-1.16/sleep_utils.egg-info/top_level.txt
```

### Comparing `sleep-utils-1.15/PKG-INFO` & `sleep-utils-1.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleep-utils
-Version: 1.15
+Version: 1.16
 Summary: A collection of tools for sleep research
 Home-page: http://github.com/skjerns/sleep-utils
 Author: skjerns
 Author-email: nomail@nomail.com
 License: GNU 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sleep-utils-1.15/README.md` & `sleep-utils-1.16/README.md`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-# sleep-utils
-
-A python toolbox for sleep researchers. Plot hypnograms, spectrograms, confusion matrices, PSG summaries
-
-<img src="./assets/d1f7592a94f0f39c4d672c5913e161ec16193458.png" title="" alt="sample_hypnogram.png" width="394">
-
-<img src="./assets/c49446ae6d84dee6e13ae14034dd12eb6bbdb48d.png" title="" alt="spectrogram_multitaper.png" width="395">
-
-<img src="md_assets/2022-07-25-13-06-18-image.png" title="" alt="" width="409">
-
-```
-Hypnogram summary
-{'TRT': 460.5,
- 'TST': 444.5,
- 'WASO': 16.0,
- 'lat_REM': 65.0,
- 'lat_S1': 0.0,
- 'lat_S2': 2.0,
- 'lat_S3': 9.0,
- 'min_REM': 109.5,
- 'min_S1': 13.5,
- 'min_S2': 214.0,
- 'min_S3': 107.5,
- 'perc_REM': 0.24634420697412823,
- 'perc_S1': 0.030371203599550055,
- 'perc_S2': 0.4814398200224972,
- 'perc_S3': 0.24184476940382452,
- 'perc_W': 0.03474484256243214,
- 'recording_length': 547.0,
- 'sleep_offset_after_rec_start': 534.0,
- 'sleep_onset_after_rec_start': 73.5}
-```
-
-#### Install
-
-```
-pip install sleep-utils
-```
-
-or
-
-```
-pip install git+https://github.com/skjerns/sleep-utils
-```
-
-#### Functionality
-
-`import sleep_utils`
-
-- hypnograms
-  
-  - load (`sleep_utils.read_hypno(file)`)
-  
-  - save(`sleep_utils.write_hypno(hypno, file)`
-  
-  - plot (`sleep_utils.plot_hypnogram(hypno)`)
-  
-  - convert (read&save)
-  
-  - print summary (TST, WASO, ...) (`sleep_utils.hypno_summary(hypno)`)
-
-- spectrograms
-  
-  - multitaper spectrogram (`sleep_utils.specgram_multitaper(data, sfreq)`)
-  
-  - welch spectrogram(`sleep_utils.specgram_welch(data, sfreq)`)
-
-- confusion matrix
-  
-  - plot inter rater confusion matrix (`sleep_utils.plot_confusion_matrix(confmat)`)
-
-- mne-edf
-  
+# sleep-utils
+
+A python toolbox for sleep researchers. Plot hypnograms, spectrograms, confusion matrices, PSG summaries
+
+<img src="./assets/d1f7592a94f0f39c4d672c5913e161ec16193458.png" title="" alt="sample_hypnogram.png" width="394">
+
+<img src="./assets/c49446ae6d84dee6e13ae14034dd12eb6bbdb48d.png" title="" alt="spectrogram_multitaper.png" width="395">
+
+<img src="md_assets/2022-07-25-13-06-18-image.png" title="" alt="" width="409">
+
+```
+Hypnogram summary
+{'TRT': 460.5,
+ 'TST': 444.5,
+ 'WASO': 16.0,
+ 'lat_REM': 65.0,
+ 'lat_S1': 0.0,
+ 'lat_S2': 2.0,
+ 'lat_S3': 9.0,
+ 'min_REM': 109.5,
+ 'min_S1': 13.5,
+ 'min_S2': 214.0,
+ 'min_S3': 107.5,
+ 'perc_REM': 0.24634420697412823,
+ 'perc_S1': 0.030371203599550055,
+ 'perc_S2': 0.4814398200224972,
+ 'perc_S3': 0.24184476940382452,
+ 'perc_W': 0.03474484256243214,
+ 'recording_length': 547.0,
+ 'sleep_offset_after_rec_start': 534.0,
+ 'sleep_onset_after_rec_start': 73.5}
+```
+
+#### Install
+
+```
+pip install sleep-utils
+```
+
+or
+
+```
+pip install git+https://github.com/skjerns/sleep-utils
+```
+
+#### Functionality
+
+`import sleep_utils`
+
+- hypnograms
+  
+  - load (`sleep_utils.read_hypno(file)`)
+  
+  - save(`sleep_utils.write_hypno(hypno, file)`
+  
+  - plot (`sleep_utils.plot_hypnogram(hypno)`)
+  
+  - convert (read&save)
+  
+  - print summary (TST, WASO, ...) (`sleep_utils.hypno_summary(hypno)`)
+
+- spectrograms
+  
+  - multitaper spectrogram (`sleep_utils.specgram_multitaper(data, sfreq)`)
+  
+  - welch spectrogram(`sleep_utils.specgram_welch(data, sfreq)`)
+
+- confusion matrix
+  
+  - plot inter rater confusion matrix (`sleep_utils.plot_confusion_matrix(confmat)`)
+
+- mne-edf
+  
   - save MNE to edf (`sleep_utils.write_mne_edf(raw, filename)`)
```

### Comparing `sleep-utils-1.15/sleep_utils/sigproc.py` & `sleep-utils-1.16/sleep_utils/sigproc.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,722 +1,722 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Oct 24 09:47:39 2018
-@author: SimonKern
-"""
-import mne
-import warnings
-import scipy
-import numpy as np
-from PIL import Image
-from scipy.signal import correlate, get_window, iirnotch
-from scipy.signal import butter, lfilter, convolve2d, welch, hilbert
-from scipy.stats import zscore
-
-
-# window types used as tapers without parameters
-WTYPES = ['boxcar', 'triang', 'blackman', 'hamming', 'hann', 'bartlett', 
-         'flattop', 'parzen', 'bohman', 'blackmanharris', 'nuttall',
-         'barthann']
-
-###### Begin of functions
-
-
-def dig2phys(signal, dmin, dmax, pmin, pmax):
-    """converts digital to analogue signals"""
-    m = (pmax-pmin) / (dmax-dmin)
-    physical = m * signal
-    return physical
-
-def phys2dig(signal, dmin, dmax, pmin, pmax):
-   """converts analogue to digital signals"""
-   m = (dmax-dmin)/(pmax-pmin) 
-   digital = (m * signal).astype(np.int, copy=False)
-   return digital
-
-
-def rfft_mag(signals):
-    """
-    Returns the magnitude of the fft of a signal: sqrt(real^2+imag^2)
-    Will return only the real part of frequencies (arraylength//2), see rfft
-   
-    :param signals: 1D or 2D array
-    :returns: the magnitude of the frequencies in the signal
-    """
-
-    w = rfft(signals) 
-    mag = np.abs(w) # same as np.abs(w)
-    return mag
-
-
-def rfft(signals, *args, **kwargs):
-    """
-    wrapper for rFFT, mainly for checking differences of Python and C
-    Input should be of length power of 2 for optimization purposes.
-    Returns the arraylength // 2 (unlike rfft, which does weird wlen//2 +1)
-    
-    :param signals: a 1D or 2D signal, where each row contains one window of data
-    :returns: complex array of fft results, 
-              Note: in JSON I save a complex array as two lists with real and imaginary part
-    """
-    if not isinstance(signals, np.ndarray): 
-        signals = np.asarray(signals)    
-    wlen = signals.shape[-1]
-    if not ((wlen & (wlen - 1)) == 0): 
-        warnings.warn('Input array should have length power of 2 for fft, but is: {}'.format(wlen))
-    w = scipy.fftpack.fft(signals)[...,:signals.shape[-1]//2]
-    assert w.shape[-1] == signals.shape[-1]//2, 'w.shape = {}'.format(w.shape)
-    return w
-
-
-
-
-def abs2(x):
-    """highly optimized version for magnitude taking.
-       if there are problems, just remove the decorator line @numba.vectorize(...)
-       if working with float32, need to change signature to inlcude ,numba.float32(numba.complex64)
-    """
-    return x.real**2 + x.imag**2
-
-
-def welchs(signals, nperseg=None, overlap=0.0, taper_name='boxcar'):
-    """
-    A minimal implementation of Welch's method, optimized ~10x faster than previously, 
-    even faster than scipy.signal.welch().
-    This is also equivalent to the normal rfft(), if used with standard parameters
-    
-    If nperseg=0 we have a standard fft.
-    If nperseg>0 and overlap=0 we have Barlett's methd
-    If nperseg>0 and overlap>0 we have Welch's method (use a taper in this case)
-        
-    :param signals: The signals on which to perform Welchs (1D or 2D)
-    :param nperseg: How many samples per segment for the calculation of the FFT
-    :param overlap: How many samples should overlap between segments (int or float)
-                    if float: is interpreted as ratio of nperseg
-                    eg overlap 0.5 = 0.5*nperseg
-    :param taper_name: Which taper to use, if overlap>0, it is recommended to use a taper
-    :returns: The Welch's frequency estimate of the signal as magnitudes
-    """
-    from sklearn import feature_extraction
-
-    signals = np.atleast_2d(signals)
-    siglen = signals.shape[-1]
-    
-    if nperseg is None: nperseg = siglen
-    if isinstance(overlap, float): overlap = overlap*nperseg
-    if siglen%nperseg!=0: warnings.warn('window length should be a multiple of npseg')
-
-    # get window only once, else it will be created for each segment, swallowing computation
-    taper = get_window(taper_name, nperseg, False).astype(int) if taper_name not in ['boxcar', None] else None
-    
-    # this step we have to take to get to the next segment
-    step = int(nperseg - overlap)
-    n_segments    = (siglen-nperseg)//step +1
-    
-    # fastest way to extract patches using np.lib.stride_tricks.as_strided via sklearn
-    fft_segments = feature_extraction.image.extract_patches(signals, patch_shape=(len(signals),nperseg), extraction_step=step)
-    fft_segments = fft_segments.reshape([n_segments, len(signals), nperseg])
-    fft_segments = np.swapaxes(fft_segments, 0,1)
-
-    # apply taper
-    if taper is not None:
-        fft_segments  = np.multiply(fft_segments, taper)
-        
-    # apply fft and take squared magnitude
-    w = rfft(fft_segments)
-    w_mag = abs2(w)
-    fft_result = np.mean(w_mag, axis=1)
-    return fft_result
-
-
-def welchs_unoptimized(signals, nperseg=None, overlap=0.0, taper_name='boxcar'):
-    """
-    A minimal implementation of Welch's method, unoptimized, should be equivalent to welchs()
-    It's kept here for archive purposes and for C-compatibility, also to check 
-    the optimized version in case of changes.
-    
-    If nperseg=0 we have a standard fft.
-    If nperseg>0 and overlap=0 we have Barlett's methd
-    If nperseg>0 and overlap>0 we have Welch's method (use a taper in this case)
-    
-    :param signals: The signals on which to perform Welchs (1D or 2D)
-    :param nperseg: How many samples per segment for the calculation of the FFT
-    :param overlap: How many samples should overlap between segments (int or float)
-                    if float: is interpreted as ratio of nperseg
-                    eg overlap 0.5 = 0.5*nperseg
-    :param taper_name: Which taper to use, if overlap>0, it is recommended to use a taper
-    :returns: The Welch's frequency estimate of the signal as magnitudes
-    """
-    signals = np.atleast_2d(signals)
-    
-    siglen = signals.shape[-1]
-    if nperseg is None: nperseg = siglen
-    if isinstance(overlap, float): overlap = overlap*nperseg
-    if siglen%nperseg!=0: warnings.warn('window length should be a multiple of npseg')
-
-    step = int(nperseg - overlap) # distance between windows that we extract
-    n_segments = (siglen-nperseg)//step + 1 # this is how many windows we can extract from the signal
-    fft_signals = []
-    # loop through the signals (in C you can start at the second loop as we only have 1D arrays)
-    for sig in signals:
-        # collect one fft result per segment
-        # in fft_mean we save a running mean of the fft segments
-        fft_mean = np.zeros(nperseg//2) 
-        # loop through the signal in step sizes that allow for overlap
-        for i in range(0, siglen, step):
-            # only take full segments
-            if i+nperseg>siglen: 
-                break 
-            # extract segment
-            segment = sig[i:i+nperseg]
-            # taper segment if necessary
-            if taper_name is not None:
-                segment = taper(segment, taper_name)
-            # take FFT and add to fft results for segments
-            w = rfft(segment)
-            # this is the same as saving all segments and taking a mean later,
-            # but prevents us from having to keep intermediate results
-            fft_mean += (np.abs(w)**2) / n_segments 
-        # take the mean spectral values for all segments
-        fft_signals.append(fft_mean)
-    return np.array(fft_signals)
-
-
-def moving_average(signals, N):
-    signals = np.atleast_2d(signals).astype(dtype=int, copy=False)
-    return convolve2d(signals, np.ones((1, N))/N, mode='valid')
-    
-
-def binnedmean(signals, target_size=None, bin_edges=None, func=None):
-    """
-    cuts a signal in n parts, applies a function to each part (e.g. mean)
-    this way we can go from an array of length M to an array of length N<M
-    by taking the mean of the elemts of each part, where the number of parts is N
-        
-    :param target_size: The number of bins that we should interpolate to
-    :bin_edges: custom bin edges, if targed size is not present. Bin edges is a list of tuples
-                each tuple represents the edges of the bin [inc, excl].
-    :func: a function that should be applied, standard is mean. 
-           this function needs to operate only on the first dimension
-    """
-    # we only deal with 2D data in the given DTYPE
-    signals = np.atleast_2d(signals)
-
-    assert signals.ndim<3
-    # signal length
-    slen = signals.shape[1]
-    # if there are no bin edges provided, we are creating the bin edges
-    # using the target_size.
-    # that means, we create target_size bins, that are equally spaced
-    # around the signal
-    if bin_edges is None and target_size is not None:
-        bin_edges = np.linspace(0, slen, target_size+1, dtype=np.int)
-        bin_edges = np.repeat(bin_edges,2)[1:-1]
-        bin_edges = bin_edges.reshape([-1,2])
-    # if no function is provided, we take the mean of each bin
-    if func is None:
-        func = lambda s: np.mean(s, axis=1)
-    
-    new_array = np.zeros([signals.shape[0], len(bin_edges)])
-    
-    # now we run over the original array and always take all values of each bin
-    # in the original signal. then we apply the function
-    # that is provided on that bin and write the result to a new array
-    for i, [e1,e2] in enumerate(bin_edges):
-        bin_entries = signals[:,e1:e2]
-        reduced = func(bin_entries)
-        new_array[:,i] = reduced
-        
-    return new_array
-   
-
-def bands2bins(bands, window_len, sfreq):    
-    """
-    A function that turns frequency bands into bin-edges to be used to extract these bands
-    from a fft function
-    
-    :param bands: a list of 2-tuples, each 2-tuple containing a frequency lower and upper bound
-    :param window_len: the length of the window that the FFT will be applied to
-    :param sfreq: the sampling frequency of the signal
-    """
-    sfreq = int(sfreq)
-    window_len=int(window_len)
-    round2=lambda x,y=None: round(x+1e-15,y)
-    bins = []
-    for l,h in bands:
-        bin_lower = int(round2(l*window_len/sfreq)) # np.floor rounds down
-        bin_upper = int(round2(h*window_len/sfreq))  # np.ceil rounds up
-        bins.append([bin_lower, bin_upper])
-    return bins
-
-
-def create_specband_bin_edges(window_len=None, sfreq=None):
-    """
-    Given a FFT-window length and a sampling frequency, 
-    compute the bin edges for common brain frequencies
-    :param window_len: length in sample numbers, if None, will just return bands and not bins
-    :param sfreq: sampling frequency, if None, will just return bands and not bins
-    :returns: edges for [slowos, delta, theta, alpha1, spindle, beta1, beta2, gamma]
-    
-    BRAIN_BAND_NAMES_ = ['so', 'delta', 'theta', 'alpha1', 'alpha2', 'beta1', 'beta2', 'gamma']
-    
-    """
-    if sfreq is None: sfreq=window_len
-    
-    slowos   = [0, 1]
-    delta   = [1, 4]
-    theta   = [4, 8]
-    alpha1  = [8, 10]
-    spindle = [10, 14]
-    beta1   = [13, 16]
-    beta2   = [16, 20]
-    gamma   = [20, 35]
-    
-    # this is the order of the bands
-    # result is a list of tuples, where each tuple is the bin edge
-    bands = [slowos, delta, theta, alpha1, spindle, beta1, beta2, gamma]
-    if window_len is None and sfreq is None: return bands
-    # calculate the bin positions corresponding to frequency edges
-    bins = bands2bins(bands, window_len, sfreq)
-    return bins # this is a list of tuples, e.g. [(0,30),(30,60),(60,120)]
-
-     
-
-def taper(signals, window_name):
-    """
-    filters/tapers given signals or signal with a window with window-name. allowed names are:
-        ['boxcar', 'triang', 'blackman', 'hamming', 'hann', 'bartlett',
-        'flattop', 'parzen', 'bohman', 'blackmanharris', 'nuttall',
-        'barthann'] 
-                
-    :param signals: A 1D signals or a 2D array with signals x samples
-    :param window_name: the name of the taper
-    :returns: the tapered signals
-    """  
-    if window_name in [None, '', 'boxcar']: return signals
-    if window_name.lower() not in ['hamming', 'hann', 'blackman', 'blackmanharris']:
-        warnings.warn('Up to this point, this window is not tested in C code: {}.'.format(window_name))
-    if isinstance(signals, list): signals = np.array(signals)
-    assert signals.ndim in [1,2], 'signals must be 1D or 2D'
-    # how long is the signal?
-    wlen = signals.shape[0] if signals.ndim==1 else signals.shape[1]
-    # get the window function using scipy
-    window = get_window(window_name, wlen, False)
-    # filter our input signal
-    tapered = signals*window  
-    return tapered
-
-
-def extract_windows(signal, length, distance=1.0, group_n=0, group_d=0, hypno=None, taper_name=None):
-    """
-    From a signal, extract windows every N seconds for a length of L.
-    Can be grouped in groups on group_n, with distance between last samplepoint of one group
-    and the first sample of the next group being group_d.
-    only complete groups will be returned    
-    
-    :param signal: the signal to take windows from
-                   if the signal is 2D, the format signaln x samples is assumed
-    :param length: The length of each window in sample space
-    :param distance: the distance between each windows
-                     if distance is an int, it will be interpreted as a spacing in sample space
-                     if distance is a float, it will be interpreted as relative to the length
-                     e.g. distance=0.5 will produce windows with overlap of 50%
-    :param group_n: how many windows to extract before leaving a space to the next group of windows
-    :param group_d: how much space between batches
-                     if distance is an int, it will be interpreted as a spacing in sample space
-                     if distance is a float, it will be interpreted as relative to the length
-                     e.g. group_d=0.5 will produce windows in groups with distance between groups 
-                     of 50% window length 
-    :param hypno: a hypnogram annotation. It will automatically be inferred what spacing the 
-                  hypnogram uses and what annotation frequency
-    """
-    # pass through if length is None
-    if length is None: 
-        return (signal, hypno)
-    
-    assert (group_n==0 and group_d==0) or (group_n>0 and group_d>0), \
-            'group parameters must both be supplied'
-    assert distance>0, 'distance must be positive'
-    assert length>0, 'length must be positive'
-    if hypno is not None: assert type(hypno) is np.ndarray, 'must be numpy array'
-    assert type(signal) is np.ndarray, 'must be numpy array'
-    
-    siglen = len(signal) if signal.ndim==1 else signal.shape[1]
-    distance = distance if type(distance) is int else int(distance*length)
-    group_d  = group_d if type(group_d) is int else int(group_d*length)
-
-    assert length<=siglen, 'length must be smaller than siglen'
-   
-    if signal.ndim == 1: signal = [signal] # to make the iterator work in 1D case
-    
-    
-    # inefficient implenentation, but makes sure everything is correct
-    
-    all_sigs = []
-    for subsig in signal:
-        i = 0
-        g = 0 # group counter
-        sigs = []
-        while i <= siglen-length:
-            s = subsig[i:i+length]
-            sigs.append(s)
-            i+=distance
-            g+=1
-            if g>=group_n and group_n>0:
-                i+=group_d+length-distance
-                g=0
-        all_sigs.append(np.array(sigs))
-        
-    all_sigs = np.array(all_sigs)
-    if all_sigs.shape[0]==1: all_sigs = all_sigs.reshape(-1, length)
-    
-    # match a new hypnogram to the extracted epochs
-    if hypno is not None:
-        s_per_hypno = siglen/len(hypno)
-        i = 0
-        g = 0 # group counter
-        new_hypno = []
-        while i <= siglen-length:
-            h = hypno[int(i/s_per_hypno)]
-            new_hypno.append(h)
-            i+=distance
-            g+=1
-            if g>=group_n and group_n>0:
-                i+=group_d+length-distance
-                g=0
-    windows   = np.array(all_sigs, copy=False)
-    if taper_name is not None: windows = taper(windows, taper_name)
-    if hypno is not None: new_hypno = np.array(new_hypno, dtype = hypno.dtype) 
-    return windows if hypno is None else (windows, new_hypno)
-
-
-def correlate_specto(signal1, signal2, sfreq):
-    """
-    create a cross-correlation of two signals using the spectogram
-    """
-    
-    sfreq1 = 256
-    sfreq2 = 200
-    n_samples1 = int(sfreq1)
-    n_samples2 = int(sfreq2)
-    
-    # get fft results 
-    signal1_trunc = signal1[:int((len(signal1)//n_samples1)*(n_samples1))].reshape([-1,n_samples1])
-    signal2_trunc = signal2[:int((len(signal2)//n_samples2)*(n_samples2))].reshape([-1,n_samples2])
-    
-    # get FFT via Welchs
-    freq1, spec1 = welch(signal1_trunc, fs=sfreq1, window='boxcar', nperseg=sfreq1, noverlap=0)
-    freq2, spec2 = welch(signal2_trunc, fs=sfreq2, window='boxcar', nperseg=sfreq2, noverlap=0)
-    
-    # truncate from 2 to 15 Hz
-    spec1 = spec1[:,np.argmax(freq1>2):np.argmax(freq1>15)]
-    spec2 = spec2[:,np.argmax(freq1>2):np.argmax(freq1>15)]
-  
-    # transform to dB
-    spec1 = (np.log10(spec1+1)*20).T
-    spec2 = (np.log10(spec2+1)*20).T
-
-    # make row-wise correlation
-    corr = np.array([correlate(zscore(row1), zscore(row2)) for row1, row2 in zip(spec1,spec2)]).mean(0)
-    return corr
-
-
-def coeff_var_env(signal, sfreq, band=(0.5, 4), mid_sec=30):
-    """Coefficient of the variance of the envelope (CVE) calculation
-    
-    as defined in  https://doi.org/10.1016/j.neuroimage.2018.01.063
-    
-    :param epoch: one epoch of data, 1D data as array
-    :type epoch: np.ndarray
-    :return: CVE of this epoch
-    :rtype: TYPE
-    """
-    sig = np.atleast_2d(signal)
-    sig_filtered = np.atleast_2d(bandfilter(sig, sfreq, *band, method='iir',
-                                            iir_params={'order':4, 
-                                                        'ftype':'butter'}))
-    ht_sig_filtered = np.abs(hilbert(sig_filtered))
-    
-    eeg_envelope = np.sqrt(sig_filtered**2 + ht_sig_filtered**2)
-    
-    t_excess = int(signal.shape[-1] -  mid_sec*sfreq)//2
-    middle_env = eeg_envelope[:, t_excess:-t_excess]
-    assert abs(middle_env.shape[1]-mid_sec*sfreq)<2
-    
-    mean = np.mean(middle_env)
-    sd = np.std(middle_env)
-    
-    cve = sd/(mean*0.523)  # [..] with 0.523 being the value for Gaussian waves
-     
-    return cve
-
-def get_shift_specto(signal1, signal2, sfreq = 256, w_seconds=1, limit_to=1):
-    """
-    a more robust version to align two eeg recordings using fourier transformations
-    accuracy of this method depends on w_seconds
-    
-    
-    :param signal1: a 1D signal
-    :param signal2: a 1D signal
-    :param sfreq: the sampling frequency of the signals
-    :param w_seconds: how many chunks should be used to create the FFT. This determines the accuracy
-    """
-    assert signal1.ndim==1
-    assert signal2.ndim==1
-    assert np.all([len(signal1)>sfreq*60*5]), 'need at least 5 minutes of data'
-    if len(signal1)>len(signal2)*2: 
-        warnings.warn('signal1 is significantly larger than signal2: \
-                      is the sampling frequency the same?')
-    if len(signal2)>len(signal1)*2: 
-        warnings.warn('signal2 is significantly larger than signal1: \
-                      is the sampling frequency the same?')
-    
-    n_samples = int(w_seconds*sfreq)
-    
-    # get fft results 
-    signal1_trunc = signal1[:int((len(signal1)//n_samples)*(n_samples))].reshape([-1,n_samples])
-    signal2_trunc = signal2[:int((len(signal2)//n_samples)*(n_samples))].reshape([-1,n_samples])
-    
-    # get FFT via Welchs
-    freq1, spec1 = welch(signal1_trunc, fs=sfreq, window='blackmanharris', nperseg=sfreq, noverlap=0.667*sfreq)
-    freq2, spec2 = welch(signal2_trunc, fs=sfreq, window='blackmanharris', nperseg=sfreq, noverlap=0.667*sfreq)
-    
-    # truncate from 2 to 15 Hz
-    spec1 = spec1[:,np.argmax(freq1>2):np.argmax(freq1>15)]
-    spec2 = spec2[:,np.argmax(freq1>2):np.argmax(freq1>15)]
-  
-    # transform to dB
-    spec1 = (np.log10(spec1+1)*20).T
-    spec2 = (np.log10(spec2+1)*20).T
-
-    # make row-wise correlation
-    corr = np.array([correlate(zscore(row1), zscore(row2)) for row1, row2 in zip(spec1,spec2)]).mean(0)
-    half = len(corr)-spec1.shape[1]
-    corr[:int(half-sfreq*60**2*limit_to//n_samples)] = 0
-    corr[int(half+sfreq*60**2*limit_to//n_samples):] = 0
-    peak = corr.argmax()
-    shift = (len(corr)-spec1.shape[1]- peak) * n_samples
-    return -shift
-
-
-def get_shift_spindle(signal1, signal2, sfreq, limit_to=1):
-    """
-    Taking two frontal channels, will try to recover the shift
-    via aligning the spindle band. This should filter out a lot
-    of other non-related noise and be quite robust for sleep recordings
-    
-    Shift will be searched for within 1h of the recording start
-    
-    :param signal1: a 1D signal
-    :param signal2: a 1D signal
-    :param limit_to: limit to +- this hour
-    """
-    assert signal1.ndim==1
-    assert signal2.ndim==1
-    if len(signal1)>len(signal2)*2: 
-        warnings.warn('signal1 is significantly larger than signal2: \
-                      is the sampling frequency the same?')
-    if len(signal2)>len(signal1)*2: 
-        warnings.warn('signal2 is significantly larger than signal1: \
-                      is the sampling frequency the same?')
-        
-    sigma1 = butter_bandpass_filter(signal1/signal1.max(), 7, 14, sfreq, 5)
-    sigma2 = butter_bandpass_filter(signal2/signal2.max(), 7, 14, sfreq, 5)
-    
-    corr = correlate(sigma1, sigma2)
-    # sometimes there are some weird correlations if the signals are shifted
-    # extremely. We assume that the recording alignment must lie within 
-    # 1 h of either recording start
-    half = len(corr)//2
-    corr[:half-sfreq*60**2*limit_to] = 0
-    corr[half+sfreq*60**2*limit_to:] = 0
-    peak = corr.argmax()
-    shift = len(signal2) - peak -1 
-    print(shift/sfreq, ' seconds')
-#    plt.plot(corr)
-    return -shift    
-
-
-    
-def get_shift(signal1, signal2, sfreq, limit_to=1):
-    """
-    find the shift of signal1 to signal2, used for aligning two signals
-    
-    Data must have the same sampling frequency
-    
-    The output will be how much we need to roll signal2 to match signal1
-    np.roll(signal2, shift)
-    
-    :param signal1: a 1D signal
-    :param signal2: a 1D signal
-    """
-    assert signal1.ndim==1
-    assert signal2.ndim==1
-    if len(signal1)>len(signal2)*2: 
-        warnings.warn('signal1 is significantly larger than signal2: \
-                      is the sampling frequency the same?')
-    if len(signal2)>len(signal1)*2: 
-        warnings.warn('signal2 is significantly larger than signal1: \
-                      is the sampling frequency the same?')
-    if signal1.max()>10: signal1 = zscore(signal1, axis=None)
-    if signal2.max()>10: signal2 = zscore(signal2, axis=None)
-    
-    signal1 = butter_bandpass_filter(signal1/signal1.max(), 1, 30, sfreq, 5)
-    signal2 = butter_bandpass_filter(signal2/signal2.max(), 1, 30, sfreq, 5)
-    
-    corr = correlate(signal1, signal2)
-    half = len(corr)//2
-    corr[:half-sfreq*60**2*limit_to] = 0
-    corr[half+sfreq*60**2*limit_to:] = 0
-    peak = corr.argmax()
-    shift = len(signal2) - peak -1 
-    return -shift
-
-def get_correlation(signal1, signal2, sfreq, llim=2, ulim=20):
-    """
-    find the shift of signal1 to signal2, used for aligning two signals
-    
-    Data must have the same sampling frequency
-    
-    The output will be how much we need to roll signal2 to match signal1
-    np.roll(signal2, shift)
-    
-    :param signal1: a 1D signal
-    :param signal2: a 1D signal
-    """
-    assert signal1.ndim==1
-    assert signal2.ndim==1
-    if len(signal1)>len(signal2)*2: 
-        warnings.warn('signal1 is significantly larger than signal2: \
-                      is the sampling frequency the same?')
-    if len(signal2)>len(signal1)*2: 
-        warnings.warn('signal2 is significantly larger than signal1: \
-                      is the sampling frequency the same?')
-    if signal1.max()>10: signal1 = zscore(signal1, axis=None)
-    if signal2.max()>10: signal2 = zscore(signal2, axis=None)
-    
-    signal1 = butter_bandpass_filter(signal1, 0.1, 30, sfreq, 5)
-    signal2 = butter_bandpass_filter(signal2, 0.1, 30, sfreq, 5)
-    
-    corr = correlate(np.abs(signal1), np.abs(signal2))
-    return corr
-
-
-def resample(data, o_sfreq, t_sfreq):
-    """
-    resample a signal using MNE resample functions
-    This automatically is optimized for EEG applying filters etc
-    
-    :param raw:     a 1D data array
-    :param o_sfreq: the original sampling frequency
-    :param t_sfreq: the target sampling frequency
-    :returns: the resampled signal
-    """
-    if o_sfreq==t_sfreq: return data
-    raw = np.atleast_2d(data)
-    n_jobs = min(len(raw), 8)
-    ch_names=['ch{}'.format(i) for i in range(len(raw))]
-    info = mne.create_info(ch_names=ch_names, sfreq=o_sfreq, ch_types=['eeg'])
-    raw_mne = mne.io.RawArray(raw, info, verbose='WARNING')
-    resampled = raw_mne.resample(t_sfreq, n_jobs=n_jobs, verbose='WARNING')
-    new_raw = resampled.get_data().squeeze()
-    return new_raw.astype(raw.dtype, copy=False)
-
-def resize(array, target_size):
-    """
-    Resize a 1D array containing a signal/
-    or a 2D array of several signasl as rows of any type (int/float) 
-    by taking nearest neighbours to fill gaps within the rows
-    
-    :param array: any type of array
-    :param target_size: the target size of the last dimension
-    """
-    array = np.atleast_2d(array)
-    new_array = []
-    for row in array:
-        pil_row = Image.fromarray(row.reshape([1,-1]))
-        pil_resized = pil_row.resize((target_size,1), Image.NEAREST)
-        new_array.append(np.array(pil_resized).squeeze())
-    return np.array(new_array).squeeze()
-    
-    
-
-def bandfilter(data, sfreq, l_freq, h_freq, **kwargs):
-    """Use mne.io.RawArray.filter to create a bandpath filter for this signal
-    
-    Can be either 1D or 2D signal
-    
-    :param raw: the signal
-    :param sfreq: the sampling frequency of the signal
-    :param l_freq: the lower frequency
-    :param h_freq: the higher frequency
-    """
-    assert data.ndim<3, 'Data must be 2D or 1D'
-    ndim = data.ndim
-    data = np.atleast_2d(data)
-    ch_names = [f'ch{i}' for i,_ in enumerate(data)]
-    info = mne.create_info(ch_names=ch_names, sfreq=sfreq, ch_types=['eeg'])
-    raw = mne.io.RawArray(data, info, verbose='WARNING', copy='both')
-    raw = raw.filter(l_freq, h_freq, verbose='WARNING', **kwargs)
-    new_data = raw.get_data()
-    return new_data.squeeze() if ndim==1 else new_data
-
-def notch(data, sfreq=256, f0=50):
-    fs = sfreq  # Sample frequency (Hz)
-    Q = 30.0  # Quality factor
-    w0 = f0/(fs/2)
-    b, a = iirnotch(w0, Q)
-    filtered = lfilter(b,a, data)
-    return filtered.astype(data, copy=False)
-
-########### unchecked functions!! be aware
-
-def highpass(signal, sfreq, hz):
-    fc = hz/sfreq  # Cutoff frequency as a fraction of the sampling rate (in (0, 0.5)).
-    b = 0.08  # Transition band, as a fraction of the sampling rate (in (0, 0.5)).
-    N = int(np.ceil((4 / b)))
-    if not N % 2: N += 1  # Make sure that N is odd.
-    n = np.arange(N)
-     
-    # Compute a low-pass filter.
-    h = np.sinc(2 * fc * (n - (N - 1) / 2.))
-    w = np.blackman(N)
-    h = h * w
-    h = h / np.sum(h)
-     
-    # Create a high-pass filter from the low-pass filter through spectral inversion.
-    h = -h
-    h[(N - 1) // 2] += 1
-    return np.convolve(signal, h)
-
-def butter_bandpass(lowcut, highcut, fs, order=5):
-    nyq = 0.5 * fs
-    low = lowcut / nyq
-    high = highcut / nyq
-    b, a = butter(order, [low, high], btype='band')
-    return b, a
-
-def butter_bandpass_filter(data, lowcut, highcut, fs, order=5):
-    b, a = butter_bandpass(lowcut, highcut, fs, order=order)
-    y = lfilter(b, a, data)
-    return y
-
-def lowpass(signal, sfreq, hz): 
-    fc = hz/sfreq  # Cutoff frequency as a fraction of the sampling rate (in (0, 0.5)).
-    b = 0.08  # Transition band, as a fraction of the sampling rate (in (0, 0.5)).
-    N = int(np.ceil((4 / b)))
-    if not N % 2: N += 1  # Make sure that N is odd.
-    n = np.arange(N)
-     
-    # Compute sinc filter.
-    h = np.sinc(2 * fc * (n - (N - 1) / 2.))
-     
-    # Compute Blackman window.
-    w = 0.42 - 0.5 * np.cos(2 * np.pi * n / (N - 1)) + \
-        0.08 * np.cos(4 * np.pi * n / (N - 1))
-     
-    # Multiply sinc filter with window.
-    h = h * w
-     
-    # Normalize to get unity gain.
-    h = h // np.sum(h)
+# -*- coding: utf-8 -*-
+"""
+Created on Wed Oct 24 09:47:39 2018
+@author: SimonKern
+"""
+import mne
+import warnings
+import scipy
+import numpy as np
+from PIL import Image
+from scipy.signal import correlate, get_window, iirnotch
+from scipy.signal import butter, lfilter, convolve2d, welch, hilbert
+from scipy.stats import zscore
+
+
+# window types used as tapers without parameters
+WTYPES = ['boxcar', 'triang', 'blackman', 'hamming', 'hann', 'bartlett', 
+         'flattop', 'parzen', 'bohman', 'blackmanharris', 'nuttall',
+         'barthann']
+
+###### Begin of functions
+
+
+def dig2phys(signal, dmin, dmax, pmin, pmax):
+    """converts digital to analogue signals"""
+    m = (pmax-pmin) / (dmax-dmin)
+    physical = m * signal
+    return physical
+
+def phys2dig(signal, dmin, dmax, pmin, pmax):
+   """converts analogue to digital signals"""
+   m = (dmax-dmin)/(pmax-pmin) 
+   digital = (m * signal).astype(np.int, copy=False)
+   return digital
+
+
+def rfft_mag(signals):
+    """
+    Returns the magnitude of the fft of a signal: sqrt(real^2+imag^2)
+    Will return only the real part of frequencies (arraylength//2), see rfft
+   
+    :param signals: 1D or 2D array
+    :returns: the magnitude of the frequencies in the signal
+    """
+
+    w = rfft(signals) 
+    mag = np.abs(w) # same as np.abs(w)
+    return mag
+
+
+def rfft(signals, *args, **kwargs):
+    """
+    wrapper for rFFT, mainly for checking differences of Python and C
+    Input should be of length power of 2 for optimization purposes.
+    Returns the arraylength // 2 (unlike rfft, which does weird wlen//2 +1)
+    
+    :param signals: a 1D or 2D signal, where each row contains one window of data
+    :returns: complex array of fft results, 
+              Note: in JSON I save a complex array as two lists with real and imaginary part
+    """
+    if not isinstance(signals, np.ndarray): 
+        signals = np.asarray(signals)    
+    wlen = signals.shape[-1]
+    if not ((wlen & (wlen - 1)) == 0): 
+        warnings.warn('Input array should have length power of 2 for fft, but is: {}'.format(wlen))
+    w = scipy.fftpack.fft(signals)[...,:signals.shape[-1]//2]
+    assert w.shape[-1] == signals.shape[-1]//2, 'w.shape = {}'.format(w.shape)
+    return w
+
+
+
+
+def abs2(x):
+    """highly optimized version for magnitude taking.
+       if there are problems, just remove the decorator line @numba.vectorize(...)
+       if working with float32, need to change signature to inlcude ,numba.float32(numba.complex64)
+    """
+    return x.real**2 + x.imag**2
+
+
+def welchs(signals, nperseg=None, overlap=0.0, taper_name='boxcar'):
+    """
+    A minimal implementation of Welch's method, optimized ~10x faster than previously, 
+    even faster than scipy.signal.welch().
+    This is also equivalent to the normal rfft(), if used with standard parameters
+    
+    If nperseg=0 we have a standard fft.
+    If nperseg>0 and overlap=0 we have Barlett's methd
+    If nperseg>0 and overlap>0 we have Welch's method (use a taper in this case)
+        
+    :param signals: The signals on which to perform Welchs (1D or 2D)
+    :param nperseg: How many samples per segment for the calculation of the FFT
+    :param overlap: How many samples should overlap between segments (int or float)
+                    if float: is interpreted as ratio of nperseg
+                    eg overlap 0.5 = 0.5*nperseg
+    :param taper_name: Which taper to use, if overlap>0, it is recommended to use a taper
+    :returns: The Welch's frequency estimate of the signal as magnitudes
+    """
+    from sklearn import feature_extraction
+
+    signals = np.atleast_2d(signals)
+    siglen = signals.shape[-1]
+    
+    if nperseg is None: nperseg = siglen
+    if isinstance(overlap, float): overlap = overlap*nperseg
+    if siglen%nperseg!=0: warnings.warn('window length should be a multiple of npseg')
+
+    # get window only once, else it will be created for each segment, swallowing computation
+    taper = get_window(taper_name, nperseg, False).astype(int) if taper_name not in ['boxcar', None] else None
+    
+    # this step we have to take to get to the next segment
+    step = int(nperseg - overlap)
+    n_segments    = (siglen-nperseg)//step +1
+    
+    # fastest way to extract patches using np.lib.stride_tricks.as_strided via sklearn
+    fft_segments = feature_extraction.image.extract_patches(signals, patch_shape=(len(signals),nperseg), extraction_step=step)
+    fft_segments = fft_segments.reshape([n_segments, len(signals), nperseg])
+    fft_segments = np.swapaxes(fft_segments, 0,1)
+
+    # apply taper
+    if taper is not None:
+        fft_segments  = np.multiply(fft_segments, taper)
+        
+    # apply fft and take squared magnitude
+    w = rfft(fft_segments)
+    w_mag = abs2(w)
+    fft_result = np.mean(w_mag, axis=1)
+    return fft_result
+
+
+def welchs_unoptimized(signals, nperseg=None, overlap=0.0, taper_name='boxcar'):
+    """
+    A minimal implementation of Welch's method, unoptimized, should be equivalent to welchs()
+    It's kept here for archive purposes and for C-compatibility, also to check 
+    the optimized version in case of changes.
+    
+    If nperseg=0 we have a standard fft.
+    If nperseg>0 and overlap=0 we have Barlett's methd
+    If nperseg>0 and overlap>0 we have Welch's method (use a taper in this case)
+    
+    :param signals: The signals on which to perform Welchs (1D or 2D)
+    :param nperseg: How many samples per segment for the calculation of the FFT
+    :param overlap: How many samples should overlap between segments (int or float)
+                    if float: is interpreted as ratio of nperseg
+                    eg overlap 0.5 = 0.5*nperseg
+    :param taper_name: Which taper to use, if overlap>0, it is recommended to use a taper
+    :returns: The Welch's frequency estimate of the signal as magnitudes
+    """
+    signals = np.atleast_2d(signals)
+    
+    siglen = signals.shape[-1]
+    if nperseg is None: nperseg = siglen
+    if isinstance(overlap, float): overlap = overlap*nperseg
+    if siglen%nperseg!=0: warnings.warn('window length should be a multiple of npseg')
+
+    step = int(nperseg - overlap) # distance between windows that we extract
+    n_segments = (siglen-nperseg)//step + 1 # this is how many windows we can extract from the signal
+    fft_signals = []
+    # loop through the signals (in C you can start at the second loop as we only have 1D arrays)
+    for sig in signals:
+        # collect one fft result per segment
+        # in fft_mean we save a running mean of the fft segments
+        fft_mean = np.zeros(nperseg//2) 
+        # loop through the signal in step sizes that allow for overlap
+        for i in range(0, siglen, step):
+            # only take full segments
+            if i+nperseg>siglen: 
+                break 
+            # extract segment
+            segment = sig[i:i+nperseg]
+            # taper segment if necessary
+            if taper_name is not None:
+                segment = taper(segment, taper_name)
+            # take FFT and add to fft results for segments
+            w = rfft(segment)
+            # this is the same as saving all segments and taking a mean later,
+            # but prevents us from having to keep intermediate results
+            fft_mean += (np.abs(w)**2) / n_segments 
+        # take the mean spectral values for all segments
+        fft_signals.append(fft_mean)
+    return np.array(fft_signals)
+
+
+def moving_average(signals, N):
+    signals = np.atleast_2d(signals).astype(dtype=int, copy=False)
+    return convolve2d(signals, np.ones((1, N))/N, mode='valid')
+    
+
+def binnedmean(signals, target_size=None, bin_edges=None, func=None):
+    """
+    cuts a signal in n parts, applies a function to each part (e.g. mean)
+    this way we can go from an array of length M to an array of length N<M
+    by taking the mean of the elemts of each part, where the number of parts is N
+        
+    :param target_size: The number of bins that we should interpolate to
+    :bin_edges: custom bin edges, if targed size is not present. Bin edges is a list of tuples
+                each tuple represents the edges of the bin [inc, excl].
+    :func: a function that should be applied, standard is mean. 
+           this function needs to operate only on the first dimension
+    """
+    # we only deal with 2D data in the given DTYPE
+    signals = np.atleast_2d(signals)
+
+    assert signals.ndim<3
+    # signal length
+    slen = signals.shape[1]
+    # if there are no bin edges provided, we are creating the bin edges
+    # using the target_size.
+    # that means, we create target_size bins, that are equally spaced
+    # around the signal
+    if bin_edges is None and target_size is not None:
+        bin_edges = np.linspace(0, slen, target_size+1, dtype=np.int)
+        bin_edges = np.repeat(bin_edges,2)[1:-1]
+        bin_edges = bin_edges.reshape([-1,2])
+    # if no function is provided, we take the mean of each bin
+    if func is None:
+        func = lambda s: np.mean(s, axis=1)
+    
+    new_array = np.zeros([signals.shape[0], len(bin_edges)])
+    
+    # now we run over the original array and always take all values of each bin
+    # in the original signal. then we apply the function
+    # that is provided on that bin and write the result to a new array
+    for i, [e1,e2] in enumerate(bin_edges):
+        bin_entries = signals[:,e1:e2]
+        reduced = func(bin_entries)
+        new_array[:,i] = reduced
+        
+    return new_array
+   
+
+def bands2bins(bands, window_len, sfreq):    
+    """
+    A function that turns frequency bands into bin-edges to be used to extract these bands
+    from a fft function
+    
+    :param bands: a list of 2-tuples, each 2-tuple containing a frequency lower and upper bound
+    :param window_len: the length of the window that the FFT will be applied to
+    :param sfreq: the sampling frequency of the signal
+    """
+    sfreq = int(sfreq)
+    window_len=int(window_len)
+    round2=lambda x,y=None: round(x+1e-15,y)
+    bins = []
+    for l,h in bands:
+        bin_lower = int(round2(l*window_len/sfreq)) # np.floor rounds down
+        bin_upper = int(round2(h*window_len/sfreq))  # np.ceil rounds up
+        bins.append([bin_lower, bin_upper])
+    return bins
+
+
+def create_specband_bin_edges(window_len=None, sfreq=None):
+    """
+    Given a FFT-window length and a sampling frequency, 
+    compute the bin edges for common brain frequencies
+    :param window_len: length in sample numbers, if None, will just return bands and not bins
+    :param sfreq: sampling frequency, if None, will just return bands and not bins
+    :returns: edges for [slowos, delta, theta, alpha1, spindle, beta1, beta2, gamma]
+    
+    BRAIN_BAND_NAMES_ = ['so', 'delta', 'theta', 'alpha1', 'alpha2', 'beta1', 'beta2', 'gamma']
+    
+    """
+    if sfreq is None: sfreq=window_len
+    
+    slowos   = [0, 1]
+    delta   = [1, 4]
+    theta   = [4, 8]
+    alpha1  = [8, 10]
+    spindle = [10, 14]
+    beta1   = [13, 16]
+    beta2   = [16, 20]
+    gamma   = [20, 35]
+    
+    # this is the order of the bands
+    # result is a list of tuples, where each tuple is the bin edge
+    bands = [slowos, delta, theta, alpha1, spindle, beta1, beta2, gamma]
+    if window_len is None and sfreq is None: return bands
+    # calculate the bin positions corresponding to frequency edges
+    bins = bands2bins(bands, window_len, sfreq)
+    return bins # this is a list of tuples, e.g. [(0,30),(30,60),(60,120)]
+
+     
+
+def taper(signals, window_name):
+    """
+    filters/tapers given signals or signal with a window with window-name. allowed names are:
+        ['boxcar', 'triang', 'blackman', 'hamming', 'hann', 'bartlett',
+        'flattop', 'parzen', 'bohman', 'blackmanharris', 'nuttall',
+        'barthann'] 
+                
+    :param signals: A 1D signals or a 2D array with signals x samples
+    :param window_name: the name of the taper
+    :returns: the tapered signals
+    """  
+    if window_name in [None, '', 'boxcar']: return signals
+    if window_name.lower() not in ['hamming', 'hann', 'blackman', 'blackmanharris']:
+        warnings.warn('Up to this point, this window is not tested in C code: {}.'.format(window_name))
+    if isinstance(signals, list): signals = np.array(signals)
+    assert signals.ndim in [1,2], 'signals must be 1D or 2D'
+    # how long is the signal?
+    wlen = signals.shape[0] if signals.ndim==1 else signals.shape[1]
+    # get the window function using scipy
+    window = get_window(window_name, wlen, False)
+    # filter our input signal
+    tapered = signals*window  
+    return tapered
+
+
+def extract_windows(signal, length, distance=1.0, group_n=0, group_d=0, hypno=None, taper_name=None):
+    """
+    From a signal, extract windows every N seconds for a length of L.
+    Can be grouped in groups on group_n, with distance between last samplepoint of one group
+    and the first sample of the next group being group_d.
+    only complete groups will be returned    
+    
+    :param signal: the signal to take windows from
+                   if the signal is 2D, the format signaln x samples is assumed
+    :param length: The length of each window in sample space
+    :param distance: the distance between each windows
+                     if distance is an int, it will be interpreted as a spacing in sample space
+                     if distance is a float, it will be interpreted as relative to the length
+                     e.g. distance=0.5 will produce windows with overlap of 50%
+    :param group_n: how many windows to extract before leaving a space to the next group of windows
+    :param group_d: how much space between batches
+                     if distance is an int, it will be interpreted as a spacing in sample space
+                     if distance is a float, it will be interpreted as relative to the length
+                     e.g. group_d=0.5 will produce windows in groups with distance between groups 
+                     of 50% window length 
+    :param hypno: a hypnogram annotation. It will automatically be inferred what spacing the 
+                  hypnogram uses and what annotation frequency
+    """
+    # pass through if length is None
+    if length is None: 
+        return (signal, hypno)
+    
+    assert (group_n==0 and group_d==0) or (group_n>0 and group_d>0), \
+            'group parameters must both be supplied'
+    assert distance>0, 'distance must be positive'
+    assert length>0, 'length must be positive'
+    if hypno is not None: assert type(hypno) is np.ndarray, 'must be numpy array'
+    assert type(signal) is np.ndarray, 'must be numpy array'
+    
+    siglen = len(signal) if signal.ndim==1 else signal.shape[1]
+    distance = distance if type(distance) is int else int(distance*length)
+    group_d  = group_d if type(group_d) is int else int(group_d*length)
+
+    assert length<=siglen, 'length must be smaller than siglen'
+   
+    if signal.ndim == 1: signal = [signal] # to make the iterator work in 1D case
+    
+    
+    # inefficient implenentation, but makes sure everything is correct
+    
+    all_sigs = []
+    for subsig in signal:
+        i = 0
+        g = 0 # group counter
+        sigs = []
+        while i <= siglen-length:
+            s = subsig[i:i+length]
+            sigs.append(s)
+            i+=distance
+            g+=1
+            if g>=group_n and group_n>0:
+                i+=group_d+length-distance
+                g=0
+        all_sigs.append(np.array(sigs))
+        
+    all_sigs = np.array(all_sigs)
+    if all_sigs.shape[0]==1: all_sigs = all_sigs.reshape(-1, length)
+    
+    # match a new hypnogram to the extracted epochs
+    if hypno is not None:
+        s_per_hypno = siglen/len(hypno)
+        i = 0
+        g = 0 # group counter
+        new_hypno = []
+        while i <= siglen-length:
+            h = hypno[int(i/s_per_hypno)]
+            new_hypno.append(h)
+            i+=distance
+            g+=1
+            if g>=group_n and group_n>0:
+                i+=group_d+length-distance
+                g=0
+    windows   = np.array(all_sigs, copy=False)
+    if taper_name is not None: windows = taper(windows, taper_name)
+    if hypno is not None: new_hypno = np.array(new_hypno, dtype = hypno.dtype) 
+    return windows if hypno is None else (windows, new_hypno)
+
+
+def correlate_specto(signal1, signal2, sfreq):
+    """
+    create a cross-correlation of two signals using the spectogram
+    """
+    
+    sfreq1 = 256
+    sfreq2 = 200
+    n_samples1 = int(sfreq1)
+    n_samples2 = int(sfreq2)
+    
+    # get fft results 
+    signal1_trunc = signal1[:int((len(signal1)//n_samples1)*(n_samples1))].reshape([-1,n_samples1])
+    signal2_trunc = signal2[:int((len(signal2)//n_samples2)*(n_samples2))].reshape([-1,n_samples2])
+    
+    # get FFT via Welchs
+    freq1, spec1 = welch(signal1_trunc, fs=sfreq1, window='boxcar', nperseg=sfreq1, noverlap=0)
+    freq2, spec2 = welch(signal2_trunc, fs=sfreq2, window='boxcar', nperseg=sfreq2, noverlap=0)
+    
+    # truncate from 2 to 15 Hz
+    spec1 = spec1[:,np.argmax(freq1>2):np.argmax(freq1>15)]
+    spec2 = spec2[:,np.argmax(freq1>2):np.argmax(freq1>15)]
+  
+    # transform to dB
+    spec1 = (np.log10(spec1+1)*20).T
+    spec2 = (np.log10(spec2+1)*20).T
+
+    # make row-wise correlation
+    corr = np.array([correlate(zscore(row1), zscore(row2)) for row1, row2 in zip(spec1,spec2)]).mean(0)
+    return corr
+
+
+def coeff_var_env(signal, sfreq, band=(0.5, 4), mid_sec=30):
+    """Coefficient of the variance of the envelope (CVE) calculation
+    
+    as defined in  https://doi.org/10.1016/j.neuroimage.2018.01.063
+    
+    :param epoch: one epoch of data, 1D data as array
+    :type epoch: np.ndarray
+    :return: CVE of this epoch
+    :rtype: TYPE
+    """
+    sig = np.atleast_2d(signal)
+    sig_filtered = np.atleast_2d(bandfilter(sig, sfreq, *band, method='iir',
+                                            iir_params={'order':4, 
+                                                        'ftype':'butter'}))
+    ht_sig_filtered = np.abs(hilbert(sig_filtered))
+    
+    eeg_envelope = np.sqrt(sig_filtered**2 + ht_sig_filtered**2)
+    
+    t_excess = int(signal.shape[-1] -  mid_sec*sfreq)//2
+    middle_env = eeg_envelope[:, t_excess:-t_excess]
+    assert abs(middle_env.shape[1]-mid_sec*sfreq)<2
+    
+    mean = np.mean(middle_env)
+    sd = np.std(middle_env)
+    
+    cve = sd/(mean*0.523)  # [..] with 0.523 being the value for Gaussian waves
+     
+    return cve
+
+def get_shift_specto(signal1, signal2, sfreq = 256, w_seconds=1, limit_to=1):
+    """
+    a more robust version to align two eeg recordings using fourier transformations
+    accuracy of this method depends on w_seconds
+    
+    
+    :param signal1: a 1D signal
+    :param signal2: a 1D signal
+    :param sfreq: the sampling frequency of the signals
+    :param w_seconds: how many chunks should be used to create the FFT. This determines the accuracy
+    """
+    assert signal1.ndim==1
+    assert signal2.ndim==1
+    assert np.all([len(signal1)>sfreq*60*5]), 'need at least 5 minutes of data'
+    if len(signal1)>len(signal2)*2: 
+        warnings.warn('signal1 is significantly larger than signal2: \
+                      is the sampling frequency the same?')
+    if len(signal2)>len(signal1)*2: 
+        warnings.warn('signal2 is significantly larger than signal1: \
+                      is the sampling frequency the same?')
+    
+    n_samples = int(w_seconds*sfreq)
+    
+    # get fft results 
+    signal1_trunc = signal1[:int((len(signal1)//n_samples)*(n_samples))].reshape([-1,n_samples])
+    signal2_trunc = signal2[:int((len(signal2)//n_samples)*(n_samples))].reshape([-1,n_samples])
+    
+    # get FFT via Welchs
+    freq1, spec1 = welch(signal1_trunc, fs=sfreq, window='blackmanharris', nperseg=sfreq, noverlap=0.667*sfreq)
+    freq2, spec2 = welch(signal2_trunc, fs=sfreq, window='blackmanharris', nperseg=sfreq, noverlap=0.667*sfreq)
+    
+    # truncate from 2 to 15 Hz
+    spec1 = spec1[:,np.argmax(freq1>2):np.argmax(freq1>15)]
+    spec2 = spec2[:,np.argmax(freq1>2):np.argmax(freq1>15)]
+  
+    # transform to dB
+    spec1 = (np.log10(spec1+1)*20).T
+    spec2 = (np.log10(spec2+1)*20).T
+
+    # make row-wise correlation
+    corr = np.array([correlate(zscore(row1), zscore(row2)) for row1, row2 in zip(spec1,spec2)]).mean(0)
+    half = len(corr)-spec1.shape[1]
+    corr[:int(half-sfreq*60**2*limit_to//n_samples)] = 0
+    corr[int(half+sfreq*60**2*limit_to//n_samples):] = 0
+    peak = corr.argmax()
+    shift = (len(corr)-spec1.shape[1]- peak) * n_samples
+    return -shift
+
+
+def get_shift_spindle(signal1, signal2, sfreq, limit_to=1):
+    """
+    Taking two frontal channels, will try to recover the shift
+    via aligning the spindle band. This should filter out a lot
+    of other non-related noise and be quite robust for sleep recordings
+    
+    Shift will be searched for within 1h of the recording start
+    
+    :param signal1: a 1D signal
+    :param signal2: a 1D signal
+    :param limit_to: limit to +- this hour
+    """
+    assert signal1.ndim==1
+    assert signal2.ndim==1
+    if len(signal1)>len(signal2)*2: 
+        warnings.warn('signal1 is significantly larger than signal2: \
+                      is the sampling frequency the same?')
+    if len(signal2)>len(signal1)*2: 
+        warnings.warn('signal2 is significantly larger than signal1: \
+                      is the sampling frequency the same?')
+        
+    sigma1 = butter_bandpass_filter(signal1/signal1.max(), 7, 14, sfreq, 5)
+    sigma2 = butter_bandpass_filter(signal2/signal2.max(), 7, 14, sfreq, 5)
+    
+    corr = correlate(sigma1, sigma2)
+    # sometimes there are some weird correlations if the signals are shifted
+    # extremely. We assume that the recording alignment must lie within 
+    # 1 h of either recording start
+    half = len(corr)//2
+    corr[:half-sfreq*60**2*limit_to] = 0
+    corr[half+sfreq*60**2*limit_to:] = 0
+    peak = corr.argmax()
+    shift = len(signal2) - peak -1 
+    print(shift/sfreq, ' seconds')
+#    plt.plot(corr)
+    return -shift    
+
+
+    
+def get_shift(signal1, signal2, sfreq, limit_to=1):
+    """
+    find the shift of signal1 to signal2, used for aligning two signals
+    
+    Data must have the same sampling frequency
+    
+    The output will be how much we need to roll signal2 to match signal1
+    np.roll(signal2, shift)
+    
+    :param signal1: a 1D signal
+    :param signal2: a 1D signal
+    """
+    assert signal1.ndim==1
+    assert signal2.ndim==1
+    if len(signal1)>len(signal2)*2: 
+        warnings.warn('signal1 is significantly larger than signal2: \
+                      is the sampling frequency the same?')
+    if len(signal2)>len(signal1)*2: 
+        warnings.warn('signal2 is significantly larger than signal1: \
+                      is the sampling frequency the same?')
+    if signal1.max()>10: signal1 = zscore(signal1, axis=None)
+    if signal2.max()>10: signal2 = zscore(signal2, axis=None)
+    
+    signal1 = butter_bandpass_filter(signal1/signal1.max(), 1, 30, sfreq, 5)
+    signal2 = butter_bandpass_filter(signal2/signal2.max(), 1, 30, sfreq, 5)
+    
+    corr = correlate(signal1, signal2)
+    half = len(corr)//2
+    corr[:half-sfreq*60**2*limit_to] = 0
+    corr[half+sfreq*60**2*limit_to:] = 0
+    peak = corr.argmax()
+    shift = len(signal2) - peak -1 
+    return -shift
+
+def get_correlation(signal1, signal2, sfreq, llim=2, ulim=20):
+    """
+    find the shift of signal1 to signal2, used for aligning two signals
+    
+    Data must have the same sampling frequency
+    
+    The output will be how much we need to roll signal2 to match signal1
+    np.roll(signal2, shift)
+    
+    :param signal1: a 1D signal
+    :param signal2: a 1D signal
+    """
+    assert signal1.ndim==1
+    assert signal2.ndim==1
+    if len(signal1)>len(signal2)*2: 
+        warnings.warn('signal1 is significantly larger than signal2: \
+                      is the sampling frequency the same?')
+    if len(signal2)>len(signal1)*2: 
+        warnings.warn('signal2 is significantly larger than signal1: \
+                      is the sampling frequency the same?')
+    if signal1.max()>10: signal1 = zscore(signal1, axis=None)
+    if signal2.max()>10: signal2 = zscore(signal2, axis=None)
+    
+    signal1 = butter_bandpass_filter(signal1, 0.1, 30, sfreq, 5)
+    signal2 = butter_bandpass_filter(signal2, 0.1, 30, sfreq, 5)
+    
+    corr = correlate(np.abs(signal1), np.abs(signal2))
+    return corr
+
+
+def resample(data, o_sfreq, t_sfreq):
+    """
+    resample a signal using MNE resample functions
+    This automatically is optimized for EEG applying filters etc
+    
+    :param raw:     a 1D data array
+    :param o_sfreq: the original sampling frequency
+    :param t_sfreq: the target sampling frequency
+    :returns: the resampled signal
+    """
+    if o_sfreq==t_sfreq: return data
+    raw = np.atleast_2d(data)
+    n_jobs = min(len(raw), 8)
+    ch_names=['ch{}'.format(i) for i in range(len(raw))]
+    info = mne.create_info(ch_names=ch_names, sfreq=o_sfreq, ch_types=['eeg'])
+    raw_mne = mne.io.RawArray(raw, info, verbose='WARNING')
+    resampled = raw_mne.resample(t_sfreq, n_jobs=n_jobs, verbose='WARNING')
+    new_raw = resampled.get_data().squeeze()
+    return new_raw.astype(raw.dtype, copy=False)
+
+def resize(array, target_size):
+    """
+    Resize a 1D array containing a signal/
+    or a 2D array of several signasl as rows of any type (int/float) 
+    by taking nearest neighbours to fill gaps within the rows
+    
+    :param array: any type of array
+    :param target_size: the target size of the last dimension
+    """
+    array = np.atleast_2d(array)
+    new_array = []
+    for row in array:
+        pil_row = Image.fromarray(row.reshape([1,-1]))
+        pil_resized = pil_row.resize((target_size,1), Image.NEAREST)
+        new_array.append(np.array(pil_resized).squeeze())
+    return np.array(new_array).squeeze()
+    
+    
+
+def bandfilter(data, sfreq, l_freq, h_freq, **kwargs):
+    """Use mne.io.RawArray.filter to create a bandpath filter for this signal
+    
+    Can be either 1D or 2D signal
+    
+    :param raw: the signal
+    :param sfreq: the sampling frequency of the signal
+    :param l_freq: the lower frequency
+    :param h_freq: the higher frequency
+    """
+    assert data.ndim<3, 'Data must be 2D or 1D'
+    ndim = data.ndim
+    data = np.atleast_2d(data)
+    ch_names = [f'ch{i}' for i,_ in enumerate(data)]
+    info = mne.create_info(ch_names=ch_names, sfreq=sfreq, ch_types=['eeg'])
+    raw = mne.io.RawArray(data, info, verbose='WARNING', copy='both')
+    raw = raw.filter(l_freq, h_freq, verbose='WARNING', **kwargs)
+    new_data = raw.get_data()
+    return new_data.squeeze() if ndim==1 else new_data
+
+def notch(data, sfreq=256, f0=50):
+    fs = sfreq  # Sample frequency (Hz)
+    Q = 30.0  # Quality factor
+    w0 = f0/(fs/2)
+    b, a = iirnotch(w0, Q)
+    filtered = lfilter(b,a, data)
+    return filtered.astype(data, copy=False)
+
+########### unchecked functions!! be aware
+
+def highpass(signal, sfreq, hz):
+    fc = hz/sfreq  # Cutoff frequency as a fraction of the sampling rate (in (0, 0.5)).
+    b = 0.08  # Transition band, as a fraction of the sampling rate (in (0, 0.5)).
+    N = int(np.ceil((4 / b)))
+    if not N % 2: N += 1  # Make sure that N is odd.
+    n = np.arange(N)
+     
+    # Compute a low-pass filter.
+    h = np.sinc(2 * fc * (n - (N - 1) / 2.))
+    w = np.blackman(N)
+    h = h * w
+    h = h / np.sum(h)
+     
+    # Create a high-pass filter from the low-pass filter through spectral inversion.
+    h = -h
+    h[(N - 1) // 2] += 1
+    return np.convolve(signal, h)
+
+def butter_bandpass(lowcut, highcut, fs, order=5):
+    nyq = 0.5 * fs
+    low = lowcut / nyq
+    high = highcut / nyq
+    b, a = butter(order, [low, high], btype='band')
+    return b, a
+
+def butter_bandpass_filter(data, lowcut, highcut, fs, order=5):
+    b, a = butter_bandpass(lowcut, highcut, fs, order=order)
+    y = lfilter(b, a, data)
+    return y
+
+def lowpass(signal, sfreq, hz): 
+    fc = hz/sfreq  # Cutoff frequency as a fraction of the sampling rate (in (0, 0.5)).
+    b = 0.08  # Transition band, as a fraction of the sampling rate (in (0, 0.5)).
+    N = int(np.ceil((4 / b)))
+    if not N % 2: N += 1  # Make sure that N is odd.
+    n = np.arange(N)
+     
+    # Compute sinc filter.
+    h = np.sinc(2 * fc * (n - (N - 1) / 2.))
+     
+    # Compute Blackman window.
+    w = 0.42 - 0.5 * np.cos(2 * np.pi * n / (N - 1)) + \
+        0.08 * np.cos(4 * np.pi * n / (N - 1))
+     
+    # Multiply sinc filter with window.
+    h = h * w
+     
+    # Normalize to get unity gain.
+    h = h // np.sum(h)
     return np.convolve(signal, h)
```

### Comparing `sleep-utils-1.15/sleep_utils/tools.py` & `sleep-utils-1.16/sleep_utils/tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,546 +1,553 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Thu Oct  4 11:22:20 2018
-
-@author: skjerns
-
-This file contains all functions that deal with IO
-
-"""
-import os
-import numpy as np
-import time
-import mne
-from io import StringIO
-import warnings
-import logging
-from pprint import pprint
-from datetime import datetime, timezone, timedelta
-
-def sleep(seconds):
-    if seconds > 1:
-        for s in range(seconds):
-            time.sleep(1)
-    else:
-        time.sleep(seconds)
-        
-class AttrDict(dict):
-    def __init__(self, *args, **kwargs):
-        super(AttrDict, self).__init__(*args, **kwargs)
-        self.__dict__ = self
-        
-
-def log(msg, *args, **kwargs):
-    """
-    Displays timestamp next to message
-    """
-    msg = '[{}] '.format(time.strftime('%H:%M:%S')) + msg
-    print(msg, flush=True, *args, **kwargs)
-    
-
-def analyze_function(fun):
-    """
-    checks a couple of things for a function:
-        is it scale invariant?
-        is it ud/lr flip invariant?
-    """
-    signal = np.sin(np.linspace(0,100, 1000))
-    out  = fun(signal)
-    out2 = fun(signal*2)
-    if np.allclose(out, out2):
-        print('Scale invariant')
-    elif np.allclose(out*2, out2):
-        print('Preserves scale')
-    else:
-        print('Changes scaling')
-        
-    out  = fun(signal)
-    out2 = fun(signal+2)
-    if np.allclose(out, out2):
-        print('Shift invariant')
-    elif np.allclose(out+2, out2):
-        print('Preserves shift')
-    else:
-        print('Changes shift')
-
-def hypno_summary(hypno, epochlen=30, verbose=True):
-    """
-    param hypno: a hypnogram with stages in format
-                 W:0, S1:1, S2:2, S3:3, REM:4
-    param epochlen: the lenght of each entry in the hypnogram, e.g. 30 seconds
-    
-    summarizes the sleep parameters according to the AASM recommendations
-
-    
-        TST:     total sleep time - sum of minutes of sleep stages other than W
-        TRT:     total recording time - duration from sleep onset to offset
-        WASO:    total time spent in Wake between sleep onset/offset in minutes
-        min S1:  total time spent in S1 in minutes
-        min S2:  total time spent in S2 in minutes
-        min S3:  total time spent in S3 in minutes
-        min REM: total time spent in REM in minutes
-        % WASO:  percentage Wake after sleep onset relative to TRT
-        % S1:    relative time spent in S1 to TST
-        % S2:    relative time spent in S2 to TST
-        % S3:    relative time spent in S3 to TST
-        % REM:   relative time spent in REM to TST
-        lat S1:  latency of first S1 epoch after sleep onset in minutes
-        lat S2:  latency of first S2 epoch after sleep onset in minutes
-        lat S3:  latency of first S3 epoch after sleep onset in minutes
-        lat REM: latency of first REM epoch after sleep onset in minutes
-
-    For details and definitions see Iber et al (2007) The AASM Manual for the 
-    Scoring of Sleep and Associated Events. 
-    
-    NB:
-    sleep onset is defined by the AASM as the first non Wake epoch.
-    Currently all parameters using lights out/lights on (eg. sleep efficiency)
-    are not supported yet. Therefore, TRT will rely on sleep onset and sleep
-    offset as markers for its calculation.
-
-        
-    """
-    hypno = np.array(hypno)
-    
-    sleep_stages = {'W':0, 'S1':1, 'S2':2, 'SWS':3, 'REM':4}
-    # do some sanity checks
-    for stage, num in sleep_stages.items():
-        if not num in hypno:
-            warnings.warn(f'Stage {stage} not found in hypnogram')
-    for stage in np.unique(hypno):
-        if not stage in sleep_stages.values():
-            warnings.warn(f'Found annotation with unknown value {stage}. '\
-                          f'can only understand stages {sleep_stages}. '
-                          'calculations will likely be wrong. Please '
-                          'either transform to another stage (e.g. W) or' 
-                          ' remove from hypnogram.')
-                
-    onset = np.where(hypno!=0)[0][0] # first non-W epoch
-    offset = np.where(hypno!=0)[0][-1] # last non-W epoch
-    
-    TST = (sum(hypno!=0)*epochlen)/60
-    TRT = (offset-onset)*epochlen/60
-    
-    WASO = TRT-TST
-    min_S1 = sum(hypno==1)*epochlen/60
-    min_S2 = sum(hypno==2)*epochlen/60
-    min_S3 = sum(hypno==3)*epochlen/60
-    min_REM = sum(hypno==4)*epochlen/60
-    
-    perc_W = WASO/TRT
-    perc_S1 = min_S1/TST
-    perc_S2 = min_S2/TST
-    perc_S3 = min_S3/TST
-    perc_REM = min_REM/TST
-
-    lat_S1 = (np.argmax(hypno==1)-onset)*epochlen/60
-    lat_S2 = (np.argmax(hypno==2)-onset)*epochlen/60
-    lat_S3 = (np.argmax(hypno==3)-onset)*epochlen/60
-    lat_REM = (np.argmax(hypno==4)-onset)*epochlen/60
-
-    sleep_onset_after_rec_start = onset*epochlen/60 # now convert to minutes
-    sleep_offset_after_rec_start = offset*epochlen/60 # now convert to minutes
-    recording_length = len(hypno)*epochlen/60
-    
-    summary = locals().copy()
-    ignore = ['verbose', 'epochlen', 'stage', 'sleep_stages', 'num', 'hypno',
-              'offset', 'onset']
-    for var in ignore:
-        del summary[var]
-
-    if verbose: pprint(summary)
-
-    return summary
-
-
-    
-def read_hypno(hypno_file, epochlen = 30, epochlen_infile=None, mode='auto', 
-               exp_seconds=None, conf_dict=None, verbose=True):
-    """
-    reads a hypnogram file as created by VisBrain or as CSV type 
-    (or also some custom cases like the Dreams database)
-    
-    :param hypno_file: a path to the hypnogram
-    :param epochlen: how many seconds per label in output
-    :param epochlen_infile: how many seconds per label in original file
-    :param mode: 'auto', 'time' or 'csv', see SleepDev/docs/hypnogram.md
-    :param exp_seconds: How many seconds does the matching recording have?
-    """
-    assert str(type(epochlen)()) == '0'
-    assert epochlen_infile is None or str(type(epochlen_infile)()) == '0'
-    
-    if isinstance(hypno_file, str):
-        with open(hypno_file, 'r') as file:
-            content = file.read()
-            content = content.replace('\r', '') # remove windows style \r\n
-    elif isinstance(hypno_file, StringIO):
-        content = hypno_file.read()
-        content = content.replace('\r', '') # remove windows style \r\n
-            
-    #conversion dictionary
-    if conf_dict is None:
-        conv_dict = {'W':0, 'WAKE':0, 'N1': 1, 'N2': 2, 'N3': 3, 'R':4, 'REM': 4, 'ART': 9,
-                     -1:9, '-1':9, **{i:i for i in range(0, 10)}, **{f'{i}':i for i in range(0, 10)}}
-    
-    lines = content.split('\n')
-    if mode=='auto':
-        if lines[0].startswith('*'): # if there is a star, we assume it's the visbrain type
-            mode = 'time'
-        elif lines[0].replace('-', '')[0].isnumeric():
-            mode = 'csv'
-        elif lines[0].startswith('[HypnogramAASM]'):
-            mode = 'dreams'
-        elif lines[0].startswith(' Epoch Number ,Start Time ,Sleep Stage'):
-            mode = 'alice'
-        elif lines[0].startswith('EPOCH=') and lines[1].startswith('START='):
-            mode = 'csv'
-            lines = [l.upper() for l in lines[2:]]
-        else:
-            known_stage = [l.upper() in conv_dict for l in lines]
-            if all(known_stage):
-                mode='csv'
-            else:
-                mode=None
-            
-    if mode=='time':
-        if epochlen_infile is not None:
-            warnings.warn('epochlen_infile has been supplied, but hypnogram is time based,'
-                          'will be ignored')
-        stages = []
-        prev_t = 0
-        for line in lines:
-            if len(line.strip())==0:   continue
-            if line[0] in '*#%/\\"\'': continue # this line seems to be a comment
-            s, t = line.split('\t')
-            t = float(t)
-            s = conv_dict[s]
-            l = int(np.round((t-prev_t))) # length of this stage
-            stages.extend([s]*l)
-            prev_t = t
-            
-    elif mode=='csv':
-        if exp_seconds and not epochlen_infile:
-            epochlen_infile=exp_seconds//len(lines)
-            if verbose: print('[INFO] Assuming csv annotations with one entry per {} seconds'.format(epochlen_infile))
-
-        elif epochlen_infile is None: 
-            if len(lines) < 2400: # we assume no recording is longer than 20 hours
-                epochlen_infile = 30
-                if verbose: print('[INFO] Assuming csv annotations are per epoch')
-            else:
-                epochlen_infile = 1 
-                if verbose: print('[INFO] Assuming csv annotations are per second')
-        lines = [line.split('\t')[0] if '\t' in line else line for line in lines]
-        lines = [conv_dict[l]  if l in conv_dict else l for l in lines if len(l)>0]
-        lines = [[line]*epochlen_infile for line in lines]
-        stages = np.array([conv_dict[l] for l in np.array(lines).flatten()])
-    
-    # for the Dreams Database    
-    elif mode=='dreams':
-        epochlen_infile = 5
-        conv_dict = {-2:5,-1:5, 0:5, 1:3, 2:2, 3:1, 4:4, 5:0}    
-        lines = [[int(line)] for line in lines[1:] if len(line)>0]
-        lines = [[line]*epochlen_infile for line in lines]
-        stages = np.array([conv_dict[l] for l in np.array(lines).flatten()])
-        
-    elif mode=='alice':
-        epochlen_infile = 30
-        conv_dict = {'WK':0,'N1':1, 'N2':2, 'N3':3, 'REM':4}  
-        lines = [line.split(',')[-1] for line in lines[1:] if len(line)>0]
-        lines = [[line]*epochlen_infile for line in lines]
-        try: stages = np.array([conv_dict[l] for l in np.array(lines).flatten()])
-        except KeyError as e:
-            print('Unknown sleep stage in file')
-            raise e
-    else:
-        raise ValueError('This is not a recognized hypnogram: {}'.format(hypno_file))
-        
-    stages = stages[::epochlen]
-    if len(stages)==0:
-        logging.warning('hypnogram loading failed, len == 0')
-        
-    return np.array(stages)
-   
-    
-def hypno2time(hypno, seconds_per_epoch=1):
-    """
-    Converts a hypnogram into the format as defined by visbrain
-    """
-    hypno = np.repeat(hypno, seconds_per_epoch)
-    s = '*Duration_sec {}\n'.format(len(hypno))
-    stages = ['Wake', 'N1', 'N2', 'N3', 'REM', 'Art']
-    d = dict(enumerate(stages))
-    hypno_str = [d[h] for h in hypno]
-    
-    last_stage=hypno_str[0]
-    
-    for second, stage in enumerate(hypno_str):
-        if stage!=last_stage:
-            s += '{}\t{}\n'.format(last_stage, second)
-            last_stage=stage
-    s += '{}\t{}\n'.format(stage, second+1)
-    return s
-
-def write_hypno_time(hypno, filename, seconds_per_annotation=30, comment=None, overwrite=False):
-    """
-    Save hypnogram data with visbrain style 
-    The exact onset of each sleep stage is annotated in time space.
-    This format is recommended for saving hypnograms
-    
-    :param filename: where to save the data
-    :param hypno: The hypnogram either as list or np.array
-    :param seconds_per_epoch: How many seconds each annotation contains
-    :param overwrite: overwrite file?
-    """
-    assert not os.path.exists(filename) or overwrite, 'File already exists, no overwrite'
-    hypno = np.repeat(hypno, seconds_per_annotation)
-    hypno_str = hypno2time(hypno)
-    if comment is not None:
-        comment = comment.replace('\n', '\n*')
-        hypno_str = '*' + comment + '\n' + hypno_str
-        hypno_str = hypno_str.replace('\n\n', '\n')
-    with open(filename, 'w') as f:
-        f.write(hypno_str)    
-    return True
-        
-    
-def write_hypno_csv(hypno, filename, seconds_per_annotation = 30, mode = 'seconds',
-                    overwrite = False):
-    """
-    Save hypnogram data. Expects hypnogram to be based on epoch basis.
-    it is saved as a csv-style file with one entry per second (default) and a new-line as separator
-    
-    :param filename: where to save the data
-    :param hypno: The hypnogram either as list or np.array
-    :param seconds_per_annotation: how many seconds does one annotation account for
-    :param mode: 'seconds' or 'epochs':
-                 'seconds' : writes one annotation per second
-                 'epochs': write one annotation per 30 seconds
-    :param overwrite: overwrite file?
-    """
-    assert not os.path.exists(filename) or overwrite, 'File already exists, no overwrite'
-    assert mode in ['seconds', 'epochs'],'Mode must be seconds or epochs, is {}'.format(mode) 
-    hypno = np.array(hypno, copy=False)
-    try:
-        if np.any(np.logical_or(hypno>5, hypno<0)):
-            raise ValueError('Contains values outside of [0, 5], which stage should that be?? ')
-        with open(filename, 'w') as f:
-            hypno_rep = [str(v) for v in np.repeat(hypno, seconds_per_annotation)]
-            if mode=='epochs':
-                hypno_rep = hypno_rep[::30]
-            hypno_str = '\n'.join(hypno_rep)
-            f.write(hypno_str)
-    except Exception as e:
-        print(e)
-        return False
-    return True
-
-
-def write_hypno(hypno, filename, mode='time', seconds_per_annotation = 30, comment = None,
-                overwrite = False):
-    """
-    Writes a hypnogram to file
-    
-        0 Wake
-        1 N1
-        2 N2
-        3 N3
-        4 REM
-        5 Artefact / unknown
-        
-    :param filename: the filename under which to save a hypnogram
-    :param hypno: a 1D array with sleep stage annotations.
-    :param mode: 'time' or 'csv'
-                 time: will save with the visbrain format (default)
-                 csv: will save as a simple csv file
-    :param seconds_per_annotation: how many seconds does one annotation account for
-    :param comment: A comment that is added to the beginning if the file
-    :param overwrite: Overwrite file if already present?
-    """
-
-    assert seconds_per_annotation>=1
-    if mode=='time':
-        if not filename.endswith('.hypno'):
-            warnings.warn('Filename ends in ".{}", recommended to end in .hypno'.format(
-                           os.path.splitext(filename)[1]))
-        write_hypno_time(hypno, filename, seconds_per_annotation=seconds_per_annotation, 
-                         comment=comment, overwrite=overwrite)
-    elif mode=='csv':
-        write_hypno_csv(hypno, filename, seconds_per_annotation=seconds_per_annotation, 
-                        overwrite=overwrite)
-    else:
-        raise ValueError('Unkown mode {}, must be time or csv'.format(mode))
-
-
-    
-
-def transform_hypno(hypno, t_dict):
-    """
-    Will transform the hypnogram according to a lookup dictionary
-    :param data: input data, will not be altered
-    :param hypno: a hypnogram
-    :param t_dict: a dictionary with lookup values.
-                   if a value of hypno is not in t_dict it will not be altered
-    :returns: data, new_hypnogram             
-    """
-    hypno_values = np.unique(hypno)
-    mapping = {h:h for h in hypno_values}
-    mapping.update(t_dict)
-    new_hypno = [mapping[h] for h in hypno]
-    if type(hypno)==np.ndarray: new_hypno = np.array(new_hypno, dtype=hypno.dtype)
-    return  new_hypno
-
-def convert_hypnogram(hypno_file_in, hypno_file_out, **kwargs):
-    """
-    takes an arbitrary hypnogram and converts it to a time based format
-    
-    :param hypno_file_in:  A string pointing to a hypnogrma file
-    :param hypno_file_out: Where the converted hypnogram should be saved
-    """
-    assert not os.path.exists(hypno_file_out)
-    hypno = read_hypno(hypno_file_in, **kwargs)
-    return write_hypno(hypno, hypno_file_out)
-    
-
-
-def _time_format(seconds):
-    """ returns a string with a fitting string"""
-    return '{:02d}:{:02d} hours'.format(seconds//3600, seconds%3600//60)
-
-
-    
-
-def _stamp_to_dt(utc_stamp):
-    """Convert timestamp to datetime object in Windows-friendly way."""
-    if 'datetime' in str(type(utc_stamp)): return utc_stamp
-    # The min on windows is 86400
-    stamp = [int(s) for s in utc_stamp]
-    if len(stamp) == 1:  # In case there is no microseconds information
-        stamp.append(0)
-    return (datetime.fromtimestamp(0, tz=timezone.utc) +
-            timedelta(0, stamp[0], stamp[1]))  # day, sec, μs
-
-
-def write_mne_edf(mne_raw, fname, picks=None, tmin=0, tmax=None, 
-                  overwrite=False, verbose=False):
-    """
-    Saves the raw content of an MNE.io.Raw and its subclasses to
-    a file using the EDF+/BDF filetype
-    pyEDFlib is used to save the raw contents of the RawArray to disk
-    Parameters
-    ----------
-    mne_raw : mne.io.Raw
-        An object with super class mne.io.Raw that contains the data
-        to save
-    fname : string
-        File name of the new dataset. This has to be a new filename
-        unless data have been preloaded. Filenames should end with .edf
-    picks : array-like of int | None
-        Indices of channels to include. If None all channels are kept.
-    tmin : float | None
-        Time in seconds of first sample to save. If None first sample
-        is used.
-    tmax : float | None
-        Time in seconds of last sample to save. If None last sample
-        is used.
-    overwrite : bool
-        If True, the destination file (if it exists) will be overwritten.
-        If False (default), an error will be raised if the file exists.
-    """
-    import pyedflib # pip install pyedflib
-    from pyedflib import FILETYPE_BDF, FILETYPE_BDFPLUS, FILETYPE_EDF, FILETYPE_EDFPLUS
-    if not issubclass(type(mne_raw), mne.io.BaseRaw):
-        raise TypeError('Must be mne.io.Raw type')
-    if not overwrite and os.path.exists(fname):
-        raise OSError('File already exists. No overwrite.')
-        
-    # static settings
-    has_annotations = True if len(mne_raw.annotations)>0 else False
-    if os.path.splitext(fname)[-1] == '.edf':
-        file_type = FILETYPE_EDFPLUS if has_annotations else FILETYPE_EDF
-        dmin, dmax = -32768, 32767 
-    else:
-        file_type = FILETYPE_BDFPLUS if has_annotations else FILETYPE_BDF
-        dmin, dmax = -8388608, 8388607
-    
-    print('saving to {}, filetype {}'.format(fname, file_type))
-    sfreq = mne_raw.info['sfreq']
-    date = _stamp_to_dt(mne_raw.info['meas_date'])
-    
-    if tmin:
-        date += timedelta(seconds=tmin)
-    # no conversion necessary, as pyedflib can handle datetime.
-    #date = date.strftime('%d %b %Y %H:%M:%S')
-    first_sample = int(sfreq*tmin)
-    last_sample  = int(sfreq*tmax) if tmax is not None else None
-
-    
-    # convert data
-    channels = mne_raw.get_data(picks, 
-                                start = first_sample,
-                                stop  = last_sample)
-    
-    # convert to microvolts to scale up precision
-    eeg_chs = [ch_type=='eeg' for ch_type in mne_raw.get_channel_types()]
-    channels[eeg_chs,:] *= 1e6
-
-    # set conversion parameters
-    n_channels = len(channels)
-    
-    # create channel from this   
-    try:
-        f = pyedflib.EdfWriter(fname,
-                               n_channels=n_channels, 
-                               file_type=file_type)
-        
-        channel_info = []
-        
-        ch_idx = range(n_channels) if picks is None else picks
-        keys = list(mne_raw._orig_units.keys())
-        for i in ch_idx:
-            try:
-                ch_dict = {'label': mne_raw.ch_names[i], 
-                           'dimension': mne_raw._orig_units[keys[i]], 
-                           'sample_rate': mne_raw._raw_extras[0]['n_samps'][i], 
-                           'physical_min': mne_raw._raw_extras[0]['physical_min'][i], 
-                           'physical_max': mne_raw._raw_extras[0]['physical_max'][i], 
-                           'digital_min':  mne_raw._raw_extras[0]['digital_min'][i], 
-                           'digital_max':  mne_raw._raw_extras[0]['digital_max'][i], 
-                           'transducer': '', 
-                           'prefilter': ''}
-            except:
-                ch_dict = {'label': mne_raw.ch_names[i], 
-                           'dimension': mne_raw._orig_units[keys[i]], 
-                           'sample_rate': sfreq, 
-                           'physical_min': channels[i].min(), 
-                           'physical_max': channels[i].max(), 
-                           'digital_min':  dmin, 
-                           'digital_max':  dmax, 
-                           'transducer': '', 
-                           'prefilter': ''}
-        
-            channel_info.append(ch_dict)
-            
-        subject_info = mne_raw._raw_extras[0].get('subject_info',{})
-        f.setPatientCode(subject_info.get('id', '0'))
-        f.setPatientName(subject_info.get('name', 'noname'))
-        f.setTechnician('mne-gist-save-edf-skjerns')
-        f.setSignalHeaders(channel_info)
-        f.setStartdatetime(date)
-        f.writeSamples(channels)
-        
-        for annotation in mne_raw.annotations:
-            onset = annotation['onset']
-            duration = annotation['duration']
-            description = annotation['description']
-            f.writeAnnotation(onset, duration, description)
-        
-    except Exception as e:
-        raise e
-    finally:
-        f.close()    
-    return True
-
-
-            
-        
+# -*- coding: utf-8 -*-
+"""
+Created on Thu Oct  4 11:22:20 2018
+
+@author: skjerns
+
+This file contains all functions that deal with IO
+
+"""
+import os
+import time
+import warnings
+import logging
+import itertools
+import tempfile
+import mne
+import numpy as np
+from io import StringIO
+from pprint import pprint
+from datetime import datetime, timezone, timedelta
+
+
+    
+def sleep(seconds):
+    if seconds > 1:
+        for s in range(seconds):
+            time.sleep(1)
+    else:
+        time.sleep(seconds)
+
+def log(msg, *args, **kwargs):
+    """
+    Displays timestamp next to message
+    """
+    msg = '[{}] '.format(time.strftime('%H:%M:%S')) + msg
+    print(msg, flush=True, *args, **kwargs)
+
+
+def analyze_function(fun):
+    """
+    checks a couple of things for a function:
+        is it scale invariant?
+        is it ud/lr flip invariant?
+    """
+    signal = np.sin(np.linspace(0,100, 1000))
+    out  = fun(signal)
+    out2 = fun(signal*2)
+    if np.allclose(out, out2):
+        print('Scale invariant')
+    elif np.allclose(out*2, out2):
+        print('Preserves scale')
+    else:
+        print('Changes scaling')
+
+    out  = fun(signal)
+    out2 = fun(signal+2)
+    if np.allclose(out, out2):
+        print('Shift invariant')
+    elif np.allclose(out+2, out2):
+        print('Preserves shift')
+    else:
+        print('Changes shift')
+
+def hypno_summary(hypno, epochlen=30, verbose=True):
+    """
+    param hypno: a hypnogram with stages in format
+                 W:0, S1:1, S2:2, S3:3, REM:4
+    param epochlen: the lenght of each entry in the hypnogram, e.g. 30 seconds
+
+    summarizes the sleep parameters according to the AASM recommendations
+
+
+        TST:     total sleep time - sum of minutes of sleep stages other than W
+        TRT:     total recording time - duration from sleep onset to offset
+        WASO:    total time spent in Wake between sleep onset/offset in minutes
+        min S1:  total time spent in S1 in minutes
+        min S2:  total time spent in S2 in minutes
+        min S3:  total time spent in S3 in minutes
+        min REM: total time spent in REM in minutes
+        % WASO:  percentage Wake after sleep onset relative to TRT
+        % S1:    relative time spent in S1 to TST
+        % S2:    relative time spent in S2 to TST
+        % S3:    relative time spent in S3 to TST
+        % REM:   relative time spent in REM to TST
+        lat S1:  latency of first S1 epoch after sleep onset in minutes
+        lat S2:  latency of first S2 epoch after sleep onset in minutes
+        lat S3:  latency of first S3 epoch after sleep onset in minutes
+        lat REM: latency of first REM epoch after sleep onset in minutes
+
+    For details and definitions see Iber et al (2007) The AASM Manual for the
+    Scoring of Sleep and Associated Events.
+
+    NB:
+    sleep onset is defined by the AASM as the first non Wake epoch.
+    Currently all parameters using lights out/lights on (eg. sleep efficiency)
+    are not supported yet. Therefore, TRT will rely on sleep onset and sleep
+    offset as markers for its calculation.
+
+
+    """
+    hypno = np.array(hypno)
+
+    sleep_stages = {'W':0, 'S1':1, 'S2':2, 'SWS':3, 'REM':4}
+    # do some sanity checks
+    for stage, num in sleep_stages.items():
+        if not num in hypno:
+            warnings.warn(f'Stage {stage} not found in hypnogram')
+    for stage in np.unique(hypno):
+        if not stage in sleep_stages.values():
+            warnings.warn(f'Found annotation with unknown value {stage}. '\
+                          f'can only understand stages {sleep_stages}. '
+                          'calculations will likely be wrong. Please '
+                          'either transform to another stage (e.g. W) or'
+                          ' remove from hypnogram.')
+
+    onset = np.where(hypno!=0)[0][0] # first non-W epoch
+    offset = np.where(hypno!=0)[0][-1] # last non-W epoch
+
+    TST = (sum(hypno!=0)*epochlen)/60
+    TRT = (offset-onset)*epochlen/60
+
+    WASO = TRT-TST
+    min_S1 = sum(hypno==1)*epochlen/60
+    min_S2 = sum(hypno==2)*epochlen/60
+    min_S3 = sum(hypno==3)*epochlen/60
+    min_REM = sum(hypno==4)*epochlen/60
+
+    perc_W = WASO/TRT
+    perc_S1 = min_S1/TST
+    perc_S2 = min_S2/TST
+    perc_S3 = min_S3/TST
+    perc_REM = min_REM/TST
+
+    lat_S1 = (np.argmax(hypno==1)-onset)*epochlen/60
+    lat_S2 = (np.argmax(hypno==2)-onset)*epochlen/60
+    lat_S3 = (np.argmax(hypno==3)-onset)*epochlen/60
+    lat_REM = (np.argmax(hypno==4)-onset)*epochlen/60
+
+    sleep_onset_after_rec_start = onset*epochlen/60 # now convert to minutes
+    sleep_offset_after_rec_start = offset*epochlen/60 # now convert to minutes
+    recording_length = len(hypno)*epochlen/60
+
+    summary = locals().copy()
+    ignore = ['verbose', 'epochlen', 'stage', 'sleep_stages', 'num', 'hypno',
+              'offset', 'onset']
+    for var in ignore:
+        del summary[var]
+
+    if verbose: pprint(summary)
+
+    return summary
+
+def infer_hypno_file(filename):
+    folder, filename = os.path.split(filename)
+    possible_names = [filename + '.txt']
+    possible_names += [filename + '.csv']
+    possible_names += [os.path.splitext(filename)[0] + '.txt']
+    possible_names += [os.path.splitext(filename)[0] + '.csv']
+    possible_names += [os.path.splitext(filename)[0] + '_hypnogram.csv']
+    possible_names += [os.path.splitext(filename)[0] + '_hypnogram.txt']
+    possible_names += [os.path.splitext(filename)[0] + '_hypno.csv']
+    possible_names += [os.path.splitext(filename)[0] + '_hypno.txt']
+
+    for file in possible_names:
+        if os.path.exists(os.path.join(folder, file)):
+            return os.path.join(folder, file)
+    warnings.warn(f'No Hypnogram found for {filename}, looked for: {possible_names}')
+    return False
+
+
+def read_hypno(hypno_file, epochlen = 30, epochlen_infile=None, mode='auto',
+               exp_seconds=None, conf_dict=None, verbose=True):
+    """
+    reads a hypnogram file as created by VisBrain or as CSV type
+    (or also some custom cases like the Dreams database)
+
+    :param hypno_file: a path to the hypnogram
+    :param epochlen: how many seconds per label in output
+    :param epochlen_infile: how many seconds per label in original file
+    :param mode: 'auto', 'time' or 'csv', see SleepDev/docs/hypnogram.md
+    :param exp_seconds: How many seconds does the matching recording have?
+    """
+    assert str(type(epochlen)()) == '0'
+    assert epochlen_infile is None or str(type(epochlen_infile)()) == '0'
+
+    if isinstance(hypno_file, str):
+        with open(hypno_file, 'r') as file:
+            content = file.read()
+            content = content.replace('\r', '') # remove windows style \r\n
+    elif isinstance(hypno_file, StringIO):
+        content = hypno_file.read()
+        content = content.replace('\r', '') # remove windows style \r\n
+
+    #conversion dictionary
+    if conf_dict is None:
+        conv_dict = {'W':0, 'WAKE':0, 'N1': 1, 'N2': 2, 'N3': 3, 'R':4, 'REM': 4, 'ART': 9,
+                     -1:9, '-1':9, **{i:i for i in range(0, 10)}, **{f'{i}':i for i in range(0, 10)}}
+
+    lines = content.split('\n')
+    if mode=='auto':
+        if lines[0].startswith('*'): # if there is a star, we assume it's the visbrain type
+            mode = 'time'
+        elif lines[0].replace('-', '')[0].isnumeric():
+            mode = 'csv'
+        elif lines[0].startswith('[HypnogramAASM]'):
+            mode = 'dreams'
+        elif lines[0].startswith(' Epoch Number ,Start Time ,Sleep Stage'):
+            mode = 'alice'
+        elif lines[0].startswith('EPOCH=') and lines[1].startswith('START='):
+            mode = 'csv'
+            lines = [l.upper() for l in lines[2:]]
+        else:
+            known_stage = [l.upper() in conv_dict for l in lines]
+            if all(known_stage):
+                mode='csv'
+            else:
+                mode=None
+
+    if mode=='time':
+        if epochlen_infile is not None:
+            warnings.warn('epochlen_infile has been supplied, but hypnogram is time based,'
+                          'will be ignored')
+        stages = []
+        prev_t = 0
+        for line in lines:
+            if len(line.strip())==0:   continue
+            if line[0] in '*#%/\\"\'': continue # this line seems to be a comment
+            s, t = line.split('\t')
+            t = float(t)
+            s = conv_dict[s]
+            l = int(np.round((t-prev_t))) # length of this stage
+            stages.extend([s]*l)
+            prev_t = t
+
+    elif mode=='csv':
+        if exp_seconds and not epochlen_infile:
+            epochlen_infile=exp_seconds//len(lines)
+            if verbose: print('[INFO] Assuming csv annotations with one entry per {} seconds'.format(epochlen_infile))
+
+        elif epochlen_infile is None:
+            if len(lines) < 2400: # we assume no recording is longer than 20 hours
+                epochlen_infile = 30
+                if verbose: print('[INFO] Assuming csv annotations are per epoch')
+            else:
+                epochlen_infile = 1
+                if verbose: print('[INFO] Assuming csv annotations are per second')
+        lines = [line.split('\t')[0] if '\t' in line else line for line in lines]
+        lines = [conv_dict[l]  if l in conv_dict else l for l in lines if len(l)>0]
+        lines = [[line]*epochlen_infile for line in lines]
+        stages = np.array([conv_dict[l] for l in np.array(lines).flatten()])
+
+    # for the Dreams Database
+    elif mode=='dreams':
+        epochlen_infile = 5
+        conv_dict = {-2:5,-1:5, 0:5, 1:3, 2:2, 3:1, 4:4, 5:0}
+        lines = [[int(line)] for line in lines[1:] if len(line)>0]
+        lines = [[line]*epochlen_infile for line in lines]
+        stages = np.array([conv_dict[l] for l in np.array(lines).flatten()])
+
+    elif mode=='alice':
+        epochlen_infile = 30
+        conv_dict = {'WK':0,'N1':1, 'N2':2, 'N3':3, 'REM':4}
+        lines = [line.split(',')[-1] for line in lines[1:] if len(line)>0]
+        lines = [[line]*epochlen_infile for line in lines]
+        try: stages = np.array([conv_dict[l] for l in np.array(lines).flatten()])
+        except KeyError as e:
+            print('Unknown sleep stage in file')
+            raise e
+    else:
+        raise ValueError('This is not a recognized hypnogram: {}'.format(hypno_file))
+
+    stages = stages[::epochlen]
+    if len(stages)==0:
+        logging.warning('hypnogram loading failed, len == 0')
+
+    return np.array(stages)
+
+
+def hypno2time(hypno, seconds_per_epoch=1):
+    """
+    Converts a hypnogram into the format as defined by visbrain
+    """
+    hypno = np.repeat(hypno, seconds_per_epoch)
+    s = '*Duration_sec {}\n'.format(len(hypno))
+    stages = ['Wake', 'N1', 'N2', 'N3', 'REM', 'Art']
+    d = dict(enumerate(stages))
+    hypno_str = [d[h] for h in hypno]
+
+    last_stage=hypno_str[0]
+
+    for second, stage in enumerate(hypno_str):
+        if stage!=last_stage:
+            s += '{}\t{}\n'.format(last_stage, second)
+            last_stage=stage
+    s += '{}\t{}\n'.format(stage, second+1)
+    return s
+
+def write_hypno_time(hypno, filename, seconds_per_annotation=30, comment=None, overwrite=False):
+    """
+    Save hypnogram data with visbrain style
+    The exact onset of each sleep stage is annotated in time space.
+    This format is recommended for saving hypnograms
+
+    :param filename: where to save the data
+    :param hypno: The hypnogram either as list or np.array
+    :param seconds_per_epoch: How many seconds each annotation contains
+    :param overwrite: overwrite file?
+    """
+    assert not os.path.exists(filename) or overwrite, 'File already exists, no overwrite'
+    hypno = np.repeat(hypno, seconds_per_annotation)
+    hypno_str = hypno2time(hypno)
+    if comment is not None:
+        comment = comment.replace('\n', '\n*')
+        hypno_str = '*' + comment + '\n' + hypno_str
+        hypno_str = hypno_str.replace('\n\n', '\n')
+    with open(filename, 'w') as f:
+        f.write(hypno_str)
+    return True
+
+
+def write_hypno_csv(hypno, filename, seconds_per_annotation = 30, mode = 'seconds',
+                    overwrite = False):
+    """
+    Save hypnogram data. Expects hypnogram to be based on epoch basis.
+    it is saved as a csv-style file with one entry per second (default) and a new-line as separator
+
+    :param filename: where to save the data
+    :param hypno: The hypnogram either as list or np.array
+    :param seconds_per_annotation: how many seconds does one annotation account for
+    :param mode: 'seconds' or 'epochs':
+                 'seconds' : writes one annotation per second
+                 'epochs': write one annotation per 30 seconds
+    :param overwrite: overwrite file?
+    """
+    assert not os.path.exists(filename) or overwrite, 'File already exists, no overwrite'
+    assert mode in ['seconds', 'epochs'],'Mode must be seconds or epochs, is {}'.format(mode)
+    hypno = np.array(hypno, copy=False)
+    try:
+        if np.any(np.logical_or(hypno>5, hypno<0)):
+            raise ValueError('Contains values outside of [0, 5], which stage should that be?? ')
+        with open(filename, 'w') as f:
+            hypno_rep = [str(v) for v in np.repeat(hypno, seconds_per_annotation)]
+            if mode=='epochs':
+                hypno_rep = hypno_rep[::30]
+            hypno_str = '\n'.join(hypno_rep)
+            f.write(hypno_str)
+    except Exception as e:
+        print(e)
+        return False
+    return True
+
+
+def write_hypno(hypno, filename, mode='time', seconds_per_annotation = 30, comment = None,
+                overwrite = False):
+    """
+    Writes a hypnogram to file
+
+        0 Wake
+        1 N1
+        2 N2
+        3 N3
+        4 REM
+        5 Artefact / unknown
+
+    :param filename: the filename under which to save a hypnogram
+    :param hypno: a 1D array with sleep stage annotations.
+    :param mode: 'time' or 'csv'
+                 time: will save with the visbrain format (default)
+                 csv: will save as a simple csv file
+    :param seconds_per_annotation: how many seconds does one annotation account for
+    :param comment: A comment that is added to the beginning if the file
+    :param overwrite: Overwrite file if already present?
+    """
+
+    assert seconds_per_annotation>=1
+    if mode=='time':
+        if not filename.endswith('.hypno'):
+            warnings.warn('Filename ends in ".{}", recommended to end in .hypno'.format(
+                           os.path.splitext(filename)[1]))
+        write_hypno_time(hypno, filename, seconds_per_annotation=seconds_per_annotation,
+                         comment=comment, overwrite=overwrite)
+    elif mode=='csv':
+        write_hypno_csv(hypno, filename, seconds_per_annotation=seconds_per_annotation,
+                        overwrite=overwrite)
+    else:
+        raise ValueError('Unkown mode {}, must be time or csv'.format(mode))
+
+
+
+
+def transform_hypno(hypno, t_dict):
+    """
+    Will transform the hypnogram according to a lookup dictionary
+    :param data: input data, will not be altered
+    :param hypno: a hypnogram
+    :param t_dict: a dictionary with lookup values.
+                   if a value of hypno is not in t_dict it will not be altered
+    :returns: data, new_hypnogram
+    """
+    hypno_values = np.unique(hypno)
+    mapping = {h:h for h in hypno_values}
+    mapping.update(t_dict)
+    new_hypno = [mapping[h] for h in hypno]
+    if type(hypno)==np.ndarray: new_hypno = np.array(new_hypno, dtype=hypno.dtype)
+    return  new_hypno
+
+def convert_hypnogram(hypno_file_in, hypno_file_out, **kwargs):
+    """
+    takes an arbitrary hypnogram and converts it to a time based format
+
+    :param hypno_file_in:  A string pointing to a hypnogrma file
+    :param hypno_file_out: Where the converted hypnogram should be saved
+    """
+    assert not os.path.exists(hypno_file_out)
+    hypno = read_hypno(hypno_file_in, **kwargs)
+    return write_hypno(hypno, hypno_file_out)
+
+
+def _time_format(seconds):
+    """ returns a string with a fitting string"""
+    return '{:02d}:{:02d} hours'.format(seconds//3600, seconds%3600//60)
+
+
+def _stamp_to_dt(utc_stamp):
+    """Convert timestamp to datetime object in Windows-friendly way."""
+    if 'datetime' in str(type(utc_stamp)): return utc_stamp
+    # The min on windows is 86400
+    stamp = [int(s) for s in utc_stamp]
+    if len(stamp) == 1:  # In case there is no microseconds information
+        stamp.append(0)
+    return (datetime.fromtimestamp(0, tz=timezone.utc) +
+            timedelta(0, stamp[0], stamp[1]))  # day, sec, μs
+
+
+def write_mne_edf(mne_raw, fname, picks=None, tmin=0, tmax=None,
+                  overwrite=False, verbose=False):
+    """
+    Saves the raw content of an MNE.io.Raw and its subclasses to
+    a file using the EDF+/BDF filetype
+    pyEDFlib is used to save the raw contents of the RawArray to disk
+    Parameters
+    ----------
+    mne_raw : mne.io.Raw
+        An object with super class mne.io.Raw that contains the data
+        to save
+    fname : string
+        File name of the new dataset. This has to be a new filename
+        unless data have been preloaded. Filenames should end with .edf
+    picks : array-like of int | None
+        Indices of channels to include. If None all channels are kept.
+    tmin : float | None
+        Time in seconds of first sample to save. If None first sample
+        is used.
+    tmax : float | None
+        Time in seconds of last sample to save. If None last sample
+        is used.
+    overwrite : bool
+        If True, the destination file (if it exists) will be overwritten.
+        If False (default), an error will be raised if the file exists.
+    """
+    import pyedflib # pip install pyedflib
+    from pyedflib import FILETYPE_BDF, FILETYPE_BDFPLUS, FILETYPE_EDF, FILETYPE_EDFPLUS
+    if not issubclass(type(mne_raw), mne.io.BaseRaw):
+        raise TypeError('Must be mne.io.Raw type')
+    if not overwrite and os.path.exists(fname):
+        raise OSError('File already exists. No overwrite.')
+
+    # static settings
+    has_annotations = True if len(mne_raw.annotations)>0 else False
+    if os.path.splitext(fname)[-1] == '.edf':
+        file_type = FILETYPE_EDFPLUS if has_annotations else FILETYPE_EDF
+        dmin, dmax = -32768, 32767
+    else:
+        file_type = FILETYPE_BDFPLUS if has_annotations else FILETYPE_BDF
+        dmin, dmax = -8388608, 8388607
+
+    print('saving to {}, filetype {}'.format(fname, file_type))
+    sfreq = mne_raw.info['sfreq']
+    date = _stamp_to_dt(mne_raw.info['meas_date'])
+
+    if tmin:
+        date += timedelta(seconds=tmin)
+    # no conversion necessary, as pyedflib can handle datetime.
+    #date = date.strftime('%d %b %Y %H:%M:%S')
+    first_sample = int(sfreq*tmin)
+    last_sample  = int(sfreq*tmax) if tmax is not None else None
+
+
+    # convert data
+    channels = mne_raw.get_data(picks,
+                                start = first_sample,
+                                stop  = last_sample)
+
+    # convert to microvolts to scale up precision
+    eeg_chs = [ch_type=='eeg' for ch_type in mne_raw.get_channel_types()]
+    channels[eeg_chs,:] *= 1e6
+
+    # set conversion parameters
+    n_channels = len(channels)
+
+    # create channel from this
+    try:
+        f = pyedflib.EdfWriter(fname,
+                               n_channels=n_channels,
+                               file_type=file_type)
+
+        channel_info = []
+
+        ch_idx = range(n_channels) if picks is None else picks
+        keys = list(mne_raw._orig_units.keys())
+        for i in ch_idx:
+            try:
+                ch_dict = {'label': mne_raw.ch_names[i],
+                           'dimension': mne_raw._orig_units[keys[i]],
+                           'sample_rate': mne_raw._raw_extras[0]['n_samps'][i],
+                           'physical_min': mne_raw._raw_extras[0]['physical_min'][i],
+                           'physical_max': mne_raw._raw_extras[0]['physical_max'][i],
+                           'digital_min':  mne_raw._raw_extras[0]['digital_min'][i],
+                           'digital_max':  mne_raw._raw_extras[0]['digital_max'][i],
+                           'transducer': '',
+                           'prefilter': ''}
+            except:
+                ch_dict = {'label': mne_raw.ch_names[i],
+                           'dimension': mne_raw._orig_units[keys[i]],
+                           'sample_rate': sfreq,
+                           'physical_min': channels[i].min(),
+                           'physical_max': channels[i].max(),
+                           'digital_min':  dmin,
+                           'digital_max':  dmax,
+                           'transducer': '',
+                           'prefilter': ''}
+
+            channel_info.append(ch_dict)
+
+        subject_info = mne_raw._raw_extras[0].get('subject_info',{})
+        f.setPatientCode(subject_info.get('id', '0'))
+        f.setPatientName(subject_info.get('name', 'noname'))
+        f.setTechnician('mne-gist-save-edf-skjerns')
+        f.setSignalHeaders(channel_info)
+        f.setStartdatetime(date)
+        f.writeSamples(channels)
+
+        for annotation in mne_raw.annotations:
+            onset = annotation['onset']
+            duration = annotation['duration']
+            description = annotation['description']
+            f.writeAnnotation(onset, duration, description)
+
+    except Exception as e:
+        raise e
+    finally:
+        f.close()
+    return True
```

### Comparing `sleep-utils-1.15/sleep_utils.egg-info/PKG-INFO` & `sleep-utils-1.16/sleep_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleep-utils
-Version: 1.15
+Version: 1.16
 Summary: A collection of tools for sleep research
 Home-page: http://github.com/skjerns/sleep-utils
 Author: skjerns
 Author-email: nomail@nomail.com
 License: GNU 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

