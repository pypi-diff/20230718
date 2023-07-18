# Comparing `tmp/django-vendor-0.4.5.tar.gz` & `tmp/django-vendor-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vendor-0.4.5.tar", last modified: Wed Jul 12 17:35:33 2023, max compression
+gzip compressed data, was "django-vendor-0.4.6.tar", last modified: Tue Jul 18 20:29:24 2023, max compression
```

## Comparing `django-vendor-0.4.5.tar` & `django-vendor-0.4.6.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.556460 django-vendor-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-12 17:35:33.556460 django-vendor-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-12 17:34:11.000000 django-vendor-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-12 17:34:11.000000 django-vendor-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:35:33.556460 django-vendor-0.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.532460 django-vendor-0.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.536460 django-vendor-0.4.5/src/django_vendor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-12 17:35:33.000000 django-vendor-0.4.5/src/django_vendor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-12 17:35:33.000000 django-vendor-0.4.5/src/django_vendor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:35:33.000000 django-vendor-0.4.5/src/django_vendor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-12 17:35:33.000000 django-vendor-0.4.5/src/django_vendor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 17:35:33.000000 django-vendor-0.4.5/src/django_vendor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.536460 django-vendor-0.4.5/src/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.536460 django-vendor-0.4.5/src/vendor/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.536460 django-vendor-0.4.5/src/vendor/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/api/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.536460 django-vendor-0.4.5/src/vendor/api/v1/authorizenet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/api/v1/authorizenet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14742 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/api/v1/authorizenet/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.536460 django-vendor-0.4.5/src/vendor/api/v1/stripe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/api/v1/stripe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/api/v1/stripe/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.536460 django-vendor-0.4.5/src/vendor/encrypt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/encrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/encrypt/cleartext.py
--rw-r--r--   0 runner    (1001) docker     (123)    18433 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.544460 django-vendor-0.4.5/src/vendor/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0002_auto_20200912_0142.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0003_auto_20200915_1839.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0004_offer_offer_description.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0005_auto_20200930_2037.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0006_auto_20201005_2257.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0007_offer_list_bundle_items.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0008_offer_allow_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0009_auto_20201111_0743.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0010_auto_20201112_0138.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0011_auto_20201120_1750.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0012_auto_20201123_1848.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0013_auto_20201202_1759.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0014_term_types_update_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0015_uuid_payments_receipts.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0016_auto_20201203_2011.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0017_auto_20201203_2107.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0018_add_uuid_address_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0019_fill_uuid_address_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0020_lock_uuid_address_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0021_auto_20210408_2303.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0022_offer_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0023_profile_null_false.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0024_offer_deleted.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0025_auto_20210914_0025.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0026_auto_20210914_1209.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0027_bugfix_vendor_notes_invoice_history.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0028_add_trial_date_term_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0029_alter_customerprofile_currency_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0030_auto_20220414_1055.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0031_pre_invoice_status_change.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0032_alter_invoice_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0033_payment_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0034_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0035_add_subscription_relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0036_post_payment_status_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0037_auto_20220609_1644.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0038_auto_20220719_0944.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0039_customerprofile_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0040_auto_20221020_1617.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0041_offer_billing_start_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0042_offer_is_promotional.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0043_invoice_global_discount.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/0044_site_settings_stripe_processor_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.544460 django-vendor-0.4.5/src/vendor/models/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/models/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/models/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)    17557 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/models/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/models/modelmanagers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/models/offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/models/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/models/price.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/models/product.py
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/models/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/models/receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/models/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/models/tax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/models/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/models/wishlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.544460 django-vendor-0.4.5/src/vendor/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62438 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/processors/authorizenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/processors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/processors/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)    53235 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/processors/stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.548460 django-vendor-0.4.5/src/vendor/signals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/signals/stripe_signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.532460 django-vendor-0.4.5/src/vendor/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.548460 django-vendor-0.4.5/src/vendor/templates/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/address_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/checkout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.548460 django-vendor-0.4.5/src/vendor/templates/vendor/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/dummy/payment_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.548460 django-vendor-0.4.5/src/vendor/templates/vendor/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/includes/account_info_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/includes/billing_address_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/includes/cost_overview.html
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/includes/edit_link.html
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/includes/payment_form.html
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/integration_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/invoice_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/invoice_history_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/invoice_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.552460 django-vendor-0.4.5/src/vendor/templates/vendor/manage/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/manage/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/manage/config.html
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/manage/config_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/manage/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/manage/invoice_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/manage/invoice_list.html
--rw-r--r--   0 runner    (1001) docker     (123)    20128 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/manage/offer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/manage/offers.html
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/manage/payment_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/manage/processor_site_config.html
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/manage/processor_site_config_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/manage/product.html
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/manage/products.html
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/manage/profile_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/manage/profile_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/manage/receipt_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/manage/receipt_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/manage/subscription_add_payment.html
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/manage/subscription_create.html
--rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/manage/subscription_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/orderitem_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/orderitem_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/orderitem_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/ordersummary.html
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/payment.html
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/payment_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/payment_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/payment_summary.html
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/purchase_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/purchase_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/refund_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templates/vendor/refund_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.552460 django-vendor-0.4.5/src/vendor/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/templatetags/admin_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.552460 django-vendor-0.4.5/src/vendor/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    30579 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49307 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/tests/test_authorizenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    42637 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/tests/test_stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.552460 django-vendor-0.4.5/src/vendor/urls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/urls/vendor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/urls/vendor_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:33.552460 django-vendor-0.4.5/src/vendor/views/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/views/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/views/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/views/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/views/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/views/vendor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18072 2023-07-12 17:34:11.000000 django-vendor-0.4.5/src/vendor/views/vendor_admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.240274 django-vendor-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-18 20:29:24.240274 django-vendor-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-18 20:28:06.000000 django-vendor-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-18 20:28:06.000000 django-vendor-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 20:29:24.240274 django-vendor-0.4.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.216274 django-vendor-0.4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.220274 django-vendor-0.4.6/src/django_vendor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-18 20:29:24.000000 django-vendor-0.4.6/src/django_vendor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-18 20:29:24.000000 django-vendor-0.4.6/src/django_vendor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 20:29:24.000000 django-vendor-0.4.6/src/django_vendor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-18 20:29:24.000000 django-vendor-0.4.6/src/django_vendor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 20:29:24.000000 django-vendor-0.4.6/src/django_vendor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.220274 django-vendor-0.4.6/src/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.220274 django-vendor-0.4.6/src/vendor/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.220274 django-vendor-0.4.6/src/vendor/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/api/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.220274 django-vendor-0.4.6/src/vendor/api/v1/authorizenet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/api/v1/authorizenet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14742 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/api/v1/authorizenet/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.220274 django-vendor-0.4.6/src/vendor/api/v1/stripe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/api/v1/stripe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/api/v1/stripe/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.220274 django-vendor-0.4.6/src/vendor/encrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/encrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/encrypt/cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18433 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.228274 django-vendor-0.4.6/src/vendor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0002_auto_20200912_0142.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0003_auto_20200915_1839.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0004_offer_offer_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0005_auto_20200930_2037.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0006_auto_20201005_2257.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0007_offer_list_bundle_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0008_offer_allow_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0009_auto_20201111_0743.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0010_auto_20201112_0138.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0011_auto_20201120_1750.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0012_auto_20201123_1848.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0013_auto_20201202_1759.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0014_term_types_update_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0015_uuid_payments_receipts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0016_auto_20201203_2011.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0017_auto_20201203_2107.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0018_add_uuid_address_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0019_fill_uuid_address_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0020_lock_uuid_address_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0021_auto_20210408_2303.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0022_offer_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0023_profile_null_false.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0024_offer_deleted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0025_auto_20210914_0025.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0026_auto_20210914_1209.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0027_bugfix_vendor_notes_invoice_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0028_add_trial_date_term_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0029_alter_customerprofile_currency_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0030_auto_20220414_1055.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0031_pre_invoice_status_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0032_alter_invoice_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0033_payment_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0034_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0035_add_subscription_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0036_post_payment_status_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0037_auto_20220609_1644.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0038_auto_20220719_0944.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0039_customerprofile_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0040_auto_20221020_1617.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0041_offer_billing_start_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0042_offer_is_promotional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0043_invoice_global_discount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/0044_site_settings_stripe_processor_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.228274 django-vendor-0.4.6/src/vendor/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/models/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/models/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17557 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/models/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/models/modelmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/models/offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/models/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/models/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/models/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/models/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/models/receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/models/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/models/tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/models/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/models/wishlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.232274 django-vendor-0.4.6/src/vendor/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62443 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/processors/authorizenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/processors/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53235 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/processors/stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.232274 django-vendor-0.4.6/src/vendor/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/signals/stripe_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.216274 django-vendor-0.4.6/src/vendor/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.232274 django-vendor-0.4.6/src/vendor/templates/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/address_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/checkout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.232274 django-vendor-0.4.6/src/vendor/templates/vendor/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/dummy/payment_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.236274 django-vendor-0.4.6/src/vendor/templates/vendor/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/includes/account_info_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/includes/billing_address_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/includes/cost_overview.html
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/includes/edit_link.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/includes/payment_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/integration_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/invoice_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/invoice_history_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/invoice_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.236274 django-vendor-0.4.6/src/vendor/templates/vendor/manage/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/manage/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/manage/config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/manage/config_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/manage/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/manage/invoice_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/manage/invoice_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20128 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/manage/offer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/manage/offers.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/manage/payment_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/manage/processor_site_config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/manage/processor_site_config_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/manage/product.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/manage/products.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/manage/profile_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/manage/profile_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/manage/receipt_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/manage/receipt_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/manage/subscription_add_payment.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/manage/subscription_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/manage/subscription_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/orderitem_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/orderitem_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/orderitem_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/ordersummary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/payment.html
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/payment_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/payment_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/payment_summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/purchase_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/purchase_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/refund_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templates/vendor/refund_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.236274 django-vendor-0.4.6/src/vendor/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/templatetags/admin_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.240274 django-vendor-0.4.6/src/vendor/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    30579 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49307 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/tests/test_authorizenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42637 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/tests/test_stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.240274 django-vendor-0.4.6/src/vendor/urls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/urls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/urls/vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/urls/vendor_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:29:24.240274 django-vendor-0.4.6/src/vendor/views/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/views/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/views/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/views/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/views/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/views/vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18072 2023-07-18 20:28:06.000000 django-vendor-0.4.6/src/vendor/views/vendor_admin.py
```

### Comparing `django-vendor-0.4.5/PKG-INFO` & `django-vendor-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vendor
-Version: 0.4.5
+Version: 0.4.6
 Summary: Django App Toolkit for selling digital and physical goods online.
 Author: Roberto Himmelbauer
 Author-email: Grant Viklund <renderbox@gmail.com>
 Project-URL: Homepage, https://github.com/renderbox/django-vendor
 Project-URL: Bug Tracker, https://github.com/renderbox/django-vendor/issues
 Keywords: django,app
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django-vendor-0.4.5/README.md` & `django-vendor-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/pyproject.toml` & `django-vendor-0.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 [project]
 name = "django-vendor"
