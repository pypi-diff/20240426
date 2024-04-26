# Comparing `tmp/veg2hab-0.1.0.tar.gz` & `tmp/veg2hab-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veg2hab-0.1.0.tar", max compression
+gzip compressed data, was "veg2hab-0.1.1.tar", max compression
```

## Comparing `veg2hab-0.1.0.tar` & `veg2hab-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0     1277 2024-04-16 15:19:38.457188 veg2hab-0.1.0/README.md
--rw-r--r--   0        0        0      760 2024-04-16 15:19:38.457188 veg2hab-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       72 2024-04-16 15:19:38.457188 veg2hab-0.1.0/veg2hab/__init__.py
--rw-r--r--   0        0        0     5403 2024-04-18 16:01:28.416523 veg2hab-0.1.0/veg2hab/acces_db.py
--rw-r--r--   0        0        0     6371 2024-04-16 15:25:00.491484 veg2hab-0.1.0/veg2hab/criteria.py
--rw-r--r--   0        0        0     7323 2024-04-16 15:25:00.491484 veg2hab-0.1.0/veg2hab/definitietabel.py
--rw-r--r--   0        0        0     5229 2024-04-19 09:31:14.436812 veg2hab-0.1.0/veg2hab/enums.py
--rw-r--r--   0        0        0      576 2024-04-16 15:25:00.491484 veg2hab-0.1.0/veg2hab/fgr.py
--rw-r--r--   0        0        0    10773 2024-04-16 15:25:00.491484 veg2hab-0.1.0/veg2hab/habitat.py
--rw-r--r--   0        0        0     4993 2024-04-19 09:38:18.833792 veg2hab-0.1.0/veg2hab/io/arcgis.py
--rw-r--r--   0        0        0      494 2024-04-16 15:19:38.457188 veg2hab-0.1.0/veg2hab/io/cli.py
--rw-r--r--   0        0        0     3894 2024-04-18 12:07:14.492852 veg2hab-0.1.0/veg2hab/io/common.py
--rw-r--r--   0        0        0     3201 2024-04-18 12:08:16.291133 veg2hab-0.1.0/veg2hab/main.py
--rw-r--r--   0        0        0    11181 2024-04-19 09:31:14.436812 veg2hab-0.1.0/veg2hab/mozaiek.py
--rw-r--r--   0        0        0 13900219 2024-04-16 15:19:38.507193 veg2hab-0.1.0/veg2hab/package_data/FGR.json
--rw-r--r--   0        0        0    39384 2024-04-18 12:26:25.547664 veg2hab-0.1.0/veg2hab/package_data/opgeschoonde_definitietabel.xlsx
--rw-r--r--   0        0        0    19151 2024-04-18 12:26:23.546338 veg2hab-0.1.0/veg2hab/package_data/opgeschoonde_waswordt.xlsx
--rw-r--r--   0        0        0     2774 2024-04-18 15:28:38.736658 veg2hab-0.1.0/veg2hab/package_data/toolbox.pyt
--rw-r--r--   0        0        0    12687 2024-04-03 14:54:35.748994 veg2hab-0.1.0/veg2hab/validation.py
--rw-r--r--   0        0        0    15069 2024-04-03 14:54:35.748994 veg2hab-0.1.0/veg2hab/vegetatietypen.py
--rw-r--r--   0        0        0    45253 2024-04-18 16:01:28.676829 veg2hab-0.1.0/veg2hab/vegkartering.py
--rw-r--r--   0        0        0     4585 2024-04-16 15:25:00.491484 veg2hab-0.1.0/veg2hab/waswordtlijst.py
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 veg2hab-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7626 2024-04-26 10:24:39.656747 veg2hab-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0     2993 2024-04-26 10:24:39.656747 veg2hab-0.1.1/README.md
+-rw-r--r--   0        0        0      855 2024-04-26 10:24:40.052746 veg2hab-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       72 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/__init__.py
+-rw-r--r--   0        0        0     1173 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/__main__.py
+-rw-r--r--   0        0        0     5396 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/access_db.py
+-rw-r--r--   0        0        0      411 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/constants.py
+-rw-r--r--   0        0        0     6384 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/criteria.py
+-rw-r--r--   0        0        0     7489 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/definitietabel.py
+-rw-r--r--   0        0        0     5202 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/enums.py
+-rw-r--r--   0        0        0      576 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/fgr.py
+-rw-r--r--   0        0        0    10773 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/habitat.py
+-rw-r--r--   0        0        0     5030 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/io/arcgis.py
+-rw-r--r--   0        0        0     2328 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/io/cli.py
+-rw-r--r--   0        0        0     4078 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/io/common.py
+-rw-r--r--   0        0        0     2941 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/main.py
+-rw-r--r--   0        0        0    11233 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/mozaiek.py
+-rw-r--r--   0        0        0 13900219 2024-04-26 10:24:40.104746 veg2hab-0.1.1/veg2hab/package_data/FGR.json
+-rw-r--r--   0        0        0      130 2024-04-26 10:24:40.804745 veg2hab-0.1.1/veg2hab/package_data/opgeschoonde_definitietabel.xlsx
+-rw-r--r--   0        0        0      130 2024-04-26 10:24:40.804745 veg2hab-0.1.1/veg2hab/package_data/opgeschoonde_waswordt.xlsx
+-rw-r--r--   0        0        0     3085 2024-04-26 10:24:40.804745 veg2hab-0.1.1/veg2hab/package_data/toolbox.pyt
+-rw-r--r--   0        0        0    13084 2024-04-26 10:24:40.804745 veg2hab-0.1.1/veg2hab/validation.py
+-rw-r--r--   0        0        0    15069 2024-04-26 10:24:40.804745 veg2hab-0.1.1/veg2hab/vegetatietypen.py
+-rw-r--r--   0        0        0    45254 2024-04-26 10:24:40.808745 veg2hab-0.1.1/veg2hab/vegkartering.py
+-rw-r--r--   0        0        0     4585 2024-04-26 10:24:40.808745 veg2hab-0.1.1/veg2hab/waswordtlijst.py
+-rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 veg2hab-0.1.1/PKG-INFO
```

### Comparing `veg2hab-0.1.0/pyproject.toml` & `veg2hab-0.1.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 [tool.poetry]
 name = "veg2hab"
