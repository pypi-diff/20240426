# Comparing `tmp/gaiaAssociation-1.2.2.tar.gz` & `tmp/gaiaAssociation-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaiaAssociation-1.2.2.tar", last modified: Sun Mar 31 20:48:07 2024, max compression
+gzip compressed data, was "gaiaAssociation-1.2.4.tar", last modified: Fri Apr 26 17:58:57 2024, max compression
```

## Comparing `gaiaAssociation-1.2.2.tar` & `gaiaAssociation-1.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 samuelrosean   (501) staff       (20)        0 2024-03-31 20:48:07.040180 gaiaAssociation-1.2.2/
--rw-r--r--   0 samuelrosean   (501) staff       (20)     1075 2023-03-15 22:44:54.000000 gaiaAssociation-1.2.2/LICENSE
--rw-r--r--   0 samuelrosean   (501) staff       (20)      829 2024-03-31 20:48:07.039949 gaiaAssociation-1.2.2/PKG-INFO
--rw-r--r--   0 samuelrosean   (501) staff       (20)    10398 2024-03-12 14:33:27.000000 gaiaAssociation-1.2.2/README.md
-drwxr-xr-x   0 samuelrosean   (501) staff       (20)        0 2024-03-31 20:48:07.038300 gaiaAssociation-1.2.2/gaiaAssociation/
--rw-r--r--   0 samuelrosean   (501) staff       (20)        0 2023-09-09 00:18:41.000000 gaiaAssociation-1.2.2/gaiaAssociation/__init__.py
--rw-r--r--   0 samuelrosean   (501) staff       (20)    43036 2024-03-31 20:42:16.000000 gaiaAssociation-1.2.2/gaiaAssociation/gaiaAssociation.py
-drwxr-xr-x   0 samuelrosean   (501) staff       (20)        0 2024-03-31 20:48:07.039668 gaiaAssociation-1.2.2/gaiaAssociation.egg-info/
--rw-r--r--   0 samuelrosean   (501) staff       (20)      829 2024-03-31 20:48:06.000000 gaiaAssociation-1.2.2/gaiaAssociation.egg-info/PKG-INFO
--rw-r--r--   0 samuelrosean   (501) staff       (20)      363 2024-03-31 20:48:07.000000 gaiaAssociation-1.2.2/gaiaAssociation.egg-info/SOURCES.txt
--rw-r--r--   0 samuelrosean   (501) staff       (20)        1 2024-03-31 20:48:06.000000 gaiaAssociation-1.2.2/gaiaAssociation.egg-info/dependency_links.txt
--rw-r--r--   0 samuelrosean   (501) staff       (20)       62 2024-03-31 20:48:06.000000 gaiaAssociation-1.2.2/gaiaAssociation.egg-info/entry_points.txt
--rw-r--r--   0 samuelrosean   (501) staff       (20)        1 2024-03-31 20:48:06.000000 gaiaAssociation-1.2.2/gaiaAssociation.egg-info/not-zip-safe
--rw-r--r--   0 samuelrosean   (501) staff       (20)      112 2024-03-31 20:48:06.000000 gaiaAssociation-1.2.2/gaiaAssociation.egg-info/requires.txt
--rw-r--r--   0 samuelrosean   (501) staff       (20)       16 2024-03-31 20:48:06.000000 gaiaAssociation-1.2.2/gaiaAssociation.egg-info/top_level.txt
--rw-r--r--   0 samuelrosean   (501) staff       (20)       38 2024-03-31 20:48:07.040242 gaiaAssociation-1.2.2/setup.cfg
--rw-r--r--   0 samuelrosean   (501) staff       (20)     1155 2024-03-31 20:48:00.000000 gaiaAssociation-1.2.2/setup.py
+drwxr-xr-x   0 samuelrosean   (501) staff       (20)        0 2024-04-26 17:58:57.874904 gaiaAssociation-1.2.4/
+-rw-r--r--   0 samuelrosean   (501) staff       (20)     1075 2023-03-15 22:44:54.000000 gaiaAssociation-1.2.4/LICENSE
+-rw-r--r--   0 samuelrosean   (501) staff       (20)      829 2024-04-26 17:58:57.874695 gaiaAssociation-1.2.4/PKG-INFO
+-rw-r--r--   0 samuelrosean   (501) staff       (20)    11098 2024-03-31 21:10:28.000000 gaiaAssociation-1.2.4/README.md
+drwxr-xr-x   0 samuelrosean   (501) staff       (20)        0 2024-04-26 17:58:57.873270 gaiaAssociation-1.2.4/gaiaAssociation/
+-rw-r--r--   0 samuelrosean   (501) staff       (20)        0 2023-09-09 00:18:41.000000 gaiaAssociation-1.2.4/gaiaAssociation/__init__.py
+-rw-r--r--   0 samuelrosean   (501) staff       (20)    43639 2024-04-26 17:53:23.000000 gaiaAssociation-1.2.4/gaiaAssociation/gaiaAssociation.py
+drwxr-xr-x   0 samuelrosean   (501) staff       (20)        0 2024-04-26 17:58:57.874437 gaiaAssociation-1.2.4/gaiaAssociation.egg-info/
+-rw-r--r--   0 samuelrosean   (501) staff       (20)      829 2024-04-26 17:58:57.000000 gaiaAssociation-1.2.4/gaiaAssociation.egg-info/PKG-INFO
+-rw-r--r--   0 samuelrosean   (501) staff       (20)      363 2024-04-26 17:58:57.000000 gaiaAssociation-1.2.4/gaiaAssociation.egg-info/SOURCES.txt
+-rw-r--r--   0 samuelrosean   (501) staff       (20)        1 2024-04-26 17:58:57.000000 gaiaAssociation-1.2.4/gaiaAssociation.egg-info/dependency_links.txt
+-rw-r--r--   0 samuelrosean   (501) staff       (20)       62 2024-04-26 17:58:57.000000 gaiaAssociation-1.2.4/gaiaAssociation.egg-info/entry_points.txt
+-rw-r--r--   0 samuelrosean   (501) staff       (20)        1 2024-04-26 17:58:57.000000 gaiaAssociation-1.2.4/gaiaAssociation.egg-info/not-zip-safe
+-rw-r--r--   0 samuelrosean   (501) staff       (20)      112 2024-04-26 17:58:57.000000 gaiaAssociation-1.2.4/gaiaAssociation.egg-info/requires.txt
+-rw-r--r--   0 samuelrosean   (501) staff       (20)       16 2024-04-26 17:58:57.000000 gaiaAssociation-1.2.4/gaiaAssociation.egg-info/top_level.txt
+-rw-r--r--   0 samuelrosean   (501) staff       (20)       38 2024-04-26 17:58:57.874953 gaiaAssociation-1.2.4/setup.cfg
+-rw-r--r--   0 samuelrosean   (501) staff       (20)     1155 2024-04-26 17:57:16.000000 gaiaAssociation-1.2.4/setup.py
```

### Comparing `gaiaAssociation-1.2.2/LICENSE` & `gaiaAssociation-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gaiaAssociation-1.2.2/PKG-INFO` & `gaiaAssociation-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaiaAssociation
-Version: 1.2.2
+Version: 1.2.4
 Summary: Compare ATAC-seq data to loci.
 Home-page: https://github.com/samrosean/gaiaAssociation
 Author: Samuel Rosean
 Author-email: samuel.rosean@einsteinmed.edu
 License: MIT
 Keywords: ATAC-seq loci enrichment
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gaiaAssociation-1.2.2/README.md` & `gaiaAssociation-1.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 
  https://pip.pypa.io/en/stable/installation/
 
 The above link will also help if you need to upgrade or update your pip installation.
 
 ### Installing Required Libraries
 		