-version = "0.4.5"
+version = "0.4.6"
 
 authors = [
   { name="Grant Viklund", email="renderbox@gmail.com" },
   { name="Roberto Himmelbauer" }
 ]
 description = "Django App Toolkit for selling digital and physical goods online."
 readme = "README.md"
```

### Comparing `django-vendor-0.4.5/src/django_vendor.egg-info/PKG-INFO` & `django-vendor-0.4.6/src/django_vendor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vendor
-Version: 0.4.5
+Version: 0.4.6
 Summary: Django App Toolkit for selling digital and physical goods online.
 Author: Roberto Himmelbauer
 Author-email: Grant Viklund <renderbox@gmail.com>
 Project-URL: Homepage, https://github.com/renderbox/django-vendor
 Project-URL: Bug Tracker, https://github.com/renderbox/django-vendor/issues
 Keywords: django,app
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django-vendor-0.4.5/src/django_vendor.egg-info/SOURCES.txt` & `django-vendor-0.4.6/src/django_vendor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/admin.py` & `django-vendor-0.4.6/src/vendor/admin.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/api/v1/authorizenet/views.py` & `django-vendor-0.4.6/src/vendor/api/v1/authorizenet/views.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/api/v1/stripe/views.py` & `django-vendor-0.4.6/src/vendor/api/v1/stripe/views.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/api/v1/urls.py` & `django-vendor-0.4.6/src/vendor/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/api/v1/views.py` & `django-vendor-0.4.6/src/vendor/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/apps.py` & `django-vendor-0.4.6/src/vendor/apps.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/config.py` & `django-vendor-0.4.6/src/vendor/config.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/forms.py` & `django-vendor-0.4.6/src/vendor/forms.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/integrations.py` & `django-vendor-0.4.6/src/vendor/integrations.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0001_initial.py` & `django-vendor-0.4.6/src/vendor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0003_auto_20200915_1839.py` & `django-vendor-0.4.6/src/vendor/migrations/0003_auto_20200915_1839.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0005_auto_20200930_2037.py` & `django-vendor-0.4.6/src/vendor/migrations/0005_auto_20200930_2037.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0006_auto_20201005_2257.py` & `django-vendor-0.4.6/src/vendor/migrations/0006_auto_20201005_2257.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0008_offer_allow_multiple.py` & `django-vendor-0.4.6/src/vendor/migrations/0008_offer_allow_multiple.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0009_auto_20201111_0743.py` & `django-vendor-0.4.6/src/vendor/migrations/0009_auto_20201111_0743.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0010_auto_20201112_0138.py` & `django-vendor-0.4.6/src/vendor/migrations/0010_auto_20201112_0138.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0011_auto_20201120_1750.py` & `django-vendor-0.4.6/src/vendor/migrations/0011_auto_20201120_1750.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0012_auto_20201123_1848.py` & `django-vendor-0.4.6/src/vendor/migrations/0012_auto_20201123_1848.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0013_auto_20201202_1759.py` & `django-vendor-0.4.6/src/vendor/migrations/0013_auto_20201202_1759.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0014_term_types_update_value.py` & `django-vendor-0.4.6/src/vendor/migrations/0014_term_types_update_value.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0015_uuid_payments_receipts.py` & `django-vendor-0.4.6/src/vendor/migrations/0015_uuid_payments_receipts.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0016_auto_20201203_2011.py` & `django-vendor-0.4.6/src/vendor/migrations/0016_auto_20201203_2011.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0017_auto_20201203_2107.py` & `django-vendor-0.4.6/src/vendor/migrations/0017_auto_20201203_2107.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0018_add_uuid_address_profile.py` & `django-vendor-0.4.6/src/vendor/migrations/0018_add_uuid_address_profile.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0019_fill_uuid_address_profile.py` & `django-vendor-0.4.6/src/vendor/migrations/0019_fill_uuid_address_profile.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0020_lock_uuid_address_profile.py` & `django-vendor-0.4.6/src/vendor/migrations/0020_lock_uuid_address_profile.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0021_auto_20210408_2303.py` & `django-vendor-0.4.6/src/vendor/migrations/0021_auto_20210408_2303.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0023_profile_null_false.py` & `django-vendor-0.4.6/src/vendor/migrations/0023_profile_null_false.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0025_auto_20210914_0025.py` & `django-vendor-0.4.6/src/vendor/migrations/0025_auto_20210914_0025.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0026_auto_20210914_1209.py` & `django-vendor-0.4.6/src/vendor/migrations/0026_auto_20210914_1209.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0027_bugfix_vendor_notes_invoice_history.py` & `django-vendor-0.4.6/src/vendor/migrations/0027_bugfix_vendor_notes_invoice_history.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0028_add_trial_date_term_details.py` & `django-vendor-0.4.6/src/vendor/migrations/0028_add_trial_date_term_details.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0029_alter_customerprofile_currency_and_more.py` & `django-vendor-0.4.6/src/vendor/migrations/0029_alter_customerprofile_currency_and_more.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0030_auto_20220414_1055.py` & `django-vendor-0.4.6/src/vendor/migrations/0030_auto_20220414_1055.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0031_pre_invoice_status_change.py` & `django-vendor-0.4.6/src/vendor/migrations/0031_pre_invoice_status_change.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0033_payment_status.py` & `django-vendor-0.4.6/src/vendor/migrations/0033_payment_status.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0034_subscription.py` & `django-vendor-0.4.6/src/vendor/migrations/0034_subscription.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0035_add_subscription_relation.py` & `django-vendor-0.4.6/src/vendor/migrations/0035_add_subscription_relation.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0036_post_payment_status_change.py` & `django-vendor-0.4.6/src/vendor/migrations/0036_post_payment_status_change.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0037_auto_20220609_1644.py` & `django-vendor-0.4.6/src/vendor/migrations/0037_auto_20220609_1644.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0038_auto_20220719_0944.py` & `django-vendor-0.4.6/src/vendor/migrations/0038_auto_20220719_0944.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0040_auto_20221020_1617.py` & `django-vendor-0.4.6/src/vendor/migrations/0040_auto_20221020_1617.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0042_offer_is_promotional.py` & `django-vendor-0.4.6/src/vendor/migrations/0042_offer_is_promotional.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/migrations/0044_site_settings_stripe_processor_rename.py` & `django-vendor-0.4.6/src/vendor/migrations/0044_site_settings_stripe_processor_rename.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/models/__init__.py` & `django-vendor-0.4.6/src/vendor/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/models/address.py` & `django-vendor-0.4.6/src/vendor/models/address.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/models/base.py` & `django-vendor-0.4.6/src/vendor/models/base.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/models/choice.py` & `django-vendor-0.4.6/src/vendor/models/choice.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/models/invoice.py` & `django-vendor-0.4.6/src/vendor/models/invoice.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/models/modelmanagers.py` & `django-vendor-0.4.6/src/vendor/models/modelmanagers.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/models/offer.py` & `django-vendor-0.4.6/src/vendor/models/offer.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/models/payment.py` & `django-vendor-0.4.6/src/vendor/models/payment.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/models/price.py` & `django-vendor-0.4.6/src/vendor/models/price.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/models/profile.py` & `django-vendor-0.4.6/src/vendor/models/profile.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/models/receipt.py` & `django-vendor-0.4.6/src/vendor/models/receipt.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/models/subscription.py` & `django-vendor-0.4.6/src/vendor/models/subscription.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/models/tax.py` & `django-vendor-0.4.6/src/vendor/models/tax.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/models/utils.py` & `django-vendor-0.4.6/src/vendor/models/utils.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/models/validator.py` & `django-vendor-0.4.6/src/vendor/models/validator.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/models/wishlist.py` & `django-vendor-0.4.6/src/vendor/models/wishlist.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/processors/__init__.py` & `django-vendor-0.4.6/src/vendor/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/processors/authorizenet.py` & `django-vendor-0.4.6/src/vendor/processors/authorizenet.py`

 * *Files 0% similar despite different names*

```diff
@@ -595,15 +595,15 @@
     def subscription_payment(self, subscription):
         """
         subscription: Type: OrderItem
         Creates a subscription for a user. Subscriptions can be monthy or yearly.objects.all()
         """
         # Setting subscription details
         self.transaction_type = apicontractsv1.ARBSubscriptionType()
