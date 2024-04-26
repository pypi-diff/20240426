# Comparing `tmp/pyretailscience-0.2.0.tar.gz` & `tmp/pyretailscience-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyretailscience-0.2.0.tar", max compression
+gzip compressed data, was "pyretailscience-0.3.0.tar", max compression
```

## Comparing `pyretailscience-0.2.0.tar` & `pyretailscience-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0     3860 2024-03-13 19:31:43.539586 pyretailscience-0.2.0/LICENSE
--rw-r--r--   0        0        0     2698 2024-03-13 19:31:43.539586 pyretailscience-0.2.0/README.md
--rw-r--r--   0        0        0     1014 2024-03-13 19:32:49.412082 pyretailscience-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-13 19:31:43.547586 pyretailscience-0.2.0/pyretailscience/__init__.py
--rw-r--r--   0        0        0    13529 2024-03-13 19:31:43.547586 pyretailscience-0.2.0/pyretailscience/customer.py
--rw-r--r--   0        0        0        0 2024-03-13 19:31:43.547586 pyretailscience-0.2.0/pyretailscience/data/__init__.py
--rw-r--r--   0        0        0     1165 2024-03-13 19:31:43.547586 pyretailscience-0.2.0/pyretailscience/data/cli.py
--rw-r--r--   0        0        0    17441 2024-03-13 19:31:43.547586 pyretailscience-0.2.0/pyretailscience/data/contracts.py
--rw-r--r--   0        0        0    15906 2024-03-13 19:31:43.547586 pyretailscience-0.2.0/pyretailscience/data/simulation.py
--rw-r--r--   0        0        0     1210 2024-03-13 19:31:43.547586 pyretailscience-0.2.0/pyretailscience/style/graph_utils.py
--rw-r--r--   0        0        0     9316 2024-03-13 19:31:43.547586 pyretailscience-0.2.0/pyretailscience/style/tailwind.py
--rw-r--r--   0        0        0     3620 1970-01-01 00:00:00.000000 pyretailscience-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3860 2024-04-26 11:18:31.449879 pyretailscience-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2701 2024-04-26 11:18:31.449879 pyretailscience-0.3.0/README.md
+-rw-r--r--   0        0        0     1056 2024-04-26 11:19:40.609992 pyretailscience-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/__init__.py
+-rw-r--r--   0        0        0    15090 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/customer.py
+-rw-r--r--   0        0        0        0 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/data/__init__.py
+-rw-r--r--   0        0        0     1165 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/data/cli.py
+-rw-r--r--   0        0        0    17441 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/data/contracts.py
+-rw-r--r--   0        0        0    16021 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/data/simulation.py
+-rw-r--r--   0        0        0    12493 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/range_planning.py
+-rw-r--r--   0        0        0     9192 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/segmentation.py
+-rw-r--r--   0        0        0     3528 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/standard_graphs.py
+-rw-r--r--   0        0        0     2488 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/style/graph_utils.py
+-rw-r--r--   0        0        0     9316 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/style/tailwind.py
+-rw-r--r--   0        0        0     3707 1970-01-01 00:00:00.000000 pyretailscience-0.3.0/PKG-INFO
```

### Comparing `pyretailscience-0.2.0/LICENSE` & `pyretailscience-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyretailscience-0.2.0/README.md` & `pyretailscience-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,33 +19,36 @@
 ## Quick Start
 
 ### Generating Simulated Data
 
 The `pyretailscience` package provides a command-line interface for generating simulated transaction data.
 
 #### Usage
+
 ```bash
 pyretailscience --config_file=<config_file_path> [--verbose=<True|False>] [--seed=<seed_number>] [output]
 ```
 
 #### Options and Arguments