-version = "0.1.0"
+version = "0.1.1"
 description = "Package voor automatisch omzetten van vegetatiekarteringen naar habitatkaarten"
 authors = ["Spheer.ai <info@spheer.ai>"]
 readme = "README.md"
 
+[tool.poetry.scripts]
+veg2hab = "veg2hab.__main__:main"
+
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 geopandas = ">=0.10.0"
 openpyxl = ">=3.0.0"
 xlrd = ">=2.0.1"
 pyodbc= ">=4.0.1"
 pydantic = ">=1.0,<2.0"
 setuptools = "<60.0.0"
 pygeos = "^0.14"
 typing-extensions = "4.7.1"
+click = "^8.1.7"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = ">=6.0.0"
 black = ">=23.0.0"
 isort = ">=5.0.0"
 pytest = ">=7.0.0"
+pyright = "^1.1.359"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.setuptools.package_data]
 veg2hab = ["veg2hab/package_data/*"]
```

### Comparing `veg2hab-0.1.0/veg2hab/acces_db.py` & `veg2hab-0.1.1/veg2hab/access_db.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 import warnings
 from pathlib import Path
 from typing import Any, Dict, Tuple, Union
 
 import pandas as pd
 import pyodbc
 
-# __all__ = ["read_access_tables"]
-
 
 class TableNames(enum.Enum):
     ELEMENT = "Element"
     KARTERINGVEGETATIETYPE = "KarteringVegetatietype"
     VEGETATIETYPE = "VegetatieType"
     SBBTYPE = "SbbType"
 
