# Comparing `tmp/met_annot_unifier-0.0.3.tar.gz` & `tmp/met_annot_unifier-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "met_annot_unifier-0.0.3.tar", max compression
+gzip compressed data, was "met_annot_unifier-0.0.4.tar", max compression
```

## Comparing `met_annot_unifier-0.0.3.tar` & `met_annot_unifier-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1077 2024-04-21 15:20:14.964575 met_annot_unifier-0.0.3/LICENSE
--rw-r--r--   0        0        0     4691 2024-04-21 15:20:14.964575 met_annot_unifier-0.0.3/README.md
--rw-r--r--   0        0        0        0 2024-04-21 15:20:14.992575 met_annot_unifier-0.0.3/met_annot_unifier/__init__.py
--rw-r--r--   0        0        0        0 2024-04-21 15:20:14.992575 met_annot_unifier-0.0.3/met_annot_unifier/aligner/__init__.py
--rw-r--r--   0        0        0     6607 2024-04-21 15:20:14.992575 met_annot_unifier-0.0.3/met_annot_unifier/aligner/aligner.py
--rw-r--r--   0        0        0     8077 2024-04-21 15:20:14.992575 met_annot_unifier-0.0.3/met_annot_unifier/aligner/parser.py
--rw-r--r--   0        0        0     2644 2024-04-21 15:20:14.992575 met_annot_unifier-0.0.3/met_annot_unifier/aligner/utils.py
--rw-r--r--   0        0        0     4593 2024-04-21 15:20:14.992575 met_annot_unifier-0.0.3/met_annot_unifier/cli.py
--rw-r--r--   0        0        0    10938 2024-04-21 15:20:14.992575 met_annot_unifier-0.0.3/met_annot_unifier/config/column_config.json
--rw-r--r--   0        0        0      694 2024-04-21 15:20:14.992575 met_annot_unifier-0.0.3/met_annot_unifier/exceptions.py
--rw-r--r--   0        0        0      267 2024-04-21 15:20:14.992575 met_annot_unifier-0.0.3/met_annot_unifier/foo.py
--rw-r--r--   0        0        0     2409 2024-04-21 15:20:34.028720 met_annot_unifier-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5538 1970-01-01 00:00:00.000000 met_annot_unifier-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-26 13:45:30.393365 met_annot_unifier-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4691 2024-04-26 13:45:30.393365 met_annot_unifier-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-26 13:45:30.421365 met_annot_unifier-0.0.4/met_annot_unifier/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:45:30.421365 met_annot_unifier-0.0.4/met_annot_unifier/aligner/__init__.py
+-rw-r--r--   0        0        0     7539 2024-04-26 13:45:30.421365 met_annot_unifier-0.0.4/met_annot_unifier/aligner/aligner.py
+-rw-r--r--   0        0        0     9393 2024-04-26 13:45:30.425366 met_annot_unifier-0.0.4/met_annot_unifier/aligner/parser.py
+-rw-r--r--   0        0        0     2644 2024-04-26 13:45:30.425366 met_annot_unifier-0.0.4/met_annot_unifier/aligner/utils.py
+-rw-r--r--   0        0        0     4947 2024-04-26 13:45:30.425366 met_annot_unifier-0.0.4/met_annot_unifier/cli.py
+-rw-r--r--   0        0        0    10938 2024-04-26 13:45:30.425366 met_annot_unifier-0.0.4/met_annot_unifier/config/column_config.json
+-rw-r--r--   0        0        0      694 2024-04-26 13:45:30.425366 met_annot_unifier-0.0.4/met_annot_unifier/exceptions.py
+-rw-r--r--   0        0        0      267 2024-04-26 13:45:30.425366 met_annot_unifier-0.0.4/met_annot_unifier/foo.py
+-rw-r--r--   0        0        0     2409 2024-04-26 13:45:48.893399 met_annot_unifier-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5538 1970-01-01 00:00:00.000000 met_annot_unifier-0.0.4/PKG-INFO
```

### Comparing `met_annot_unifier-0.0.3/LICENSE` & `met_annot_unifier-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `met_annot_unifier-0.0.3/README.md` & `met_annot_unifier-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `met_annot_unifier-0.0.3/met_annot_unifier/aligner/aligner.py` & `met_annot_unifier-0.0.4/met_annot_unifier/aligner/aligner.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,17 +10,23 @@
     process_isdb_data,
     process_sirius_data,
     standardize_column_names,
 )
 from met_annot_unifier.aligner.utils import count_sources, determine_source
 from met_annot_unifier.exceptions import DataFileError
 
