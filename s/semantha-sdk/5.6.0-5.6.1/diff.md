# Comparing `tmp/semantha_sdk-5.6.0.tar.gz` & `tmp/semantha_sdk-5.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantha_sdk-5.6.0.tar", max compression
+gzip compressed data, was "semantha_sdk-5.6.1.tar", max compression
```

## Comparing `semantha_sdk-5.6.0.tar` & `semantha_sdk-5.6.1.tar`

### file list

```diff
@@ -1,199 +1,199 @@
--rw-r--r--   0        0        0    11545 2022-12-09 10:06:55.386837 semantha_sdk-5.6.0/LICENSE
--rw-r--r--   0        0        0     1618 2023-07-12 16:11:36.552533 semantha_sdk-5.6.0/pyproject.toml
--rw-r--r--   0        0        0    17578 2023-07-12 16:09:09.354313 semantha_sdk-5.6.0/README.md
--rw-r--r--   0        0        0     1288 2023-05-11 17:26:57.327736 semantha_sdk-5.6.0/semantha_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 06:39:31.917641 semantha_sdk-5.6.0/semantha_sdk/api/__init__.py
--rw-r--r--   0        0        0     1681 2023-07-12 16:01:12.009737 semantha_sdk-5.6.0/semantha_sdk/api/answers.py
--rw-r--r--   0        0        0     1004 2023-07-12 16:01:11.925323 semantha_sdk-5.6.0/semantha_sdk/api/bulk.py
--rw-r--r--   0        0        0      839 2023-07-12 16:01:11.928367 semantha_sdk-5.6.0/semantha_sdk/api/bulk_domains.py
--rw-r--r--   0        0        0      817 2023-07-12 16:01:11.961988 semantha_sdk-5.6.0/semantha_sdk/api/bulk_model.py
--rw-r--r--   0        0        0     1792 2023-07-12 16:01:11.949923 semantha_sdk-5.6.0/semantha_sdk/api/bulkdomains_documentclasses.py
--rw-r--r--   0        0        0     1576 2023-07-12 16:01:11.932882 semantha_sdk-5.6.0/semantha_sdk/api/bulkdomains_domain.py
--rw-r--r--   0        0        0     3766 2023-07-12 16:01:11.955987 semantha_sdk-5.6.0/semantha_sdk/api/bulkdomains_referencedocuments.py
--rw-r--r--   0        0        0     3283 2023-07-12 16:01:11.959984 semantha_sdk-5.6.0/semantha_sdk/api/bulkdomains_references.py
--rw-r--r--   0        0        0     1346 2023-07-12 16:01:11.970505 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_boostwords.py
--rw-r--r--   0        0        0      923 2023-07-12 16:01:11.974018 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_class.py
--rw-r--r--   0        0        0     1913 2023-07-12 16:01:11.972507 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_classes.py
--rw-r--r--   0        0        0     1735 2023-07-12 16:01:11.979031 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_dataproperties.py
--rw-r--r--   0        0        0     3018 2023-07-12 16:01:11.967502 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_domain.py
--rw-r--r--   0        0        0      836 2023-07-12 16:01:11.964493 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_domains.py
--rw-r--r--   0        0        0     1662 2023-07-12 16:01:11.982028 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_instances.py
--rw-r--r--   0        0        0     1661 2023-07-12 16:01:11.987149 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_metadata.py
--rw-r--r--   0        0        0     1373 2023-07-12 16:01:11.991675 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_namedentities.py
--rw-r--r--   0        0        0     1603 2023-07-12 16:01:11.994297 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_rules.py
--rw-r--r--   0        0        0     1261 2023-07-12 16:01:11.996205 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_stopwords.py
--rw-r--r--   0        0        0     1322 2023-07-12 16:01:11.997201 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_synonyms.py
--rw-r--r--   0        0        0     1098 2023-07-12 16:01:11.977031 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodelclass_instances.py
--rw-r--r--   0        0        0     1262 2023-07-12 16:01:12.089837 semantha_sdk-5.6.0/semantha_sdk/api/child_extractorclasses.py
--rw-r--r--   0        0        0     5664 2023-07-12 16:01:12.036865 semantha_sdk-5.6.0/semantha_sdk/api/clusters.py
--rw-r--r--   0        0        0     1168 2023-07-12 16:01:11.999201 semantha_sdk-5.6.0/semantha_sdk/api/currentuser.py
--rw-r--r--   0        0        0     1425 2023-07-12 16:01:12.004205 semantha_sdk-5.6.0/semantha_sdk/api/diff.py
--rw-r--r--   0        0        0     4012 2023-07-12 16:01:12.012736 semantha_sdk-5.6.0/semantha_sdk/api/documentannotations.py
--rw-r--r--   0        0        0     1565 2023-07-12 16:01:12.017262 semantha_sdk-5.6.0/semantha_sdk/api/documentclass.py
--rw-r--r--   0        0        0     1997 2023-07-12 16:01:12.015263 semantha_sdk-5.6.0/semantha_sdk/api/documentclasses.py
--rw-r--r--   0        0        0     3464 2023-07-12 16:01:12.019266 semantha_sdk-5.6.0/semantha_sdk/api/documentcomparisons.py
--rw-r--r--   0        0        0     8589 2023-07-12 16:01:12.021795 semantha_sdk-5.6.0/semantha_sdk/api/documents.py
--rw-r--r--   0        0        0     4497 2023-07-12 16:01:12.007737 semantha_sdk-5.6.0/semantha_sdk/api/domain.py
--rw-r--r--   0        0        0     1157 2023-07-12 16:01:12.005736 semantha_sdk-5.6.0/semantha_sdk/api/domains.py
--rw-r--r--   0        0        0      905 2023-07-12 16:01:12.067244 semantha_sdk-5.6.0/semantha_sdk/api/info.py
--rw-r--r--   0        0        0     1757 2023-07-12 16:01:12.068246 semantha_sdk-5.6.0/semantha_sdk/api/languages.py
--rw-r--r--   0        0        0     1595 2023-07-12 16:01:12.070245 semantha_sdk-5.6.0/semantha_sdk/api/model.py
--rw-r--r--   0        0        0     1019 2023-07-12 16:01:12.075763 semantha_sdk-5.6.0/semantha_sdk/api/model_attributes.py
--rw-r--r--   0        0        0     1460 2023-07-12 16:01:12.079763 semantha_sdk-5.6.0/semantha_sdk/api/model_boostword.py
--rw-r--r--   0        0        0     1924 2023-07-12 16:01:12.077767 semantha_sdk-5.6.0/semantha_sdk/api/model_boostwords.py
--rw-r--r--   0        0        0     2088 2023-07-12 16:01:12.081765 semantha_sdk-5.6.0/semantha_sdk/api/model_dataproperties.py
--rw-r--r--   0        0        0     1505 2023-07-12 16:01:12.084812 semantha_sdk-5.6.0/semantha_sdk/api/model_dataproperty.py
--rw-r--r--   0        0        0      840 2023-07-12 16:01:12.071249 semantha_sdk-5.6.0/semantha_sdk/api/model_datatypes.py
--rw-r--r--   0        0        0     5566 2023-07-12 16:01:12.074753 semantha_sdk-5.6.0/semantha_sdk/api/model_domain.py
--rw-r--r--   0        0        0      816 2023-07-12 16:01:12.072249 semantha_sdk-5.6.0/semantha_sdk/api/model_domains.py
--rw-r--r--   0        0        0     1830 2023-07-12 16:01:12.088836 semantha_sdk-5.6.0/semantha_sdk/api/model_extractorclass.py
--rw-r--r--   0        0        0     2487 2023-07-12 16:01:12.086823 semantha_sdk-5.6.0/semantha_sdk/api/model_extractorclasses.py
--rw-r--r--   0        0        0      951 2023-07-12 16:01:12.090831 semantha_sdk-5.6.0/semantha_sdk/api/model_extractors.py
--rw-r--r--   0        0        0     1536 2023-07-12 16:01:12.094343 semantha_sdk-5.6.0/semantha_sdk/api/model_extractortable.py
--rw-r--r--   0        0        0     2103 2023-07-12 16:01:12.092835 semantha_sdk-5.6.0/semantha_sdk/api/model_extractortables.py
--rw-r--r--   0        0        0      855 2023-07-12 16:01:12.128055 semantha_sdk-5.6.0/semantha_sdk/api/model_extractortypes.py
--rw-r--r--   0        0        0      969 2023-07-12 16:01:12.095353 semantha_sdk-5.6.0/semantha_sdk/api/model_formatters.py
--rw-r--r--   0        0        0     1904 2023-07-12 16:01:12.101358 semantha_sdk-5.6.0/semantha_sdk/api/model_metadata.py
--rw-r--r--   0        0        0      852 2023-07-12 16:01:12.129053 semantha_sdk-5.6.0/semantha_sdk/api/model_metadatatypes.py
--rw-r--r--   0        0        0     1970 2023-07-12 16:01:12.104354 semantha_sdk-5.6.0/semantha_sdk/api/model_namedentities.py
--rw-r--r--   0        0        0     1494 2023-07-12 16:01:12.105482 semantha_sdk-5.6.0/semantha_sdk/api/model_namedentity.py
--rw-r--r--   0        0        0      982 2023-07-12 16:01:12.106482 semantha_sdk-5.6.0/semantha_sdk/api/model_objectproperties.py
--rw-r--r--   0        0        0     1441 2023-07-12 16:01:12.102358 semantha_sdk-5.6.0/semantha_sdk/api/model_onemetadata.py
--rw-r--r--   0        0        0     1401 2023-07-12 16:01:12.111486 semantha_sdk-5.6.0/semantha_sdk/api/model_regex.py
--rw-r--r--   0        0        0     1850 2023-07-12 16:01:12.108485 semantha_sdk-5.6.0/semantha_sdk/api/model_regexes.py
--rw-r--r--   0        0        0     1444 2023-07-12 16:01:12.116004 semantha_sdk-5.6.0/semantha_sdk/api/model_relation.py
--rw-r--r--   0        0        0     1902 2023-07-12 16:01:12.113482 semantha_sdk-5.6.0/semantha_sdk/api/model_relations.py
--rw-r--r--   0        0        0     1388 2023-07-12 16:01:12.121535 semantha_sdk-5.6.0/semantha_sdk/api/model_rule.py
--rw-r--r--   0        0        0      999 2023-07-12 16:01:12.118013 semantha_sdk-5.6.0/semantha_sdk/api/model_rulefunctions.py
--rw-r--r--   0        0        0     1962 2023-07-12 16:01:12.119536 semantha_sdk-5.6.0/semantha_sdk/api/model_rules.py
--rw-r--r--   0        0        0     1449 2023-07-12 16:01:12.124045 semantha_sdk-5.6.0/semantha_sdk/api/model_stopword.py
--rw-r--r--   0        0        0     1907 2023-07-12 16:01:12.122533 semantha_sdk-5.6.0/semantha_sdk/api/model_stopwords.py
--rw-r--r--   0        0        0     1430 2023-07-12 16:01:12.127054 semantha_sdk-5.6.0/semantha_sdk/api/model_synonym.py
--rw-r--r--   0        0        0     1882 2023-07-12 16:01:12.126054 semantha_sdk-5.6.0/semantha_sdk/api/model_synonyms.py
--rw-r--r--   0        0        0     1217 2023-07-12 16:01:12.022796 semantha_sdk-5.6.0/semantha_sdk/api/modelclasses.py
--rw-r--r--   0        0        0     3928 2023-07-12 16:01:12.025320 semantha_sdk-5.6.0/semantha_sdk/api/modelinstances.py
--rw-r--r--   0        0        0     1450 2023-07-12 16:01:12.099352 semantha_sdk-5.6.0/semantha_sdk/api/modelont_instance.py
--rw-r--r--   0        0        0     2592 2023-07-12 16:01:12.098353 semantha_sdk-5.6.0/semantha_sdk/api/modelont_instances.py
--rw-r--r--   0        0        0     1663 2023-07-12 16:01:12.038854 semantha_sdk-5.6.0/semantha_sdk/api/namedentities.py
--rw-r--r--   0        0        0     1711 2023-07-12 16:01:12.046376 semantha_sdk-5.6.0/semantha_sdk/api/paragraph.py
--rw-r--r--   0        0        0      792 2023-07-12 16:01:12.044363 semantha_sdk-5.6.0/semantha_sdk/api/paragraphs.py
--rw-r--r--   0        0        0     2267 2023-07-12 16:01:12.042852 semantha_sdk-5.6.0/semantha_sdk/api/referencedocument.py
--rw-r--r--   0        0        0    13183 2023-07-12 16:01:12.031320 semantha_sdk-5.6.0/semantha_sdk/api/referencedocuments.py
--rw-r--r--   0        0        0    22267 2023-07-12 16:01:12.052898 semantha_sdk-5.6.0/semantha_sdk/api/references.py
--rw-r--r--   0        0        0      867 2023-07-12 16:01:12.001202 semantha_sdk-5.6.0/semantha_sdk/api/roles.py
--rw-r--r--   0        0        0     2113 2023-06-29 06:39:31.918640 semantha_sdk-5.6.0/semantha_sdk/api/semantha_api.py
--rw-r--r--   0        0        0      413 2023-06-29 06:39:31.920640 semantha_sdk-5.6.0/semantha_sdk/api/semantha_endpoint.py
--rw-r--r--   0        0        0      967 2023-07-12 16:01:12.050218 semantha_sdk-5.6.0/semantha_sdk/api/sentence.py
--rw-r--r--   0        0        0      786 2023-07-12 16:01:12.047385 semantha_sdk-5.6.0/semantha_sdk/api/sentences.py
--rw-r--r--   0        0        0     1497 2023-07-12 16:01:12.054983 semantha_sdk-5.6.0/semantha_sdk/api/settings.py
--rw-r--r--   0        0        0     5081 2023-07-12 16:01:12.057028 semantha_sdk-5.6.0/semantha_sdk/api/similaritymatrix.py
--rw-r--r--   0        0        0     3934 2023-07-12 16:01:12.058000 semantha_sdk-5.6.0/semantha_sdk/api/similaritymatrix_cluster.py
--rw-r--r--   0        0        0      963 2023-07-12 16:01:12.040852 semantha_sdk-5.6.0/semantha_sdk/api/statistic.py
--rw-r--r--   0        0        0     1207 2023-07-12 16:01:12.060028 semantha_sdk-5.6.0/semantha_sdk/api/summarizations.py
--rw-r--r--   0        0        0      931 2023-07-12 16:01:12.061997 semantha_sdk-5.6.0/semantha_sdk/api/tag.py
--rw-r--r--   0        0        0     1285 2023-07-12 16:01:12.063995 semantha_sdk-5.6.0/semantha_sdk/api/tag_referencedocuments.py
--rw-r--r--   0        0        0     1018 2023-07-12 16:01:12.061028 semantha_sdk-5.6.0/semantha_sdk/api/tags.py
--rw-r--r--   0        0        0     1383 2023-07-12 16:01:12.065238 semantha_sdk-5.6.0/semantha_sdk/api/validation.py
--rw-r--r--   0        0        0     5700 2023-07-12 16:01:12.372308 semantha_sdk-5.6.0/semantha_sdk/model/__init__.py
--rw-r--r--   0        0        0      617 2023-07-12 16:01:12.305463 semantha_sdk-5.6.0/semantha_sdk/model/annotation_cell.py
--rw-r--r--   0        0        0      689 2023-07-12 16:01:12.245293 semantha_sdk-5.6.0/semantha_sdk/model/annotation_page.py
--rw-r--r--   0        0        0      582 2023-07-12 16:01:12.332539 semantha_sdk-5.6.0/semantha_sdk/model/answer.py
--rw-r--r--   0        0        0      548 2023-07-12 16:01:12.282596 semantha_sdk-5.6.0/semantha_sdk/model/answer_reference.py
--rw-r--r--   0        0        0      658 2023-07-12 16:01:12.352331 semantha_sdk-5.6.0/semantha_sdk/model/argument.py
--rw-r--r--   0        0        0      547 2023-07-12 16:01:12.339095 semantha_sdk-5.6.0/semantha_sdk/model/attribute_overview.py
--rw-r--r--   0        0        0      581 2023-07-12 16:01:12.230242 semantha_sdk-5.6.0/semantha_sdk/model/boost_word.py
--rw-r--r--   0        0        0      989 2023-07-12 16:01:12.264429 semantha_sdk-5.6.0/semantha_sdk/model/class_bulk.py
--rw-r--r--   0        0        0      515 2023-07-12 16:01:12.253293 semantha_sdk-5.6.0/semantha_sdk/model/clustered_document.py
--rw-r--r--   0        0        0      717 2023-07-12 16:01:12.319004 semantha_sdk-5.6.0/semantha_sdk/model/clustering_response.py
--rw-r--r--   0        0        0      519 2023-07-12 16:01:12.233237 semantha_sdk-5.6.0/semantha_sdk/model/column.py
--rw-r--r--   0        0        0     1201 2023-07-12 16:01:12.302276 semantha_sdk-5.6.0/semantha_sdk/model/complex_property.py
--rw-r--r--   0        0        0      627 2023-07-12 16:01:12.320004 semantha_sdk-5.6.0/semantha_sdk/model/condition.py
--rw-r--r--   0        0        0      587 2023-07-12 16:01:12.303277 semantha_sdk-5.6.0/semantha_sdk/model/condition_value.py
--rw-r--r--   0        0        0      545 2023-07-12 16:01:12.270379 semantha_sdk-5.6.0/semantha_sdk/model/current_user.py
--rw-r--r--   0        0        0      639 2023-07-12 16:01:12.346320 semantha_sdk-5.6.0/semantha_sdk/model/data_property.py
--rw-r--r--   0        0        0      483 2023-07-12 16:01:12.320998 semantha_sdk-5.6.0/semantha_sdk/model/difference.py
--rw-r--r--   0        0        0      532 2023-07-12 16:01:12.304280 semantha_sdk-5.6.0/semantha_sdk/model/distance.py
--rw-r--r--   0        0        0     1302 2023-07-12 16:01:12.298274 semantha_sdk-5.6.0/semantha_sdk/model/document.py
--rw-r--r--   0        0        0     1004 2023-07-12 16:01:12.341091 semantha_sdk-5.6.0/semantha_sdk/model/document_class.py
--rw-r--r--   0        0        0      773 2023-07-12 16:01:12.309466 semantha_sdk-5.6.0/semantha_sdk/model/document_class_bulk.py
--rw-r--r--   0        0        0      582 2023-07-12 16:01:12.306464 semantha_sdk-5.6.0/semantha_sdk/model/document_class_node.py
--rw-r--r--   0        0        0      660 2023-07-12 16:01:12.272382 semantha_sdk-5.6.0/semantha_sdk/model/document_cluster.py
--rw-r--r--   0        0        0     1078 2023-07-12 16:01:12.268382 semantha_sdk-5.6.0/semantha_sdk/model/document_information.py
--rw-r--r--   0        0        0      510 2023-07-12 16:01:12.329536 semantha_sdk-5.6.0/semantha_sdk/model/document_meta_data.py
--rw-r--r--   0        0        0      505 2023-07-12 16:01:12.236760 semantha_sdk-5.6.0/semantha_sdk/model/document_named_entity.py
--rw-r--r--   0        0        0      533 2023-07-12 16:01:12.226714 semantha_sdk-5.6.0/semantha_sdk/model/document_table.py
--rw-r--r--   0        0        0      577 2023-07-12 16:01:12.292129 semantha_sdk-5.6.0/semantha_sdk/model/domain.py
--rw-r--r--   0        0        0      454 2023-07-12 16:01:12.314988 semantha_sdk-5.6.0/semantha_sdk/model/entity.py
--rw-r--r--   0        0        0      705 2023-07-12 16:01:12.307459 semantha_sdk-5.6.0/semantha_sdk/model/expression.py
--rw-r--r--   0        0        0      604 2023-07-12 16:01:12.279596 semantha_sdk-5.6.0/semantha_sdk/model/extraction_area.py
--rw-r--r--   0        0        0      757 2023-07-12 16:01:12.317005 semantha_sdk-5.6.0/semantha_sdk/model/extraction_file.py
--rw-r--r--   0        0        0      546 2023-07-12 16:01:12.350333 semantha_sdk-5.6.0/semantha_sdk/model/extraction_reference.py
--rw-r--r--   0        0        0      671 2023-07-12 16:01:12.311460 semantha_sdk-5.6.0/semantha_sdk/model/extractor.py
--rw-r--r--   0        0        0      762 2023-07-12 16:01:12.242775 semantha_sdk-5.6.0/semantha_sdk/model/extractor_attribute.py
--rw-r--r--   0        0        0      924 2023-07-12 16:01:12.343095 semantha_sdk-5.6.0/semantha_sdk/model/extractor_class.py
--rw-r--r--   0        0        0      704 2023-07-12 16:01:12.337097 semantha_sdk-5.6.0/semantha_sdk/model/extractor_class_overview.py
--rw-r--r--   0        0        0      908 2023-07-12 16:01:12.323002 semantha_sdk-5.6.0/semantha_sdk/model/extractor_table.py
--rw-r--r--   0        0        0      882 2023-07-12 16:01:12.349335 semantha_sdk-5.6.0/semantha_sdk/model/features.py
--rw-r--r--   0        0        0      412 2023-07-12 16:01:12.278594 semantha_sdk-5.6.0/semantha_sdk/model/field.py
--rw-r--r--   0        0        0      522 2023-07-12 16:01:12.251300 semantha_sdk-5.6.0/semantha_sdk/model/file_reference.py
--rw-r--r--   0        0        0      508 2023-07-12 16:01:12.284111 semantha_sdk-5.6.0/semantha_sdk/model/finding.py
--rw-r--r--   0        0        0      495 2023-07-12 16:01:12.287129 semantha_sdk-5.6.0/semantha_sdk/model/formatter.py
--rw-r--r--   0        0        0      540 2023-07-12 16:01:12.312461 semantha_sdk-5.6.0/semantha_sdk/model/info.py
--rw-r--r--   0        0        0      889 2023-07-12 16:01:12.249294 semantha_sdk-5.6.0/semantha_sdk/model/instance.py
--rw-r--r--   0        0        0      547 2023-07-12 16:01:12.330531 semantha_sdk-5.6.0/semantha_sdk/model/instance_child.py
--rw-r--r--   0        0        0      575 2023-07-12 16:01:12.254818 semantha_sdk-5.6.0/semantha_sdk/model/instance_overview.py
--rw-r--r--   0        0        0      415 2023-07-12 16:01:12.260316 semantha_sdk-5.6.0/semantha_sdk/model/label.py
--rw-r--r--   0        0        0      478 2023-07-12 16:01:12.238770 semantha_sdk-5.6.0/semantha_sdk/model/language_detection.py
--rw-r--r--   0        0        0      602 2023-07-12 16:01:12.269377 semantha_sdk-5.6.0/semantha_sdk/model/linked_instance.py
--rw-r--r--   0        0        0      490 2023-07-12 16:01:12.255334 semantha_sdk-5.6.0/semantha_sdk/model/linked_value.py
--rw-r--r--   0        0        0      421 2023-07-12 16:01:12.237770 semantha_sdk-5.6.0/semantha_sdk/model/matcher.py
--rw-r--r--   0        0        0      611 2023-07-12 16:01:12.328537 semantha_sdk-5.6.0/semantha_sdk/model/matrix_row.py
--rw-r--r--   0        0        0      509 2023-07-12 16:01:12.273382 semantha_sdk-5.6.0/semantha_sdk/model/meta_info_page.py
--rw-r--r--   0        0        0      506 2023-07-12 16:01:12.299276 semantha_sdk-5.6.0/semantha_sdk/model/metadata.py
--rw-r--r--   0        0        0      437 2023-07-12 16:01:12.307459 semantha_sdk-5.6.0/semantha_sdk/model/metadata_value.py
--rw-r--r--   0        0        0      557 2023-07-12 16:01:12.286131 semantha_sdk-5.6.0/semantha_sdk/model/model_class.py
--rw-r--r--   0        0        0     1553 2023-07-12 16:01:12.289699 semantha_sdk-5.6.0/semantha_sdk/model/model_instance.py
--rw-r--r--   0        0        0      495 2023-07-12 16:01:12.296275 semantha_sdk-5.6.0/semantha_sdk/model/named_entity.py
--rw-r--r--   0        0        0      491 2023-07-12 16:01:12.336080 semantha_sdk-5.6.0/semantha_sdk/model/overview.py
--rw-r--r--   0        0        0      844 2023-07-12 16:01:12.301275 semantha_sdk-5.6.0/semantha_sdk/model/page.py
--rw-r--r--   0        0        0      551 2023-07-12 16:01:12.354334 semantha_sdk-5.6.0/semantha_sdk/model/page_content.py
--rw-r--r--   0        0        0     1023 2023-07-12 16:01:12.316004 semantha_sdk-5.6.0/semantha_sdk/model/paragraph.py
--rw-r--r--   0        0        0      493 2023-07-12 16:01:12.277595 semantha_sdk-5.6.0/semantha_sdk/model/paragraph_update.py
--rw-r--r--   0        0        0      538 2023-07-12 16:01:12.327531 semantha_sdk-5.6.0/semantha_sdk/model/plotly_chart.py
--rw-r--r--   0        0        0      587 2023-07-12 16:01:12.276592 semantha_sdk-5.6.0/semantha_sdk/model/process_information.py
--rw-r--r--   0        0        0      506 2023-07-12 16:01:12.344098 semantha_sdk-5.6.0/semantha_sdk/model/range.py
--rw-r--r--   0        0        0      461 2023-07-12 16:01:12.347335 semantha_sdk-5.6.0/semantha_sdk/model/rect.py
--rw-r--r--   0        0        0      831 2023-07-12 16:01:12.266388 semantha_sdk-5.6.0/semantha_sdk/model/reference.py
--rw-r--r--   0        0        0      754 2023-07-12 16:01:12.355437 semantha_sdk-5.6.0/semantha_sdk/model/reference_documents_response_container.py
--rw-r--r--   0        0        0      467 2023-07-12 16:01:12.357259 semantha_sdk-5.6.0/semantha_sdk/model/regex.py
--rw-r--r--   0        0        0      705 2023-07-12 16:01:12.282596 semantha_sdk-5.6.0/semantha_sdk/model/relation.py
--rw-r--r--   0        0        0      514 2023-07-12 16:01:12.348332 semantha_sdk-5.6.0/semantha_sdk/model/relation_condition.py
--rw-r--r--   0        0        0      716 2023-07-12 16:01:12.275591 semantha_sdk-5.6.0/semantha_sdk/model/response_meta_info.py
--rw-r--r--   0        0        0      523 2023-07-12 16:01:12.262853 semantha_sdk-5.6.0/semantha_sdk/model/row.py
--rw-r--r--   0        0        0      670 2023-07-12 16:01:12.246293 semantha_sdk-5.6.0/semantha_sdk/model/rule.py
--rw-r--r--   0        0        0      554 2023-07-12 16:01:12.335070 semantha_sdk-5.6.0/semantha_sdk/model/rule_function.py
--rw-r--r--   0        0        0      591 2023-07-12 16:01:12.313464 semantha_sdk-5.6.0/semantha_sdk/model/rule_overview.py
--rw-r--r--   0        0        0      650 2023-06-29 06:39:31.921661 semantha_sdk-5.6.0/semantha_sdk/model/semantha_entity.py
--rw-r--r--   0        0        0      905 2023-07-12 16:01:12.271384 semantha_sdk-5.6.0/semantha_sdk/model/semantic_model.py
--rw-r--r--   0        0        0      525 2023-07-12 16:01:12.280596 semantha_sdk-5.6.0/semantha_sdk/model/semi_super_vised_document.py
--rw-r--r--   0        0        0      830 2023-07-12 16:01:12.331537 semantha_sdk-5.6.0/semantha_sdk/model/sentence.py
--rw-r--r--   0        0        0     1757 2023-07-12 16:01:12.325531 semantha_sdk-5.6.0/semantha_sdk/model/settings.py
--rw-r--r--   0        0        0      464 2023-07-12 16:01:12.247297 semantha_sdk-5.6.0/semantha_sdk/model/simple_property.py
--rw-r--r--   0        0        0      702 2023-07-12 16:01:12.293197 semantha_sdk-5.6.0/semantha_sdk/model/smart_cluster_response_container.py
--rw-r--r--   0        0        0      892 2023-07-12 16:01:12.353333 semantha_sdk-5.6.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py
--rw-r--r--   0        0        0      640 2023-07-12 16:01:12.291128 semantha_sdk-5.6.0/semantha_sdk/model/statistic.py
--rw-r--r--   0        0        0      490 2023-07-12 16:01:12.318007 semantha_sdk-5.6.0/semantha_sdk/model/stop_word.py
--rw-r--r--   0        0        0      577 2023-07-12 16:01:12.310463 semantha_sdk-5.6.0/semantha_sdk/model/synonym.py
--rw-r--r--   0        0        0      476 2023-07-12 16:01:12.334057 semantha_sdk-5.6.0/semantha_sdk/model/table.py
--rw-r--r--   0        0        0      450 2023-07-12 16:01:12.345320 semantha_sdk-5.6.0/semantha_sdk/model/table_cell.py
--rw-r--r--   0        0        0      572 2023-07-12 16:01:12.338094 semantha_sdk-5.6.0/semantha_sdk/model/table_instance.py
--rw-r--r--   0        0        0      469 2023-07-12 16:01:12.294207 semantha_sdk-5.6.0/semantha_sdk/model/tag_docs.py
--rw-r--r--   0        0        0      471 2023-07-12 16:01:12.351331 semantha_sdk-5.6.0/semantha_sdk/model/version.py
--rw-r--r--   0        0        0       47 2023-05-11 17:26:57.519543 semantha_sdk-5.6.0/semantha_sdk/request/__init__.py
--rw-r--r--   0        0        0      552 2023-05-11 17:26:57.521550 semantha_sdk-5.6.0/semantha_sdk/request/semantha_request.py
--rw-r--r--   0        0        0       57 2023-05-11 17:26:57.522556 semantha_sdk-5.6.0/semantha_sdk/response/__init__.py
--rw-r--r--   0        0        0      107 2023-05-11 17:26:57.524555 semantha_sdk-5.6.0/semantha_sdk/response/semantha_error.py
--rw-r--r--   0        0        0     3712 2023-06-20 12:43:00.735650 semantha_sdk-5.6.0/semantha_sdk/response/semantha_response.py
--rw-r--r--   0        0        0       37 2023-05-11 17:26:57.527555 semantha_sdk-5.6.0/semantha_sdk/rest/__init__.py
--rw-r--r--   0        0        0     4354 2023-05-11 17:26:57.528555 semantha_sdk-5.6.0/semantha_sdk/rest/rest_client.py
--rw-r--r--   0        0        0    18061 1970-01-01 00:00:00.000000 semantha_sdk-5.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11545 2022-12-09 10:06:55.386837 semantha_sdk-5.6.1/LICENSE
+-rw-r--r--   0        0        0     1618 2023-07-18 15:04:37.513452 semantha_sdk-5.6.1/pyproject.toml
+-rw-r--r--   0        0        0    17613 2023-07-12 16:12:16.190051 semantha_sdk-5.6.1/README.md
+-rw-r--r--   0        0        0     1288 2023-05-11 17:26:57.327736 semantha_sdk-5.6.1/semantha_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 06:39:31.917641 semantha_sdk-5.6.1/semantha_sdk/api/__init__.py
+-rw-r--r--   0        0        0     1681 2023-07-14 17:54:31.844525 semantha_sdk-5.6.1/semantha_sdk/api/answers.py
+-rw-r--r--   0        0        0     1004 2023-07-14 17:54:31.802523 semantha_sdk-5.6.1/semantha_sdk/api/bulk.py
+-rw-r--r--   0        0        0      839 2023-07-14 17:54:31.803525 semantha_sdk-5.6.1/semantha_sdk/api/bulk_domains.py
+-rw-r--r--   0        0        0      817 2023-07-14 17:54:31.820524 semantha_sdk-5.6.1/semantha_sdk/api/bulk_model.py
+-rw-r--r--   0        0        0     1792 2023-07-14 17:54:31.815524 semantha_sdk-5.6.1/semantha_sdk/api/bulkdomains_documentclasses.py
+-rw-r--r--   0        0        0     1576 2023-07-14 17:54:31.807525 semantha_sdk-5.6.1/semantha_sdk/api/bulkdomains_domain.py
+-rw-r--r--   0        0        0     3766 2023-07-14 17:54:31.818526 semantha_sdk-5.6.1/semantha_sdk/api/bulkdomains_referencedocuments.py
+-rw-r--r--   0        0        0     3283 2023-07-14 17:54:31.819525 semantha_sdk-5.6.1/semantha_sdk/api/bulkdomains_references.py
+-rw-r--r--   0        0        0     1346 2023-07-14 17:54:31.824525 semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_boostwords.py
+-rw-r--r--   0        0        0      923 2023-07-14 17:54:31.826525 semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_class.py
+-rw-r--r--   0        0        0     1913 2023-07-14 17:54:31.825526 semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_classes.py
+-rw-r--r--   0        0        0     1735 2023-07-14 17:54:31.829527 semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_dataproperties.py
+-rw-r--r--   0        0        0     3018 2023-07-14 17:54:31.823524 semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_domain.py
+-rw-r--r--   0        0        0      836 2023-07-14 17:54:31.822524 semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_domains.py
+-rw-r--r--   0        0        0     1662 2023-07-14 17:54:31.830529 semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_instances.py
+-rw-r--r--   0        0        0     1661 2023-07-14 17:54:31.833524 semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_metadata.py
+-rw-r--r--   0        0        0     1373 2023-07-14 17:54:31.835526 semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_namedentities.py
+-rw-r--r--   0        0        0     1603 2023-07-14 17:54:31.836524 semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_rules.py
+-rw-r--r--   0        0        0     1261 2023-07-14 17:54:31.837525 semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_stopwords.py
+-rw-r--r--   0        0        0     1322 2023-07-14 17:54:31.838525 semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_synonyms.py
+-rw-r--r--   0        0        0     1098 2023-07-14 17:54:31.828529 semantha_sdk-5.6.1/semantha_sdk/api/bulkmodelclass_instances.py
+-rw-r--r--   0        0        0     1262 2023-07-14 17:54:31.887525 semantha_sdk-5.6.1/semantha_sdk/api/child_extractorclasses.py
+-rw-r--r--   0        0        0     5664 2023-07-14 17:54:31.858524 semantha_sdk-5.6.1/semantha_sdk/api/clusters.py
+-rw-r--r--   0        0        0     1168 2023-07-14 17:54:31.838525 semantha_sdk-5.6.1/semantha_sdk/api/currentuser.py
+-rw-r--r--   0        0        0     1425 2023-07-14 17:54:31.841525 semantha_sdk-5.6.1/semantha_sdk/api/diff.py
+-rw-r--r--   0        0        0     4012 2023-07-14 17:54:31.846525 semantha_sdk-5.6.1/semantha_sdk/api/documentannotations.py
+-rw-r--r--   0        0        0     1565 2023-07-18 15:02:58.506013 semantha_sdk-5.6.1/semantha_sdk/api/documentclass.py
+-rw-r--r--   0        0        0     1997 2023-07-14 17:54:31.847526 semantha_sdk-5.6.1/semantha_sdk/api/documentclasses.py
+-rw-r--r--   0        0        0     3464 2023-07-14 17:54:31.850526 semantha_sdk-5.6.1/semantha_sdk/api/documentcomparisons.py
+-rw-r--r--   0        0        0     8589 2023-07-14 17:54:31.851528 semantha_sdk-5.6.1/semantha_sdk/api/documents.py
+-rw-r--r--   0        0        0     4497 2023-07-14 17:54:31.843526 semantha_sdk-5.6.1/semantha_sdk/api/domain.py
+-rw-r--r--   0        0        0     1157 2023-07-14 17:54:31.841525 semantha_sdk-5.6.1/semantha_sdk/api/domains.py
+-rw-r--r--   0        0        0      905 2023-07-14 17:54:31.874525 semantha_sdk-5.6.1/semantha_sdk/api/info.py
+-rw-r--r--   0        0        0     1757 2023-07-14 17:54:31.875527 semantha_sdk-5.6.1/semantha_sdk/api/languages.py
+-rw-r--r--   0        0        0     1595 2023-07-14 17:54:31.876526 semantha_sdk-5.6.1/semantha_sdk/api/model.py
+-rw-r--r--   0        0        0     1019 2023-07-14 17:54:31.880525 semantha_sdk-5.6.1/semantha_sdk/api/model_attributes.py
+-rw-r--r--   0        0        0     1460 2023-07-14 17:54:31.882526 semantha_sdk-5.6.1/semantha_sdk/api/model_boostword.py
+-rw-r--r--   0        0        0     1924 2023-07-14 17:54:31.881527 semantha_sdk-5.6.1/semantha_sdk/api/model_boostwords.py
+-rw-r--r--   0        0        0     2088 2023-07-14 17:54:31.883525 semantha_sdk-5.6.1/semantha_sdk/api/model_dataproperties.py
+-rw-r--r--   0        0        0     1505 2023-07-14 17:54:31.884525 semantha_sdk-5.6.1/semantha_sdk/api/model_dataproperty.py
+-rw-r--r--   0        0        0      840 2023-07-14 17:54:31.877526 semantha_sdk-5.6.1/semantha_sdk/api/model_datatypes.py
+-rw-r--r--   0        0        0     5566 2023-07-14 17:54:31.879528 semantha_sdk-5.6.1/semantha_sdk/api/model_domain.py
+-rw-r--r--   0        0        0      816 2023-07-14 17:54:31.878526 semantha_sdk-5.6.1/semantha_sdk/api/model_domains.py
+-rw-r--r--   0        0        0     1830 2023-07-14 17:54:31.886527 semantha_sdk-5.6.1/semantha_sdk/api/model_extractorclass.py
+-rw-r--r--   0        0        0     2487 2023-07-14 17:54:31.885528 semantha_sdk-5.6.1/semantha_sdk/api/model_extractorclasses.py
+-rw-r--r--   0        0        0      951 2023-07-14 17:54:31.887525 semantha_sdk-5.6.1/semantha_sdk/api/model_extractors.py
+-rw-r--r--   0        0        0     1536 2023-07-14 17:54:31.890526 semantha_sdk-5.6.1/semantha_sdk/api/model_extractortable.py
+-rw-r--r--   0        0        0     2103 2023-07-14 17:54:31.888525 semantha_sdk-5.6.1/semantha_sdk/api/model_extractortables.py
+-rw-r--r--   0        0        0      855 2023-07-14 17:54:31.906533 semantha_sdk-5.6.1/semantha_sdk/api/model_extractortypes.py
+-rw-r--r--   0        0        0      969 2023-07-14 17:54:31.890526 semantha_sdk-5.6.1/semantha_sdk/api/model_formatters.py
+-rw-r--r--   0        0        0     1904 2023-07-14 17:54:31.893526 semantha_sdk-5.6.1/semantha_sdk/api/model_metadata.py
+-rw-r--r--   0        0        0      852 2023-07-14 17:54:31.907525 semantha_sdk-5.6.1/semantha_sdk/api/model_metadatatypes.py
+-rw-r--r--   0        0        0     1970 2023-07-14 17:54:31.896525 semantha_sdk-5.6.1/semantha_sdk/api/model_namedentities.py
+-rw-r--r--   0        0        0     1494 2023-07-14 17:54:31.897524 semantha_sdk-5.6.1/semantha_sdk/api/model_namedentity.py
+-rw-r--r--   0        0        0      982 2023-07-14 17:54:31.897524 semantha_sdk-5.6.1/semantha_sdk/api/model_objectproperties.py
+-rw-r--r--   0        0        0     1441 2023-07-14 17:54:31.894532 semantha_sdk-5.6.1/semantha_sdk/api/model_onemetadata.py
+-rw-r--r--   0        0        0     1401 2023-07-14 17:54:31.899525 semantha_sdk-5.6.1/semantha_sdk/api/model_regex.py
+-rw-r--r--   0        0        0     1850 2023-07-14 17:54:31.898525 semantha_sdk-5.6.1/semantha_sdk/api/model_regexes.py
+-rw-r--r--   0        0        0     1444 2023-07-14 17:54:31.900526 semantha_sdk-5.6.1/semantha_sdk/api/model_relation.py
+-rw-r--r--   0        0        0     1902 2023-07-14 17:54:31.900526 semantha_sdk-5.6.1/semantha_sdk/api/model_relations.py
+-rw-r--r--   0        0        0     1388 2023-07-14 17:54:31.902526 semantha_sdk-5.6.1/semantha_sdk/api/model_rule.py
+-rw-r--r--   0        0        0      999 2023-07-14 17:54:31.901524 semantha_sdk-5.6.1/semantha_sdk/api/model_rulefunctions.py
+-rw-r--r--   0        0        0     1962 2023-07-14 17:54:31.902526 semantha_sdk-5.6.1/semantha_sdk/api/model_rules.py
+-rw-r--r--   0        0        0     1449 2023-07-14 17:54:31.904526 semantha_sdk-5.6.1/semantha_sdk/api/model_stopword.py
+-rw-r--r--   0        0        0     1907 2023-07-14 17:54:31.903526 semantha_sdk-5.6.1/semantha_sdk/api/model_stopwords.py
+-rw-r--r--   0        0        0     1430 2023-07-14 17:54:31.906533 semantha_sdk-5.6.1/semantha_sdk/api/model_synonym.py
+-rw-r--r--   0        0        0     1882 2023-07-14 17:54:31.905527 semantha_sdk-5.6.1/semantha_sdk/api/model_synonyms.py
+-rw-r--r--   0        0        0     1217 2023-07-14 17:54:31.852527 semantha_sdk-5.6.1/semantha_sdk/api/modelclasses.py
+-rw-r--r--   0        0        0     3928 2023-07-14 17:54:31.853526 semantha_sdk-5.6.1/semantha_sdk/api/modelinstances.py
+-rw-r--r--   0        0        0     1450 2023-07-14 17:54:31.892527 semantha_sdk-5.6.1/semantha_sdk/api/modelont_instance.py
+-rw-r--r--   0        0        0     2592 2023-07-14 17:54:31.891525 semantha_sdk-5.6.1/semantha_sdk/api/modelont_instances.py
+-rw-r--r--   0        0        0     1663 2023-07-14 17:54:31.859526 semantha_sdk-5.6.1/semantha_sdk/api/namedentities.py
+-rw-r--r--   0        0        0     1711 2023-07-14 17:54:31.863527 semantha_sdk-5.6.1/semantha_sdk/api/paragraph.py
+-rw-r--r--   0        0        0      792 2023-07-14 17:54:31.861525 semantha_sdk-5.6.1/semantha_sdk/api/paragraphs.py
+-rw-r--r--   0        0        0     2267 2023-07-14 17:54:31.860526 semantha_sdk-5.6.1/semantha_sdk/api/referencedocument.py
+-rw-r--r--   0        0        0    13183 2023-07-14 17:54:31.857526 semantha_sdk-5.6.1/semantha_sdk/api/referencedocuments.py
+-rw-r--r--   0        0        0    22267 2023-07-14 17:54:31.866526 semantha_sdk-5.6.1/semantha_sdk/api/references.py
+-rw-r--r--   0        0        0      867 2023-07-14 17:54:31.839526 semantha_sdk-5.6.1/semantha_sdk/api/roles.py
+-rw-r--r--   0        0        0     2113 2023-06-29 06:39:31.918640 semantha_sdk-5.6.1/semantha_sdk/api/semantha_api.py
+-rw-r--r--   0        0        0      413 2023-06-29 06:39:31.920640 semantha_sdk-5.6.1/semantha_sdk/api/semantha_endpoint.py
+-rw-r--r--   0        0        0      967 2023-07-14 17:54:31.864524 semantha_sdk-5.6.1/semantha_sdk/api/sentence.py
+-rw-r--r--   0        0        0      786 2023-07-14 17:54:31.864524 semantha_sdk-5.6.1/semantha_sdk/api/sentences.py
+-rw-r--r--   0        0        0     1497 2023-07-14 17:54:31.867525 semantha_sdk-5.6.1/semantha_sdk/api/settings.py
+-rw-r--r--   0        0        0     5081 2023-07-14 17:54:31.868524 semantha_sdk-5.6.1/semantha_sdk/api/similaritymatrix.py
+-rw-r--r--   0        0        0     3934 2023-07-14 17:54:31.869529 semantha_sdk-5.6.1/semantha_sdk/api/similaritymatrix_cluster.py
+-rw-r--r--   0        0        0      963 2023-07-14 17:54:31.859526 semantha_sdk-5.6.1/semantha_sdk/api/statistic.py
+-rw-r--r--   0        0        0     1207 2023-07-14 17:54:31.870525 semantha_sdk-5.6.1/semantha_sdk/api/summarizations.py
+-rw-r--r--   0        0        0      931 2023-07-14 17:54:31.872525 semantha_sdk-5.6.1/semantha_sdk/api/tag.py
+-rw-r--r--   0        0        0     1285 2023-07-14 17:54:31.872525 semantha_sdk-5.6.1/semantha_sdk/api/tag_referencedocuments.py
+-rw-r--r--   0        0        0     1018 2023-07-14 17:54:31.871525 semantha_sdk-5.6.1/semantha_sdk/api/tags.py
+-rw-r--r--   0        0        0     1383 2023-07-14 17:54:31.873525 semantha_sdk-5.6.1/semantha_sdk/api/validation.py
+-rw-r--r--   0        0        0     5700 2023-07-18 15:02:58.509020 semantha_sdk-5.6.1/semantha_sdk/model/__init__.py
+-rw-r--r--   0        0        0      617 2023-07-14 17:54:31.973524 semantha_sdk-5.6.1/semantha_sdk/model/annotation_cell.py
+-rw-r--r--   0        0        0      689 2023-07-14 17:54:32.025529 semantha_sdk-5.6.1/semantha_sdk/model/annotation_page.py
+-rw-r--r--   0        0        0      582 2023-07-14 17:54:31.978544 semantha_sdk-5.6.1/semantha_sdk/model/answer.py
+-rw-r--r--   0        0        0      548 2023-07-14 17:54:32.007527 semantha_sdk-5.6.1/semantha_sdk/model/answer_reference.py
+-rw-r--r--   0        0        0      658 2023-07-14 17:54:31.998526 semantha_sdk-5.6.1/semantha_sdk/model/argument.py
+-rw-r--r--   0        0        0      547 2023-07-14 17:54:32.009525 semantha_sdk-5.6.1/semantha_sdk/model/attribute_overview.py
+-rw-r--r--   0        0        0      581 2023-07-14 17:54:32.008527 semantha_sdk-5.6.1/semantha_sdk/model/boost_word.py
+-rw-r--r--   0        0        0      989 2023-07-14 17:54:31.999525 semantha_sdk-5.6.1/semantha_sdk/model/class_bulk.py
+-rw-r--r--   0        0        0      515 2023-07-14 17:54:31.987527 semantha_sdk-5.6.1/semantha_sdk/model/clustered_document.py
+-rw-r--r--   0        0        0      717 2023-07-14 17:54:31.993524 semantha_sdk-5.6.1/semantha_sdk/model/clustering_response.py
+-rw-r--r--   0        0        0      519 2023-07-14 17:54:32.023526 semantha_sdk-5.6.1/semantha_sdk/model/column.py
+-rw-r--r--   0        0        0     1201 2023-07-14 17:54:32.020528 semantha_sdk-5.6.1/semantha_sdk/model/complex_property.py
+-rw-r--r--   0        0        0      627 2023-07-14 17:54:32.001525 semantha_sdk-5.6.1/semantha_sdk/model/condition.py
+-rw-r--r--   0        0        0      587 2023-07-14 17:54:32.001525 semantha_sdk-5.6.1/semantha_sdk/model/condition_value.py
+-rw-r--r--   0        0        0      545 2023-07-14 17:54:32.002526 semantha_sdk-5.6.1/semantha_sdk/model/current_user.py
+-rw-r--r--   0        0        0      639 2023-07-14 17:54:32.004526 semantha_sdk-5.6.1/semantha_sdk/model/data_property.py
+-rw-r--r--   0        0        0      483 2023-07-14 17:54:32.026527 semantha_sdk-5.6.1/semantha_sdk/model/difference.py
+-rw-r--r--   0        0        0      532 2023-07-14 17:54:31.967525 semantha_sdk-5.6.1/semantha_sdk/model/distance.py
+-rw-r--r--   0        0        0     1302 2023-07-14 17:54:32.029529 semantha_sdk-5.6.1/semantha_sdk/model/document.py
+-rw-r--r--   0        0        0     1004 2023-07-18 15:02:58.514795 semantha_sdk-5.6.1/semantha_sdk/model/document_class.py
+-rw-r--r--   0        0        0      773 2023-07-18 15:02:58.518801 semantha_sdk-5.6.1/semantha_sdk/model/document_class_bulk.py
+-rw-r--r--   0        0        0      582 2023-07-18 15:02:58.522942 semantha_sdk-5.6.1/semantha_sdk/model/document_class_node.py
+-rw-r--r--   0        0        0      660 2023-07-14 17:54:31.992525 semantha_sdk-5.6.1/semantha_sdk/model/document_cluster.py
+-rw-r--r--   0        0        0     1078 2023-07-14 17:54:32.005525 semantha_sdk-5.6.1/semantha_sdk/model/document_information.py
+-rw-r--r--   0        0        0      510 2023-07-14 17:54:32.027529 semantha_sdk-5.6.1/semantha_sdk/model/document_meta_data.py
+-rw-r--r--   0        0        0      505 2023-07-14 17:54:31.990525 semantha_sdk-5.6.1/semantha_sdk/model/document_named_entity.py
+-rw-r--r--   0        0        0      533 2023-07-14 17:54:32.027529 semantha_sdk-5.6.1/semantha_sdk/model/document_table.py
+-rw-r--r--   0        0        0      577 2023-07-14 17:54:32.019535 semantha_sdk-5.6.1/semantha_sdk/model/domain.py
+-rw-r--r--   0        0        0      454 2023-07-14 17:54:32.011525 semantha_sdk-5.6.1/semantha_sdk/model/entity.py
+-rw-r--r--   0        0        0      705 2023-07-14 17:54:32.013526 semantha_sdk-5.6.1/semantha_sdk/model/expression.py
+-rw-r--r--   0        0        0      604 2023-07-14 17:54:31.988545 semantha_sdk-5.6.1/semantha_sdk/model/extraction_area.py
+-rw-r--r--   0        0        0      757 2023-07-14 17:54:32.000526 semantha_sdk-5.6.1/semantha_sdk/model/extraction_file.py
+-rw-r--r--   0        0        0      546 2023-07-14 17:54:31.983526 semantha_sdk-5.6.1/semantha_sdk/model/extraction_reference.py
+-rw-r--r--   0        0        0      671 2023-07-18 15:02:58.526937 semantha_sdk-5.6.1/semantha_sdk/model/extractor.py
+-rw-r--r--   0        0        0      762 2023-07-14 17:54:31.984525 semantha_sdk-5.6.1/semantha_sdk/model/extractor_attribute.py
+-rw-r--r--   0        0        0      924 2023-07-14 17:54:31.974524 semantha_sdk-5.6.1/semantha_sdk/model/extractor_class.py
+-rw-r--r--   0        0        0      704 2023-07-14 17:54:32.011525 semantha_sdk-5.6.1/semantha_sdk/model/extractor_class_overview.py
+-rw-r--r--   0        0        0      908 2023-07-14 17:54:31.979526 semantha_sdk-5.6.1/semantha_sdk/model/extractor_table.py
+-rw-r--r--   0        0        0      882 2023-07-14 17:54:32.006526 semantha_sdk-5.6.1/semantha_sdk/model/features.py
+-rw-r--r--   0        0        0      412 2023-07-14 17:54:31.983526 semantha_sdk-5.6.1/semantha_sdk/model/field.py
+-rw-r--r--   0        0        0      522 2023-07-14 17:54:32.007527 semantha_sdk-5.6.1/semantha_sdk/model/file_reference.py
+-rw-r--r--   0        0        0      508 2023-07-14 17:54:31.990525 semantha_sdk-5.6.1/semantha_sdk/model/finding.py
+-rw-r--r--   0        0        0      495 2023-07-14 17:54:31.998526 semantha_sdk-5.6.1/semantha_sdk/model/formatter.py
+-rw-r--r--   0        0        0      540 2023-07-14 17:54:32.024527 semantha_sdk-5.6.1/semantha_sdk/model/info.py
+-rw-r--r--   0        0        0      889 2023-07-14 17:54:32.009525 semantha_sdk-5.6.1/semantha_sdk/model/instance.py
+-rw-r--r--   0        0        0      547 2023-07-14 17:54:31.975525 semantha_sdk-5.6.1/semantha_sdk/model/instance_child.py
+-rw-r--r--   0        0        0      575 2023-07-14 17:54:31.995526 semantha_sdk-5.6.1/semantha_sdk/model/instance_overview.py
+-rw-r--r--   0        0        0      415 2023-07-14 17:54:32.004526 semantha_sdk-5.6.1/semantha_sdk/model/label.py
+-rw-r--r--   0        0        0      478 2023-07-14 17:54:32.023526 semantha_sdk-5.6.1/semantha_sdk/model/language_detection.py
+-rw-r--r--   0        0        0      602 2023-07-14 17:54:32.014526 semantha_sdk-5.6.1/semantha_sdk/model/linked_instance.py
+-rw-r--r--   0        0        0      490 2023-07-14 17:54:31.984525 semantha_sdk-5.6.1/semantha_sdk/model/linked_value.py
+-rw-r--r--   0        0        0      421 2023-07-18 15:02:58.531174 semantha_sdk-5.6.1/semantha_sdk/model/matcher.py
+-rw-r--r--   0        0        0      611 2023-07-14 17:54:31.982525 semantha_sdk-5.6.1/semantha_sdk/model/matrix_row.py
+-rw-r--r--   0        0        0      509 2023-07-14 17:54:31.975525 semantha_sdk-5.6.1/semantha_sdk/model/meta_info_page.py
+-rw-r--r--   0        0        0      506 2023-07-14 17:54:32.018526 semantha_sdk-5.6.1/semantha_sdk/model/metadata.py
+-rw-r--r--   0        0        0      437 2023-07-14 17:54:31.966525 semantha_sdk-5.6.1/semantha_sdk/model/metadata_value.py
+-rw-r--r--   0        0        0      557 2023-07-14 17:54:32.028529 semantha_sdk-5.6.1/semantha_sdk/model/model_class.py
+-rw-r--r--   0        0        0     1553 2023-07-14 17:54:32.000526 semantha_sdk-5.6.1/semantha_sdk/model/model_instance.py
+-rw-r--r--   0        0        0      495 2023-07-14 17:54:32.015526 semantha_sdk-5.6.1/semantha_sdk/model/named_entity.py
+-rw-r--r--   0        0        0      491 2023-07-14 17:54:32.032534 semantha_sdk-5.6.1/semantha_sdk/model/overview.py
+-rw-r--r--   0        0        0      844 2023-07-14 17:54:31.996525 semantha_sdk-5.6.1/semantha_sdk/model/page.py
+-rw-r--r--   0        0        0      551 2023-07-14 17:54:31.991525 semantha_sdk-5.6.1/semantha_sdk/model/page_content.py
+-rw-r--r--   0        0        0     1023 2023-07-14 17:54:31.995526 semantha_sdk-5.6.1/semantha_sdk/model/paragraph.py
+-rw-r--r--   0        0        0      493 2023-07-14 17:54:32.016525 semantha_sdk-5.6.1/semantha_sdk/model/paragraph_update.py
+-rw-r--r--   0        0        0      538 2023-07-14 17:54:31.986524 semantha_sdk-5.6.1/semantha_sdk/model/plotly_chart.py
+-rw-r--r--   0        0        0      587 2023-07-14 17:54:32.030530 semantha_sdk-5.6.1/semantha_sdk/model/process_information.py
+-rw-r--r--   0        0        0      506 2023-07-14 17:54:32.010526 semantha_sdk-5.6.1/semantha_sdk/model/range.py
+-rw-r--r--   0        0        0      461 2023-07-14 17:54:31.985526 semantha_sdk-5.6.1/semantha_sdk/model/rect.py
+-rw-r--r--   0        0        0      831 2023-07-14 17:54:31.992525 semantha_sdk-5.6.1/semantha_sdk/model/reference.py
+-rw-r--r--   0        0        0      754 2023-07-14 17:54:31.996525 semantha_sdk-5.6.1/semantha_sdk/model/reference_documents_response_container.py
+-rw-r--r--   0        0        0      467 2023-07-14 17:54:32.022527 semantha_sdk-5.6.1/semantha_sdk/model/regex.py
+-rw-r--r--   0        0        0      705 2023-07-14 17:54:31.997526 semantha_sdk-5.6.1/semantha_sdk/model/relation.py
+-rw-r--r--   0        0        0      514 2023-07-14 17:54:32.029529 semantha_sdk-5.6.1/semantha_sdk/model/relation_condition.py
+-rw-r--r--   0        0        0      716 2023-07-14 17:54:31.986524 semantha_sdk-5.6.1/semantha_sdk/model/response_meta_info.py
+-rw-r--r--   0        0        0      523 2023-07-14 17:54:32.032534 semantha_sdk-5.6.1/semantha_sdk/model/row.py
+-rw-r--r--   0        0        0      670 2023-07-14 17:54:32.014526 semantha_sdk-5.6.1/semantha_sdk/model/rule.py
+-rw-r--r--   0        0        0      554 2023-07-14 17:54:31.987527 semantha_sdk-5.6.1/semantha_sdk/model/rule_function.py
+-rw-r--r--   0        0        0      591 2023-07-14 17:54:32.018526 semantha_sdk-5.6.1/semantha_sdk/model/rule_overview.py
+-rw-r--r--   0        0        0      650 2023-06-29 06:39:31.921661 semantha_sdk-5.6.1/semantha_sdk/model/semantha_entity.py
+-rw-r--r--   0        0        0      905 2023-07-14 17:54:32.012527 semantha_sdk-5.6.1/semantha_sdk/model/semantic_model.py
+-rw-r--r--   0        0        0      525 2023-07-14 17:54:32.008527 semantha_sdk-5.6.1/semantha_sdk/model/semi_super_vised_document.py
+-rw-r--r--   0        0        0      830 2023-07-14 17:54:31.977542 semantha_sdk-5.6.1/semantha_sdk/model/sentence.py
+-rw-r--r--   0        0        0     1757 2023-07-14 17:54:32.003526 semantha_sdk-5.6.1/semantha_sdk/model/settings.py
+-rw-r--r--   0        0        0      464 2023-07-14 17:54:31.977542 semantha_sdk-5.6.1/semantha_sdk/model/simple_property.py
+-rw-r--r--   0        0        0      702 2023-07-14 17:54:32.026527 semantha_sdk-5.6.1/semantha_sdk/model/smart_cluster_response_container.py
+-rw-r--r--   0        0        0      892 2023-07-14 17:54:32.017526 semantha_sdk-5.6.1/semantha_sdk/model/smart_cluster_semi_supervised_request.py
+-rw-r--r--   0        0        0      640 2023-07-14 17:54:31.989529 semantha_sdk-5.6.1/semantha_sdk/model/statistic.py
+-rw-r--r--   0        0        0      490 2023-07-14 17:54:31.969525 semantha_sdk-5.6.1/semantha_sdk/model/stop_word.py
+-rw-r--r--   0        0        0      577 2023-07-14 17:54:32.030530 semantha_sdk-5.6.1/semantha_sdk/model/synonym.py
+-rw-r--r--   0        0        0      476 2023-07-14 17:54:32.021525 semantha_sdk-5.6.1/semantha_sdk/model/table.py
+-rw-r--r--   0        0        0      450 2023-07-14 17:54:31.979526 semantha_sdk-5.6.1/semantha_sdk/model/table_cell.py
+-rw-r--r--   0        0        0      572 2023-07-14 17:54:32.031527 semantha_sdk-5.6.1/semantha_sdk/model/table_instance.py
+-rw-r--r--   0        0        0      469 2023-07-14 17:54:31.994528 semantha_sdk-5.6.1/semantha_sdk/model/tag_docs.py
+-rw-r--r--   0        0        0      471 2023-07-14 17:54:31.974524 semantha_sdk-5.6.1/semantha_sdk/model/version.py
+-rw-r--r--   0        0        0       47 2023-05-11 17:26:57.519543 semantha_sdk-5.6.1/semantha_sdk/request/__init__.py
+-rw-r--r--   0        0        0      552 2023-05-11 17:26:57.521550 semantha_sdk-5.6.1/semantha_sdk/request/semantha_request.py
+-rw-r--r--   0        0        0       57 2023-05-11 17:26:57.522556 semantha_sdk-5.6.1/semantha_sdk/response/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-11 17:26:57.524555 semantha_sdk-5.6.1/semantha_sdk/response/semantha_error.py
+-rw-r--r--   0        0        0     3712 2023-06-20 12:43:00.735650 semantha_sdk-5.6.1/semantha_sdk/response/semantha_response.py
+-rw-r--r--   0        0        0       37 2023-05-11 17:26:57.527555 semantha_sdk-5.6.1/semantha_sdk/rest/__init__.py
+-rw-r--r--   0        0        0     4469 2023-07-18 15:03:46.745389 semantha_sdk-5.6.1/semantha_sdk/rest/rest_client.py
+-rw-r--r--   0        0        0    18095 1970-01-01 00:00:00.000000 semantha_sdk-5.6.1/PKG-INFO
```

### Comparing `semantha_sdk-5.6.0/LICENSE` & `semantha_sdk-5.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/pyproject.toml` & `semantha_sdk-5.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantha-sdk"
-version = "5.6.0"
+version = "5.6.1"
 description = "This is a python client sdk for accessing semantha (the semantic platform)"
 authors = [
     "Sebastian Weigelt <sebastian.weigelt@semantha.ai>",
     "Georg Müller <georg@semantha.ai>",
     "Tom Kaminski <tom.kaminski@semantha.ai>",
     "Timo Januschke <timo.januschke@semantha.ai>"
 ]