+
 - `--config_file=<config_file_path>`: The path to the configuration file for the simulation. This is a required argument.
 - `--verbose=<True|False>`: Optional. Set to `True` to see debug messages. Default is `False`.
 - `--seed=<seed_number>`: Optional. Seed for the random number generator used in the simulation. If not provided, a random seed will be used.
 - `[output]`: Optional. The path where the generated transactions will be saved in parquet format. If not provided, the transactions will be saved in the current directory.
 
 #### Examples
+
 ```bash
 # Get the default transaction config file
-wget https://raw.githubusercontent.com/Data-Simply/pyretailscience/0.1.1/data/default_data_config.yaml
+wget https://raw.githubusercontent.com/Data-Simply/pyretailscience/0.3.0/data/default_data_config.yaml
 # Generate the data file
 pyretailscience --config_file=default_data_config.yaml --seed=123 transactions.parquet
 ```
-This command will generate a file named `transactions.parquet` with the simulated transaction data, using the configuration file at default data configuration file, and a seed of `123` for the random number generator.
 
+This command will generate a file named `transactions.parquet` with the simulated transaction data, using the configuration file at default data configuration file, and a seed of `123` for the random number generator.
 
 # Contributing
 
 We welcome contributions from the community to enhance and improve pyretailscience. To contribute, please follow these steps:
 
 1. Fork the repository.
 2. Create a new branch for your feature or bug fix.
```

#### html2text {}

```diff
@@ -14,15 +14,15 @@
 argument. - `--verbose=
 False>`: Optional. Set to `True` to see debug messages. Default is `False`. -
 `--seed=`: Optional. Seed for the random number generator used in the
 simulation. If not provided, a random seed will be used. - `[output]`:
 Optional. The path where the generated transactions will be saved in parquet
 format. If not provided, the transactions will be saved in the current
 directory. #### Examples ```bash # Get the default transaction config file wget
-https://raw.githubusercontent.com/Data-Simply/pyretailscience/0.1.1/data/
+https://raw.githubusercontent.com/Data-Simply/pyretailscience/0.3.0/data/
 default_data_config.yaml # Generate the data file pyretailscience --
 config_file=default_data_config.yaml --seed=123 transactions.parquet ``` This
 command will generate a file named `transactions.parquet` with the simulated
 transaction data, using the configuration file at default data configuration
 file, and a seed of `123` for the random number generator. # Contributing We
 welcome contributions from the community to enhance and improve
 pyretailscience. To contribute, please follow these steps: 1. Fork the
```

### Comparing `pyretailscience-0.2.0/pyproject.toml` & `pyretailscience-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyretailscience"
-version = "0.2.0"
+version = "0.3.0"
 description = "Retail Data Science Tools"
 authors = ["Murray Vanwyk <2493311+mvanwyk@users.noreply.github.com>"]
 readme = "README.md"
 license = "Elastic-2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
@@ -15,14 +15,16 @@
 click = "^8.1.7"
 seaborn = "^0.13.1"
 strictyaml = "^1.7.3"
 loguru = "^0.7.2"
 tqdm = "^4.66.1"
 great-expectations = "^0.18.8"
 pre-commit ="^3.6.2"
+scipy = "^1.13.0"
+scikit-learn = "^1.4.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^4.1.0"
 
 
 [tool.poetry.group.examples.dependencies]
```

### Comparing `pyretailscience-0.2.0/pyretailscience/customer.py` & `pyretailscience-0.3.0/pyretailscience/customer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import matplotlib.pyplot as plt
+import operator
+
 import matplotlib.ticker as mtick
 import pandas as pd
 from matplotlib.axes import Axes, SubplotBase
 
 from pyretailscience.data.contracts import TransactionItemLevelContract
+from pyretailscience.style.graph_utils import GraphStyles as gs
 from pyretailscience.style.graph_utils import human_format, standard_graph_styles
 from pyretailscience.style.tailwind import COLORS