+gnps_file = "examples/data/in/gnps_output_example.tsv"
+sirius_file = "examples/data/in/sirius_output_example.tsv"
+isdb_file = "examples/data/in/isdb_output_example.tsv"
+
 
 def align_data_vertically(
-    gnps_file: Optional[str] = None, sirius_file: Optional[str] = None, isdb_file: Optional[str] = None
+    gnps_file: Optional[str] = None,
+    isdb_file: Optional[str] = None,
+    sirius_file: Optional[str] = None,
 ) -> pd.DataFrame:
     """
     Aligns and merges data from GNPS, Sirius, and ISDB datasets optionally. Files can be provided for any subset of these datasets.
     The function standardizes column names, prefixes them to indicate their source, merges the data based on 'feature_id'
     and 'IK2D', and then creates consolidated 'Sources' and 'SMILES' columns.
 
     Args:
@@ -41,101 +47,119 @@
 
     data_frames = []
 
     if gnps_file:
         gnps_data = process_gnps_data(gnps_file)
         data_frames.append(gnps_data)
 
-    if sirius_file:
-        sirius_data = process_sirius_data(sirius_file)
-        data_frames.append(sirius_data)
-
     if isdb_file:
         isdb_data = process_isdb_data(isdb_file)
         data_frames.append(isdb_data)
 
+    if sirius_file:
+        sirius_data = process_sirius_data(sirius_file)
+        data_frames.append(sirius_data)
+
     # Ensure that at least one data frame has been loaded
     if not data_frames:
         raise DataFileError()
 
     # Concatenate all available data frames
-    combined_data = pd.concat(data_frames, axis=0, ignore_index=True)
+    combined_data = pd.concat([df for df in data_frames if not df.empty], axis=0, ignore_index=True)
     # Group by 'feature_id' and 'IK2D' and combine the annotations
     merged_data = combined_data.groupby(["feature_id", "IK2D"], as_index=False).agg(
         lambda x: ", ".join(x.dropna().astype(str).unique())
     )
 
     # Create the 'Sources' column
     source_columns = [col for col in merged_data.columns if col.endswith("annotation_source")]
     merged_data["Sources"] = merged_data.apply(
         lambda row: "|".join(sorted(filter(None, [row.get(col) for col in source_columns]))), axis=1
     )
     merged_data.drop(columns=source_columns, inplace=True)
 
     # Handle the SMILES column
-    smiles_columns = [col for col in merged_data.columns if "SMILES" in col]
+    # Specify the priority order for SMILES columns explicitly
+    smiles_columns = [
+        "sirius_SMILES",  # Highest priority
+        "isdb_SMILES",
+        "gnps_SMILES",  # Lowest priority
+    ]
+
+    # Check and keep only those columns that actually exist in the merged data
+    smiles_columns = [col for col in smiles_columns if col in merged_data.columns]
     merged_data["SMILES"] = merged_data.apply(
         lambda row: next((row[col] for col in smiles_columns if row[col]), None), axis=1
     )
 
     # Select and reorder columns
     selected_columns = ["feature_id", "IK2D", "Sources", "SMILES"]
     merged_data = merged_data[selected_columns + [col for col in merged_data.columns if col not in selected_columns]]
 
     return merged_data
 
 
 def align_data_horizontally(
-    gnps_file: Optional[str] = None, sirius_file: Optional[str] = None, isdb_file: Optional[str] = None
+    canopus_file: Optional[str] = None,
+    gnps_file: Optional[str] = None,
+    isdb_file: Optional[str] = None,
+    sirius_file: Optional[str] = None,
 ) -> pd.DataFrame:
     """