-gaiaAssociation requires seven python dependancies: scipy, pandas, numpy, pyranges, seaborn, matplotlib, and setuptools. When installing gaiaAssociation through pip it will attempt to resolve these dependencies and install the necceassary versions. If this fails, each package can be downloaded using pip, for example:
+gaiaAssociation requires seven python dependancies: scipy, pandas, numpy, pyranges, seaborn, matplotlib, and setuptools. When installing gaiaAssociation through pip it will attempt to resolve these dependencies and install the necceassary versions. If this fails, each package can be downloaded individually using pip, for example:
 
     pip install scipy
 		
 ## Step 1: Install gaiaAssociation
 	
-### PyPi
+### PyPi (Recommended)
 
 #### For Command Line Usage:
 
 To install gaiaAssociation from pypi, run a pip command to install it from the pypi distribution archive
 
 	pip install gaiaAssociation
 
@@ -61,32 +61,58 @@
 
 This will allow you to use gaia inline as a python function:
 
 	gaiaAssociation.gaiaAssociation.gaiaAssociation("User/OCRfiles", "/User/lociFiles", "/User/chrsize.csv", "/User/Output", lociSelection = "/Users/lociGroups.tsv", windowSize = 10000)
 
 ### Github
 
-You can also download the source package from this github repository
+You can also download the source package from this github repository, or through the terminal using the command given below (though we only recommend this method for people with experience building python packages and managing python environments):
+
+	wget https://github.com/GreallyLab/gaiaAssociation/archive/main.zip
+
+And then unpacking this zip file using the command.
+
+	unzip main.zip
 
 From the location of this newly installed copy of the gaiaAssociation repository, run the setup command
 
 	python setup.py install
 