-import operator
 
 
 class PurchasesPerCustomer:
     """A class to plot the distribution of the number of purchases per customer.
 
     Attributes:
         cust_purchases_s (pd.Series): The number of purchases per customer.
@@ -29,15 +30,18 @@
     def plot(
         self,
         bins: int = 10,
         cumlative: bool = False,
         ax: Axes | None = None,
         draw_percentile_line: bool = False,
         percentile_line: float = 0.5,
-        source_text: str = None,
+        source_text: str | None = None,
+        title: str | None = None,
+        xlabel: str | None = None,
+        ylabel: str | None = None,
         **kwargs: dict[str, any],
     ) -> SubplotBase:
         """Plot the distribution of the number of purchases per customer.
 
         Args:
             bins (int, optional): The number of bins to plot. Defaults to 10.
             cumlative (bool, optional): Whether to plot the cumulative distribution. Defaults to False.
@@ -50,37 +54,48 @@
             SubplotBase: The Matplotlib axes of the plot
         """
 
         density = False
         if cumlative:
             density = True
 
+        if xlabel is None:
+            xlabel = "Number of purchases"
+
         ax = self.cust_purchases_s.hist(
             bins=bins,
             cumulative=cumlative,
             ax=ax,
             density=density,
             color=COLORS["green"][500],
             **kwargs,
         )
-        ax.set_xlabel("Number of purchases")
+
+        ax.set_xlabel(xlabel, fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE, labelpad=10)
         ax.xaxis.set_major_formatter(lambda x, pos: human_format(x, pos, decimals=0))
 
         ax = standard_graph_styles(ax)
 
         if cumlative:
-            plt.title("Number of Purchases Cumulative Distribution")
-            plt.ylabel("Percentage of customers")
+            if title is None:
+                title = "Number of Purchases Cumulative Distribution"
+            if ylabel is None:
+                ylabel = "Percentage of customers"
             ax.yaxis.set_major_formatter(mtick.PercentFormatter(xmax=1, decimals=0))
 
         else:
-            plt.title("Number of Purchases Distribution")
-            plt.ylabel("Number of customers")
+            if title is None:
+                title = "Number of Purchases Distribution"
+            if ylabel is None:
+                ylabel = "Number of customers"
             ax.yaxis.set_major_formatter(lambda x, pos: human_format(x, pos, decimals=0))
 
+        ax.set_title(title, fontsize=gs.DEFAULT_TITLE_FONT_SIZE, pad=15)
+        ax.set_ylabel(ylabel, fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE, labelpad=10)
+
         if draw_percentile_line:
             if percentile_line > 1 or percentile_line < 0:
                 raise ValueError("Percentile line must be between 0 and 1")
             ax.axvline(
                 x=self.purchases_percentile(percentile_line),
                 color=COLORS["red"][500],
                 linestyle="--",
@@ -92,15 +107,15 @@
         if source_text:
             ax.annotate(
                 source_text,
                 xy=(-0.1, -0.2),
                 xycoords="axes fraction",
                 ha="left",
                 va="center",
-                fontsize=10,
+                fontsize=gs.DEFAULT_SOURCE_FONT_SIZE,
             )
 
         return ax
 
     def purchases_percentile(self, percentile: float = 0.5) -> float:
         """Get the number of purchases at a given percentile.
 