-    Aligns and merges data from GNPS, Sirius, and ISDB datasets, if provided. This function merges the data horizontally,
+    Aligns and merges data from GNPS, Sirius, ISDB  and CANOPUS datasets, if provided. This function merges the data horizontally,
     keeping the data in a wide format. The function standardizes column names, prefixes them to indicate their source,
     and merges the data based on 'feature_id'.
 
     Args:
+    canopus_file (Optional[str]): File path for the CANOPUS data in TSV format.
     gnps_file (Optional[str]): File path for the GNPS data in TSV format.
-    sirius_file (Optional[str]): File path for the Sirius data in TSV format.
     isdb_file (Optional[str]): File path for the ISDB data in TSV format.
+    sirius_file (Optional[str]): File path for the Sirius data in TSV format.
 
     Returns:
     pd.DataFrame: A DataFrame with aligned and merged data from the provided sources.
     """
 
     data_frames = []
 
+    if canopus_file:
+        canopus_data = pd.read_csv(canopus_file, sep="\t")
+        canopus_data = standardize_column_names(canopus_data, "feature_id", "feature_id")
+        canopus_data = prefix_columns(canopus_data, "canopus_", exclude_columns=[])
+        data_frames.append(canopus_data)
+
     if gnps_file:
         gnps_data = pd.read_csv(gnps_file, sep="\t")
         gnps_data = standardize_column_names(gnps_data, "InChIKey-Planar", "IK2D")
         gnps_data = standardize_column_names(gnps_data, "#Scan#", "feature_id")
         gnps_data = standardize_column_names(gnps_data, "Smiles", "SMILES")
         gnps_data = prefix_columns(gnps_data, "gnps_", exclude_columns=[])
         gnps_data = standardize_column_names(gnps_data, "gnps_feature_id", "feature_id")
         data_frames.append(gnps_data)
 
+    if isdb_file:
+        isdb_data = pd.read_csv(isdb_file, sep="\t")
+        isdb_data = standardize_column_names(isdb_data, "short_inchikey", "IK2D")
+        isdb_data = standardize_column_names(isdb_data, "feature_id", "feature_id")
+        isdb_data = standardize_column_names(isdb_data, "structure_smiles", "SMILES")
+        isdb_data = prefix_columns(isdb_data, "isdb_", exclude_columns=[])
+        isdb_data = standardize_column_names(isdb_data, "isdb_feature_id", "feature_id")
+        data_frames.append(isdb_data)
+
     if sirius_file:
         # Read and process Sirius data
         sirius_data = pd.read_csv(sirius_file, sep="\t")
         sirius_data = standardize_column_names(sirius_data, "InChIkey2D", "IK2D")
         sirius_data = standardize_column_names(sirius_data, "id", "feature_id")
         sirius_data = standardize_column_names(sirius_data, "smiles", "SMILES")
         sirius_data = prefix_columns(sirius_data, "sirius_", exclude_columns=[])
         sirius_data = extract_feature_id(sirius_data, "sirius_feature_id")
         sirius_data = standardize_column_names(sirius_data, "sirius_feature_id", "feature_id")
         data_frames.append(sirius_data)
 
-    if isdb_file:
-        isdb_data = pd.read_csv(isdb_file, sep="\t")
-        isdb_data = standardize_column_names(isdb_data, "short_inchikey", "IK2D")
-        isdb_data = standardize_column_names(isdb_data, "feature_id", "feature_id")
-        isdb_data = standardize_column_names(isdb_data, "structure_smiles", "SMILES")
-        isdb_data = prefix_columns(isdb_data, "isdb_", exclude_columns=[])
-        isdb_data = standardize_column_names(isdb_data, "isdb_feature_id", "feature_id")
-        data_frames.append(isdb_data)
-
     if not data_frames:
         raise DataFileError()
 
     # Merge the dataframes horizontally on 'feature_id'
     merged_data = reduce(lambda left, right: pd.merge(left, right, on="feature_id", how="outer"), data_frames)
 
     # Create the 'Sources' column. Fill it according the content of the tool_IK2D columns.
```

### Comparing `met_annot_unifier-0.0.3/met_annot_unifier/aligner/parser.py` & `met_annot_unifier-0.0.4/met_annot_unifier/aligner/parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,23 +6,30 @@
 def parse_gnps(file_path: str) -> pd.DataFrame:
     # Read the GNPS output file
     data = pd.read_csv(file_path, sep="\t")
     # Extract necessary columns and any other processing
     return data
 
 
+def parse_isdb(file_path: str) -> pd.DataFrame:
+    # Read the ISDB output file
+    data = pd.read_csv(file_path, sep="\t")
+    # Extract necessary columns and any other processing
+    return data
+
+
 def parse_sirius(file_path: str) -> pd.DataFrame:
     # Read the Sirius output file
     data = pd.read_csv(file_path, sep="\t")
     # Extract necessary columns and any other processing
     return data
 
 
-def parse_isdb(file_path: str) -> pd.DataFrame:
-    # Read the ISDB output file
+def parse_canopus(file_path: str) -> pd.DataFrame:
+    # Read the Canopus output file
     data = pd.read_csv(file_path, sep="\t")
     # Extract necessary columns and any other processing
     return data
 
 
 def standardize_column_names(df: pd.DataFrame, original_column_name: str, final_column_name: str) -> pd.DataFrame:
     """