```

### Comparing `semantha_sdk-5.6.0/README.md` & `semantha_sdk-5.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 
 **IMPORTANT:** The SDK is still under development and interfaces may change at any time without notice.
 Use with caution and on own risk.
 
 ## Update Notes
 
 ### Version 5.6.0
-Adde most endpoints in **/api/models/* **
+Added most endpoints in **/api/models/* **
+SDK covers now 158/180 services.
 
 ### Version 5.5.0
 Removed language parameter on **/api/domains/{domainname}/references**
 Fixed bug on serialization of **/api/domains/{domainname}/modelinstances** response.
 Fixed return of binary responses of bulk services.
 
 ### Version 5.4.0
```

### Comparing `semantha_sdk-5.6.0/semantha_sdk/__init__.py` & `semantha_sdk-5.6.1/semantha_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/answers.py` & `semantha_sdk-5.6.1/semantha_sdk/api/answers.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/bulk.py` & `semantha_sdk-5.6.1/semantha_sdk/api/bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/bulk_domains.py` & `semantha_sdk-5.6.1/semantha_sdk/api/bulk_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/bulk_model.py` & `semantha_sdk-5.6.1/semantha_sdk/api/bulk_model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/bulkdomains_documentclasses.py` & `semantha_sdk-5.6.1/semantha_sdk/api/bulkdomains_documentclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/bulkdomains_domain.py` & `semantha_sdk-5.6.1/semantha_sdk/api/bulkdomains_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/bulkdomains_referencedocuments.py` & `semantha_sdk-5.6.1/semantha_sdk/api/bulkdomains_referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/bulkdomains_references.py` & `semantha_sdk-5.6.1/semantha_sdk/api/bulkdomains_references.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_boostwords.py` & `semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_boostwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_class.py` & `semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_classes.py` & `semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_classes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_dataproperties.py` & `semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_dataproperties.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_domain.py` & `semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_domains.py` & `semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_instances.py` & `semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_metadata.py` & `semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_metadata.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_namedentities.py` & `semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_rules.py` & `semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_rules.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_stopwords.py` & `semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_stopwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_synonyms.py` & `semantha_sdk-5.6.1/semantha_sdk/api/bulkmodel_synonyms.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodelclass_instances.py` & `semantha_sdk-5.6.1/semantha_sdk/api/bulkmodelclass_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/child_extractorclasses.py` & `semantha_sdk-5.6.1/semantha_sdk/api/child_extractorclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/clusters.py` & `semantha_sdk-5.6.1/semantha_sdk/api/clusters.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/currentuser.py` & `semantha_sdk-5.6.1/semantha_sdk/api/currentuser.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/diff.py` & `semantha_sdk-5.6.1/semantha_sdk/api/diff.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/documentannotations.py` & `semantha_sdk-5.6.1/semantha_sdk/api/documentannotations.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/documentclass.py` & `semantha_sdk-5.6.1/semantha_sdk/api/documentclass.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/documentclasses.py` & `semantha_sdk-5.6.1/semantha_sdk/api/documentclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/documentcomparisons.py` & `semantha_sdk-5.6.1/semantha_sdk/api/documentcomparisons.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/documents.py` & `semantha_sdk-5.6.1/semantha_sdk/api/documents.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/domain.py` & `semantha_sdk-5.6.1/semantha_sdk/api/domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/domains.py` & `semantha_sdk-5.6.1/semantha_sdk/api/domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/info.py` & `semantha_sdk-5.6.1/semantha_sdk/api/info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/languages.py` & `semantha_sdk-5.6.1/semantha_sdk/api/languages.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_attributes.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_attributes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_boostword.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_boostword.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_boostwords.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_boostwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_dataproperties.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_dataproperties.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_dataproperty.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_dataproperty.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_datatypes.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_datatypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_domain.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_domains.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_extractorclass.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_extractorclass.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_extractorclasses.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_extractorclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_extractors.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_extractors.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_extractortable.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_extractortable.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_extractortables.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_extractortables.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_extractortypes.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_extractortypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_formatters.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_formatters.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_metadata.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_metadata.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_metadatatypes.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_metadatatypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_namedentities.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_namedentity.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_namedentity.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_objectproperties.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_objectproperties.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_onemetadata.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_onemetadata.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_regex.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_regex.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_regexes.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_regexes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_relation.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_relation.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_relations.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_relations.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_rule.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_rule.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_rulefunctions.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_rulefunctions.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_rules.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_rules.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_stopword.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_stopword.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_stopwords.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_stopwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_synonym.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_synonym.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/model_synonyms.py` & `semantha_sdk-5.6.1/semantha_sdk/api/model_synonyms.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/modelclasses.py` & `semantha_sdk-5.6.1/semantha_sdk/api/modelclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/modelinstances.py` & `semantha_sdk-5.6.1/semantha_sdk/api/modelinstances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/modelont_instance.py` & `semantha_sdk-5.6.1/semantha_sdk/api/modelont_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/modelont_instances.py` & `semantha_sdk-5.6.1/semantha_sdk/api/modelont_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/namedentities.py` & `semantha_sdk-5.6.1/semantha_sdk/api/namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/paragraph.py` & `semantha_sdk-5.6.1/semantha_sdk/api/paragraph.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/paragraphs.py` & `semantha_sdk-5.6.1/semantha_sdk/api/paragraphs.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/referencedocument.py` & `semantha_sdk-5.6.1/semantha_sdk/api/referencedocument.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/referencedocuments.py` & `semantha_sdk-5.6.1/semantha_sdk/api/referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/references.py` & `semantha_sdk-5.6.1/semantha_sdk/api/references.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/roles.py` & `semantha_sdk-5.6.1/semantha_sdk/api/roles.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/semantha_api.py` & `semantha_sdk-5.6.1/semantha_sdk/api/semantha_api.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/sentence.py` & `semantha_sdk-5.6.1/semantha_sdk/api/sentence.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/sentences.py` & `semantha_sdk-5.6.1/semantha_sdk/api/sentences.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/settings.py` & `semantha_sdk-5.6.1/semantha_sdk/api/settings.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/similaritymatrix.py` & `semantha_sdk-5.6.1/semantha_sdk/api/similaritymatrix.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/similaritymatrix_cluster.py` & `semantha_sdk-5.6.1/semantha_sdk/api/similaritymatrix_cluster.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/statistic.py` & `semantha_sdk-5.6.1/semantha_sdk/api/statistic.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/summarizations.py` & `semantha_sdk-5.6.1/semantha_sdk/api/summarizations.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/tag.py` & `semantha_sdk-5.6.1/semantha_sdk/api/tag.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/tag_referencedocuments.py` & `semantha_sdk-5.6.1/semantha_sdk/api/tag_referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/tags.py` & `semantha_sdk-5.6.1/semantha_sdk/api/tags.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/api/validation.py` & `semantha_sdk-5.6.1/semantha_sdk/api/validation.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/__init__.py` & `semantha_sdk-5.6.1/semantha_sdk/model/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/annotation_cell.py` & `semantha_sdk-5.6.1/semantha_sdk/model/annotation_cell.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/annotation_page.py` & `semantha_sdk-5.6.1/semantha_sdk/model/annotation_page.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/answer.py` & `semantha_sdk-5.6.1/semantha_sdk/model/answer.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/answer_reference.py` & `semantha_sdk-5.6.1/semantha_sdk/model/answer_reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/argument.py` & `semantha_sdk-5.6.1/semantha_sdk/model/argument.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/attribute_overview.py` & `semantha_sdk-5.6.1/semantha_sdk/model/attribute_overview.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/boost_word.py` & `semantha_sdk-5.6.1/semantha_sdk/model/boost_word.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/class_bulk.py` & `semantha_sdk-5.6.1/semantha_sdk/model/class_bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/clustered_document.py` & `semantha_sdk-5.6.1/semantha_sdk/model/clustered_document.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/clustering_response.py` & `semantha_sdk-5.6.1/semantha_sdk/model/clustering_response.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/column.py` & `semantha_sdk-5.6.1/semantha_sdk/model/column.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/complex_property.py` & `semantha_sdk-5.6.1/semantha_sdk/model/complex_property.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/condition.py` & `semantha_sdk-5.6.1/semantha_sdk/model/condition.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/condition_value.py` & `semantha_sdk-5.6.1/semantha_sdk/model/condition_value.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/current_user.py` & `semantha_sdk-5.6.1/semantha_sdk/model/current_user.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/data_property.py` & `semantha_sdk-5.6.1/semantha_sdk/model/data_property.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/distance.py` & `semantha_sdk-5.6.1/semantha_sdk/model/distance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/document.py` & `semantha_sdk-5.6.1/semantha_sdk/model/document.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/document_class.py` & `semantha_sdk-5.6.1/semantha_sdk/model/document_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/document_class_bulk.py` & `semantha_sdk-5.6.1/semantha_sdk/model/document_class_bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/document_class_node.py` & `semantha_sdk-5.6.1/semantha_sdk/model/document_class_node.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/document_cluster.py` & `semantha_sdk-5.6.1/semantha_sdk/model/document_cluster.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/document_information.py` & `semantha_sdk-5.6.1/semantha_sdk/model/document_information.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/document_table.py` & `semantha_sdk-5.6.1/semantha_sdk/model/document_table.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/domain.py` & `semantha_sdk-5.6.1/semantha_sdk/model/domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/expression.py` & `semantha_sdk-5.6.1/semantha_sdk/model/expression.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/extraction_area.py` & `semantha_sdk-5.6.1/semantha_sdk/model/extraction_area.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/extraction_file.py` & `semantha_sdk-5.6.1/semantha_sdk/model/extraction_file.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/extraction_reference.py` & `semantha_sdk-5.6.1/semantha_sdk/model/extraction_reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/extractor.py` & `semantha_sdk-5.6.1/semantha_sdk/model/extractor.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/extractor_attribute.py` & `semantha_sdk-5.6.1/semantha_sdk/model/extractor_attribute.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/extractor_class.py` & `semantha_sdk-5.6.1/semantha_sdk/model/extractor_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/extractor_class_overview.py` & `semantha_sdk-5.6.1/semantha_sdk/model/extractor_class_overview.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/extractor_table.py` & `semantha_sdk-5.6.1/semantha_sdk/model/extractor_table.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/features.py` & `semantha_sdk-5.6.1/semantha_sdk/model/features.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/file_reference.py` & `semantha_sdk-5.6.1/semantha_sdk/model/file_reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/info.py` & `semantha_sdk-5.6.1/semantha_sdk/model/info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/instance.py` & `semantha_sdk-5.6.1/semantha_sdk/model/instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/instance_child.py` & `semantha_sdk-5.6.1/semantha_sdk/model/instance_child.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/instance_overview.py` & `semantha_sdk-5.6.1/semantha_sdk/model/instance_overview.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/linked_instance.py` & `semantha_sdk-5.6.1/semantha_sdk/model/linked_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/matrix_row.py` & `semantha_sdk-5.6.1/semantha_sdk/model/matrix_row.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/model_class.py` & `semantha_sdk-5.6.1/semantha_sdk/model/model_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/model_instance.py` & `semantha_sdk-5.6.1/semantha_sdk/model/model_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/page.py` & `semantha_sdk-5.6.1/semantha_sdk/model/page.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/page_content.py` & `semantha_sdk-5.6.1/semantha_sdk/model/page_content.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/paragraph.py` & `semantha_sdk-5.6.1/semantha_sdk/model/paragraph.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/plotly_chart.py` & `semantha_sdk-5.6.1/semantha_sdk/model/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/process_information.py` & `semantha_sdk-5.6.1/semantha_sdk/model/process_information.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/reference.py` & `semantha_sdk-5.6.1/semantha_sdk/model/reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/reference_documents_response_container.py` & `semantha_sdk-5.6.1/semantha_sdk/model/reference_documents_response_container.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/relation.py` & `semantha_sdk-5.6.1/semantha_sdk/model/relation.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/relation_condition.py` & `semantha_sdk-5.6.1/semantha_sdk/model/relation_condition.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/response_meta_info.py` & `semantha_sdk-5.6.1/semantha_sdk/model/response_meta_info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/row.py` & `semantha_sdk-5.6.1/semantha_sdk/model/row.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/rule.py` & `semantha_sdk-5.6.1/semantha_sdk/model/rule.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/rule_function.py` & `semantha_sdk-5.6.1/semantha_sdk/model/rule_function.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/rule_overview.py` & `semantha_sdk-5.6.1/semantha_sdk/model/rule_overview.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/semantha_entity.py` & `semantha_sdk-5.6.1/semantha_sdk/model/semantha_entity.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/semantic_model.py` & `semantha_sdk-5.6.1/semantha_sdk/model/semantic_model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/semi_super_vised_document.py` & `semantha_sdk-5.6.1/semantha_sdk/model/semi_super_vised_document.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/sentence.py` & `semantha_sdk-5.6.1/semantha_sdk/model/sentence.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/settings.py` & `semantha_sdk-5.6.1/semantha_sdk/model/settings.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/smart_cluster_response_container.py` & `semantha_sdk-5.6.1/semantha_sdk/model/smart_cluster_response_container.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py` & `semantha_sdk-5.6.1/semantha_sdk/model/smart_cluster_semi_supervised_request.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/statistic.py` & `semantha_sdk-5.6.1/semantha_sdk/model/statistic.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/synonym.py` & `semantha_sdk-5.6.1/semantha_sdk/model/synonym.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/model/table_instance.py` & `semantha_sdk-5.6.1/semantha_sdk/model/table_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/request/semantha_request.py` & `semantha_sdk-5.6.1/semantha_sdk/request/semantha_request.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/response/semantha_response.py` & `semantha_sdk-5.6.1/semantha_sdk/response/semantha_response.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.6.0/semantha_sdk/rest/rest_client.py` & `semantha_sdk-5.6.1/semantha_sdk/rest/rest_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 def _filter_json(data: dict):
     data = {k: v for k, v in data.items() if v is not None}
     return data
 
 class MediaType:
     XLSX = "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet"
     JSON = "application/json"