-        self.transaction_type.name = subscription.offer.name
+        self.transaction_type.name = subscription.offer.name[:25]
         self.transaction_type.paymentSchedule = self.create_payment_scheduale_interval_type(subscription, subscription.offer.terms)
         self.transaction_type.amount = self.to_valid_decimal(subscription.total - subscription.discounts)
         self.transaction_type.trialAmount = self.to_valid_decimal(subscription.offer.get_trial_amount())
         self.transaction_type.billTo = self.create_billing_address(apicontractsv1.nameAndAddressType())
         self.transaction_type.payment = self.create_authorize_payment()
         self.transaction_type.customer = self.create_customer_data_recurring()
```

### Comparing `django-vendor-0.4.5/src/vendor/processors/base.py` & `django-vendor-0.4.6/src/vendor/processors/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     def create_receipt_by_term_type(self, order_item, term_type):
         today = timezone.now()
         self.receipt = Receipt()
         self.receipt.profile = self.invoice.profile
         self.receipt.order_item = order_item
         self.receipt.transaction = self.payment.transaction
         self.receipt.meta.update(self.payment.result)
-        self.receipt.meta['payment_amount'] = self.payment.amount
+        self.receipt.meta['payment_amount'] = str(self.to_valid_decimal(self.payment.amount))
 
         if today > (self.payment.submitted_date - timedelta(hours=1)) or today < (self.payment.submitted_date + timedelta(hours=1)):
             start_date = order_item.offer.get_offer_start_date(self.payment.submitted_date)
         else:
             start_date = order_item.offer.get_offer_start_date(today)
 
 