-Gaia will now be runnable from the command line as described above.
+Gaia will now be runnable from the command line as described above within this folder.
 
 ## Step 2: Using gaiaAssociation:
 
 A detailed guide and example notebook for using Gaia within a jupyter notebook environment can be found [here](https://github.com/GreallyLab/gaiaAssociation-Example-Guide).
 
 
 When using gaiaAssociation on the command line you can check your installation and to get basic information on using gaiaAssociation by typing this command into your terminal.
 
 	gaia --help
 
-If correctly installed it should print out useful information about each variable and the flag to associate with each. gaiaAssocation has four required arguments, and five optional arguments. The four required arguments, which define a basic run are:
+If correctly installed it should print out useful information about each variable and the flag to associate with each. gaiaAssocation has four required arguments, and five optional arguments. 
+
+#### A Basic Run
+
+A default run on the command line using just the required arguments will therefore look like:
+
+```
+gaia \
+-a user/documents/atac \
+-g user/documents/loci \
+-c user/chrom/chrsize.csv \
+-o user/documents/output
+```
+
+And a default run in a python notebook will look like:
+
+```
+gaiaAssociation.gaiaAssociation.gaiaAssociation("user/documents/atac", "user/documents/loci", "user/chrom/chrsize.csv", user/documents/output")
+```
+
+The four required arguments, which define a basic run are:
 
 #### Required Arguments
 
 OCR Folder: the folder location of the OCR bed files stored in .txt format. The first three columns should be labeled “Chromosome”, “Start”, and “End” in that order.
 
 	-a, --atac  (either flag will work)
 
@@ -99,26 +125,14 @@
 
 	-c, --chrom (either flag will work)
 
 Output Folder: The folder location you want the results to be output into. If this folder does not already exist gaia will attempt to make it. If it does not have the permissions to do so it will exit and the user will have to run it with folder creating permissions, or they will have to make the folder themselves.
 
 	-o, --output (either flag will work)
 
-A default run on the command line will therefore look like:
-
-```
-gaia -a user/documents/atac -g user/documents/loci -c user/chrom/chrsize.csv -o user/documents/output
-```
-
-A default run in python will look like:
-
-```
-gaiaAssociation("user/documents/atac", "user/documents/loci", "user/chrom/chrsize.csv", user/documents/output")
-```
-
 #### Optional Arguments
 
 Peak Uniqueness: a cutoff value for OCR uniqueness (e.g. if given 12, then any atac peak found in more than 12 atac sets will be removed from all of them) - by default uniqueness is not considered).
 
 ```
   -u, --peakUniqueness
 ```