+    PDF = "application/pdf"
+    DOCX = "application/vnd.openxmlformats-officedocument.wordprocessingml.document"
     
 class RestClient:
 
     def __init__(self, server_url: str, api_key: str):
         self.__server_url = server_url
         self.__api_key = api_key
```

### Comparing `semantha_sdk-5.6.0/PKG-INFO` & `semantha_sdk-5.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantha-sdk
-Version: 5.6.0
+Version: 5.6.1
 Summary: This is a python client sdk for accessing semantha (the semantic platform)
 Home-page: https://semantha.de
 License: Apache-2.0
 Author: Sebastian Weigelt
 Author-email: sebastian.weigelt@semantha.ai
 Maintainer: semantha support
 Maintainer-email: support@semantha.de
@@ -40,15 +40,16 @@
 
 **IMPORTANT:** The SDK is still under development and interfaces may change at any time without notice.
 Use with caution and on own risk.
 
 ## Update Notes
 
 ### Version 5.6.0
-Adde most endpoints in **/api/models/* **
+Added most endpoints in **/api/models/* **
+SDK covers now 158/180 services.
 
 ### Version 5.5.0
 Removed language parameter on **/api/domains/{domainname}/references**
 Fixed bug on serialization of **/api/domains/{domainname}/modelinstances** response.
 Fixed return of binary responses of bulk services.
 
 ### Version 5.4.0
```

