# Comparing `tmp/omicidx-1.6.5.tar.gz` & `tmp/omicidx-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omicidx-1.6.5.tar", max compression
+gzip compressed data, was "omicidx-1.7.0.tar", max compression
```

## Comparing `omicidx-1.6.5.tar` & `omicidx-1.7.0.tar`

### file list

```diff
@@ -1,25 +1,23 @@
--rw-r--r--   0        0        0        0 2021-10-07 20:33:57.811472 omicidx-1.6.5/README.md
--rw-r--r--   0        0        0     9854 2022-06-12 18:49:26.440659 omicidx-1.6.5/omicidx/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0    47492 2022-06-12 20:15:47.493331 omicidx-1.6.5/omicidx/Untitled.ipynb
--rw-r--r--   0        0        0       19 2021-08-23 17:51:36.154366 omicidx-1.6.5/omicidx/__init__.py
--rw-r--r--   0        0        0     7776 2023-01-27 03:30:55.774356 omicidx-1.6.5/omicidx/biosample.py
--rw-r--r--   0        0        0        0 2021-08-23 17:51:36.154811 omicidx-1.6.5/omicidx/geo/__init__.py
--rw-r--r--   0        0        0    19679 2023-03-07 00:18:08.201457 omicidx-1.6.5/omicidx/geo/parser.py
--rw-r--r--   0        0        0     3136 2022-01-26 10:49:37.308533 omicidx-1.6.5/omicidx/geo/pydantic_models.py
--rw-r--r--   0        0        0     2080 2022-05-21 02:59:44.471856 omicidx-1.6.5/omicidx/geo/webutils.py
--rw-r--r--   0        0        0        0 2021-08-23 17:51:36.155471 omicidx-1.6.5/omicidx/ontologies/__init__.py
--rw-r--r--   0        0        0      500 2022-02-10 04:34:44.040798 omicidx-1.6.5/omicidx/ontologies/test_ontology_utils.py
--rw-r--r--   0        0        0     1414 2021-08-23 17:51:36.155639 omicidx-1.6.5/omicidx/ontologies/utils.py
--rw-r--r--   0        0        0     4765 2021-08-23 17:51:36.156769 omicidx-1.6.5/omicidx/schema_tools.py
--rw-r--r--   0        0        0        2 2021-08-23 17:51:36.156881 omicidx-1.6.5/omicidx/scripts/__init__.py
--rw-r--r--   0        0        0     5725 2022-08-15 18:06:45.378444 omicidx-1.6.5/omicidx/scripts/cli.py
--rw-r--r--   0        0        0     1718 2022-08-12 23:24:56.234628 omicidx-1.6.5/omicidx/scripts/geo.py
--rwxr-xr-x   0        0        0     2037 2021-08-23 17:51:36.157205 omicidx-1.6.5/omicidx/scripts/sra_entity_to_json.py
--rw-r--r--   0        0        0        0 2021-08-23 17:51:36.157285 omicidx-1.6.5/omicidx/sra/__init__.py
--rw-r--r--   0        0        0     1729 2022-08-12 22:49:32.996554 omicidx-1.6.5/omicidx/sra/ebiutils.py
--rw-r--r--   0        0        0    35506 2022-12-12 14:55:40.313193 omicidx-1.6.5/omicidx/sra/parser.py
--rw-r--r--   0        0        0     3790 2022-11-03 14:53:38.255750 omicidx-1.6.5/omicidx/sra/pydantic_models.py
--rw-r--r--   0        0        0     1972 2021-08-23 17:51:36.157816 omicidx-1.6.5/omicidx/utils.py
--rw-r--r--   0        0        0     1471 2023-03-07 00:18:21.251536 omicidx-1.6.5/pyproject.toml
--rw-r--r--   0        0        0     1364 1970-01-01 00:00:00.000000 omicidx-1.6.5/setup.py
--rw-r--r--   0        0        0     1320 1970-01-01 00:00:00.000000 omicidx-1.6.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2021-10-07 20:33:57.811472 omicidx-1.7.0/README.md
+-rw-r--r--   0        0        0     9854 2022-06-12 18:49:26.440659 omicidx-1.7.0/omicidx/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0    47492 2022-06-12 20:15:47.493331 omicidx-1.7.0/omicidx/Untitled.ipynb
+-rw-r--r--   0        0        0       19 2021-08-23 17:51:36.154366 omicidx-1.7.0/omicidx/__init__.py
+-rw-r--r--   0        0        0     7776 2023-01-27 03:30:55.774356 omicidx-1.7.0/omicidx/biosample.py
+-rw-r--r--   0        0        0        0 2021-08-23 17:51:36.154811 omicidx-1.7.0/omicidx/geo/__init__.py
+-rw-r--r--   0        0        0    19679 2023-03-07 00:18:08.201457 omicidx-1.7.0/omicidx/geo/parser.py
+-rw-r--r--   0        0        0     3162 2023-07-18 13:00:36.912904 omicidx-1.7.0/omicidx/geo/pydantic_models.py
+-rw-r--r--   0        0        0     2080 2022-05-21 02:59:44.471856 omicidx-1.7.0/omicidx/geo/webutils.py
+-rw-r--r--   0        0        0        0 2021-08-23 17:51:36.155471 omicidx-1.7.0/omicidx/ontologies/__init__.py
+-rw-r--r--   0        0        0     1414 2021-08-23 17:51:36.155639 omicidx-1.7.0/omicidx/ontologies/utils.py
+-rw-r--r--   0        0        0     4765 2021-08-23 17:51:36.156769 omicidx-1.7.0/omicidx/schema_tools.py
+-rw-r--r--   0        0        0        2 2021-08-23 17:51:36.156881 omicidx-1.7.0/omicidx/scripts/__init__.py
+-rw-r--r--   0        0        0     5725 2022-08-15 18:06:45.378444 omicidx-1.7.0/omicidx/scripts/cli.py
+-rw-r--r--   0        0        0     1718 2022-08-12 23:24:56.234628 omicidx-1.7.0/omicidx/scripts/geo.py
+-rwxr-xr-x   0        0        0     2037 2021-08-23 17:51:36.157205 omicidx-1.7.0/omicidx/scripts/sra_entity_to_json.py
+-rw-r--r--   0        0        0        0 2021-08-23 17:51:36.157285 omicidx-1.7.0/omicidx/sra/__init__.py
+-rw-r--r--   0        0        0     1729 2022-08-12 22:49:32.996554 omicidx-1.7.0/omicidx/sra/ebiutils.py
+-rw-r--r--   0        0        0    35506 2022-12-12 14:55:40.313193 omicidx-1.7.0/omicidx/sra/parser.py
+-rw-r--r--   0        0        0     4375 2023-07-18 12:55:16.533067 omicidx-1.7.0/omicidx/sra/pydantic_models.py
+-rw-r--r--   0        0        0     1972 2021-08-23 17:51:36.157816 omicidx-1.7.0/omicidx/utils.py
+-rw-r--r--   0        0        0     1563 2023-07-18 13:16:19.708691 omicidx-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1535 1970-01-01 00:00:00.000000 omicidx-1.7.0/PKG-INFO
```

### Comparing `omicidx-1.6.5/omicidx/.ipynb_checkpoints/Untitled-checkpoint.ipynb` & `omicidx-1.7.0/omicidx/.ipynb_checkpoints/Untitled-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `omicidx-1.6.5/omicidx/Untitled.ipynb` & `omicidx-1.7.0/omicidx/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `omicidx-1.6.5/omicidx/biosample.py` & `omicidx-1.7.0/omicidx/biosample.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.6.5/omicidx/geo/parser.py` & `omicidx-1.7.0/omicidx/geo/parser.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.6.5/omicidx/geo/webutils.py` & `omicidx-1.7.0/omicidx/geo/webutils.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.6.5/omicidx/ontologies/utils.py` & `omicidx-1.7.0/omicidx/ontologies/utils.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.6.5/omicidx/schema_tools.py` & `omicidx-1.7.0/omicidx/schema_tools.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.6.5/omicidx/scripts/cli.py` & `omicidx-1.7.0/omicidx/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.6.5/omicidx/scripts/geo.py` & `omicidx-1.7.0/omicidx/scripts/geo.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.6.5/omicidx/scripts/sra_entity_to_json.py` & `omicidx-1.7.0/omicidx/scripts/sra_entity_to_json.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.6.5/omicidx/sra/ebiutils.py` & `omicidx-1.7.0/omicidx/sra/ebiutils.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.6.5/omicidx/sra/parser.py` & `omicidx-1.7.0/omicidx/sra/parser.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.6.5/omicidx/sra/pydantic_models.py` & `omicidx-1.7.0/omicidx/geo/pydantic_models.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,167 +1,117 @@
 import pydantic
