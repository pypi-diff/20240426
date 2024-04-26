# Comparing `tmp/STASCAN-1.0.0.tar.gz` & `tmp/STASCAN-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STASCAN-1.0.0.tar", last modified: Wed Aug 30 07:30:30 2023, max compression
+gzip compressed data, was "dist\STASCAN-1.1.0.tar", last modified: Fri Apr 26 10:08:21 2024, max compression
```

## Comparing `STASCAN-1.0.0.tar` & `STASCAN-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 wuying    (1659) yangyg_group  (1015)        0 2023-08-30 06:30:20.919134 STASCAN-1.0.0/
--rw-r--r--   0 wuying    (1659) yangyg_group  (1015)     1064 2023-08-26 08:57:15.000000 STASCAN-1.0.0/LICENSE.txt
--rw-r--r--   0 wuying    (1659) yangyg_group  (1015)      658 2023-08-30 06:30:20.917738 STASCAN-1.0.0/PKG-INFO
--rw-r--r--   0 wuying    (1659) yangyg_group  (1015)       18 2023-08-30 07:24:04.000000 STASCAN-1.0.0/README.rst
-drwxr-xr-x   0 wuying    (1659) yangyg_group  (1015)        0 2023-08-30 06:30:20.893511 STASCAN-1.0.0/STASCAN/
--rw-r--r--   0 wuying    (1659) yangyg_group  (1015)    13398 2023-08-14 13:48:10.000000 STASCAN-1.0.0/STASCAN/StatPlot.py
--rw-r--r--   0 wuying    (1659) yangyg_group  (1015)      623 2023-08-27 14:31:13.000000 STASCAN-1.0.0/STASCAN/__init__.py
--rw-r--r--   0 wuying    (1659) yangyg_group  (1015)     6102 2023-08-11 07:49:00.000000 STASCAN-1.0.0/STASCAN/downstream.py
--rw-r--r--   0 wuying    (1659) yangyg_group  (1015)     9926 2023-08-26 08:44:34.000000 STASCAN-1.0.0/STASCAN/model.py
--rw-r--r--   0 wuying    (1659) yangyg_group  (1015)    17999 2023-08-25 13:08:12.000000 STASCAN-1.0.0/STASCAN/preparation.py
--rw-r--r--   0 wuying    (1659) yangyg_group  (1015)    19628 2023-08-28 06:50:27.000000 STASCAN-1.0.0/STASCAN/run_STASCAN.py
-drwxr-xr-x   0 wuying    (1659) yangyg_group  (1015)        0 2023-08-30 06:30:20.913905 STASCAN-1.0.0/STASCAN.egg-info/
--rw-r--r--   0 wuying    (1659) yangyg_group  (1015)      658 2023-08-30 06:30:20.000000 STASCAN-1.0.0/STASCAN.egg-info/PKG-INFO
--rw-r--r--   0 wuying    (1659) yangyg_group  (1015)      340 2023-08-30 06:30:20.000000 STASCAN-1.0.0/STASCAN.egg-info/SOURCES.txt
--rw-r--r--   0 wuying    (1659) yangyg_group  (1015)        1 2023-08-30 06:30:20.000000 STASCAN-1.0.0/STASCAN.egg-info/dependency_links.txt
--rw-r--r--   0 wuying    (1659) yangyg_group  (1015)        1 2023-08-29 08:34:36.000000 STASCAN-1.0.0/STASCAN.egg-info/not-zip-safe
--rw-r--r--   0 wuying    (1659) yangyg_group  (1015)        9 2023-08-30 06:30:20.000000 STASCAN-1.0.0/STASCAN.egg-info/requires.txt
--rw-r--r--   0 wuying    (1659) yangyg_group  (1015)        8 2023-08-30 06:30:20.000000 STASCAN-1.0.0/STASCAN.egg-info/top_level.txt
--rw-r--r--   0 wuying    (1659) yangyg_group  (1015)       38 2023-08-30 06:30:20.920134 STASCAN-1.0.0/setup.cfg
--rw-r--r--   0 wuying    (1659) yangyg_group  (1015)     1154 2023-08-30 07:30:16.000000 STASCAN-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 10:08:21.000000 STASCAN-1.1.0/
+-rw-rw-rw-   0        0        0      653 2024-04-26 10:08:21.000000 STASCAN-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-26 10:08:21.000000 STASCAN-1.1.0/STASCAN/
+-rw-rw-rw-   0        0        0    12974 2024-04-26 07:22:55.000000 STASCAN-1.1.0/STASCAN/StatPlot.py
+-rw-rw-rw-   0        0        0      699 2024-04-26 07:22:56.000000 STASCAN-1.1.0/STASCAN/__init__.py
+-rw-rw-rw-   0        0        0     9903 2024-04-26 07:22:55.000000 STASCAN-1.1.0/STASCAN/downstream.py
+-rw-rw-rw-   0        0        0    10970 2024-04-26 07:00:55.000000 STASCAN-1.1.0/STASCAN/model.py
+-rw-rw-rw-   0        0        0    17492 2024-04-26 07:22:56.000000 STASCAN-1.1.0/STASCAN/preparation.py
+-rw-rw-rw-   0        0        0    12385 2024-04-26 07:22:56.000000 STASCAN-1.1.0/STASCAN/preparation_dbit.py
+-rw-rw-rw-   0        0        0    19628 2024-04-26 07:22:55.000000 STASCAN-1.1.0/STASCAN/run_STASCAN.py
+-rw-rw-rw-   0        0        0     7576 2024-04-26 07:22:55.000000 STASCAN-1.1.0/STASCAN/run_STASCAN_dbit.py
+drwxrwxrwx   0        0        0        0 2024-04-26 10:08:21.000000 STASCAN-1.1.0/STASCAN.egg-info/
+-rw-rw-rw-   0        0        0      653 2024-04-26 10:08:21.000000 STASCAN-1.1.0/STASCAN.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2024-04-26 10:08:21.000000 STASCAN-1.1.0/STASCAN.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 10:08:21.000000 STASCAN-1.1.0/STASCAN.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-26 10:08:21.000000 STASCAN-1.1.0/STASCAN.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2024-04-26 10:08:21.000000 STASCAN-1.1.0/STASCAN.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-26 10:08:21.000000 STASCAN-1.1.0/STASCAN.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 10:08:21.000000 STASCAN-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1127 2024-04-26 09:28:22.000000 STASCAN-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `STASCAN-1.0.0/PKG-INFO` & `STASCAN-1.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-Metadata-Version: 2.1
-Name: STASCAN
-Version: 1.0.0
-Summary: An AI-driven method for enhanced cellular organizational map in spatial transcriptomics
-Home-page: https://github.com/AbbyWY/STASCAN
-Author: Ying Wu
-Author-email: wuy@big.ac.cn
-License: MIT
-Platform: UNKNOWN
-License-File: LICENSE.txt
-
-Here we propose STASCAN, which both gene expression and the morphological information are simultaneously utilized to improve the cellular resolution of captured domains and even gap regions. Besides, STASCAN is further designed to enable cell-type predictions at subdivide-spot resolution and construction of the 3D spatial cell map from histology images alone.
-
+Metadata-Version: 1.0
+Name: STASCAN
+Version: 1.1.0
+Summary: An AI-driven method for enhanced cellular organizational map in spatial transcriptomics
+Home-page: https://github.com/AbbyWY/STASCAN
+Author: Ying Wu
+Author-email: wuy@big.ac.cn
+License: MIT
+Description: Here we propose STASCAN, which both gene expression and the morphological information are simultaneously utilized to improve the cellular resolution of captured domains and even gap regions. Besides, STASCAN is further designed to enable cell-type predictions at subdivide-spot resolution and construction of the 3D spatial cell map from histology images alone.
+Platform: UNKNOWN
```