@@ -148,14 +155,45 @@
     gnps_data = prefix_columns(gnps_data, "gnps_", exclude_columns=[])
     gnps_data = standardize_column_names(gnps_data, "gnps_IK2D", "IK2D")
     gnps_data = standardize_column_names(gnps_data, "gnps_feature_id", "feature_id")
 
     return gnps_data
 
 
+def process_isdb_data(isdb_file: str) -> pd.DataFrame:
+    """
+    Reads and processes ISDB data. This function standardizes column names, prefixes them to indicate their source,
+    and extracts 'feature_id' and 'IK2D' from the data.
+
+    Args:
+    isdb_file (str): File path for the ISDB data in TSV format.
+
+    Returns:
+    pandas.DataFrame: A DataFrame with processed ISDB data.
+
+    Example:
+    >>> isdb_file = 'path/to/isdb_data.tsv'
+    >>> isdb_data = process_isdb_data(isdb_file)
+    >>> print(isdb_data.columns)
+    Index(['feature_id', 'IK2D', ...], dtype='object')
+    """
+
+    # Read and process ISDB data
+    isdb_data = pd.read_csv(isdb_file, sep="\t")
+    isdb_data = add_source_column(isdb_data, "isdb")
+    isdb_data = standardize_column_names(isdb_data, "short_inchikey", "IK2D")
+    isdb_data = standardize_column_names(isdb_data, "feature_id", "feature_id")
+    isdb_data = standardize_column_names(isdb_data, "structure_smiles", "SMILES")
+    isdb_data = prefix_columns(isdb_data, "isdb_", exclude_columns=[])
+    isdb_data = standardize_column_names(isdb_data, "isdb_IK2D", "IK2D")
+    isdb_data = standardize_column_names(isdb_data, "isdb_feature_id", "feature_id")
+
+    return isdb_data
+
+
 def process_sirius_data(sirius_file: str) -> pd.DataFrame:
     """
     Reads and processes Sirius data. This function standardizes column names, prefixes them to indicate their source,
     and extracts 'feature_id' and 'IK2D' from the data.
 
     Args:
     sirius_file (str): File path for the Sirius data in TSV format.
@@ -180,36 +218,34 @@
     sirius_data = extract_feature_id(sirius_data, "sirius_feature_id")
     sirius_data = standardize_column_names(sirius_data, "sirius_IK2D", "IK2D")
     sirius_data = standardize_column_names(sirius_data, "sirius_feature_id", "feature_id")
 
     return sirius_data
 
 
-def process_isdb_data(isdb_file: str) -> pd.DataFrame:
+def process_canopus_data(canopus_file: str) -> pd.DataFrame:
     """