@@ -146,29 +160,37 @@
 ```
   -w, --windowSize
 ```
 
 A run from the command line using these flags will therfore look like:
 
 ```
-gaia -a user/documents/atac -g user/documents/loci -c user/chrom/chrsize.csv -o user/documents/output -l 2000 -u 10 -m user/documents/mask.txt -w 1000000
+gaia \
+-a user/documents/atac \
+-g user/documents/loci \
+-c user/chrom/chrsize.csv \
+-o user/documents/output \
+-l 2000 \
+-u 10 \
+-m user/documents/mask.txt \
+-w 1000000
 ```
 
 Within a python file it will look like:
 
 ```
 gaiaAsscoiation("user/documents/atac", "user/documents/loci", "user/chrom/chrsize.csv", "user/documents/output", lociCutoff = 2000, peakUniqueness = 10, maskRegion = "user/documents/mask.txt", windowSize = 1000000)
 ```
 ## Additional Notes
 
 1. Gaia is designed to be run on tsv and csv files in a utf-8 encoding format. Problems may arise from using files encoded in a different format, we recommend you ensure files are saved in this encoder if errors are occuring.
 
-2. Gaia does not have a built in genome build. Since the user provides the chromosome sizes, the OCR bed files, and the loci, as long as all three of these files are based on the same genome build it will run regardless of species/genome build.
+2. Gaia does not have a built in genome build. Since the user provides the chromosome sizes, the OCR bed files, and the loci, as long as all three of these files are based on the same genome build it will run regardless of species/genome build. However, this does require that the user be vigilant, as results will still be generated if you compare OCRs from the a different genome build to the loci, these results will just be biologically meaningless.
 
 3. Files inputted into Gaia do not need to be sorted. The loci files or bed files do not need to be sorted for Gaia to properly run.
 
 
 ## How Gaia Works:
 
 By dividing each chromsome into roughly equivalent gaia window sizes based on a user-given value, enrichment is modeled as a binomial variable for each window where loci are found (wherein the probability is determined by the proportion of the window covered by open chromatin regions and the count is number of loci found within that window). The sum of these binomial variables are compared against the number of global overlaps between a cell-type's OCRs and the given loci set. The non-identical binomial variables are summed utilizing the method developed by Boxiang Liu and Thomas Quertermous (https://journal.r-project.org/archive/2018/RJ-2018-011/RJ-2018-011.pdf).
 
-### Version 1.2.0
+### Version 1.2.1
```

### Comparing `gaiaAssociation-1.2.2/gaiaAssociation/gaiaAssociation.py` & `gaiaAssociation-1.2.4/gaiaAssociation/gaiaAssociation.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 
 Compare Open Chromatin Regions (e.g. ATAC-seq, DNase-seq) against loci sets (e.g. de-novo mutations, SNPs, rare variants) to detect cell-specific enrichment of loci.
 
 Find the documentation at https://github.com/GreallyLab/gaiaAssociation
 
 For help contact Samuel Rosean, samuel.rosean@einsteinmed.edu --- https://github.com/samrosean
 
-Named for James Lovelock's Gaia Hypothesis
-
+Named after James Lovelock's Gaia Hypothesis
 
