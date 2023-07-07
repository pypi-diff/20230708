# Comparing `tmp/gdptools_pygeoapi_plugin-0.0.7.dev0.tar.gz` & `tmp/gdptools_pygeoapi_plugin-0.0.8.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdptools_pygeoapi_plugin-0.0.7.dev0.tar", max compression
+gzip compressed data, was "gdptools_pygeoapi_plugin-0.0.8.dev0.tar", max compression
```

## Comparing `gdptools_pygeoapi_plugin-0.0.7.dev0.tar` & `gdptools_pygeoapi_plugin-0.0.8.dev0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1640 2022-09-08 23:56:38.751663 gdptools_pygeoapi_plugin-0.0.7.dev0/LICENSE.md
--rw-r--r--   0        0        0     2556 2022-09-08 23:56:38.701663 gdptools_pygeoapi_plugin-0.0.7.dev0/README.md
--rw-r--r--   0        0        0     2832 2023-05-18 15:39:42.124008 gdptools_pygeoapi_plugin-0.0.7.dev0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-08 15:57:52.951663 gdptools_pygeoapi_plugin-0.0.7.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/__init__.py
--rw-r--r--   0        0        0     9014 2023-03-16 15:57:07.478580 gdptools_pygeoapi_plugin-0.0.7.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/calc_weights_catalog.py
--rw-r--r--   0        0        0     2106 2023-05-18 15:03:49.530427 gdptools_pygeoapi_plugin-0.0.7.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/proc_test.py
--rw-r--r--   0        0        0     9261 2023-03-16 15:55:31.368763 gdptools_pygeoapi_plugin-0.0.7.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/run_weights_catalog.py
--rw-r--r--   0        0        0     3528 1970-01-01 00:00:00.000000 gdptools_pygeoapi_plugin-0.0.7.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1640 2022-09-08 23:56:38.751663 gdptools_pygeoapi_plugin-0.0.8.dev0/LICENSE.md
+-rw-r--r--   0        0        0     2556 2022-09-08 23:56:38.701663 gdptools_pygeoapi_plugin-0.0.8.dev0/README.md
+-rw-r--r--   0        0        0     2844 2023-07-07 22:07:39.410664 gdptools_pygeoapi_plugin-0.0.8.dev0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-08 15:57:52.951663 gdptools_pygeoapi_plugin-0.0.8.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/__init__.py
+-rw-r--r--   0        0        0     8723 2023-07-07 22:07:19.800540 gdptools_pygeoapi_plugin-0.0.8.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/calc_agg_catalog.py
+-rw-r--r--   0        0        0     7824 2023-07-07 22:07:19.800540 gdptools_pygeoapi_plugin-0.0.8.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/calc_weights_catalog.py
+-rw-r--r--   0        0        0     2106 2023-06-08 23:26:18.630490 gdptools_pygeoapi_plugin-0.0.8.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/proc_test.py
+-rw-r--r--   0        0        0     2117 2023-06-08 23:27:44.240746 gdptools_pygeoapi_plugin-0.0.8.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/proc_test_async.py
+-rw-r--r--   0        0        0     3464 1970-01-01 00:00:00.000000 gdptools_pygeoapi_plugin-0.0.8.dev0/PKG-INFO
```

### Comparing `gdptools_pygeoapi_plugin-0.0.7.dev0/LICENSE.md` & `gdptools_pygeoapi_plugin-0.0.8.dev0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gdptools_pygeoapi_plugin-0.0.7.dev0/README.md` & `gdptools_pygeoapi_plugin-0.0.8.dev0/README.md`

 * *Files identical despite different names*

### Comparing `gdptools_pygeoapi_plugin-0.0.7.dev0/pyproject.toml` & `gdptools_pygeoapi_plugin-0.0.8.dev0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "gdptools-pygeoapi-plugin"
-version = "0.0.7-dev0"
+version = "0.0.8-dev0"
 description = "Gdptools Pygeoapi Plugin"
 authors = ["Richard McDonald <rmcd@usgs.gov>"]
 license = "LICENSE.md"
 readme = "README.md"
 homepage = "https://code.usgs.gov/wma/nhgf/toolsteam/gdptools-pygeoapi-plugin"
 repository = "https://code.usgs.gov/wma/nhgf/toolsteam/gdptools-pygeoapi-plugin"
 documentation = "https://gdptools-pygeoapi-plugin.readthedocs.io"
@@ -21,47 +21,46 @@
 ]
 
 [tool.poetry.urls]
 Changelog = "https://code.usgs.gov/wma/nhgf/toolsteam/gdptools-pygeoapi-plugin/releases"
 
 [tool.poetry.dependencies]
 python = "<3.10,>=3.9"
-click = "<8"
-pygeoapi = ">0.11.0"
-numpy = "^1.21.0"
-gdptools = ">=0.0.32"
+pygeoapi = ">=0.14.0"
+gdptools = ">=0.0.34"
+requests-toolbelt = "^1.0.0"
 
 [tool.poetry.dev-dependencies]
 advbumpversion = "^1.2.0"
 pytest = "^6.2.4"
 coverage = {extras = ["toml"], version = "^5.4"}