-    Reads and processes ISDB data. This function standardizes column names, prefixes them to indicate their source,
-    and extracts 'feature_id' and 'IK2D' from the data.
+    Reads and processes Canopus data. This function standardizes column names, prefixes them to indicate their source,
+    and extracts 'feature_id' from the data.
 
     Args:
-    isdb_file (str): File path for the ISDB data in TSV format.
+    canopus_file (str): File path for the Canopus data in TSV format.
 
     Returns:
-    pandas.DataFrame: A DataFrame with processed ISDB data.
+    pandas.DataFrame: A DataFrame with processed Canopus data.
 
     Example:
-    >>> isdb_file = 'path/to/isdb_data.tsv'
-    >>> isdb_data = process_isdb_data(isdb_file)
-    >>> print(isdb_data.columns)
-    Index(['feature_id', 'IK2D', ...], dtype='object')
+    >>> canopus_file = 'path/to/canopus_data.tsv'
+    >>> canopus_data = process_canopus_data(canopus_file)
+    >>> print(canopus_data.columns)
+    Index(['feature_id', ...], dtype='object')
     """
 
-    # Read and process ISDB data
-    isdb_data = pd.read_csv(isdb_file, sep="\t")
-    isdb_data = add_source_column(isdb_data, "isdb")
-    isdb_data = standardize_column_names(isdb_data, "short_inchikey", "IK2D")
-    isdb_data = standardize_column_names(isdb_data, "feature_id", "feature_id")
-    isdb_data = standardize_column_names(isdb_data, "structure_smiles", "SMILES")
-    isdb_data = prefix_columns(isdb_data, "isdb_", exclude_columns=[])
-    isdb_data = standardize_column_names(isdb_data, "isdb_IK2D", "IK2D")
-    isdb_data = standardize_column_names(isdb_data, "isdb_feature_id", "feature_id")
+    # Read and process Canopus data
+    canopus_data = pd.read_csv(canopus_file, sep="\t")
+    canopus_data = add_source_column(canopus_data, "canopus")
+    canopus_data = standardize_column_names(canopus_data, "id", "feature_id")
+    canopus_data = prefix_columns(canopus_data, "canopus_", exclude_columns=[])
+    canopus_data = extract_feature_id(canopus_data, "canopus_feature_id")
+    canopus_data = standardize_column_names(canopus_data, "canopus_feature_id", "feature_id")
 
-    return isdb_data
+    return canopus_data
```

### Comparing `met_annot_unifier-0.0.3/met_annot_unifier/aligner/utils.py` & `met_annot_unifier-0.0.4/met_annot_unifier/aligner/utils.py`

 * *Files identical despite different names*

### Comparing `met_annot_unifier-0.0.3/met_annot_unifier/cli.py` & `met_annot_unifier-0.0.4/met_annot_unifier/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,24 +12,24 @@
     """Description for your CLI tool."""
     print("CLI is running")
     pass
 
 
 @cli.command()
 @click.option("--gnps-file", type=click.Path(exists=True), help="Path to GNPS output file.")
-@click.option("--sirius-file", type=click.Path(exists=True), help="Path to Sirius output file.")
 @click.option("--isdb-file", type=click.Path(exists=True), help="Path to ISDB output file.")
+@click.option("--sirius-file", type=click.Path(exists=True), help="Path to Sirius output file.")
 @click.option("--output", "-o", type=click.Path(), help="Output file to save the merged data.")
 def align_vertically(gnps_file: str, sirius_file: str, isdb_file: str, output: Optional[str] = None) -> None:
     """CLI tool to align and merge data from GNPS, Sirius, and ISDB.
 
     Args:
         gnps_file (str): Path to GNPS output file.
-        sirius_file (str): Path to Sirius output file.
         isdb_file (str): Path to ISDB output file.
