# Comparing `tmp/sibyl_api-0.1.0.2.tar.gz` & `tmp/sibyl_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sibyl_api-0.1.0.2.tar", max compression
+gzip compressed data, was "sibyl_api-0.1.1.tar", max compression
```

## Comparing `sibyl_api-0.1.0.2.tar` & `sibyl_api-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1077 2024-02-26 16:01:06.082941 sibyl_api-0.1.0.2/LICENSE
--rw-r--r--   0        0        0     8273 2024-02-26 16:01:06.082941 sibyl_api-0.1.0.2/README.md
--rw-r--r--   0        0        0     1892 2024-02-26 16:01:06.086941 sibyl_api-0.1.0.2/pyproject.toml
--rw-r--r--   0        0        0      243 2024-02-26 16:01:06.086941 sibyl_api-0.1.0.2/sibyl/__init__.py
--rw-r--r--   0        0        0     3498 2024-02-26 16:01:06.086941 sibyl_api-0.1.0.2/sibyl/cli.py
--rw-r--r--   0        0        0      648 2024-02-26 16:01:06.086941 sibyl_api-0.1.0.2/sibyl/config.yml
--rw-r--r--   0        0        0     3412 2024-02-26 16:01:06.086941 sibyl_api-0.1.0.2/sibyl/core.py
--rw-r--r--   0        0        0     2217 2024-02-26 16:01:06.086941 sibyl_api-0.1.0.2/sibyl/data.py
--rw-r--r--   0        0        0     1408 2024-02-26 16:01:06.086941 sibyl_api-0.1.0.2/sibyl/db/__init__.py
--rw-r--r--   0        0        0     5645 2024-02-26 16:01:06.086941 sibyl_api-0.1.0.2/sibyl/db/base.py
--rw-r--r--   0        0        0     6959 2024-02-26 16:01:06.086941 sibyl_api-0.1.0.2/sibyl/db/explorer.py
--rw-r--r--   0        0        0      642 2024-02-26 16:01:06.086941 sibyl_api-0.1.0.2/sibyl/db/output_presets.yml
--rw-r--r--   0        0        0    29264 2024-02-26 16:01:06.086941 sibyl_api-0.1.0.2/sibyl/db/preprocessing.py
--rw-r--r--   0        0        0     7264 2024-02-26 16:01:06.086941 sibyl_api-0.1.0.2/sibyl/db/schema.py
--rw-r--r--   0        0        0     4906 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/db/utils.py
--rw-r--r--   0        0        0     1749 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/helpers.py
--rw-r--r--   0        0        0      344 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/resources/__init__.py
--rw-r--r--   0        0        0    17352 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/resources/computing.py
--rw-r--r--   0        0        0     3515 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/resources/context.py
--rw-r--r--   0        0        0     9145 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/resources/entity.py
--rw-r--r--   0        0        0     8979 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/resources/feature.py
--rw-r--r--   0        0        0     2353 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/resources/group.py
--rw-r--r--   0        0        0     3662 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/resources/logger.py
--rw-r--r--   0        0        0    10497 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/resources/model.py
--rw-r--r--   0        0        0     2528 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/routes.py
--rw-r--r--   0        0        0        0 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/sample_applications/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/sample_applications/housing/__init__.py
--rw-r--r--   0        0        0     1195 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/sample_applications/housing/context_config.yml
--rw-r--r--   0        0        0     4894 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/sample_applications/housing/features.csv
--rw-r--r--   0        0        0     1249 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/sample_applications/housing/prepare_db.py
--rw-r--r--   0        0        0     1471 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/sample_applications/housing/prepare_db_config.yml
--rw-r--r--   0        0        0     7352 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/swagger.py
--rw-r--r--   0        0        0     1646 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/templates/context_config_template.yml
--rw-r--r--   0        0        0     2188 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/templates/prepare_db_config_template.yml
--rw-r--r--   0        0        0     3486 2024-02-26 16:01:06.090941 sibyl_api-0.1.0.2/sibyl/utils.py
--rw-r--r--   0        0        0     9994 1970-01-01 00:00:00.000000 sibyl_api-0.1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-26 13:53:05.403081 sibyl_api-0.1.1/LICENSE
+-rw-r--r--   0        0        0     8232 2024-04-26 13:53:05.403081 sibyl_api-0.1.1/README.md
+-rw-r--r--   0        0        0     1890 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      241 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/__init__.py
+-rw-r--r--   0        0        0     3498 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/cli.py
+-rw-r--r--   0        0        0      648 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/config.yml
+-rw-r--r--   0        0        0     3412 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/core.py
+-rw-r--r--   0        0        0     2217 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/data.py
+-rw-r--r--   0        0        0     1408 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/db/__init__.py
+-rw-r--r--   0        0        0     5645 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/db/base.py
+-rw-r--r--   0        0        0     6959 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/db/explorer.py
+-rw-r--r--   0        0        0      642 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/db/output_presets.yml
+-rw-r--r--   0        0        0    29264 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/db/preprocessing.py
+-rw-r--r--   0        0        0     7264 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/db/schema.py
+-rw-r--r--   0        0        0     4906 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/db/utils.py
+-rw-r--r--   0        0        0     1749 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/helpers.py
+-rw-r--r--   0        0        0      344 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/resources/__init__.py
+-rw-r--r--   0        0        0    17273 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/resources/computing.py
+-rw-r--r--   0        0        0     3515 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/resources/context.py
+-rw-r--r--   0        0        0     9145 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/resources/entity.py
+-rw-r--r--   0        0        0     8979 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/resources/feature.py
+-rw-r--r--   0        0        0     2353 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/resources/group.py
+-rw-r--r--   0        0        0     3662 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/resources/logger.py
+-rw-r--r--   0        0        0    10497 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/resources/model.py
+-rw-r--r--   0        0        0     2528 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/routes.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/sample_applications/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/sample_applications/housing/__init__.py
+-rw-r--r--   0        0        0     1195 2024-04-26 13:53:05.407081 sibyl_api-0.1.1/sibyl/sample_applications/housing/context_config.yml
+-rw-r--r--   0        0        0     4894 2024-04-26 13:53:05.411081 sibyl_api-0.1.1/sibyl/sample_applications/housing/features.csv
+-rw-r--r--   0        0        0     1249 2024-04-26 13:53:05.411081 sibyl_api-0.1.1/sibyl/sample_applications/housing/prepare_db.py
+-rw-r--r--   0        0        0     1471 2024-04-26 13:53:05.411081 sibyl_api-0.1.1/sibyl/sample_applications/housing/prepare_db_config.yml
+-rw-r--r--   0        0        0     7352 2024-04-26 13:53:05.411081 sibyl_api-0.1.1/sibyl/swagger.py
+-rw-r--r--   0        0        0     1646 2024-04-26 13:53:05.411081 sibyl_api-0.1.1/sibyl/templates/context_config_template.yml
+-rw-r--r--   0        0        0     2188 2024-04-26 13:53:05.411081 sibyl_api-0.1.1/sibyl/templates/prepare_db_config_template.yml
+-rw-r--r--   0        0        0     3486 2024-04-26 13:53:05.411081 sibyl_api-0.1.1/sibyl/utils.py
+-rw-r--r--   0        0        0     9951 1970-01-01 00:00:00.000000 sibyl_api-0.1.1/PKG-INFO
```

### Comparing `sibyl_api-0.1.0.2/LICENSE` & `sibyl_api-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/README.md` & `sibyl_api-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 <p align="left">
 <img width=15% src="https://dai.lids.mit.edu/wp-content/uploads/2018/06/Logo_DAI_highres.png" alt=“DAI-Lab” />
 <i>An open source project from Data to AI Lab at MIT.</i>
 </p>
 