-safety = "^1.10.3"
-mypy = "^0.910"
-typeguard = "^2.12.1"
+safety = ">=1.10.3"
+mypy = ">=0.910"
+typeguard = ">=2.12.1"
 xdoctest = {extras = ["colors"], version = "^0.15.5"}
-sphinx = "^4.1.2"
-sphinx-autobuild = "^2021.3.14"
+sphinx = ">=4.1.2"
+sphinx-autobuild = ">=2021.3.14"
 pre-commit = "^2.13.0"
-flake8 = "^3.9.2"
-black = "<=21.12b0"
-flake8-bandit = "^2.1.2"
-flake8-bugbear = "^21.4.3"
-flake8-docstrings = "^1.6.0"
-flake8-rst-docstrings = "^0.2.3"
-pep8-naming = "^0.12.0"
+flake8 = ">=3.9.2"
+black = ">=22.1.0"
+flake8-bandit = ">=2.1.2"
+flake8-bugbear = ">=21.4.3"
+flake8-docstrings = ">=1.6.0"
+flake8-rst-docstrings = ">=0.2.3"
+pep8-naming = ">=0.12.0"
 darglint = "^1.8.0"
 reorder-python-imports = "^2.6.0"
 pre-commit-hooks = "^4.0.1"
 sphinx-rtd-theme = "^0.5.2"
 sphinx-click = "^3.0.1"
 Pygments = "^2.9.0"
 poetry2conda = "^0.3.0"
-nox = "^2021.10.1"
-nox_poetry = "^0.8.6"
-types-all = "^1.0.0"
+nox = ">=2021.10.1"
+nox_poetry = ">=0.8.6"
+types-all = ">=1.0.0"
 urllib3 = "<=1.26.15"
 
 [tool.poetry.scripts]
 gdptools-pygeoapi-plugin = "gdptools_pygeoapi_plugin.__main__:main"
 
 [tool.poetry2conda]
 name = "gdptools-pygeoapi-plugin"
```

### Comparing `gdptools_pygeoapi_plugin-0.0.7.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/calc_weights_catalog.py` & `gdptools_pygeoapi_plugin-0.0.8.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/calc_agg_catalog.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,141 +2,127 @@
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Tuple
 
 import geopandas as gpd
-from gdptools import ODAPCatData
-from gdptools import WeightGen
+import pandas as pd
+from gdptools import AggGen
+from gdptools import ClimRCatData
 from pygeoapi.process.base import BaseProcessor
 