@@ -28,40 +26,40 @@
 
 def list_tables(conn: pyodbc.Connection):
     with conn.cursor() as cursor:
         return [i.table_name for i in cursor.tables(tableType="Table")]
 
 
 @functools.singledispatch
-def read_table(location, table_name: str, col_names: Dict[str, Any]) -> pd.DataFrame:
+def read_table(
+    location, table_name: TableNames, col_names: Dict[str, Any]
+) -> pd.DataFrame:
     """Read a table from the access_db"""
-    pass
+    raise NotImplementedError(f"invalide {location}")
 
 
 @read_table.register
 def _(
-    conn: pyodbc.Connection, table_name: str, col_names: Dict[str, Any]
+    conn: pyodbc.Connection, table_name: TableNames, col_names: Dict[str, Any]
 ) -> pd.DataFrame:
     # the pyodb is not officially suppported by pandas, so we suppress that
     # warning:
     with warnings.catch_warnings():
         warnings.simplefilter(action="ignore", category=UserWarning)
         return pd.read_sql(
-            f"SELECT {','.join(col_names.keys())} FROM {table_name}",
+            f"SELECT {','.join(col_names.keys())} FROM {table_name.value}",
             conn,
             dtype=col_names,
         )
 
 
 @read_table.register
-def _(folder: Path, table_name: str, col_names: Dict[str, Any]) -> pd.DataFrame:
-    # the pyodb is not officially suppported by pandas, so we suppress that
-    # warning:
+def _(folder: Path, table_name: TableNames, col_names: Dict[str, Any]) -> pd.DataFrame:
     return pd.read_csv(
-        folder / f"{table_name}.csv",
+        folder / f"{table_name.value}.csv",
         usecols=list(col_names.keys()),
         dtype=col_names,
     )
 
 
 def unpack_access_db(access_db_path: str, output_folder: Path):
     assert output_folder.is_dir()
@@ -111,39 +109,39 @@
     elif sys.platform.startswith("linux"):
         temp_dir = tempfile.TemporaryDirectory()
         locatie: Union[pyodbc.Connection, Path] = Path(temp_dir.name)
         unpack_access_db(acces_mdb, locatie)
 
     element = read_table(
         locatie,
-        "Element",
+        TableNames.ELEMENT,
         {"ElmID": int, "intern_id": int, "Locatietype": str},
     )
     # Uitfilteren van lijnen, selecteer alleen vlakken
     element["Locatietype"] = element["Locatietype"].str.lower()
     element = element[element.Locatietype == "v"][["ElmID", "intern_id"]]
 
     kart_veg = read_table(
         locatie,
-        "KarteringVegetatietype",
+        TableNames.KARTERINGVEGETATIETYPE,
         {"Locatie": int, "Vegetatietype": str, "Bedekking_num": int},
     )
     # BV voor GM2b -> Gm2b (elmid 10219 in ruitenaa2020)
     kart_veg.Vegetatietype = kart_veg.Vegetatietype.str.lower()
 
     vegetatietype = read_table(
         locatie,
-        "VegetatieType",
+        TableNames.VEGETATIETYPE,
         {"Code": str, "SbbType": int},
     )
     vegetatietype.Code = vegetatietype.Code.str.lower()
 
     sbbtype = read_table(
         locatie,
-        "SbbType",
+        TableNames.SBBTYPE,
         {"Cata_ID": int, "Code": str},
     )
     # Code hernoemen want er zit al een "Code" in Vegetatietype.csv
     sbbtype = sbbtype.rename(columns={"Code": "Sbb"})
 
     # SBB code toevoegen aan KarteringVegetatietype
     kart_veg = kart_veg.merge(
```

### Comparing `veg2hab-0.1.0/veg2hab/criteria.py` & `veg2hab-0.1.1/veg2hab/criteria.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 from functools import reduce
+from itertools import chain
 from operator import and_, or_
 from typing import ClassVar, List, Optional, Union
 
 import geopandas as gpd
 from pydantic import BaseModel, PrivateAttr
 
 from veg2hab.enums import FGRType, MaybeBoolean
@@ -186,15 +187,15 @@
 ) -> bool:
     """
     Geeft True als er in de lijst met voorstellen eentje met een criteria van crit_type is
     Nodig om te bepalen waarmee de gdf verrijkt moet worden (FGR etc)
     """
     # Als we een lijst van lijsten hebben, dan flattenen we die
     if any(isinstance(i, list) for i in voorstellen):