### Comparing `STASCAN-1.0.0/STASCAN/StatPlot.py` & `STASCAN-1.1.0/STASCAN/StatPlot.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,424 +1,424 @@
-import matplotlib.pyplot as plt
-from mpl_toolkits.axisartist.axislines import SubplotZero
-from sklearn.metrics import confusion_matrix
-from skimage.metrics import structural_similarity as ssim
-from itertools import cycle
-from sklearn.metrics import roc_curve, auc
-from sklearn.preprocessing import label_binarize
-import cv2
-import numpy as np
-import itertools
-import json
-import os
-import glob
-import matplotlib.image as imgplt
-
-
-
-
-
-class Metric():
-
-    def __init__(self):
-
-        """
-        Metrics.
-
-        """
-
-        self.name = "Metric"
-
-
-
-    def Loss_Accuracy_Curve(self, input_file, output_path):
-
-        """
-        Visualization of loss curve and accuracy curve.
-
-        Parameters
-        ----------
-        input_file
-            Path of input files.
-        output_path
-            Path of output files.
-        """
-
-        with open(input_file) as f:
-            loss = list(map(float, f.readlines()[0].split()))
-        with open(input_file) as f:
-            val_loss = list(map(float, f.readlines()[1].split()))
-        with open(input_file) as f:
-            accuracy = list(map(float, f.readlines()[2].split()))
-        with open(input_file) as f:
-            val_accuracy = list(map(float, f.readlines()[3].split()))
-
-        x = range(1, len(loss)+1)
-
-        plt.figure(figsize=(12, 5))
-
-        # Loss Curve
-        plt.subplot(1, 2, 1)
-        plt.xlim(0, len(loss)+1)
-        plt.ylim(0, max(max(loss), max(val_loss))+1)
-        plt.xlabel('Epoch')
-        plt.ylabel('Loss')
-        plt.xticks(np.arange(0, len(loss)+1, 10))
-
-        plt.plot(x, loss, c='#228B22', linestyle=':', linewidth=1, label='Train')
-        plt.scatter(x, loss, c='#228B22', s=1, marker='o')
-        plt.text(x[-1]+1, loss[-1], '%.2f' % loss[-1], ha='center', va='bottom', fontsize=5)
-
-        plt.plot(x, val_loss, c='#1874CD', linestyle=':', linewidth=1, label='Test')
-        plt.scatter(x, val_loss, c='#1874CD', s=1, marker='o')
-        plt.text(x[-1], val_loss[-1], '%.2f' % val_loss[-1], ha='center', va='bottom', fontsize=5)
-
-        plt.legend(loc='upper right', fontsize=5)
-
-        # Accuracy Curve
-        plt.subplot(1, 2, 2)
-        plt.xlim(0, len(accuracy) + 1)
-        plt.ylim(0, 1)
-        plt.xlabel('Epoch')
-        plt.ylabel('Accuracy')
-        plt.xticks(np.arange(0, len(accuracy) + 1, 10))
-
-        plt.plot(x, accuracy, c='#EE7600', linestyle=':', linewidth=1, label='Train')
-        plt.scatter(x, accuracy, c='#EE7600', s=1, marker='o')
-        plt.text(x[-1] + 1, accuracy[-1] + 0.02, '%.2f' % (accuracy[-1] * 100) + "%", ha='center', va='bottom', fontsize=5)
-
-        plt.plot(x, val_accuracy, c='#CD2626', linestyle=':', linewidth=1, label='Test')
-        plt.scatter(x, val_accuracy, c='#CD2626', s=1, marker='o')
-        plt.text(x[-1], val_accuracy[-1] - 0.06, '%.2f' % (val_accuracy[-1] * 100) + "%", ha='center', va='bottom', fontsize=5)
-
-        plt.legend(loc='lower left', fontsize=5)
-
-        plt.savefig(output_path + "/Accr-Loss.pdf")
-
-
-
-    def plot_confusion_matrix(self, cm, classes, output_fig):
-
-        """
-        Plotting confusion matrix.
-
-        Parameters
-        ----------
-        cm
-            Inputted confusion matrix.
-        classes
-            List of predicted classes.
-        output_fig
-            Path of output files.
-        """
-        
-        plt.figure(figsize=(5, 5))
-
-        cm = cm.astype('float') / cm.sum(axis=1)[:, np.newaxis]
-        plt.imshow(cm, interpolation='nearest', cmap=plt.cm.Reds)
-        plt.title('The Recall Value of Classes')
-        plt.colorbar()
-        tick_marks = np.arange(len(classes))
-        plt.xticks(tick_marks, classes, rotation=45)
-        plt.yticks(tick_marks, classes)
-        thresh = cm.max() / 2.
-        for i, j in itertools.product(range(cm.shape[0]), range(cm.shape[1])):
-            plt.text(j, i, '{:.2f}'.format(cm[i, j]), horizontalalignment="center", color="white" if cm[i, j] > thresh else "black")
-            #plt.text(j, i + 0.3, '(' + '{:,}'.format(cm[i, j]) + ')', horizontalalignment="center", color="black", fontsize=6)
-        plt.tight_layout()
-        plt.ylabel('Truth')
-        plt.xlabel('Prediction')
-        plt.savefig(output_fig)
-
-
-
-    def Confusion_Matrix(self, image_path, predicted_path, label, output_fig):
-
-        """
-        Visualization of confusion matrix.
-
-        Parameters
-        ----------
-        image_path
-            Path of image folder.
-        predicted_path
-            Path of predicted files.
-        label
-            List of predicted labels.
-        output_fig
-            Path of output files.
-        """
-
-        imgsLib = []
-        for n in label:
-            imgsLib.extend(glob.glob(os.path.join(image_path + "/" + n + "/", "*.png")))
-
-        Labels = {}
-        for each in imgsLib:
-            Labels[each.split("/")[-1].split(".")[0].split("-")[1]+'-'+each.split("/")[-1].split(".")[0].split("-")[2]] = [each.split("/")[-1].split("-")[0]]
-
-        with open(predicted_path) as f:
-            for line in f.readlines():
-                temp = line.split()
-                if temp[0] in Labels.keys():
-                    Labels[temp[0]].append(temp[2])
-
-        for each in Labels:
-            if len(Labels[each]) != 2:
-                print("Error!")
-                print(str(each))
-
-
-        label_true, label_pred = [], []
-        for each in Labels.keys():
-            label_true.append(Labels[each][0])
-            label_pred.append(Labels[each][1])
-
-        cm = confusion_matrix(label_true, label_pred, labels=label)
-        self.plot_confusion_matrix(cm, label, output_fig+"/Confusion_Matrix.pdf")
-
-
-
-    def ROC_Curve(self, image_path, predicted_path, labels, color, output_fig):
-
-        """
-        Visualization of ROC curve.
-
-        Parameters
-        ----------
-        image_path
-            Path of image folder.
-        predicted_path
-            Path of predicted files with detailed probabilities.
-        labels
-            List of predicted labels.
-        color
-            List of colors for labels.
-        output_fig
-            Path of output files.
-        """
-
-        digtal_label, label_digtal = {}, {}
-        labels.sort()
-        for i in range(len(labels)):
-            digtal_label[i] = labels[i]
-            label_digtal[labels[i]] = i
-
-        imgsLib = []
-        for n in labels:
-            imgsLib.extend(glob.glob(os.path.join(image_path + "/" + n + "/", "*.png")))
-
-        Label_true = {}
-        for each in imgsLib:
-            Label_true[each.split("/")[-1].split(".")[0].split("-")[1] + '-' + each.split("/")[-1].split(".")[0].split("-")[2]] = [each.split("/")[-1].split("-")[0]]
-
-        label_true_digtal = []
-        for each in Label_true:
-            label_true_digtal.append(label_digtal[Label_true[each][0]])
-
-        y_test = label_binarize(np.array(label_true_digtal), classes=list(range(0, len(labels))))
-        n_classes = y_test.shape[1]
-
-        with open(predicted_path) as f:
-            for line in f.readlines():
-                temp = line.split()
-                if temp[0] in Label_true.keys():
-                    temp[1:-2] = [float(k) for k in temp[1:-2]]
-                    Label_true[temp[0]].extend(temp[1:-2])
-
-        p_type_detail = []
-        for each in Label_true:
-            p_type_detail.append(Label_true[each][1:])
-
-        y_score = np.array(p_type_detail)
-
-        fpr = dict()
-        tpr = dict()
-        roc_auc = dict()
-        for i in range(n_classes):
-            fpr[i], tpr[i], _ = roc_curve(y_test[:, i], y_score[:, i])
-            roc_auc[i] = auc(fpr[i], tpr[i])
-
-        lw = 2
-        plt.figure(figsize=(5, 5))
-
-        colors = cycle(color)
-        for i, color, label in zip(range(n_classes), colors, cycle(list(label_digtal.keys()))):
-            plt.plot(fpr[i], tpr[i], color=color, lw=2, label=label + '(AUC = {1:0.3f})' ''.format(i, roc_auc[i]))
-
-        plt.plot([0, 1], [0, 1], 'k--', lw=lw)
-        plt.xlim([0.0, 1.0])
-        plt.ylim([0.0, 1.05])
-        plt.xlabel('False Positive Rate')
-        plt.ylabel('True Positive Rate')
-        plt.legend(loc="lower right", fontsize=7)
-        plt.savefig(output_fig)
-
-
-
-    def SSIM(self, imfil1, imfil2):
-
-        """
-        Calculation of SSIM.
-
-        Parameters
-        ----------
-        imfil1
-            Path of image 1.
-        imfil2
-            Path of image 2.
-        """
-
-        img1 = cv2.imread(imfil1)
-        (h, w) = img1.shape[:2]
-        img2 = cv2.imread(imfil2)
-        resized = cv2.resize(img2, (w, h))
-        (h1, w1) = resized.shape[:2]
-        img1 = cv2.cvtColor(img1, cv2.COLOR_BGR2RGB)
-        img2 = cv2.cvtColor(resized, cv2.COLOR_BGR2RGB)
-
-        return ssim(img1, img2, multichannel=True)
-
-
-
-
-
-class Check():
-
-    def __init__(self):
-
-        """
-        Visualization of pre-labelling or imputing.
-
-        """
-
-        self.name = "Check"
-
-
-
-    def Check_PriorSpot(self, adjust_raw_spot, prior_spot, image_path, label_color, output_path, pointsize=5, back_image=False):
-
-        """
-        Visualization of pre-labelling.
-
-        Parameters
-        ----------
-        adjust_raw_spot
-            Path of the adjusted raw spot file.
-        prior_spot
-            Path of the prior spot file.
-        image_path
-            Path of the original H&E staining image.
-        label_color
-            Dictionary of label colors.
-        output_path
-            Path of the output files.
-        pointsize
-            Size of scatter points.
-        back_image
-            Shown of the original H&E staining image.
-        """
-
-        Image = imgplt.imread(image_path)
-        h, w, _ = Image.shape
-        colors = label_color
-
-        rawspot = {}
-        with open(adjust_raw_spot) as f:
-            for line in f.readlines():
-                temp = line.split()
-                rawspot[temp[-1]] = temp[0:2]
-
-        priorspot = {}
-        select = []
-        with open(prior_spot) as f:
-            for line in f.readlines():
-                temp = line.split()
-                priorspot[temp[0]] = [temp[-1], temp[1], temp[2]]
-                select.append(temp)
-
-        fig = plt.figure(figsize=(10, 10))
-        ax = SubplotZero(fig, 1, 1, 1)
-        fig.add_subplot(ax)
-
-        ax.set_xlim(left=0, right=int(max(h, w)))
-        ax.set_ylim(bottom=int(max(h, w)), top=0)
-        ax.set_xticks([])
-        ax.set_yticks([])
-
-        if back_image == True:
-            plt.imshow(Image)
-
-        for each in rawspot.keys():
-            plt.scatter(float(rawspot[each][0]), float(rawspot[each][1]), c='white', marker='o', s=pointsize+2, edgecolors='black', linewidths=0.1)
-        for each in priorspot.keys():
-            plt.scatter(float(priorspot[each][1]), float(priorspot[each][2]), c=colors[priorspot[each][0]], marker='o', s=pointsize)
-        plt.savefig(output_path + "/Check_PriorSpot.pdf")
-
-        selectnum = list(set([x[-1] for x in select]))
-        Label_selectnum = {}
-        for each in selectnum:
-            Label_selectnum[each] = 0
-        for each in select:
-            Label_selectnum[each[-1]] = Label_selectnum[each[-1]] + 1
-        info_select = json.dumps(Label_selectnum, sort_keys=False)
-
-        f = open(output_path + "stat.txt", "w")
-        f.write(info_select)
-        f.close()
-
-
-
-    def Check_ImputedSpot(self, adjust_raw_spot, imputed_spot, image_path, output_path, pointsize=5, back_image=False):
-
-        """
-        Visualization of imputing.
-
-        Parameters
-        ----------
-        adjust_raw_spot
-            Path of the adjusted raw spot file.
-        imputed_spot
-            Path of the imputed spot file.
-        image_path
-            Path of the original H&E staining image.
-        output_path
-            Path of the output files.
-        pointsize
-            Size of scatter points.
-        back_image
-            Shown of the original H&E staining image.
-        """
-
-        Image = imgplt.imread(image_path)
-        h, w, _ = Image.shape
-
-        rawspot = {}
-        with open(adjust_raw_spot) as f:
-            for line in f.readlines():
-                temp = line.split()
-                rawspot[temp[-1]] = temp[0:2]
-
-        imputedspot = {}
-        with open(imputed_spot) as f:
-            for line in f.readlines():
-                temp = line.split()
-                imputedspot[temp[-1]] = temp[0:2]
-
-        fig = plt.figure(figsize=(10, 10))
-        ax = SubplotZero(fig, 1, 1, 1)
-        fig.add_subplot(ax)
-
-        ax.set_xlim(left=0, right=int(max(h, w)))
-        ax.set_ylim(bottom=int(max(h, w)), top=0)
-        ax.set_xticks([])
-        ax.set_yticks([])
-
-        if back_image == True:
-            plt.imshow(Image)
-
-        for each in rawspot.keys():
-            plt.scatter(float(rawspot[each][0]), float(rawspot[each][1]), c='red', marker='o', s=pointsize)
-        for each in imputedspot.keys():
-            plt.scatter(float(imputedspot[each][0]), float(imputedspot[each][1]), c='blue', marker='o', s=pointsize)
-        plt.savefig(output_path + "/Check_ImputedSpot.pdf")
-
+import matplotlib.pyplot as plt
+from mpl_toolkits.axisartist.axislines import SubplotZero
+from sklearn.metrics import confusion_matrix
+from skimage.metrics import structural_similarity as ssim
+from itertools import cycle
+from sklearn.metrics import roc_curve, auc
+from sklearn.preprocessing import label_binarize
+import cv2
+import numpy as np
+import itertools
+import json
+import os
+import glob
+import matplotlib.image as imgplt
+
+
+
+
+
+class Metric():
+
+    def __init__(self):
+
+        """
+        Metrics.
+
+        """
+
+        self.name = "Metric"
+
+
+
+    def Loss_Accuracy_Curve(self, input_file, output_path):
+
+        """
+        Visualization of loss curve and accuracy curve.
+
+        Parameters
+        ----------
+        input_file
+            Path of input files.
+        output_path
+            Path of output files.
+        """
+
+        with open(input_file) as f:
+            loss = list(map(float, f.readlines()[0].split()))
+        with open(input_file) as f:
+            val_loss = list(map(float, f.readlines()[1].split()))
+        with open(input_file) as f:
+            accuracy = list(map(float, f.readlines()[2].split()))
+        with open(input_file) as f:
+            val_accuracy = list(map(float, f.readlines()[3].split()))
+
+        x = range(1, len(loss)+1)
+
+        plt.figure(figsize=(12, 5))
+
+        # Loss Curve
+        plt.subplot(1, 2, 1)
+        plt.xlim(0, len(loss)+1)
+        plt.ylim(0, max(max(loss), max(val_loss))+1)
+        plt.xlabel('Epoch')
+        plt.ylabel('Loss')
+        plt.xticks(np.arange(0, len(loss)+1, 10))
+
+        plt.plot(x, loss, c='#228B22', linestyle=':', linewidth=1, label='Train')
+        plt.scatter(x, loss, c='#228B22', s=1, marker='o')
+        plt.text(x[-1]+1, loss[-1], '%.2f' % loss[-1], ha='center', va='bottom', fontsize=5)
+
+        plt.plot(x, val_loss, c='#1874CD', linestyle=':', linewidth=1, label='Test')
+        plt.scatter(x, val_loss, c='#1874CD', s=1, marker='o')
+        plt.text(x[-1], val_loss[-1], '%.2f' % val_loss[-1], ha='center', va='bottom', fontsize=5)
+
+        plt.legend(loc='upper right', fontsize=5)
+
+        # Accuracy Curve
+        plt.subplot(1, 2, 2)
+        plt.xlim(0, len(accuracy) + 1)
+        plt.ylim(0, 1)
+        plt.xlabel('Epoch')
+        plt.ylabel('Accuracy')
+        plt.xticks(np.arange(0, len(accuracy) + 1, 10))
+
+        plt.plot(x, accuracy, c='#EE7600', linestyle=':', linewidth=1, label='Train')
+        plt.scatter(x, accuracy, c='#EE7600', s=1, marker='o')
+        plt.text(x[-1] + 1, accuracy[-1] + 0.02, '%.2f' % (accuracy[-1] * 100) + "%", ha='center', va='bottom', fontsize=5)
+
+        plt.plot(x, val_accuracy, c='#CD2626', linestyle=':', linewidth=1, label='Test')
+        plt.scatter(x, val_accuracy, c='#CD2626', s=1, marker='o')
+        plt.text(x[-1], val_accuracy[-1] - 0.06, '%.2f' % (val_accuracy[-1] * 100) + "%", ha='center', va='bottom', fontsize=5)
+
+        plt.legend(loc='lower left', fontsize=5)
+
+        plt.savefig(output_path + "/Accr-Loss.pdf")
+
+
+
+    def plot_confusion_matrix(self, cm, classes, output_fig):
+
+        """
+        Plotting confusion matrix.
+
+        Parameters
+        ----------
+        cm
+            Inputted confusion matrix.
+        classes
+            List of predicted classes.
+        output_fig
+            Path of output files.
+        """
+        
+        plt.figure(figsize=(5, 5))
+
+        cm = cm.astype('float') / cm.sum(axis=1)[:, np.newaxis]
+        plt.imshow(cm, interpolation='nearest', cmap=plt.cm.Reds)
+        plt.title('The Recall Value of Classes')
+        plt.colorbar()
+        tick_marks = np.arange(len(classes))
+        plt.xticks(tick_marks, classes, rotation=45)
+        plt.yticks(tick_marks, classes)
+        thresh = cm.max() / 2.
+        for i, j in itertools.product(range(cm.shape[0]), range(cm.shape[1])):
+            plt.text(j, i, '{:.2f}'.format(cm[i, j]), horizontalalignment="center", color="white" if cm[i, j] > thresh else "black")
+            #plt.text(j, i + 0.3, '(' + '{:,}'.format(cm[i, j]) + ')', horizontalalignment="center", color="black", fontsize=6)
+        plt.tight_layout()
+        plt.ylabel('Truth')
+        plt.xlabel('Prediction')
+        plt.savefig(output_fig)
+
+
+
+    def Confusion_Matrix(self, image_path, predicted_path, label, output_fig):
+
+        """
+        Visualization of confusion matrix.
+
+        Parameters
+        ----------
+        image_path
+            Path of image folder.
+        predicted_path
+            Path of predicted files.
+        label
+            List of predicted labels.
+        output_fig
+            Path of output files.
+        """
+
+        imgsLib = []
+        for n in label:
+            imgsLib.extend(glob.glob(os.path.join(image_path + "/" + n + "/", "*.png")))
+
+        Labels = {}
+        for each in imgsLib:
+            Labels[each.split("/")[-1].split(".")[0].split("-")[1]+'-'+each.split("/")[-1].split(".")[0].split("-")[2]] = [each.split("/")[-1].split("-")[0]]
+
+        with open(predicted_path) as f:
+            for line in f.readlines():
+                temp = line.split()
+                if temp[0] in Labels.keys():
+                    Labels[temp[0]].append(temp[2])
+
+        for each in Labels:
+            if len(Labels[each]) != 2:
+                print("Error!")
+                print(str(each))
+
+
+        label_true, label_pred = [], []
+        for each in Labels.keys():
+            label_true.append(Labels[each][0])
+            label_pred.append(Labels[each][1])
+
+        cm = confusion_matrix(label_true, label_pred, labels=label)
+        self.plot_confusion_matrix(cm, label, output_fig+"/Confusion_Matrix.pdf")
+
+
+
+    def ROC_Curve(self, image_path, predicted_path, labels, color, output_fig):
+
+        """
+        Visualization of ROC curve.
+
+        Parameters
+        ----------
+        image_path
+            Path of image folder.
+        predicted_path
+            Path of predicted files with detailed probabilities.
+        labels
+            List of predicted labels.
+        color
+            List of colors for labels.
+        output_fig
+            Path of output files.
+        """
+
+        digtal_label, label_digtal = {}, {}
+        labels.sort()
+        for i in range(len(labels)):
+            digtal_label[i] = labels[i]
+            label_digtal[labels[i]] = i
+
+        imgsLib = []
+        for n in labels:
+            imgsLib.extend(glob.glob(os.path.join(image_path + "/" + n + "/", "*.png")))
+
+        Label_true = {}
+        for each in imgsLib:
+            Label_true[each.split("/")[-1].split(".")[0].split("-")[1] + '-' + each.split("/")[-1].split(".")[0].split("-")[2]] = [each.split("/")[-1].split("-")[0]]
+
+        label_true_digtal = []
+        for each in Label_true:
+            label_true_digtal.append(label_digtal[Label_true[each][0]])
+
+        y_test = label_binarize(np.array(label_true_digtal), classes=list(range(0, len(labels))))
+        n_classes = y_test.shape[1]
+
+        with open(predicted_path) as f:
+            for line in f.readlines():
+                temp = line.split()
+                if temp[0] in Label_true.keys():
+                    temp[1:-2] = [float(k) for k in temp[1:-2]]
+                    Label_true[temp[0]].extend(temp[1:-2])
+
+        p_type_detail = []
+        for each in Label_true:
+            p_type_detail.append(Label_true[each][1:])
+
+        y_score = np.array(p_type_detail)
+
+        fpr = dict()
+        tpr = dict()
+        roc_auc = dict()
+        for i in range(n_classes):
+            fpr[i], tpr[i], _ = roc_curve(y_test[:, i], y_score[:, i])
+            roc_auc[i] = auc(fpr[i], tpr[i])
+
+        lw = 2
+        plt.figure(figsize=(5, 5))
+
+        colors = cycle(color)
+        for i, color, label in zip(range(n_classes), colors, cycle(list(label_digtal.keys()))):
+            plt.plot(fpr[i], tpr[i], color=color, lw=2, label=label + '(AUC = {1:0.3f})' ''.format(i, roc_auc[i]))
+
+        plt.plot([0, 1], [0, 1], 'k--', lw=lw)
+        plt.xlim([0.0, 1.0])
+        plt.ylim([0.0, 1.05])
+        plt.xlabel('False Positive Rate')
+        plt.ylabel('True Positive Rate')
+        plt.legend(loc="lower right", fontsize=7)
+        plt.savefig(output_fig)
+
+
+
+    def SSIM(self, imfil1, imfil2):
+
+        """
+        Calculation of SSIM.
+
+        Parameters
+        ----------
+        imfil1
+            Path of image 1.
+        imfil2
+            Path of image 2.
+        """
+
+        img1 = cv2.imread(imfil1)
+        (h, w) = img1.shape[:2]
+        img2 = cv2.imread(imfil2)
+        resized = cv2.resize(img2, (w, h))
+        (h1, w1) = resized.shape[:2]
+        img1 = cv2.cvtColor(img1, cv2.COLOR_BGR2RGB)
+        img2 = cv2.cvtColor(resized, cv2.COLOR_BGR2RGB)
+
+        return ssim(img1, img2, multichannel=True)
+
+
+
+
+
+class Check():
+
+    def __init__(self):
+
+        """
+        Visualization of pre-labelling or imputing.
+
+        """
+
+        self.name = "Check"
+
+
+
+    def Check_PriorSpot(self, adjust_raw_spot, prior_spot, image_path, label_color, output_path, pointsize=5, back_image=False):
+
+        """
+        Visualization of pre-labelling.
+
+        Parameters
+        ----------
+        adjust_raw_spot
+            Path of the adjusted raw spot file.
+        prior_spot
+            Path of the prior spot file.
+        image_path
+            Path of the original H&E staining image.
+        label_color
+            Dictionary of label colors.
+        output_path
+            Path of the output files.
+        pointsize
+            Size of scatter points.
+        back_image
+            Shown of the original H&E staining image.
+        """
+
+        Image = imgplt.imread(image_path)
+        h, w, _ = Image.shape
+        colors = label_color
+
+        rawspot = {}
+        with open(adjust_raw_spot) as f:
+            for line in f.readlines():
+                temp = line.split()
+                rawspot[temp[-1]] = temp[0:2]
+
+        priorspot = {}
+        select = []
+        with open(prior_spot) as f:
+            for line in f.readlines():
+                temp = line.split()
+                priorspot[temp[0]] = [temp[-1], temp[1], temp[2]]
+                select.append(temp)
+
+        fig = plt.figure(figsize=(10, 10))
+        ax = SubplotZero(fig, 1, 1, 1)
+        fig.add_subplot(ax)
+
+        ax.set_xlim(left=0, right=int(max(h, w)))
+        ax.set_ylim(bottom=int(max(h, w)), top=0)
+        ax.set_xticks([])
+        ax.set_yticks([])
+
+        if back_image == True:
+            plt.imshow(Image)
+
+        for each in rawspot.keys():
+            plt.scatter(float(rawspot[each][0]), float(rawspot[each][1]), c='white', marker='o', s=pointsize+2, edgecolors='black', linewidths=0.1)
+        for each in priorspot.keys():
+            plt.scatter(float(priorspot[each][1]), float(priorspot[each][2]), c=colors[priorspot[each][0]], marker='o', s=pointsize)
+        plt.savefig(output_path + "/Check_PriorSpot.pdf")
+
+        selectnum = list(set([x[-1] for x in select]))
+        Label_selectnum = {}
+        for each in selectnum:
+            Label_selectnum[each] = 0
+        for each in select:
+            Label_selectnum[each[-1]] = Label_selectnum[each[-1]] + 1
+        info_select = json.dumps(Label_selectnum, sort_keys=False)
+
+        f = open(output_path + "stat.txt", "w")
+        f.write(info_select)
+        f.close()
+
+
+
+    def Check_ImputedSpot(self, adjust_raw_spot, imputed_spot, image_path, output_path, pointsize=5, back_image=False):
+
+        """
+        Visualization of imputing.
+
+        Parameters
+        ----------
+        adjust_raw_spot
+            Path of the adjusted raw spot file.
+        imputed_spot
+            Path of the imputed spot file.
+        image_path
+            Path of the original H&E staining image.
+        output_path
+            Path of the output files.
+        pointsize
+            Size of scatter points.
+        back_image
+            Shown of the original H&E staining image.
+        """
+
+        Image = imgplt.imread(image_path)
+        h, w, _ = Image.shape
+
+        rawspot = {}
+        with open(adjust_raw_spot) as f:
+            for line in f.readlines():
+                temp = line.split()
+                rawspot[temp[-1]] = temp[0:2]
+
+        imputedspot = {}
+        with open(imputed_spot) as f:
+            for line in f.readlines():
+                temp = line.split()
+                imputedspot[temp[-1]] = temp[0:2]
+
+        fig = plt.figure(figsize=(10, 10))
+        ax = SubplotZero(fig, 1, 1, 1)
+        fig.add_subplot(ax)
+
+        ax.set_xlim(left=0, right=int(max(h, w)))
+        ax.set_ylim(bottom=int(max(h, w)), top=0)
+        ax.set_xticks([])
+        ax.set_yticks([])
+
+        if back_image == True:
+            plt.imshow(Image)
+
+        for each in rawspot.keys():
+            plt.scatter(float(rawspot[each][0]), float(rawspot[each][1]), c='red', marker='o', s=pointsize)
+        for each in imputedspot.keys():
+            plt.scatter(float(imputedspot[each][0]), float(imputedspot[each][1]), c='blue', marker='o', s=pointsize)
+        plt.savefig(output_path + "/Check_ImputedSpot.pdf")
+
```

### Comparing `STASCAN-1.0.0/STASCAN/model.py` & `STASCAN-1.1.0/STASCAN/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,327 +1,370 @@
-import tensorflow as tf
-
-gpus = tf.config.list_physical_devices('GPU')
-for gpu in gpus:
-    tf.config.experimental.set_memory_growth(device=gpu, enable=True)
-    
-from tensorflow.keras.applications.vgg16 import VGG16
-from tensorflow.keras.models import Sequential
-from tensorflow.keras.layers import Conv2D, MaxPool2D, Activation, Dropout, Flatten, Dense
-from tensorflow.keras.optimizers import SGD
-from tensorflow.keras.preprocessing.image import ImageDataGenerator, img_to_array, load_img
-
-from tensorflow.keras.models import load_model
-import numpy as np
-import os
-
-import itertools
-import glob
-
-
-
-
-
-class BuildModel():
-
-    def __init__(self):
-
-        self.name = "BuildModel"
-
-        self.train_datagen = ImageDataGenerator(
-            rotation_range=40,
-            width_shift_range=0.2,
-            height_shift_range=0.2,
-            rescale=1 / 255,
-            shear_range=20,
-            zoom_range=0.2,
-            horizontal_flip=True,
-            fill_mode='nearest',
-        )
-
-        self.test_datagen = ImageDataGenerator(
-            rescale=1 / 255,
-        )
-
-        self.batch_size = 32
-
-
-
-    def base_model(self, traindata_path, testdata_path, output_path, n_class, lr=1e-3, epochs=50, model_name="base_model.h5"):
-
-        """
-        Build base model.
-
-        Parameters
-        ----------
-        traindata_path
-            Path of training set.
-        testdata_path
-            Path of testing set.
-        output_path
-            Path of output files.
-        n_class
-            Number of cell classes.
-        lr
-            Learning rate for SGDOptimizer.
-        epochs
-            Number of total epochs in training.
-        model_name
-            Name of trained model
-        """
-
-        vgg16_model = VGG16(weights='imagenet', include_top=False, input_shape=(224, 224, 3))
-
-        top_model = Sequential()
-        top_model.add(Flatten(input_shape=vgg16_model.output_shape[1:]))
-        top_model.add(Dense(256, activation='relu'))
-        top_model.add(Dropout(0.5))
-        top_model.add(Dense(n_class, activation='softmax'))
-        model = Sequential()
-        model.add(vgg16_model)
-        model.add(top_model)
-
-        train_generator = self.train_datagen.flow_from_directory(
-            traindata_path,
-            target_size=(224, 224),
-            batch_size=self.batch_size,
-        )
-
-        test_generator = self.test_datagen.flow_from_directory(
-            testdata_path,
-            target_size=(224, 224),
-            batch_size=self.batch_size,
-        )
-
-        print(train_generator.class_indices)
-        print(test_generator.class_indices)
-
-
-        model.compile(optimizer=SGD(lr=lr, momentum=0.9), loss='categorical_crossentropy', metrics=['accuracy'])
-        model.fit(train_generator, epochs=epochs, validation_data=test_generator)
-
-        loss, val_loss, accuracy, val_accuracy = model.history.history['loss'], model.history.history['val_loss'], model.history.history['accuracy'], model.history.history['val_accuracy']
-
-        os.makedirs(output_path + "/Models/")
-
-        log = [loss, val_loss, accuracy, val_accuracy]
-        np.savetxt(output_path + "/Models/" + "Log_BaseModel.txt", log, fmt='%s', delimiter='\t')
-
-        model.save(output_path + "/Models/" + model_name)
-
-
-
-    def finetuned_model(self, basemodel, traindata_path, testdata_path, output_path, lr=1e-4, epochs=50, model_name="finetuned_model.h5"):
-
-        """
-        Build finetuned model.
-
-        Parameters
-        ----------
-        basemodel
-            Path of base model
-        traindata_path
-            Path of training set.
-        testdata_path
-            Path of testing set.
-        output_path
-            Path of output files.
-        lr
-            Learning rate for SGDOptimizer.
-        epochs
-            Number of total epochs in training.
-        model_name
-            Name of trained model
-        """
-
-        model = load_model(basemodel)
-
-        train_generator = self.train_datagen.flow_from_directory(
-            traindata_path,
-            target_size=(224, 224),
-            batch_size=self.batch_size,
-        )
-
-        test_generator = self.test_datagen.flow_from_directory(
-            testdata_path,
-            target_size=(224, 224),
-            batch_size=self.batch_size,
-        )
-
-        print(train_generator.class_indices)
-        print(test_generator.class_indices)
-
-        model.compile(optimizer=SGD(lr=lr, momentum=0.9), loss='categorical_crossentropy', metrics=['accuracy'])
-        model.fit(train_generator, epochs=epochs, validation_data=test_generator)
-
-        loss, val_loss, accuracy, val_accuracy = model.history.history['loss'], model.history.history['val_loss'], model.history.history['accuracy'], model.history.history['val_accuracy']
-
-        if not os.path.exists(output_path + "/Models/"):
-            os.makedirs(output_path + "/Models/")
-
-        log = [loss, val_loss, accuracy, val_accuracy]
-        np.savetxt(output_path + "/Models/" + "Log_FinetunedModel.txt", log, fmt='%s', delimiter='\t')
-
-        model.save(output_path + "/Models/" + model_name)
-
-
-
-    def alltrain_model(self, traindata_path, output_path, n_class, lr=1e-3, epochs=50, model_name="alltrain_model.h5"):
-
-        """
-        Build base model.
-
-        Parameters
-        ----------
-        traindata_path
-            Path of training set.
-        output_path
-            Path of output files.
-        n_class
-            Number of cell classes.
-        lr
-            Learning rate for SGDOptimizer.
-        epochs
-            Number of total epochs in training.
-        model_name
-            Name of trained model
-        """
-
-        vgg16_model = VGG16(weights='imagenet', include_top=False, input_shape=(224, 224, 3))
-
-        top_model = Sequential()
-        top_model.add(Flatten(input_shape=vgg16_model.output_shape[1:]))
-        top_model.add(Dense(256, activation='relu'))
-        top_model.add(Dropout(0.5))
-        top_model.add(Dense(n_class, activation='softmax'))
-        model = Sequential()
-        model.add(vgg16_model)
-        model.add(top_model)
-
-        train_generator = self.train_datagen.flow_from_directory(
-            traindata_path,
-            target_size=(224, 224),
-            batch_size=self.batch_size,
-        )
-
-
-        print(train_generator.class_indices)
-
-
-        model.compile(optimizer=SGD(lr=lr, momentum=0.9), loss='categorical_crossentropy', metrics=['accuracy'])
-        model.fit(train_generator, epochs=epochs)
-
-        os.makedirs(output_path + "/Models/")
-        model.save(output_path + "/Models/" + model_name)
-
-
-
-
-
-class BuildPrediction():
-
-    def __init__(self, model, result_dir):
-
-        """
-        Build prediction.
-
-        Parameters
-        ----------
-        model
-            Path of the trained model used for prediction.
-        result_dir
-            Path of the output folder.
-        """
-
-        self.name = "Prediction"
-        self.model = load_model(model)
-        self.result_dir = result_dir
-
-        if not os.path.exists(result_dir + "/Predict/"):
-            os.makedirs(result_dir + "/Predict/")
-
-
-
-    def predict(self, image):
-
-        """
-        Build prediction.
-
-        Parameters
-        ----------
-        image
-            Image for prediction.
-        """
-
-        image = load_img(image)
-        image = image.resize((224, 224))
-        image = img_to_array(image)
-        image = image / 255
-        image = np.expand_dims(image, 0)
-        predict = self.model.predict(image)
-        classes = np.argmax(predict, axis=1)
-
-        return predict, classes
-
-
-
-    def prediction(self, input_spot, input_image, input_position, predicting_type):
-
-        """
-        Build prediction.
-
-        Parameters
-        ----------
-        input_spot
-            Spots in the dataset, which used to determine labels.
-        input_image
-            Path of images for prediction.
-        input_position
-            Position file of images.
-        predicting_type
-            Type of predicting spot images.
-        """
-
-        celltype = list(set([x[-1] for x in input_spot]))
-        celltype.sort()
-        label = {}
-        for i in range(len(celltype)):
-            label[i] = celltype[i]
-        print(label)
-
-        imgsLib = []
-        imgsLib.extend(glob.glob(os.path.join(input_image + "/", "*.png")))
-
-        pre_type = []
-        pre_type_detail = []
-
-        for each in imgsLib:
-            pre_detail, pre = self.predict(each)
-            imgname = each.split("/")[-1].split(".")[0]
-            pre_type.append([imgname, int(pre), label[int(pre)]])
-            pre_temp = list(itertools.chain.from_iterable(pre_detail.tolist()))
-            temp = [imgname]
-            temp.extend(pre_temp)
-            pre_type_detail.append(temp)
-
-        coor = {}
-        with open(input_position) as f:
-            for line in f.readlines():
-                temp = line.split()
-                coor[temp[2]] = [temp[0], temp[1]]
-
-        filltype = []
-        for each in pre_type:
-            if each[0] in coor.keys():
-                temp = each
-                temp.extend(coor[each[0]])
-                filltype.append(temp)
-        np.savetxt(self.result_dir + "/Predict/" + predicting_type + "_predict.txt", filltype, fmt='%s', delimiter='\t')
-
-        filltype_detail = []
-        for each in pre_type_detail:
-            if each[0] in coor.keys():
-                temp = each
-                temp.extend(coor[each[0]])
-                filltype_detail.append(temp)
-        np.savetxt(self.result_dir + "/Predict/" + predicting_type + "predict_detail.txt", filltype_detail, fmt='%s', delimiter='\t')
-
+import tensorflow as tf
+
+gpus = tf.config.list_physical_devices('GPU')
+for gpu in gpus:
+    tf.config.experimental.set_memory_growth(device=gpu, enable=True)
+    
+from tensorflow.keras.applications.vgg16 import VGG16
+from tensorflow.keras.models import Sequential
+from tensorflow.keras.layers import Conv2D, MaxPool2D, Activation, Dropout, Flatten, Dense
+from tensorflow.keras.optimizers import SGD
+from tensorflow.keras.preprocessing.image import ImageDataGenerator, img_to_array, load_img
+
+from tensorflow.keras.models import load_model
+import numpy as np
+import os
+
+import itertools
+import glob
+
+
+
+
+
+class BuildModel():
+
+    def __init__(self):
+
+        self.name = "BuildModel"
+
+        self.train_datagen = ImageDataGenerator(
+            rotation_range=40,
+            width_shift_range=0.2,
+            height_shift_range=0.2,
+            rescale=1 / 255,
+            shear_range=20,
+            zoom_range=0.2,
+            horizontal_flip=True,
+            fill_mode='nearest',
+        )
+
+        self.test_datagen = ImageDataGenerator(
+            rescale=1 / 255,
+        )
+
+        self.batch_size = 32
+
+
+
+    def base_model(self, traindata_path, testdata_path, output_path, n_class, lr=1e-3, epochs=50, model_name="base_model.h5"):
+
+        """
+        Build base model.
+
+        Parameters
+        ----------
+        traindata_path
+            Path of training set.
+        testdata_path
+            Path of testing set.
+        output_path
+            Path of output files.
+        n_class
+            Number of cell classes.
+        lr
+            Learning rate for SGDOptimizer.
+        epochs
+            Number of total epochs in training.
+        model_name
+            Name of trained model
+        """
+
+        vgg16_model = VGG16(weights='imagenet', include_top=False, input_shape=(224, 224, 3))
+
+        top_model = Sequential()
+        top_model.add(Flatten(input_shape=vgg16_model.output_shape[1:]))
+        top_model.add(Dense(256, activation='relu'))
+        top_model.add(Dropout(0.5))
+        top_model.add(Dense(n_class, activation='softmax'))
+        model = Sequential()
+        model.add(vgg16_model)
+        model.add(top_model)
+
+        train_generator = self.train_datagen.flow_from_directory(
+            traindata_path,
+            target_size=(224, 224),
+            batch_size=self.batch_size,
+        )
+
+        test_generator = self.test_datagen.flow_from_directory(
+            testdata_path,
+            target_size=(224, 224),
+            batch_size=self.batch_size,
+        )
+
+        print(train_generator.class_indices)
+        print(test_generator.class_indices)
+
+
+        model.compile(optimizer=SGD(lr=lr, momentum=0.9), loss='categorical_crossentropy', metrics=['accuracy'])
+        model.fit(train_generator, epochs=epochs, validation_data=test_generator)
+
+        loss, val_loss, accuracy, val_accuracy = model.history.history['loss'], model.history.history['val_loss'], model.history.history['accuracy'], model.history.history['val_accuracy']
+
+        os.makedirs(output_path + "/Models/")
+
+        log = [loss, val_loss, accuracy, val_accuracy]
+        np.savetxt(output_path + "/Models/" + "Log_BaseModel.txt", log, fmt='%s', delimiter='\t')
+
+        model.save(output_path + "/Models/" + model_name)
+
+
+
+    def finetuned_model(self, basemodel, traindata_path, testdata_path, output_path, lr=1e-4, epochs=50, model_name="finetuned_model.h5"):
+
+        """
+        Build finetuned model.
+
+        Parameters
+        ----------
+        basemodel
+            Path of base model
+        traindata_path
+            Path of training set.
+        testdata_path
+            Path of testing set.
+        output_path
+            Path of output files.
+        lr
+            Learning rate for SGDOptimizer.
+        epochs
+            Number of total epochs in training.
+        model_name
+            Name of trained model
+        """
+
+        model = load_model(basemodel)
+
+        train_generator = self.train_datagen.flow_from_directory(
+            traindata_path,
+            target_size=(224, 224),
+            batch_size=self.batch_size,
+        )
+
+        test_generator = self.test_datagen.flow_from_directory(
+            testdata_path,
+            target_size=(224, 224),
+            batch_size=self.batch_size,
+        )
+
+        print(train_generator.class_indices)
+        print(test_generator.class_indices)
+
+        model.compile(optimizer=SGD(lr=lr, momentum=0.9), loss='categorical_crossentropy', metrics=['accuracy'])
+        model.fit(train_generator, epochs=epochs, validation_data=test_generator)
+
+        loss, val_loss, accuracy, val_accuracy = model.history.history['loss'], model.history.history['val_loss'], model.history.history['accuracy'], model.history.history['val_accuracy']
+
+        if not os.path.exists(output_path + "/Models/"):
+            os.makedirs(output_path + "/Models/")
+
+        log = [loss, val_loss, accuracy, val_accuracy]
+        np.savetxt(output_path + "/Models/" + "Log_FinetunedModel.txt", log, fmt='%s', delimiter='\t')
+
+        model.save(output_path + "/Models/" + model_name)
+
+
+
+    def alltrain_model(self, traindata_path, output_path, n_class, lr=1e-3, epochs=50, model_name="alltrain_model.h5"):
+
+        """
+        Build base model.
+
+        Parameters
+        ----------
+        traindata_path
+            Path of training set.
+        output_path
+            Path of output files.
+        n_class
+            Number of cell classes.
+        lr
+            Learning rate for SGDOptimizer.
+        epochs
+            Number of total epochs in training.
+        model_name
+            Name of trained model
+        """
+
+        vgg16_model = VGG16(weights='imagenet', include_top=False, input_shape=(224, 224, 3))
+
+        top_model = Sequential()
+        top_model.add(Flatten(input_shape=vgg16_model.output_shape[1:]))
+        top_model.add(Dense(256, activation='relu'))
+        top_model.add(Dropout(0.5))
+        top_model.add(Dense(n_class, activation='softmax'))
+        model = Sequential()
+        model.add(vgg16_model)
+        model.add(top_model)
+
+        train_generator = self.train_datagen.flow_from_directory(
+            traindata_path,
+            target_size=(224, 224),
+            batch_size=self.batch_size,
+        )
+
+
+        print(train_generator.class_indices)
+
+
+        model.compile(optimizer=SGD(lr=lr, momentum=0.9), loss='categorical_crossentropy', metrics=['accuracy'])
+        model.fit(train_generator, epochs=epochs)
+
+        os.makedirs(output_path + "/Models/")
+        model.save(output_path + "/Models/" + model_name)
+
+
+
+
+
+class BuildPrediction():
+
+    def __init__(self, model, result_dir):
+
+        """
+        Build prediction.
+
+        Parameters
+        ----------
+        model
+            Path of the trained model used for prediction.
+        result_dir
+            Path of the output folder.
+        """
+
+        self.name = "Prediction"
+        self.model = load_model(model)
+        self.result_dir = result_dir
+
+        if not os.path.exists(result_dir + "/Predict/"):
+            os.makedirs(result_dir + "/Predict/")
+
+
+
+    def predict(self, image):
+
+        """
+        Build prediction.
+
+        Parameters
+        ----------
+        image
+            Image for prediction.
+        """
+
+        image = load_img(image)
+        image = image.resize((224, 224))
+        image = img_to_array(image)
+        image = image / 255
+        image = np.expand_dims(image, 0)
+        predict = self.model.predict(image)
+        classes = np.argmax(predict, axis=1)
+
+        return predict, classes
+
+
+
+    def prediction(self, input_spot, input_image, input_position, predicting_type):
+
+        """
+        Build prediction.
+
+        Parameters
+        ----------
+        input_spot
+            Spots in the dataset, which used to determine labels.
+        input_image
+            Path of images for prediction.
+        input_position
+            Position file of images.
+        predicting_type
+            Type of predicting spot images.
+        """
+
+        celltype = list(set([x[-1] for x in input_spot]))
+        celltype.sort()
+        label = {}
+        for i in range(len(celltype)):
+            label[i] = celltype[i]
+        print(label)
+
+        imgsLib = []
+        imgsLib.extend(glob.glob(os.path.join(input_image + "/", "*.png")))
+
+        pre_type = []
+        pre_type_detail = []
+
+        for each in imgsLib:
+            pre_detail, pre = self.predict(each)
+            imgname = each.split("/")[-1].split(".")[0]
+            pre_type.append([imgname, int(pre), label[int(pre)]])
+            pre_temp = list(itertools.chain.from_iterable(pre_detail.tolist()))
+            temp = [imgname]
+            temp.extend(pre_temp)
+            pre_type_detail.append(temp)
+
+        coor = {}
+        with open(input_position) as f:
+            for line in f.readlines():
+                temp = line.split()
+                coor[temp[2]] = [temp[0], temp[1]]
+
+        filltype = []
+        for each in pre_type:
+            if each[0] in coor.keys():
+                temp = each
+                temp.extend(coor[each[0]])
+                filltype.append(temp)
+        np.savetxt(self.result_dir + "/Predict/" + predicting_type + "_predict.txt", filltype, fmt='%s', delimiter='\t')
+
+        filltype_detail = []
+        for each in pre_type_detail:
+            if each[0] in coor.keys():
+                temp = each
+                temp.extend(coor[each[0]])
+                filltype_detail.append(temp)
+        np.savetxt(self.result_dir + "/Predict/" + predicting_type + "predict_detail.txt", filltype_detail, fmt='%s', delimiter='\t')
+
+
+
+    def prediction_dbit(self, input_spot, input_image, predicting_type):
+
+        """
+        Build prediction.
+
+        Parameters
+        ----------
+        input_spot
+            Spots in the dataset, which used to determine labels.
+        input_image
+            Path of images for prediction.
+        predicting_type
+            Type of predicting spot images.
+        """
+
+        celltype = list(set([x[-1] for x in input_spot]))
+        celltype.sort()
+        label = {}
+        for i in range(len(celltype)):
+            label[i] = celltype[i]
+        print(label)
+
+        imgsLib = []
+        imgsLib.extend(glob.glob(os.path.join(input_image + "/", "*.png")))
+
+        pre_type = []
+        pre_type_detail = []
+
+        for each in imgsLib:
+            pre_detail, pre = self.predict(each)
+            imgname = each.split("/")[-1].split(".")[0]
+            pre_type.append([imgname, int(pre), label[int(pre)]])
+            pre_temp = list(itertools.chain.from_iterable(pre_detail.tolist()))
+            temp = [imgname]
+            temp.extend(pre_temp)
+            pre_type_detail.append(temp)
+
+        np.savetxt(self.result_dir + "/Predict/" + predicting_type + "_predict.txt", pre_type, fmt='%s', delimiter='\t')
+        np.savetxt(self.result_dir + "/Predict/" + predicting_type + "predict_detail.txt", pre_type_detail, fmt='%s', delimiter='\t')
+
+
```

### Comparing `STASCAN-1.0.0/STASCAN/preparation.py` & `STASCAN-1.1.0/STASCAN/preparation.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,508 +1,508 @@
-from pylab import *
-import numpy as np
-import cv2
-import os
-import random
-import glob
-import shutil
-from PIL import Image
-
-
-
-
-
-class Generator():
-
-    def __init__(self, record_dir, position, image, crop_size):
-
-        """
-        Preparation of spot images.
-
-        Parameters
-        ----------
-        record_dir
-            Path of the output folder.
-        position
-            The position of raw spots. Standard output file for Space Ranger.
-        image
-            The original H&E staining images, used for Space Ranger previously.
-        crop_size
-            Pixel radius of spot images.
-        """
-
-        self.name = "Generator"
-
-        self.record_dir = record_dir
-
-        self.position = []
-        with open(position) as f:
-            for line in f.readlines():
-                temp = line.split(',')
-                if int(temp[1]) == 1:
-                    self.position.append([int(temp[-1].split('\n')[0]), int(temp[-2]), temp[0]])
-        self.position.sort(key=lambda x: (x[1], x[0]))
-        print("The number of raw spots : ", len(self.position))
-        
-        self.Data = {}
-        for each in self.position:
-            self.Data[each[2]] = [each[0], each[1]]
-
-        self.rawimage = image
-        self.crop_size = crop_size
-
-
-
-    def SpotImage_generator(self, type):
-
-        """
-        Generator of spot images.
-
-        Parameters
-        ----------
-        type: {'RawSpot', 'PriorSpot', 'ImputedSpot'}
-            Type of spots.
-        """
-
-        img = cv2.imread(self.rawimage)
-        crop_size = self.crop_size
-
-        if type == 'RawSpot':
-            position = self.position
-            for each in position:
-                k = each[2].replace("\"", "")
-                cropped = img[int(each[1]) - crop_size:int(each[1]) + crop_size,
-                          int(each[0]) - crop_size:int(each[0]) + crop_size]
-                cv2.imwrite(self.record_dir + "/RawSpot/" + k + ".png", cropped)
-        elif type == 'PriorSpot':
-            position = self.prior_spot
-            for each in position:
-                k = each[0].replace("\"", "")
-                cropped = img[int(each[2]) - crop_size:int(each[2]) + crop_size,
-                          int(each[1]) - crop_size:int(each[1]) + crop_size]
-                celltype = each[-1]
-                cv2.imwrite(self.record_dir + "/PriorSpot/" + celltype + "-" + k + ".png", cropped)
-        elif type == 'ImputedSpot':
-            position = self.imputed_spot
-            for each in position:
-                k = each[2].replace("\"", "")
-                each[0], each[1] = float(each[0]), float(each[1])
-                cropped = img[int(each[1]) - crop_size:int(each[1]) + crop_size,
-                          int(each[0]) - crop_size:int(each[0]) + crop_size]
-                cv2.imwrite(self.record_dir + "/ImputedSpot/" + k + ".png", cropped)
-        else:
-            print("ERROR :The type of SpotImage doesn't exist!")
-
-
-
-    def SubSpotImage_generator(self, type):
-
-        """
-        Generator of subdivided spot images.
-
-        Parameters
-        ----------
-        type: {'raw_divided', 'prior_divided'}
-            Type of spots.
-        """
-
-        imgsLib = []
-        subloc = []
-        position = self.Data
-
-        if type == 'raw_divided':
-            img_path = self.record_dir + "/RawSpot/"
-            save_path = self.record_dir + "/SubSpot/raw_divided/"
-            #position = self.Data
-        if type == 'prior_divided':
-            img_path = self.record_dir + "/PriorSpot/"
-            save_path = self.record_dir + "/SubSpot/prior_divided/"
-            #position = {}
-            #if self.prior_spot == True:
-            #    for each in self.prior_spot:
-            #        position[each[0]] = [int(each[1]), int(each[2])]
-            #else:
-            #with open(self.record_dir + "/PriorSpot/prior_spot.txt") as f:
-            #    for line in f.readlines():
-            #        temp = line.split()
-            #        position[temp[0]] = [float(temp[1]), float(temp[2])]          
-        
-        
-
-        imgsLib.extend(glob.glob(os.path.join(img_path, "*.png")))
-
-        for each in imgsLib:
-            # img
-            image = Image.open(each)
-            img = image.convert('RGB')
-            w = img.size[0]
-            h = img.size[1]
-            rawname = each.split("/")[-1].split(".")[0]
-            img_1 = img.crop([0, 0, w / 2, h / 2])
-            img_1.save(save_path + rawname + "_1.png")
-            img_2 = img.crop([w / 2, 0, w, h / 2])
-            img_2.save(save_path + rawname + "_2.png")
-            img_3 = img.crop([0, h / 2, w / 2, h])
-            img_3.save(save_path + rawname + "_3.png")
-            img_4 = img.crop([w / 2, h / 2, w, h])
-            img_4.save(save_path + rawname + "_4.png")
-            # loc
-            rawname = each.split("/")[-1].split(".")[0].split("-")[-2] + "-" + each.split("/")[-1].split(".")[0].split("-")[-1]
-            rawxy = position[rawname]
-            subloc_1 = [rawxy[0] - self.crop_size / 2, rawxy[1] - self.crop_size / 2, rawname + '_1']
-            subloc.append(subloc_1)
-            subloc_2 = [rawxy[0] + self.crop_size / 2, rawxy[1] - self.crop_size / 2, rawname + '_2']
-            subloc.append(subloc_2)
-            subloc_3 = [rawxy[0] - self.crop_size / 2, rawxy[1] + self.crop_size / 2, rawname + '_3']
-            subloc.append(subloc_3)
-            subloc_4 = [rawxy[0] + self.crop_size / 2, rawxy[1] + self.crop_size / 2, rawname + '_4']
-            subloc.append(subloc_4)
-
-        newsubloc = np.array(subloc)
-        np.savetxt(save_path + "subloc.txt", newsubloc, fmt='%s', delimiter='\t')
-
-
-
-    def PriorSpot_generator(self, prelabel_path, strategies='joint', threshold_proportion = 0.6, threshold_ration = 1.5):
-
-        """
-        Generator of prior spot.
-
-        Parameters
-        ----------
-        prelabel_path
-            Path of prelabel files.
-        strategies: {'joint', 'single_proportion', 'single_ration'}
-            Type of strategies to label the cell types for each spot.
-        threshold_proportion
-            The threshold of prior spot selection. Spots which the proportion of dominant cell types reached the threshold were selected as prior spots.
-        threshold_ration
-            The threshold of prior spot selection. Spots which the proportion of dominant cell types exceeded the given multiple of the proportion of secondary cell types were selected as prior spots.
-        """
-
-        self.prelabel_strategies = strategies
-        self.threshold_proportion = threshold_proportion
-        self.threshold_ration = threshold_ration
-        print("The strategy of pre-labelling is: " + str(self.prelabel_strategies))
-
-        if not os.path.exists(self.record_dir+"/PriorSpot/"):
-            os.makedirs(self.record_dir+"/PriorSpot/")
-
-        #self.Data = {}
-        #for each in self.position:
-        #    self.Data[each[2]] = [each[0], each[1]]
-
-        spot_C = {}
-        with open(prelabel_path + "Cell2location_prelabelling.txt") as f:
-            for line in f.readlines():
-                temp = line.split()
-                spot_C[temp[0]] = temp[1:]
-        with open(prelabel_path + "Cell2location_prelabelling.txt") as f:
-            Label_C = f.readlines()[0].split()
-
-        prior_spot = []
-
-        if self.prelabel_strategies == 'joint':
-            spot_S = {}
-            with open(prelabel_path + "Seurat_prelabelling.txt") as f:
-                for line in f.readlines():
-                    temp = line.split()
-                    spot_S[temp[0]] = temp[1:]
-            with open(prelabel_path + "Seurat_prelabelling.txt") as f:
-                Label_S = f.readlines()[0].split()
-
-            for each in self.Data.keys():
-                if each in spot_C.keys() and each in spot_S.keys():
-                    value_C = [float(k) for k in spot_C[each]]
-                    maxtype_C = Label_C[value_C.index(max(value_C))]
-                    value_S = [float(k) for k in spot_S[each]]
-                    maxtype_S = Label_S[value_S.index(max(value_S))]
-                    if maxtype_C == maxtype_S:
-                        temp = [each]
-                        temp.extend(self.Data[each])
-                        temp.extend([maxtype_C, maxtype_S])
-                        prior_spot.append(temp)
-
-        if self.prelabel_strategies == 'single_proportion':
-            print("The threshold of cell proportion is: " + str(threshold_proportion))
-            for each in self.Data.keys():
-                if each in spot_C.keys():
-                    value_C = [float(k) for k in spot_C[each]]
-                    maxtype_C = Label_C[value_C.index(max(value_C))]
-                    if max(value_C) / sum(value_C) > threshold_proportion:
-                        temp = [each]
-                        temp.extend(self.Data[each])
-                        temp.extend([maxtype_C, maxtype_C])
-                        prior_spot.append(temp)
-
-        if self.prelabel_strategies == 'single_ration':
-            print("The threshold of cell ration is: " + str(threshold_ration))
-            for each in self.Data.keys():
-                if each in spot_C.keys():
-                    value_C = [float(k) for k in spot_C[each]]
-                    ctype = Label_C[value_C.index(max(value_C))]
-                    value_C.sort()
-                    if value_C[-1] > value_C[-2] * threshold_ration:
-                        temp = [each]
-                        temp.extend(self.Data[each])
-                        temp.extend([ctype, ctype])
-                        prior_spot.append(temp)
-
-        self.prior_spot = prior_spot
-        print("The number of prior spots : ", len(prior_spot))
-        np.savetxt(self.record_dir+"/PriorSpot/prior_spot.txt", prior_spot, fmt='%s', delimiter='\t')
-        self.SpotImage_generator("PriorSpot")
-
-        return prior_spot
-
-
-
-    def RawSpot_generator(self):
-
-        if not os.path.exists(self.record_dir + "/RawSpot/"):
-            os.makedirs(self.record_dir + "/RawSpot/")
-
-        self.SpotImage_generator("RawSpot")
-
-
-
-    def SubSpot_generator(self):
-
-        if not os.path.exists(self.record_dir + "/SubSpot/"):
-            os.makedirs(self.record_dir + "/SubSpot/")
-        if not os.path.exists(self.record_dir + "/SubSpot/raw_divided/"):
-            os.makedirs(self.record_dir + "/SubSpot/raw_divided/")
-        if not os.path.exists(self.record_dir + "/SubSpot/prior_divided/"):
-            os.makedirs(self.record_dir + "/SubSpot/prior_divided")
-
-        self.SubSpotImage_generator("raw_divided")
-        self.SubSpotImage_generator("prior_divided")
-
-
-
-    def ImputedSpot_generator(self):
-
-        if not os.path.exists(self.record_dir + "/ImputedSpot/"):
-            os.makedirs(self.record_dir + "/ImputedSpot/")
-
-        all_s = []
-        sess = []
-        s = int(self.position[0][1])
-
-        for i in range(len(self.position)):
-            if self.position[i][1] == s:
-                sess.append(self.position[i])
-            else:
-                if int(self.position[i][1]) < s + self.crop_size:
-                    sess.append(self.position[i])
-                else:
-                    maxv = int(self.position[i - 1][1])
-                    averv = (s + maxv) / 2
-                    for j in range(len(sess)):
-                        sess[j][1] = averv
-                    all_s.append(sess)
-                    sess = []
-                    s = self.position[i][1]
-                    sess.append(self.position[i])
-
-        maxv = int(self.position[-1][1])
-        averv = (s + maxv) / 2
-        for j in range(len(sess)):
-            sess[j][1] = averv
-        all_s.append(sess)
-
-        for each in all_s:
-            each.sort(key=lambda x: (x[0]))
-
-        alls = []
-        for i in range(len(all_s)):
-            for j in range(len(all_s[i])):
-                alls.append(all_s[i][j])
-
-        np.savetxt(self.record_dir + "/ImputedSpot/adjust_raw_spot.txt", alls, fmt='%s', delimiter='\t')
-
-        fill = []
-
-        for i in range(len(all_s)):
-            for j in range(len(all_s[i]) - 1):
-                a = int(all_s[i][j + 1][0]) - int(all_s[i][j][0])
-                nx = int(all_s[i][j][0]) + a / 2
-                ny = int(all_s[i][j][1]) + int(a / ((3 ** 0.5) * 2))
-                nl = 'new-down' + all_s[i][j][2]
-                fill.append(nx)
-                fill.append(ny)
-                fill.append(nl)
-                ny = int(all_s[i][j][1]) - int(a / ((3 ** 0.5) * 2))
-                nl = 'new-up' + all_s[i][j][2]
-                fill.append(nx)
-                fill.append(ny)
-                fill.append(nl)
-
-        newfill = np.array(fill)
-        newfill = newfill.reshape(int(len(newfill) / 3), 3)
-
-        np.savetxt(self.record_dir + "/ImputedSpot/imputed_spot.txt", newfill, fmt='%s', delimiter='\t')
-        print("The number of imputed spots : ", len(newfill))
-
-        self.imputed_spot = newfill.tolist()
-        self.SpotImage_generator("ImputedSpot")
-
-
-
-
-
-class Shuffler():
-
-    def __init__(self, record_dir):
-
-        """
-        Shuffler of spot images.
-
-        Parameters
-        ----------
-        record_dir
-            Path of the input folder.
-        """
-
-        self.name = "Shuffler"
-        self.record_dir = record_dir
-
-
-
-    def Dataset_divider(self, input_spot, shuffle_scale=0.2):
-
-        """
-        Divider of spot image dataset.
-
-        Parameters
-        ----------
-        input_spot
-            Spots in the dataset, which used to determine cell classes.
-        shuffle_scale
-            Shuffle scale between training and testing sets.
-        """
-
-        Dir = list(set([x[-1] for x in input_spot]))
-
-        os.makedirs(self.record_dir + "/train/")
-        os.makedirs(self.record_dir + "/test/")
-        for each in Dir:
-            os.makedirs(self.record_dir + "/train/" + each)
-            os.makedirs(self.record_dir + "/test/" + each)
-
-        imgsLib = []
-        for n in Dir:
-            imgsLib.extend(glob.glob(os.path.join(self.record_dir, n + "*.png")))
-            for each in imgsLib:
-                dirpath = self.record_dir + "/train/" + n + "/"
-                shutil.move(each, dirpath)
-            imgsLib = []
-
-        imgsLib = []
-        for n in Dir:
-            imgsLib.extend(glob.glob(os.path.join(self.record_dir + "/train/" + n + "/", "*.png")))
-            np.random.shuffle(imgsLib)
-            num = int(len(imgsLib) * shuffle_scale)
-            for i in range(len(imgsLib[:num])):
-                scrpath = imgsLib[i]
-                dispath = self.record_dir + "/test/" + n + "/"
-                shutil.move(scrpath, dispath)
-            imgsLib = []
-
-
-
-    def KCross_divider(self, K_group, output_path):
-
-        """
-        Divider of K-fold cross image dataset.
-
-        Parameters
-        ----------
-        K_group
-            Number of fold cross.
-        output_path
-            Path of output folders.
-        """
-
-        rawimg = []
-        rawimg.extend(glob.glob(os.path.join(self.record_dir, "*.png")))
-
-        allcelltype = []
-        for each in rawimg:
-            allcelltype.append(each.split("/")[-1].split("-")[0])
-
-        Dir = list(set(allcelltype))
-
-        for i in range(K_group):
-            os.makedirs(output_path + "/group" + str(i+1) + "/")
-            os.makedirs(output_path + "/test" + str(i+1) + "/")
-            for each in rawimg:
-                shutil.copy(each, output_path + "/group" + str(i+1) + "/")
-            imgsLib = []
-            for n in Dir:
-                os.makedirs(output_path + "/group" + str(i+1) + "/" + n + "/")
-                os.makedirs(output_path + "/test" + str(i+1) + "/" + n + "/")
-                imgsLib.extend(glob.glob(os.path.join(output_path + "/group" + str(i+1) + "/", n + "*.png")))
-                for m in imgsLib:
-                    shutil.move(m, output_path + "/group" + str(i+1) + "/" + n + "/")
-                imgsLib = []
-                imgsLib.extend(glob.glob(os.path.join(output_path + "/group" + str(i+1) + "/" + n + "/", "*.png")))
-                np.random.shuffle(imgsLib)
-                num = int(len(imgsLib)/K_group)
-                for j in range(len(imgsLib[:num])):
-                    shutil.move(imgsLib[j], output_path + "/test" + str(i+1) + "/" + n + "/")
-                imgsLib = []
-
-
-
-
-
-class Detection():
-
-    def __init__(self):
-
-        """
-        Detection of spot images.
-
-        """
-
-        self.name = "Detection"
-
-
-
-    def DetectWhiteRegion(self, input_path, grey_level, threshold):
-
-        """
-        Detection of spot images with lagre white regions.
-
-        Parameters
-        ----------
-        input_path
-            Path of input images.
-        grey_level
-            Grey-level threshold of the image.
-        threshold
-            Threshold of white regions.
-        """
-        
-        imgsLib = []
-        imgsLib.extend(glob.glob(os.path.join(input_path, "*.png")))
-        
-        if not os.path.exists(input_path + "/whiteimg/"):
-            os.makedirs(input_path + "/whiteimg/")
-
-
-        for each in imgsLib:
-            img = Image.open(each)
-            imgG = img.convert('L')
-
-            rows = imgG.size[0]
-            cols = imgG.size[1]
-
-            q = 0
-            for i in range(rows):
-                for j in range(cols):
-                    if imgG.getpixel((i, j)) > grey_level:
-                        q += 1
-                        
-            if q/(rows*cols) > threshold:
+from pylab import *
+import numpy as np
+import cv2
+import os
+import random
+import glob
+import shutil
+from PIL import Image
+
+
+
+
+
+class Generator():
+
+    def __init__(self, record_dir, position, image, crop_size):
+
+        """
+        Preparation of spot images.
+
+        Parameters
+        ----------
+        record_dir
+            Path of the output folder.
+        position
+            The position of raw spots. Standard output file for Space Ranger.
+        image
+            The original H&E staining images, used for Space Ranger previously.
+        crop_size
+            Pixel radius of spot images.
+        """
+
+        self.name = "Generator"
+
+        self.record_dir = record_dir
+
+        self.position = []
+        with open(position) as f:
+            for line in f.readlines():
+                temp = line.split(',')
+                if int(temp[1]) == 1:
+                    self.position.append([int(temp[-1].split('\n')[0]), int(temp[-2]), temp[0]])
+        self.position.sort(key=lambda x: (x[1], x[0]))
+        print("The number of raw spots : ", len(self.position))
+        
+        self.Data = {}
+        for each in self.position:
+            self.Data[each[2]] = [each[0], each[1]]
+
+        self.rawimage = image
+        self.crop_size = crop_size
+
+
+
+    def SpotImage_generator(self, type):
+
+        """
+        Generator of spot images.
+
+        Parameters
+        ----------
+        type: {'RawSpot', 'PriorSpot', 'ImputedSpot'}
+            Type of spots.
+        """
+
+        img = cv2.imread(self.rawimage)
+        crop_size = self.crop_size
+
+        if type == 'RawSpot':
+            position = self.position
+            for each in position:
+                k = each[2].replace("\"", "")
+                cropped = img[int(each[1]) - crop_size:int(each[1]) + crop_size,
+                          int(each[0]) - crop_size:int(each[0]) + crop_size]
+                cv2.imwrite(self.record_dir + "/RawSpot/" + k + ".png", cropped)
+        elif type == 'PriorSpot':
+            position = self.prior_spot
+            for each in position:
+                k = each[0].replace("\"", "")
+                cropped = img[int(each[2]) - crop_size:int(each[2]) + crop_size,
+                          int(each[1]) - crop_size:int(each[1]) + crop_size]
+                celltype = each[-1]
+                cv2.imwrite(self.record_dir + "/PriorSpot/" + celltype + "-" + k + ".png", cropped)
+        elif type == 'ImputedSpot':
+            position = self.imputed_spot
+            for each in position:
+                k = each[2].replace("\"", "")
+                each[0], each[1] = float(each[0]), float(each[1])
+                cropped = img[int(each[1]) - crop_size:int(each[1]) + crop_size,
+                          int(each[0]) - crop_size:int(each[0]) + crop_size]
+                cv2.imwrite(self.record_dir + "/ImputedSpot/" + k + ".png", cropped)
+        else:
+            print("ERROR :The type of SpotImage doesn't exist!")
+
+
+
+    def SubSpotImage_generator(self, type):
+
+        """
+        Generator of subdivided spot images.
+
+        Parameters
+        ----------
+        type: {'raw_divided', 'prior_divided'}
+            Type of spots.
+        """
+
+        imgsLib = []
+        subloc = []
+        position = self.Data
+
+        if type == 'raw_divided':
+            img_path = self.record_dir + "/RawSpot/"
+            save_path = self.record_dir + "/SubSpot/raw_divided/"
+            #position = self.Data
+        if type == 'prior_divided':
+            img_path = self.record_dir + "/PriorSpot/"
+            save_path = self.record_dir + "/SubSpot/prior_divided/"
+            #position = {}
+            #if self.prior_spot == True:
+            #    for each in self.prior_spot:
+            #        position[each[0]] = [int(each[1]), int(each[2])]
+            #else:
+            #with open(self.record_dir + "/PriorSpot/prior_spot.txt") as f:
+            #    for line in f.readlines():
+            #        temp = line.split()
+            #        position[temp[0]] = [float(temp[1]), float(temp[2])]          
+        
+        
+
+        imgsLib.extend(glob.glob(os.path.join(img_path, "*.png")))
+
+        for each in imgsLib:
+            # img
+            image = Image.open(each)
+            img = image.convert('RGB')
+            w = img.size[0]
+            h = img.size[1]
+            rawname = each.split("/")[-1].split(".")[0]
+            img_1 = img.crop([0, 0, w / 2, h / 2])
+            img_1.save(save_path + rawname + "_1.png")
+            img_2 = img.crop([w / 2, 0, w, h / 2])
+            img_2.save(save_path + rawname + "_2.png")
+            img_3 = img.crop([0, h / 2, w / 2, h])
+            img_3.save(save_path + rawname + "_3.png")
+            img_4 = img.crop([w / 2, h / 2, w, h])
+            img_4.save(save_path + rawname + "_4.png")
+            # loc
+            rawname = each.split("/")[-1].split(".")[0].split("-")[-2] + "-" + each.split("/")[-1].split(".")[0].split("-")[-1]
+            rawxy = position[rawname]
+            subloc_1 = [rawxy[0] - self.crop_size / 2, rawxy[1] - self.crop_size / 2, rawname + '_1']
+            subloc.append(subloc_1)
+            subloc_2 = [rawxy[0] + self.crop_size / 2, rawxy[1] - self.crop_size / 2, rawname + '_2']
+            subloc.append(subloc_2)
+            subloc_3 = [rawxy[0] - self.crop_size / 2, rawxy[1] + self.crop_size / 2, rawname + '_3']
+            subloc.append(subloc_3)
+            subloc_4 = [rawxy[0] + self.crop_size / 2, rawxy[1] + self.crop_size / 2, rawname + '_4']
+            subloc.append(subloc_4)
+
+        newsubloc = np.array(subloc)
+        np.savetxt(save_path + "subloc.txt", newsubloc, fmt='%s', delimiter='\t')
+
+
+
+    def PriorSpot_generator(self, prelabel_path, strategies='joint', threshold_proportion = 0.6, threshold_ration = 1.5):
+
+        """
+        Generator of prior spot.
+
+        Parameters
+        ----------
+        prelabel_path
+            Path of prelabel files.
+        strategies: {'joint', 'single_proportion', 'single_ration'}
+            Type of strategies to label the cell types for each spot.
+        threshold_proportion
+            The threshold of prior spot selection. Spots which the proportion of dominant cell types reached the threshold were selected as prior spots.
+        threshold_ration
+            The threshold of prior spot selection. Spots which the proportion of dominant cell types exceeded the given multiple of the proportion of secondary cell types were selected as prior spots.
+        """
+
+        self.prelabel_strategies = strategies
+        self.threshold_proportion = threshold_proportion
+        self.threshold_ration = threshold_ration
+        print("The strategy of pre-labelling is: " + str(self.prelabel_strategies))
+
+        if not os.path.exists(self.record_dir+"/PriorSpot/"):
+            os.makedirs(self.record_dir+"/PriorSpot/")
+
+        #self.Data = {}
+        #for each in self.position:
+        #    self.Data[each[2]] = [each[0], each[1]]
+
+        spot_C = {}
+        with open(prelabel_path + "Cell2location_prelabelling.txt") as f:
+            for line in f.readlines():
+                temp = line.split()
+                spot_C[temp[0]] = temp[1:]
+        with open(prelabel_path + "Cell2location_prelabelling.txt") as f:
+            Label_C = f.readlines()[0].split()
+
+        prior_spot = []
+
+        if self.prelabel_strategies == 'joint':
+            spot_S = {}
+            with open(prelabel_path + "Seurat_prelabelling.txt") as f:
+                for line in f.readlines():
+                    temp = line.split()
+                    spot_S[temp[0]] = temp[1:]
+            with open(prelabel_path + "Seurat_prelabelling.txt") as f:
+                Label_S = f.readlines()[0].split()
+
+            for each in self.Data.keys():
+                if each in spot_C.keys() and each in spot_S.keys():
+                    value_C = [float(k) for k in spot_C[each]]
+                    maxtype_C = Label_C[value_C.index(max(value_C))]
+                    value_S = [float(k) for k in spot_S[each]]
+                    maxtype_S = Label_S[value_S.index(max(value_S))]
+                    if maxtype_C == maxtype_S:
+                        temp = [each]
+                        temp.extend(self.Data[each])
+                        temp.extend([maxtype_C, maxtype_S])
+                        prior_spot.append(temp)
+
+        if self.prelabel_strategies == 'single_proportion':
+            print("The threshold of cell proportion is: " + str(threshold_proportion))
+            for each in self.Data.keys():
+                if each in spot_C.keys():
+                    value_C = [float(k) for k in spot_C[each]]
+                    maxtype_C = Label_C[value_C.index(max(value_C))]
+                    if max(value_C) / sum(value_C) > threshold_proportion:
+                        temp = [each]
+                        temp.extend(self.Data[each])
+                        temp.extend([maxtype_C, maxtype_C])
+                        prior_spot.append(temp)
+
+        if self.prelabel_strategies == 'single_ration':
+            print("The threshold of cell ration is: " + str(threshold_ration))
+            for each in self.Data.keys():
+                if each in spot_C.keys():
+                    value_C = [float(k) for k in spot_C[each]]
+                    ctype = Label_C[value_C.index(max(value_C))]
+                    value_C.sort()
+                    if value_C[-1] > value_C[-2] * threshold_ration:
+                        temp = [each]
+                        temp.extend(self.Data[each])
+                        temp.extend([ctype, ctype])
+                        prior_spot.append(temp)
+
+        self.prior_spot = prior_spot
+        print("The number of prior spots : ", len(prior_spot))
+        np.savetxt(self.record_dir+"/PriorSpot/prior_spot.txt", prior_spot, fmt='%s', delimiter='\t')
+        self.SpotImage_generator("PriorSpot")
+
+        return prior_spot
+
+
+
+    def RawSpot_generator(self):
+
+        if not os.path.exists(self.record_dir + "/RawSpot/"):
+            os.makedirs(self.record_dir + "/RawSpot/")
+
+        self.SpotImage_generator("RawSpot")
+
+
+
+    def SubSpot_generator(self):
+
+        if not os.path.exists(self.record_dir + "/SubSpot/"):
+            os.makedirs(self.record_dir + "/SubSpot/")
+        if not os.path.exists(self.record_dir + "/SubSpot/raw_divided/"):
+            os.makedirs(self.record_dir + "/SubSpot/raw_divided/")
+        if not os.path.exists(self.record_dir + "/SubSpot/prior_divided/"):
+            os.makedirs(self.record_dir + "/SubSpot/prior_divided")
+
+        self.SubSpotImage_generator("raw_divided")
+        self.SubSpotImage_generator("prior_divided")
+
+
+
+    def ImputedSpot_generator(self):
+
+        if not os.path.exists(self.record_dir + "/ImputedSpot/"):
+            os.makedirs(self.record_dir + "/ImputedSpot/")
+
+        all_s = []
+        sess = []
+        s = int(self.position[0][1])
+
+        for i in range(len(self.position)):
+            if self.position[i][1] == s:
+                sess.append(self.position[i])
+            else:
+                if int(self.position[i][1]) < s + self.crop_size:
+                    sess.append(self.position[i])
+                else:
+                    maxv = int(self.position[i - 1][1])
+                    averv = (s + maxv) / 2
+                    for j in range(len(sess)):
+                        sess[j][1] = averv
+                    all_s.append(sess)
+                    sess = []
+                    s = self.position[i][1]
+                    sess.append(self.position[i])
+
+        maxv = int(self.position[-1][1])
+        averv = (s + maxv) / 2
+        for j in range(len(sess)):
+            sess[j][1] = averv
+        all_s.append(sess)
+
+        for each in all_s:
+            each.sort(key=lambda x: (x[0]))
+
+        alls = []
+        for i in range(len(all_s)):
+            for j in range(len(all_s[i])):
+                alls.append(all_s[i][j])
+
+        np.savetxt(self.record_dir + "/ImputedSpot/adjust_raw_spot.txt", alls, fmt='%s', delimiter='\t')
+
+        fill = []
+
+        for i in range(len(all_s)):
+            for j in range(len(all_s[i]) - 1):
+                a = int(all_s[i][j + 1][0]) - int(all_s[i][j][0])
+                nx = int(all_s[i][j][0]) + a / 2
+                ny = int(all_s[i][j][1]) + int(a / ((3 ** 0.5) * 2))
+                nl = 'new-down' + all_s[i][j][2]
+                fill.append(nx)
+                fill.append(ny)
+                fill.append(nl)
+                ny = int(all_s[i][j][1]) - int(a / ((3 ** 0.5) * 2))
+                nl = 'new-up' + all_s[i][j][2]
+                fill.append(nx)
+                fill.append(ny)
+                fill.append(nl)
+
+        newfill = np.array(fill)
+        newfill = newfill.reshape(int(len(newfill) / 3), 3)
+
+        np.savetxt(self.record_dir + "/ImputedSpot/imputed_spot.txt", newfill, fmt='%s', delimiter='\t')
+        print("The number of imputed spots : ", len(newfill))
+
+        self.imputed_spot = newfill.tolist()
+        self.SpotImage_generator("ImputedSpot")
+
+
+
+
+
+class Shuffler():
+
+    def __init__(self, record_dir):
+
+        """
+        Shuffler of spot images.
+
+        Parameters
+        ----------
+        record_dir
+            Path of the input folder.
+        """
+
+        self.name = "Shuffler"
+        self.record_dir = record_dir
+
+
+
+    def Dataset_divider(self, input_spot, shuffle_scale=0.2):
+
+        """
+        Divider of spot image dataset.
+
+        Parameters
+        ----------
+        input_spot
+            Spots in the dataset, which used to determine cell classes.
+        shuffle_scale
+            Shuffle scale between training and testing sets.
+        """
+
+        Dir = list(set([x[-1] for x in input_spot]))
+
+        os.makedirs(self.record_dir + "/train/")
+        os.makedirs(self.record_dir + "/test/")
+        for each in Dir:
+            os.makedirs(self.record_dir + "/train/" + each)
+            os.makedirs(self.record_dir + "/test/" + each)
+
+        imgsLib = []
+        for n in Dir:
+            imgsLib.extend(glob.glob(os.path.join(self.record_dir, n + "*.png")))
+            for each in imgsLib:
+                dirpath = self.record_dir + "/train/" + n + "/"
+                shutil.move(each, dirpath)
+            imgsLib = []
+
+        imgsLib = []
+        for n in Dir:
+            imgsLib.extend(glob.glob(os.path.join(self.record_dir + "/train/" + n + "/", "*.png")))
+            np.random.shuffle(imgsLib)
+            num = int(len(imgsLib) * shuffle_scale)
+            for i in range(len(imgsLib[:num])):
+                scrpath = imgsLib[i]
+                dispath = self.record_dir + "/test/" + n + "/"
+                shutil.move(scrpath, dispath)
+            imgsLib = []
+
+
+
+    def KCross_divider(self, K_group, output_path):
+
+        """
+        Divider of K-fold cross image dataset.
+
+        Parameters
+        ----------
+        K_group
+            Number of fold cross.
+        output_path
+            Path of output folders.
+        """
+
+        rawimg = []
+        rawimg.extend(glob.glob(os.path.join(self.record_dir, "*.png")))
+
+        allcelltype = []
+        for each in rawimg:
+            allcelltype.append(each.split("/")[-1].split("-")[0])
+
+        Dir = list(set(allcelltype))
+
+        for i in range(K_group):
+            os.makedirs(output_path + "/group" + str(i+1) + "/")
+            os.makedirs(output_path + "/test" + str(i+1) + "/")
+            for each in rawimg:
+                shutil.copy(each, output_path + "/group" + str(i+1) + "/")
+            imgsLib = []
+            for n in Dir:
+                os.makedirs(output_path + "/group" + str(i+1) + "/" + n + "/")
+                os.makedirs(output_path + "/test" + str(i+1) + "/" + n + "/")
+                imgsLib.extend(glob.glob(os.path.join(output_path + "/group" + str(i+1) + "/", n + "*.png")))
+                for m in imgsLib:
+                    shutil.move(m, output_path + "/group" + str(i+1) + "/" + n + "/")
+                imgsLib = []
+                imgsLib.extend(glob.glob(os.path.join(output_path + "/group" + str(i+1) + "/" + n + "/", "*.png")))
+                np.random.shuffle(imgsLib)
+                num = int(len(imgsLib)/K_group)
+                for j in range(len(imgsLib[:num])):
+                    shutil.move(imgsLib[j], output_path + "/test" + str(i+1) + "/" + n + "/")
+                imgsLib = []
+
+
+
+
+
+class Detection():
+
+    def __init__(self):
+
+        """
+        Detection of spot images.
+
+        """
+
+        self.name = "Detection"
+
+
+
+    def DetectWhiteRegion(self, input_path, grey_level, threshold):
+
+        """
+        Detection of spot images with lagre white regions.
+
+        Parameters
+        ----------
+        input_path
+            Path of input images.
+        grey_level
+            Grey-level threshold of the image.
+        threshold
+            Threshold of white regions.
+        """
+        
+        imgsLib = []
+        imgsLib.extend(glob.glob(os.path.join(input_path, "*.png")))
+        
+        if not os.path.exists(input_path + "/whiteimg/"):
+            os.makedirs(input_path + "/whiteimg/")
+
+
+        for each in imgsLib:
+            img = Image.open(each)
+            imgG = img.convert('L')
+
+            rows = imgG.size[0]
+            cols = imgG.size[1]
+
+            q = 0
+            for i in range(rows):
+                for j in range(cols):
+                    if imgG.getpixel((i, j)) > grey_level:
+                        q += 1
+                        
+            if q/(rows*cols) > threshold:
                 shutil.move(each, input_path + "/whiteimg/")