-from pydantic import BaseModel
+from pydantic import (BaseModel, constr)
 import json
-from datetime import datetime
-from typing import List, Dict, Optional
+from datetime import datetime, date
+from typing import List, Dict
 
 
-class Attribute(BaseModel):
-    tag: str = None
-    value: str = None
-
-
-class Xref(BaseModel):
-    db: str = None
-    id: str = None
-
-
-class Identifier(BaseModel):
-    namespace: str = None
-    id: str = None
-
-
-class FileAlternative(BaseModel):
-    url: str = None
-    free_egress: str = None
-    access_type: str = None
-    org: str = None
-
-
-class FileSet(BaseModel):
-    cluster: str = "public"
-    filename: str = None
-    url: str = None
-    size: int = 0
-    date: datetime = None
-    md5: str = None
-    sratoolkit: str = "1"
-    alternatives: List[FileAlternative]
-
-
-class BaseQualityCount(BaseModel):
-    quality: int = 0
-    count: int = 0
-
-
-class BaseQualities(List[BaseQualityCount]):
-    pass
-
-
-class TaxCountEntry(BaseModel):
-    rank: str = None
-    name: str = None
-    parent: int = None
-    total_count: int = 0
-    self_count: int = 0
-    tax_id: int
-
-
-class TaxCountAnalysis(BaseModel):
-    nspot_analyze: int = None
-    total_spots: int = None
-    mapped_spots: int = None
-    tax_counts: List[TaxCountEntry] = None
-
-
-class RunRead(BaseModel):
-    index: int
-    count: int
-    mean_length: float = 0.0
-    sd_length: float = 0.0
-
-
-class BaseCounts(List[Dict[str, int]]):
-    pass
-
-
-class LiveList(BaseModel):
-    lastupdate: datetime = None
-    published: datetime = None
-    received: datetime = None
-    status: str = "live"
-    insdc: bool = True
-
-
-class SraRun(LiveList, BaseModel):
-    alias: str = None
-    run_date: datetime = None
-    run_center: str = None
-    center_name: str = None
-    accession: str
-    total_spots: int = 0
-    total_bases: int = 0
-    size: int = 0
-    load_done: bool = True
-    published: datetime = None
-    is_public: bool = True
-    cluster_name: str = "public"
-    static_data_available: str = "1"
-    avg_length: float = 0.0
-    experiment_accession: str
-    attributes: List[Attribute] = None
-    files: List[FileSet] = None
-    qualities: BaseQualities = None
-    base_counts: BaseCounts = None
-    reads: List[RunRead] = None
-    tax_analysis: TaxCountAnalysis = None
-
-
-class SraStudy(LiveList, BaseModel):
-    abstract: str = None
-    BioProject: str = None
-    Geo: str = None
-    accession: str
-    alias: str = None
-    center_name: str = None
-    broker_name: str = None
+class GEOBase(BaseModel):
+    title: str
+    status: str
+    submission_date: date = None
+    last_update_date: date = None
+
+
+class GEOName(BaseModel):
+    first: str = None
+    middle: str = None
+    last: str = None
+
+
+class GEOContact(BaseModel):
+    city: str = None
+    name: GEOName = None
+    email: str = None
+    state: str = None
+    address: str = None
+    department: str = None
+    country: str = None
+    web_link: str = None
+    institute: str = None
+    zip_postal_code: str = None
+    phone: str = None
+
+
+class GEOPlatform(GEOBase):
+    accession: constr(pattern='GPL\d+')
+    status: str
+    _entity: str = "GPL"
+    contact: GEOContact = None
+    summary: str = None
+    organism: str = None
+    sample_id: List[constr(pattern='GSM\d+')] = []
+    series_id: List[constr(pattern='GSE\d+')] = []
+    technology: str = None
     description: str = None