@@ -172,14 +187,17 @@
     def plot(
         self,
         bins: int = 10,
         cumlative: bool = False,
         ax: Axes | None = None,
         draw_percentile_line: bool = False,
         percentile_line: float = 0.5,
+        title: str | None = None,
+        xlabel: str | None = None,
+        ylabel: str | None = None,
         source_text: str = None,
         **kwargs: dict[str, any],
     ) -> SubplotBase:
         """Plot the distribution of the average number of days between purchases per customer.
 
         Args:
             bins (int, optional): The number of bins to plot. Defaults to 10.
@@ -200,29 +218,39 @@
             bins=bins,
             cumulative=cumlative,
             ax=ax,
             density=density,
             color=COLORS["green"][500],
             **kwargs,
         )
-        plt.xlabel("Average Number of Days Between Purchases")
+
+        if xlabel is None:
+            xlabel = "Average Number of Days Between Purchases"
+        ax.set_xlabel(xlabel, fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE, labelpad=10)
         ax.xaxis.set_major_formatter(lambda x, pos: human_format(x, pos, decimals=0))
 
         ax = standard_graph_styles(ax)
 
         if cumlative:
-            plt.title("Average Days Between Purchases Cumulative Distribution")
-            plt.ylabel("Percentage of Customers")
+            if title is None:
+                title = "Average Days Between Purchases Cumulative Distribution"
+            if ylabel is None:
+                ylabel = "Percentage of Customers"
             ax.yaxis.set_major_formatter(mtick.PercentFormatter(xmax=1, decimals=0))
 
         else:
-            plt.title("Average Days Between Purchases Distribution")
-            plt.ylabel("Number of Customers")
+            if title is None:
+                title = "Average Days Between Purchases Distribution"
+            if ylabel is None:
+                ylabel = "Number of Customers"
             ax.yaxis.set_major_formatter(lambda x, pos: human_format(x, pos, decimals=0))
 
+        ax.set_title(title, fontsize=gs.DEFAULT_TITLE_FONT_SIZE, pad=15)
+        ax.set_ylabel(ylabel, fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE, labelpad=10)
+
         if draw_percentile_line:
             if percentile_line > 1 or percentile_line < 0:
                 raise ValueError("Percentile line must be between 0 and 1")
             ax.axvline(
                 x=self.purchases_percentile(percentile_line),
                 color=COLORS["red"][500],
                 linestyle="--",
@@ -235,15 +263,15 @@
         if source_text:
             ax.annotate(
                 source_text,
                 xy=(-0.1, -0.2),
                 xycoords="axes fraction",
                 ha="left",
                 va="center",
-                fontsize=10,
+                fontsize=gs.DEFAULT_SOURCE_FONT_SIZE,
             )
 
         return ax
 
     def purchases_percentile(self, percentile: float = 0.5) -> float:
         """Get the average number of days between purchases at a given percentile.
 
@@ -302,50 +330,62 @@
 
         self.n_unique_customers = df["customer_id"].nunique()
 
     def plot(
         self,
         cumlative: bool = False,
         ax: Axes | None = None,
+        title: str | None = None,
+        xlabel: str | None = None,
+        ylabel: str | None = None,
         source_text: str = None,
         **kwargs: dict[str, any],
     ) -> SubplotBase:
         """Plot the churn rate by number of purchases.
 
         Args:
             cumlative (bool, optional): Whether to plot the cumulative distribution. Defaults to False.
             ax (Axes, optional): The Matplotlib axes to plot the graph on. Defaults to None.
 
         Returns:
             SubplotBase: The Matplotlib axes of the plot
         """
         if cumlative:
             cumulative_churn_rate_s = self.purchase_dist_df["churned"].cumsum().div(self.n_unique_customers)
-            ax = cumulative_churn_rate_s.plot.area(color=COLORS["green"][500])
+            ax = cumulative_churn_rate_s.plot.area(
+                color=COLORS["green"][500],
+                **kwargs,
+            )
             ax.set_xlim(self.purchase_dist_df.index.min(), self.purchase_dist_df.index.max())
         else:
             ax = self.purchase_dist_df["churned_pct"].plot.bar(
                 rot=0,
                 color=COLORS["green"][500],
                 width=0.8,
                 **kwargs,
             )
 
         standard_graph_styles(ax)
 
-        # Format y axis as a percent
+        if title is None:
+            title = "Churn Rate by Number of Purchases"
+        if xlabel is None:
+            xlabel = "Number of Purchases"
+        if ylabel is None:
+            ylabel = "% Churned"
+
         ax.yaxis.set_major_formatter(mtick.PercentFormatter(xmax=1.0))