@@ -469,15 +469,15 @@
         Process/subscribies recurring payments throught the payement gateway and creates a payment model for each subscription.
         If a payment is completed it will create a receipt for the subscription
         """
         if not self.is_card_valid():
             return None
 
         for subscription in self.invoice.get_recurring_order_items():
-            self.create_payment_model()
+            self.create_payment_model(amount=self.to_valid_decimal(subscription.total - subscription.discounts))
             self.subscription_payment(subscription)
             self.save_payment_transaction_result()
             self.update_invoice_status(InvoiceStatus.COMPLETE)
             
             if self.is_transaction_and_invoice_complete():
                 self.create_subscription_model()
                 self.invoice.save_discounts_vendor_notes()
```

### Comparing `django-vendor-0.4.5/src/vendor/processors/stripe.py` & `django-vendor-0.4.6/src/vendor/processors/stripe.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/signals/stripe_signals.py` & `django-vendor-0.4.6/src/vendor/signals/stripe_signals.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/checkout.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/checkout.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/includes/account_info_form.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/includes/account_info_form.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/includes/billing_address_form.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/includes/billing_address_form.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/includes/cost_overview.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/includes/cost_overview.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/includes/payment_form.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/includes/payment_form.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/integration_form.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/integration_form.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/invoice_detail.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/invoice_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/invoice_history_detail.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/invoice_history_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/invoice_list.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/invoice_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/manage/config_list.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/manage/config_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/manage/dashboard.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/manage/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/manage/invoice_detail.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/manage/invoice_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/manage/invoice_list.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/manage/invoice_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/manage/offer.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/manage/offer.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/manage/offers.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/manage/offers.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/manage/payment_list.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/manage/payment_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/manage/processor_site_config_list.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/manage/processor_site_config_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/manage/product.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/manage/product.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/manage/products.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/manage/products.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/manage/profile_detail.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/manage/profile_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/manage/profile_list.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/manage/profile_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/manage/receipt_detail.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/manage/receipt_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/manage/receipt_list.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/manage/receipt_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/manage/subscription_add_payment.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/manage/subscription_add_payment.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/manage/subscription_create.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/manage/subscription_create.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/manage/subscription_detail.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/manage/subscription_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/orderitem_list.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/orderitem_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/ordersummary.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/ordersummary.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/payment_summary.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/payment_summary.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/purchase_detail.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/purchase_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/purchase_list.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/purchase_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templates/vendor/refund_list.html` & `django-vendor-0.4.6/src/vendor/templates/vendor/refund_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/templatetags/admin_tags.py` & `django-vendor-0.4.6/src/vendor/templatetags/admin_tags.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/tests/__init__.py` & `django-vendor-0.4.6/src/vendor/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/tests/test_authorizenet.py` & `django-vendor-0.4.6/src/vendor/tests/test_authorizenet.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/tests/test_processor.py` & `django-vendor-0.4.6/src/vendor/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/tests/test_stripe.py` & `django-vendor-0.4.6/src/vendor/tests/test_stripe.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/urls/vendor.py` & `django-vendor-0.4.6/src/vendor/urls/vendor.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/urls/vendor_admin.py` & `django-vendor-0.4.6/src/vendor/urls/vendor_admin.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/utils.py` & `django-vendor-0.4.6/src/vendor/utils.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/views/__init__.py` & `django-vendor-0.4.6/src/vendor/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/views/config.py` & `django-vendor-0.4.6/src/vendor/views/config.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/views/integration.py` & `django-vendor-0.4.6/src/vendor/views/integration.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/views/mixin.py` & `django-vendor-0.4.6/src/vendor/views/mixin.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/views/report.py` & `django-vendor-0.4.6/src/vendor/views/report.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/views/vendor.py` & `django-vendor-0.4.6/src/vendor/views/vendor.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.5/src/vendor/views/vendor_admin.py` & `django-vendor-0.4.6/src/vendor/views/vendor_admin.py`

 * *Files identical despite different names*