-    study_type: str = None
-    title: str = None
-    identifiers: List[Identifier] = None
-    attributes: List[Attribute] = None
-    pubmed_ids: List[int] = None
+    distribution: str = None
+    manufacturer: List[str] = []
+    data_row_count: int = None
+    contributor: List[GEOName] = []
+    relation: List[str] = []
+    manufacture_protocol: str = None
+
+
+class GEOCharacteristic(BaseModel):
+    tag: str
+    value: str = None  # there are apparently some of these
+
+
+class GEOChannel(BaseModel):
+    label: str = None
+    taxid: List[int] = []
+    molecule: str = None
+    organism: str = None
+    source_name: str = None
+    label_protocol: str = None
+    growth_protocol: str = None
+    extract_protocol: str = None
+    treatment_protocol: str = None
+    characteristics: List[GEOCharacteristic] = []
 
 
-class SraExperiment(LiveList, BaseModel):
-    accession: str
-    attributes: List[Attribute] = None
-    alias: str = None
-    center_name: str = None
-    design: str = None
+class GEOSample(GEOBase):
+    type: str
+    anchor: str = None
+    _entity: None
+    contact: GEOContact = None
     description: str = None
-    identifiers: List[Identifier] = None
-    instrument_model: str = None
-    library_name: str = None
-    library_construction_protocol: str = None
-    library_layout_orientation: str = None
-    library_layout_length: float = None
-    library_layout_sdev: float = None
-    library_strategy: str = None
+    accession: constr(pattern='GSM\d+')
+    biosample: constr(pattern='SAM[A-Z]+\d+') = None
+    tag_count: int = None
+    tag_length: float = None
+    platform_id: constr(pattern='GPL\d+')
+    hyb_protocol: str = None
+    channel_count: int = 0
+    scan_protocol: str = None
+    data_row_count: int = 0
     library_source: str = None