-        voorstellen = [item for sublist in voorstellen for item in sublist]
+        voorstellen = list(chain.from_iterable(voorstellen))
     return any(
         (
             voorstel.mits.is_criteria_type_present(criteria_type)
             if voorstel.mits is not None
             else False
         )
         for voorstel in voorstellen
```

### Comparing `veg2hab-0.1.0/veg2hab/definitietabel.py` & `veg2hab-0.1.1/veg2hab/definitietabel.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         self.df["Mozaiekregel"] = (
             self.df["mozaiekjson"]
             .loc[self.df["mozaiekjson"].notnull()]
             .apply(MozaiekRegel.parse_raw)
         )
         # Aanmaken dict keys die gebruikt gaan worden om de mozaiekregels te checken
         # TODO: Om deze isinstance heenwerken voor modulariteit
+        # TODO: Idealiter komt dit een een soort post_init (https://stackoverflow.com/questions/66571079/alter-field-after-instantiation-in-pydantic-basemodel-class)
         self.df["Mozaiekregel"].apply(
             lambda regel: regel.determine_keys()
             if isinstance(regel, StandaardMozaiekregel)
             else None
         )
 
     @classmethod
```

### Comparing `veg2hab-0.1.0/veg2hab/enums.py` & `veg2hab-0.1.1/veg2hab/enums.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,23 +23,33 @@
         else:
             return self
 
     def __bool__(self):
         raise RuntimeError("Cannot convert MaybeBoolean to bool")
 
     def __and__(self, other):
-        and_order = {MaybeBoolean.FALSE: 1, MaybeBoolean.POSTPONE: 2, MaybeBoolean.CANNOT_BE_AUTOMATED: 3, MaybeBoolean.TRUE: 4}
-        and_resolver = {1: MaybeBoolean.FALSE, 2: MaybeBoolean.POSTPONE, 3: MaybeBoolean.CANNOT_BE_AUTOMATED, 4: MaybeBoolean.TRUE}
+        and_order = {
+            MaybeBoolean.FALSE: 1,
+            MaybeBoolean.POSTPONE: 2,
+            MaybeBoolean.CANNOT_BE_AUTOMATED: 3,
+            MaybeBoolean.TRUE: 4,
+        }
+        and_resolver = {v: k for k, v in and_order.items()}
         if not isinstance(other, MaybeBoolean):
             return NotImplemented
         return and_resolver[min(and_order[self], and_order[other])]
 
     def __or__(self, other):
-        or_order = {MaybeBoolean.FALSE: 1, MaybeBoolean.CANNOT_BE_AUTOMATED: 2, MaybeBoolean.POSTPONE: 3, MaybeBoolean.TRUE: 4}
-        or_resolver = {1: MaybeBoolean.FALSE, 2: MaybeBoolean.CANNOT_BE_AUTOMATED, 3: MaybeBoolean.POSTPONE, 4: MaybeBoolean.TRUE}
+        or_order = {
+            MaybeBoolean.FALSE: 1,
+            MaybeBoolean.CANNOT_BE_AUTOMATED: 2,
+            MaybeBoolean.POSTPONE: 3,
+            MaybeBoolean.TRUE: 4,
+        }
+        or_resolver = {v: k for k, v in or_order.items()}
         if not isinstance(other, MaybeBoolean):
             return NotImplemented
         return or_resolver[max(or_order[self], or_order[other])]
 
 
 class Kwaliteit(Enum):
     NVT = "Nvt"  # bijvoorbeeld in het geval van H000
```

### Comparing `veg2hab-0.1.0/veg2hab/fgr.py` & `veg2hab-0.1.1/veg2hab/fgr.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.1.0/veg2hab/habitat.py` & `veg2hab-0.1.1/veg2hab/habitat.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.1.0/veg2hab/io/arcgis.py` & `veg2hab-0.1.1/veg2hab/io/arcgis.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             aprx.activeMap.addLayer(layer)
         except Exception as e:
             logging.warning(
                 f"Kon de output niet toevoegen aan de kaart. Lees deze handmatig in vanaf {filename}"
             )
             logging.error(str(e))
 
-    def instantiate_loggers(self) -> None:
+    def instantiate_loggers(self, log_level: int = logging.INFO) -> None:
         """Instantiate the loggers for the module."""
 
         class ArcpyAddMessageHandler(logging.Handler):
             def emit(self, record: logging.LogRecord):
                 import arcpy
 
                 msg = self.format(record)
@@ -78,15 +78,15 @@
                 else:
                     # this will map debug into info, but that's just
                     # the way it is now..
                     arcpy.AddMessage(msg)
 
         logging.basicConfig(
             format="%(asctime)s - %(levelname)s - %(message)s",
-            level=logging.INFO,
+            level=log_level,
             handlers=[ArcpyAddMessageHandler()],
         )
 
 
 def _schema_to_param_list(param_schema: dict) -> List["arcpy.Parameter"]:
     import arcpy
 
@@ -112,15 +112,15 @@
             direction="Input",
         )
 
         if field_name == "shapefile":
             shapefile_param = param
 
         if field_name == "access_mdb_path":
