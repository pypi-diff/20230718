# Comparing `tmp/djangoldp_account-2.3.8.tar.gz` & `tmp/djangoldp_account-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_account-2.3.8.tar", last modified: Fri Feb 25 15:38:02 2022, max compression
+gzip compressed data, was "dist/djangoldp_account-2.3.9.tar", last modified: Tue Apr 12 06:24:14 2022, max compression
```

## Comparing `djangoldp_account-2.3.8.tar` & `djangoldp_account-2.3.9.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account.egg-info/
--rw-r--r--   0 root         (0) root         (0)      303 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     4971 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      155 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)     7838 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      720 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      303 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/
--rw-rw-rw-   0 root         (0) root         (0)     9300 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/tests/
--rw-rw-rw-   0 root         (0) root         (0)     7440 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/tests/tests_auth_backends.py
--rw-rw-rw-   0 root         (0) root         (0)      713 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/tests/models.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2201 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/tests/tests_update.py
--rw-rw-rw-   0 root         (0) root         (0)      738 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/tests/runner.py
--rw-rw-rw-   0 root         (0) root         (0)     9586 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/endpoints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/endpoints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9594 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/endpoints/rp_login.py
--rw-rw-rw-   0 root         (0) root         (0)     1296 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/endpoints/webfinger.py
--rw-rw-rw-   0 root         (0) root         (0)     1122 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)       70 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/registration/activation_email_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)      374 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)      213 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/registration/password_change_form.html
--rw-rw-rw-   0 root         (0) root         (0)      215 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/registration/password_reset_email.html
--rw-rw-rw-   0 root         (0) root         (0)      329 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      134 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/registration/activation_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      929 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)      212 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/registration/registration_form.html
--rw-rw-rw-   0 root         (0) root         (0)      209 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      235 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/registration/activation_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      808 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/registration/lost_user.html
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/registration/password_reset_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)      135 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/registration/activate.html
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/registration/password_reset_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      145 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/registration/registration_closed.html
--rw-rw-rw-   0 root         (0) root         (0)      112 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/registration/logout.html
--rw-rw-rw-   0 root         (0) root         (0)     2969 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/registration/login.html
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/registration/password_change_done.html
--rw-rw-rw-   0 root         (0) root         (0)      170 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/registration/registration_complete.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/templates/oidc_provider/
--rw-rw-rw-   0 root         (0) root         (0)     1375 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/oidc_provider/authorize.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/templates/password/
--rw-rw-rw-   0 root         (0) root         (0)      614 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/password/email.html
--rw-rw-rw-   0 root         (0) root         (0)      877 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/templates/django_registration/
--rw-rw-rw-   0 root         (0) root         (0)      119 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/django_registration/activation_email_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)       42 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/django_registration/registration_base.html
--rw-rw-rw-   0 root         (0) root         (0)      580 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/django_registration/activation_email_body.txt
--rw-rw-rw-   0 root         (0) root         (0)      580 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/django_registration/activation_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      576 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/django_registration/registration_form.html
--rw-rw-rw-   0 root         (0) root         (0)      264 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/django_registration/registration_closed.html
--rw-rw-rw-   0 root         (0) root         (0)      385 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/django_registration/registration_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      364 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/templates/django_registration/activation_failed.html
--rw-rw-rw-   0 root         (0) root         (0)     1346 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     2265 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)     1142 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      584 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/management/commands/mock_account.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1837 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/management/commands/create_distant_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     2919 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/management/commands/import_csv.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/management/commands/fill_user_fields.py
--rw-rw-rw-   0 root         (0) root         (0)       49 2022-02-25 15:38:00.000000 djangoldp_account-2.3.8/djangoldp_account/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      865 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/factories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10465 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/locale/de/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      380 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/locale/de/LC_MESSAGES/django.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    14085 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/locale/es/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     8589 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/locale/es/LC_MESSAGES/django.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    13987 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/locale/fr/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     8349 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/locale/fr/LC_MESSAGES/django.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/locale/en/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    13553 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/locale/en/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     8055 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/locale/en/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)      551 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/forms.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/static/
--rw-rw-rw-   0 root         (0) root         (0)     2675 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/static/base.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/static/registration/
--rw-rw-rw-   0 root         (0) root         (0)      624 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/static/registration/login.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/static/oidc_provider/
--rw-rw-rw-   0 root         (0) root         (0)      270 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/static/oidc_provider/authorize.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/static/django_registration/
--rw-rw-rw-   0 root         (0) root         (0)      246 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/static/django_registration/registration_form.css
--rw-rw-rw-   0 root         (0) root         (0)      493 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/auth/
--rw-rw-rw-   0 root         (0) root         (0)     6749 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/auth/backends.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1614 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/auth/middleware.py
--rw-rw-rw-   0 root         (0) root         (0)     3114 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/auth/solid.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/djangoldp_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-25 15:38:02.000000 djangoldp_account-2.3.8/djangoldp_account/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1052 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/migrations/0002_auto_20190917_1141.py
--rw-rw-rw-   0 root         (0) root         (0)      614 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/migrations/0012_auto_20200501_1433.py
--rw-rw-rw-   0 root         (0) root         (0)      655 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/migrations/0007_auto_20200130_1242.py
--rw-rw-rw-   0 root         (0) root         (0)     4931 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1239 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/migrations/0010_auto_20200501_1207.py
--rw-rw-rw-   0 root         (0) root         (0)     1286 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/migrations/0014_auto_20200610_1323.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/migrations/0016_auto_20200903_1049.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      602 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/migrations/0011_auto_20200501_1420.py
--rw-rw-rw-   0 root         (0) root         (0)     1275 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/migrations/0009_auto_20200429_1346.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/migrations/0003_auto_20191024_0854.py
--rw-rw-rw-   0 root         (0) root         (0)      648 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/migrations/0006_auto_20200121_1321.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/migrations/0013_auto_20200505_1733.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/migrations/0005_ldpuser_default_redirect_uri.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/migrations/0017_auto_20200910_1606.py
--rw-rw-rw-   0 root         (0) root         (0)      656 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/migrations/0008_auto_20200130_1251.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/migrations/0015_auto_20200617_1817.py
--rw-rw-rw-   0 root         (0) root         (0)      407 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/migrations/0018_auto_20210223_2254.py
--rw-rw-rw-   0 root         (0) root         (0)      606 2022-02-25 15:37:48.000000 djangoldp_account-2.3.8/djangoldp_account/migrations/0004_auto_20191203_0921.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      303 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     4971 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      155 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)     8430 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       61 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      720 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      303 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/
+-rw-rw-rw-   0 root         (0) root         (0)     9300 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     7440 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/tests/tests_auth_backends.py
+-rw-rw-rw-   0 root         (0) root         (0)      713 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/tests/models.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2201 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/tests/tests_update.py
+-rw-rw-rw-   0 root         (0) root         (0)      738 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/tests/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     9586 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/endpoints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/endpoints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9594 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/endpoints/rp_login.py
+-rw-rw-rw-   0 root         (0) root         (0)     1296 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/endpoints/webfinger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1122 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/activation_email_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      374 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      213 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/password_change_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      215 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/password_reset_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      329 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      134 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/activation_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      929 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      212 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/registration_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      209 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      235 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/activation_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      808 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/lost_user.html
+-rw-rw-rw-   0 root         (0) root         (0)      139 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/password_reset_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      135 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/activate.html
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/password_reset_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      145 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/registration_closed.html
+-rw-rw-rw-   0 root         (0) root         (0)      112 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/logout.html
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/login.html
+-rw-rw-rw-   0 root         (0) root         (0)      121 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/password_change_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      170 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/registration/registration_complete.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/templates/oidc_provider/
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/oidc_provider/authorize.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/templates/password/
+-rw-rw-rw-   0 root         (0) root         (0)      614 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/password/email.html
+-rw-rw-rw-   0 root         (0) root         (0)      877 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/activation_email_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)       42 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/registration_base.html
+-rw-rw-rw-   0 root         (0) root         (0)      580 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/activation_email_body.txt
+-rw-rw-rw-   0 root         (0) root         (0)      580 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/activation_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      576 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/registration_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      264 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/registration_closed.html
+-rw-rw-rw-   0 root         (0) root         (0)      385 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/registration_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      364 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/activation_failed.html
+-rw-rw-rw-   0 root         (0) root         (0)     1346 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2446 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     1142 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      584 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/management/commands/mock_account.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1837 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/management/commands/create_distant_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2919 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/management/commands/import_csv.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/management/commands/fill_user_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)       49 2022-04-12 06:24:13.000000 djangoldp_account-2.3.9/djangoldp_account/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      865 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10465 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/locale/de/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      380 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/locale/de/LC_MESSAGES/django.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    14085 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/locale/es/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     8589 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/locale/es/LC_MESSAGES/django.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    13987 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/locale/fr/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     8349 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/locale/fr/LC_MESSAGES/django.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    13553 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/locale/en/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     8055 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/locale/en/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)      551 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/static/
+-rw-rw-rw-   0 root         (0) root         (0)     2675 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/static/base.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/static/registration/
+-rw-rw-rw-   0 root         (0) root         (0)      624 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/static/registration/login.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/static/oidc_provider/
+-rw-rw-rw-   0 root         (0) root         (0)      270 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/static/oidc_provider/authorize.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/static/django_registration/
+-rw-rw-rw-   0 root         (0) root         (0)      246 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/static/django_registration/registration_form.css
+-rw-rw-rw-   0 root         (0) root         (0)      493 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/auth/
+-rw-rw-rw-   0 root         (0) root         (0)     6749 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/auth/backends.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1614 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/auth/middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)     3114 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/auth/solid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/djangoldp_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 06:24:14.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0002_auto_20190917_1141.py
+-rw-rw-rw-   0 root         (0) root         (0)      614 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0012_auto_20200501_1433.py
+-rw-rw-rw-   0 root         (0) root         (0)      655 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0007_auto_20200130_1242.py
+-rw-rw-rw-   0 root         (0) root         (0)     4931 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0010_auto_20200501_1207.py
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0014_auto_20200610_1323.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0016_auto_20200903_1049.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      602 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0011_auto_20200501_1420.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0009_auto_20200429_1346.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0003_auto_20191024_0854.py
+-rw-rw-rw-   0 root         (0) root         (0)      648 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0006_auto_20200121_1321.py
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0013_auto_20200505_1733.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0005_ldpuser_default_redirect_uri.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0017_auto_20200910_1606.py
+-rw-rw-rw-   0 root         (0) root         (0)      656 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0008_auto_20200130_1251.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0015_auto_20200617_1817.py
+-rw-rw-rw-   0 root         (0) root         (0)      407 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0018_auto_20210223_2254.py
+-rw-rw-rw-   0 root         (0) root         (0)      606 2022-04-12 06:24:01.000000 djangoldp_account-2.3.9/djangoldp_account/migrations/0004_auto_20191203_0921.py
```

### Comparing `djangoldp_account-2.3.8/djangoldp_account.egg-info/SOURCES.txt` & `djangoldp_account-2.3.9/djangoldp_account.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/README.md` & `djangoldp_account-2.3.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -62,17 +62,23 @@
 
 Optionally you can configure which user fields which you would like to include on the registration form by including `REGISTRATION_FIELDS` in settings.py
 
 ```python
 REGISTRATION_FIELDS = ('username', 'email', 'password1', 'password2')
 ```
 