+####
 '''
 
 ##Primary function for associating ATAC and GWAS
 def gaiaAssociation(atacLocation, gwasLocation, chromosomeSize, outputLocation, uniqueCount=0, lociCutoff=0, lociSelection = 0, subsettingRegion=0, windowSize = 100000, overlapSaveValue=1):
         
     ## ensure all the given locations and files are accesible and real
     if not os.path.exists(atacLocation):
@@ -589,76 +589,85 @@
             dictWindows[reorderCellNames[count] + gwasNames[count2]] = list(tempRange2.NumberOverlaps)
             
             ## If Indels exist we need to do some more expansive calculations
             if indels == True:
             
                 ## if indels exist in this particular gwas set continue on to indel caluclations
                 if gwasNonZeroPyranges[count2]:
-                
-                    ##Grab all indels that overlap with the current ATAC set
-                    indelRangeTemp = gwasNonZeroPyranges[count2].coverage(item)
-                    indelOverlap = indelRangeTemp.df
-                    
-                    ## keep only those that overlap
-                    indelOverlap = indelOverlap[indelOverlap["NumberOverlaps"] > 0]
-                    
-                    ##now create a list of every bp where an indel exists at
-                    indelOverlap = indelOverlap.reset_index(drop=True)
-                    indelOverlap['range']=indelOverlap.apply(lambda x : list(range(x['Start'],x['End'])),1)
-                    indelChroDict = {}
-                    for item in list(set(indelOverlap.Chromosome)):
-                        indelChroLoop = indelOverlap[indelOverlap["Chromosome"] == item]
-                        indelLoopLocations = [item for sublist in indelChroLoop["range"] for item in sublist]
-                        indelChroDict[item] = indelLoopLocations
-                    
-                    indelExtraOverlap = []
-                    
-                    ##Get the number of these overlaps for each window so we can add them to the count
-                    indelDoubleOverlap = indelOverlap.drop(['range', 'NumberOverlaps'], axis=1)
-                    indelDoubleOverlap = pr.PyRanges(indelDoubleOverlap)
-                    doubleOverlapCount = windowsRange.coverage(indelDoubleOverlap)
-                    doubleOverlapList = list(doubleOverlapCount.NumberOverlaps)
+                    if item:
                     
-                    ## for each window space, find how much length of indel exists in the window
-                    for windowCount, windowItem in enumerate(windowStarts):
-                            
-                        if windowChrs[windowCount] in indelChroDict:
-                            indelWindowSize = [num for num in indelChroDict[windowChrs[windowCount]] if num <= windowEnds[windowCount] and num >= windowStarts[windowCount]]
-                        else:
-                            indelWindowSize = []
+                        ##Grab all indels that overlap with the current ATAC set
+                        print("GWAS")
+                        print(gwasNonZeroPyranges[count2])
+                        print("ATAC")
+                        print(item)
+                        print("Count #")
+                        print(count2)
+                        print("---")
+                        indelRangeTemp = gwasNonZeroPyranges[count2].coverage(item)
+                        
+                        indelOverlap = indelRangeTemp.df
+                        
+                        ## keep only those that overlap
+                        indelOverlap = indelOverlap[indelOverlap["NumberOverlaps"] > 0]
+                        
+                        ##now create a list of every bp where an indel exists at
+                        indelOverlap = indelOverlap.reset_index(drop=True)
+                        indelOverlap['range']=indelOverlap.apply(lambda x : list(range(x['Start'],x['End'])),1)
+                        indelChroDict = {}
+                        for itemChr in list(set(indelOverlap.Chromosome)):
+                            indelChroLoop = indelOverlap[indelOverlap["Chromosome"] == itemChr]
+                            indelLoopLocations = [itemx for sublist in indelChroLoop["range"] for itemx in sublist]
+                            indelChroDict[item] = indelLoopLocations
+                        
+                        indelExtraOverlap = []
+                        
+                        ##Get the number of these overlaps for each window so we can add them to the count
+                        indelDoubleOverlap = indelOverlap.drop(['range', 'NumberOverlaps'], axis=1)
+                        indelDoubleOverlap = pr.PyRanges(indelDoubleOverlap)
+                        doubleOverlapCount = windowsRange.coverage(indelDoubleOverlap)
+                        doubleOverlapList = list(doubleOverlapCount.NumberOverlaps)
+                        
+                        ## for each window space, find how much length of indel exists in the window
+                        for windowCount, windowItem in enumerate(windowStarts):
+                                
+                            if windowChrs[windowCount] in indelChroDict:
+                                indelWindowSize = [num for num in indelChroDict[windowChrs[windowCount]] if num <= windowEnds[windowCount] and num >= windowStarts[windowCount]]
+                            else:
+                                indelWindowSize = []
+                                
+                            ## if none exist, add zero to list of indel overlap, if it does add the total number of bp that do
+                            if len(indelWindowSize) == 0:
+                                indelExtraOverlap.append(0)
+                            else:
+                                indelSize = len(indelWindowSize)
+                                indelExtraOverlap.append(indelSize)
                             
-                        ## if none exist, add zero to list of indel overlap, if it does add the total number of bp that do
-                        if len(indelWindowSize) == 0:
-                            indelExtraOverlap.append(0)
-                        else:
-                            indelSize = len(indelWindowSize)
-                            indelExtraOverlap.append(indelSize)
+                        ##grab the number of peaks per window
+                        listCount = dictWindows[reorderCellNames[count] + "PeakCount"]
                         
-                    ##grab the number of peaks per window
-                    listCount = dictWindows[reorderCellNames[count] + "PeakCount"]
-                    
-                    ##multiply the extra length we need to add to every atac peak within every window
-                    listSize = [a*b for a,b in zip(listCount,indelExtraOverlap)]
-                    
-                    ## take this extra size to calculate an added probability
-                    listProb = [a/b for a,b in zip(listSize, dictWindows["Size"])]
-                    
-                    ##Add this probability to the base probability for a gwas specific probability
-                    dictWindows[reorderCellNames[count]+ gwasNames[count2] + "Prob"] = [a+b for a,b in zip(dictWindows[reorderCellNames[count]], listProb)]
-                    
-                    ##Add number of indel overlaps
-                    dictWindows[reorderCellNames[count] + gwasNames[count2] + "IndelOverlap"] =  doubleOverlapList
-                    
-                    ## Get the total number of indels in region to add to count
-                    totalIndelRange = windowsRange.coverage(gwasNonZeroPyranges[count2])
-                    totalIndelList = list(totalIndelRange.NumberOverlaps)
+                        ##multiply the extra length we need to add to every atac peak within every window
+                        listSize = [a*b for a,b in zip(listCount,indelExtraOverlap)]
+                        
+                        ## take this extra size to calculate an added probability
+                        listProb = [a/b for a,b in zip(listSize, dictWindows["Size"])]
+                        
+                        ##Add this probability to the base probability for a gwas specific probability
+                        dictWindows[reorderCellNames[count]+ gwasNames[count2] + "Prob"] = [a+b for a,b in zip(dictWindows[reorderCellNames[count]], listProb)]
+                        
+                        ##Add number of indel overlaps
+                        dictWindows[reorderCellNames[count] + gwasNames[count2] + "IndelOverlap"] =  doubleOverlapList
+                        
+                        ## Get the total number of indels in region to add to count
+                        totalIndelRange = windowsRange.coverage(gwasNonZeroPyranges[count2])
+                        totalIndelList = list(totalIndelRange.NumberOverlaps)
+                        
+                        ## add the count of indels to the original gwas count
+                        dictWindows[reorderCellNames[count] + gwasNames[count2]] = [a+b for a,b in zip(dictWindows[reorderCellNames[count] + gwasNames[count2]], totalIndelList)]
                     
-                    ## add the count of indels to the original gwas count
-                    dictWindows[reorderCellNames[count] + gwasNames[count2]] = [a+b for a,b in zip(dictWindows[reorderCellNames[count] + gwasNames[count2]], totalIndelList)]
-                
 
     ## check to see if you can make a subfolder
     if not os.path.exists(outputLocation+ '/overlaps'):
         os.mkdir(outputLocation + '/overlaps')
         if not os.path.exists(outputLocation + '/overlaps'):
             print("Output folder cannot be modified, so overlaps will not be saved. Try running again with higher permissions.")
             overlapSave = False
```

### Comparing `gaiaAssociation-1.2.2/gaiaAssociation.egg-info/PKG-INFO` & `gaiaAssociation-1.2.4/gaiaAssociation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaiaAssociation
-Version: 1.2.2
+Version: 1.2.4
 Summary: Compare ATAC-seq data to loci.
 Home-page: https://github.com/samrosean/gaiaAssociation
 Author: Samuel Rosean
 Author-email: samuel.rosean@einsteinmed.edu
 License: MIT
 Keywords: ATAC-seq loci enrichment
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gaiaAssociation-1.2.2/setup.py` & `gaiaAssociation-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('requirements.txt') as f:
     requirements = f.readlines()
   
 long_description = 'Compare ATAC-seq datasets against loci datasets to see if there is a specific enrichment between a particular loci set in a cell type'
   
 setup(
         name ='gaiaAssociation',
-        version ='1.2.2',
+        version ='1.2.4',
         author ='Samuel Rosean',
         author_email ='samuel.rosean@einsteinmed.edu',
         url ='https://github.com/samrosean/gaiaAssociation',
         description ='Compare ATAC-seq data to loci.',
         long_description = long_description,
         long_description_content_type ="text/markdown",
         license ='MIT',
```