-            param.filter.list = ["mdb"]
+            param.filter.list = ["mdb", "accdb"]
 
         if "enum" in field_info.keys():
             param.filter.type = "ValueList"
             param.filter.list = field_info["enum"]
 
         outputs.append(param)
```

### Comparing `veg2hab-0.1.0/veg2hab/io/common.py` & `veg2hab-0.1.1/veg2hab/io/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,48 +9,52 @@
 
 class AccessDBInputs(BaseModel):
     label: ClassVar[str] = "digitale_standaard"
     description: ClassVar[str] = "Draai veg2hab o.b.v. de digitale standaard"
     shapefile: str = Field(
         description="Locatie van de vegetatiekartering",
     )
-    ElmID_col: str = Field(
+    elmid_col: str = Field(
         description="De kolomnaam van de ElementID in de Shapefile; deze wordt gematched aan de Element tabel in de AccessDB",
     )
     access_mdb_path: Path = Field(
         description="Locatie van de .mdb file van de digitale standaard",
     )
     opmerkingen_column: Optional[str] = Field(
-        default=None, description="kolomnaam van de opmerking als deze er is"
+        default=None,
+        description="Opmerking kolom (optioneel), deze wordt onveranderd aan de output meegegeven",
     )
     datum_column: Optional[str] = Field(
-        default=None, description="kolomnaam van de datum als deze er is"
+        default=None,
+        description="Datum kolom (optioneel), deze wordt onveranderd aan de output meegegeven",
     )
 
 
 class ShapefileInputs(BaseModel):
     label: ClassVar[str] = "vector_bestand"
     description: ClassVar[str] = "Draai veg2hab o.b.v. een vector bestand"
     shapefile: str = Field(
         description="Locatie van de vegetatiekartering",
     )
-    ElmID_col: str = Field(
+    elmid_col: str = Field(
         description="De kolomnaam van de ElementID in de Shapefile; uniek per vlak",
     )
     vegtype_col_format: Literal["single", "multi"] = Field(
         description='"single" als complexen in 1 kolom zitten of "multi" als er meerdere kolommen zijn',
     )
     sbb_of_vvn: Literal["VvN", "SBB", "beide"] = Field(
         description='"VvN" als VvN de voorname vertaling is vanuit het lokale type, "SBB" voor SBB en "beide" als beide er zijn.'
     )
     datum_col: Optional[str] = Field(
-        default=None, description="kolomnaam van de datum als deze er is"
+        default=None,
+        description="Datum kolom (optioneel), deze wordt onveranderd aan de output meegegeven",
     )
     opmerking_col: Optional[str] = Field(
-        default=None, description="kolomnaam van de opmerking als deze er is"
+        default=None,
+        description="Opmerking kolom (optioneel), deze wordt onveranderd aan de output meegegeven",
     )
     SBB_col: Optional[str] = Field(
         default=None,
         description="kolomnaam van de SBB vegetatietypen als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char)",
     )
     VvN_col: Optional[str] = Field(
         default=None,
@@ -74,15 +78,15 @@
     # make the constructor private
     def __new__(cls):
         raise TypeError(
             "Interface is a singleton class and cannot only be accessed through get_instance"
         )
 
     @classmethod
-    def get_instance(cls) -> Self:
+    def get_instance(cls):
         if Interface.__instance is None:
             Interface.__instance = object.__new__(cls)
         return Interface.__instance
 
     def shape_id_to_filename(self, shapefile_id: str) -> str:
         """Convert the shapefile id to a (temporary) file and returns the filename"""
         return shapefile_id
@@ -90,9 +94,9 @@
     @abstractmethod
     def output_shapefile(self, shapefile_id: str, gdf: gpd.GeoDataFrame) -> None:
         """Output the shapefile with the given id.
         ID would either be a path to a shapefile or an identifier to a shapefile in ArcGIS or QGIS.
         """
 
     @abstractmethod
-    def instantiate_loggers(self) -> None:
+    def instantiate_loggers(self, log_level: int) -> None:
         """Instantiate the loggers for the module."""
```

### Comparing `veg2hab-0.1.0/veg2hab/main.py` & `veg2hab-0.1.1/veg2hab/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,47 @@
 import logging
 from pathlib import Path
 from textwrap import dedent
 from typing import Union
 
 import geopandas as gpd
-from pkg_resources import resource_filename
 
+from veg2hab import constants
 from veg2hab.definitietabel import DefinitieTabel
 from veg2hab.fgr import FGR
 from veg2hab.io.common import AccessDBInputs, Interface, ShapefileInputs
 from veg2hab.vegkartering import Kartering
 from veg2hab.waswordtlijst import WasWordtLijst
 
 
 def installation_instructions():
-    data_file_path = resource_filename("veg2hab", "package_data/toolbox.pyt")
     print(
         dedent(
             f"""
     To install the veg2hab toolbox, go to add Python toolbox in ArcGIS Pro and select the file at the following location:
-        {data_file_path}
+        {constants.TOOLBOX_PYT_PATH}
 """
         )
     )
 
 
 def run(params: Union[AccessDBInputs, ShapefileInputs]):
     logging.info(f"Starting veg2hab met input parameters: {params.json()}")
 
-    wwl_filepath = resource_filename(
-        "veg2hab", "package_data/opgeschoonde_waswordt.xlsx"
-    )
-    wwl = WasWordtLijst.from_excel(wwl_filepath)
+    wwl = WasWordtLijst.from_excel(Path(constants.WWL_PATH))
 
-    logging.info(f"WasWordtLijst is ingelezen van {wwl_filepath}")
+    logging.info(f"WasWordtLijst is ingelezen van {constants.WWL_PATH}")
 
-    def_filepath = resource_filename(
-        "veg2hab", "package_data/opgeschoonde_definitietabel.xlsx"
-    )
-    deftabel = DefinitieTabel.from_excel(def_filepath)
+    deftabel = DefinitieTabel.from_excel(Path(constants.DEFTABEL_PATH))
 
-    logging.info(f"Definitietabel is ingelezen van {def_filepath}")
+    logging.info(f"Definitietabel is ingelezen van {constants.DEFTABEL_PATH}")
 
-    fgr = FGR(Path(resource_filename("veg2hab", "package_data/FGR.json")))
+    fgr = FGR(Path(constants.FGR_PATH))
 
-    logging.info(f"FGR is ingelezen")
+    logging.info(f"FGR is ingelezen van {constants.FGR_PATH}")
 
     filename = Interface.get_instance().shape_id_to_filename(params.shapefile)
 
     if filename != params.shapefile:
         logging.info(
             f"Tijdelijke versie van {params.shapefile} is opgeslagen in {filename}"
         )
```

### Comparing `veg2hab-0.1.0/veg2hab/mozaiek.py` & `veg2hab-0.1.1/veg2hab/mozaiek.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,17 @@
         )
     )
 
     if not mozaiek_present.any():
         return None
 
     # Eerst trekken we een lijn om alle shapes met mozaiekregels
-    buffered_boundary = gdf[mozaiek_present].buffer(buffer).boundary.to_frame(name="geometry")
+    buffered_boundary = (
+        gdf[mozaiek_present].buffer(buffer).boundary.to_frame(name="geometry")
+    )
     assert buffered_boundary.crs == gdf.crs
 
     # NOTE: Deze buffered_ prefix wordt ook in calc_mozaiek_percentages_from_overlay_gdf gebruikt
     buffered_boundary["buffered_ElmID"] = gdf["ElmID"]
     buffered_boundary["full_line_length"] = buffered_boundary.length
 
     # Dan leggen we alle lijnen over de originele gdf
@@ -254,18 +256,21 @@
         habtype_percentages = group["part_line_percentage"]
         # Als er geen habitatkeuzes zijn, dan geven we HXXXX terug
         # TODO: pak de grootste keuze als er meerdere zijn
         #       Wat als de grootste nog None is en de kleinere wel een keuze heeft?
         key_tuples = group.HabitatKeuze.apply(
             lambda keuzes:
             # Als len(keuzes) == 0, dan is er geen vegtype opgegeven, dus H0000
-            ("H0000", True, Kwaliteit.NVT) if len(keuzes) == 0 else
+            ("H0000", True, Kwaliteit.NVT)
+            if len(keuzes) == 0
+            else
             # Als de keuze None is, dan is deze nog niet bepaald, dus HXXXX
-            ("HXXXX", True, Kwaliteit.NVT) if keuzes[0] is None else
-            (
+            ("HXXXX", True, Kwaliteit.NVT)
+            if keuzes[0] is None
+            else (
                 keuzes[0].habtype,
                 keuzes[0].zelfstandig,
                 keuzes[0].kwaliteit,
             )
         )
         habtype_percentage_dict = defaultdict(int)
         for key, percentage in zip(key_tuples, habtype_percentages):
```

### Comparing `veg2hab-0.1.0/veg2hab/package_data/FGR.json` & `veg2hab-0.1.1/veg2hab/package_data/FGR.json`

 * *Files identical despite different names*

### Comparing `veg2hab-0.1.0/veg2hab/validation.py` & `veg2hab-0.1.1/veg2hab/validation.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,18 +85,29 @@
         warnings.warn(
             f"Percentages do not add up to 100% for row: {row.name}, result: {ret_values}"
         )
 
     return ret_values
 
 
+def clean_up_habtypen(gdf: gpd.GeoDataFrame, habtype_cols: List[str]):
+    """
+    Schoont habitattypecodes op
+
+    Haalt _ weg zodat H2130_B en H2130B als dezelfde worden gezien
+    """
+    for col in habtype_cols:
+        gdf[col] = gdf[col].str.replace("_", "")
+    return gdf
+
+
 def parse_habitat_percentages(
     gdf: gpd.GeoDataFrame,
-    habtype_cols: str = "Habtype",
-    percentage_cols: Optional[str] = "Perc",
+    habtype_cols_regex: str = "Habtype\d+",
+    percentage_cols_regex: Optional[str] = "Perc\d+",
     how_to_handle_missing_percentages: Literal[
         None, "split_equally", "select_first"
     ] = None,
 ) -> gpd.GeoDataFrame:
     """
     Args:
         gdf: A GeoDataFrame containing habitat types and their percentages
@@ -108,36 +119,40 @@
         habtype_cols: De string waarmee de habitattypekolommen moeten beginnen, bijvoorbeeld Habtype voor Habtype1, Habtype2, Habtype3
         percentage_cols: De string waarmee de percentagekolommen moeten beginnen
         how_to_handle_missing_percentages: Hoe om te gaan met ontbrekende percentages.
                                            Bij None zal de functie een foutmelding geven als er ontbrekende percentages zijn.
                                            Bij "split_equally" zal de ieder habitattype een gelijk percentage krijgen (100/n_habtypes).
                                            Bij "select_first" zal enkel het eerste habitattype gebruikt worden; deze krijgt dan ook 100%.
     """
-    if (percentage_cols is not None) == (
+    if (percentage_cols_regex is not None) == (
         how_to_handle_missing_percentages is not None
     ):  # xor
         raise ValueError(
             "You should specify exactly one of percentage_cols or how_to_handle_missing_percentages, not both"
         )
 
-    habtype_cols = [c for c in gdf.columns if re.fullmatch(f"{habtype_cols}\d+", c)]
+    habtype_cols = [c for c in gdf.columns if re.fullmatch(habtype_cols_regex, c)]
     if len(habtype_cols) == 0:
         raise ValueError(
             f"Expected nonzero of habitat and percentage columns, but found {len(habtype_cols)} hab columns"
         )
-    if percentage_cols is not None:
+    if percentage_cols_regex is not None:
         percentage_cols = [
-            c for c in gdf.columns if re.fullmatch(f"{percentage_cols}\d+", c)
+            c for c in gdf.columns if re.fullmatch(percentage_cols_regex, c)
         ]
         gdf[percentage_cols] = gdf[percentage_cols].apply(pd.to_numeric, errors="raise")
 
         if len(habtype_cols) != len(percentage_cols):
             raise ValueError(
                 f"Expected same number of habitat and percentage columns, but found {len(habtype_cols)} hab columns and {len(percentage_cols)} percentage columns"
             )
+    else:
+        percentage_cols = None
+
+    gdf = clean_up_habtypen(gdf, habtype_cols)
 
     return gpd.GeoDataFrame(
         data={
             "hab_perc": gdf.apply(
                 lambda row: _convert_row_to_dict(
                     row,
                     habtype_cols,
```

### Comparing `veg2hab-0.1.0/veg2hab/vegetatietypen.py` & `veg2hab-0.1.1/veg2hab/vegetatietypen.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.1.0/veg2hab/vegkartering.py` & `veg2hab-0.1.1/veg2hab/vegkartering.py`

 * *Files identical despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 from typing import List, Optional, Union
 
 import geopandas as gpd
 import pandas as pd
 from typing_extensions import Literal, Self
 
-from veg2hab.acces_db import read_access_tables
+from veg2hab.access_db import read_access_tables
 from veg2hab.criteria import FGRCriterium, is_criteria_type_present
 from veg2hab.enums import KeuzeStatus, Kwaliteit
 from veg2hab.fgr import FGR
 from veg2hab.habitat import (
     HabitatVoorstel,
     rank_habitatkeuzes,
     try_to_determine_habkeuze,
```

### Comparing `veg2hab-0.1.0/veg2hab/waswordtlijst.py` & `veg2hab-0.1.1/veg2hab/waswordtlijst.py`

 * *Files identical despite different names*

