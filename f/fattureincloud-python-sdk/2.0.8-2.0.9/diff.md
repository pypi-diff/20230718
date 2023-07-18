# Comparing `tmp/fattureincloud-python-sdk-2.0.8.tar.gz` & `tmp/fattureincloud-python-sdk-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fattureincloud-python-sdk-2.0.8.tar", last modified: Tue Jul 19 09:02:37 2022, max compression
+gzip compressed data, was "fattureincloud-python-sdk-2.0.9.tar", last modified: Thu Sep 22 14:35:49 2022, max compression
```

## Comparing `fattureincloud-python-sdk-2.0.8.tar` & `fattureincloud-python-sdk-2.0.9.tar`

### file list

```diff
@@ -1,503 +1,503 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 09:02:36.994613 fattureincloud-python-sdk-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-07-19 09:01:47.000000 fattureincloud-python-sdk-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    35983 2022-07-19 09:02:36.994613 fattureincloud-python-sdk-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    35539 2022-07-19 09:01:47.000000 fattureincloud-python-sdk-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 09:02:36.870612 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 09:02:36.874612 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    34875 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/archive_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    28737 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/cashbook_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    28328 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/clients_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     5872 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/companies_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    78427 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/info_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    68498 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/issued_documents_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    22465 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/issued_e_invoices_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    28348 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/products_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    38910 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/receipts_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    57774 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/received_documents_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    65145 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/settings_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    28601 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/suppliers_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    38772 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/taxes_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     9753 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    38971 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 09:02:36.874612 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/apis/
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16778 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     5278 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 09:02:36.874612 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/filter/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/filter/condition.py
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/filter/conjunction.py
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/filter/disjunction.py
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/filter/expression.py
--rw-r--r--   0 runner    (1001) docker     (121)     3582 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/filter/filter.py
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/filter/operator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 09:02:36.938612 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14253 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/archive_document.py
--rw-r--r--   0 runner    (1001) docker     (121)    12086 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/attachment_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    15647 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/cashbook_entry.py
--rw-r--r--   0 runner    (1001) docker     (121)    12617 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/cashbook_entry_document.py
--rw-r--r--   0 runner    (1001) docker     (121)    12718 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/cashbook_entry_kind.py
--rw-r--r--   0 runner    (1001) docker     (121)    12366 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/cashbook_entry_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    12593 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/city.py
--rw-r--r--   0 runner    (1001) docker     (121)    24386 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    12499 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/client_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    14391 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/company.py
--rw-r--r--   0 runner    (1001) docker     (121)    14603 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/company_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    12829 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/company_info_access_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    13282 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/company_info_plan_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    16985 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/company_info_plan_info_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    12429 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/company_info_plan_info_functions_status.py
--rw-r--r--   0 runner    (1001) docker     (121)    12859 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/company_info_plan_info_limits.py
--rw-r--r--   0 runner    (1001) docker     (121)    12390 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/company_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    13788 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/controlled_company.py
--rw-r--r--   0 runner    (1001) docker     (121)    12167 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_archive_document_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12170 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_archive_document_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12147 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_cashbook_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12150 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_cashbook_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12076 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_client_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12079 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_client_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12046 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_f24_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12049 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_f24_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12578 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_issued_document_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12160 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_issued_document_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12157 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_payment_account_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12160 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_payment_account_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12147 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_payment_method_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12150 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_payment_method_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12086 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_product_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12089 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_product_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12527 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_receipt_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12089 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_receipt_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12636 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_received_document_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12180 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_received_document_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12096 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_supplier_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12099 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_supplier_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12087 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_vat_type_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12090 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_vat_type_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12991 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/currency.py
--rw-r--r--   0 runner    (1001) docker     (121)    12208 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/default_payment_terms_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    13152 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/detailed_country.py
--rw-r--r--   0 runner    (1001) docker     (121)    12584 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/document_template.py
--rw-r--r--   0 runner    (1001) docker     (121)    13265 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/e_invoice_rejection_reason.py
--rw-r--r--   0 runner    (1001) docker     (121)    16634 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/email_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    12299 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/email_data_default_sender_email.py
--rw-r--r--   0 runner    (1001) docker     (121)    14877 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/email_schedule.py
--rw-r--r--   0 runner    (1001) docker     (121)    13520 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/email_schedule_include.py
--rw-r--r--   0 runner    (1001) docker     (121)    23755 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/entity.py
--rw-r--r--   0 runner    (1001) docker     (121)    12499 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/entity_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    14887 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/f24.py
--rw-r--r--   0 runner    (1001) docker     (121)    12430 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/f24_status.py
--rw-r--r--   0 runner    (1001) docker     (121)    11983 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/function_status.py
--rw-r--r--   0 runner    (1001) docker     (121)    12161 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_archive_document_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12141 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_cashbook_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12070 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_client_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12121 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_company_info_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12260 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_e_invoice_rejection_reason_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12101 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_email_data_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12190 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_existing_issued_document_totals_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12253 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_existing_issued_document_totals_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12210 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_existing_received_document_totals_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12273 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_existing_received_document_totals_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12040 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_f24_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12301 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_issued_document_pre_create_info_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12151 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_issued_document_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12175 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_new_issued_document_totals_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12238 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_new_issued_document_totals_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12195 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_new_received_document_totals_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12258 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_new_received_document_totals_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12151 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_payment_account_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12141 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_payment_method_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12080 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_product_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12230 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_receipt_pre_create_info_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12080 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_receipt_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12243 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_receipts_monthly_totals_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12256 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_received_document_pre_create_info_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12171 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_received_document_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12090 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_supplier_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    13178 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_user_info_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12119 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_user_info_response_email_confirmation_state.py
--rw-r--r--   0 runner    (1001) docker     (121)    12910 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_user_info_response_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    12081 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_vat_type_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    46994 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document.py
--rw-r--r--   0 runner    (1001) docker     (121)    16080 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_ei_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    16217 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_extra_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    17693 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_items_list_item.py
--rw-r--r--   0 runner    (1001) docker     (121)    12156 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_options.py
--rw-r--r--   0 runner    (1001) docker     (121)    15084 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_payments_list_item.py
--rw-r--r--   0 runner    (1001) docker     (121)    12606 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_payments_list_item_payment_terms.py
--rw-r--r--   0 runner    (1001) docker     (121)    18269 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_pre_create_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    15760 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_pre_create_info_default_values.py
--rw-r--r--   0 runner    (1001) docker     (121)    13117 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_pre_create_info_extra_data_default_values.py
--rw-r--r--   0 runner    (1001) docker     (121)    12157 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_pre_create_info_items_default_values.py
--rw-r--r--   0 runner    (1001) docker     (121)    12207 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_status.py
--rw-r--r--   0 runner    (1001) docker     (121)    18149 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_totals.py
--rw-r--r--   0 runner    (1001) docker     (121)    13095 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    12291 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/language.py
--rw-r--r--   0 runner    (1001) docker     (121)    12021 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_archive_categories_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    18151 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_archive_documents_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12264 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_archive_documents_response_page.py
--rw-r--r--   0 runner    (1001) docker     (121)    12235 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_cashbook_entries_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12144 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_cities_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    18014 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_clients_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12173 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_clients_response_page.py
--rw-r--r--   0 runner    (1001) docker     (121)    12003 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_cost_centers_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    11997 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_countries_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12184 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_currencies_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12051 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_delivery_notes_default_causals_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12176 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_detailed_countries_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    18719 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_f24_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12061 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_f24_response_aggregated_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    12334 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_f24_response_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (121)    12140 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_f24_response_page.py
--rw-r--r--   0 runner    (1001) docker     (121)    18136 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_issued_documents_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12254 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_issued_documents_response_page.py
--rw-r--r--   0 runner    (1001) docker     (121)    12181 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_languages_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12242 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_payment_accounts_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12232 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_payment_methods_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12021 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_product_categories_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    18029 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_products_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12183 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_products_response_page.py
--rw-r--r--   0 runner    (1001) docker     (121)    18029 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_receipts_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12183 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_receipts_response_page.py
--rw-r--r--   0 runner    (1001) docker     (121)    12048 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_received_document_categories_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    18166 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_received_documents_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12274 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_received_documents_response_page.py
--rw-r--r--   0 runner    (1001) docker     (121)    12012 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_revenue_centers_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    18044 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_suppliers_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12193 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_suppliers_response_page.py
--rw-r--r--   0 runner    (1001) docker     (121)    12238 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_templates_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12012 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_units_of_measure_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12276 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_user_companies_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12223 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_user_companies_response_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    12172 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_vat_types_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12167 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_archive_document_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12170 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_archive_document_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12147 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_cashbook_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12150 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_cashbook_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12076 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_client_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12079 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_client_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12046 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_f24_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12049 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_f24_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12578 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_issued_document_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12160 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_issued_document_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12157 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_payment_account_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12160 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_payment_account_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12147 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_payment_method_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12150 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_payment_method_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12086 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_product_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12089 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_product_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12086 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_receipt_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12089 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_receipt_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12177 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_received_document_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12180 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_received_document_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12096 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_supplier_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12099 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_supplier_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12087 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_vat_type_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12090 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_vat_type_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12675 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/monthly_total.py
--rw-r--r--   0 runner    (1001) docker     (121)    11717 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/numeration.py
--rw-r--r--   0 runner    (1001) docker     (121)    11524 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/numeration_item.py
--rw-r--r--   0 runner    (1001) docker     (121)    12409 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/original_document_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    15257 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/pagination.py
--rw-r--r--   0 runner    (1001) docker     (121)    13995 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/payment_account.py
--rw-r--r--   0 runner    (1001) docker     (121)    12141 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/payment_account_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    15505 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/payment_method.py
--rw-r--r--   0 runner    (1001) docker     (121)    12361 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/payment_method_details.py
--rw-r--r--   0 runner    (1001) docker     (121)    12102 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/payment_method_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    12542 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/permission_level.py
--rw-r--r--   0 runner    (1001) docker     (121)    18977 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)    14435 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/permissions_fic_issued_documents_detailed.py
--rw-r--r--   0 runner    (1001) docker     (121)    18370 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/product.py
--rw-r--r--   0 runner    (1001) docker     (121)    16841 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/receipt.py
--rw-r--r--   0 runner    (1001) docker     (121)    13384 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/receipt_items_list_item.py
--rw-r--r--   0 runner    (1001) docker     (121)    14457 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/receipt_pre_create_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    12438 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/receipt_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    21781 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/received_document.py
--rw-r--r--   0 runner    (1001) docker     (121)    12323 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/received_document_entity.py
--rw-r--r--   0 runner    (1001) docker     (121)    14992 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/received_document_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    12050 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/received_document_info_default_values.py
--rw-r--r--   0 runner    (1001) docker     (121)    12083 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/received_document_info_items_default_values.py
--rw-r--r--   0 runner    (1001) docker     (121)    14892 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/received_document_items_list_item.py
--rw-r--r--   0 runner    (1001) docker     (121)    14391 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/received_document_payments_list_item.py
--rw-r--r--   0 runner    (1001) docker     (121)    12351 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/received_document_payments_list_item_payment_terms.py
--rw-r--r--   0 runner    (1001) docker     (121)    14280 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/received_document_totals.py
--rw-r--r--   0 runner    (1001) docker     (121)    12395 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/received_document_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    12129 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/schedule_email_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12216 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/send_e_invoice_request.py
--rw-r--r--   0 runner    (1001) docker     (121)    12680 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/send_e_invoice_request_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    12226 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/send_e_invoice_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12339 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/send_e_invoice_response_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    12251 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/sender_email.py
--rw-r--r--   0 runner    (1001) docker     (121)    12093 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/show_totals_mode.py
--rw-r--r--   0 runner    (1001) docker     (121)    19100 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/supplier.py
--rw-r--r--   0 runner    (1001) docker     (121)    12513 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/supplier_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    12169 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/upload_archive_attachment_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12157 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/upload_f24_attachment_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12190 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/upload_issued_document_attachment_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12196 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/upload_received_document_attachment_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    13813 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/user.py
--rw-r--r--   0 runner    (1001) docker     (121)    12560 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/user_company_role.py
--rw-r--r--   0 runner    (1001) docker     (121)    12278 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/vat_item.py
--rw-r--r--   0 runner    (1001) docker     (121)    12476 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/vat_kind.py
--rw-r--r--   0 runner    (1001) docker     (121)    11673 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/vat_list.py
--rw-r--r--   0 runner    (1001) docker     (121)    14809 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/vat_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    12881 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/verify_e_invoice_xml_error_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12568 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/verify_e_invoice_xml_error_response_error.py
--rw-r--r--   0 runner    (1001) docker     (121)    12049 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/verify_e_invoice_xml_error_response_extra.py
--rw-r--r--   0 runner    (1001) docker     (121)    12277 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/verify_e_invoice_xml_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12113 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/verify_e_invoice_xml_response_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    82198 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 09:02:36.938612 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (121)    21630 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 09:02:36.942612 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/oauth2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/oauth2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4206 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/oauth2/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (121)     3346 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/oauth2/scopes.py
--rw-r--r--   0 runner    (1001) docker     (121)    14756 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 09:02:36.870612 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    35983 2022-07-19 09:02:36.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    23916 2022-07-19 09:02:36.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-19 09:02:36.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-07-19 09:02:36.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-07-19 09:02:36.000000 fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-07-19 09:02:36.994613 fattureincloud-python-sdk-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 09:02:36.994613 fattureincloud-python-sdk-2.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)     8096 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_archive_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_archive_document.py
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_attachment_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     9023 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_cashbook_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2587 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_cashbook_entry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_cashbook_entry_document.py
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_cashbook_entry_kind.py
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_cashbook_entry_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_city.py
--rw-r--r--   0 runner    (1001) docker     (121)     6253 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_client_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    28786 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_clients_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4079 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_companies_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2683 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_company.py
--rw-r--r--   0 runner    (1001) docker     (121)     3511 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_company_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1680 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_company_info_access_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     2549 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_company_info_plan_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_company_info_plan_info_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_company_info_plan_info_functions_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_company_info_plan_info_limits.py
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_company_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_condition.py
--rw-r--r--   0 runner    (1001) docker     (121)     2800 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_conjunction.py
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_controlled_company.py
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_archive_document_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     1875 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_archive_document_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_cashbook_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2663 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_cashbook_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     6568 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_client_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     6561 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_client_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2490 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_f24_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2497 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_f24_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2738 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_issued_document_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2745 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_issued_document_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1914 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_payment_account_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     1921 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_payment_account_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3175 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_payment_method_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     3182 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_payment_method_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3141 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_product_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     3157 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_product_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4273 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_receipt_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     4289 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_receipt_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     5158 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_received_document_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     4627 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_received_document_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3050 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_supplier_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     3057 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_supplier_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1908 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_vat_type_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     1924 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_create_vat_type_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_currency.py
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_default_payment_terms_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_detailed_country.py
--rw-r--r--   0 runner    (1001) docker     (121)     2797 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_disjunction.py
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_document_template.py
--rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_e_invoice_rejection_reason.py
--rw-r--r--   0 runner    (1001) docker     (121)     2412 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_email_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_email_data_default_sender_email.py
--rw-r--r--   0 runner    (1001) docker     (121)     2043 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_email_schedule.py
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_email_schedule_include.py
--rw-r--r--   0 runner    (1001) docker     (121)     6510 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     2841 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_f24.py
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_f24_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     7131 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_function_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_archive_document_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2468 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_cashbook_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     6554 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_client_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3700 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_company_info_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_e_invoice_rejection_reason_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2585 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_email_data_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2817 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_existing_issued_document_totals_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2075 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_existing_issued_document_totals_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4700 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_existing_received_document_totals_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_existing_received_document_totals_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2476 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_f24_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3553 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_issued_document_pre_create_info_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2724 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_issued_document_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2782 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_new_issued_document_totals_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2040 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_new_issued_document_totals_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4664 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_new_received_document_totals_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2073 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_new_received_document_totals_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_payment_account_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3161 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_payment_method_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3127 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_product_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2097 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_receipt_pre_create_info_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4259 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_receipt_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_receipts_monthly_totals_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2582 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_received_document_pre_create_info_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4606 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_received_document_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3027 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_supplier_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2421 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_user_info_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_user_info_response_email_confirmation_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_user_info_response_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_get_vat_type_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    17687 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_info_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     5242 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_issued_document.py
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_issued_document_ei_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_issued_document_extra_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2778 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_issued_document_items_list_item.py
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_issued_document_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     3020 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_issued_document_payments_list_item.py
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_issued_document_payments_list_item_payment_terms.py
--rw-r--r--   0 runner    (1001) docker     (121)     3972 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_issued_document_pre_create_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_issued_document_pre_create_info_default_values.py
--rw-r--r--   0 runner    (1001) docker     (121)     1668 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_issued_document_pre_create_info_extra_data_default_values.py
--rw-r--r--   0 runner    (1001) docker     (121)     2094 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_issued_document_pre_create_info_items_default_values.py
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_issued_document_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_issued_document_totals.py
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_issued_document_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    21276 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_issued_documents_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     3765 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_issued_e_invoices_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_language.py
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_archive_categories_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3297 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_archive_documents_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2442 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_archive_documents_response_page.py
--rw-r--r--   0 runner    (1001) docker     (121)     3140 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_cashbook_entries_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2152 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_cities_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     7713 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_clients_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     6970 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_clients_response_page.py
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_cost_centers_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_countries_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_currencies_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_delivery_notes_default_causals_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_detailed_countries_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4938 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_f24_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_f24_response_aggregated_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_f24_response_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3774 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_f24_response_page.py
--rw-r--r--   0 runner    (1001) docker     (121)     5070 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_issued_documents_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4219 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_issued_documents_response_page.py
--rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_languages_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_payment_accounts_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4887 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_payment_methods_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_product_categories_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     6053 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_products_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     5240 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_products_response_page.py
--rw-r--r--   0 runner    (1001) docker     (121)     8073 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_receipts_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     7260 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_receipts_response_page.py
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_received_document_categories_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     5801 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_received_documents_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4863 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_received_documents_response_page.py
--rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_revenue_centers_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     5791 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_suppliers_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4965 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_suppliers_response_page.py
--rw-r--r--   0 runner    (1001) docker     (121)     1623 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_templates_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_units_of_measure_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     5141 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_user_companies_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4721 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_user_companies_response_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2627 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_list_vat_types_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_archive_document_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     1875 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_archive_document_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2481 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_cashbook_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2488 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_cashbook_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     6568 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_client_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     6575 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_client_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2489 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_f24_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2497 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_f24_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2737 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_issued_document_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2745 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_issued_document_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1914 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_payment_account_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     1921 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_payment_account_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3174 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_payment_method_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     3182 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_payment_method_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3141 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_product_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     3157 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_product_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4272 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_receipt_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     4288 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_receipt_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4619 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_received_document_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     4626 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_received_document_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3050 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_supplier_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     3057 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_supplier_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1908 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_vat_type_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     1924 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_modify_vat_type_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_monthly_total.py
--rw-r--r--   0 runner    (1001) docker     (121)     1376 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_numeration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_numeration_item.py
--rw-r--r--   0 runner    (1001) docker     (121)     5983 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (121)      893 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_operator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_original_document_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_pagination.py
--rw-r--r--   0 runner    (1001) docker     (121)     1660 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_payment_account.py
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_payment_account_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     2962 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_payment_method.py
--rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_payment_method_details.py
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_payment_method_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_permission_level.py
--rw-r--r--   0 runner    (1001) docker     (121)     4311 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2165 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_permissions_fic_issued_documents_detailed.py
--rw-r--r--   0 runner    (1001) docker     (121)     2830 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_product.py
--rw-r--r--   0 runner    (1001) docker     (121)    13661 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_products_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4020 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_receipt.py
--rw-r--r--   0 runner    (1001) docker     (121)     2109 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_receipt_items_list_item.py
--rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_receipt_pre_create_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_receipt_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    17834 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_receipts_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6101 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_received_document.py
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_received_document_entity.py
--rw-r--r--   0 runner    (1001) docker     (121)     2550 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_received_document_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_received_document_info_default_values.py
--rw-r--r--   0 runner    (1001) docker     (121)     1354 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_received_document_info_items_default_values.py
--rw-r--r--   0 runner    (1001) docker     (121)     2427 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_received_document_items_list_item.py
--rw-r--r--   0 runner    (1001) docker     (121)     2131 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_received_document_payments_list_item.py
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_received_document_payments_list_item_payment_terms.py
--rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_received_document_totals.py
--rw-r--r--   0 runner    (1001) docker     (121)     1164 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_received_document_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    26117 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_received_documents_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2260 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_schedule_email_request.py
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_scopes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_send_e_invoice_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_send_e_invoice_request_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_send_e_invoice_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_send_e_invoice_response_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_sender_email.py
--rw-r--r--   0 runner    (1001) docker     (121)    17335 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_settings_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_show_totals_mode.py
--rw-r--r--   0 runner    (1001) docker     (121)     2755 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_supplier.py
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_supplier_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    13078 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_suppliers_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    10352 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_taxes_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1541 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_upload_archive_attachment_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_upload_f24_attachment_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_upload_issued_document_attachment_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_upload_received_document_attachment_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1685 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (121)     5503 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_user_company_role.py
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_vat_item.py
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_vat_kind.py
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_vat_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_vat_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_verify_e_invoice_xml_error_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_verify_e_invoice_xml_error_response_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     1352 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_verify_e_invoice_xml_error_response_extra.py
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_verify_e_invoice_xml_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-07-19 09:01:48.000000 fattureincloud-python-sdk-2.0.8/test/test_verify_e_invoice_xml_response_data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 14:35:49.953003 fattureincloud-python-sdk-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    36467 2022-09-22 14:35:49.953003 fattureincloud-python-sdk-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    36023 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 14:35:49.865002 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 14:35:49.869002 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34875 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/archive_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28737 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/cashbook_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28328 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/clients_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5872 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/companies_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    78427 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/info_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68498 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/issued_documents_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22465 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/issued_e_invoices_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28348 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/products_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38910 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/receipts_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    57774 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/received_documents_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    65145 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/settings_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28601 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/suppliers_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38772 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/taxes_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9753 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38971 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 14:35:49.869002 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/apis/
+-rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16778 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5278 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 14:35:49.873002 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/filter/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/filter/condition.py
+-rw-r--r--   0 runner    (1001) docker     (121)      903 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/filter/conjunction.py
+-rw-r--r--   0 runner    (1001) docker     (121)      902 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/filter/disjunction.py
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/filter/expression.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3582 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/filter/filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/filter/operator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 14:35:49.917003 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14253 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/archive_document.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12086 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/attachment_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15647 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/cashbook_entry.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12617 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/cashbook_entry_document.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12718 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/cashbook_entry_kind.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12366 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/cashbook_entry_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12593 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/city.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24319 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12499 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/client_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14391 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/company.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14603 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/company_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12829 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/company_info_access_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13282 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/company_info_plan_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16985 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/company_info_plan_info_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12429 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/company_info_plan_info_functions_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12859 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/company_info_plan_info_limits.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12390 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/company_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13788 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/controlled_company.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12167 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_archive_document_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12170 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_archive_document_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12147 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_cashbook_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12150 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_cashbook_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12076 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_client_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12079 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_client_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12046 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_f24_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12049 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_f24_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12578 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_issued_document_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12160 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_issued_document_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12157 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_payment_account_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12160 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_payment_account_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12147 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_payment_method_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12150 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_payment_method_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12086 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_product_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12089 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_product_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12527 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_receipt_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12089 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_receipt_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12636 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_received_document_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12180 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_received_document_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12096 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_supplier_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12099 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_supplier_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12087 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_vat_type_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12090 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_vat_type_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12991 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/currency.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13152 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/detailed_country.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12584 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/document_template.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13265 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/e_invoice_rejection_reason.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16634 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/email_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12299 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/email_data_default_sender_email.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14877 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/email_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13520 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/email_schedule_include.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23688 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/entity.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12499 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14887 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/f24.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12430 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/f24_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11983 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/function_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12161 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_archive_document_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12141 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_cashbook_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12070 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_client_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12121 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_company_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12260 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_e_invoice_rejection_reason_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12101 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_email_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12190 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_existing_issued_document_totals_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12253 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_existing_issued_document_totals_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12210 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_existing_received_document_totals_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12273 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_existing_received_document_totals_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12040 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_f24_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12301 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_issued_document_pre_create_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12151 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_issued_document_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12175 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_new_issued_document_totals_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12238 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_new_issued_document_totals_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12195 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_new_received_document_totals_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12258 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_new_received_document_totals_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12151 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_payment_account_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12141 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_payment_method_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12080 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_product_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12230 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_receipt_pre_create_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12080 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_receipt_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12243 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_receipts_monthly_totals_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12256 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_received_document_pre_create_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12171 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_received_document_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12090 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_supplier_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13178 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_user_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12119 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_user_info_response_email_confirmation_state.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12910 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_user_info_response_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12081 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_vat_type_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46994 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16080 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_ei_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16217 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_extra_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17693 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_items_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12156 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15084 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_payments_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12584 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_payments_list_item_payment_terms.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18734 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_pre_create_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15760 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_pre_create_info_default_values.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13117 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_pre_create_info_extra_data_default_values.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12157 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_pre_create_info_items_default_values.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12207 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18149 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_totals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13095 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12291 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/language.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12021 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_archive_categories_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18151 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_archive_documents_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12264 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_archive_documents_response_page.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12235 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_cashbook_entries_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12144 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_cities_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18014 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_clients_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12173 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_clients_response_page.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12003 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_cost_centers_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11997 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_countries_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12184 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_currencies_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12051 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_delivery_notes_default_causals_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12176 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_detailed_countries_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18719 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_f24_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12061 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_f24_response_aggregated_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12334 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_f24_response_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12140 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_f24_response_page.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18136 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_issued_documents_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12254 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_issued_documents_response_page.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12181 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_languages_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12242 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_payment_accounts_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12232 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_payment_methods_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12021 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_product_categories_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18029 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_products_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12183 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_products_response_page.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18029 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_receipts_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12183 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_receipts_response_page.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12048 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_received_document_categories_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18166 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_received_documents_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12274 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_received_documents_response_page.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12012 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_revenue_centers_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18044 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_suppliers_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12193 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_suppliers_response_page.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12238 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_templates_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12012 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_units_of_measure_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12276 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_user_companies_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12223 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_user_companies_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12172 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_vat_types_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12167 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_archive_document_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12170 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_archive_document_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12147 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_cashbook_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12150 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_cashbook_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12076 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_client_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12079 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_client_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12046 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_f24_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12049 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_f24_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12578 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_issued_document_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12160 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_issued_document_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12157 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_payment_account_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12160 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_payment_account_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12147 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_payment_method_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12150 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_payment_method_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12086 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_product_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12089 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_product_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12086 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_receipt_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12089 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_receipt_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12177 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_received_document_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12180 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_received_document_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12096 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_supplier_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12099 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_supplier_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12087 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_vat_type_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12090 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_vat_type_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12675 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/monthly_total.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11717 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/numeration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11524 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/numeration_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12409 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/original_document_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15257 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13995 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/payment_account.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12141 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/payment_account_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15505 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12361 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/payment_method_details.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12102 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/payment_method_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12175 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/payment_terms_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12542 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/permission_level.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18977 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14435 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/permissions_fic_issued_documents_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18370 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/product.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16841 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/receipt.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13384 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/receipt_items_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14457 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/receipt_pre_create_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12438 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/receipt_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22355 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/received_document.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12323 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/received_document_entity.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14992 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/received_document_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12050 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/received_document_info_default_values.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12083 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/received_document_info_items_default_values.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14892 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/received_document_items_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14391 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/received_document_payments_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12351 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/received_document_payments_list_item_payment_terms.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14280 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/received_document_totals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12395 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/received_document_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12129 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/schedule_email_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12216 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/send_e_invoice_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12680 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/send_e_invoice_request_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12226 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/send_e_invoice_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12339 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/send_e_invoice_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12251 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/sender_email.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12093 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/show_totals_mode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19100 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/supplier.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12513 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/supplier_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12169 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/upload_archive_attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12157 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/upload_f24_attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12190 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/upload_issued_document_attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12196 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/upload_received_document_attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13813 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12560 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/user_company_role.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12278 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/vat_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12476 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/vat_kind.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11673 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/vat_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14809 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/vat_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12881 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/verify_e_invoice_xml_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12568 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/verify_e_invoice_xml_error_response_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12049 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/verify_e_invoice_xml_error_response_extra.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12277 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/verify_e_invoice_xml_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12113 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/verify_e_invoice_xml_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    82215 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 14:35:49.917003 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (121)    21606 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 14:35:49.917003 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/oauth2/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/oauth2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4206 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/oauth2/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4120 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/oauth2/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14756 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 14:35:49.865002 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    36467 2022-09-22 14:35:49.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    23900 2022-09-22 14:35:49.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 14:35:49.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-09-22 14:35:49.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-09-22 14:35:49.000000 fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-22 14:35:49.953003 fattureincloud-python-sdk-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 14:35:49.953003 fattureincloud-python-sdk-2.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     8096 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_archive_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_archive_document.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_attachment_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9023 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_cashbook_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2587 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_cashbook_entry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_cashbook_entry_document.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_cashbook_entry_kind.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_cashbook_entry_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_city.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6209 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_client_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28728 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_clients_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4079 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_companies_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2683 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_company.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3511 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_company_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1680 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_company_info_access_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2549 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_company_info_plan_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1413 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_company_info_plan_info_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_company_info_plan_info_functions_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_company_info_plan_info_limits.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_company_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_condition.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2800 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_conjunction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_controlled_company.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_archive_document_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1875 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_archive_document_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_cashbook_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2663 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_cashbook_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6538 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_client_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6531 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_client_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2490 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_f24_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2497 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_f24_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2738 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_issued_document_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2745 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_issued_document_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1914 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_payment_account_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1921 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_payment_account_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3175 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_payment_method_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3182 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_payment_method_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3141 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_product_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3157 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_product_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4273 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_receipt_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4289 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_receipt_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5158 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_received_document_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4627 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_received_document_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3050 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_supplier_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3057 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_supplier_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1908 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_vat_type_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1924 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_create_vat_type_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_currency.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_detailed_country.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2797 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_disjunction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_document_template.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_e_invoice_rejection_reason.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2412 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_email_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_email_data_default_sender_email.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2043 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_email_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_email_schedule_include.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6466 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2841 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_f24.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_f24_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7131 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_function_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_archive_document_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2468 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_cashbook_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6524 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_client_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3700 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_company_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_e_invoice_rejection_reason_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2585 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_email_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2817 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_existing_issued_document_totals_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2075 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_existing_issued_document_totals_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4700 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_existing_received_document_totals_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_existing_received_document_totals_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2476 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_f24_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3553 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_issued_document_pre_create_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2724 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_issued_document_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2782 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_new_issued_document_totals_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2040 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_new_issued_document_totals_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4664 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_new_received_document_totals_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2073 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_new_received_document_totals_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_payment_account_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3161 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_payment_method_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3127 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_product_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2097 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_receipt_pre_create_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4259 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_receipt_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_receipts_monthly_totals_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2582 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_received_document_pre_create_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4606 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_received_document_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3027 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_supplier_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2421 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_user_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_user_info_response_email_confirmation_state.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_user_info_response_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_get_vat_type_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17687 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5242 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_issued_document.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_issued_document_ei_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_issued_document_extra_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2778 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_issued_document_items_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_issued_document_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3020 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_issued_document_payments_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1466 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_issued_document_payments_list_item_payment_terms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3972 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_issued_document_pre_create_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_issued_document_pre_create_info_default_values.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1668 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_issued_document_pre_create_info_extra_data_default_values.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2094 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_issued_document_pre_create_info_items_default_values.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_issued_document_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_issued_document_totals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_issued_document_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21276 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_issued_documents_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3765 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_issued_e_invoices_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_language.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_archive_categories_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3297 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_archive_documents_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2442 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_archive_documents_response_page.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3140 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_cashbook_entries_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2152 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_cities_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7682 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_clients_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6939 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_clients_response_page.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_cost_centers_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_countries_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_currencies_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_delivery_notes_default_causals_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_detailed_countries_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4938 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_f24_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_f24_response_aggregated_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_f24_response_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3774 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_f24_response_page.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5070 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_issued_documents_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4219 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_issued_documents_response_page.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_languages_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_payment_accounts_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4887 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_payment_methods_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_product_categories_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6053 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_products_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5240 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_products_response_page.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8073 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_receipts_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7260 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_receipts_response_page.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_received_document_categories_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5801 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_received_documents_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4863 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_received_documents_response_page.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_revenue_centers_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5791 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_suppliers_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4965 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_suppliers_response_page.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1623 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_templates_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_units_of_measure_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5141 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_user_companies_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4721 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_user_companies_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2627 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_list_vat_types_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_archive_document_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1875 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_archive_document_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2481 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_cashbook_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2488 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_cashbook_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6537 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_client_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6544 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_client_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2489 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_f24_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2497 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_f24_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2737 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_issued_document_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2745 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_issued_document_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1914 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_payment_account_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1921 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_payment_account_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3174 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_payment_method_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3182 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_payment_method_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3141 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_product_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3157 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_product_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4272 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_receipt_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4288 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_receipt_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4619 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_received_document_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4626 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_received_document_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3050 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_supplier_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3057 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_supplier_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1908 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_vat_type_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1924 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_modify_vat_type_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_monthly_total.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1376 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_numeration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_numeration_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5983 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      893 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_operator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_original_document_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1660 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_payment_account.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_payment_account_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2962 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_payment_method_details.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_payment_method_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_payment_terms_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_permission_level.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4311 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2165 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_permissions_fic_issued_documents_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2830 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_product.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13661 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_products_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4020 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2109 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_receipt_items_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_receipt_pre_create_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_receipt_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17834 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_receipts_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6101 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_received_document.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_received_document_entity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2550 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_received_document_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_received_document_info_default_values.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1354 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_received_document_info_items_default_values.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2427 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_received_document_items_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2131 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_received_document_payments_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_received_document_payments_list_item_payment_terms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_received_document_totals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1164 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_received_document_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26117 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_received_documents_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2260 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_schedule_email_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_send_e_invoice_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_send_e_invoice_request_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_send_e_invoice_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_send_e_invoice_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_sender_email.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17335 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_settings_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_show_totals_mode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2755 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_supplier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_supplier_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13078 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_suppliers_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10352 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_taxes_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1541 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_upload_archive_attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_upload_f24_attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_upload_issued_document_attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_upload_received_document_attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1685 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5503 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_user_company_role.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_vat_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_vat_kind.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_vat_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_vat_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_verify_e_invoice_xml_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_verify_e_invoice_xml_error_response_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1352 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_verify_e_invoice_xml_error_response_extra.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_verify_e_invoice_xml_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-09-22 14:34:59.000000 fattureincloud-python-sdk-2.0.9/test/test_verify_e_invoice_xml_response_data.py
```

### Comparing `fattureincloud-python-sdk-2.0.8/LICENSE` & `fattureincloud-python-sdk-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/PKG-INFO` & `fattureincloud-python-sdk-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fattureincloud-python-sdk
-Version: 2.0.8
+Version: 2.0.9
 Summary: Python SDK for the Fatture in Cloud API
 Home-page: https://github.com/fattureincloud/fattureincloud-python-sdk
 Author: Fatture in Cloud
 Author-email: info@fattureincloud.it
 License: MIT
 Keywords: fattureincloud,fatture in cloud,fatture,fic,fattureincloud sdk,fatture in cloud sdk
 Requires-Python: >=3.6