+# import tempfile
+# from pathlib import Path
+
 LOGGER = logging.getLogger(__name__)
 
 PROCESS_METADATA = {
     "version": "0.1.0",
-    "id": "calc_weights_catalog",
-    "title": "Calculate weights for area-weighted aggregation",
-    "description": "Calculate weights for OpenDAP endpoint and user-defined Features",
+    "id": "run_weights_catalog",
+    "title": "run area-weighted aggregation",
+    "description": """Run area-weighted aggredation using  OpenDAP endpoint and
+        user-defined Features""",
+    "jobControlOptions": ["sync-execute", "async-execute"],
     "keywords": ["area-weighted intersections"],
     "links": [
         {
             "type": "text/html",
             "rel": "canonical",
             "title": "information",
             "href": "https://example.org/process",
             "hreflang": "en-CA",
         }
     ],
     "inputs": {
-        "param_dict": {
-            "title": "param_json fragment for openDAP catalog",
-            "description": (
-                "The parameter json fragment associated with the ",
-                "openDAP endpoint of user interest",
-            ),
+        "cat_dict": {
+            "title": "cat_dict",
             "schema": {"type": "string"},
             "minOccurs": 1,
             "maxOccurs": 1,
         },
-        "grid_dict": {
-            "title": "grid_json_string",
+        "weights": {
+            "title": "weights_json_string",
             "schema": {"type": "string"},
             "minOccurs": 1,
             "maxOccurs": 1,
         },
         "shape_file": {
             "title": "shape_file_json_string",
             "schema": {"type": "string"},
             "minOccurs": 1,
             "maxOccurs": 1,
         },
         "shape_crs": {
-            "title": "shape_crs_string",
-            "schema": {
-                "type": "string",
-            },
+            "title": "shape_file_crs_string",
+            "schema": {"type": "string"},
             "minOccurs": 1,
             "maxOccurs": 1,
         },
         "shape_poly_idx": {
             "title": "shape_poly_idx_string",
             "schema": {
                 "type": "string",
             },
             "minOccurs": 1,
             "maxOccurs": 1,
         },
-        "wght_gen_proj": {
-            "title": "Projection string (epsg code or proj string)",
-            "schema": {"type": "string"},
-            "minOccurs": 1,
-            "maxOccurs": 1,
-        },
         "start_date": {
             "title": "Beginning date to pull from openDAP endpoint",
             "schema": {"type": "string"},
             "minOccurs": 1,
             "maxOccurs": 1,
         },
         "end_date": {
             "title": "Ending date to pull from openDAP endpoint",
             "schema": {"type": "string"},
             "minOccurs": 1,
             "maxOccurs": 1,
         },
     },
     "outputs": {
-        "weights": {
-            "title": "Comma separated weights, id, i, j, weight",
-            "schema": {"type": "object", "contentMediaType": "application/json"},
+        "aggregated_json": {
+            "title": "json records file of aggregated values",
+            "schema": {"type": "object", "contentMediaType": "application/parquet"},
         }
     },
     "example": {
         "inputs": {
-            "param_dict": (
-                '{"aet": {"id": "terraclim", "grid_id": 116.0, "URL":'
-                ' "http://thredds.northwestknowledge.net:8080/thredds/dodsC/'
-                'agg_terraclimate_aet_1958_CurrentYear_GLOBE.nc", "tiled": "", '
-                '"variable": "aet", "varname": "aet", "long_name": '
-                '"water_evaporation_amount", "T_name": "time", "duration": '
-                '"1958-01-01/2020-12-01", "interval": "1 months", "nT": 756.0, '
-                '"units": "mm", "model": NaN, "ensemble": NaN, "scenario": "total"}, '
-                '"pet": {"id": "terraclim", "grid_id": 116.0, "URL": '
-                '"http://thredds.northwestknowledge.net:8080/thredds/dodsC/'
-                'agg_terraclimate_pet_1958_CurrentYear_GLOBE.nc", "tiled": "", '
-                '"variable": "pet", "varname": "pet", "long_name": '
-                '"water_potential_evaporation_amount", "T_name": "time", "duration": '
-                '"1958-01-01/2020-12-01", "interval": "1 months", "nT": 756.0, "units":'
-                '  "mm", "model": NaN, "ensemble": NaN, "scenario": "total"}, '
-                '"PDSI": {"id": "terraclim", "grid_id": 116.0, "URL": '
-                '"http://thredds.northwestknowledge.net:8080/thredds/dodsC/'
-                'agg_terraclimate_PDSI_1958_CurrentYear_GLOBE.nc", "tiled": "", '
-                '"variable": "PDSI", "varname": "PDSI", "long_name": '
-                '"palmer_drought_severity_index", "T_name": "time", "duration": '
-                '"1958-01-01/2020-12-01", "interval": "1 months", "nT": 756.0, '
-                '"units": "unitless", "model": NaN, "ensemble": NaN, "scenario": '
-                '"total"}}'
-            ),
-            "grid_dict": (
-                '{"aet": {"grid_id": 116.0, "X_name": "lon", "Y_name": "lat", '
-                '"X1": -179.9792, "Xn": 179.9792, "Y1": 89.9792, "Yn": -89.9792, '
-                '"resX": 0.0417, "resY": 0.0417, "ncols": 8640, "nrows": 4320, "proj": '
-                '"+proj=longlat +a=6378137 +f=0.00335281066474748 +pm=0 +no_defs", '
-                '"toptobottom": 0.0, "tile": NaN, "grid.id": NaN}, '
-                '"pet": {"grid_id": 116.0, "X_name": "lon", "Y_name": "lat", '
-                '"X1": -179.9792, "Xn": 179.9792, "Y1": 89.9792, "Yn": -89.9792, '
-                '"resX": 0.0417, "resY": 0.0417, "ncols": 8640, "nrows": 4320, "proj": '
+            "cat_dict": (
+                '{"aet": {"id": "terraclim", "asset": '
+                '"agg_terraclimate_aet_1958_CurrentYear_GLOBE", "URL": '
+                '"http://thredds.northwestknowledge.net:8080/thredds/dodsC/agg_terraclimate_aet_1958_CurrentYear_GLOBE.nc", '  # noqa: B950
+                '"type": "opendap", "varname": "aet", "variable": "aet", "description": '
+                '"water_evaporation_amount", "units": "mm", "model": null, "ensemble": null, '
+                '"scenario": "total", "T_name": "time", "duration": "1958-01-01/2021-12-01", '
+                '"interval": "1 months", "nT": 768.0, "X_name": "lon", "Y_name": "lat", "X1": '
+                '-179.97916666666666, "Xn": 179.97916666666666, "Y1": 89.97916666666667, '
+                '"Yn": -89.97916666666664, "resX": 0.041666666666666664, "resY": '
+                '0.041666666666666664, "ncols": 8640.0, "nrows": 4320.0, "crs": '
                 '"+proj=longlat +a=6378137 +f=0.00335281066474748 +pm=0 +no_defs", '
-                '"toptobottom": 0.0, "tile": NaN, "grid.id": NaN}, '
-                '"PDSI": {"grid_id": 116.0, "X_name": "lon", "Y_name": "lat", '
-                '"X1": -179.9792, "Xn": 179.9792, "Y1": 89.9792, "Yn": -89.9792, '
-                '"resX": 0.0417, "resY": 0.0417, "ncols": 8640, "nrows": 4320, "proj": '
-                '"+proj=longlat +a=6378137 +f=0.00335281066474748 +pm=0 +no_defs", '
-                '"toptobottom": 0.0, "tile": NaN, "grid.id": NaN}}'
+                '"toptobottom": false, "tiled": ""}, "pet": {"id": "terraclim", "asset": '
+                '"agg_terraclimate_pet_1958_CurrentYear_GLOBE", "URL": '
+                '"http://thredds.northwestknowledge.net:8080/thredds/dodsC/agg_terraclimate_pet_1958_CurrentYear_GLOBE.nc", '  # noqa: B950
+                '"type": "opendap", "varname": "pet", "variable": "pet", "description": '
+                '"water_potential_evaporation_amount", "units": "mm", "model": null, '
+                '"ensemble": null, "scenario": "total", "T_name": "time", "duration": '
+                '"1958-01-01/2021-12-01", "interval": "1 months", "nT": 768.0, "X_name": '
+                '"lon", "Y_name": "lat", "X1": -179.97916666666666, "Xn": 179.97916666666666, '
+                '"Y1": 89.97916666666667, "Yn": -89.97916666666664, "resX": '
+                '0.041666666666666664, "resY": 0.041666666666666664, "ncols": 8640.0, '
+                '"nrows": 4320.0, "crs": "+proj=longlat +a=6378137 +f=0.00335281066474748 '
+                '+pm=0 +no_defs", "toptobottom": false, "tiled": ""}}'
+            ),
+            "weights": (
+                '{"i":{"0":2,"1":1,"2":2,"3":1},'
+                '"index":{"0":0,"1":1,"2":2,"3":3},'
+                '"j":{"0":3,"1":3,"2":2,"3":2},'
+                '"poly_idx":{"0":"1","1":"1","2":"1","3":"1"},'
+                '"wght":{'
+                '"0":0.138616567,"1":0.001795472,"2":0.7689606915,"3":0.0906272694}}'
             ),
             "shape_file": (
                 '{"type": "FeatureCollection", "features": ['
                 '{"id": "0", "type": "Feature", "properties": {'
                 '"id": 1, "poly_idx": "1"}, "geometry": {'
                 '"type": "Polygon", "coordinates": [['
                 "[-70.60141212297273, 41.9262774500321], "
@@ -144,74 +130,88 @@
                 "[-70.5867037815952, 41.87626908934851], "
                 "[-70.61906213262577, 41.889506596588284], "
                 "[-70.60141212297273, 41.9262774500321]"
                 "]]}}]}"
             ),
             "shape_crs": "4326",
             "shape_poly_idx": "poly_idx",
-            "wght_gen_proj": "6931",
             "start_date": "1980-01-01",
             "end_date": "1980-12-31",
         }
     },
 }
 
 
-class GDPCalcWeightsCatalogProcessor(BaseProcessor):  # type: ignore
-    """Generate weights for grid-to-poly aggregation."""
+class GDPCalcAggCatalogProcessor(BaseProcessor):  # type: ignore
+    """Run area-weighted grid-to-poly aggregation."""
 
     def __init__(self, processor_def: dict[str, Any]):
         """Initialize Processor.
 
         Args:
             processor_def (_type_): _description_
         """
         super().__init__(processor_def, PROCESS_METADATA)
 
     def execute(self, data: Dict[str, Dict[str, Any]]) -> Tuple[str, Dict[str, Any]]:
-        """Execute calc_weights_catalog web service."""
-        param_dict = json.loads(str(data["param_dict"]))
-        grid_dict = json.loads(str(data["grid_dict"]))
+        """Execute run_weights_catalog web service."""
+        cat_dict = json.loads(str(data["cat_dict"]))
+        wghts = json.loads(str(data["weights"]))
         shpfile_feat = json.loads(str(data["shape_file"]))
         shp_crs = str(data["shape_crs"])
         shp_poly_idx = str(data["shape_poly_idx"])
-        wght_gen_proj = str(data["wght_gen_proj"])
         start_date = str(data["start_date"])
         end_date = str(data["end_date"])
         period = [start_date, end_date]
 
+        weights = pd.DataFrame.from_dict(wghts)
         shp_file = gpd.GeoDataFrame.from_features(shpfile_feat)
         shp_file.set_crs(shp_crs, inplace=True)
 
-        LOGGER.info(f"param_dict: {param_dict}  type: {type(param_dict)}\n")
-        LOGGER.info(f"grid_dict: {grid_dict} type: {type(grid_dict)}\n")
+        LOGGER.info(f"cat_dict: {cat_dict}  type: {type(cat_dict)}\n")
+        LOGGER.info(f"weights: {weights.head()} type: {type(weights)}\n")
         LOGGER.info(f"shp_file: {shp_file.head()} type: {type(shp_file)}\n")
         LOGGER.info(f"shp_poly_idx: {shp_poly_idx} type: {type(shp_poly_idx)}\n")
-        LOGGER.info(f"wght_gen_proj: {wght_gen_proj} type: {type(wght_gen_proj)}\n")
+        LOGGER.info(f"start_date: {start_date} type: {type(start_date)}\n")
+        LOGGER.info(f"end_date: {end_date} type: {type(end_date)}\n")
 
-        user_data = ODAPCatData(
-            param_dict=param_dict,
-            grid_dict=grid_dict,
+        user_data = ClimRCatData(
+            cat_dict=cat_dict,
             f_feature=shp_file,
             id_feature=shp_poly_idx,
             period=period,
         )
-        wght_gen = WeightGen(
-            user_data=user_data, method="serial", output_file="", weight_gen_crs=6931
+        # tempdir = tempfile.TemporaryDirectory()
+        agg_gen = AggGen(
+            user_data=user_data,
+            stat_method="masked_mean",
+            agg_engine="serial",
+            agg_writer="none",
+            weights=weights,
+        )
+        ngdf, nvals = agg_gen.calculate_agg()
+        for idx, (_key, value) in enumerate(agg_gen.agg_data.items()):
+            gdf = ngdf
+            param_values = value.cat_param
+            t_coord = param_values.T_name
+            units = param_values.units
+            varname = param_values.varname
+            time = value.da.coords[t_coord].values
+
+            df_key = pd.DataFrame(data=nvals[_key].values, columns=gdf.index.T.values)
+
+            df_key.insert(0, "units", [units] * df_key.shape[0])
+            df_key.insert(0, "varname", [varname] * df_key.shape[0])
+            df_key.insert(0, "time", time)
+
+            if idx == 0:
+                df = df_key
+            else:
+                df = pd.concat([df, df_key])
+        df.reset_index(inplace=True)
+        return "application/json", json.loads(
+            df.to_json(date_format="iso", orient="index")
         )
-
-        wghts = wght_gen.calculate_weights(intersections=True)
-        # cp = CatParams(**(json.loads(pjson)))
-        # cg = CatGrids(**(json.loads(gjson)))
-        # wght = calc_weights_catalog2(
-        #     params_json=cp,
-        #     grid_json=cg,
-        #     shp_file=shp_file,
-        #     shp_poly_idx=shp_poly_idx,
-        #     wght_gen_proj=wght_gen_proj,
-        # )
-        wghts.reset_index(inplace=True)
-        return "application/json", json.loads(wghts.to_json())
 
     def __repr__(self):  # type: ignore
         """Return representation."""
         return f"<GDPCalcWeightsCatalogProcessor> {self.name}"
```

### Comparing `gdptools_pygeoapi_plugin-0.0.7.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/proc_test.py` & `gdptools_pygeoapi_plugin-0.0.8.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/proc_test.py`

 * *Files identical despite different names*

### Comparing `gdptools_pygeoapi_plugin-0.0.7.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/run_weights_catalog.py` & `gdptools_pygeoapi_plugin-0.0.8.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/calc_weights_catalog.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,225 +1,190 @@
 """Calc_weights_catalog_proceess."""
 import json
 import logging
-import tempfile
-from pathlib import Path
 from typing import Any
 from typing import Dict
 from typing import Tuple
 
 import geopandas as gpd
-import pandas as pd
-from gdptools import AggGen
-from gdptools import ODAPCatData
+from gdptools import ClimRCatData
+from gdptools import WeightGen
 from pygeoapi.process.base import BaseProcessor
 
 LOGGER = logging.getLogger(__name__)
 
 PROCESS_METADATA = {
     "version": "0.1.0",
-    "id": "run_weights_catalog",
-    "title": "run area-weighted aggregation",
-    "description": """Run area-weighted aggredation using  OpenDAP endpoint and
-        user-defined Features""",
+    "id": "calc_weights_catalog",
+    "title": "Calculate weights for area-weighted aggregation",
+    "description": "Calculate weights for OpenDAP endpoint and user-defined Features",
+    "jobControlOptions": ["sync-execute", "async-execute"],
     "keywords": ["area-weighted intersections"],
     "links": [
         {
             "type": "text/html",
             "rel": "canonical",
             "title": "information",
             "href": "https://example.org/process",
             "hreflang": "en-CA",
         }
     ],
     "inputs": {
-        "param_dict": {
-            "title": "param_dict",
-            "schema": {"type": "string"},
-            "minOccurs": 1,
-            "maxOccurs": 1,
-        },
-        "grid_dict": {
-            "title": "grid_dict",
-            "schema": {"type": "string"},
-            "minOccurs": 1,
-            "maxOccurs": 1,
-        },
-        "weights": {
-            "title": "weights_json_string",
+        "cat_dict": {
+            "title": "Dictionary dict[key, catalog] input for ClimRCatData",
+            "description": (
+                "The parameter json fragment associated with the ",
+                "openDAP endpoint of user interest",
+            ),
             "schema": {"type": "string"},
             "minOccurs": 1,
             "maxOccurs": 1,
         },
         "shape_file": {
             "title": "shape_file_json_string",
             "schema": {"type": "string"},
             "minOccurs": 1,
             "maxOccurs": 1,
         },
         "shape_crs": {
-            "title": "shape_file_crs_string",
-            "schema": {"type": "string"},
+            "title": "shape_crs_string",
+            "schema": {
+                "type": "string",
+            },
             "minOccurs": 1,
             "maxOccurs": 1,
         },
         "shape_poly_idx": {
             "title": "shape_poly_idx_string",
             "schema": {
                 "type": "string",
             },
             "minOccurs": 1,
             "maxOccurs": 1,
         },
+        "wght_gen_proj": {
+            "title": "Projection string (epsg code or proj string)",
+            "schema": {"type": "string"},
+            "minOccurs": 1,
+            "maxOccurs": 1,
+        },
         "start_date": {
             "title": "Beginning date to pull from openDAP endpoint",
             "schema": {"type": "string"},
             "minOccurs": 1,
             "maxOccurs": 1,
         },
         "end_date": {
             "title": "Ending date to pull from openDAP endpoint",
             "schema": {"type": "string"},
             "minOccurs": 1,
             "maxOccurs": 1,
         },
     },
     "outputs": {
-        "aggregated_json": {
-            "title": "json records file of aggregated values",
+        "weights": {
+            "title": "Comma separated weights, id, i, j, weight",
             "schema": {"type": "object", "contentMediaType": "application/json"},
         }
     },
     "example": {
         "inputs": {
-            "param_dict": (
-                '{"aet": {"id": "terraclim", "grid_id": 116.0, "URL":'
-                ' "http://thredds.northwestknowledge.net:8080/thredds/dodsC/'
-                'agg_terraclimate_aet_1958_CurrentYear_GLOBE.nc", "tiled": "", '
-                '"variable": "aet", "varname": "aet", "long_name": '
-                '"water_evaporation_amount", "T_name": "time", "duration": '
-                '"1958-01-01/2020-12-01", "interval": "1 months", "nT": 756.0, '
-                '"units": "mm", "model": NaN, "ensemble": NaN, "scenario": "total"}, '
-                '"pet": {"id": "terraclim", "grid_id": 116.0, "URL": '
-                '"http://thredds.northwestknowledge.net:8080/thredds/dodsC/'
-                'agg_terraclimate_pet_1958_CurrentYear_GLOBE.nc", "tiled": "", '
-                '"variable": "pet", "varname": "pet", "long_name": '
-                '"water_potential_evaporation_amount", "T_name": "time", "duration": '
-                '"1958-01-01/2020-12-01", "interval": "1 months", "nT": 756.0, "units":'
-                '  "mm", "model": NaN, "ensemble": NaN, "scenario": "total"}, '
-                '"PDSI": {"id": "terraclim", "grid_id": 116.0, "URL": '
-                '"http://thredds.northwestknowledge.net:8080/thredds/dodsC/'
-                'agg_terraclimate_PDSI_1958_CurrentYear_GLOBE.nc", "tiled": "", '
-                '"variable": "PDSI", "varname": "PDSI", "long_name": '
-                '"palmer_drought_severity_index", "T_name": "time", "duration": '
-                '"1958-01-01/2020-12-01", "interval": "1 months", "nT": 756.0, '
-                '"units": "unitless", "model": NaN, "ensemble": NaN, "scenario": '
-                '"total"}}'
-            ),
-            "grid_dict": (
-                '{"aet": {"grid_id": 116.0, "X_name": "lon", "Y_name": "lat", '
-                '"X1": -179.9792, "Xn": 179.9792, "Y1": 89.9792, "Yn": -89.9792, '
-                '"resX": 0.0417, "resY": 0.0417, "ncols": 8640, "nrows": 4320, "proj": '
-                '"+proj=longlat +a=6378137 +f=0.00335281066474748 +pm=0 +no_defs", '
-                '"toptobottom": 0.0, "tile": NaN, "grid.id": NaN}, '
-                '"pet": {"grid_id": 116.0, "X_name": "lon", "Y_name": "lat", '
-                '"X1": -179.9792, "Xn": 179.9792, "Y1": 89.9792, "Yn": -89.9792, '
-                '"resX": 0.0417, "resY": 0.0417, "ncols": 8640, "nrows": 4320, "proj": '
+            "cat_dict": (
+                '{"aet": {"id": "terraclim", "asset": '
+                '"agg_terraclimate_aet_1958_CurrentYear_GLOBE", "URL": '
+                '"http://thredds.northwestknowledge.net:8080/thredds/dodsC/agg_terraclimate_aet_1958_CurrentYear_GLOBE.nc", '  # noqa: B950
+                '"type": "opendap", "varname": "aet", "variable": "aet", "description": '
+                '"water_evaporation_amount", "units": "mm", "model": null, "ensemble": null, '
+                '"scenario": "total", "T_name": "time", "duration": "1958-01-01/2021-12-01", '
+                '"interval": "1 months", "nT": 768.0, "X_name": "lon", "Y_name": "lat", "X1": '
+                '-179.97916666666666, "Xn": 179.97916666666666, "Y1": 89.97916666666667, '
+                '"Yn": -89.97916666666664, "resX": 0.041666666666666664, "resY": '
+                '0.041666666666666664, "ncols": 8640.0, "nrows": 4320.0, "crs": '
                 '"+proj=longlat +a=6378137 +f=0.00335281066474748 +pm=0 +no_defs", '
-                '"toptobottom": 0.0, "tile": NaN, "grid.id": NaN}, '
-                '"PDSI": {"grid_id": 116.0, "X_name": "lon", "Y_name": "lat", '
-                '"X1": -179.9792, "Xn": 179.9792, "Y1": 89.9792, "Yn": -89.9792, '
-                '"resX": 0.0417, "resY": 0.0417, "ncols": 8640, "nrows": 4320, "proj": '
-                '"+proj=longlat +a=6378137 +f=0.00335281066474748 +pm=0 +no_defs", '
-                '"toptobottom": 0.0, "tile": NaN, "grid.id": NaN}}'
-            ),
-            "weights": (
-                '{"i":{"0":2,"1":1,"2":2,"3":1},'
-                '"index":{"0":0,"1":1,"2":2,"3":3},'
-                '"j":{"0":3,"1":3,"2":2,"3":2},'
-                '"poly_idx":{"0":"1","1":"1","2":"1","3":"1"},'
-                '"wght":{'
-                '"0":0.138616567,"1":0.001795472,"2":0.7689606915,"3":0.0906272694}}'
+                '"toptobottom": false, "tiled": ""}, "pet": {"id": "terraclim", "asset": '
+                '"agg_terraclimate_pet_1958_CurrentYear_GLOBE", "URL": '
+                '"http://thredds.northwestknowledge.net:8080/thredds/dodsC/agg_terraclimate_pet_1958_CurrentYear_GLOBE.nc", '  # noqa: B950
+                '"type": "opendap", "varname": "pet", "variable": "pet", "description": '
+                '"water_potential_evaporation_amount", "units": "mm", "model": null, '
+                '"ensemble": null, "scenario": "total", "T_name": "time", "duration": '
+                '"1958-01-01/2021-12-01", "interval": "1 months", "nT": 768.0, "X_name": '
+                '"lon", "Y_name": "lat", "X1": -179.97916666666666, "Xn": 179.97916666666666, '
+                '"Y1": 89.97916666666667, "Yn": -89.97916666666664, "resX": '
+                '0.041666666666666664, "resY": 0.041666666666666664, "ncols": 8640.0, '
+                '"nrows": 4320.0, "crs": "+proj=longlat +a=6378137 +f=0.00335281066474748 '
+                '+pm=0 +no_defs", "toptobottom": false, "tiled": ""}}'
             ),
             "shape_file": (
-                '{"type": "FeatureCollection", "features": ['
-                '{"id": "0", "type": "Feature", "properties": {'
-                '"id": 1, "poly_idx": "1"}, "geometry": {'
-                '"type": "Polygon", "coordinates": [['
-                "[-70.60141212297273, 41.9262774500321], "
-                "[-70.57199544021768, 41.91303994279233], "
-                "[-70.5867037815952, 41.87626908934851], "
-                "[-70.61906213262577, 41.889506596588284], "
-                "[-70.60141212297273, 41.9262774500321]"
-                "]]}}]}"
+                '{"type": "FeatureCollection", "features": [{"id": "0", "type": "Feature", '
+                '"properties": {"id": 1, "poly_idx": "1"}, "geometry": {"type": "Polygon", '
+                '"coordinates": [[[-70.60141212297273, 41.9262774500321], '
+                "[-70.57199544021768, 41.91303994279233], [-70.5867037815952, "
+                "41.87626908934851], [-70.61906213262577, 41.889506596588284], "
+                "[-70.60141212297273, 41.9262774500321]]]}}]}"
             ),
             "shape_crs": "4326",
             "shape_poly_idx": "poly_idx",
+            "wght_gen_proj": "6931",
             "start_date": "1980-01-01",
             "end_date": "1980-12-31",
         }
     },
 }
 
 
-class GDPRunWeightsCatalogProcessor(BaseProcessor):  # type: ignore
-    """Run area-weighted grid-to-poly aggregation."""
+class GDPCalcWeightsCatalogProcessor(BaseProcessor):  # type: ignore
+    """Generate weights for grid-to-poly aggregation."""
 
     def __init__(self, processor_def: dict[str, Any]):
         """Initialize Processor.
 
         Args:
             processor_def (_type_): _description_
         """
         super().__init__(processor_def, PROCESS_METADATA)
 
     def execute(self, data: Dict[str, Dict[str, Any]]) -> Tuple[str, Dict[str, Any]]:
-        """Execute run_weights_catalog web service."""
-        param_dict = json.loads(str(data["param_dict"]))
-        grid_dict = json.loads(str(data["grid_dict"]))
-        wghts = json.loads(str(data["weights"]))
+        """Execute calc_weights_catalog web service."""
+        # print(data)
+        cat_dict = json.loads(str(data["cat_dict"]))
         shpfile_feat = json.loads(str(data["shape_file"]))
         shp_crs = str(data["shape_crs"])
         shp_poly_idx = str(data["shape_poly_idx"])
+        wght_gen_proj = str(data["wght_gen_proj"])
         start_date = str(data["start_date"])
         end_date = str(data["end_date"])
         period = [start_date, end_date]
 
-        weights = pd.DataFrame.from_dict(wghts)
         shp_file = gpd.GeoDataFrame.from_features(shpfile_feat)
         shp_file.set_crs(shp_crs, inplace=True)
 
-        LOGGER.info(f"param_dict: {param_dict}  type: {type(param_dict)}\n")
-        LOGGER.info(f"grid_dict: {grid_dict} type: {type(grid_dict)}\n")
-        LOGGER.info(f"weights: {weights} type: {type(weights)}\n")
+        LOGGER.info(f"param_dict: {cat_dict}  type: {type(cat_dict)}\n")
         LOGGER.info(f"shp_file: {shp_file.head()} type: {type(shp_file)}\n")
         LOGGER.info(f"shp_poly_idx: {shp_poly_idx} type: {type(shp_poly_idx)}\n")
-        LOGGER.info(f"start_date: {start_date} type: {type(start_date)}\n")
-        LOGGER.info(f"end_date: {end_date} type: {type(end_date)}\n")
+        LOGGER.info(f"wght_gen_proj: {wght_gen_proj} type: {type(wght_gen_proj)}\n")
 
-        user_data = ODAPCatData(
-            param_dict=param_dict,
-            grid_dict=grid_dict,
+        user_data = ClimRCatData(
+            cat_dict=cat_dict,
             f_feature=shp_file,
             id_feature=shp_poly_idx,
             period=period,
         )
-        tempdir = tempfile.TemporaryDirectory()
-        agg_gen = AggGen(
-            user_data=user_data,
-            stat_method="masked_average",
-            agg_engine="serial",
-            agg_writer="json",
-            out_path=tempdir.name,
-            file_prefix="temp_outfile",
-            weights=weights,
+        wght_gen = WeightGen(
+            user_data=user_data, method="serial", output_file="", weight_gen_crs=6931
         )
-        ngdf, nvals = agg_gen.calculate_agg()
-
-        ofile = Path(tempdir.name) / "temp_outfile.json"
 
-        df = pd.read_json(ofile)
-        return "application/json", df.to_json(orient="records", date_format="iso")
+        wghts = wght_gen.calculate_weights(intersections=True)
+        # cp = CatParams(**(json.loads(pjson)))
+        # cg = CatGrids(**(json.loads(gjson)))
+        # wght = calc_weights_catalog2(
+        #     params_json=cp,
+        #     grid_json=cg,
+        #     shp_file=shp_file,
+        #     shp_poly_idx=shp_poly_idx,
+        #     wght_gen_proj=wght_gen_proj,
+        # )
+        wghts.reset_index(inplace=True)
+        return "application/json", json.loads(wghts.to_json())
 
     def __repr__(self):  # type: ignore
         """Return representation."""
         return f"<GDPCalcWeightsCatalogProcessor> {self.name}"
```

### Comparing `gdptools_pygeoapi_plugin-0.0.7.dev0/PKG-INFO` & `gdptools_pygeoapi_plugin-0.0.8.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: gdptools-pygeoapi-plugin
-Version: 0.0.7.dev0
+Version: 0.0.8.dev0
 Summary: Gdptools Pygeoapi Plugin
 Home-page: https://code.usgs.gov/wma/nhgf/toolsteam/gdptools-pygeoapi-plugin
 License: LICENSE.md
 Author: Richard McDonald
 Author-email: rmcd@usgs.gov
 Requires-Python: >=3.9,<3.10
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: click (<8)
-Requires-Dist: gdptools (>=0.0.32)
-Requires-Dist: numpy (>=1.21.0,<2.0.0)
-Requires-Dist: pygeoapi (>0.11.0)
+Requires-Dist: gdptools (>=0.0.34)
+Requires-Dist: pygeoapi (>=0.14.0)
+Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Project-URL: Changelog, https://code.usgs.gov/wma/nhgf/toolsteam/gdptools-pygeoapi-plugin/releases
 Project-URL: Documentation, https://gdptools-pygeoapi-plugin.readthedocs.io
 Project-URL: Repository, https://code.usgs.gov/wma/nhgf/toolsteam/gdptools-pygeoapi-plugin
 Description-Content-Type: text/markdown
 
 ---
```