+        sirius_file (str): Path to Sirius output file.
         output (str, optional): Output file to save the merged data. Defaults to None.
 
     Returns:
         A dataframe with the aligned data (if the output option is used, the dataframe is saved to a file)
     """
     aligned_data = align_data_vertically(gnps_file, sirius_file, isdb_file)
 
@@ -37,31 +37,41 @@
         aligned_data.to_csv(output, index=False, sep="\t")
         click.echo(f"Aligned data saved to {output}")
     else:
         click.echo(aligned_data)
 
 
 @cli.command()
-@click.option("--gnps-file", type=click.Path(exists=True), help="Path to GNPS output file.")
-@click.option("--sirius-file", type=click.Path(exists=True), help="Path to Sirius output file.")
-@click.option("--isdb-file", type=click.Path(exists=True), help="Path to ISDB output file.")
+@click.option("--canopus-file", type=click.Path(), default=None, help="Path to CANOPUS output file.")
+@click.option("--gnps-file", type=click.Path(), default=None, help="Path to GNPS output file.")
+@click.option("--isdb-file", type=click.Path(), default=None, help="Path to ISDB output file.")
+@click.option("--sirius-file", type=click.Path(), default=None, help="Path to Sirius output file.")
 @click.option("--output", "-o", type=click.Path(), help="Output file to save the merged data.")
-def align_horizontally(gnps_file: str, sirius_file: str, isdb_file: str, output: Optional[str] = None) -> None:
-    """CLI tool to align and merge data from GNPS, Sirius, and ISDB horizontally.
+def align_horizontally(
+    canopus_file: Optional[str],
+    gnps_file: Optional[str],
+    isdb_file: Optional[str],
+    sirius_file: Optional[str],
+    output: Optional[str] = None,
+) -> None:
+    """CLI tool to align and merge data from CANOPUS, GNPS, Sirius, and ISDB horizontally.
 
     Args:
-        gnps_file (str): Path to GNPS output file.
-        sirius_file (str): Path to Sirius output file.
-        isdb_file (str): Path to ISDB output file.
-        output (str, optional): Output file to save the merged data. Defaults to None.
+        canopus_file (Optional[str]): Path to CANOPUS output file.
+        gnps_file (Optional[str]): Path to GNPS output file.
+        sirius_file (Optional[str]): Path to Sirius output file.
+        isdb_file (Optional[str]): Path to ISDB output file.
+        output (Optional[str]): Output file to save the merged data.
 
     Returns:
         A dataframe with the aligned data (if the output option is used, the dataframe is saved to a file)
     """
-    aligned_data = align_data_horizontally(gnps_file, sirius_file, isdb_file)
+    aligned_data = align_data_horizontally(
+        canopus_file=canopus_file, gnps_file=gnps_file, isdb_file=isdb_file, sirius_file=sirius_file
+    )
 
     if output:
         aligned_data.to_csv(output, index=False, sep="\t")
         click.echo(f"Aligned data saved to {output}")
     else:
         click.echo(aligned_data)
```

### Comparing `met_annot_unifier-0.0.3/met_annot_unifier/config/column_config.json` & `met_annot_unifier-0.0.4/met_annot_unifier/config/column_config.json`

 * *Files identical despite different names*

### Comparing `met_annot_unifier-0.0.3/met_annot_unifier/exceptions.py` & `met_annot_unifier-0.0.4/met_annot_unifier/exceptions.py`

 * *Files identical despite different names*

### Comparing `met_annot_unifier-0.0.3/pyproject.toml` & `met_annot_unifier-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "met-annot-unifier"
-version = "0.0.3"
+version = "0.0.4"
 description = "A Python project to combine tabular outputs from GNPS, Sirius and ISDB"
 authors = ["Pierre-Marie Allard <pierre-marie.allard@unifr.ch>"]
 repository = "https://github.com/mapp-metabolomics-unit/met-annot-unifier"
 documentation = "https://mapp-metabolomics-unit.github.io/met-annot-unifier/"
 readme = "README.md"
 packages = [
   {include = "met_annot_unifier"}
```

### Comparing `met_annot_unifier-0.0.3/PKG-INFO` & `met_annot_unifier-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: met-annot-unifier
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python project to combine tabular outputs from GNPS, Sirius and ISDB
 Home-page: https://github.com/mapp-metabolomics-unit/met-annot-unifier
 Author: Pierre-Marie Allard
 Author-email: pierre-marie.allard@unifr.ch
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