@@ -17,16 +17,16 @@
 
 Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy. 
 
 The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2.0.19
-- Package version: 2.0.8
+- API version: 2.0.20
+- Package version: 2.0.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.fattureincloud.it](https://www.fattureincloud.it)
 
 ## Requirements.
 
 Python >= 3.6
 
@@ -58,14 +58,24 @@
 from fattureincloud_python_sdk.model.create_archive_document_request import CreateArchiveDocumentRequest
 from fattureincloud_python_sdk.model.create_archive_document_response import CreateArchiveDocumentResponse
 from fattureincloud_python_sdk.model.get_archive_document_response import GetArchiveDocumentResponse
 from fattureincloud_python_sdk.model.list_archive_documents_response import ListArchiveDocumentsResponse
 from fattureincloud_python_sdk.model.modify_archive_document_request import ModifyArchiveDocumentRequest
 from fattureincloud_python_sdk.model.modify_archive_document_response import ModifyArchiveDocumentResponse
 from fattureincloud_python_sdk.model.upload_archive_attachment_response import UploadArchiveAttachmentResponse
+# Defining the host is optional and defaults to https://api-v2.fattureincloud.it
+# See configuration.py for a list of all supported configuration parameters.
+configuration = fattureincloud_python_sdk.Configuration(
+    host = "https://api-v2.fattureincloud.it"
+)
+
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
 
 # Configure OAuth2 access token for authorization: OAuth2AuthenticationCodeFlow
 configuration = fattureincloud_python_sdk.Configuration(
     access_token = "YOUR_ACCESS_TOKEN"
 )
 
 
@@ -238,15 +248,14 @@
  - [CreateReceivedDocumentRequest](docs/CreateReceivedDocumentRequest.md)
  - [CreateReceivedDocumentResponse](docs/CreateReceivedDocumentResponse.md)
  - [CreateSupplierRequest](docs/CreateSupplierRequest.md)
  - [CreateSupplierResponse](docs/CreateSupplierResponse.md)
  - [CreateVatTypeRequest](docs/CreateVatTypeRequest.md)
  - [CreateVatTypeResponse](docs/CreateVatTypeResponse.md)
  - [Currency](docs/Currency.md)
- - [DefaultPaymentTermsType](docs/DefaultPaymentTermsType.md)
  - [DetailedCountry](docs/DetailedCountry.md)
  - [DocumentTemplate](docs/DocumentTemplate.md)
  - [EInvoiceRejectionReason](docs/EInvoiceRejectionReason.md)
  - [EmailData](docs/EmailData.md)
  - [EmailDataDefaultSenderEmail](docs/EmailDataDefaultSenderEmail.md)
  - [EmailSchedule](docs/EmailSchedule.md)
  - [EmailScheduleInclude](docs/EmailScheduleInclude.md)
@@ -367,14 +376,15 @@
  - [OriginalDocumentType](docs/OriginalDocumentType.md)
  - [Pagination](docs/Pagination.md)
  - [PaymentAccount](docs/PaymentAccount.md)
  - [PaymentAccountType](docs/PaymentAccountType.md)
  - [PaymentMethod](docs/PaymentMethod.md)
  - [PaymentMethodDetails](docs/PaymentMethodDetails.md)
  - [PaymentMethodType](docs/PaymentMethodType.md)
+ - [PaymentTermsType](docs/PaymentTermsType.md)
  - [PermissionLevel](docs/PermissionLevel.md)
  - [Permissions](docs/Permissions.md)
  - [PermissionsFicIssuedDocumentsDetailed](docs/PermissionsFicIssuedDocumentsDetailed.md)
  - [Product](docs/Product.md)
  - [Receipt](docs/Receipt.md)
  - [ReceiptItemsListItem](docs/ReceiptItemsListItem.md)
  - [ReceiptPreCreateInfo](docs/ReceiptPreCreateInfo.md)
```

### Comparing `fattureincloud-python-sdk-2.0.8/README.md` & `fattureincloud-python-sdk-2.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy. 
 
 The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2.0.19
-- Package version: 2.0.8
+- API version: 2.0.20
+- Package version: 2.0.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.fattureincloud.it](https://www.fattureincloud.it)
 
 ## Requirements.
 
 Python >= 3.6
 
@@ -45,14 +45,24 @@
 from fattureincloud_python_sdk.model.create_archive_document_request import CreateArchiveDocumentRequest
 from fattureincloud_python_sdk.model.create_archive_document_response import CreateArchiveDocumentResponse
 from fattureincloud_python_sdk.model.get_archive_document_response import GetArchiveDocumentResponse
 from fattureincloud_python_sdk.model.list_archive_documents_response import ListArchiveDocumentsResponse
 from fattureincloud_python_sdk.model.modify_archive_document_request import ModifyArchiveDocumentRequest
 from fattureincloud_python_sdk.model.modify_archive_document_response import ModifyArchiveDocumentResponse
 from fattureincloud_python_sdk.model.upload_archive_attachment_response import UploadArchiveAttachmentResponse
+# Defining the host is optional and defaults to https://api-v2.fattureincloud.it
+# See configuration.py for a list of all supported configuration parameters.
+configuration = fattureincloud_python_sdk.Configuration(
+    host = "https://api-v2.fattureincloud.it"
+)
+
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
 
 # Configure OAuth2 access token for authorization: OAuth2AuthenticationCodeFlow
 configuration = fattureincloud_python_sdk.Configuration(
     access_token = "YOUR_ACCESS_TOKEN"
 )
 
 
@@ -225,15 +235,14 @@
  - [CreateReceivedDocumentRequest](docs/CreateReceivedDocumentRequest.md)
  - [CreateReceivedDocumentResponse](docs/CreateReceivedDocumentResponse.md)
  - [CreateSupplierRequest](docs/CreateSupplierRequest.md)
  - [CreateSupplierResponse](docs/CreateSupplierResponse.md)
  - [CreateVatTypeRequest](docs/CreateVatTypeRequest.md)
  - [CreateVatTypeResponse](docs/CreateVatTypeResponse.md)
  - [Currency](docs/Currency.md)
- - [DefaultPaymentTermsType](docs/DefaultPaymentTermsType.md)
  - [DetailedCountry](docs/DetailedCountry.md)
  - [DocumentTemplate](docs/DocumentTemplate.md)
  - [EInvoiceRejectionReason](docs/EInvoiceRejectionReason.md)
  - [EmailData](docs/EmailData.md)
  - [EmailDataDefaultSenderEmail](docs/EmailDataDefaultSenderEmail.md)
  - [EmailSchedule](docs/EmailSchedule.md)
  - [EmailScheduleInclude](docs/EmailScheduleInclude.md)
@@ -354,14 +363,15 @@
  - [OriginalDocumentType](docs/OriginalDocumentType.md)
  - [Pagination](docs/Pagination.md)
  - [PaymentAccount](docs/PaymentAccount.md)
  - [PaymentAccountType](docs/PaymentAccountType.md)
  - [PaymentMethod](docs/PaymentMethod.md)
  - [PaymentMethodDetails](docs/PaymentMethodDetails.md)
  - [PaymentMethodType](docs/PaymentMethodType.md)
+ - [PaymentTermsType](docs/PaymentTermsType.md)
  - [PermissionLevel](docs/PermissionLevel.md)
  - [Permissions](docs/Permissions.md)
  - [PermissionsFicIssuedDocumentsDetailed](docs/PermissionsFicIssuedDocumentsDetailed.md)
  - [Product](docs/Product.md)
  - [Receipt](docs/Receipt.md)
  - [ReceiptItemsListItem](docs/ReceiptItemsListItem.md)
  - [ReceiptPreCreateInfo](docs/ReceiptPreCreateInfo.md)
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/__init__.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # flake8: noqa
 
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 # import ApiClient
 from fattureincloud_python_sdk.api_client import ApiClient
 
 # import Configuration
 from fattureincloud_python_sdk.configuration import Configuration
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/archive_api.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/archive_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/cashbook_api.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/cashbook_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/clients_api.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/clients_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/companies_api.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/companies_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/info_api.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/info_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/issued_documents_api.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/issued_documents_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/issued_e_invoices_api.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/issued_e_invoices_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/products_api.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/products_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/receipts_api.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/receipts_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/received_documents_api.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/received_documents_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/settings_api.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/settings_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/suppliers_api.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/suppliers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/taxes_api.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/taxes_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api/user_api.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api/user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/api_client.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
@@ -83,15 +83,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = "FattureInCloud/2.0.8/Python-SDK"
+        self.user_agent = "FattureInCloud/2.0.9/Python-SDK"
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/apis/__init__.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/configuration.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
@@ -399,16 +399,16 @@
 
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
-            "Version of the API: 2.0.19\n"
-            "SDK Package Version: 2.0.8".format(env=sys.platform, pyversion=sys.version)
+            "Version of the API: 2.0.20\n"
+            "SDK Package Version: 2.0.9".format(env=sys.platform, pyversion=sys.version)
         )
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/exceptions.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/filter/condition.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/filter/condition.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/filter/conjunction.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/filter/conjunction.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/filter/disjunction.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/filter/disjunction.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/filter/filter.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/filter/filter.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/archive_document.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/archive_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/attachment_data.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/attachment_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/cashbook_entry.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/cashbook_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/cashbook_entry_document.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/cashbook_entry_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/cashbook_entry_kind.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/cashbook_entry_kind.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/cashbook_entry_type.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/cashbook_entry_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/city.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/city.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/client.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -28,23 +28,21 @@
     OpenApiModel,
 )
 from fattureincloud_python_sdk.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from fattureincloud_python_sdk.model.client_type import ClientType