-The workflow starts at : http://127.0.0.1:8000/accounts/register/
+This will be sufficient to change the user fields on display on the form. If you want to customise the form (for example by [adding a model relationship to the user](https://stackoverflow.com/questions/14726725/python-django-django-registration-add-an-extra-field/14879316#14879316)), then you can override the setting `REGISTRATION_USER_FORM` to replace it altogether. The form you supply should extend `djangoldp_account.forms.LDPUserForm` or at minimum `django_registration.forms.RegistrationForm`
 
-Then, override template by copying the directory `djangoldp_account/templates/django_registration/` to your project and modify them.
+```
+REGISTRATION_USER_FORM: "djangoldp_hiphopcommunity.forms.HipHopUserForm"
+```
+
+In either case, at a minimum the registration form fields must include the fields `('username', 'email', 'password1', 'password2')`
+
+Visit http://127.0.0.1:8000/auth/register/ to access the registration form
 
 ### Enabling account activation without mail
 
 Optionally, you can also enable the user account activation without sending the activation mail, by setting:
 
 ```yaml
 SIMPLE_REGISTRATION: True
```

### Comparing `djangoldp_account-2.3.8/setup.cfg` & `djangoldp_account-2.3.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/views.py` & `djangoldp_account-2.3.9/djangoldp_account/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/tests/tests_auth_backends.py` & `djangoldp_account-2.3.9/djangoldp_account/tests/tests_auth_backends.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/tests/models.py` & `djangoldp_account-2.3.9/djangoldp_account/tests/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/tests/tests_update.py` & `djangoldp_account-2.3.9/djangoldp_account/tests/tests_update.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/tests/runner.py` & `djangoldp_account-2.3.9/djangoldp_account/tests/runner.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/models.py` & `djangoldp_account-2.3.9/djangoldp_account/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/endpoints/rp_login.py` & `djangoldp_account-2.3.9/djangoldp_account/endpoints/rp_login.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/endpoints/webfinger.py` & `djangoldp_account-2.3.9/djangoldp_account/endpoints/webfinger.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/permissions.py` & `djangoldp_account-2.3.9/djangoldp_account/permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/templates/registration/password_reset_form.html` & `djangoldp_account-2.3.9/djangoldp_account/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/templates/registration/lost_user.html` & `djangoldp_account-2.3.9/djangoldp_account/templates/registration/lost_user.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/templates/registration/login.html` & `djangoldp_account-2.3.9/djangoldp_account/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/templates/oidc_provider/authorize.html` & `djangoldp_account-2.3.9/djangoldp_account/templates/oidc_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/templates/password/email.html` & `djangoldp_account-2.3.9/djangoldp_account/templates/password/email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/templates/base.html` & `djangoldp_account-2.3.9/djangoldp_account/templates/base.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/templates/django_registration/activation_email_body.txt` & `djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/activation_email_body.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/templates/django_registration/activation_complete.html` & `djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/activation_complete.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/templates/django_registration/registration_form.html` & `djangoldp_account-2.3.9/djangoldp_account/templates/django_registration/registration_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/admin.py` & `djangoldp_account-2.3.9/djangoldp_account/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/djangoldp_urls.py` & `djangoldp_account-2.3.9/djangoldp_account/djangoldp_urls.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """djangoldp project URL Configuration"""
 
+from pydoc import locate
 from django.conf import settings
 from django.conf.urls import url, include
 from django.contrib.auth.models import Group
 from django.views.decorators.csrf import csrf_exempt
 
 from djangoldp.permissions import LDPPermissions
 from djangoldp.views import LDPViewSet
@@ -13,23 +14,26 @@
     LDPAccountRegistrationView
 
 Group._meta.serializer_fields = ['name']
 Group._meta.anonymous_perms = getattr(settings, 'GROUP_ANONYMOUS_PERMISSIONS', ['view'])
 Group._meta.authenticated_perms = getattr(settings, 'GROUP_AUTHENTICATED_PERMISSIONS', ['inherit'])
 Group._meta.owner_perms = getattr(settings, 'GROUP_OWNER_PERMISSIONS', ['inherit'])
 
+user_form_override = getattr(settings, 'REGISTRATION_USER_FORM', None)
+user_form = LDPUserForm if user_form_override is None else locate(user_form_override)
+
 urlpatterns = [
     url(r'^groups/',
         LDPViewSet.urls(model=Group, fields=['@id', 'name', 'user_set'],
                         permission_classes=getattr(settings, 'GROUP_PERMISSION_CLASSES', [LDPPermissions]),
         )
     ),
     url(r'^auth/register/$',
         LDPAccountRegistrationView.as_view(
-            form_class=LDPUserForm
+            form_class=user_form
         ),
         name='django_registration_register',
     ),
     url(r'^auth/login/$', LDPAccountLoginView.as_view(),name='login'),
     url(r'^auth/', include('django_registration.backends.activation.urls')),
     url(r'^auth/', include('django.contrib.auth.urls')),
     url(r'^accounts/', LDPViewSet.urls(model=Account, permission_classes=[LDPPermissions], model_prefix='pk_lookup',
```

### Comparing `djangoldp_account-2.3.8/djangoldp_account/errors.py` & `djangoldp_account-2.3.9/djangoldp_account/errors.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/management/commands/mock_account.py` & `djangoldp_account-2.3.9/djangoldp_account/management/commands/mock_account.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/management/commands/create_distant_admin.py` & `djangoldp_account-2.3.9/djangoldp_account/management/commands/create_distant_admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/management/commands/import_csv.py` & `djangoldp_account-2.3.9/djangoldp_account/management/commands/import_csv.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/management/commands/fill_user_fields.py` & `djangoldp_account-2.3.9/djangoldp_account/management/commands/fill_user_fields.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/factories.py` & `djangoldp_account-2.3.9/djangoldp_account/factories.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/locale/de/LC_MESSAGES/django.po` & `djangoldp_account-2.3.9/djangoldp_account/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/locale/es/LC_MESSAGES/django.po` & `djangoldp_account-2.3.9/djangoldp_account/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/locale/es/LC_MESSAGES/django.mo` & `djangoldp_account-2.3.9/djangoldp_account/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/locale/fr/LC_MESSAGES/django.po` & `djangoldp_account-2.3.9/djangoldp_account/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/locale/fr/LC_MESSAGES/django.mo` & `djangoldp_account-2.3.9/djangoldp_account/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/locale/en/LC_MESSAGES/django.po` & `djangoldp_account-2.3.9/djangoldp_account/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/locale/en/LC_MESSAGES/django.mo` & `djangoldp_account-2.3.9/djangoldp_account/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/forms.py` & `djangoldp_account-2.3.9/djangoldp_account/forms.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/static/base.css` & `djangoldp_account-2.3.9/djangoldp_account/static/base.css`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/static/registration/login.css` & `djangoldp_account-2.3.9/djangoldp_account/static/registration/login.css`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/auth/backends.py` & `djangoldp_account-2.3.9/djangoldp_account/auth/backends.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/auth/middleware.py` & `djangoldp_account-2.3.9/djangoldp_account/auth/middleware.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/auth/solid.py` & `djangoldp_account-2.3.9/djangoldp_account/auth/solid.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/djangoldp_settings.py` & `djangoldp_account-2.3.9/djangoldp_account/djangoldp_settings.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/migrations/0002_auto_20190917_1141.py` & `djangoldp_account-2.3.9/djangoldp_account/migrations/0002_auto_20190917_1141.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/migrations/0012_auto_20200501_1433.py` & `djangoldp_account-2.3.9/djangoldp_account/migrations/0012_auto_20200501_1433.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/migrations/0007_auto_20200130_1242.py` & `djangoldp_account-2.3.9/djangoldp_account/migrations/0007_auto_20200130_1242.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/migrations/0001_initial.py` & `djangoldp_account-2.3.9/djangoldp_account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/migrations/0010_auto_20200501_1207.py` & `djangoldp_account-2.3.9/djangoldp_account/migrations/0010_auto_20200501_1207.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/migrations/0014_auto_20200610_1323.py` & `djangoldp_account-2.3.9/djangoldp_account/migrations/0014_auto_20200610_1323.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/migrations/0016_auto_20200903_1049.py` & `djangoldp_account-2.3.9/djangoldp_account/migrations/0016_auto_20200903_1049.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/migrations/0011_auto_20200501_1420.py` & `djangoldp_account-2.3.9/djangoldp_account/migrations/0011_auto_20200501_1420.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/migrations/0009_auto_20200429_1346.py` & `djangoldp_account-2.3.9/djangoldp_account/migrations/0009_auto_20200429_1346.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/migrations/0003_auto_20191024_0854.py` & `djangoldp_account-2.3.9/djangoldp_account/migrations/0003_auto_20191024_0854.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/migrations/0006_auto_20200121_1321.py` & `djangoldp_account-2.3.9/djangoldp_account/migrations/0006_auto_20200121_1321.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/migrations/0013_auto_20200505_1733.py` & `djangoldp_account-2.3.9/djangoldp_account/migrations/0013_auto_20200505_1733.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/migrations/0017_auto_20200910_1606.py` & `djangoldp_account-2.3.9/djangoldp_account/migrations/0017_auto_20200910_1606.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/migrations/0008_auto_20200130_1251.py` & `djangoldp_account-2.3.9/djangoldp_account/migrations/0008_auto_20200130_1251.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/migrations/0015_auto_20200617_1817.py` & `djangoldp_account-2.3.9/djangoldp_account/migrations/0015_auto_20200617_1817.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-2.3.8/djangoldp_account/migrations/0004_auto_20191203_0921.py` & `djangoldp_account-2.3.9/djangoldp_account/migrations/0004_auto_20191203_0921.py`

 * *Files identical despite different names*