-    library_selection: str = None
-    library_layout: str = None
-    xrefs: List[Xref] = None
-    platform: str = None
-    sample_accession: str = None
-    study_accession: str = None
-    title: str = None
-
-
-class SraSample(LiveList, BaseModel):
-    accession: str
-    geo: str = None
-    BioSample: str = None
-    title: str = None
-    alias: str = None
-    organism: str = None
-    taxon_id: int = None
+    overall_design: str = None
+    sra_experiment: constr(pattern='[DES]RX\d+') = None
+    data_processing: str = None
+    supplemental_files: List[str] = []
+    channels: List[GEOChannel] = []
+    contributor: List[GEOName] = []
+
+
+class GEOSeries(GEOBase):
+    accession: constr(pattern='GSE\d+')
+    subseries: List[constr(pattern='GSE\d+')] = []
+    bioprojects: List[constr(pattern='PRJ[A-Z]+\d+')] = []
+    sra_studies: List[constr(pattern='[ESD]RP\d+')] = []
+    _entity: str = "GSE"
+    contact: GEOContact = None
+    type: List[str] = []
+    summary: str = None
+    relation: List[str] = []
+    pubmed_id: List[int] = []
+    sample_id: List[constr(pattern='GSM\d+')]=[]
+    sample_taxid: List[int] = []
+    sample_organism: List[str] = []
+    platform_id: List[constr(pattern='GPL\d+')]=[]
+    platform_taxid: List[int] = []
+    platform_organism: List[str] = []
+    data_processing: str = None
     description: str = None
-    identifiers: List[Identifier] = None
-    attributes: List[Attribute] = None
-    xrefs: List[Xref] = None
-
-
-class FullSraRun(SraRun):
-    experiment: Optional[SraExperiment] = None
-    sample: Optional[SraSample] = None
-    study: Optional[SraStudy] = None
+    supplemental_files: List[str] = []
+    overall_design: str = None
+    contributor: List[GEOName] = []
```

### Comparing `omicidx-1.6.5/omicidx/utils.py` & `omicidx-1.7.0/omicidx/utils.py`

 * *Files identical despite different names*

### Comparing `omicidx-1.6.5/pyproject.toml` & `omicidx-1.7.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 [tool.dephell.main]
 from = {format = "poetry", path = "pyproject.toml"}
 to = {format = "setuppy", path = "setup.py"}
 
 [tool.poetry]
 name = "omicidx"
-version = "1.6.5"
+version = "1.7.0"
 readme = "README.md"
 description = """The OmicIDX project collects, reprocesses, and then republishes metadata from multiple public genomics repositories. Included are the NCBI SRA, Biosample, and GEO databases. Publication is via the cloud data warehouse platform Bigquery, a set of performant search and retrieval APIs, and a set of json-format files for easy incorporation into other projects."""
 authors = ["Sean Davis <seandavi@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/omicidx/omicidx-parsers"
 keywords = ["genomics", "bioinformatics", "open data", "API"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-pydantic = "*"
 requests = "^2.22"
 Click = "*"
 sd_cloud_utils = "*"
 aiohttp = "^3.6.2"
 tenacity = "^8.0.1"
 pendulum = "^2.1.2"
 httpx = "*"
 trio = "^0.22.0"
+pydantic = "^2.0.3"
+biopython = "^1.81"
+pronto = "^2.5.4"
+orjson = "^3.9.2"
+databases = "^0.7.0"
+pytest = "^7.4.0"
 
 [tool.poetry.dev-dependencies]
-mypy = "^0.720.0"
-pytest = "^5.1"
 rope = "^0.14.0"
-pytest-sugar = "^0.9.2"
-pytest-cov = "^2.8.1"
 yapf = "^0.28.0"
 pydoc-markdown = "^2.0"
 sphinx = "^5.1.0"
 ipython = "^8.0.1"
 black = "^22.6.0"
 sphinx-click = "^4.3.0"
 sphinx-material = {git = "https://github.com/bashtage/sphinx-material", rev = "main"}
 sphinx-autodoc-typehints = "^1.19.2"
 
 [tool.poetry.scripts]
 omicidx_tool = 'omicidx.scripts.geo:cli'
 
+[tool.poetry.group.dev.dependencies]
+mypy = "^1.4.1"
+pytest = "^7.4.0"
+
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