-    from fattureincloud_python_sdk.model.default_payment_terms_type import (
-        DefaultPaymentTermsType,
-    )
     from fattureincloud_python_sdk.model.payment_method import PaymentMethod
+    from fattureincloud_python_sdk.model.payment_terms_type import PaymentTermsType
     from fattureincloud_python_sdk.model.vat_type import VatType
 
     globals()["ClientType"] = ClientType
-    globals()["DefaultPaymentTermsType"] = DefaultPaymentTermsType
     globals()["PaymentMethod"] = PaymentMethod
+    globals()["PaymentTermsType"] = PaymentTermsType
     globals()["VatType"] = VatType
 
 
 class Client(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -183,15 +181,15 @@
                 none_type,
             ),  # noqa: E501
             "default_vat": (VatType,),  # noqa: E501
             "default_payment_terms": (
                 int,
                 none_type,
             ),  # noqa: E501
-            "default_payment_terms_type": (DefaultPaymentTermsType,),  # noqa: E501
+            "default_payment_terms_type": (PaymentTermsType,),  # noqa: E501
             "default_payment_method": (PaymentMethod,),  # noqa: E501
             "bank_name": (
                 str,
                 none_type,
             ),  # noqa: E501
             "bank_iban": (
                 str,
@@ -222,19 +220,19 @@
                 none_type,
             ),  # noqa: E501
             "has_intent_declaration": (
                 bool,
                 none_type,
             ),  # noqa: E501
             "intent_declaration_protocol_number": (
-                date,
+                str,
                 none_type,
             ),  # noqa: E501
             "intent_declaration_protocol_date": (
-                str,
+                date,
                 none_type,
             ),  # noqa: E501
             "created_at": (
                 str,
                 none_type,
             ),  # noqa: E501
             "updated_at": (
@@ -345,27 +343,27 @@
             email (str, none_type): Client email.. [optional]  # noqa: E501
             certified_email (str, none_type): Client certified email.. [optional]  # noqa: E501
             phone (str, none_type): Client phone.. [optional]  # noqa: E501
             fax (str, none_type): Client fax.. [optional]  # noqa: E501
             notes (str, none_type): Extra notes.. [optional]  # noqa: E501
             default_vat (VatType): [optional]  # noqa: E501
             default_payment_terms (int, none_type): [optional]  # noqa: E501
-            default_payment_terms_type (DefaultPaymentTermsType): [optional]  # noqa: E501
+            default_payment_terms_type (PaymentTermsType): [optional]  # noqa: E501
             default_payment_method (PaymentMethod): [optional]  # noqa: E501
             bank_name (str, none_type): Client bank name.. [optional]  # noqa: E501
             bank_iban (str, none_type): Client iban.. [optional]  # noqa: E501
             bank_swift_code (str, none_type): Client bank swift code.. [optional]  # noqa: E501
             shipping_address (str, none_type): Client shipping address.. [optional]  # noqa: E501
             e_invoice (bool, none_type): Use e-invoices for this entity. [optional]  # noqa: E501
             ei_code (str, none_type): E-invoice code. [optional]  # noqa: E501
             discount_highlight (bool, none_type): Discount Highlight.. [optional]  # noqa: E501
             default_discount (float, none_type): Default discount.. [optional]  # noqa: E501
             has_intent_declaration (bool, none_type): Has intent declaration.. [optional]  # noqa: E501
-            intent_declaration_protocol_number (date, none_type): Intent declaration protocol number.. [optional]  # noqa: E501
-            intent_declaration_protocol_date (str, none_type): Intent declaration protocol date.. [optional]  # noqa: E501
+            intent_declaration_protocol_number (str, none_type): Intent declaration protocol number.. [optional]  # noqa: E501
+            intent_declaration_protocol_date (date, none_type): Intent declaration protocol date.. [optional]  # noqa: E501
             created_at (str, none_type): [optional]  # noqa: E501
             updated_at (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop("_check_type", True)
         _spec_property_naming = kwargs.pop("_spec_property_naming", True)
         _path_to_item = kwargs.pop("_path_to_item", ())
@@ -472,27 +470,27 @@
             email (str, none_type): Client email.. [optional]  # noqa: E501
             certified_email (str, none_type): Client certified email.. [optional]  # noqa: E501
             phone (str, none_type): Client phone.. [optional]  # noqa: E501
             fax (str, none_type): Client fax.. [optional]  # noqa: E501
             notes (str, none_type): Extra notes.. [optional]  # noqa: E501
             default_vat (VatType): [optional]  # noqa: E501
             default_payment_terms (int, none_type): [optional]  # noqa: E501
-            default_payment_terms_type (DefaultPaymentTermsType): [optional]  # noqa: E501
+            default_payment_terms_type (PaymentTermsType): [optional]  # noqa: E501
             default_payment_method (PaymentMethod): [optional]  # noqa: E501
             bank_name (str, none_type): Client bank name.. [optional]  # noqa: E501
             bank_iban (str, none_type): Client iban.. [optional]  # noqa: E501
             bank_swift_code (str, none_type): Client bank swift code.. [optional]  # noqa: E501
             shipping_address (str, none_type): Client shipping address.. [optional]  # noqa: E501
             e_invoice (bool, none_type): Use e-invoices for this entity. [optional]  # noqa: E501
             ei_code (str, none_type): E-invoice code. [optional]  # noqa: E501
             discount_highlight (bool, none_type): Discount Highlight.. [optional]  # noqa: E501
             default_discount (float, none_type): Default discount.. [optional]  # noqa: E501
             has_intent_declaration (bool, none_type): Has intent declaration.. [optional]  # noqa: E501
-            intent_declaration_protocol_number (date, none_type): Intent declaration protocol number.. [optional]  # noqa: E501
-            intent_declaration_protocol_date (str, none_type): Intent declaration protocol date.. [optional]  # noqa: E501
+            intent_declaration_protocol_number (str, none_type): Intent declaration protocol number.. [optional]  # noqa: E501
+            intent_declaration_protocol_date (date, none_type): Intent declaration protocol date.. [optional]  # noqa: E501
             created_at (str, none_type): [optional]  # noqa: E501
             updated_at (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop("_check_type", True)
         _spec_property_naming = kwargs.pop("_spec_property_naming", False)
         _path_to_item = kwargs.pop("_path_to_item", ())
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/client_type.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/client_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/company.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/company.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/company_info.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/company_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/company_info_access_info.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/company_info_access_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/company_info_plan_info.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/company_info_plan_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/company_info_plan_info_functions.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/company_info_plan_info_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/company_info_plan_info_functions_status.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/company_info_plan_info_functions_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/company_info_plan_info_limits.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/company_info_plan_info_limits.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/company_type.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/company_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/controlled_company.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/controlled_company.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_archive_document_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_archive_document_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_archive_document_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_archive_document_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_cashbook_entry_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_cashbook_entry_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_cashbook_entry_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_cashbook_entry_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_client_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_client_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_client_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_client_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_f24_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_f24_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_f24_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_f24_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_issued_document_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_issued_document_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_issued_document_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_issued_document_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_payment_account_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_payment_account_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_payment_account_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_payment_account_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_payment_method_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_payment_method_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_payment_method_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_payment_method_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_product_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_product_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_product_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_product_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_receipt_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_receipt_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_receipt_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_receipt_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_received_document_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_received_document_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_received_document_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_received_document_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_supplier_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_supplier_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_supplier_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_supplier_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_vat_type_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_vat_type_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -32,15 +32,15 @@
 
 def lazy_import():
     from fattureincloud_python_sdk.model.vat_type import VatType
 
     globals()["VatType"] = VatType
 
 
-class CreateVatTypeRequest(ModelNormal):
+class CreateVatTypeResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -111,15 +111,15 @@
     read_only_vars = {}
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CreateVatTypeRequest - a model defined in OpenAPI
+        """CreateVatTypeResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -202,15 +202,15 @@
             "_configuration",
             "_visited_composed_classes",
         ]
     )
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CreateVatTypeRequest - a model defined in OpenAPI
+        """CreateVatTypeResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/create_vat_type_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_vat_type_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -32,15 +32,15 @@
 
 def lazy_import():
     from fattureincloud_python_sdk.model.vat_type import VatType
 
     globals()["VatType"] = VatType
 
 
-class CreateVatTypeResponse(ModelNormal):
+class GetVatTypeResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -111,15 +111,15 @@
     read_only_vars = {}
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CreateVatTypeResponse - a model defined in OpenAPI
+        """GetVatTypeResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -202,15 +202,15 @@
             "_configuration",
             "_visited_composed_classes",
         ]
     )
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CreateVatTypeResponse - a model defined in OpenAPI
+        """GetVatTypeResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/currency.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/currency.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/default_payment_terms_type.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/payment_terms_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -26,15 +26,15 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel,
 )
 from fattureincloud_python_sdk.exceptions import ApiAttributeError
 
 
-class DefaultPaymentTermsType(ModelSimple):
+class PaymentTermsType(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -96,23 +96,23 @@
             "_configuration",
             "_visited_composed_classes",
         ]
     )
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """DefaultPaymentTermsType - a model defined in OpenAPI
+        """PaymentTermsType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Default payment terms.. if omitted defaults to "standard", must be one of ["standard", "end_of_month", ]  # noqa: E501
+            args[0] (str): Payment terms Type.. if omitted defaults to "standard", must be one of ["standard", "end_of_month", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Default payment terms.. if omitted defaults to "standard", must be one of ["standard", "end_of_month", ]  # noqa: E501
+            value (str): Payment terms Type.. if omitted defaults to "standard", must be one of ["standard", "end_of_month", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -188,23 +188,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """DefaultPaymentTermsType - a model defined in OpenAPI
+        """PaymentTermsType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Default payment terms.. if omitted defaults to "standard", must be one of ["standard", "end_of_month", ]  # noqa: E501
+            args[0] (str): Payment terms Type.. if omitted defaults to "standard", must be one of ["standard", "end_of_month", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Default payment terms.. if omitted defaults to "standard", must be one of ["standard", "end_of_month", ]  # noqa: E501
+            value (str): Payment terms Type.. if omitted defaults to "standard", must be one of ["standard", "end_of_month", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/detailed_country.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/detailed_country.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/document_template.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/document_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/e_invoice_rejection_reason.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/e_invoice_rejection_reason.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/email_data.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/email_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/email_data_default_sender_email.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/email_data_default_sender_email.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/email_schedule.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/email_schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/email_schedule_include.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/email_schedule_include.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/entity.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,24 +27,22 @@
     validate_get_composed_info,
     OpenApiModel,
 )
 from fattureincloud_python_sdk.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fattureincloud_python_sdk.model.default_payment_terms_type import (
-        DefaultPaymentTermsType,
-    )
     from fattureincloud_python_sdk.model.entity_type import EntityType
     from fattureincloud_python_sdk.model.payment_method import PaymentMethod
+    from fattureincloud_python_sdk.model.payment_terms_type import PaymentTermsType
     from fattureincloud_python_sdk.model.vat_type import VatType
 
-    globals()["DefaultPaymentTermsType"] = DefaultPaymentTermsType
     globals()["EntityType"] = EntityType
     globals()["PaymentMethod"] = PaymentMethod
+    globals()["PaymentTermsType"] = PaymentTermsType
     globals()["VatType"] = VatType
 
 
 class Entity(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -183,15 +181,15 @@
                 none_type,
             ),  # noqa: E501
             "default_vat": (VatType,),  # noqa: E501
             "default_payment_terms": (
                 int,
                 none_type,
             ),  # noqa: E501
-            "default_payment_terms_type": (DefaultPaymentTermsType,),  # noqa: E501
+            "default_payment_terms_type": (PaymentTermsType,),  # noqa: E501
             "default_payment_method": (PaymentMethod,),  # noqa: E501
             "bank_name": (
                 str,
                 none_type,
             ),  # noqa: E501
             "bank_iban": (
                 str,
@@ -214,19 +212,19 @@
                 none_type,
             ),  # noqa: E501
             "has_intent_declaration": (
                 bool,
                 none_type,
             ),  # noqa: E501
             "intent_declaration_protocol_number": (
-                date,
+                str,
                 none_type,
             ),  # noqa: E501
             "intent_declaration_protocol_date": (
-                str,
+                date,
                 none_type,
             ),  # noqa: E501
             "created_at": (
                 str,
                 none_type,
             ),  # noqa: E501
             "updated_at": (
@@ -335,25 +333,25 @@
             email (str, none_type): Email.. [optional]  # noqa: E501
             certified_email (str, none_type): Certified email.. [optional]  # noqa: E501
             phone (str, none_type): Phone.. [optional]  # noqa: E501
             fax (str, none_type): Fax.. [optional]  # noqa: E501
             notes (str, none_type): Extra notes.. [optional]  # noqa: E501
             default_vat (VatType): [optional]  # noqa: E501
             default_payment_terms (int, none_type): [Only for client] Default payment terms.. [optional]  # noqa: E501
-            default_payment_terms_type (DefaultPaymentTermsType): [optional]  # noqa: E501
+            default_payment_terms_type (PaymentTermsType): [optional]  # noqa: E501
             default_payment_method (PaymentMethod): [optional]  # noqa: E501
             bank_name (str, none_type): [Only for client] Bank name.. [optional]  # noqa: E501
             bank_iban (str, none_type): [Only for client] Iban.. [optional]  # noqa: E501
             bank_swift_code (str, none_type): [Only for client] Bank swift code.. [optional]  # noqa: E501
             shipping_address (str, none_type): [Only for client] Shipping address.. [optional]  # noqa: E501
             e_invoice (bool, none_type): [Only for client] Use e-invoices.. [optional]  # noqa: E501
             ei_code (str, none_type): [Only for client] E-invoices code.. [optional]  # noqa: E501
             has_intent_declaration (bool, none_type): [Only for client] Has intent declaration.. [optional]  # noqa: E501
-            intent_declaration_protocol_number (date, none_type): [Only for client] Intent declaration protocol number.. [optional]  # noqa: E501
-            intent_declaration_protocol_date (str, none_type): [Only for client] Intent declaration protocol date.. [optional]  # noqa: E501
+            intent_declaration_protocol_number (str, none_type): [Only for client] Intent declaration protocol number.. [optional]  # noqa: E501
+            intent_declaration_protocol_date (date, none_type): [Only for client] Intent declaration protocol date.. [optional]  # noqa: E501
             created_at (str, none_type): [optional]  # noqa: E501
             updated_at (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop("_check_type", True)
         _spec_property_naming = kwargs.pop("_spec_property_naming", True)
         _path_to_item = kwargs.pop("_path_to_item", ())
@@ -460,25 +458,25 @@
             email (str, none_type): Email.. [optional]  # noqa: E501
             certified_email (str, none_type): Certified email.. [optional]  # noqa: E501
             phone (str, none_type): Phone.. [optional]  # noqa: E501
             fax (str, none_type): Fax.. [optional]  # noqa: E501
             notes (str, none_type): Extra notes.. [optional]  # noqa: E501
             default_vat (VatType): [optional]  # noqa: E501
             default_payment_terms (int, none_type): [Only for client] Default payment terms.. [optional]  # noqa: E501
-            default_payment_terms_type (DefaultPaymentTermsType): [optional]  # noqa: E501
+            default_payment_terms_type (PaymentTermsType): [optional]  # noqa: E501
             default_payment_method (PaymentMethod): [optional]  # noqa: E501
             bank_name (str, none_type): [Only for client] Bank name.. [optional]  # noqa: E501
             bank_iban (str, none_type): [Only for client] Iban.. [optional]  # noqa: E501
             bank_swift_code (str, none_type): [Only for client] Bank swift code.. [optional]  # noqa: E501
             shipping_address (str, none_type): [Only for client] Shipping address.. [optional]  # noqa: E501
             e_invoice (bool, none_type): [Only for client] Use e-invoices.. [optional]  # noqa: E501
             ei_code (str, none_type): [Only for client] E-invoices code.. [optional]  # noqa: E501
             has_intent_declaration (bool, none_type): [Only for client] Has intent declaration.. [optional]  # noqa: E501
-            intent_declaration_protocol_number (date, none_type): [Only for client] Intent declaration protocol number.. [optional]  # noqa: E501
-            intent_declaration_protocol_date (str, none_type): [Only for client] Intent declaration protocol date.. [optional]  # noqa: E501
+            intent_declaration_protocol_number (str, none_type): [Only for client] Intent declaration protocol number.. [optional]  # noqa: E501
+            intent_declaration_protocol_date (date, none_type): [Only for client] Intent declaration protocol date.. [optional]  # noqa: E501
             created_at (str, none_type): [optional]  # noqa: E501
             updated_at (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop("_check_type", True)
         _spec_property_naming = kwargs.pop("_spec_property_naming", False)
         _path_to_item = kwargs.pop("_path_to_item", ())
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/entity_type.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/entity_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/f24.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/f24.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/f24_status.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/f24_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/function_status.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/function_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_archive_document_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_archive_document_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_cashbook_entry_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_cashbook_entry_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_client_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_client_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_company_info_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_company_info_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_e_invoice_rejection_reason_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_e_invoice_rejection_reason_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_email_data_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_email_data_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_existing_issued_document_totals_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_existing_issued_document_totals_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_existing_issued_document_totals_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_existing_issued_document_totals_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_existing_received_document_totals_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_existing_received_document_totals_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_existing_received_document_totals_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_existing_received_document_totals_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_f24_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_f24_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_issued_document_pre_create_info_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_issued_document_pre_create_info_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_issued_document_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_issued_document_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_new_issued_document_totals_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_new_issued_document_totals_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_new_issued_document_totals_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_new_issued_document_totals_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_new_received_document_totals_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_new_received_document_totals_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_new_received_document_totals_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_new_received_document_totals_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_payment_account_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_payment_account_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_payment_method_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_payment_method_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_product_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_product_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_receipt_pre_create_info_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_receipt_pre_create_info_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_receipt_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_receipt_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_receipts_monthly_totals_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_receipts_monthly_totals_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_received_document_pre_create_info_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_received_document_pre_create_info_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_received_document_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_received_document_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_supplier_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_supplier_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_user_info_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_user_info_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_user_info_response_email_confirmation_state.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_user_info_response_email_confirmation_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_user_info_response_info.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/get_user_info_response_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/get_vat_type_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/create_vat_type_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -32,15 +32,15 @@
 
 def lazy_import():
     from fattureincloud_python_sdk.model.vat_type import VatType
 
     globals()["VatType"] = VatType
 
 
-class GetVatTypeResponse(ModelNormal):
+class CreateVatTypeRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -111,15 +111,15 @@
     read_only_vars = {}
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """GetVatTypeResponse - a model defined in OpenAPI
+        """CreateVatTypeRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -202,15 +202,15 @@
             "_configuration",
             "_visited_composed_classes",
         ]
     )
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """GetVatTypeResponse - a model defined in OpenAPI
+        """CreateVatTypeRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_ei_data.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_ei_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_extra_data.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_extra_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_items_list_item.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_items_list_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_options.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_payments_list_item.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_payments_list_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_payments_list_item_payment_terms.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_payments_list_item_payment_terms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -26,14 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel,
 )
 from fattureincloud_python_sdk.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fattureincloud_python_sdk.model.payment_terms_type import PaymentTermsType
+
+    globals()["PaymentTermsType"] = PaymentTermsType
+
+
 class IssuedDocumentPaymentsListItemPaymentTerms(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
@@ -50,30 +56,25 @@
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
-    allowed_values = {
-        ("type",): {
-            "None": None,
-            "STANDARD": "standard",
-            "END_OF_MONTH": "end_of_month",
-        },
-    }
+    allowed_values = {}
 
     validations = {}
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (
             bool,
             date,
             datetime,
             dict,
             float,
             int,
@@ -90,23 +91,21 @@
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
             "days": (
                 int,
                 none_type,
             ),  # noqa: E501
-            "type": (
-                str,
-                none_type,
-            ),  # noqa: E501
+            "type": (PaymentTermsType,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -151,15 +150,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             days (int, none_type): The number of days by which the payment must be made.. [optional]  # noqa: E501
-            type (str, none_type): Payment terms type.. [optional]  # noqa: E501
+            type (PaymentTermsType): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop("_check_type", True)
         _spec_property_naming = kwargs.pop("_spec_property_naming", True)
         _path_to_item = kwargs.pop("_path_to_item", ())
         _configuration = kwargs.pop("_configuration", None)
         _visited_composed_classes = kwargs.pop("_visited_composed_classes", ())
@@ -243,15 +242,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             days (int, none_type): The number of days by which the payment must be made.. [optional]  # noqa: E501
-            type (str, none_type): Payment terms type.. [optional]  # noqa: E501
+            type (PaymentTermsType): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop("_check_type", True)
         _spec_property_naming = kwargs.pop("_spec_property_naming", False)
         _path_to_item = kwargs.pop("_path_to_item", ())
         _configuration = kwargs.pop("_configuration", None)
         _visited_composed_classes = kwargs.pop("_visited_composed_classes", ())
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_pre_create_info.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_pre_create_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -38,14 +38,15 @@
     )
     from fattureincloud_python_sdk.model.issued_document_pre_create_info_extra_data_default_values import (
         IssuedDocumentPreCreateInfoExtraDataDefaultValues,
     )
     from fattureincloud_python_sdk.model.issued_document_pre_create_info_items_default_values import (
         IssuedDocumentPreCreateInfoItemsDefaultValues,
     )
+    from fattureincloud_python_sdk.model.language import Language
     from fattureincloud_python_sdk.model.numeration import Numeration
     from fattureincloud_python_sdk.model.payment_account import PaymentAccount
     from fattureincloud_python_sdk.model.payment_method import PaymentMethod
     from fattureincloud_python_sdk.model.vat_type import VatType
 
     globals()["Currency"] = Currency
     globals()["DocumentTemplate"] = DocumentTemplate
@@ -54,14 +55,15 @@
     ] = IssuedDocumentPreCreateInfoDefaultValues
     globals()[
         "IssuedDocumentPreCreateInfoExtraDataDefaultValues"
     ] = IssuedDocumentPreCreateInfoExtraDataDefaultValues
     globals()[
         "IssuedDocumentPreCreateInfoItemsDefaultValues"
     ] = IssuedDocumentPreCreateInfoItemsDefaultValues
+    globals()["Language"] = Language
     globals()["Numeration"] = Numeration
     globals()["PaymentAccount"] = PaymentAccount
     globals()["PaymentMethod"] = PaymentMethod
     globals()["VatType"] = VatType
 
 
 class IssuedDocumentPreCreateInfo(ModelNormal):
@@ -162,14 +164,18 @@
                 [PaymentAccount],
                 none_type,
             ),  # noqa: E501
             "vat_types_list": (
                 [VatType],
                 none_type,
             ),  # noqa: E501
+            "languages_list": (
+                [Language],
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -182,14 +188,15 @@
         "currencies_list": "currencies_list",  # noqa: E501
         "templates_list": "templates_list",  # noqa: E501
         "dn_templates_list": "dn_templates_list",  # noqa: E501
         "ai_templates_list": "ai_templates_list",  # noqa: E501
         "payment_methods_list": "payment_methods_list",  # noqa: E501
         "payment_accounts_list": "payment_accounts_list",  # noqa: E501
         "vat_types_list": "vat_types_list",  # noqa: E501
+        "languages_list": "languages_list",  # noqa: E501
     }
 
     read_only_vars = {}
 
     _composed_schemas = {}
 
     @classmethod
@@ -237,14 +244,15 @@
             currencies_list ([Currency], none_type): Currencies list.. [optional]  # noqa: E501
             templates_list ([DocumentTemplate], none_type): Document templates list.. [optional]  # noqa: E501
             dn_templates_list ([DocumentTemplate], none_type): Delivery note templates list.. [optional]  # noqa: E501
             ai_templates_list ([DocumentTemplate], none_type): Accompanying invoice templates list.. [optional]  # noqa: E501
             payment_methods_list ([PaymentMethod], none_type): Payment methods list.. [optional]  # noqa: E501
             payment_accounts_list ([PaymentAccount], none_type): Payment accounts list.. [optional]  # noqa: E501
             vat_types_list ([VatType], none_type): Vat types list.. [optional]  # noqa: E501
+            languages_list ([Language], none_type): Languages list.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop("_check_type", True)
         _spec_property_naming = kwargs.pop("_spec_property_naming", True)
         _path_to_item = kwargs.pop("_path_to_item", ())
         _configuration = kwargs.pop("_configuration", None)
         _visited_composed_classes = kwargs.pop("_visited_composed_classes", ())
@@ -340,14 +348,15 @@
             currencies_list ([Currency], none_type): Currencies list.. [optional]  # noqa: E501
             templates_list ([DocumentTemplate], none_type): Document templates list.. [optional]  # noqa: E501
             dn_templates_list ([DocumentTemplate], none_type): Delivery note templates list.. [optional]  # noqa: E501
             ai_templates_list ([DocumentTemplate], none_type): Accompanying invoice templates list.. [optional]  # noqa: E501
             payment_methods_list ([PaymentMethod], none_type): Payment methods list.. [optional]  # noqa: E501
             payment_accounts_list ([PaymentAccount], none_type): Payment accounts list.. [optional]  # noqa: E501
             vat_types_list ([VatType], none_type): Vat types list.. [optional]  # noqa: E501
+            languages_list ([Language], none_type): Languages list.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop("_check_type", True)
         _spec_property_naming = kwargs.pop("_spec_property_naming", False)
         _path_to_item = kwargs.pop("_path_to_item", ())
         _configuration = kwargs.pop("_configuration", None)
         _visited_composed_classes = kwargs.pop("_visited_composed_classes", ())
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_pre_create_info_default_values.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_pre_create_info_default_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_pre_create_info_extra_data_default_values.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_pre_create_info_extra_data_default_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_pre_create_info_items_default_values.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_pre_create_info_items_default_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_status.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_totals.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_totals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/issued_document_type.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/issued_document_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/language.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/language.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_archive_categories_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_archive_categories_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_archive_documents_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_archive_documents_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_archive_documents_response_page.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_archive_documents_response_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_cashbook_entries_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_cashbook_entries_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_cities_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_cities_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_clients_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_clients_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_clients_response_page.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_clients_response_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_cost_centers_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_cost_centers_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_countries_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_countries_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_currencies_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_currencies_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_delivery_notes_default_causals_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_delivery_notes_default_causals_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_detailed_countries_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_detailed_countries_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_f24_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_f24_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_f24_response_aggregated_data.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_f24_response_aggregated_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_f24_response_aggregation.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_f24_response_aggregation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_f24_response_page.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_f24_response_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_issued_documents_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_issued_documents_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_issued_documents_response_page.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_issued_documents_response_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_languages_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_languages_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_payment_accounts_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_payment_accounts_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_payment_methods_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_payment_methods_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_product_categories_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_product_categories_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_products_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_products_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_products_response_page.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_products_response_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_receipts_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_receipts_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_receipts_response_page.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_receipts_response_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_received_document_categories_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_received_document_categories_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_received_documents_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_received_documents_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_received_documents_response_page.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_received_documents_response_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_revenue_centers_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_revenue_centers_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_suppliers_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_suppliers_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_suppliers_response_page.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_suppliers_response_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_templates_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_templates_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_units_of_measure_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_units_of_measure_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_user_companies_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_user_companies_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_user_companies_response_data.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_user_companies_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/list_vat_types_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/list_vat_types_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_archive_document_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_archive_document_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_archive_document_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_archive_document_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_cashbook_entry_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_cashbook_entry_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_cashbook_entry_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_cashbook_entry_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_client_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_client_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_client_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_client_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_f24_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_f24_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_f24_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_f24_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_issued_document_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_issued_document_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_issued_document_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_issued_document_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_payment_account_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_payment_account_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_payment_account_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_payment_account_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_payment_method_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_payment_method_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_payment_method_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_payment_method_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_product_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_product_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_product_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_product_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_receipt_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_receipt_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_receipt_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_receipt_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_received_document_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_received_document_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_received_document_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_received_document_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_supplier_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_supplier_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_supplier_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_supplier_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_vat_type_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_vat_type_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/modify_vat_type_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/modify_vat_type_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/monthly_total.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/monthly_total.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/numeration.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/numeration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/numeration_item.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/numeration_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/original_document_type.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/original_document_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/pagination.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/payment_account.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/payment_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/payment_account_type.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/payment_account_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/payment_method.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/payment_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/payment_method_details.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/payment_method_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/payment_method_type.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/payment_method_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/permission_level.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/permission_level.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/permissions.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/permissions_fic_issued_documents_detailed.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/permissions_fic_issued_documents_detailed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/product.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/product.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/receipt.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/receipt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/receipt_items_list_item.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/receipt_items_list_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/receipt_pre_create_info.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/receipt_pre_create_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/receipt_type.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/receipt_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/received_document.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/received_document.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -204,14 +204,22 @@
                 str,
                 none_type,
             ),  # noqa: E501
             "attachment_token": (
                 str,
                 none_type,
             ),  # noqa: E501
+            "created_at": (
+                str,
+                none_type,
+            ),  # noqa: E501
+            "updated_at": (
+                str,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -237,14 +245,16 @@
         "tax_deductibility": "tax_deductibility",  # noqa: E501
         "vat_deductibility": "vat_deductibility",  # noqa: E501
         "items_list": "items_list",  # noqa: E501
         "payments_list": "payments_list",  # noqa: E501
         "attachment_url": "attachment_url",  # noqa: E501
         "attachment_preview_url": "attachment_preview_url",  # noqa: E501
         "attachment_token": "attachment_token",  # noqa: E501
+        "created_at": "created_at",  # noqa: E501
+        "updated_at": "updated_at",  # noqa: E501
     }
 
     read_only_vars = {
         "amount_gross",  # noqa: E501
         "next_due_date",  # noqa: E501
         "attachment_url",  # noqa: E501
         "attachment_preview_url",  # noqa: E501
@@ -310,14 +320,16 @@
             tax_deductibility (float, none_type): Tax deducibility percentage.. [optional]  # noqa: E501
             vat_deductibility (float, none_type): Vat deducibility percentage.. [optional]  # noqa: E501
             items_list ([ReceivedDocumentItemsListItem], none_type): [optional]  # noqa: E501
             payments_list ([ReceivedDocumentPaymentsListItem], none_type): [optional]  # noqa: E501
             attachment_url (str, none_type): [Read Only] Attachment url.. [optional]  # noqa: E501
             attachment_preview_url (str, none_type): [Read Only] Attachment preview url.. [optional]  # noqa: E501
             attachment_token (str, none_type): Uploaded attachement token.. [optional]  # noqa: E501
+            created_at (str, none_type): [optional]  # noqa: E501
+            updated_at (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop("_check_type", True)
         _spec_property_naming = kwargs.pop("_spec_property_naming", True)
         _path_to_item = kwargs.pop("_path_to_item", ())
         _configuration = kwargs.pop("_configuration", None)
         _visited_composed_classes = kwargs.pop("_visited_composed_classes", ())
@@ -426,14 +438,16 @@
             tax_deductibility (float, none_type): Tax deducibility percentage.. [optional]  # noqa: E501
             vat_deductibility (float, none_type): Vat deducibility percentage.. [optional]  # noqa: E501
             items_list ([ReceivedDocumentItemsListItem], none_type): [optional]  # noqa: E501
             payments_list ([ReceivedDocumentPaymentsListItem], none_type): [optional]  # noqa: E501
             attachment_url (str, none_type): [Read Only] Attachment url.. [optional]  # noqa: E501
             attachment_preview_url (str, none_type): [Read Only] Attachment preview url.. [optional]  # noqa: E501
             attachment_token (str, none_type): Uploaded attachement token.. [optional]  # noqa: E501
+            created_at (str, none_type): [optional]  # noqa: E501
+            updated_at (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop("_check_type", True)
         _spec_property_naming = kwargs.pop("_spec_property_naming", False)
         _path_to_item = kwargs.pop("_path_to_item", ())
         _configuration = kwargs.pop("_configuration", None)
         _visited_composed_classes = kwargs.pop("_visited_composed_classes", ())
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/received_document_entity.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/received_document_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/received_document_info.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/received_document_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/received_document_info_default_values.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/received_document_info_default_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/received_document_info_items_default_values.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/received_document_info_items_default_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/received_document_items_list_item.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/received_document_items_list_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/received_document_payments_list_item.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/received_document_payments_list_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/received_document_payments_list_item_payment_terms.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/received_document_payments_list_item_payment_terms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/received_document_totals.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/received_document_totals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/received_document_type.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/received_document_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/schedule_email_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/schedule_email_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/send_e_invoice_request.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/send_e_invoice_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/send_e_invoice_request_data.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/send_e_invoice_request_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/send_e_invoice_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/send_e_invoice_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/send_e_invoice_response_data.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/send_e_invoice_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/sender_email.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/sender_email.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/show_totals_mode.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/show_totals_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/supplier.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/supplier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/supplier_type.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/supplier_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/upload_archive_attachment_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/upload_archive_attachment_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/upload_f24_attachment_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/upload_f24_attachment_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/upload_issued_document_attachment_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/upload_issued_document_attachment_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/upload_received_document_attachment_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/upload_received_document_attachment_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/user.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/user_company_role.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/user_company_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/vat_item.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/vat_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/vat_kind.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/vat_kind.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/vat_list.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/vat_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/vat_type.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/vat_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/verify_e_invoice_xml_error_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/verify_e_invoice_xml_error_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/verify_e_invoice_xml_error_response_error.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/verify_e_invoice_xml_error_response_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/verify_e_invoice_xml_error_response_extra.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/verify_e_invoice_xml_error_response_extra.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/verify_e_invoice_xml_response.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/verify_e_invoice_xml_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model/verify_e_invoice_xml_response_data.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model/verify_e_invoice_xml_response_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/model_utils.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
@@ -193,15 +193,15 @@
 
     def __deepcopy__(self, memo):
         cls = self.__class__
 
         if self.get("_spec_property_naming", False):
             new_inst = cls._new_from_openapi_data()
         else:
-            new_inst = cls.__new__(cls)
+            new_inst = cls.__new__(cls, **self.__dict__)
 
         for k, v in self.__dict__.items():
             setattr(new_inst, k, deepcopy(v, memo))
         return new_inst
 
     def __new__(cls, *args, **kwargs):
         # this function uses the discriminator to
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/models/__init__.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,17 +92,14 @@
     CreateSupplierResponse,
 )
 from fattureincloud_python_sdk.model.create_vat_type_request import CreateVatTypeRequest
 from fattureincloud_python_sdk.model.create_vat_type_response import (
     CreateVatTypeResponse,
 )
 from fattureincloud_python_sdk.model.currency import Currency
-from fattureincloud_python_sdk.model.default_payment_terms_type import (
-    DefaultPaymentTermsType,
-)
 from fattureincloud_python_sdk.model.detailed_country import DetailedCountry
 from fattureincloud_python_sdk.model.document_template import DocumentTemplate
 from fattureincloud_python_sdk.model.e_invoice_rejection_reason import (
     EInvoiceRejectionReason,
 )
 from fattureincloud_python_sdk.model.email_data import EmailData
 from fattureincloud_python_sdk.model.email_data_default_sender_email import (
@@ -383,14 +380,15 @@
 from fattureincloud_python_sdk.model.original_document_type import OriginalDocumentType
 from fattureincloud_python_sdk.model.pagination import Pagination
 from fattureincloud_python_sdk.model.payment_account import PaymentAccount
 from fattureincloud_python_sdk.model.payment_account_type import PaymentAccountType
 from fattureincloud_python_sdk.model.payment_method import PaymentMethod
 from fattureincloud_python_sdk.model.payment_method_details import PaymentMethodDetails
 from fattureincloud_python_sdk.model.payment_method_type import PaymentMethodType
+from fattureincloud_python_sdk.model.payment_terms_type import PaymentTermsType
 from fattureincloud_python_sdk.model.permission_level import PermissionLevel
 from fattureincloud_python_sdk.model.permissions import Permissions
 from fattureincloud_python_sdk.model.permissions_fic_issued_documents_detailed import (
     PermissionsFicIssuedDocumentsDetailed,
 )
 from fattureincloud_python_sdk.model.product import Product
 from fattureincloud_python_sdk.model.receipt import Receipt
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/oauth2/oauth2.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/oauth2/oauth2.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/oauth2/scopes.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/oauth2/scopes.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,14 +38,23 @@
 
     # Read permission to the issued Proformas
     ISSUED_DOCUMENTS_PROFORMAS_READ = "issued_documents.proformas:r"
 
     # Read permission to the issued Delivery Notes
     ISSUED_DOCUMENTS_DELIVERY_NOTES_READ = "issued_documents.delivery_notes:r"
 
+    # Read permission to the issued Work Reports
+    ISSUED_DOCUMENTS_WORK_REPORTS_READ = "issued_documents.work_reports:r"
+
+    # Read permission to the issued Supplier Orders
+    ISSUED_DOCUMENTS_SUPPLIER_ORDERS_READ = "issued_documents.supplier_orders:r"
+
+    # Read permission to the issued Self Invoices
+    ISSUED_DOCUMENTS_SELF_INVOICES_READ = "issued_documents.self_invoices:r"
+
     # Write permission to the issued Invoices
     ISSUED_DOCUMENTS_INVOICES_ALL = "issued_documents.invoices:a"
 
     # Write permission to the issued Credit Notes
     ISSUED_DOCUMENTS_CREDIT_NOTES_ALL = "issued_documents.credit_notes:a"
 
     # Write permission to the issued issued Receipts
@@ -59,14 +68,23 @@
 
     # Write permission to the issued Proformas
     ISSUED_DOCUMENTS_PROFORMAS_ALL = "issued_documents.proformas:a"
 
     # Write permission to the issued Delivery Notes
     ISSUED_DOCUMENTS_DELIVERY_NOTES_ALL = "issued_documents.delivery_notes:a"
 
+    # Write permission to the issued Work Reports
+    ISSUED_DOCUMENTS_WORK_REPORTS_ALL = "issued_documents.work_reports:a"
+
+    # Write permission to the issued Supplier Orders
+    ISSUED_DOCUMENTS_SUPPLIER_ORDERS_ALL = "issued_documents.supplier_orders:a"
+
+    # Write permission to the issued Self Invoices
+    ISSUED_DOCUMENTS_SELF_INVOICES_ALL = "issued_documents.self_invoices:a"
+
     # Read permission to the Received Documents
     RECEIVED_DOCUMENTS_READ = "received_documents:r"
 
     # Write permission to the Received Documents
     RECEIVED_DOCUMENTS_ALL = "received_documents:a"
 
     # Read permission to the Stock movements
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk/rest.py` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk.egg-info/PKG-INFO` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fattureincloud-python-sdk
-Version: 2.0.8
+Version: 2.0.9
 Summary: Python SDK for the Fatture in Cloud API
 Home-page: https://github.com/fattureincloud/fattureincloud-python-sdk
 Author: Fatture in Cloud
 Author-email: info@fattureincloud.it
 License: MIT
 Keywords: fattureincloud,fatture in cloud,fatture,fic,fattureincloud sdk,fatture in cloud sdk
 Requires-Python: >=3.6
@@ -17,16 +17,16 @@
 
 Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy. 
 
 The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2.0.19
-- Package version: 2.0.8
+- API version: 2.0.20
+- Package version: 2.0.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.fattureincloud.it](https://www.fattureincloud.it)
 
 ## Requirements.
 
 Python >= 3.6
 
@@ -58,14 +58,24 @@
 from fattureincloud_python_sdk.model.create_archive_document_request import CreateArchiveDocumentRequest
 from fattureincloud_python_sdk.model.create_archive_document_response import CreateArchiveDocumentResponse
 from fattureincloud_python_sdk.model.get_archive_document_response import GetArchiveDocumentResponse
 from fattureincloud_python_sdk.model.list_archive_documents_response import ListArchiveDocumentsResponse
 from fattureincloud_python_sdk.model.modify_archive_document_request import ModifyArchiveDocumentRequest
 from fattureincloud_python_sdk.model.modify_archive_document_response import ModifyArchiveDocumentResponse
 from fattureincloud_python_sdk.model.upload_archive_attachment_response import UploadArchiveAttachmentResponse
+# Defining the host is optional and defaults to https://api-v2.fattureincloud.it
+# See configuration.py for a list of all supported configuration parameters.
+configuration = fattureincloud_python_sdk.Configuration(
+    host = "https://api-v2.fattureincloud.it"
+)
+
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
 
 # Configure OAuth2 access token for authorization: OAuth2AuthenticationCodeFlow
 configuration = fattureincloud_python_sdk.Configuration(
     access_token = "YOUR_ACCESS_TOKEN"
 )
 
 
@@ -238,15 +248,14 @@
  - [CreateReceivedDocumentRequest](docs/CreateReceivedDocumentRequest.md)
  - [CreateReceivedDocumentResponse](docs/CreateReceivedDocumentResponse.md)
  - [CreateSupplierRequest](docs/CreateSupplierRequest.md)
  - [CreateSupplierResponse](docs/CreateSupplierResponse.md)
  - [CreateVatTypeRequest](docs/CreateVatTypeRequest.md)
  - [CreateVatTypeResponse](docs/CreateVatTypeResponse.md)
  - [Currency](docs/Currency.md)
- - [DefaultPaymentTermsType](docs/DefaultPaymentTermsType.md)
  - [DetailedCountry](docs/DetailedCountry.md)
  - [DocumentTemplate](docs/DocumentTemplate.md)
  - [EInvoiceRejectionReason](docs/EInvoiceRejectionReason.md)
  - [EmailData](docs/EmailData.md)
  - [EmailDataDefaultSenderEmail](docs/EmailDataDefaultSenderEmail.md)
  - [EmailSchedule](docs/EmailSchedule.md)
  - [EmailScheduleInclude](docs/EmailScheduleInclude.md)
@@ -367,14 +376,15 @@
  - [OriginalDocumentType](docs/OriginalDocumentType.md)
  - [Pagination](docs/Pagination.md)
  - [PaymentAccount](docs/PaymentAccount.md)
  - [PaymentAccountType](docs/PaymentAccountType.md)
  - [PaymentMethod](docs/PaymentMethod.md)
  - [PaymentMethodDetails](docs/PaymentMethodDetails.md)
  - [PaymentMethodType](docs/PaymentMethodType.md)
+ - [PaymentTermsType](docs/PaymentTermsType.md)
  - [PermissionLevel](docs/PermissionLevel.md)
  - [Permissions](docs/Permissions.md)
  - [PermissionsFicIssuedDocumentsDetailed](docs/PermissionsFicIssuedDocumentsDetailed.md)
  - [Product](docs/Product.md)
  - [Receipt](docs/Receipt.md)
  - [ReceiptItemsListItem](docs/ReceiptItemsListItem.md)
  - [ReceiptPreCreateInfo](docs/ReceiptPreCreateInfo.md)
```

### Comparing `fattureincloud-python-sdk-2.0.8/fattureincloud_python_sdk.egg-info/SOURCES.txt` & `fattureincloud-python-sdk-2.0.9/fattureincloud_python_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,14 @@
 fattureincloud_python_sdk/model/create_received_document_request.py
 fattureincloud_python_sdk/model/create_received_document_response.py
 fattureincloud_python_sdk/model/create_supplier_request.py
 fattureincloud_python_sdk/model/create_supplier_response.py
 fattureincloud_python_sdk/model/create_vat_type_request.py
 fattureincloud_python_sdk/model/create_vat_type_response.py
 fattureincloud_python_sdk/model/currency.py
-fattureincloud_python_sdk/model/default_payment_terms_type.py
 fattureincloud_python_sdk/model/detailed_country.py
 fattureincloud_python_sdk/model/document_template.py
 fattureincloud_python_sdk/model/e_invoice_rejection_reason.py
 fattureincloud_python_sdk/model/email_data.py
 fattureincloud_python_sdk/model/email_data_default_sender_email.py
 fattureincloud_python_sdk/model/email_schedule.py
 fattureincloud_python_sdk/model/email_schedule_include.py
@@ -205,14 +204,15 @@
 fattureincloud_python_sdk/model/original_document_type.py
 fattureincloud_python_sdk/model/pagination.py
 fattureincloud_python_sdk/model/payment_account.py
 fattureincloud_python_sdk/model/payment_account_type.py
 fattureincloud_python_sdk/model/payment_method.py
 fattureincloud_python_sdk/model/payment_method_details.py
 fattureincloud_python_sdk/model/payment_method_type.py
+fattureincloud_python_sdk/model/payment_terms_type.py
 fattureincloud_python_sdk/model/permission_level.py
 fattureincloud_python_sdk/model/permissions.py
 fattureincloud_python_sdk/model/permissions_fic_issued_documents_detailed.py
 fattureincloud_python_sdk/model/product.py
 fattureincloud_python_sdk/model/receipt.py
 fattureincloud_python_sdk/model/receipt_items_list_item.py
 fattureincloud_python_sdk/model/receipt_pre_create_info.py
@@ -300,15 +300,14 @@
 test/test_create_received_document_request.py
 test/test_create_received_document_response.py
 test/test_create_supplier_request.py
 test/test_create_supplier_response.py
 test/test_create_vat_type_request.py
 test/test_create_vat_type_response.py
 test/test_currency.py
-test/test_default_payment_terms_type.py
 test/test_detailed_country.py
 test/test_disjunction.py
 test/test_document_template.py
 test/test_e_invoice_rejection_reason.py
 test/test_email_data.py
 test/test_email_data_default_sender_email.py
 test/test_email_schedule.py
@@ -436,14 +435,15 @@
 test/test_original_document_type.py
 test/test_pagination.py
 test/test_payment_account.py
 test/test_payment_account_type.py
 test/test_payment_method.py
 test/test_payment_method_details.py
 test/test_payment_method_type.py
+test/test_payment_terms_type.py
 test/test_permission_level.py
 test/test_permissions.py
 test/test_permissions_fic_issued_documents_detailed.py
 test/test_product.py
 test/test_products_api.py
 test/test_receipt.py
 test/test_receipt_items_list_item.py
```

### Comparing `fattureincloud-python-sdk-2.0.8/setup.py` & `fattureincloud-python-sdk-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
     Fatture in Cloud API v2 - API Reference
 
     Connect your software with Fatture in Cloud, the invoicing platform chosen by more than 400.000 businesses in Italy.   The Fatture in Cloud API is based on REST, and makes possible to interact with the user related data prior authorization via OAuth2 protocol.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.19
+    The version of the OpenAPI document: 2.0.20
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "fattureincloud-python-sdk"
-VERSION = "2.0.8"
+VERSION = "2.0.9"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_archive_api.py` & `fattureincloud-python-sdk-2.0.9/test/test_archive_api.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_archive_document.py` & `fattureincloud-python-sdk-2.0.9/test/test_archive_document.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_attachment_data.py` & `fattureincloud-python-sdk-2.0.9/test/test_attachment_data.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_cashbook_api.py` & `fattureincloud-python-sdk-2.0.9/test/test_cashbook_api.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_cashbook_entry.py` & `fattureincloud-python-sdk-2.0.9/test/test_cashbook_entry.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_cashbook_entry_document.py` & `fattureincloud-python-sdk-2.0.9/test/test_cashbook_entry_document.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_cashbook_entry_kind.py` & `fattureincloud-python-sdk-2.0.9/test/test_cashbook_entry_kind.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_cashbook_entry_type.py` & `fattureincloud-python-sdk-2.0.9/test/test_cashbook_entry_type.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_city.py` & `fattureincloud-python-sdk-2.0.9/test/test_city.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_client.py` & `fattureincloud-python-sdk-2.0.9/test/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,28 @@
 
 
 import json
 import sys
 import unittest
 
 import fattureincloud_python_sdk
+from fattureincloud_python_sdk.model.payment_terms_type import PaymentTermsType
 from functions import json_serial
 from functions import create_from_json
 from fattureincloud_python_sdk.model.client_type import ClientType
-from fattureincloud_python_sdk.model.default_payment_terms_type import (
-    DefaultPaymentTermsType,
-)
+
 from fattureincloud_python_sdk.model.payment_method import PaymentMethod
 from fattureincloud_python_sdk.model.vat_type import VatType
 from fattureincloud_python_sdk.model.payment_account import PaymentAccount
 from fattureincloud_python_sdk.model.payment_account_type import PaymentAccountType
 from fattureincloud_python_sdk.model.payment_method_details import PaymentMethodDetails
 from fattureincloud_python_sdk.model.payment_method_type import PaymentMethodType
 
 globals()["ClientType"] = ClientType
-globals()["DefaultPaymentTermsType"] = DefaultPaymentTermsType
+globals()["PaymentTermsType"] = PaymentTermsType
 globals()["PaymentMethod"] = PaymentMethod
 globals()["VatType"] = VatType
 from fattureincloud_python_sdk.model.client import Client
 
 
 class TestClient(unittest.TestCase):
     """Client unit test stubs"""
@@ -73,15 +72,15 @@
                 notes="IVA non imponibile ai sensi dell articolo 123, comma 2",
                 e_invoice=True,
                 ei_type="2",
                 ei_description="ei_description_example",
                 is_disabled=True,
             ),
             default_payment_terms=30,
-            default_payment_terms_type=DefaultPaymentTermsType("standard"),
+            default_payment_terms_type=PaymentTermsType("standard"),
             default_payment_method=PaymentMethod(
                 id=1,
                 name="name_example",
                 type=PaymentMethodType("standard"),
                 is_default=True,
                 default_payment_account=PaymentAccount(
                     id=1,
```

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_client_type.py` & `fattureincloud-python-sdk-2.0.9/test/test_client_type.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_clients_api.py` & `fattureincloud-python-sdk-2.0.9/test/test_clients_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,22 @@
     Contact: info@fattureincloud.it
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 import unittest.mock
+from fattureincloud_python_sdk.model.payment_terms_type import PaymentTermsType
 import functions
 import fattureincloud_python_sdk
 from fattureincloud_python_sdk.rest import RESTResponse
 from fattureincloud_python_sdk.api.clients_api import ClientsApi
 from fattureincloud_python_sdk.model.client import Client
 from fattureincloud_python_sdk.model.client_type import ClientType
-from fattureincloud_python_sdk.model.default_payment_terms_type import (
-    DefaultPaymentTermsType,
-)
+
 from fattureincloud_python_sdk.model.payment_account import PaymentAccount
 from fattureincloud_python_sdk.model.payment_account_type import PaymentAccountType
 from fattureincloud_python_sdk.model.payment_method import PaymentMethod
 from fattureincloud_python_sdk.model.payment_method_details import PaymentMethodDetails
 from fattureincloud_python_sdk.model.payment_method_type import PaymentMethodType
 from fattureincloud_python_sdk.model.vat_type import VatType
 from fattureincloud_python_sdk.model.create_client_response import CreateClientResponse
@@ -84,15 +83,15 @@
                     notes="IVA non imponibile ai sensi dell articolo 123, comma 2",
                     e_invoice=True,
                     ei_type="2",
                     ei_description="ei_description_example",
                     is_disabled=True,
                 ),
                 default_payment_terms=30,
-                default_payment_terms_type=DefaultPaymentTermsType("standard"),
+                default_payment_terms_type=PaymentTermsType("standard"),
                 default_payment_method=PaymentMethod(
                     id=1,
                     name="name_example",
                     type=PaymentMethodType("standard"),
                     is_default=True,
                     default_payment_account=PaymentAccount(
                         id=1,
@@ -184,15 +183,15 @@
                     notes="IVA non imponibile ai sensi dell articolo 123, comma 2",
                     e_invoice=True,
                     ei_type="2",
                     ei_description="ei_description_example",
                     is_disabled=True,
                 ),
                 default_payment_terms=30,
-                default_payment_terms_type=DefaultPaymentTermsType("standard"),
+                default_payment_terms_type=PaymentTermsType("standard"),
                 default_payment_method=PaymentMethod(
                     id=1,
                     name="name_example",
                     type=PaymentMethodType("standard"),
                     is_default=True,
                     default_payment_account=PaymentAccount(
                         id=1,
@@ -272,15 +271,15 @@
                         notes="IVA non imponibile ai sensi dell articolo 123, comma 2",
                         e_invoice=True,
                         ei_type="2",
                         ei_description="ei_description_example",
                         is_disabled=True,
                     ),
                     default_payment_terms=30,
-                    default_payment_terms_type=DefaultPaymentTermsType("standard"),
+                    default_payment_terms_type=PaymentTermsType("standard"),
                     default_payment_method=PaymentMethod(
                         id=1,
                         name="name_example",
                         type=PaymentMethodType("standard"),
                         is_default=True,
                         default_payment_account=PaymentAccount(
                             id=1,
@@ -339,15 +338,15 @@
                         notes="IVA non imponibile ai sensi dell articolo 123, comma 2",
                         e_invoice=True,
                         ei_type="2",
                         ei_description="ei_description_example",
                         is_disabled=True,
                     ),
                     default_payment_terms=30,
-                    default_payment_terms_type=DefaultPaymentTermsType("standard"),
+                    default_payment_terms_type=PaymentTermsType("standard"),
                     default_payment_method=PaymentMethod(
                         id=1,
                         name="name_example",
                         type=PaymentMethodType("standard"),
                         is_default=True,
                         default_payment_account=PaymentAccount(
                             id=1,
@@ -427,15 +426,15 @@
                     notes="IVA non imponibile ai sensi dell articolo 123, comma 2",
                     e_invoice=True,
                     ei_type="2",
                     ei_description="ei_description_example",
                     is_disabled=True,
                 ),
                 default_payment_terms=30,
-                default_payment_terms_type=DefaultPaymentTermsType("standard"),
+                default_payment_terms_type=PaymentTermsType("standard"),
                 default_payment_method=PaymentMethod(
                     id=1,
                     name="name_example",
                     type=PaymentMethodType("standard"),
                     is_default=True,
                     default_payment_account=PaymentAccount(
                         id=1,
```

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_companies_api.py` & `fattureincloud-python-sdk-2.0.9/test/test_companies_api.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_company.py` & `fattureincloud-python-sdk-2.0.9/test/test_company.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_company_info.py` & `fattureincloud-python-sdk-2.0.9/test/test_company_info.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_company_info_access_info.py` & `fattureincloud-python-sdk-2.0.9/test/test_company_info_access_info.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_company_info_plan_info.py` & `fattureincloud-python-sdk-2.0.9/test/test_company_info_plan_info.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_company_info_plan_info_functions.py` & `fattureincloud-python-sdk-2.0.9/test/test_company_info_plan_info_functions.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_company_info_plan_info_functions_status.py` & `fattureincloud-python-sdk-2.0.9/test/test_company_info_plan_info_functions_status.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_company_info_plan_info_limits.py` & `fattureincloud-python-sdk-2.0.9/test/test_company_info_plan_info_limits.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_company_type.py` & `fattureincloud-python-sdk-2.0.9/test/test_company_type.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_condition.py` & `fattureincloud-python-sdk-2.0.9/test/test_condition.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_conjunction.py` & `fattureincloud-python-sdk-2.0.9/test/test_conjunction.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_controlled_company.py` & `fattureincloud-python-sdk-2.0.9/test/test_controlled_company.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_archive_document_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_archive_document_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_archive_document_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_archive_document_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_cashbook_entry_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_cashbook_entry_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_cashbook_entry_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_cashbook_entry_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_client_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_client_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 
 
 import json
 import sys
 import unittest
 
 import fattureincloud_python_sdk
+from fattureincloud_python_sdk.model.payment_terms_type import PaymentTermsType
 from functions import json_serial
 from functions import create_from_json
 from fattureincloud_python_sdk.model.client import Client
 from fattureincloud_python_sdk.model.client_type import ClientType
-from fattureincloud_python_sdk.model.default_payment_terms_type import (
-    DefaultPaymentTermsType,
-)
+
 from fattureincloud_python_sdk.model.payment_account import PaymentAccount
 from fattureincloud_python_sdk.model.payment_account_type import PaymentAccountType
 from fattureincloud_python_sdk.model.payment_method import PaymentMethod
 from fattureincloud_python_sdk.model.payment_method_details import PaymentMethodDetails
 from fattureincloud_python_sdk.model.payment_method_type import PaymentMethodType
 from fattureincloud_python_sdk.model.vat_type import VatType
 
@@ -72,15 +71,15 @@
                     notes="IVA non imponibile ai sensi dell articolo 123, comma 2",
                     e_invoice=True,
                     ei_type="2",
                     ei_description="ei_description_example",
                     is_disabled=True,
                 ),
                 default_payment_terms=30,
-                default_payment_terms_type=DefaultPaymentTermsType("standard"),
+                default_payment_terms_type=PaymentTermsType("standard"),
                 default_payment_method=PaymentMethod(
                     id=1,
                     name="name_example",
                     type=PaymentMethodType("standard"),
                     is_default=True,
                     default_payment_account=PaymentAccount(
                         id=1,
```

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_client_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_client_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,21 @@
 
 import json
 import sys
 import unittest
 
 from fattureincloud_python_sdk.model.client import Client
 from fattureincloud_python_sdk.model.client_type import ClientType
-from fattureincloud_python_sdk.model.default_payment_terms_type import (
-    DefaultPaymentTermsType,
-)
+
 from fattureincloud_python_sdk.model.payment_account import PaymentAccount
 from fattureincloud_python_sdk.model.payment_account_type import PaymentAccountType
 from fattureincloud_python_sdk.model.payment_method import PaymentMethod
 from fattureincloud_python_sdk.model.payment_method_details import PaymentMethodDetails
 from fattureincloud_python_sdk.model.payment_method_type import PaymentMethodType
+from fattureincloud_python_sdk.model.payment_terms_type import PaymentTermsType
 from fattureincloud_python_sdk.model.vat_type import VatType
 from fattureincloud_python_sdk.model.client import Client
 
 globals()["Client"] = Client
 from functions import json_serial
 from fattureincloud_python_sdk.model.create_client_response import CreateClientResponse
 
@@ -71,15 +70,15 @@
                     notes="IVA non imponibile ai sensi dell articolo 123, comma 2",
                     e_invoice=True,
                     ei_type="2",
                     ei_description="ei_description_example",
                     is_disabled=True,
                 ),
                 default_payment_terms=30,
-                default_payment_terms_type=DefaultPaymentTermsType("standard"),
+                default_payment_terms_type=PaymentTermsType("standard"),
                 default_payment_method=PaymentMethod(
                     id=1,
                     name="name_example",
                     type=PaymentMethodType("standard"),
                     is_default=True,
                     default_payment_account=PaymentAccount(
                         id=1,
```

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_f24_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_f24_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_f24_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_f24_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_issued_document_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_issued_document_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_issued_document_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_issued_document_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_payment_account_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_payment_account_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_payment_account_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_payment_account_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_payment_method_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_payment_method_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_payment_method_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_product_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_product_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_product_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_product_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_receipt_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_receipt_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_receipt_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_receipt_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_received_document_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_received_document_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_received_document_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_received_document_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_supplier_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_supplier_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_supplier_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_supplier_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_vat_type_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_vat_type_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_create_vat_type_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_create_vat_type_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_currency.py` & `fattureincloud-python-sdk-2.0.9/test/test_currency.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_default_payment_terms_type.py` & `fattureincloud-python-sdk-2.0.9/test/test_payment_terms_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,31 +12,31 @@
 import json
 import sys
 import unittest
 
 import fattureincloud_python_sdk
 from functions import json_serial
 from functions import create_from_json
-from fattureincloud_python_sdk.model.default_payment_terms_type import (
-    DefaultPaymentTermsType,
+from fattureincloud_python_sdk.model.payment_terms_type import (
+    PaymentTermsType,
 )
 
 
-class TestDefaultPaymentTermsType(unittest.TestCase):
-    """DefaultPaymentTermsType unit test stubs"""
+class TestPaymentTermsType(unittest.TestCase):
+    """PaymentTermsType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDefaultPaymentTermsType(self):
-        """Test DefaultPaymentTermsType"""
-        model = DefaultPaymentTermsType("standard")
+    def testPaymentTermsType(self):
+        """Test PaymentTermsType"""
+        model = PaymentTermsType("standard")
         expected_json = "standard"
         actual_json = model.value
         assert actual_json == expected_json
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_detailed_country.py` & `fattureincloud-python-sdk-2.0.9/test/test_detailed_country.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_disjunction.py` & `fattureincloud-python-sdk-2.0.9/test/test_disjunction.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_document_template.py` & `fattureincloud-python-sdk-2.0.9/test/test_document_template.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_e_invoice_rejection_reason.py` & `fattureincloud-python-sdk-2.0.9/test/test_e_invoice_rejection_reason.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_email_data.py` & `fattureincloud-python-sdk-2.0.9/test/test_email_data.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_email_data_default_sender_email.py` & `fattureincloud-python-sdk-2.0.9/test/test_email_data_default_sender_email.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_email_schedule.py` & `fattureincloud-python-sdk-2.0.9/test/test_email_schedule.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_email_schedule_include.py` & `fattureincloud-python-sdk-2.0.9/test/test_email_schedule_include.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_entity.py` & `fattureincloud-python-sdk-2.0.9/test/test_entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,33 +10,32 @@
 
 
 import json
 import sys
 import unittest
 
 import fattureincloud_python_sdk
+from fattureincloud_python_sdk.model.payment_terms_type import PaymentTermsType
 from functions import json_serial
 from functions import create_from_json
 from fattureincloud_python_sdk.model.client import Client
-from fattureincloud_python_sdk.model.default_payment_terms_type import (
-    DefaultPaymentTermsType,
-)
+
 from fattureincloud_python_sdk.model.entity_type import EntityType
 from fattureincloud_python_sdk.model.payment_account import PaymentAccount
 from fattureincloud_python_sdk.model.payment_account_type import PaymentAccountType
 from fattureincloud_python_sdk.model.payment_method import PaymentMethod
 from fattureincloud_python_sdk.model.payment_method_details import PaymentMethodDetails
 from fattureincloud_python_sdk.model.payment_method_type import PaymentMethodType
 from fattureincloud_python_sdk.model.supplier import Supplier
 from fattureincloud_python_sdk.model.supplier_type import SupplierType
 from fattureincloud_python_sdk.model.vat_type import VatType
 from fattureincloud_python_sdk.model.entity import Entity
 
 globals()["Client"] = Client
-globals()["DefaultPaymentTermsType"] = DefaultPaymentTermsType
+globals()["PaymentTermsType"] = PaymentTermsType
 globals()["PaymentMethod"] = PaymentMethod
 globals()["Supplier"] = Supplier
 globals()["SupplierType"] = SupplierType
 globals()["VatType"] = VatType
 
 
 class TestEntity(unittest.TestCase):
@@ -78,15 +77,15 @@
                 notes="IVA non imponibile ai sensi dell articolo 123, comma 2",
                 e_invoice=True,
                 ei_type="2",
                 ei_description="ei_description_example",
                 is_disabled=True,
             ),
             default_payment_terms=30,
-            default_payment_terms_type=DefaultPaymentTermsType("standard"),
+            default_payment_terms_type=PaymentTermsType("standard"),
             default_payment_method=PaymentMethod(
                 id=1,
                 name="name_example",
                 type=PaymentMethodType("standard"),
                 is_default=True,
                 default_payment_account=PaymentAccount(
                     id=1,
```

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_entity_type.py` & `fattureincloud-python-sdk-2.0.9/test/test_entity_type.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_f24.py` & `fattureincloud-python-sdk-2.0.9/test/test_f24.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_f24_status.py` & `fattureincloud-python-sdk-2.0.9/test/test_f24_status.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_filter.py` & `fattureincloud-python-sdk-2.0.9/test/test_filter.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_function_status.py` & `fattureincloud-python-sdk-2.0.9/test/test_function_status.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_archive_document_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_archive_document_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_cashbook_entry_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_cashbook_entry_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_client_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_client_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 
 
 import json
 import sys
 import unittest
 
 import fattureincloud_python_sdk
+from fattureincloud_python_sdk.model.payment_terms_type import PaymentTermsType
 from functions import json_serial
 from functions import create_from_json
 from fattureincloud_python_sdk.model.client import Client
 from fattureincloud_python_sdk.model.client_type import ClientType
-from fattureincloud_python_sdk.model.default_payment_terms_type import (
-    DefaultPaymentTermsType,
-)
+
 from fattureincloud_python_sdk.model.payment_account import PaymentAccount
 from fattureincloud_python_sdk.model.payment_account_type import PaymentAccountType
 from fattureincloud_python_sdk.model.payment_method import PaymentMethod
 from fattureincloud_python_sdk.model.payment_method_details import PaymentMethodDetails
 from fattureincloud_python_sdk.model.payment_method_type import PaymentMethodType
 from fattureincloud_python_sdk.model.vat_type import VatType
 
@@ -72,15 +71,15 @@
                     notes="IVA non imponibile ai sensi dell articolo 123, comma 2",
                     e_invoice=True,
                     ei_type="2",
                     ei_description="ei_description_example",
                     is_disabled=True,
                 ),
                 default_payment_terms=30,
-                default_payment_terms_type=DefaultPaymentTermsType("standard"),
+                default_payment_terms_type=PaymentTermsType("standard"),
                 default_payment_method=PaymentMethod(
                     id=1,
                     name="name_example",
                     type=PaymentMethodType("standard"),
                     is_default=True,
                     default_payment_account=PaymentAccount(
                         id=1,
```

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_company_info_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_company_info_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_e_invoice_rejection_reason_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_e_invoice_rejection_reason_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_email_data_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_email_data_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_existing_issued_document_totals_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_existing_issued_document_totals_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_existing_issued_document_totals_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_existing_issued_document_totals_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_existing_received_document_totals_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_existing_received_document_totals_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_existing_received_document_totals_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_existing_received_document_totals_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_f24_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_f24_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_issued_document_pre_create_info_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_issued_document_pre_create_info_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_issued_document_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_issued_document_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_new_issued_document_totals_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_new_issued_document_totals_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_new_issued_document_totals_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_new_issued_document_totals_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_new_received_document_totals_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_new_received_document_totals_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_new_received_document_totals_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_new_received_document_totals_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_payment_account_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_payment_account_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_payment_method_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_product_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_product_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_receipt_pre_create_info_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_receipt_pre_create_info_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_receipt_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_receipt_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_receipts_monthly_totals_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_receipts_monthly_totals_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_received_document_pre_create_info_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_received_document_pre_create_info_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_received_document_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_received_document_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_supplier_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_supplier_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_user_info_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_user_info_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_user_info_response_email_confirmation_state.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_user_info_response_email_confirmation_state.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_user_info_response_info.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_user_info_response_info.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_get_vat_type_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_get_vat_type_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_info_api.py` & `fattureincloud-python-sdk-2.0.9/test/test_info_api.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_issued_document.py` & `fattureincloud-python-sdk-2.0.9/test/test_issued_document.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_issued_document_ei_data.py` & `fattureincloud-python-sdk-2.0.9/test/test_issued_document_ei_data.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_issued_document_extra_data.py` & `fattureincloud-python-sdk-2.0.9/test/test_issued_document_extra_data.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_issued_document_items_list_item.py` & `fattureincloud-python-sdk-2.0.9/test/test_issued_document_items_list_item.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_issued_document_options.py` & `fattureincloud-python-sdk-2.0.9/test/test_issued_document_options.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_issued_document_payments_list_item.py` & `fattureincloud-python-sdk-2.0.9/test/test_issued_document_payments_list_item.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_issued_document_payments_list_item_payment_terms.py` & `fattureincloud-python-sdk-2.0.9/test/test_issued_document_payments_list_item_payment_terms.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 
 import sys
 import unittest
 
 import fattureincloud_python_sdk
 import json
+from fattureincloud_python_sdk.model.payment_terms_type import PaymentTermsType
 from functions import json_serial
 from fattureincloud_python_sdk.model.issued_document_payments_list_item_payment_terms import (
     IssuedDocumentPaymentsListItemPaymentTerms,
 )
 
 
 class TestIssuedDocumentPaymentsListItemPaymentTerms(unittest.TestCase):
@@ -27,15 +28,15 @@
         pass
 
     def tearDown(self):
         pass
 
     def testIssuedDocumentPaymentsListItemPaymentTerms(self):
         """Test IssuedDocumentPaymentsListItemPaymentTerms"""
-        model = IssuedDocumentPaymentsListItemPaymentTerms(days=2, type="standard")
+        model = IssuedDocumentPaymentsListItemPaymentTerms(days=2, type=PaymentTermsType("standard"))
         expected_json = '{"days": 2, "type": "standard"}'
         actual_json = json.dumps(model.to_dict(), default=json_serial)
         assert actual_json == expected_json
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_issued_document_pre_create_info.py` & `fattureincloud-python-sdk-2.0.9/test/test_issued_document_pre_create_info.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_issued_document_pre_create_info_default_values.py` & `fattureincloud-python-sdk-2.0.9/test/test_issued_document_pre_create_info_default_values.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_issued_document_pre_create_info_extra_data_default_values.py` & `fattureincloud-python-sdk-2.0.9/test/test_issued_document_pre_create_info_extra_data_default_values.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_issued_document_pre_create_info_items_default_values.py` & `fattureincloud-python-sdk-2.0.9/test/test_issued_document_pre_create_info_items_default_values.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_issued_document_status.py` & `fattureincloud-python-sdk-2.0.9/test/test_issued_document_status.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_issued_document_totals.py` & `fattureincloud-python-sdk-2.0.9/test/test_issued_document_totals.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_issued_document_type.py` & `fattureincloud-python-sdk-2.0.9/test/test_issued_document_type.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_issued_documents_api.py` & `fattureincloud-python-sdk-2.0.9/test/test_issued_documents_api.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_issued_e_invoices_api.py` & `fattureincloud-python-sdk-2.0.9/test/test_issued_e_invoices_api.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_language.py` & `fattureincloud-python-sdk-2.0.9/test/test_language.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_archive_categories_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_archive_categories_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_archive_documents_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_archive_documents_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_archive_documents_response_page.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_archive_documents_response_page.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_cashbook_entries_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_cashbook_entries_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_cities_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_cities_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_clients_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_clients_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 from functions import create_from_json
 from fattureincloud_python_sdk.model.client import Client
 from fattureincloud_python_sdk.model.list_clients_response_page import (
     ListClientsResponsePage,
 )
 from fattureincloud_python_sdk.model.pagination import Pagination
 from fattureincloud_python_sdk.model.client_type import ClientType
-from fattureincloud_python_sdk.model.default_payment_terms_type import (
-    DefaultPaymentTermsType,
-)
+from fattureincloud_python_sdk.model.payment_terms_type import PaymentTermsType
 from fattureincloud_python_sdk.model.payment_account import PaymentAccount
 from fattureincloud_python_sdk.model.payment_account_type import PaymentAccountType
 from fattureincloud_python_sdk.model.payment_method import PaymentMethod
 from fattureincloud_python_sdk.model.payment_method_details import PaymentMethodDetails
 from fattureincloud_python_sdk.model.payment_method_type import PaymentMethodType
 from fattureincloud_python_sdk.model.vat_type import VatType
 
@@ -79,15 +77,15 @@
                         notes="IVA non imponibile ai sensi dell articolo 123, comma 2",
                         e_invoice=True,
                         ei_type="2",
                         ei_description="ei_description_example",
                         is_disabled=True,
                     ),
                     default_payment_terms=30,
-                    default_payment_terms_type=DefaultPaymentTermsType("standard"),
+                    default_payment_terms_type=PaymentTermsType("standard"),
                     default_payment_method=PaymentMethod(
                         id=1,
                         name="name_example",
                         type=PaymentMethodType("standard"),
                         is_default=True,
                         default_payment_account=PaymentAccount(
                             id=1,
```

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_clients_response_page.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_clients_response_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,15 @@
 
 globals()["Client"] = Client
 from fattureincloud_python_sdk.model.list_clients_response_page import (
     ListClientsResponsePage,
 )
 from fattureincloud_python_sdk.model.pagination import Pagination
 from fattureincloud_python_sdk.model.client_type import ClientType
-from fattureincloud_python_sdk.model.default_payment_terms_type import (
-    DefaultPaymentTermsType,
-)
+from fattureincloud_python_sdk.model.payment_terms_type import PaymentTermsType
 from fattureincloud_python_sdk.model.payment_account import PaymentAccount
 from fattureincloud_python_sdk.model.payment_account_type import PaymentAccountType
 from fattureincloud_python_sdk.model.payment_method import PaymentMethod
 from fattureincloud_python_sdk.model.payment_method_details import PaymentMethodDetails
 from fattureincloud_python_sdk.model.payment_method_type import PaymentMethodType
 from fattureincloud_python_sdk.model.vat_type import VatType
 
@@ -76,15 +74,15 @@
                         notes="IVA non imponibile ai sensi dell articolo 123, comma 2",
                         e_invoice=True,
                         ei_type="2",
                         ei_description="ei_description_example",
                         is_disabled=True,
                     ),
                     default_payment_terms=30,
-                    default_payment_terms_type=DefaultPaymentTermsType("standard"),
+                    default_payment_terms_type=PaymentTermsType("standard"),
                     default_payment_method=PaymentMethod(
                         id=1,
                         name="name_example",
                         type=PaymentMethodType("standard"),
                         is_default=True,
                         default_payment_account=PaymentAccount(
                             id=1,
```

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_cost_centers_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_cost_centers_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_countries_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_countries_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_currencies_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_currencies_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_delivery_notes_default_causals_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_delivery_notes_default_causals_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_detailed_countries_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_detailed_countries_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_f24_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_f24_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_f24_response_aggregated_data.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_f24_response_aggregated_data.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_f24_response_aggregation.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_f24_response_aggregation.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_f24_response_page.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_f24_response_page.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_issued_documents_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_issued_documents_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_issued_documents_response_page.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_issued_documents_response_page.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_languages_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_languages_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_payment_accounts_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_payment_accounts_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_payment_methods_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_payment_methods_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_product_categories_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_product_categories_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_products_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_products_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_products_response_page.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_products_response_page.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_receipts_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_receipts_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_receipts_response_page.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_receipts_response_page.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_received_document_categories_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_received_document_categories_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_received_documents_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_received_documents_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_received_documents_response_page.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_received_documents_response_page.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_revenue_centers_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_revenue_centers_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_suppliers_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_suppliers_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_suppliers_response_page.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_suppliers_response_page.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_templates_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_templates_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_units_of_measure_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_units_of_measure_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_user_companies_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_user_companies_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_user_companies_response_data.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_user_companies_response_data.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_list_vat_types_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_list_vat_types_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_archive_document_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_archive_document_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_archive_document_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_archive_document_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_cashbook_entry_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_cashbook_entry_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_cashbook_entry_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_cashbook_entry_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_client_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_client_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 import unittest
 
 import fattureincloud_python_sdk
 from functions import json_serial
 from functions import create_from_json
 from fattureincloud_python_sdk.model.client import Client
 from fattureincloud_python_sdk.model.client_type import ClientType
-from fattureincloud_python_sdk.model.default_payment_terms_type import (
-    DefaultPaymentTermsType,
-)
+from fattureincloud_python_sdk.model.payment_terms_type import PaymentTermsType
 from fattureincloud_python_sdk.model.payment_account import PaymentAccount
 from fattureincloud_python_sdk.model.payment_account_type import PaymentAccountType
 from fattureincloud_python_sdk.model.payment_method import PaymentMethod
 from fattureincloud_python_sdk.model.payment_method_details import PaymentMethodDetails
 from fattureincloud_python_sdk.model.payment_method_type import PaymentMethodType
 from fattureincloud_python_sdk.model.vat_type import VatType
 
@@ -72,15 +70,15 @@
                     notes="IVA non imponibile ai sensi dell articolo 123, comma 2",
                     e_invoice=True,
                     ei_type="2",
                     ei_description="ei_description_example",
                     is_disabled=True,
                 ),
                 default_payment_terms=30,
-                default_payment_terms_type=DefaultPaymentTermsType("standard"),
+                default_payment_terms_type=PaymentTermsType("standard"),
                 default_payment_method=PaymentMethod(
                     id=1,
                     name="name_example",
                     type=PaymentMethodType("standard"),
                     is_default=True,
                     default_payment_account=PaymentAccount(
                         id=1,
```

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_client_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_client_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 import unittest
 
 import fattureincloud_python_sdk
 from functions import json_serial
 from functions import create_from_json
 from fattureincloud_python_sdk.model.client import Client
 from fattureincloud_python_sdk.model.client_type import ClientType
-from fattureincloud_python_sdk.model.default_payment_terms_type import (
-    DefaultPaymentTermsType,
-)
+from fattureincloud_python_sdk.model.payment_terms_type import PaymentTermsType
 from fattureincloud_python_sdk.model.payment_account import PaymentAccount
 from fattureincloud_python_sdk.model.payment_account_type import PaymentAccountType
 from fattureincloud_python_sdk.model.payment_method import PaymentMethod
 from fattureincloud_python_sdk.model.payment_method_details import PaymentMethodDetails
 from fattureincloud_python_sdk.model.payment_method_type import PaymentMethodType
 from fattureincloud_python_sdk.model.vat_type import VatType
 
@@ -72,15 +70,15 @@
                     notes="IVA non imponibile ai sensi dell articolo 123, comma 2",
                     e_invoice=True,
                     ei_type="2",
                     ei_description="ei_description_example",
                     is_disabled=True,
                 ),
                 default_payment_terms=30,
-                default_payment_terms_type=DefaultPaymentTermsType("standard"),
+                default_payment_terms_type=PaymentTermsType("standard"),
                 default_payment_method=PaymentMethod(
                     id=1,
                     name="name_example",
                     type=PaymentMethodType("standard"),
                     is_default=True,
                     default_payment_account=PaymentAccount(
                         id=1,
```

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_f24_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_f24_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_f24_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_f24_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_issued_document_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_issued_document_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_issued_document_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_issued_document_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_payment_account_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_payment_account_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_payment_account_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_payment_account_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_payment_method_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_payment_method_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_payment_method_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_product_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_product_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_product_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_product_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_receipt_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_receipt_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_receipt_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_receipt_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_received_document_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_received_document_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_received_document_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_received_document_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_supplier_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_supplier_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_supplier_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_supplier_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_vat_type_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_vat_type_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_modify_vat_type_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_modify_vat_type_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_monthly_total.py` & `fattureincloud-python-sdk-2.0.9/test/test_monthly_total.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_numeration.py` & `fattureincloud-python-sdk-2.0.9/test/test_numeration.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_numeration_item.py` & `fattureincloud-python-sdk-2.0.9/test/test_numeration_item.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_oauth2.py` & `fattureincloud-python-sdk-2.0.9/test/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_operator.py` & `fattureincloud-python-sdk-2.0.9/test/test_operator.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_original_document_type.py` & `fattureincloud-python-sdk-2.0.9/test/test_original_document_type.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_pagination.py` & `fattureincloud-python-sdk-2.0.9/test/test_pagination.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_payment_account.py` & `fattureincloud-python-sdk-2.0.9/test/test_payment_account.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_payment_account_type.py` & `fattureincloud-python-sdk-2.0.9/test/test_payment_account_type.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_payment_method.py` & `fattureincloud-python-sdk-2.0.9/test/test_payment_method.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_payment_method_details.py` & `fattureincloud-python-sdk-2.0.9/test/test_payment_method_details.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_payment_method_type.py` & `fattureincloud-python-sdk-2.0.9/test/test_payment_method_type.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_permission_level.py` & `fattureincloud-python-sdk-2.0.9/test/test_permission_level.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_permissions.py` & `fattureincloud-python-sdk-2.0.9/test/test_permissions.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_permissions_fic_issued_documents_detailed.py` & `fattureincloud-python-sdk-2.0.9/test/test_permissions_fic_issued_documents_detailed.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_product.py` & `fattureincloud-python-sdk-2.0.9/test/test_product.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_products_api.py` & `fattureincloud-python-sdk-2.0.9/test/test_products_api.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_receipt.py` & `fattureincloud-python-sdk-2.0.9/test/test_receipt.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_receipt_items_list_item.py` & `fattureincloud-python-sdk-2.0.9/test/test_receipt_items_list_item.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_receipt_pre_create_info.py` & `fattureincloud-python-sdk-2.0.9/test/test_receipt_pre_create_info.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_receipt_type.py` & `fattureincloud-python-sdk-2.0.9/test/test_receipt_type.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_receipts_api.py` & `fattureincloud-python-sdk-2.0.9/test/test_receipts_api.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_received_document.py` & `fattureincloud-python-sdk-2.0.9/test/test_received_document.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_received_document_entity.py` & `fattureincloud-python-sdk-2.0.9/test/test_received_document_entity.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_received_document_info.py` & `fattureincloud-python-sdk-2.0.9/test/test_received_document_info.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_received_document_info_default_values.py` & `fattureincloud-python-sdk-2.0.9/test/test_received_document_info_default_values.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_received_document_info_items_default_values.py` & `fattureincloud-python-sdk-2.0.9/test/test_received_document_info_items_default_values.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_received_document_items_list_item.py` & `fattureincloud-python-sdk-2.0.9/test/test_received_document_items_list_item.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_received_document_payments_list_item.py` & `fattureincloud-python-sdk-2.0.9/test/test_received_document_payments_list_item.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_received_document_payments_list_item_payment_terms.py` & `fattureincloud-python-sdk-2.0.9/test/test_received_document_payments_list_item_payment_terms.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_received_document_totals.py` & `fattureincloud-python-sdk-2.0.9/test/test_received_document_totals.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_received_document_type.py` & `fattureincloud-python-sdk-2.0.9/test/test_received_document_type.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_received_documents_api.py` & `fattureincloud-python-sdk-2.0.9/test/test_received_documents_api.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_schedule_email_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_schedule_email_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_send_e_invoice_request.py` & `fattureincloud-python-sdk-2.0.9/test/test_send_e_invoice_request.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_send_e_invoice_request_data.py` & `fattureincloud-python-sdk-2.0.9/test/test_send_e_invoice_request_data.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_send_e_invoice_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_send_e_invoice_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_send_e_invoice_response_data.py` & `fattureincloud-python-sdk-2.0.9/test/test_send_e_invoice_response_data.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_sender_email.py` & `fattureincloud-python-sdk-2.0.9/test/test_sender_email.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_settings_api.py` & `fattureincloud-python-sdk-2.0.9/test/test_settings_api.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_show_totals_mode.py` & `fattureincloud-python-sdk-2.0.9/test/test_show_totals_mode.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_supplier.py` & `fattureincloud-python-sdk-2.0.9/test/test_supplier.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_supplier_type.py` & `fattureincloud-python-sdk-2.0.9/test/test_supplier_type.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_suppliers_api.py` & `fattureincloud-python-sdk-2.0.9/test/test_suppliers_api.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_taxes_api.py` & `fattureincloud-python-sdk-2.0.9/test/test_taxes_api.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_upload_archive_attachment_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_upload_archive_attachment_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_upload_f24_attachment_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_upload_f24_attachment_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_upload_issued_document_attachment_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_upload_issued_document_attachment_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_upload_received_document_attachment_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_upload_received_document_attachment_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_user.py` & `fattureincloud-python-sdk-2.0.9/test/test_user.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_user_api.py` & `fattureincloud-python-sdk-2.0.9/test/test_user_api.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_user_company_role.py` & `fattureincloud-python-sdk-2.0.9/test/test_user_company_role.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_vat_item.py` & `fattureincloud-python-sdk-2.0.9/test/test_vat_item.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_vat_kind.py` & `fattureincloud-python-sdk-2.0.9/test/test_vat_kind.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_vat_list.py` & `fattureincloud-python-sdk-2.0.9/test/test_vat_list.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_vat_type.py` & `fattureincloud-python-sdk-2.0.9/test/test_vat_type.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_verify_e_invoice_xml_error_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_verify_e_invoice_xml_error_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_verify_e_invoice_xml_error_response_error.py` & `fattureincloud-python-sdk-2.0.9/test/test_verify_e_invoice_xml_error_response_error.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_verify_e_invoice_xml_error_response_extra.py` & `fattureincloud-python-sdk-2.0.9/test/test_verify_e_invoice_xml_error_response_extra.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_verify_e_invoice_xml_response.py` & `fattureincloud-python-sdk-2.0.9/test/test_verify_e_invoice_xml_response.py`

 * *Files identical despite different names*

### Comparing `fattureincloud-python-sdk-2.0.8/test/test_verify_e_invoice_xml_response_data.py` & `fattureincloud-python-sdk-2.0.9/test/test_verify_e_invoice_xml_response_data.py`

 * *Files identical despite different names*