-<!-- Uncomment these lines after releasing the package to PyPI for version and downloads badges -->
-<!--[![PyPI Shield](https://img.shields.io/pypi/v/sibylapp.svg)](https://pypi.python.org/pypi/sibylapp)-->
-<!--[![Downloads](https://pepy.tech/badge/sibylapp)](https://pepy.tech/project/sibylapp)-->
-
-[![Travis CI Shield](https://travis-ci.org/HDI-Project/sibylapp.svg?branch=master)](https://travis-ci.org/HDI-Project/sibylapp)
-[![Coverage Status](https://codecov.io/gh/HDI-Project/sibylapp/branch/master/graph/badge.svg)](https://codecov.io/gh/HDI-Project/sibylapp)
+[![PyPI - Version](https://img.shields.io/pypi/v/sibyl-api)](https://pypi.org/project/sibyl-api/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sibyl-api)](https://pypi.org/project/sibyl-api/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/sibyl-api)](https://pypi.org/project/sibyl-api/)
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/sibyl-dev/sibyl-api/python-test.yml)](https://github.com/sibyl-dev/sibyl-api/actions/workflows/python-test.yml)
+[![Static Badge](https://img.shields.io/badge/slack-sibyl-purple?logo=slack)](https://join.slack.com/t/sibyl-ml/shared_invite/zt-2dyfwbgo7-2ALinuT2KDZpsVJ4rntJuA)
 
 # Sibyl-API
 
-APIs for explainable ML.
+REST-API endpoints for understanding and interacting with ML models. 
 
--   API Documentation: [https://sibyl-ml.dev/sibyl-api/](https://sibyl-ml.dev/sibyl-api/)
+| Important Links                               |                                                                      |
+| --------------------------------------------- | -------------------------------------------------------------------- |
+| :book: **[Documentation]**                    | Quickstart and user guides                                           |
+| :memo: **[API Reference]**                    | Endpoint usage and details                                           |
+| :scroll: **[License]**                        | The repository is published under the MIT License.                   |
+| :computer: **[Website]**                      | Check out the Sibyl Project Website for more information.            |
+
+[Website]: https://sibyl-ml.dev/
+[Documentation]: https://dtail.gitbook.io/sibyl/
+[License]: https://github.com/sibyl-dev/sibyl-api/blob/dev/LICENSE
+[Community]: https://join.slack.com/t/sibyl-ml/shared_invite/zt-2dyfwbgo7-2ALinuT2KDZpsVJ4rntJuA
+[API Reference]: https://sibyl-ml.dev/sibyl-api/
 
 # Overview
 
-Interpretability is perhaps most impactful in situations where humans make decisions with input from amachine learning model. In such situations, humans have traditionally made decisions without ML models, and as such use the ML model predictions as an aideto improve their effectiveness or speed.
-In these cases, explanations can serve many functions. They may help build user trust in the model, identify possible mistakes in the model’s prediction, expedite decisionmaking, maintain accountability, validate their hypotheses, or satisfy curiosity.
+Sibyl-API offers API endpoints for easy-to-understand ML model explanations and smooth interactions. 
 
-Sibylapp is an online interactive tool built on the top of Sibyl (python library) to provide explanations to predictive models on tabular data.
+To get started with Sibyl-API, follow the instructions below or in our documentation to setup your Sibyl database. From there, 
+you can easily make model predictions, get and modify information about model features, and get a variety of explanations
+about your models and their predictions.
 
 # Install
 
 ## Requirements
 
-**Sibyl-API** has been developed and tested on [Python 3.9, 3.10, and 3.11](https://www.python.org/downloads/), and on [MongoDB version 6 and 7](https://www.mongodb.com/try/download/community).
+**Sibyl-API** requires [MongoDB version 6 or 7](https://www.mongodb.com/try/download/community).
 
 To install MongoDB, follow the instructions
 [here](https://www.mongodb.com/docs/manual/administration/install-community/).
 
 ## Install from PyPi
 
 Sibyl-API can be installed from pypi:
@@ -111,21 +122,22 @@
 
 | `feature` | `type` | `description`        | `negative_description`         | `values`                    |
 |-----------|--------|----------------------|--------------------------------|-----------------------------|
 | size      | numerical | size in square feet  |                                |                             |
 | has_ac    | boolean | has air conditioning | does not have air conditioning |                             |
 | nghbrh    | categorical | neighborhood         |                                | [Oceanview, Ridge, Oakvale] |
 
-**realapp**: A pickled `pyreal.RealApp` object. This object is used to generate explanations for the model.
+**realapp**: A pickled `pyreal.RealApp` object. This object is used to generate explanations for the model. 
+See [the pyreal documentation](https://dtail.gitbook.io/pyreal/) for details on setting this up.
 
 ### Optional inputs
 Additionally, you can configure APIs futher with:
 
 **config**: a configuration file (YAML or python dictionary) specifying
-additional settings. See `sibyl/db/config_template.yml` for options.
+additional settings. See our [config documentation](https://dtail.gitbook.io/sibyl/user-guides/preparing-the-database/configuring-applications) for details.
 
 **categories**: a table with the categories used to make predictions. Each row should correspond to a single category.
 
 Columns:
   - `category` (*required*): the name of the category
   - `description`: a description of the category
   - `color`: color to use for the category
@@ -171,32 +183,9 @@
 
 sibyl run -E development -v -D [DATABASE_NAME]
 ```
 
 You can then access your APIs locally at http://localhost:3000/apidocs
 
 # Contributing Guide
-We appreciate contributions of all kinds! To contribute code to the repo please follow these steps:
-1. Clone and install the library and load in your test database(s) following the instructions above.
-2. Make a new branch off of `dev` with a descriptive name describing your change.
-3. Make changes to that branch, committing and pushing code as you go.
-4. Run the following commands to ensure your code passed required code style guidelines and tests:
-```
-# Run all tests
-poetry run invoke test
-
-# Run unit tests only
-poetry run invoke test-unit
-
-# Fix most linting errors
-poetry run invoke fix-lint
+We appreciate contributions of all kinds! See [our contributing guide](https://dtail.gitbook.io/sibyl/developer-guides/contributing-to-sibyl) for instructions.
 
-# Ensure no linting errors remain
-poetry run invoke lint
-```
-5. You can manually run `sibyl/test_apis_on_database.ipynb` on your database(s) to test further.
-6. Before making a PR with your final changes, update the api docs by running Sibyl with the -G flag, ie.
-```
-# Generate docs
-poetry run sibyl run -G
-```
-8. Once all tests/linting pass, push all code and make a pull request. One all checks pass and the PR has been approved, merge your code and delete the branch.
```

### Comparing `sibyl_api-0.1.0.2/pyproject.toml` & `sibyl_api-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 authors = ["MIT Data To AI Lab"]
 description = "Explanation tool for machine learning"
 license = "MIT"
 name = "sibyl-api"
 packages = [{include = "sibyl"}]
 readme = "README.md"
-version = "0.1.0.2"
+version = "0.1.1"
 
 repository = "https://github.com/DAI-Lab/sibyl-api"
 
 keywords = ["sibyl-api", "sibyl", "api"]
 
 classifiers = [
   'Development Status :: 2 - Pre-Alpha',
```

### Comparing `sibyl_api-0.1.0.2/sibyl/cli.py` & `sibyl_api-0.1.1/sibyl/cli.py`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/config.yml` & `sibyl_api-0.1.1/sibyl/config.yml`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/core.py` & `sibyl_api-0.1.1/sibyl/core.py`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/data.py` & `sibyl_api-0.1.1/sibyl/data.py`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/db/__init__.py` & `sibyl_api-0.1.1/sibyl/db/__init__.py`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/db/base.py` & `sibyl_api-0.1.1/sibyl/db/base.py`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/db/explorer.py` & `sibyl_api-0.1.1/sibyl/db/explorer.py`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/db/output_presets.yml` & `sibyl_api-0.1.1/sibyl/db/output_presets.yml`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/db/preprocessing.py` & `sibyl_api-0.1.1/sibyl/db/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/db/schema.py` & `sibyl_api-0.1.1/sibyl/db/schema.py`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/db/utils.py` & `sibyl_api-0.1.1/sibyl/db/utils.py`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/helpers.py` & `sibyl_api-0.1.1/sibyl/helpers.py`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/resources/computing.py` & `sibyl_api-0.1.1/sibyl/resources/computing.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,16 +131,15 @@
         entities = [dict(entity_dict[row_id], **{"eid": row_id}) for row_id in entity_dict]
     return pd.DataFrame(entities)
 
 
 class SingleChangePredictions(Resource):
     def post(self):
         """
-        Get the resulting model predictions after changing the value of a single feature
-        of an entity for each feature-value pair provided in the request.
+        Change one feature value at a time and get the resulting model predictions.
         ---
         tags:
           - computing
         requestBody:
            required: true
            content:
              application/json:
```

### Comparing `sibyl_api-0.1.0.2/sibyl/resources/context.py` & `sibyl_api-0.1.1/sibyl/resources/context.py`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/resources/entity.py` & `sibyl_api-0.1.1/sibyl/resources/entity.py`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/resources/feature.py` & `sibyl_api-0.1.1/sibyl/resources/feature.py`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/resources/group.py` & `sibyl_api-0.1.1/sibyl/resources/group.py`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/resources/logger.py` & `sibyl_api-0.1.1/sibyl/resources/logger.py`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/resources/model.py` & `sibyl_api-0.1.1/sibyl/resources/model.py`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/routes.py` & `sibyl_api-0.1.1/sibyl/routes.py`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/sample_applications/housing/context_config.yml` & `sibyl_api-0.1.1/sibyl/sample_applications/housing/context_config.yml`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/sample_applications/housing/features.csv` & `sibyl_api-0.1.1/sibyl/sample_applications/housing/features.csv`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/sample_applications/housing/prepare_db.py` & `sibyl_api-0.1.1/sibyl/sample_applications/housing/prepare_db.py`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/sample_applications/housing/prepare_db_config.yml` & `sibyl_api-0.1.1/sibyl/sample_applications/housing/prepare_db_config.yml`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/swagger.py` & `sibyl_api-0.1.1/sibyl/swagger.py`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/templates/context_config_template.yml` & `sibyl_api-0.1.1/sibyl/templates/context_config_template.yml`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/templates/prepare_db_config_template.yml` & `sibyl_api-0.1.1/sibyl/templates/prepare_db_config_template.yml`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/sibyl/utils.py` & `sibyl_api-0.1.1/sibyl/utils.py`

 * *Files identical despite different names*

### Comparing `sibyl_api-0.1.0.2/PKG-INFO` & `sibyl_api-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sibyl-api
-Version: 0.1.0.2
+Version: 0.1.1
 Summary: Explanation tool for machine learning
 Home-page: https://github.com/DAI-Lab/sibyl-api
 License: MIT
 Keywords: sibyl-api,sibyl,api
 Author: MIT Data To AI Lab
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -41,39 +41,50 @@
 Description-Content-Type: text/markdown
 
 <p align="left">
 <img width=15% src="https://dai.lids.mit.edu/wp-content/uploads/2018/06/Logo_DAI_highres.png" alt=“DAI-Lab” />
 <i>An open source project from Data to AI Lab at MIT.</i>
 </p>
 
-<!-- Uncomment these lines after releasing the package to PyPI for version and downloads badges -->
-<!--[![PyPI Shield](https://img.shields.io/pypi/v/sibylapp.svg)](https://pypi.python.org/pypi/sibylapp)-->
-<!--[![Downloads](https://pepy.tech/badge/sibylapp)](https://pepy.tech/project/sibylapp)-->
-
-[![Travis CI Shield](https://travis-ci.org/HDI-Project/sibylapp.svg?branch=master)](https://travis-ci.org/HDI-Project/sibylapp)
-[![Coverage Status](https://codecov.io/gh/HDI-Project/sibylapp/branch/master/graph/badge.svg)](https://codecov.io/gh/HDI-Project/sibylapp)
+[![PyPI - Version](https://img.shields.io/pypi/v/sibyl-api)](https://pypi.org/project/sibyl-api/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sibyl-api)](https://pypi.org/project/sibyl-api/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/sibyl-api)](https://pypi.org/project/sibyl-api/)
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/sibyl-dev/sibyl-api/python-test.yml)](https://github.com/sibyl-dev/sibyl-api/actions/workflows/python-test.yml)
+[![Static Badge](https://img.shields.io/badge/slack-sibyl-purple?logo=slack)](https://join.slack.com/t/sibyl-ml/shared_invite/zt-2dyfwbgo7-2ALinuT2KDZpsVJ4rntJuA)
 
 # Sibyl-API
 
-APIs for explainable ML.
+REST-API endpoints for understanding and interacting with ML models. 
 
--   API Documentation: [https://sibyl-ml.dev/sibyl-api/](https://sibyl-ml.dev/sibyl-api/)
+| Important Links                               |                                                                      |
+| --------------------------------------------- | -------------------------------------------------------------------- |
+| :book: **[Documentation]**                    | Quickstart and user guides                                           |
+| :memo: **[API Reference]**                    | Endpoint usage and details                                           |
+| :scroll: **[License]**                        | The repository is published under the MIT License.                   |
+| :computer: **[Website]**                      | Check out the Sibyl Project Website for more information.            |
+
+[Website]: https://sibyl-ml.dev/
+[Documentation]: https://dtail.gitbook.io/sibyl/
+[License]: https://github.com/sibyl-dev/sibyl-api/blob/dev/LICENSE
+[Community]: https://join.slack.com/t/sibyl-ml/shared_invite/zt-2dyfwbgo7-2ALinuT2KDZpsVJ4rntJuA
+[API Reference]: https://sibyl-ml.dev/sibyl-api/
 
 # Overview
 
-Interpretability is perhaps most impactful in situations where humans make decisions with input from amachine learning model. In such situations, humans have traditionally made decisions without ML models, and as such use the ML model predictions as an aideto improve their effectiveness or speed.
-In these cases, explanations can serve many functions. They may help build user trust in the model, identify possible mistakes in the model’s prediction, expedite decisionmaking, maintain accountability, validate their hypotheses, or satisfy curiosity.
+Sibyl-API offers API endpoints for easy-to-understand ML model explanations and smooth interactions. 
 
-Sibylapp is an online interactive tool built on the top of Sibyl (python library) to provide explanations to predictive models on tabular data.
+To get started with Sibyl-API, follow the instructions below or in our documentation to setup your Sibyl database. From there, 
+you can easily make model predictions, get and modify information about model features, and get a variety of explanations
+about your models and their predictions.
 
 # Install
 
 ## Requirements
 
-**Sibyl-API** has been developed and tested on [Python 3.9, 3.10, and 3.11](https://www.python.org/downloads/), and on [MongoDB version 6 and 7](https://www.mongodb.com/try/download/community).
+**Sibyl-API** requires [MongoDB version 6 or 7](https://www.mongodb.com/try/download/community).
 
 To install MongoDB, follow the instructions
 [here](https://www.mongodb.com/docs/manual/administration/install-community/).
 
 ## Install from PyPi
 
 Sibyl-API can be installed from pypi:
@@ -153,21 +164,22 @@
 
 | `feature` | `type` | `description`        | `negative_description`         | `values`                    |
 |-----------|--------|----------------------|--------------------------------|-----------------------------|
 | size      | numerical | size in square feet  |                                |                             |
 | has_ac    | boolean | has air conditioning | does not have air conditioning |                             |
 | nghbrh    | categorical | neighborhood         |                                | [Oceanview, Ridge, Oakvale] |
 
-**realapp**: A pickled `pyreal.RealApp` object. This object is used to generate explanations for the model.
+**realapp**: A pickled `pyreal.RealApp` object. This object is used to generate explanations for the model. 
+See [the pyreal documentation](https://dtail.gitbook.io/pyreal/) for details on setting this up.
 
 ### Optional inputs
 Additionally, you can configure APIs futher with:
 
 **config**: a configuration file (YAML or python dictionary) specifying
-additional settings. See `sibyl/db/config_template.yml` for options.
+additional settings. See our [config documentation](https://dtail.gitbook.io/sibyl/user-guides/preparing-the-database/configuring-applications) for details.
 
 **categories**: a table with the categories used to make predictions. Each row should correspond to a single category.
 
 Columns:
   - `category` (*required*): the name of the category
   - `description`: a description of the category
   - `color`: color to use for the category
@@ -213,33 +225,10 @@
 
 sibyl run -E development -v -D [DATABASE_NAME]
 ```
 
 You can then access your APIs locally at http://localhost:3000/apidocs
 
 # Contributing Guide
-We appreciate contributions of all kinds! To contribute code to the repo please follow these steps:
-1. Clone and install the library and load in your test database(s) following the instructions above.
-2. Make a new branch off of `dev` with a descriptive name describing your change.
-3. Make changes to that branch, committing and pushing code as you go.
-4. Run the following commands to ensure your code passed required code style guidelines and tests:
-```
-# Run all tests
-poetry run invoke test
-
-# Run unit tests only
-poetry run invoke test-unit
-
-# Fix most linting errors
-poetry run invoke fix-lint
+We appreciate contributions of all kinds! See [our contributing guide](https://dtail.gitbook.io/sibyl/developer-guides/contributing-to-sibyl) for instructions.
 
-# Ensure no linting errors remain
-poetry run invoke lint
-```
-5. You can manually run `sibyl/test_apis_on_database.ipynb` on your database(s) to test further.
-6. Before making a PR with your final changes, update the api docs by running Sibyl with the -G flag, ie.
-```
-# Generate docs
-poetry run sibyl run -G
-```
-8. Once all tests/linting pass, push all code and make a pull request. One all checks pass and the PR has been approved, merge your code and delete the branch.
```