```

### Comparing `STASCAN-1.0.0/STASCAN/run_STASCAN.py` & `STASCAN-1.1.0/STASCAN/run_STASCAN.py`

 * *Files identical despite different names*

### Comparing `STASCAN-1.0.0/STASCAN.egg-info/PKG-INFO` & `STASCAN-1.1.0/STASCAN.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-Metadata-Version: 2.1
-Name: STASCAN
-Version: 1.0.0
-Summary: An AI-driven method for enhanced cellular organizational map in spatial transcriptomics
-Home-page: https://github.com/AbbyWY/STASCAN
-Author: Ying Wu
-Author-email: wuy@big.ac.cn
-License: MIT
-Platform: UNKNOWN
-License-File: LICENSE.txt
-
-Here we propose STASCAN, which both gene expression and the morphological information are simultaneously utilized to improve the cellular resolution of captured domains and even gap regions. Besides, STASCAN is further designed to enable cell-type predictions at subdivide-spot resolution and construction of the 3D spatial cell map from histology images alone.
-
+Metadata-Version: 1.0
+Name: STASCAN
+Version: 1.1.0
+Summary: An AI-driven method for enhanced cellular organizational map in spatial transcriptomics
+Home-page: https://github.com/AbbyWY/STASCAN
+Author: Ying Wu
+Author-email: wuy@big.ac.cn
+License: MIT
+Description: Here we propose STASCAN, which both gene expression and the morphological information are simultaneously utilized to improve the cellular resolution of captured domains and even gap regions. Besides, STASCAN is further designed to enable cell-type predictions at subdivide-spot resolution and construction of the 3D spatial cell map from histology images alone.
+Platform: UNKNOWN
```

### Comparing `STASCAN-1.0.0/setup.py` & `STASCAN-1.1.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from setuptools import Command, find_packages, setup
-
-__lib_name__ = "STASCAN"
-__lib_version__ = "1.0.0"
-__description__ = "An AI-driven method for enhanced cellular organizational map in spatial transcriptomics"
-__url__ = "https://github.com/AbbyWY/STASCAN"
-__author__ = "Ying Wu"
-__author_email__ = "wuy@big.ac.cn"
-__license__ = "MIT"
-__requires__ = ["requests",]
-__long_description__ = "Here we propose STASCAN, which both gene expression and the morphological information are simultaneously utilized to improve the cellular resolution of captured domains and even gap regions. Besides, STASCAN is further designed to enable cell-type predictions at subdivide-spot resolution and construction of the 3D spatial cell map from histology images alone."
-
-
-setup(
-    name = __lib_name__,
-    version = __lib_version__,
-    description = __description__,
-    url = __url__,
-    author = __author__,
-    author_email = __author_email__,
-    license = __license__,
-    packages = ['STASCAN'],
-    install_requires = __requires__,
-    zip_safe = False,
-    include_package_data = True,
-    long_description = __long_description__
-)
+from setuptools import Command, find_packages, setup
+
+__lib_name__ = "STASCAN"
+__lib_version__ = "1.1.0"
+__description__ = "An AI-driven method for enhanced cellular organizational map in spatial transcriptomics"
+__url__ = "https://github.com/AbbyWY/STASCAN"
+__author__ = "Ying Wu"
+__author_email__ = "wuy@big.ac.cn"
+__license__ = "MIT"
+__requires__ = ["requests",]
+__long_description__ = "Here we propose STASCAN, which both gene expression and the morphological information are simultaneously utilized to improve the cellular resolution of captured domains and even gap regions. Besides, STASCAN is further designed to enable cell-type predictions at subdivide-spot resolution and construction of the 3D spatial cell map from histology images alone."
+
+
+setup(
+    name = __lib_name__,
+    version = __lib_version__,
+    description = __description__,
+    url = __url__,
+    author = __author__,
+    author_email = __author_email__,
+    license = __license__,
+    packages = ['STASCAN'],
+    install_requires = __requires__,
+    zip_safe = False,
+    include_package_data = True,
+    long_description = __long_description__
+)
```