-        ax.set_xlabel("Number of Purchases")
-        ax.set_ylabel("% Churned")
-        ax.set_title("Churn Rate by Number of Purchases")
+        ax.set_xlabel(xlabel, fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE, labelpad=10)
+        ax.set_ylabel(ylabel, fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE, labelpad=10)
+        ax.set_title(title, fontsize=gs.DEFAULT_TITLE_FONT_SIZE, pad=15)
 
         if source_text:
             ax.annotate(
                 source_text,
                 xy=(-0.1, -0.2),
                 xycoords="axes fraction",
                 ha="left",
                 va="center",
-                fontsize=10,
+                fontsize=gs.DEFAULT_SOURCE_FONT_SIZE,
             )
 
         return ax
```

### Comparing `pyretailscience-0.2.0/pyretailscience/data/cli.py` & `pyretailscience-0.3.0/pyretailscience/data/cli.py`

 * *Files identical despite different names*

### Comparing `pyretailscience-0.2.0/pyretailscience/data/contracts.py` & `pyretailscience-0.3.0/pyretailscience/data/contracts.py`

 * *Files identical despite different names*

### Comparing `pyretailscience-0.2.0/pyretailscience/data/simulation.py` & `pyretailscience-0.3.0/pyretailscience/data/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,18 +345,20 @@
             date (date): Date of the simulation
 
         Returns:
             None
         """
         num_new_customers = self.rnd_generator.poisson(self.config["customers"]["average_new_customers_per_day"])
         logger.debug(f"Adding {num_new_customers} new customers")
+        last_customer_id = len(self.customers)
+        last_new_customer_id = last_customer_id + num_new_customers
         self.customers.extend(
             [
                 self._create_customer(customer_id=new_customer_id)
-                for new_customer_id in range(len(self.customers) + 1, num_new_customers + 1)
+                for new_customer_id in range(last_customer_id + 1, last_new_customer_id + 1)
             ]
         )
         # Simulate each customer
         for customer in self.customers:
             customer.step(date)
 
     def run(self) -> None:
```

### Comparing `pyretailscience-0.2.0/pyretailscience/style/tailwind.py` & `pyretailscience-0.3.0/pyretailscience/style/tailwind.py`

 * *Files identical despite different names*

### Comparing `pyretailscience-0.2.0/PKG-INFO` & `pyretailscience-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyretailscience
-Version: 0.2.0
+Version: 0.3.0
 Summary: Retail Data Science Tools
 License: Elastic-2.0
 Author: Murray Vanwyk
 Author-email: 2493311+mvanwyk@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,16 @@
 Requires-Dist: great-expectations (>=0.18.8,<0.19.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: pre-commit (>=3.6.2,<4.0.0)
 Requires-Dist: pyarrow (>=14.0.2,<15.0.0)
+Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
+Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Requires-Dist: seaborn (>=0.13.1,<0.14.0)
 Requires-Dist: strictyaml (>=1.7.3,<2.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 ![pyretailscience logo](https://raw.githubusercontent.com/Data-Simply/pyretailscience/main/logo.png)
 
@@ -44,33 +46,36 @@
 ## Quick Start
 
 ### Generating Simulated Data
 
 The `pyretailscience` package provides a command-line interface for generating simulated transaction data.
 
 #### Usage
+
 ```bash
 pyretailscience --config_file=<config_file_path> [--verbose=<True|False>] [--seed=<seed_number>] [output]
 ```
 
 #### Options and Arguments
+
 - `--config_file=<config_file_path>`: The path to the configuration file for the simulation. This is a required argument.
 - `--verbose=<True|False>`: Optional. Set to `True` to see debug messages. Default is `False`.
 - `--seed=<seed_number>`: Optional. Seed for the random number generator used in the simulation. If not provided, a random seed will be used.
 - `[output]`: Optional. The path where the generated transactions will be saved in parquet format. If not provided, the transactions will be saved in the current directory.
 
 #### Examples
+
 ```bash
 # Get the default transaction config file
-wget https://raw.githubusercontent.com/Data-Simply/pyretailscience/0.1.1/data/default_data_config.yaml
+wget https://raw.githubusercontent.com/Data-Simply/pyretailscience/0.3.0/data/default_data_config.yaml
 # Generate the data file
 pyretailscience --config_file=default_data_config.yaml --seed=123 transactions.parquet
 ```
-This command will generate a file named `transactions.parquet` with the simulated transaction data, using the configuration file at default data configuration file, and a seed of `123` for the random number generator.
 
+This command will generate a file named `transactions.parquet` with the simulated transaction data, using the configuration file at default data configuration file, and a seed of `123` for the random number generator.
 
 # Contributing
 
 We welcome contributions from the community to enhance and improve pyretailscience. To contribute, please follow these steps:
 
 1. Fork the repository.
 2. Create a new branch for your feature or bug fix.
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: pyretailscience Version: 0.2.0 Summary: Retail Data
+Metadata-Version: 2.1 Name: pyretailscience Version: 0.3.0 Summary: Retail Data
 Science Tools License: Elastic-2.0 Author: Murray Vanwyk Author-email:
 2493311+mvanwyk@users.noreply.github.com Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: click
 (>=8.1.7,<9.0.0) Requires-Dist: great-expectations (>=0.18.8,<0.19.0) Requires-
 Dist: loguru (>=0.7.2,<0.8.0) Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0) Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: pre-commit (>=3.6.2,<4.0.0) Requires-Dist: pyarrow
-(>=14.0.2,<15.0.0) Requires-Dist: seaborn (>=0.13.1,<0.14.0) Requires-Dist:
-strictyaml (>=1.7.3,<2.0.0) Requires-Dist: tqdm (>=4.66.1,<5.0.0) Description-
-Content-Type: text/markdown ![pyretailscience logo](https://
+(>=14.0.2,<15.0.0) Requires-Dist: scikit-learn (>=1.4.2,<2.0.0) Requires-Dist:
+scipy (>=1.13.0,<2.0.0) Requires-Dist: seaborn (>=0.13.1,<0.14.0) Requires-
+Dist: strictyaml (>=1.7.3,<2.0.0) Requires-Dist: tqdm (>=4.66.1,<5.0.0)
+Description-Content-Type: text/markdown ![pyretailscience logo](https://
 raw.githubusercontent.com/Data-Simply/pyretailscience/main/logo.png) #
 PyRetailScience â¡ Democratizing retail data analytics for all retailers â¡
 ## ð¤ What is PyRetailScience? pyretailscience is a Python package designed
 for performing analytics on retail data. Additionally, the package includes
 functionality for generating test data to facilitate testing and development.
 ## Installation To install pyretailscience, use the following pip command:
 ```bash pip install pyretailscience ``` ## Quick Start ### Generating Simulated
@@ -26,15 +27,15 @@
 argument. - `--verbose=
 False>`: Optional. Set to `True` to see debug messages. Default is `False`. -
 `--seed=`: Optional. Seed for the random number generator used in the
 simulation. If not provided, a random seed will be used. - `[output]`:
 Optional. The path where the generated transactions will be saved in parquet
 format. If not provided, the transactions will be saved in the current
 directory. #### Examples ```bash # Get the default transaction config file wget
-https://raw.githubusercontent.com/Data-Simply/pyretailscience/0.1.1/data/
+https://raw.githubusercontent.com/Data-Simply/pyretailscience/0.3.0/data/
 default_data_config.yaml # Generate the data file pyretailscience --
 config_file=default_data_config.yaml --seed=123 transactions.parquet ``` This
 command will generate a file named `transactions.parquet` with the simulated
 transaction data, using the configuration file at default data configuration
 file, and a seed of `123` for the random number generator. # Contributing We
 welcome contributions from the community to enhance and improve
 pyretailscience. To contribute, please follow these steps: 1. Fork the
```

