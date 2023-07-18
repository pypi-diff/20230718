# Comparing `tmp/aleksis_core-3.1.2.tar.gz` & `tmp/aleksis_core-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_core-3.1.2.tar", max compression
+gzip compressed data, was "aleksis_core-3.1.3.tar", max compression
```

## Comparing `aleksis_core-3.1.2.tar` & `aleksis_core-3.1.3.tar`

### file list

```diff
@@ -1,490 +1,490 @@
--rw-r--r--   0        0        0    38157 2023-07-05 19:54:43.393550 aleksis_core-3.1.2/CHANGELOG.rst
--rw-r--r--   0        0        0    14353 2023-07-05 19:54:43.393550 aleksis_core-3.1.2/LICENCE.rst
--rw-r--r--   0        0        0     3786 2023-07-05 19:54:43.393550 aleksis_core-3.1.2/README.rst
--rw-r--r--   0        0        0      194 2023-07-05 19:54:43.393550 aleksis_core-3.1.2/aleksis/core/__init__.py
--rw-r--r--   0        0        0      464 2023-07-05 19:54:43.393550 aleksis_core-3.1.2/aleksis/core/__main__.py
--rw-r--r--   0        0        0      510 2023-07-05 19:58:31.878172 aleksis_core-3.1.2/aleksis/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1068 2023-07-05 19:58:35.354303 aleksis_core-3.1.2/aleksis/core/__pycache__/__main__.cpython-311.pyc
--rw-r--r--   0        0        0     2061 2023-07-05 19:58:42.118558 aleksis_core-3.1.2/aleksis/core/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0        0        0    11380 2023-07-05 19:58:38.138408 aleksis_core-3.1.2/aleksis/core/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0     2533 2023-07-05 19:58:31.942174 aleksis_core-3.1.2/aleksis/core/__pycache__/celery.cpython-311.pyc
--rw-r--r--   0        0        0     3716 2023-07-05 19:58:42.298565 aleksis_core-3.1.2/aleksis/core/__pycache__/checks.cpython-311.pyc
--rw-r--r--   0        0        0    17897 2023-07-05 19:58:41.434532 aleksis_core-3.1.2/aleksis/core/__pycache__/data_checks.cpython-311.pyc
--rw-r--r--   0        0        0     5154 2023-07-05 19:58:42.318566 aleksis_core-3.1.2/aleksis/core/__pycache__/health_checks.cpython-311.pyc
--rw-r--r--   0        0        0     8423 2023-07-05 19:58:41.518535 aleksis_core-3.1.2/aleksis/core/__pycache__/managers.cpython-311.pyc
--rw-r--r--   0        0        0    31446 2023-07-05 19:58:41.454533 aleksis_core-3.1.2/aleksis/core/__pycache__/mixins.cpython-311.pyc
--rw-r--r--   0        0        0    85606 2023-07-05 19:58:40.354492 aleksis_core-3.1.2/aleksis/core/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0    22237 2023-07-05 19:58:42.478572 aleksis_core-3.1.2/aleksis/core/__pycache__/preferences.cpython-311.pyc
--rw-r--r--   0        0        0     1370 2023-07-05 19:58:38.198410 aleksis_core-3.1.2/aleksis/core/__pycache__/registries.cpython-311.pyc
--rw-r--r--   0        0        0    16523 2023-07-05 19:58:42.154559 aleksis_core-3.1.2/aleksis/core/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0    44046 2023-07-05 19:58:35.430306 aleksis_core-3.1.2/aleksis/core/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0        0        0     3825 2023-07-05 19:58:41.542537 aleksis_core-3.1.2/aleksis/core/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0        0        0      950 2023-07-05 19:54:43.393550 aleksis_core-3.1.2/aleksis/core/admin.py
--rw-r--r--   0        0        0     8519 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/apps.py
--rw-r--r--   0        0        0     1338 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/celery.py
--rw-r--r--   0        0        0     2751 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/checks.py
--rw-r--r--   0        0        0    11534 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/data_checks.py
--rw-r--r--   0        0        0      741 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/decorators.py
--rw-r--r--   0        0        0     5556 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/filters.py
--rw-r--r--   0        0        0    31619 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/forms.py
--rw-r--r--   0        0        0     3175 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/app/apollo.js
--rw-r--r--   0        0        0     1089 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/app/dateTimeFormats.js
--rw-r--r--   0        0        0      197 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/app/i18n.js
--rw-r--r--   0        0        0      157 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/app/router.js
--rw-r--r--   0        0        0      133 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/app/sentry.js
--rw-r--r--   0        0        0      793 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/app/vuetify.js
--rw-r--r--   0        0        0     4485 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/LegacyBaseTemplate.vue
--rw-r--r--   0        0        0      158 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/Parent.vue
--rw-r--r--   0        0        0      335 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/about/About.vue
--rw-r--r--   0        0        0     1971 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/about/AboutAleksis.vue
--rw-r--r--   0        0        0     3831 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/about/InstalledAppCard.vue
--rw-r--r--   0        0        0     1003 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/about/InstalledAppsList.vue
--rw-r--r--   0        0        0      351 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/about/installedApps.graphql
--rw-r--r--   0        0        0     2411 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/AccountMenu.vue
--rw-r--r--   0        0        0     9590 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/App.vue
--rw-r--r--   0        0        0      314 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/BrandLogo.vue
--rw-r--r--   0        0        0     1064 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/ErrorPage.vue
--rw-r--r--   0        0        0     1470 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/LanguageForm.vue
--rw-r--r--   0        0        0     3778 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/SideNav.vue
--rw-r--r--   0        0        0     1454 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/SidenavSearch.vue
--rw-r--r--   0        0        0      747 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/SnackbarItem.vue
--rw-r--r--   0        0        0     1932 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/Splash.vue
--rw-r--r--   0        0        0      124 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/customMenu.graphql
--rw-r--r--   0        0        0      205 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/dynamicRoutes.graphql
--rw-r--r--   0        0        0       42 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/messages.graphql
--rw-r--r--   0        0        0       59 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/ping.graphql
--rw-r--r--   0        0        0      139 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/searchSnippets.graphql
--rw-r--r--   0        0        0      412 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/systemProperties.graphql
--rw-r--r--   0        0        0      322 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/whoAmI.graphql
--rw-r--r--   0        0        0     2558 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue
--rw-r--r--   0        0        0     1884 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue
--rw-r--r--   0        0        0      220 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/authorized_oauth_applications/accessTokens.graphql
--rw-r--r--   0        0        0       65 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/authorized_oauth_applications/revokeOauthToken.graphql
--rw-r--r--   0        0        0     3482 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue
--rw-r--r--   0        0        0     1910 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue
--rw-r--r--   0        0        0      925 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/celery_progress/TaskListItem.vue
--rw-r--r--   0        0        0      432 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/celery_progress/celeryProgress.graphql
--rw-r--r--   0        0        0      191 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/celery_progress/celeryProgressBottom.graphql
--rw-r--r--   0        0        0      118 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/celery_progress/celeryProgressFetched.graphql
--rw-r--r--   0        0        0      655 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/generic/AvatarClickbox.vue
--rw-r--r--   0        0        0      212 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/generic/BackButton.vue
--rw-r--r--   0        0        0      598 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/generic/ButtonMenu.vue
--rw-r--r--   0        0        0      981 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/generic/DetailView.vue
--rw-r--r--   0        0        0      408 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/generic/ListView.vue
--rw-r--r--   0        0        0      268 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/generic/MessageBox.vue
--rw-r--r--   0        0        0     1914 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/generic/ObjectOverview.vue
--rw-r--r--   0        0        0      269 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/generic/SmallContainer.vue
--rw-r--r--   0        0        0     2017 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/generic/UpdateIndicator.vue
--rw-r--r--   0        0        0     3232 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue
--rw-r--r--   0        0        0      706 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/group/GroupCollection.vue
--rw-r--r--   0        0        0     3034 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/notifications/NotificationItem.vue
--rw-r--r--   0        0        0     2616 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/notifications/NotificationList.vue
--rw-r--r--   0        0        0      107 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/notifications/markNotificationRead.graphql
--rw-r--r--   0        0        0      200 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/notifications/myNotifications.graphql
--rw-r--r--   0        0        0     1017 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/pdf/DownloadPDF.vue
--rw-r--r--   0        0        0       78 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/pdf/pdf.graphql
--rw-r--r--   0        0        0     1410 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/person/AdditionalImage.vue
--rw-r--r--   0        0        0     1082 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/person/AvatarContent.vue
--rw-r--r--   0        0        0     2892 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/person/PersonActions.vue
--rw-r--r--   0        0        0      527 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue
--rw-r--r--   0        0        0      759 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/person/PersonCollection.vue
--rw-r--r--   0        0        0     7423 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/person/PersonOverview.vue
--rw-r--r--   0        0        0      108 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/person/avatarContent.graphql
--rw-r--r--   0        0        0      196 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/person/personActions.graphql
--rw-r--r--   0        0        0      575 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/person/personOverview.graphql
--rw-r--r--   0        0        0     3858 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/two_factor/TwoFactor.vue
--rw-r--r--   0        0        0     1512 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue
--rw-r--r--   0        0        0      589 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue
--rw-r--r--   0        0        0      385 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/two_factor/twoFactor.graphql
--rw-r--r--   0        0        0      390 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/css/global.scss
--rw-r--r--   0        0        0     2561 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/index.js
--rw-r--r--   0        0        0    10763 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/messages/de.json
--rw-r--r--   0        0        0     9741 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/messages/en.json
--rw-r--r--   0        0        0    12252 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/messages/ru.json
--rw-r--r--   0        0        0    14534 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/messages/uk.json
--rw-r--r--   0        0        0     1211 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/mixins/aleksis.js
--rw-r--r--   0        0        0      538 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/mixins/error404.js
--rw-r--r--   0        0        0     3441 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/mixins/menus.js
--rw-r--r--   0        0        0     2256 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/mixins/offline.js
--rw-r--r--   0        0        0      736 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/mixins/permissions.js
--rw-r--r--   0        0        0     2154 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/mixins/routes.js
--rw-r--r--   0        0        0     1619 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/mixins/useRegisterSW.js
--rw-r--r--   0        0        0     6380 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/plugins/aleksis.js
--rw-r--r--   0        0        0      450 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/routeValidators.js
--rw-r--r--   0        0        0    36573 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/frontend/routes.js
--rw-r--r--   0        0        0     2642 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/health_checks.py
--rw-r--r--   0        0        0      487 2023-07-05 19:58:43.062594 aleksis_core-3.1.2/aleksis/core/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74307 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      463 2023-07-05 19:58:43.050593 aleksis_core-3.1.2/aleksis/core/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      894 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    63806 2023-07-05 19:58:43.038593 aleksis_core-3.1.2/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   126085 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      567 2023-07-05 19:58:43.006592 aleksis_core-3.1.2/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1118 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      942 2023-07-05 19:58:42.990591 aleksis_core-3.1.2/aleksis/core/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    77782 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-07-05 19:58:43.022592 aleksis_core-3.1.2/aleksis/core/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      810 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     2584 2023-07-05 19:58:43.146597 aleksis_core-3.1.2/aleksis/core/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    82875 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-07-05 19:58:43.146597 aleksis_core-3.1.2/aleksis/core/locale/la/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/locale/la/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      361 2023-07-05 19:58:43.106596 aleksis_core-3.1.2/aleksis/core/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74237 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-07-05 19:58:43.058594 aleksis_core-3.1.2/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    80303 2023-07-05 19:58:43.146597 aleksis_core-3.1.2/aleksis/core/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   144575 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      713 2023-07-05 19:58:43.182598 aleksis_core-3.1.2/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1321 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      361 2023-07-05 19:58:42.998592 aleksis_core-3.1.2/aleksis/core/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74177 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-07-05 19:58:42.990591 aleksis_core-3.1.2/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    77610 2023-07-05 19:58:43.118596 aleksis_core-3.1.2/aleksis/core/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   131787 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      713 2023-07-05 19:58:43.070594 aleksis_core-3.1.2/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1331 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0        0 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/management/__init__.py
--rw-r--r--   0        0        0     3957 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/management/commands/convert_urls_to_routes.py
--rw-r--r--   0        0        0      945 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/management/commands/vite.py
--rw-r--r--   0        0        0      439 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/management/commands/webpack_bundle.py
--rw-r--r--   0        0        0     4690 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/managers.py
--rw-r--r--   0        0        0    51004 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0001_initial.py
--rw-r--r--   0        0        0     2473 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0002_school_term.py
--rw-r--r--   0        0        0      531 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0003_drop_image_cropping.py
--rw-r--r--   0        0        0      796 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0004_add_permissions_for_group_stats.py
--rw-r--r--   0        0        0     1252 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0005_timestamped_activity_notification.py
--rw-r--r--   0        0        0     1567 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0006_dashboard_widget_size.py
--rw-r--r--   0        0        0     1396 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0007_dashboard_widget_order.py
--rw-r--r--   0        0        0     2311 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0008_data_check_result.py
--rw-r--r--   0        0        0     1052 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0009_default_dashboard.py
--rw-r--r--   0        0        0      952 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0010_external_link_widget.py
--rw-r--r--   0        0        0      829 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0011_globalpermissions_options.py
--rw-r--r--   0        0        0      501 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0012_valid_from_announcement.py
--rw-r--r--   0        0        0     2270 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0013_pdf_file.py
--rw-r--r--   0        0        0      533 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0014_alter_pdffile_file.py
--rw-r--r--   0        0        0     1174 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0015_oauth_permissions.py
--rw-r--r--   0        0        0     1538 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0016_taskuserassignment.py
--rw-r--r--   0        0        0      426 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0017_dashboardwidget_broken.py
--rw-r--r--   0        0        0      897 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0018_pdffile_html_file.py
--rw-r--r--   0        0        0     2177 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0019_fix_uniqueness_per_site.py
--rw-r--r--   0        0        0      542 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0020_pdf_file_person_optional.py
--rw-r--r--   0        0        0     1084 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0021_drop_persons_accounts_perm.py
--rw-r--r--   0        0        0      923 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0022_public_favicon.py
--rw-r--r--   0        0        0     6340 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0023_oauth_application_model.py
--rw-r--r--   0        0        0      714 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0024_oauth_grant_types_optional.py
--rw-r--r--   0        0        0     1717 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0025_oauth_align_user_fk.py
--rw-r--r--   0        0        0      582 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py
--rw-r--r--   0        0        0      457 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0027_person_place_of_birth.py
--rw-r--r--   0        0        0      947 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0028_char_field_not_null.py
--rw-r--r--   0        0        0     1465 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0029_invitations.py
--rw-r--r--   0        0        0     1776 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0030_user_attributes.py
--rw-r--r--   0        0        0      526 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0031_oauthapplication_icon.py
--rw-r--r--   0        0        0      340 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0032_remove_person_is_active.py
--rw-r--r--   0        0        0     2416 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0033_update_photo_avatar.py
--rw-r--r--   0        0        0      816 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0034_invite_permission.py
--rw-r--r--   0        0        0     1781 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0035_preference_model_unique.py
--rw-r--r--   0        0        0      626 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0036_additionalfields_helptext_required.py
--rw-r--r--   0        0        0      917 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0037_add_static_content_widget.py
--rw-r--r--   0        0        0      522 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0038_notification_send_at.py
--rw-r--r--   0        0        0     1029 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0039_personal_ical_url.py
--rw-r--r--   0        0        0      613 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py
--rw-r--r--   0        0        0      516 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0041_update_gender_choices.py
--rw-r--r--   0        0        0      547 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0042_pdffile_empty.py
--rw-r--r--   0        0        0     2261 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0043_task_assignment_meta.py
--rw-r--r--   0        0        0      532 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0044_task_assignment_result_fetched.py
--rw-r--r--   0        0        0      486 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0045_data_check_result_fix_check_field.py
--rw-r--r--   0        0        0   290966 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0046_notification_create_field_icon.py
--rw-r--r--   0        0        0     2717 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0047_add_room_model.py
--rw-r--r--   0        0        0   893996 2023-07-05 19:54:43.417551 aleksis_core-3.1.2/aleksis/core/migrations/0048_delete_personalicalurl.py
--rw-r--r--   0        0        0      580 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py
--rw-r--r--   0        0        0        0 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/migrations/__init__.py
--rw-r--r--   0        0        0    19769 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/mixins.py
--rw-r--r--   0        0        0    51781 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/models.py
--rw-r--r--   0        0        0    13478 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/preferences.py
--rw-r--r--   0        0        0      692 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/registries.py
--rw-r--r--   0        0        0    16018 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/rules.py
--rw-r--r--   0        0        0     7486 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/__init__.py
--rw-r--r--   0        0        0     1301 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/base.py
--rw-r--r--   0        0        0     3049 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/celery_progress.py
--rw-r--r--   0        0        0      585 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/custom_menu.py
--rw-r--r--   0        0        0      459 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/dynamic_routes.py
--rw-r--r--   0        0        0     2046 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/group.py
--rw-r--r--   0        0        0     1743 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/installed_apps.py
--rw-r--r--   0        0        0      265 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/message.py
--rw-r--r--   0        0        0     1296 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/notification.py
--rw-r--r--   0        0        0     1179 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/oauth.py
--rw-r--r--   0        0        0      535 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/pdf.py
--rw-r--r--   0        0        0      124 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/permissions.py
--rw-r--r--   0        0        0     9708 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/person.py
--rw-r--r--   0        0        0      191 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/room.py
--rw-r--r--   0        0        0      163 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/school_term.py
--rw-r--r--   0        0        0      868 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/search.py
--rw-r--r--   0        0        0     1343 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/site_preferences.py
--rw-r--r--   0        0        0     1651 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/system_properties.py
--rw-r--r--   0        0        0     3297 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/two_factor.py
--rw-r--r--   0        0        0      829 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/user.py
--rw-r--r--   0        0        0      418 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/search_indexes.py
--rw-r--r--   0        0        0    39939 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/settings.py
--rw-r--r--   0        0        0    49621 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/static/img/aleksis-banner.svg
--rw-r--r--   0        0        0     1862 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/static/img/aleksis-favicon.png
--rw-r--r--   0        0        0    17172 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/static/img/aleksis-icon-maskable.png
--rw-r--r--   0        0        0     7843 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/img/aleksis-icon-maskable.svg
--rw-r--r--   0        0        0    31902 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/img/aleksis-icon.png
--rw-r--r--   0        0        0     7346 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/img/aleksis-icon.svg
--rw-r--r--   0        0        0    19126 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/img/fallback.png
--rw-r--r--   0        0        0     2237 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/img/hero.svg
--rw-r--r--   0        0        0      490 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/js/copy_button.js
--rw-r--r--   0        0        0      521 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/js/edit_dashboard.js
--rw-r--r--   0        0        0      618 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/js/helper.js
--rw-r--r--   0        0        0      984 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/js/include_ajax_live.js
--rw-r--r--   0        0        0     4350 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/js/main.js
--rw-r--r--   0        0        0     1654 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/js/multi_select.js
--rw-r--r--   0        0        0     3495 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/js/search.js
--rw-r--r--   0        0        0     2578 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/js/serviceworker.js
--rw-r--r--   0        0        0      271 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/print-simple.css
--rw-r--r--   0        0        0     1627 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/print.css
--rw-r--r--   0        0        0      187 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/print_landscape.css
--rw-r--r--   0        0        0     1064 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/public/materialize-custom.scss
--rw-r--r--   0        0        0    15745 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/public/style.scss
--rw-r--r--   0        0        0    11345 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/public/theme.scss
--rw-r--r--   0        0        0     6876 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/tables.py
--rw-r--r--   0        0        0     2330 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/tasks.py
--rw-r--r--   0        0        0      838 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/403.html
--rw-r--r--   0        0        0      789 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/404.html
--rw-r--r--   0        0        0      918 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/500.html
--rw-r--r--   0        0        0       76 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/503.html
--rw-r--r--   0        0        0      851 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/account_inactive.html
--rw-r--r--   0        0        0      169 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/email/base_message.txt
--rw-r--r--   0        0        0      525 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/email/email_confirmation_message.txt
--rw-r--r--   0        0        0     1255 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/email_confirm.html
--rw-r--r--   0        0        0      804 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/password_change.html
--rw-r--r--   0        0        0      888 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/password_change_disabled.html
--rw-r--r--   0        0        0     1376 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/password_reset.html
--rw-r--r--   0        0        0      825 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/password_reset_done.html
--rw-r--r--   0        0        0     2305 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/password_reset_from_key.html
--rw-r--r--   0        0        0      649 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/password_reset_from_key_done.html
--rw-r--r--   0        0        0      500 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/password_set.html
--rw-r--r--   0        0        0      888 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/signup.html
--rw-r--r--   0        0        0      838 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/signup_closed.html
--rw-r--r--   0        0        0      820 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/verification_email_required.html
--rw-r--r--   0        0        0     1160 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/verification_sent.html
--rw-r--r--   0        0        0      979 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/components/chips.html
--rw-r--r--   0        0        0      350 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/components/materialize-chips.html
--rw-r--r--   0        0        0      225 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/components/msgbox.html
--rw-r--r--   0        0        0      958 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/components/pagination.html
--rw-r--r--   0        0        0      486 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/components/text_collapsible.html
--rw-r--r--   0        0        0      483 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/additional_field/edit.html
--rw-r--r--   0        0        0      594 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/additional_field/list.html
--rw-r--r--   0        0        0     1053 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/announcement/form.html
--rw-r--r--   0        0        0     1900 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/announcement/list.html
--rw-r--r--   0        0        0     3099 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/base.html
--rw-r--r--   0        0        0     2454 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/base_print.html
--rw-r--r--   0        0        0     1178 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/base_simple_print.html
--rw-r--r--   0        0        0      628 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/dashboard_widget/create.html
--rw-r--r--   0        0        0      635 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html
--rw-r--r--   0        0        0      626 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/dashboard_widget/edit.html
--rw-r--r--   0        0        0      262 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/dashboard_widget/external_link_widget.html
--rw-r--r--   0        0        0     1349 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/dashboard_widget/list.html
--rw-r--r--   0        0        0      226 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/dashboard_widget/static_content_widget.html
--rw-r--r--   0        0        0     3879 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/data_check/list.html
--rw-r--r--   0        0        0     2233 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/edit_dashboard.html
--rw-r--r--   0        0        0        0 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/empty.html
--rw-r--r--   0        0        0     5310 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/group/child_groups.html
--rw-r--r--   0        0        0      650 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/group/edit.html
--rw-r--r--   0        0        0     3382 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/group/full.html
--rw-r--r--   0        0        0     1019 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/group/list.html
--rw-r--r--   0        0        0      465 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/group_type/edit.html
--rw-r--r--   0        0        0      564 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/group_type/list.html
--rw-r--r--   0        0        0     2504 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/index.html
--rw-r--r--   0        0        0      777 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/pages/delete.html
--rw-r--r--   0        0        0     6832 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/pages/system_status.html
--rw-r--r--   0        0        0      603 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/pages/test_pdf.html
--rw-r--r--   0        0        0       93 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/address.html
--rw-r--r--   0        0        0      189 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/admins_list.html
--rw-r--r--   0        0        0     1632 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/announcements.html
--rw-r--r--   0        0        0     1472 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/avatar_content.html
--rw-r--r--   0        0        0      319 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/copy_button.html
--rw-r--r--   0        0        0     1089 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/crud_events.html
--rw-r--r--   0        0        0      389 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/edit_dashboard_widget.html
--rw-r--r--   0        0        0     1624 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/meta.html
--rw-r--r--   0        0        0      414 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/on_page_menu.html
--rw-r--r--   0        0        0      260 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/save_button.html
--rw-r--r--   0        0        0     2374 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/splash_screen.html
--rw-r--r--   0        0        0      325 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/turnable.html
--rw-r--r--   0        0        0      915 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/perms/assign.html
--rw-r--r--   0        0        0     2478 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/perms/list.html
--rw-r--r--   0        0        0      376 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/person/collection.html
--rw-r--r--   0        0        0      649 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/person/create.html
--rw-r--r--   0        0        0      645 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/person/edit.html
--rw-r--r--   0        0        0     1165 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/person/list.html
--rw-r--r--   0        0        0      455 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/school_term/create.html
--rw-r--r--   0        0        0      451 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/school_term/edit.html
--rw-r--r--   0        0        0      556 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/school_term/list.html
--rw-r--r--   0        0        0      935 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/vue_index.html
--rw-r--r--   0        0        0     3921 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/django_tables2/materialize.html
--rw-r--r--   0        0        0      981 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/dynamic_preferences/form.html
--rw-r--r--   0        0        0      376 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/dynamic_preferences/sections.html
--rw-r--r--   0        0        0      764 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/invitations/disabled.html
--rw-r--r--   0        0        0     1281 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/invitations/enter.html
--rw-r--r--   0        0        0     1162 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/invitations/forms/_invite.html
--rw-r--r--   0        0        0      102 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/invitations/messages/invite_accepted.txt
--rw-r--r--   0        0        0      171 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/material/field_errors.html
--rw-r--r--   0        0        0     1232 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html
--rw-r--r--   0        0        0     1897 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/material/fields/colorfield_colorwidget.html
--rw-r--r--   0        0        0     1009 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html
--rw-r--r--   0        0        0     1009 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/material/fields/django_select2_select2widget.html
--rw-r--r--   0        0        0      253 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/material/non_field_errors.html
--rw-r--r--   0        0        0      663 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/oauth2_provider/application/create.html
--rw-r--r--   0        0        0     2335 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/oauth2_provider/application/detail.html
--rw-r--r--   0        0        0      669 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/oauth2_provider/application/edit.html
--rw-r--r--   0        0        0     1074 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/oauth2_provider/application/list.html
--rw-r--r--   0        0        0     2686 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/oauth2_provider/authorize.html
--rw-r--r--   0        0        0      887 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/offline.html
--rw-r--r--   0        0        0       42 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/search/indexes/core/group_text.txt
--rw-r--r--   0        0        0       69 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/search/indexes/core/person_text.txt
--rw-r--r--   0        0        0       42 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/search/indexes/core/room_text.txt
--rw-r--r--   0        0        0     3171 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/search/search.html
--rw-r--r--   0        0        0      243 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/search/searchbar_snippet.html
--rw-r--r--   0        0        0      150 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/search/searchbar_snippets.html
--rw-r--r--   0        0        0      169 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/sms/notification.txt
--rw-r--r--   0        0        0      893 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/socialaccount/authentication_error.html
--rw-r--r--   0        0        0     1268 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/socialaccount/connections.html
--rw-r--r--   0        0        0     1289 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/socialaccount/login.html
--rw-r--r--   0        0        0      809 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/socialaccount/login_cancelled.html
--rw-r--r--   0        0        0     1012 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/socialaccount/signup.html
--rw-r--r--   0        0        0     1434 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/socialaccount/snippets/provider_list.html
--rw-r--r--   0        0        0      630 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/templated_email/base.email
--rw-r--r--   0        0        0     1527 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/templated_email/celery_failure.email
--rw-r--r--   0        0        0      994 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/templated_email/data_checks.email
--rw-r--r--   0        0        0      990 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/templated_email/email.css
--rw-r--r--   0        0        0     1102 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/templated_email/invitation.email
--rw-r--r--   0        0        0     1461 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/templated_email/notification.email
--rw-r--r--   0        0        0      668 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/templated_email/person_changed.email
--rw-r--r--   0        0        0      219 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/two_factor/_base_focus.html
--rw-r--r--   0        0        0      877 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/two_factor/_wizard_actions.html
--rw-r--r--   0        0        0      119 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/two_factor/_wizard_forms.html
--rw-r--r--   0        0        0     1780 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/backup_tokens.html
--rw-r--r--   0        0        0     6712 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/login.html
--rw-r--r--   0        0        0      943 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/otp_required.html
--rw-r--r--   0        0        0      986 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/phone_register.html
--rw-r--r--   0        0        0     3312 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/setup.html
--rw-r--r--   0        0        0     2127 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/setup_complete.html
--rw-r--r--   0        0        0      786 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/two_factor/profile/disable.html
--rw-r--r--   0        0        0        0 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templatetags/__init__.py
--rw-r--r--   0        0        0       99 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templatetags/apps.py
--rw-r--r--   0        0        0      394 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templatetags/dashboard.py
--rw-r--r--   0        0        0     1618 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templatetags/data_helpers.py
--rw-r--r--   0        0        0     1523 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templatetags/html_helpers.py
--rw-r--r--   0        0        0      206 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templatetags/msg_box.py
--rw-r--r--   0        0        0     3696 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/browser/test_selenium.py
--rw-r--r--   0        0        0     6596 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/models/test.pdf
--rw-r--r--   0        0        0     6562 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/models/test_group.py
--rw-r--r--   0        0        0     1520 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/models/test_group_sync.py
--rw-r--r--   0        0        0     3049 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/models/test_notification.py
--rw-r--r--   0        0        0     4003 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/models/test_pdffile.py
--rw-r--r--   0        0        0      427 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/models/test_person.py
--rw-r--r--   0        0        0     5503 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/regression/test_regression.py
--rw-r--r--   0        0        0      683 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/regression/view_oauth.py
--rw-r--r--   0        0        0     1021 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/templatetags/test_data_helpers.py
--rw-r--r--   0        0        0     2292 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/views/test_account.py
--rw-r--r--   0        0        0    18734 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/urls.py
--rw-r--r--   0        0        0        0 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/util/__init__.py
--rw-r--r--   0        0        0      176 2023-07-05 19:58:33.254224 aleksis_core-3.1.2/aleksis/core/util/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    14902 2023-07-05 19:58:38.202410 aleksis_core-3.1.2/aleksis/core/util/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0    10101 2023-07-05 19:58:41.534536 aleksis_core-3.1.2/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc
--rw-r--r--   0        0        0    24932 2023-07-05 19:58:33.266224 aleksis_core-3.1.2/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     1500 2023-07-05 19:58:35.266300 aleksis_core-3.1.2/aleksis/core/util/__pycache__/email.cpython-311.pyc
--rw-r--r--   0        0        0      771 2023-07-05 19:58:41.570537 aleksis_core-3.1.2/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     5712 2023-07-05 19:58:41.542537 aleksis_core-3.1.2/aleksis/core/util/__pycache__/notifications.cpython-311.pyc
--rw-r--r--   0        0        0     9548 2023-07-05 19:58:42.170560 aleksis_core-3.1.2/aleksis/core/util/__pycache__/predicates.cpython-311.pyc
--rw-r--r--   0        0        0     2181 2023-07-05 19:58:38.274413 aleksis_core-3.1.2/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc
--rw-r--r--   0        0        0      664 2023-07-05 19:58:38.270413 aleksis_core-3.1.2/aleksis/core/util/__pycache__/spdx.cpython-311.pyc
--rw-r--r--   0        0        0    10969 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/util/apps.py
--rw-r--r--   0        0        0     5970 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/util/auth_helpers.py
--rw-r--r--   0        0        0     7920 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/util/celery_progress.py
--rw-r--r--   0        0        0      197 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/util/context_processors.py
--rw-r--r--   0        0        0    16042 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/core_helpers.py
--rw-r--r--   0        0        0      986 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/email.py
--rw-r--r--   0        0        0     1175 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/forms.py
--rw-r--r--   0        0        0     2895 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/frontend_helpers.py
--rw-r--r--   0        0        0     2375 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/ldap.py
--rw-r--r--   0        0        0   192829 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/licenses.json
--rw-r--r--   0        0        0     2255 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/messages.py
--rw-r--r--   0        0        0     2091 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/middlewares.py
--rw-r--r--   0        0        0      850 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/model_helpers.py
--rw-r--r--   0        0        0     3732 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/notifications.py
--rw-r--r--   0        0        0     6131 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/pdf.py
--rw-r--r--   0        0        0     5583 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/predicates.py
--rw-r--r--   0        0        0      936 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/sass_helpers.py
--rw-r--r--   0        0        0      524 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/search.py
--rw-r--r--   0        0        0      130 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/spdx.py
--rw-r--r--   0        0        0     1673 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/tables.py
--rw-r--r--   0        0        0    55996 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/views.py
--rw-r--r--   0        0        0    10257 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/vite.config.js
--rw-r--r--   0        0        0      173 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/wsgi.py
--rw-r--r--   0        0        0       45 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/conftest.py
--rw-r--r--   0        0        0      581 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/docs/Makefile
--rw-r--r--   0        0        0   127432 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/docs/_static/2fa.png
--rw-r--r--   0        0        0    71362 2023-07-05 19:54:43.441552 aleksis_core-3.1.2/docs/_static/accept_invite.png
--rw-r--r--   0        0        0    72621 2023-07-05 19:54:43.441552 aleksis_core-3.1.2/docs/_static/create_dashboard_widget.png
--rw-r--r--   0        0        0    41935 2023-07-05 19:54:43.441552 aleksis_core-3.1.2/docs/_static/create_social_application.png
--rw-r--r--   0        0        0    72508 2023-07-05 19:54:43.441552 aleksis_core-3.1.2/docs/_static/dashboard.png
--rw-r--r--   0        0        0    87601 2023-07-05 19:54:43.441552 aleksis_core-3.1.2/docs/_static/dashboard_widgets.png
--rw-r--r--   0        0        0   119523 2023-07-05 19:54:43.441552 aleksis_core-3.1.2/docs/_static/data_checks.png
--rw-r--r--   0        0        0    81386 2023-07-05 19:54:43.441552 aleksis_core-3.1.2/docs/_static/edit_dashboard.png
--rw-r--r--   0        0        0    85722 2023-07-05 19:54:43.445552 aleksis_core-3.1.2/docs/_static/edit_default_dashboard.png
--rw-r--r--   0        0        0   107979 2023-07-05 19:54:43.445552 aleksis_core-3.1.2/docs/_static/invitations.png
--rw-r--r--   0        0        0   177681 2023-07-05 19:54:43.445552 aleksis_core-3.1.2/docs/_static/invite_existing.png
--rw-r--r--   0        0        0    44868 2023-07-05 19:54:43.445552 aleksis_core-3.1.2/docs/_static/pwa_desktop_chromium.png
--rw-r--r--   0        0        0    69215 2023-07-05 19:54:43.445552 aleksis_core-3.1.2/docs/_static/pwa_mobile_chromium.png
--rw-r--r--   0        0        0   128479 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/_static/pwa_mobile_firefox.png
--rw-r--r--   0        0        0   108973 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/_static/pwa_mobile_safari.png
--rw-r--r--   0        0        0    69804 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/_static/signup.png
--rw-r--r--   0        0        0      132 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/00_index.rst
--rw-r--r--   0        0        0     4231 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/01_core_concepts.rst
--rw-r--r--   0        0        0     8067 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/10_install.rst
--rw-r--r--   0        0        0     1872 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/15_config_files.rst
--rw-r--r--   0        0        0     2086 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/16_config_options.rst
--rw-r--r--   0        0        0     1648 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/17_storage.rst
--rw-r--r--   0        0        0      803 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/18_mail.rst
--rw-r--r--   0        0        0     1509 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/21_ldap.rst
--rw-r--r--   0        0        0     3037 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/22_registration.rst
--rw-r--r--   0        0        0     1467 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/23_socialaccounts.rst
--rw-r--r--   0        0        0     3218 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/31_monitoring.rst
--rw-r--r--   0        0        0     1012 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/32_tasks.rst
--rw-r--r--   0        0        0     1393 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/33_data_checks.rst
--rw-r--r--   0        0        0     4610 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/50_dashboard.rst
--rw-r--r--   0        0        0     6393 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/conf.py
--rw-r--r--   0        0        0      132 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/dev/00_index.rst
--rw-r--r--   0        0        0     4058 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/dev/01_setup.rst
--rw-r--r--   0        0        0     1427 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/dev/02_install_apps.rst
--rw-r--r--   0        0        0     3117 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/dev/03_run_tests.rst
--rw-r--r--   0        0        0     4519 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/dev/04_materialize_templates.rst
--rw-r--r--   0        0        0      289 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/dev/05_extensible_models.rst
--rw-r--r--   0        0        0     1148 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/dev/06_merging_app_settings.rst
--rw-r--r--   0        0        0     1349 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/dev/10_dashboard_widgets.rst
--rw-r--r--   0        0        0      514 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/index.rst
--rw-r--r--   0        0        0      787 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/make.bat
--rw-r--r--   0        0        0       95 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/00_index.rst
--rw-r--r--   0        0        0       69 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/01_checks.rst
--rw-r--r--   0        0        0       70 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/02_managers.rst
--rw-r--r--   0        0        0       64 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/03_mixins.rst
--rw-r--r--   0        0        0       84 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/04_models.rst
--rw-r--r--   0        0        0      108 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/05_registries.rst
--rw-r--r--   0        0        0       93 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/06_search_indexes.rst
--rw-r--r--   0        0        0       79 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/07_tables.rst
--rw-r--r--   0        0        0       90 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/08_tasks.rst
--rw-r--r--   0        0        0     1017 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/09_utils.rst
--rw-r--r--   0        0        0       71 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/10_views.rst
--rw-r--r--   0        0        0       77 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/11_filters.rst
--rw-r--r--   0        0        0      373 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/12_template_tags.rst
--rw-r--r--   0        0        0      112 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/user/00_index.rst
--rw-r--r--   0        0        0     1152 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/user/01_registration.rst
--rw-r--r--   0        0        0     3465 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/user/02_personal_account.rst
--rw-r--r--   0        0        0     1770 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/user/10_dashboard.rst
--rw-r--r--   0        0        0     2607 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/user/20_pwa.rst
--rw-r--r--   0        0        0     5377 2023-07-05 19:55:26.067160 aleksis_core-3.1.2/pyproject.toml
--rw-r--r--   0        0        0     2599 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/tox.ini
--rw-r--r--   0        0        0     8603 1970-01-01 00:00:00.000000 aleksis_core-3.1.2/PKG-INFO
+-rw-r--r--   0        0        0    38552 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/CHANGELOG.rst
+-rw-r--r--   0        0        0    14353 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/LICENCE.rst
+-rw-r--r--   0        0        0     3786 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/README.rst
+-rw-r--r--   0        0        0      194 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/__init__.py
+-rw-r--r--   0        0        0      464 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/__main__.py
+-rw-r--r--   0        0        0      510 2023-07-18 19:30:55.806599 aleksis_core-3.1.3/aleksis/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1068 2023-07-18 19:30:57.254654 aleksis_core-3.1.3/aleksis/core/__pycache__/__main__.cpython-311.pyc
+-rw-r--r--   0        0        0     2061 2023-07-18 19:31:01.578817 aleksis_core-3.1.3/aleksis/core/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0        0        0    11380 2023-07-18 19:30:58.842714 aleksis_core-3.1.3/aleksis/core/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0     2533 2023-07-18 19:30:55.866602 aleksis_core-3.1.3/aleksis/core/__pycache__/celery.cpython-311.pyc
+-rw-r--r--   0        0        0     3716 2023-07-18 19:31:01.686821 aleksis_core-3.1.3/aleksis/core/__pycache__/checks.cpython-311.pyc
+-rw-r--r--   0        0        0    17897 2023-07-18 19:31:01.106799 aleksis_core-3.1.3/aleksis/core/__pycache__/data_checks.cpython-311.pyc
+-rw-r--r--   0        0        0     5154 2023-07-18 19:31:01.698821 aleksis_core-3.1.3/aleksis/core/__pycache__/health_checks.cpython-311.pyc
+-rw-r--r--   0        0        0     8423 2023-07-18 19:31:01.150801 aleksis_core-3.1.3/aleksis/core/__pycache__/managers.cpython-311.pyc
+-rw-r--r--   0        0        0    31446 2023-07-18 19:31:01.114799 aleksis_core-3.1.3/aleksis/core/__pycache__/mixins.cpython-311.pyc
+-rw-r--r--   0        0        0    85606 2023-07-18 19:31:00.378772 aleksis_core-3.1.3/aleksis/core/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0    22237 2023-07-18 19:31:01.794825 aleksis_core-3.1.3/aleksis/core/__pycache__/preferences.cpython-311.pyc
+-rw-r--r--   0        0        0     1370 2023-07-18 19:30:58.866715 aleksis_core-3.1.3/aleksis/core/__pycache__/registries.cpython-311.pyc
+-rw-r--r--   0        0        0    16523 2023-07-18 19:31:01.610818 aleksis_core-3.1.3/aleksis/core/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0    44051 2023-07-18 19:30:57.282655 aleksis_core-3.1.3/aleksis/core/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0        0        0     3825 2023-07-18 19:31:01.162801 aleksis_core-3.1.3/aleksis/core/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0        0        0      950 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/admin.py
+-rw-r--r--   0        0        0     8519 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/apps.py
+-rw-r--r--   0        0        0     1338 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/celery.py
+-rw-r--r--   0        0        0     2751 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/checks.py
+-rw-r--r--   0        0        0    11534 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/data_checks.py
+-rw-r--r--   0        0        0      741 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/decorators.py
+-rw-r--r--   0        0        0     5556 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/filters.py
+-rw-r--r--   0        0        0    31619 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/forms.py
+-rw-r--r--   0        0        0     3175 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/app/apollo.js
+-rw-r--r--   0        0        0     1089 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/app/dateTimeFormats.js
+-rw-r--r--   0        0        0      197 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/app/i18n.js
+-rw-r--r--   0        0        0      157 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/app/router.js
+-rw-r--r--   0        0        0      133 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/app/sentry.js
+-rw-r--r--   0        0        0      793 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/app/vuetify.js
+-rw-r--r--   0        0        0     4485 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/LegacyBaseTemplate.vue
+-rw-r--r--   0        0        0      158 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/Parent.vue
+-rw-r--r--   0        0        0      335 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/about/About.vue
+-rw-r--r--   0        0        0     1971 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/about/AboutAleksis.vue
+-rw-r--r--   0        0        0     3831 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/about/InstalledAppCard.vue
+-rw-r--r--   0        0        0     1003 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/about/InstalledAppsList.vue
+-rw-r--r--   0        0        0      351 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/about/installedApps.graphql
+-rw-r--r--   0        0        0     2411 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/AccountMenu.vue
+-rw-r--r--   0        0        0     9590 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/App.vue
+-rw-r--r--   0        0        0      314 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/BrandLogo.vue
+-rw-r--r--   0        0        0     1064 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/ErrorPage.vue
+-rw-r--r--   0        0        0     1470 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/LanguageForm.vue
+-rw-r--r--   0        0        0     3778 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/SideNav.vue
+-rw-r--r--   0        0        0     1454 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/SidenavSearch.vue
+-rw-r--r--   0        0        0      747 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/SnackbarItem.vue
+-rw-r--r--   0        0        0     1932 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/Splash.vue
+-rw-r--r--   0        0        0      124 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/customMenu.graphql
+-rw-r--r--   0        0        0      205 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/dynamicRoutes.graphql
+-rw-r--r--   0        0        0       42 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/messages.graphql
+-rw-r--r--   0        0        0       59 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/ping.graphql
+-rw-r--r--   0        0        0      139 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/searchSnippets.graphql
+-rw-r--r--   0        0        0      412 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/systemProperties.graphql
+-rw-r--r--   0        0        0      322 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/whoAmI.graphql
+-rw-r--r--   0        0        0     2558 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue
+-rw-r--r--   0        0        0     1884 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue
+-rw-r--r--   0        0        0      220 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/authorized_oauth_applications/accessTokens.graphql
+-rw-r--r--   0        0        0       65 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/authorized_oauth_applications/revokeOauthToken.graphql
+-rw-r--r--   0        0        0     3482 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue
+-rw-r--r--   0        0        0     1910 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue
+-rw-r--r--   0        0        0      925 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/celery_progress/TaskListItem.vue
+-rw-r--r--   0        0        0      432 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/celery_progress/celeryProgress.graphql
+-rw-r--r--   0        0        0      191 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/celery_progress/celeryProgressBottom.graphql
+-rw-r--r--   0        0        0      118 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/celery_progress/celeryProgressFetched.graphql
+-rw-r--r--   0        0        0      655 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/generic/AvatarClickbox.vue
+-rw-r--r--   0        0        0      212 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/generic/BackButton.vue
+-rw-r--r--   0        0        0      598 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/generic/ButtonMenu.vue
+-rw-r--r--   0        0        0      981 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/generic/DetailView.vue
+-rw-r--r--   0        0        0      408 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/generic/ListView.vue
+-rw-r--r--   0        0        0      268 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/generic/MessageBox.vue
+-rw-r--r--   0        0        0     1914 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/generic/ObjectOverview.vue
+-rw-r--r--   0        0        0      269 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/generic/SmallContainer.vue
+-rw-r--r--   0        0        0     2017 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/generic/UpdateIndicator.vue
+-rw-r--r--   0        0        0     3232 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue
+-rw-r--r--   0        0        0      706 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/group/GroupCollection.vue
+-rw-r--r--   0        0        0     3034 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/notifications/NotificationItem.vue
+-rw-r--r--   0        0        0     2616 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/notifications/NotificationList.vue
+-rw-r--r--   0        0        0      107 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/notifications/markNotificationRead.graphql
+-rw-r--r--   0        0        0      200 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/notifications/myNotifications.graphql
+-rw-r--r--   0        0        0     1017 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/pdf/DownloadPDF.vue
+-rw-r--r--   0        0        0       78 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/pdf/pdf.graphql
+-rw-r--r--   0        0        0     1410 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/person/AdditionalImage.vue
+-rw-r--r--   0        0        0     1082 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/person/AvatarContent.vue
+-rw-r--r--   0        0        0     2892 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/person/PersonActions.vue
+-rw-r--r--   0        0        0      527 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue
+-rw-r--r--   0        0        0      759 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/person/PersonCollection.vue
+-rw-r--r--   0        0        0     7423 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/person/PersonOverview.vue
+-rw-r--r--   0        0        0      108 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/person/avatarContent.graphql
+-rw-r--r--   0        0        0      196 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/person/personActions.graphql
+-rw-r--r--   0        0        0      575 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/person/personOverview.graphql
+-rw-r--r--   0        0        0     3858 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/two_factor/TwoFactor.vue
+-rw-r--r--   0        0        0     1512 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue
+-rw-r--r--   0        0        0      589 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue
+-rw-r--r--   0        0        0      385 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/two_factor/twoFactor.graphql
+-rw-r--r--   0        0        0      390 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/css/global.scss
+-rw-r--r--   0        0        0     2561 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/index.js
+-rw-r--r--   0        0        0    10763 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/messages/de.json
+-rw-r--r--   0        0        0     9741 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/messages/en.json
+-rw-r--r--   0        0        0    12252 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/messages/ru.json
+-rw-r--r--   0        0        0    14534 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/messages/uk.json
+-rw-r--r--   0        0        0     1211 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/mixins/aleksis.js
+-rw-r--r--   0        0        0      538 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/mixins/error404.js
+-rw-r--r--   0        0        0     3441 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/mixins/menus.js
+-rw-r--r--   0        0        0     2256 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/mixins/offline.js
+-rw-r--r--   0        0        0      736 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/mixins/permissions.js
+-rw-r--r--   0        0        0     2154 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/mixins/routes.js
+-rw-r--r--   0        0        0     1619 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/mixins/useRegisterSW.js
+-rw-r--r--   0        0        0     6380 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/plugins/aleksis.js
+-rw-r--r--   0        0        0      450 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/routeValidators.js
+-rw-r--r--   0        0        0    36573 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/routes.js
+-rw-r--r--   0        0        0     2642 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/health_checks.py
+-rw-r--r--   0        0        0      487 2023-07-18 19:31:02.242842 aleksis_core-3.1.3/aleksis/core/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74307 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      463 2023-07-18 19:31:02.242842 aleksis_core-3.1.3/aleksis/core/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      894 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    63806 2023-07-18 19:31:02.266843 aleksis_core-3.1.3/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   126085 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      567 2023-07-18 19:31:02.242842 aleksis_core-3.1.3/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1118 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      942 2023-07-18 19:31:02.210841 aleksis_core-3.1.3/aleksis/core/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    77782 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-07-18 19:31:02.206840 aleksis_core-3.1.3/aleksis/core/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      810 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     2584 2023-07-18 19:31:02.210841 aleksis_core-3.1.3/aleksis/core/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    82875 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-18 19:31:02.194840 aleksis_core-3.1.3/aleksis/core/locale/la/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/la/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      361 2023-07-18 19:31:02.226841 aleksis_core-3.1.3/aleksis/core/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74237 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-18 19:31:02.230841 aleksis_core-3.1.3/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    80303 2023-07-18 19:31:02.218841 aleksis_core-3.1.3/aleksis/core/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   144575 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      713 2023-07-18 19:31:02.202840 aleksis_core-3.1.3/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1321 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      361 2023-07-18 19:31:02.246842 aleksis_core-3.1.3/aleksis/core/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74177 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-18 19:31:02.226841 aleksis_core-3.1.3/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    77610 2023-07-18 19:31:02.226841 aleksis_core-3.1.3/aleksis/core/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   131787 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      713 2023-07-18 19:31:02.214841 aleksis_core-3.1.3/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1331 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0        0 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/management/__init__.py
+-rw-r--r--   0        0        0     3957 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/management/commands/convert_urls_to_routes.py
+-rw-r--r--   0        0        0     1095 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/management/commands/vite.py
+-rw-r--r--   0        0        0      439 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/management/commands/webpack_bundle.py
+-rw-r--r--   0        0        0     4690 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/managers.py
+-rw-r--r--   0        0        0    51004 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2473 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0002_school_term.py
+-rw-r--r--   0        0        0      531 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0003_drop_image_cropping.py
+-rw-r--r--   0        0        0      796 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0004_add_permissions_for_group_stats.py
+-rw-r--r--   0        0        0     1252 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0005_timestamped_activity_notification.py
+-rw-r--r--   0        0        0     1567 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0006_dashboard_widget_size.py
+-rw-r--r--   0        0        0     1396 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0007_dashboard_widget_order.py
+-rw-r--r--   0        0        0     2311 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0008_data_check_result.py
+-rw-r--r--   0        0        0     1052 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0009_default_dashboard.py
+-rw-r--r--   0        0        0      952 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0010_external_link_widget.py
+-rw-r--r--   0        0        0      829 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0011_globalpermissions_options.py
+-rw-r--r--   0        0        0      501 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0012_valid_from_announcement.py
+-rw-r--r--   0        0        0     2270 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0013_pdf_file.py
+-rw-r--r--   0        0        0      533 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0014_alter_pdffile_file.py
+-rw-r--r--   0        0        0     1174 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0015_oauth_permissions.py
+-rw-r--r--   0        0        0     1538 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0016_taskuserassignment.py
+-rw-r--r--   0        0        0      426 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0017_dashboardwidget_broken.py
+-rw-r--r--   0        0        0      897 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0018_pdffile_html_file.py
+-rw-r--r--   0        0        0     2177 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0019_fix_uniqueness_per_site.py
+-rw-r--r--   0        0        0      542 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0020_pdf_file_person_optional.py
+-rw-r--r--   0        0        0     1084 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0021_drop_persons_accounts_perm.py
+-rw-r--r--   0        0        0      923 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0022_public_favicon.py
+-rw-r--r--   0        0        0     6340 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0023_oauth_application_model.py
+-rw-r--r--   0        0        0      714 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0024_oauth_grant_types_optional.py
+-rw-r--r--   0        0        0     1717 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0025_oauth_align_user_fk.py
+-rw-r--r--   0        0        0      582 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py
+-rw-r--r--   0        0        0      457 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0027_person_place_of_birth.py
+-rw-r--r--   0        0        0      947 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0028_char_field_not_null.py
+-rw-r--r--   0        0        0     1465 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0029_invitations.py
+-rw-r--r--   0        0        0     1776 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0030_user_attributes.py
+-rw-r--r--   0        0        0      526 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0031_oauthapplication_icon.py
+-rw-r--r--   0        0        0      340 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0032_remove_person_is_active.py
+-rw-r--r--   0        0        0     2416 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0033_update_photo_avatar.py
+-rw-r--r--   0        0        0      816 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0034_invite_permission.py
+-rw-r--r--   0        0        0     1781 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0035_preference_model_unique.py
+-rw-r--r--   0        0        0      626 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0036_additionalfields_helptext_required.py
+-rw-r--r--   0        0        0      917 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0037_add_static_content_widget.py
+-rw-r--r--   0        0        0      522 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0038_notification_send_at.py
+-rw-r--r--   0        0        0     1029 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0039_personal_ical_url.py
+-rw-r--r--   0        0        0      613 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py
+-rw-r--r--   0        0        0      516 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0041_update_gender_choices.py
+-rw-r--r--   0        0        0      547 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0042_pdffile_empty.py
+-rw-r--r--   0        0        0     2261 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0043_task_assignment_meta.py
+-rw-r--r--   0        0        0      532 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0044_task_assignment_result_fetched.py
+-rw-r--r--   0        0        0      486 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0045_data_check_result_fix_check_field.py
+-rw-r--r--   0        0        0   290966 2023-07-18 19:29:19.670983 aleksis_core-3.1.3/aleksis/core/migrations/0046_notification_create_field_icon.py
+-rw-r--r--   0        0        0     2717 2023-07-18 19:29:19.670983 aleksis_core-3.1.3/aleksis/core/migrations/0047_add_room_model.py
+-rw-r--r--   0        0        0   893996 2023-07-18 19:29:19.674983 aleksis_core-3.1.3/aleksis/core/migrations/0048_delete_personalicalurl.py
+-rw-r--r--   0        0        0      580 2023-07-18 19:29:19.674983 aleksis_core-3.1.3/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:29:19.674983 aleksis_core-3.1.3/aleksis/core/migrations/__init__.py
+-rw-r--r--   0        0        0    19769 2023-07-18 19:29:19.674983 aleksis_core-3.1.3/aleksis/core/mixins.py
+-rw-r--r--   0        0        0    51781 2023-07-18 19:29:19.674983 aleksis_core-3.1.3/aleksis/core/models.py
+-rw-r--r--   0        0        0    13478 2023-07-18 19:29:19.674983 aleksis_core-3.1.3/aleksis/core/preferences.py
+-rw-r--r--   0        0        0      692 2023-07-18 19:29:19.674983 aleksis_core-3.1.3/aleksis/core/registries.py
+-rw-r--r--   0        0        0    16018 2023-07-18 19:29:19.674983 aleksis_core-3.1.3/aleksis/core/rules.py
+-rw-r--r--   0        0        0     7486 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/__init__.py
+-rw-r--r--   0        0        0     1301 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/base.py
+-rw-r--r--   0        0        0     3049 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/celery_progress.py
+-rw-r--r--   0        0        0      585 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/custom_menu.py
+-rw-r--r--   0        0        0      459 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/dynamic_routes.py
+-rw-r--r--   0        0        0     2046 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/group.py
+-rw-r--r--   0        0        0     1743 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/installed_apps.py
+-rw-r--r--   0        0        0      265 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/message.py
+-rw-r--r--   0        0        0     1296 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/notification.py
+-rw-r--r--   0        0        0     1179 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/oauth.py
+-rw-r--r--   0        0        0      535 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/pdf.py
+-rw-r--r--   0        0        0      124 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/permissions.py
+-rw-r--r--   0        0        0     9708 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/person.py
+-rw-r--r--   0        0        0      191 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/room.py
+-rw-r--r--   0        0        0      163 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/school_term.py
+-rw-r--r--   0        0        0      868 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/search.py
+-rw-r--r--   0        0        0     1343 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/site_preferences.py
+-rw-r--r--   0        0        0     1651 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/system_properties.py
+-rw-r--r--   0        0        0     3297 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/two_factor.py
+-rw-r--r--   0        0        0      829 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/user.py
+-rw-r--r--   0        0        0      418 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/search_indexes.py
+-rw-r--r--   0        0        0    39943 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/settings.py
+-rw-r--r--   0        0        0    49621 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/static/img/aleksis-banner.svg
+-rw-r--r--   0        0        0     1862 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/static/img/aleksis-favicon.png
+-rw-r--r--   0        0        0    17172 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/static/img/aleksis-icon-maskable.png
+-rw-r--r--   0        0        0     7843 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/static/img/aleksis-icon-maskable.svg
+-rw-r--r--   0        0        0    31902 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/static/img/aleksis-icon.png
+-rw-r--r--   0        0        0     7346 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/img/aleksis-icon.svg
+-rw-r--r--   0        0        0    19126 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/img/fallback.png
+-rw-r--r--   0        0        0     2237 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/img/hero.svg
+-rw-r--r--   0        0        0      490 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/js/copy_button.js
+-rw-r--r--   0        0        0      521 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/js/edit_dashboard.js
+-rw-r--r--   0        0        0      618 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/js/helper.js
+-rw-r--r--   0        0        0      984 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/js/include_ajax_live.js
+-rw-r--r--   0        0        0     4350 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/js/main.js
+-rw-r--r--   0        0        0     1654 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/js/multi_select.js
+-rw-r--r--   0        0        0     3495 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/js/search.js
+-rw-r--r--   0        0        0     2578 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/js/serviceworker.js
+-rw-r--r--   0        0        0      271 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/print-simple.css
+-rw-r--r--   0        0        0     1627 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/print.css
+-rw-r--r--   0        0        0      187 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/print_landscape.css
+-rw-r--r--   0        0        0     1064 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/public/materialize-custom.scss
+-rw-r--r--   0        0        0    15745 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/public/style.scss
+-rw-r--r--   0        0        0    11345 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/public/theme.scss
+-rw-r--r--   0        0        0     6876 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/tables.py
+-rw-r--r--   0        0        0     2330 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/tasks.py
+-rw-r--r--   0        0        0      838 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/403.html
+-rw-r--r--   0        0        0      789 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/404.html
+-rw-r--r--   0        0        0      918 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/500.html
+-rw-r--r--   0        0        0       76 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/503.html
+-rw-r--r--   0        0        0      851 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/account_inactive.html
+-rw-r--r--   0        0        0      169 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/email/base_message.txt
+-rw-r--r--   0        0        0      525 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/email/email_confirmation_message.txt
+-rw-r--r--   0        0        0     1255 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/email_confirm.html
+-rw-r--r--   0        0        0      804 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/password_change.html
+-rw-r--r--   0        0        0      888 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/password_change_disabled.html
+-rw-r--r--   0        0        0     1376 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/password_reset.html
+-rw-r--r--   0        0        0      825 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/password_reset_done.html
+-rw-r--r--   0        0        0     2305 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/password_reset_from_key.html
+-rw-r--r--   0        0        0      649 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/password_reset_from_key_done.html
+-rw-r--r--   0        0        0      500 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/password_set.html
+-rw-r--r--   0        0        0      888 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/signup.html
+-rw-r--r--   0        0        0      838 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/signup_closed.html
+-rw-r--r--   0        0        0      820 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/verification_email_required.html
+-rw-r--r--   0        0        0     1160 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/verification_sent.html
+-rw-r--r--   0        0        0      979 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/components/chips.html
+-rw-r--r--   0        0        0      350 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/components/materialize-chips.html
+-rw-r--r--   0        0        0      225 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/components/msgbox.html
+-rw-r--r--   0        0        0      958 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/components/pagination.html
+-rw-r--r--   0        0        0      486 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/components/text_collapsible.html
+-rw-r--r--   0        0        0      483 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/core/additional_field/edit.html
+-rw-r--r--   0        0        0      594 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/core/additional_field/list.html
+-rw-r--r--   0        0        0     1053 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/core/announcement/form.html
+-rw-r--r--   0        0        0     1900 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/announcement/list.html
+-rw-r--r--   0        0        0     3099 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/base.html
+-rw-r--r--   0        0        0     2454 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/base_print.html
+-rw-r--r--   0        0        0     1212 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/base_simple_print.html
+-rw-r--r--   0        0        0      628 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/dashboard_widget/create.html
+-rw-r--r--   0        0        0      635 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html
+-rw-r--r--   0        0        0      626 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/dashboard_widget/edit.html
+-rw-r--r--   0        0        0      262 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/dashboard_widget/external_link_widget.html
+-rw-r--r--   0        0        0     1349 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/dashboard_widget/list.html
+-rw-r--r--   0        0        0      226 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/dashboard_widget/static_content_widget.html
+-rw-r--r--   0        0        0     3879 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/data_check/list.html
+-rw-r--r--   0        0        0     2233 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/edit_dashboard.html
+-rw-r--r--   0        0        0        0 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/empty.html
+-rw-r--r--   0        0        0     5310 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/group/child_groups.html
+-rw-r--r--   0        0        0      650 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/group/edit.html
+-rw-r--r--   0        0        0     3382 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/group/full.html
+-rw-r--r--   0        0        0     1019 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/group/list.html
+-rw-r--r--   0        0        0      465 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/group_type/edit.html
+-rw-r--r--   0        0        0      564 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/group_type/list.html
+-rw-r--r--   0        0        0     2504 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/index.html
+-rw-r--r--   0        0        0      777 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/pages/delete.html
+-rw-r--r--   0        0        0     6832 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/pages/system_status.html
+-rw-r--r--   0        0        0      603 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/pages/test_pdf.html
+-rw-r--r--   0        0        0       93 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/address.html
+-rw-r--r--   0        0        0      189 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/admins_list.html
+-rw-r--r--   0        0        0     1632 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/announcements.html
+-rw-r--r--   0        0        0     1472 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/avatar_content.html
+-rw-r--r--   0        0        0      319 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/copy_button.html
+-rw-r--r--   0        0        0     1089 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/crud_events.html
+-rw-r--r--   0        0        0      389 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/edit_dashboard_widget.html
+-rw-r--r--   0        0        0     1624 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/meta.html
+-rw-r--r--   0        0        0      414 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/on_page_menu.html
+-rw-r--r--   0        0        0      260 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/save_button.html
+-rw-r--r--   0        0        0     2374 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/splash_screen.html
+-rw-r--r--   0        0        0      325 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/turnable.html
+-rw-r--r--   0        0        0      915 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/perms/assign.html
+-rw-r--r--   0        0        0     2478 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/perms/list.html
+-rw-r--r--   0        0        0      376 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/person/collection.html
+-rw-r--r--   0        0        0      649 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/person/create.html
+-rw-r--r--   0        0        0      645 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/person/edit.html
+-rw-r--r--   0        0        0     1165 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/person/list.html
+-rw-r--r--   0        0        0      455 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/school_term/create.html
+-rw-r--r--   0        0        0      451 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/school_term/edit.html
+-rw-r--r--   0        0        0      556 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/school_term/list.html
+-rw-r--r--   0        0        0      935 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/vue_index.html
+-rw-r--r--   0        0        0     3921 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/django_tables2/materialize.html
+-rw-r--r--   0        0        0      981 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/dynamic_preferences/form.html
+-rw-r--r--   0        0        0      376 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/dynamic_preferences/sections.html
+-rw-r--r--   0        0        0      764 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/invitations/disabled.html
+-rw-r--r--   0        0        0     1281 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/invitations/enter.html
+-rw-r--r--   0        0        0     1162 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/invitations/forms/_invite.html
+-rw-r--r--   0        0        0      102 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/invitations/messages/invite_accepted.txt
+-rw-r--r--   0        0        0      171 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/material/field_errors.html
+-rw-r--r--   0        0        0     1232 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html
+-rw-r--r--   0        0        0     1897 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/material/fields/colorfield_colorwidget.html
+-rw-r--r--   0        0        0     1009 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html
+-rw-r--r--   0        0        0     1009 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/material/fields/django_select2_select2widget.html
+-rw-r--r--   0        0        0      253 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/material/non_field_errors.html
+-rw-r--r--   0        0        0      663 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/oauth2_provider/application/create.html
+-rw-r--r--   0        0        0     2335 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/oauth2_provider/application/detail.html
+-rw-r--r--   0        0        0      669 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/oauth2_provider/application/edit.html
+-rw-r--r--   0        0        0     1074 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/oauth2_provider/application/list.html
+-rw-r--r--   0        0        0     2686 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/oauth2_provider/authorize.html
+-rw-r--r--   0        0        0      887 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/offline.html
+-rw-r--r--   0        0        0       42 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/search/indexes/core/group_text.txt
+-rw-r--r--   0        0        0       69 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/search/indexes/core/person_text.txt
+-rw-r--r--   0        0        0       42 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/search/indexes/core/room_text.txt
+-rw-r--r--   0        0        0     3171 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/search/search.html
+-rw-r--r--   0        0        0      243 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/search/searchbar_snippet.html
+-rw-r--r--   0        0        0      150 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/search/searchbar_snippets.html
+-rw-r--r--   0        0        0      169 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/sms/notification.txt
+-rw-r--r--   0        0        0      893 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/socialaccount/authentication_error.html
+-rw-r--r--   0        0        0     1268 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/socialaccount/connections.html
+-rw-r--r--   0        0        0     1289 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/socialaccount/login.html
+-rw-r--r--   0        0        0      809 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/socialaccount/login_cancelled.html
+-rw-r--r--   0        0        0     1012 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/socialaccount/signup.html
+-rw-r--r--   0        0        0     1434 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/socialaccount/snippets/provider_list.html
+-rw-r--r--   0        0        0      630 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/templated_email/base.email
+-rw-r--r--   0        0        0     1527 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/templated_email/celery_failure.email
+-rw-r--r--   0        0        0      994 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/templated_email/data_checks.email
+-rw-r--r--   0        0        0      990 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/templated_email/email.css
+-rw-r--r--   0        0        0     1102 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/templated_email/invitation.email
+-rw-r--r--   0        0        0     1461 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/templated_email/notification.email
+-rw-r--r--   0        0        0      668 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/templated_email/person_changed.email
+-rw-r--r--   0        0        0      219 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/two_factor/_base_focus.html
+-rw-r--r--   0        0        0      877 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/two_factor/_wizard_actions.html
+-rw-r--r--   0        0        0      119 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/two_factor/_wizard_forms.html
+-rw-r--r--   0        0        0     1780 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/backup_tokens.html
+-rw-r--r--   0        0        0     6712 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/login.html
+-rw-r--r--   0        0        0      943 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/otp_required.html
+-rw-r--r--   0        0        0      986 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/phone_register.html
+-rw-r--r--   0        0        0     3312 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/setup.html
+-rw-r--r--   0        0        0     2127 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/setup_complete.html
+-rw-r--r--   0        0        0      786 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/two_factor/profile/disable.html
+-rw-r--r--   0        0        0        0 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templatetags/__init__.py
+-rw-r--r--   0        0        0       99 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templatetags/apps.py
+-rw-r--r--   0        0        0      394 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templatetags/dashboard.py
+-rw-r--r--   0        0        0     1618 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templatetags/data_helpers.py
+-rw-r--r--   0        0        0     1523 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templatetags/html_helpers.py
+-rw-r--r--   0        0        0      206 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templatetags/msg_box.py
+-rw-r--r--   0        0        0     3696 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/tests/browser/test_selenium.py
+-rw-r--r--   0        0        0     6596 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/tests/models/test.pdf
+-rw-r--r--   0        0        0     6562 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/tests/models/test_group.py
+-rw-r--r--   0        0        0     1520 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/tests/models/test_group_sync.py
+-rw-r--r--   0        0        0     3049 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/tests/models/test_notification.py
+-rw-r--r--   0        0        0     4003 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/tests/models/test_pdffile.py
+-rw-r--r--   0        0        0      427 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/tests/models/test_person.py
+-rw-r--r--   0        0        0     5503 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/tests/regression/test_regression.py
+-rw-r--r--   0        0        0      683 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/tests/regression/view_oauth.py
+-rw-r--r--   0        0        0     1021 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/tests/templatetags/test_data_helpers.py
+-rw-r--r--   0        0        0     2292 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/tests/views/test_account.py
+-rw-r--r--   0        0        0    18734 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/urls.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/__init__.py
+-rw-r--r--   0        0        0      176 2023-07-18 19:30:56.514626 aleksis_core-3.1.3/aleksis/core/util/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    14902 2023-07-18 19:30:58.866715 aleksis_core-3.1.3/aleksis/core/util/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0    10101 2023-07-18 19:31:01.162801 aleksis_core-3.1.3/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc
+-rw-r--r--   0        0        0    24932 2023-07-18 19:30:56.522626 aleksis_core-3.1.3/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     1500 2023-07-18 19:30:57.174651 aleksis_core-3.1.3/aleksis/core/util/__pycache__/email.cpython-311.pyc
+-rw-r--r--   0        0        0      771 2023-07-18 19:31:01.186802 aleksis_core-3.1.3/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     5712 2023-07-18 19:31:01.166801 aleksis_core-3.1.3/aleksis/core/util/__pycache__/notifications.cpython-311.pyc
+-rw-r--r--   0        0        0     9548 2023-07-18 19:31:01.610818 aleksis_core-3.1.3/aleksis/core/util/__pycache__/predicates.cpython-311.pyc
+-rw-r--r--   0        0        0     2181 2023-07-18 19:30:58.902716 aleksis_core-3.1.3/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0      664 2023-07-18 19:30:58.898716 aleksis_core-3.1.3/aleksis/core/util/__pycache__/spdx.cpython-311.pyc
+-rw-r--r--   0        0        0    10969 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/apps.py
+-rw-r--r--   0        0        0     5970 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/auth_helpers.py
+-rw-r--r--   0        0        0     7920 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/celery_progress.py
+-rw-r--r--   0        0        0      197 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/context_processors.py
+-rw-r--r--   0        0        0    16042 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/core_helpers.py
+-rw-r--r--   0        0        0      986 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/email.py
+-rw-r--r--   0        0        0     1175 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/forms.py
+-rw-r--r--   0        0        0     2901 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/frontend_helpers.py
+-rw-r--r--   0        0        0     2375 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/ldap.py
+-rw-r--r--   0        0        0   192829 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/licenses.json
+-rw-r--r--   0        0        0     2255 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/messages.py
+-rw-r--r--   0        0        0     2091 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/middlewares.py
+-rw-r--r--   0        0        0      850 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/model_helpers.py
+-rw-r--r--   0        0        0     3732 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/notifications.py
+-rw-r--r--   0        0        0     6131 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/pdf.py
+-rw-r--r--   0        0        0     5583 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/predicates.py
+-rw-r--r--   0        0        0      936 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/sass_helpers.py
+-rw-r--r--   0        0        0      524 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/aleksis/core/util/search.py
+-rw-r--r--   0        0        0      130 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/aleksis/core/util/spdx.py
+-rw-r--r--   0        0        0     1673 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/aleksis/core/util/tables.py
+-rw-r--r--   0        0        0    55996 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/aleksis/core/views.py
+-rw-r--r--   0        0        0    10257 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/aleksis/core/vite.config.js
+-rw-r--r--   0        0        0      173 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/aleksis/core/wsgi.py
+-rw-r--r--   0        0        0       45 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/conftest.py
+-rw-r--r--   0        0        0      581 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/docs/Makefile
+-rw-r--r--   0        0        0   127432 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/docs/_static/2fa.png
+-rw-r--r--   0        0        0    71362 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/docs/_static/accept_invite.png
+-rw-r--r--   0        0        0    72621 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/docs/_static/create_dashboard_widget.png
+-rw-r--r--   0        0        0    41935 2023-07-18 19:29:19.702984 aleksis_core-3.1.3/docs/_static/create_social_application.png
+-rw-r--r--   0        0        0    72508 2023-07-18 19:29:19.702984 aleksis_core-3.1.3/docs/_static/dashboard.png
+-rw-r--r--   0        0        0    87601 2023-07-18 19:29:19.702984 aleksis_core-3.1.3/docs/_static/dashboard_widgets.png
+-rw-r--r--   0        0        0   119523 2023-07-18 19:29:19.702984 aleksis_core-3.1.3/docs/_static/data_checks.png
+-rw-r--r--   0        0        0    81386 2023-07-18 19:29:19.702984 aleksis_core-3.1.3/docs/_static/edit_dashboard.png
+-rw-r--r--   0        0        0    85722 2023-07-18 19:29:19.706984 aleksis_core-3.1.3/docs/_static/edit_default_dashboard.png
+-rw-r--r--   0        0        0   107979 2023-07-18 19:29:19.706984 aleksis_core-3.1.3/docs/_static/invitations.png
+-rw-r--r--   0        0        0   177681 2023-07-18 19:29:19.706984 aleksis_core-3.1.3/docs/_static/invite_existing.png
+-rw-r--r--   0        0        0    44868 2023-07-18 19:29:19.706984 aleksis_core-3.1.3/docs/_static/pwa_desktop_chromium.png
+-rw-r--r--   0        0        0    69215 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/_static/pwa_mobile_chromium.png
+-rw-r--r--   0        0        0   128479 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/_static/pwa_mobile_firefox.png
+-rw-r--r--   0        0        0   108973 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/_static/pwa_mobile_safari.png
+-rw-r--r--   0        0        0    69804 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/_static/signup.png
+-rw-r--r--   0        0        0      132 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/00_index.rst
+-rw-r--r--   0        0        0     4231 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/01_core_concepts.rst
+-rw-r--r--   0        0        0     8067 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/10_install.rst
+-rw-r--r--   0        0        0     1872 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/15_config_files.rst
+-rw-r--r--   0        0        0     2086 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/16_config_options.rst
+-rw-r--r--   0        0        0     1648 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/17_storage.rst
+-rw-r--r--   0        0        0      803 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/18_mail.rst
+-rw-r--r--   0        0        0     1509 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/21_ldap.rst
+-rw-r--r--   0        0        0     3037 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/22_registration.rst
+-rw-r--r--   0        0        0     1467 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/23_socialaccounts.rst
+-rw-r--r--   0        0        0     3218 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/31_monitoring.rst
+-rw-r--r--   0        0        0     1012 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/32_tasks.rst
+-rw-r--r--   0        0        0     1393 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/33_data_checks.rst
+-rw-r--r--   0        0        0     4610 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/50_dashboard.rst
+-rw-r--r--   0        0        0     6393 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/conf.py
+-rw-r--r--   0        0        0      132 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/dev/00_index.rst
+-rw-r--r--   0        0        0     4058 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/dev/01_setup.rst
+-rw-r--r--   0        0        0     1427 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/dev/02_install_apps.rst
+-rw-r--r--   0        0        0     3117 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/dev/03_run_tests.rst
+-rw-r--r--   0        0        0     4519 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/dev/04_materialize_templates.rst
+-rw-r--r--   0        0        0      289 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/dev/05_extensible_models.rst
+-rw-r--r--   0        0        0     1148 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/dev/06_merging_app_settings.rst
+-rw-r--r--   0        0        0     1349 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/dev/10_dashboard_widgets.rst
+-rw-r--r--   0        0        0      514 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/index.rst
+-rw-r--r--   0        0        0      787 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/make.bat
+-rw-r--r--   0        0        0       95 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/00_index.rst
+-rw-r--r--   0        0        0       69 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/01_checks.rst
+-rw-r--r--   0        0        0       70 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/02_managers.rst
+-rw-r--r--   0        0        0       64 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/03_mixins.rst
+-rw-r--r--   0        0        0       84 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/04_models.rst
+-rw-r--r--   0        0        0      108 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/05_registries.rst
+-rw-r--r--   0        0        0       93 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/06_search_indexes.rst
+-rw-r--r--   0        0        0       79 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/07_tables.rst
+-rw-r--r--   0        0        0       90 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/08_tasks.rst
+-rw-r--r--   0        0        0     1017 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/09_utils.rst
+-rw-r--r--   0        0        0       71 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/10_views.rst
+-rw-r--r--   0        0        0       77 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/11_filters.rst
+-rw-r--r--   0        0        0      373 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/12_template_tags.rst
+-rw-r--r--   0        0        0      112 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/user/00_index.rst
+-rw-r--r--   0        0        0     1152 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/user/01_registration.rst
+-rw-r--r--   0        0        0     3465 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/user/02_personal_account.rst
+-rw-r--r--   0        0        0     1770 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/user/10_dashboard.rst
+-rw-r--r--   0        0        0     2607 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/user/20_pwa.rst
+-rw-r--r--   0        0        0     5409 2023-07-18 19:29:40.519767 aleksis_core-3.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2599 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/tox.ini
+-rw-r--r--   0        0        0     8657 1970-01-01 00:00:00.000000 aleksis_core-3.1.3/PKG-INFO
```

### Comparing `aleksis_core-3.1.2/CHANGELOG.rst` & `aleksis_core-3.1.3/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,25 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
+`3.1.3`_ – 2023-07-18
+---------------------
+
+Fixed
+~~~~~
+
+* [Docker] The build could silently continue even if frontend bundling failed, resulting
+  in an incomplete AlekSIS frontend app.
+* Rendering of "simple" PDF templates failed when used with S3 storage.
+* Log messages on some loggers did not contain log message
+
 `3.1.2`_ - 2023-07-05
 ---------------------
 
 Changed
 ~~~~~~~
 
 * uWSGI is now installed together with AlekSIS-Core per default.
@@ -1191,7 +1202,8 @@
 .. _3.0b1: https://edugit.org/AlekSIS/official/AlekSIS-Core/-/tags/3.0b1
 .. _3.0b2: https://edugit.org/AlekSIS/official/AlekSIS-Core/-/tags/3.0b2
 .. _3.0b3: https://edugit.org/AlekSIS/official/AlekSIS-Core/-/tags/3.0b3
 .. _3.0: https://edugit.org/AlekSIS/official/AlekSIS-Core/-/tags/3.0
 .. _3.1: https://edugit.org/AlekSIS/official/AlekSIS-Core/-/tags/3.1
 .. _3.1.1: https://edugit.org/AlekSIS/official/AlekSIS-Core/-/tags/3.1.1
 .. _3.1.2: https://edugit.org/AlekSIS/official/AlekSIS-Core/-/tags/3.1.2
+.. _3.1.3: https://edugit.org/AlekSIS/official/AlekSIS-Core/-/tags/3.1.3
```

### Comparing `aleksis_core-3.1.2/LICENCE.rst` & `aleksis_core-3.1.3/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/README.rst` & `aleksis_core-3.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/__pycache__/__main__.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/__pycache__/__main__.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 464
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/__pycache__/admin.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/__pycache__/admin.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 950
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/__pycache__/apps.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/__pycache__/apps.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 8519
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/__pycache__/celery.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/__pycache__/celery.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 1338
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/__pycache__/checks.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/__pycache__/checks.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 2751
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/__pycache__/data_checks.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/__pycache__/data_checks.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 11534
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/__pycache__/health_checks.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/__pycache__/health_checks.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 2642
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/__pycache__/managers.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/__pycache__/managers.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 4690
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/__pycache__/mixins.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/__pycache__/mixins.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 19769
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/__pycache__/models.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/__pycache__/models.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 51781
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 16
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/__pycache__/preferences.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/__pycache__/preferences.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 13478
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/__pycache__/registries.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/__pycache__/registries.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 692
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/__pycache__/rules.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/__pycache__/rules.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 16018
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/__pycache__/settings.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/__pycache__/settings.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
-files sz: 39939
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+files sz: 39943
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 18
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a0301
@@ -3113,15 +3113,15 @@
                 9808 BUILD_CONST_KEY_MAP      2
                 9810 LOAD_NAME              239 (LOGGING)
                 9812 EXTENDED_ARG             1
                 9814 LOAD_CONST             379 ('root')
                 9816 STORE_SUBSCR
    
     940         9820 EXTENDED_ARG             1
-                9822 LOAD_CONST             380 ('{asctime} {levelname} {name}[{process}]: {msg}')
+                9822 LOAD_CONST             380 ('{asctime} {levelname} {name}[{process}]: {message}')
    
     941         9824 EXTENDED_ARG             1
                 9826 LOAD_CONST             381 ('{')
    
     939         9828 EXTENDED_ARG             1
                 9830 LOAD_CONST             382 (('format', 'style'))
                 9832 BUILD_CONST_KEY_MAP      2
@@ -4715,15 +4715,15 @@
       ('href', 'title', 'style')
       ('font-family', 'font-weight', 'text-decoration', 'font-variant')
       'console'
       'logging.level'
       'WARNING'
       ('handlers', 'level')
       'root'
-      '{asctime} {levelname} {name}[{process}]: {msg}'
+      '{asctime} {levelname} {name}[{process}]: {message}'
       '{'
       ('format', 'style')
       'formatters'
       'verbose'
       'class'
       'logging.NullHandler'
       'handlers'
```

### Comparing `aleksis_core-3.1.2/aleksis/core/__pycache__/tasks.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/__pycache__/tasks.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 2330
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/admin.py` & `aleksis_core-3.1.3/aleksis/core/admin.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/apps.py` & `aleksis_core-3.1.3/aleksis/core/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/celery.py` & `aleksis_core-3.1.3/aleksis/core/celery.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/checks.py` & `aleksis_core-3.1.3/aleksis/core/checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/data_checks.py` & `aleksis_core-3.1.3/aleksis/core/data_checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/decorators.py` & `aleksis_core-3.1.3/aleksis/core/decorators.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/filters.py` & `aleksis_core-3.1.3/aleksis/core/filters.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/forms.py` & `aleksis_core-3.1.3/aleksis/core/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/app/apollo.js` & `aleksis_core-3.1.3/aleksis/core/frontend/app/apollo.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/app/dateTimeFormats.js` & `aleksis_core-3.1.3/aleksis/core/frontend/app/dateTimeFormats.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/app/vuetify.js` & `aleksis_core-3.1.3/aleksis/core/frontend/app/vuetify.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/LegacyBaseTemplate.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/LegacyBaseTemplate.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/about/AboutAleksis.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/about/AboutAleksis.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/about/InstalledAppCard.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/about/InstalledAppCard.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/about/InstalledAppsList.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/about/InstalledAppsList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/app/AccountMenu.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/app/AccountMenu.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/app/App.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/app/App.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/app/ErrorPage.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/app/ErrorPage.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/app/LanguageForm.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/app/LanguageForm.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/app/SideNav.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/app/SideNav.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/app/SidenavSearch.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/app/SidenavSearch.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/app/SnackbarItem.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/app/SnackbarItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/app/Splash.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/app/Splash.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/celery_progress/TaskListItem.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/celery_progress/TaskListItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/generic/AvatarClickbox.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/generic/AvatarClickbox.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/generic/ButtonMenu.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/generic/ButtonMenu.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/generic/DetailView.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/generic/DetailView.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/generic/ObjectOverview.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/generic/ObjectOverview.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/generic/UpdateIndicator.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/generic/UpdateIndicator.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/group/GroupCollection.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/group/GroupCollection.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/notifications/NotificationItem.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/notifications/NotificationItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/notifications/NotificationList.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/notifications/NotificationList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/pdf/DownloadPDF.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/pdf/DownloadPDF.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/person/AdditionalImage.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/person/AdditionalImage.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/person/AvatarContent.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/person/AvatarContent.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/person/PersonActions.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/person/PersonActions.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/person/PersonCollection.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/person/PersonCollection.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/person/PersonOverview.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/person/PersonOverview.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/person/personOverview.graphql` & `aleksis_core-3.1.3/aleksis/core/frontend/components/person/personOverview.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/two_factor/TwoFactor.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/two_factor/TwoFactor.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue` & `aleksis_core-3.1.3/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/index.js` & `aleksis_core-3.1.3/aleksis/core/frontend/index.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/messages/de.json` & `aleksis_core-3.1.3/aleksis/core/frontend/messages/de.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/messages/en.json` & `aleksis_core-3.1.3/aleksis/core/frontend/messages/en.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/messages/ru.json` & `aleksis_core-3.1.3/aleksis/core/frontend/messages/ru.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/messages/uk.json` & `aleksis_core-3.1.3/aleksis/core/frontend/messages/uk.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/mixins/aleksis.js` & `aleksis_core-3.1.3/aleksis/core/frontend/mixins/aleksis.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/mixins/error404.js` & `aleksis_core-3.1.3/aleksis/core/frontend/mixins/error404.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/mixins/menus.js` & `aleksis_core-3.1.3/aleksis/core/frontend/mixins/menus.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/mixins/offline.js` & `aleksis_core-3.1.3/aleksis/core/frontend/mixins/offline.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/mixins/permissions.js` & `aleksis_core-3.1.3/aleksis/core/frontend/mixins/permissions.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/mixins/routes.js` & `aleksis_core-3.1.3/aleksis/core/frontend/mixins/routes.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/mixins/useRegisterSW.js` & `aleksis_core-3.1.3/aleksis/core/frontend/mixins/useRegisterSW.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/plugins/aleksis.js` & `aleksis_core-3.1.3/aleksis/core/frontend/plugins/aleksis.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/frontend/routes.js` & `aleksis_core-3.1.3/aleksis/core/frontend/routes.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/health_checks.py` & `aleksis_core-3.1.3/aleksis/core/health_checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/ar/LC_MESSAGES/django.po` & `aleksis_core-3.1.3/aleksis/core/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.3/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_core-3.1.3/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_core-3.1.3/aleksis/core/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo` & `aleksis_core-3.1.3/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.3/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/fr/LC_MESSAGES/django.mo` & `aleksis_core-3.1.3/aleksis/core/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/fr/LC_MESSAGES/django.po` & `aleksis_core-3.1.3/aleksis/core/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.3/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/la/LC_MESSAGES/django.mo` & `aleksis_core-3.1.3/aleksis/core/locale/la/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/la/LC_MESSAGES/django.po` & `aleksis_core-3.1.3/aleksis/core/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/la/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.3/aleksis/core/locale/la/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_core-3.1.3/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.3/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/ru/LC_MESSAGES/django.mo` & `aleksis_core-3.1.3/aleksis/core/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/ru/LC_MESSAGES/django.po` & `aleksis_core-3.1.3/aleksis/core/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo` & `aleksis_core-3.1.3/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.3/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_core-3.1.3/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.3/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/uk/LC_MESSAGES/django.mo` & `aleksis_core-3.1.3/aleksis/core/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/uk/LC_MESSAGES/django.po` & `aleksis_core-3.1.3/aleksis/core/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo` & `aleksis_core-3.1.3/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.3/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/management/commands/convert_urls_to_routes.py` & `aleksis_core-3.1.3/aleksis/core/management/commands/convert_urls_to_routes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/management/commands/vite.py` & `aleksis_core-3.1.3/aleksis/core/management/commands/vite.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 
 from django.conf import settings
+from django.core.management.base import CommandError
 
 from django_yarnpkg.management.base import BaseYarnCommand
 from django_yarnpkg.yarn import yarn_adapter
 
 from ...util.frontend_helpers import run_vite, write_vite_values
 
 
@@ -22,8 +23,10 @@
         write_vite_values(os.path.join(settings.NODE_MODULES_ROOT, "django-vite-values.json"))
 
         # Install Node dependencies
         if not options["no_install"]:
             yarn_adapter.install(settings.YARN_INSTALLED_APPS)
 
         # Run Vite build
-        run_vite([options["command"]])
+        ret = run_vite([options["command"]])
+        if ret != 0:
+            raise CommandError("yarn command failed", returncode=ret)
```

### Comparing `aleksis_core-3.1.2/aleksis/core/managers.py` & `aleksis_core-3.1.3/aleksis/core/managers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0001_initial.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0002_school_term.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0002_school_term.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0003_drop_image_cropping.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0003_drop_image_cropping.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0004_add_permissions_for_group_stats.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0004_add_permissions_for_group_stats.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0005_timestamped_activity_notification.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0005_timestamped_activity_notification.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0006_dashboard_widget_size.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0006_dashboard_widget_size.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0007_dashboard_widget_order.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0007_dashboard_widget_order.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0008_data_check_result.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0008_data_check_result.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0009_default_dashboard.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0009_default_dashboard.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0010_external_link_widget.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0010_external_link_widget.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0011_globalpermissions_options.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0011_globalpermissions_options.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0013_pdf_file.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0013_pdf_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0014_alter_pdffile_file.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0014_alter_pdffile_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0015_oauth_permissions.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0015_oauth_permissions.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0016_taskuserassignment.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0016_taskuserassignment.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0018_pdffile_html_file.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0018_pdffile_html_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0019_fix_uniqueness_per_site.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0019_fix_uniqueness_per_site.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0020_pdf_file_person_optional.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0020_pdf_file_person_optional.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0021_drop_persons_accounts_perm.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0021_drop_persons_accounts_perm.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0022_public_favicon.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0022_public_favicon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0023_oauth_application_model.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0023_oauth_application_model.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0024_oauth_grant_types_optional.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0024_oauth_grant_types_optional.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0025_oauth_align_user_fk.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0025_oauth_align_user_fk.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0028_char_field_not_null.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0028_char_field_not_null.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0029_invitations.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0029_invitations.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0030_user_attributes.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0030_user_attributes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0031_oauthapplication_icon.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0031_oauthapplication_icon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0033_update_photo_avatar.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0033_update_photo_avatar.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0034_invite_permission.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0034_invite_permission.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0035_preference_model_unique.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0035_preference_model_unique.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0036_additionalfields_helptext_required.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0036_additionalfields_helptext_required.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0037_add_static_content_widget.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0037_add_static_content_widget.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0038_notification_send_at.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0038_notification_send_at.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0039_personal_ical_url.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0039_personal_ical_url.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0041_update_gender_choices.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0041_update_gender_choices.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0042_pdffile_empty.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0042_pdffile_empty.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0043_task_assignment_meta.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0043_task_assignment_meta.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0044_task_assignment_result_fetched.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0044_task_assignment_result_fetched.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0046_notification_create_field_icon.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0046_notification_create_field_icon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0047_add_room_model.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0047_add_room_model.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0048_delete_personalicalurl.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0048_delete_personalicalurl.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py` & `aleksis_core-3.1.3/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/mixins.py` & `aleksis_core-3.1.3/aleksis/core/mixins.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/models.py` & `aleksis_core-3.1.3/aleksis/core/models.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/preferences.py` & `aleksis_core-3.1.3/aleksis/core/preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/registries.py` & `aleksis_core-3.1.3/aleksis/core/registries.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/rules.py` & `aleksis_core-3.1.3/aleksis/core/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/schema/__init__.py` & `aleksis_core-3.1.3/aleksis/core/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/schema/base.py` & `aleksis_core-3.1.3/aleksis/core/schema/base.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/schema/celery_progress.py` & `aleksis_core-3.1.3/aleksis/core/schema/celery_progress.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/schema/custom_menu.py` & `aleksis_core-3.1.3/aleksis/core/schema/custom_menu.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/schema/group.py` & `aleksis_core-3.1.3/aleksis/core/schema/group.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/schema/installed_apps.py` & `aleksis_core-3.1.3/aleksis/core/schema/installed_apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/schema/notification.py` & `aleksis_core-3.1.3/aleksis/core/schema/notification.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/schema/oauth.py` & `aleksis_core-3.1.3/aleksis/core/schema/oauth.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/schema/pdf.py` & `aleksis_core-3.1.3/aleksis/core/schema/pdf.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/schema/person.py` & `aleksis_core-3.1.3/aleksis/core/schema/person.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/schema/search.py` & `aleksis_core-3.1.3/aleksis/core/schema/search.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/schema/site_preferences.py` & `aleksis_core-3.1.3/aleksis/core/schema/site_preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/schema/system_properties.py` & `aleksis_core-3.1.3/aleksis/core/schema/system_properties.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/schema/two_factor.py` & `aleksis_core-3.1.3/aleksis/core/schema/two_factor.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/schema/user.py` & `aleksis_core-3.1.3/aleksis/core/schema/user.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/settings.py` & `aleksis_core-3.1.3/aleksis/core/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -933,15 +933,15 @@
 # Set root logging level as default
 LOGGING["root"] = {
     "handlers": ["console"],
     "level": _settings.get("logging.level", "WARNING"),
 }
 # Configure global log Format
 LOGGING["formatters"]["verbose"] = {
-    "format": "{asctime} {levelname} {name}[{process}]: {msg}",
+    "format": "{asctime} {levelname} {name}[{process}]: {message}",
     "style": "{",
 }
 # Add null handler for selective silencing
 LOGGING["handlers"]["null"] = {"class": "logging.NullHandler"}
 # Make console logging independent of DEBUG
 LOGGING["handlers"]["console"]["filters"].remove("require_debug_true")
 # Use root log level for console
```

### Comparing `aleksis_core-3.1.2/aleksis/core/static/img/aleksis-banner.svg` & `aleksis_core-3.1.3/aleksis/core/static/img/aleksis-banner.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/static/img/aleksis-favicon.png` & `aleksis_core-3.1.3/aleksis/core/static/img/aleksis-favicon.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/static/img/aleksis-icon-maskable.png` & `aleksis_core-3.1.3/aleksis/core/static/img/aleksis-icon-maskable.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/static/img/aleksis-icon-maskable.svg` & `aleksis_core-3.1.3/aleksis/core/static/img/aleksis-icon-maskable.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/static/img/aleksis-icon.png` & `aleksis_core-3.1.3/aleksis/core/static/img/aleksis-icon.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/static/img/aleksis-icon.svg` & `aleksis_core-3.1.3/aleksis/core/static/img/aleksis-icon.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/static/img/fallback.png` & `aleksis_core-3.1.3/aleksis/core/static/img/fallback.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/static/img/hero.svg` & `aleksis_core-3.1.3/aleksis/core/static/img/hero.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/static/js/edit_dashboard.js` & `aleksis_core-3.1.3/aleksis/core/static/js/edit_dashboard.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/static/js/helper.js` & `aleksis_core-3.1.3/aleksis/core/static/js/helper.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/static/js/include_ajax_live.js` & `aleksis_core-3.1.3/aleksis/core/static/js/include_ajax_live.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/static/js/main.js` & `aleksis_core-3.1.3/aleksis/core/static/js/main.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/static/js/multi_select.js` & `aleksis_core-3.1.3/aleksis/core/static/js/multi_select.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/static/js/search.js` & `aleksis_core-3.1.3/aleksis/core/static/js/search.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/static/js/serviceworker.js` & `aleksis_core-3.1.3/aleksis/core/static/js/serviceworker.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/static/print.css` & `aleksis_core-3.1.3/aleksis/core/static/print.css`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/static/public/materialize-custom.scss` & `aleksis_core-3.1.3/aleksis/core/static/public/materialize-custom.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/static/public/style.scss` & `aleksis_core-3.1.3/aleksis/core/static/public/style.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/static/public/theme.scss` & `aleksis_core-3.1.3/aleksis/core/static/public/theme.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/tables.py` & `aleksis_core-3.1.3/aleksis/core/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/tasks.py` & `aleksis_core-3.1.3/aleksis/core/tasks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/403.html` & `aleksis_core-3.1.3/aleksis/core/templates/403.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/404.html` & `aleksis_core-3.1.3/aleksis/core/templates/404.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/500.html` & `aleksis_core-3.1.3/aleksis/core/templates/500.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/account/account_inactive.html` & `aleksis_core-3.1.3/aleksis/core/templates/account/account_inactive.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/account/email/email_confirmation_message.txt` & `aleksis_core-3.1.3/aleksis/core/templates/account/email/email_confirmation_message.txt`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/account/email_confirm.html` & `aleksis_core-3.1.3/aleksis/core/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/account/password_change.html` & `aleksis_core-3.1.3/aleksis/core/templates/account/password_change.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/account/password_change_disabled.html` & `aleksis_core-3.1.3/aleksis/core/templates/account/password_change_disabled.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/account/password_reset.html` & `aleksis_core-3.1.3/aleksis/core/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/account/password_reset_done.html` & `aleksis_core-3.1.3/aleksis/core/templates/account/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/account/password_reset_from_key.html` & `aleksis_core-3.1.3/aleksis/core/templates/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/account/password_reset_from_key_done.html` & `aleksis_core-3.1.3/aleksis/core/templates/account/password_reset_from_key_done.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/account/signup.html` & `aleksis_core-3.1.3/aleksis/core/templates/account/signup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/account/signup_closed.html` & `aleksis_core-3.1.3/aleksis/core/templates/account/signup_closed.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/account/verification_email_required.html` & `aleksis_core-3.1.3/aleksis/core/templates/account/verification_email_required.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/account/verification_sent.html` & `aleksis_core-3.1.3/aleksis/core/templates/account/verification_sent.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/components/chips.html` & `aleksis_core-3.1.3/aleksis/core/templates/components/chips.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/components/pagination.html` & `aleksis_core-3.1.3/aleksis/core/templates/components/pagination.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/additional_field/list.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/additional_field/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/announcement/form.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/announcement/form.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/announcement/list.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/announcement/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/base.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/base.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/base_print.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/base_print.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/base_simple_print.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/base_simple_print.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 {% load static i18n any_js sass_tags %}
 {% get_current_language as LANGUAGE_CODE %}
 
 <!DOCTYPE html>
 <html lang="{{ LANGUAGE_CODE }}">
 <head>
+  <base href="{{ BASE_URL }}" />
+
   {% include "core/partials/meta.html" %}
 
   <title>
     {% block no_browser_title %}
       {% block browser_title %}{% endblock %} —
     {% endblock %}
     {{ SITE_PREFERENCES.general__title }}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% load static i18n any_js sass_tags %} {% get_current_language as
 LANGUAGE_CODE %}
-{% include "core/partials/meta.html" %}
+ {% include "core/partials/meta.html" %}
 {% include_css "material-design-icons" %} {% include_css "Roboto100" %} {%
 include_css "Roboto300" %} {% include_css "Roboto400" %} {% include_css
 "Roboto500" %} {% include_css "Roboto700" %} {% include_css "Roboto900" %} {%
 include_css "paper-css" %}
 
 css" %}"/> {% block size %}
  {% endblock %} {% block extra_head %}{% endblock %}
```

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/dashboard_widget/create.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/dashboard_widget/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/dashboard_widget/edit.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/dashboard_widget/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/dashboard_widget/list.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/dashboard_widget/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/data_check/list.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/data_check/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/edit_dashboard.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/edit_dashboard.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/group/child_groups.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/group/child_groups.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/group/edit.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/group/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/group/full.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/group/full.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/group/list.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/group/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/group_type/list.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/group_type/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/index.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/index.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/pages/delete.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/pages/delete.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/pages/system_status.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/pages/system_status.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/pages/test_pdf.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/pages/test_pdf.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/partials/announcements.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/partials/announcements.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/partials/avatar_content.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/partials/avatar_content.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/partials/crud_events.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/partials/crud_events.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/partials/meta.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/partials/meta.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/partials/splash_screen.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/partials/splash_screen.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/perms/assign.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/perms/assign.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/perms/list.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/perms/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/person/create.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/person/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/person/edit.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/person/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/person/list.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/person/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/school_term/list.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/school_term/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/core/vue_index.html` & `aleksis_core-3.1.3/aleksis/core/templates/core/vue_index.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/django_tables2/materialize.html` & `aleksis_core-3.1.3/aleksis/core/templates/django_tables2/materialize.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/dynamic_preferences/form.html` & `aleksis_core-3.1.3/aleksis/core/templates/dynamic_preferences/form.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/invitations/disabled.html` & `aleksis_core-3.1.3/aleksis/core/templates/invitations/disabled.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/invitations/enter.html` & `aleksis_core-3.1.3/aleksis/core/templates/invitations/enter.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/invitations/forms/_invite.html` & `aleksis_core-3.1.3/aleksis/core/templates/invitations/forms/_invite.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html` & `aleksis_core-3.1.3/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/material/fields/colorfield_colorwidget.html` & `aleksis_core-3.1.3/aleksis/core/templates/material/fields/colorfield_colorwidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html` & `aleksis_core-3.1.3/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/material/fields/django_select2_select2widget.html` & `aleksis_core-3.1.3/aleksis/core/templates/material/fields/django_select2_select2widget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/oauth2_provider/application/create.html` & `aleksis_core-3.1.3/aleksis/core/templates/oauth2_provider/application/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/oauth2_provider/application/detail.html` & `aleksis_core-3.1.3/aleksis/core/templates/oauth2_provider/application/detail.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/oauth2_provider/application/edit.html` & `aleksis_core-3.1.3/aleksis/core/templates/oauth2_provider/application/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/oauth2_provider/application/list.html` & `aleksis_core-3.1.3/aleksis/core/templates/oauth2_provider/application/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/oauth2_provider/authorize.html` & `aleksis_core-3.1.3/aleksis/core/templates/oauth2_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/offline.html` & `aleksis_core-3.1.3/aleksis/core/templates/offline.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/search/search.html` & `aleksis_core-3.1.3/aleksis/core/templates/search/search.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/socialaccount/authentication_error.html` & `aleksis_core-3.1.3/aleksis/core/templates/socialaccount/authentication_error.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/socialaccount/connections.html` & `aleksis_core-3.1.3/aleksis/core/templates/socialaccount/connections.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/socialaccount/login.html` & `aleksis_core-3.1.3/aleksis/core/templates/socialaccount/login.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/socialaccount/login_cancelled.html` & `aleksis_core-3.1.3/aleksis/core/templates/socialaccount/login_cancelled.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/socialaccount/signup.html` & `aleksis_core-3.1.3/aleksis/core/templates/socialaccount/signup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/socialaccount/snippets/provider_list.html` & `aleksis_core-3.1.3/aleksis/core/templates/socialaccount/snippets/provider_list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/templated_email/base.email` & `aleksis_core-3.1.3/aleksis/core/templates/templated_email/base.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/templated_email/celery_failure.email` & `aleksis_core-3.1.3/aleksis/core/templates/templated_email/celery_failure.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/templated_email/data_checks.email` & `aleksis_core-3.1.3/aleksis/core/templates/templated_email/data_checks.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/templated_email/email.css` & `aleksis_core-3.1.3/aleksis/core/templates/templated_email/email.css`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/templated_email/invitation.email` & `aleksis_core-3.1.3/aleksis/core/templates/templated_email/invitation.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/templated_email/notification.email` & `aleksis_core-3.1.3/aleksis/core/templates/templated_email/notification.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/templated_email/person_changed.email` & `aleksis_core-3.1.3/aleksis/core/templates/templated_email/person_changed.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/two_factor/_wizard_actions.html` & `aleksis_core-3.1.3/aleksis/core/templates/two_factor/_wizard_actions.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/backup_tokens.html` & `aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/backup_tokens.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/login.html` & `aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/login.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/otp_required.html` & `aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/otp_required.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/phone_register.html` & `aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/phone_register.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/setup.html` & `aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/setup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/setup_complete.html` & `aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/setup_complete.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templates/two_factor/profile/disable.html` & `aleksis_core-3.1.3/aleksis/core/templates/two_factor/profile/disable.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templatetags/data_helpers.py` & `aleksis_core-3.1.3/aleksis/core/templatetags/data_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/templatetags/html_helpers.py` & `aleksis_core-3.1.3/aleksis/core/templatetags/html_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/tests/browser/test_selenium.py` & `aleksis_core-3.1.3/aleksis/core/tests/browser/test_selenium.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/tests/models/test.pdf` & `aleksis_core-3.1.3/aleksis/core/tests/models/test.pdf`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/tests/models/test_group.py` & `aleksis_core-3.1.3/aleksis/core/tests/models/test_group.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/tests/models/test_group_sync.py` & `aleksis_core-3.1.3/aleksis/core/tests/models/test_group_sync.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/tests/models/test_notification.py` & `aleksis_core-3.1.3/aleksis/core/tests/models/test_notification.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/tests/models/test_pdffile.py` & `aleksis_core-3.1.3/aleksis/core/tests/models/test_pdffile.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/tests/regression/test_regression.py` & `aleksis_core-3.1.3/aleksis/core/tests/regression/test_regression.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/tests/regression/view_oauth.py` & `aleksis_core-3.1.3/aleksis/core/tests/regression/view_oauth.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/tests/templatetags/test_data_helpers.py` & `aleksis_core-3.1.3/aleksis/core/tests/templatetags/test_data_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/tests/views/test_account.py` & `aleksis_core-3.1.3/aleksis/core/tests/views/test_account.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/urls.py` & `aleksis_core-3.1.3/aleksis/core/urls.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/util/__pycache__/apps.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/util/__pycache__/apps.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 10969
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 7920
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 26
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 16042
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 12
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/util/__pycache__/email.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/util/__pycache__/email.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 986
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc`

 * *Files 15% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 850
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/util/__pycache__/notifications.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/util/__pycache__/notifications.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 3732
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/util/__pycache__/predicates.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/util/__pycache__/predicates.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 5583
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 936
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/util/__pycache__/spdx.cpython-311.pyc` & `aleksis_core-3.1.3/aleksis/core/util/__pycache__/spdx.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
 files sz: 130
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.2/aleksis/core/util/apps.py` & `aleksis_core-3.1.3/aleksis/core/util/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/util/auth_helpers.py` & `aleksis_core-3.1.3/aleksis/core/util/auth_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/util/celery_progress.py` & `aleksis_core-3.1.3/aleksis/core/util/celery_progress.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/util/core_helpers.py` & `aleksis_core-3.1.3/aleksis/core/util/core_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/util/email.py` & `aleksis_core-3.1.3/aleksis/core/util/email.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/util/forms.py` & `aleksis_core-3.1.3/aleksis/core/util/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/util/frontend_helpers.py` & `aleksis_core-3.1.3/aleksis/core/util/frontend_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,30 +45,30 @@
     vite_values["cacheDir"] = settings.CACHE_DIR
     vite_values["node_modules"] = settings.JS_ROOT
 
     with open(out_path, "w") as out:
         json.dump(vite_values, out)
 
 
-def run_vite(args: Optional[Sequence[str]] = None) -> None:
+def run_vite(args: Optional[Sequence[str]] = None) -> int:
     args = list(args) if args else []
 
     config_path = os.path.join(settings.BASE_DIR, "aleksis", "core", "vite.config.js")
     shutil.copy(config_path, settings.NODE_MODULES_ROOT)
 
     mode = "development" if settings.DEBUG else "production"
     args += ["-m", mode]
 
     log_level = settings.LOGGING["root"]["level"]
     if settings.DEBUG or log_level == "DEBUG":
         args.append("-d")
     log_level = {"INFO": "info", "WARNING": "warn", "ERROR": "error"}.get(log_level, "silent")
     args += ["-l", log_level]
 
-    yarn_adapter.call_yarn(["run", "vite"] + args)
+    return yarn_adapter.call_yarn(["run", "vite"] + args)
 
 
 def get_language_cookie(code: str) -> str:
     """Build a cookie string to set a new language."""
     cookie_parts = [f"{settings.LANGUAGE_COOKIE_NAME}={code}"]
     args = dict(
         max_age=settings.LANGUAGE_COOKIE_AGE,
```

### Comparing `aleksis_core-3.1.2/aleksis/core/util/ldap.py` & `aleksis_core-3.1.3/aleksis/core/util/ldap.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/util/licenses.json` & `aleksis_core-3.1.3/aleksis/core/util/licenses.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/util/messages.py` & `aleksis_core-3.1.3/aleksis/core/util/messages.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/util/middlewares.py` & `aleksis_core-3.1.3/aleksis/core/util/middlewares.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/util/model_helpers.py` & `aleksis_core-3.1.3/aleksis/core/util/model_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/util/notifications.py` & `aleksis_core-3.1.3/aleksis/core/util/notifications.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/util/pdf.py` & `aleksis_core-3.1.3/aleksis/core/util/pdf.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/util/predicates.py` & `aleksis_core-3.1.3/aleksis/core/util/predicates.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/util/sass_helpers.py` & `aleksis_core-3.1.3/aleksis/core/util/sass_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/util/search.py` & `aleksis_core-3.1.3/aleksis/core/util/search.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/util/tables.py` & `aleksis_core-3.1.3/aleksis/core/util/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/views.py` & `aleksis_core-3.1.3/aleksis/core/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/aleksis/core/vite.config.js` & `aleksis_core-3.1.3/aleksis/core/vite.config.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/Makefile` & `aleksis_core-3.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/_static/2fa.png` & `aleksis_core-3.1.3/docs/_static/2fa.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/_static/accept_invite.png` & `aleksis_core-3.1.3/docs/_static/accept_invite.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/_static/create_dashboard_widget.png` & `aleksis_core-3.1.3/docs/_static/create_dashboard_widget.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/_static/create_social_application.png` & `aleksis_core-3.1.3/docs/_static/create_social_application.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/_static/dashboard.png` & `aleksis_core-3.1.3/docs/_static/dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/_static/dashboard_widgets.png` & `aleksis_core-3.1.3/docs/_static/dashboard_widgets.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/_static/data_checks.png` & `aleksis_core-3.1.3/docs/_static/data_checks.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/_static/edit_dashboard.png` & `aleksis_core-3.1.3/docs/_static/edit_dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/_static/edit_default_dashboard.png` & `aleksis_core-3.1.3/docs/_static/edit_default_dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/_static/invitations.png` & `aleksis_core-3.1.3/docs/_static/invitations.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/_static/invite_existing.png` & `aleksis_core-3.1.3/docs/_static/invite_existing.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/_static/pwa_desktop_chromium.png` & `aleksis_core-3.1.3/docs/_static/pwa_desktop_chromium.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/_static/pwa_mobile_chromium.png` & `aleksis_core-3.1.3/docs/_static/pwa_mobile_chromium.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/_static/pwa_mobile_firefox.png` & `aleksis_core-3.1.3/docs/_static/pwa_mobile_firefox.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/_static/pwa_mobile_safari.png` & `aleksis_core-3.1.3/docs/_static/pwa_mobile_safari.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/_static/signup.png` & `aleksis_core-3.1.3/docs/_static/signup.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/admin/01_core_concepts.rst` & `aleksis_core-3.1.3/docs/admin/01_core_concepts.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/admin/10_install.rst` & `aleksis_core-3.1.3/docs/admin/10_install.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/admin/15_config_files.rst` & `aleksis_core-3.1.3/docs/admin/15_config_files.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/admin/16_config_options.rst` & `aleksis_core-3.1.3/docs/admin/16_config_options.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/admin/17_storage.rst` & `aleksis_core-3.1.3/docs/admin/17_storage.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/admin/18_mail.rst` & `aleksis_core-3.1.3/docs/admin/18_mail.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/admin/21_ldap.rst` & `aleksis_core-3.1.3/docs/admin/21_ldap.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/admin/22_registration.rst` & `aleksis_core-3.1.3/docs/admin/22_registration.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/admin/23_socialaccounts.rst` & `aleksis_core-3.1.3/docs/admin/23_socialaccounts.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/admin/31_monitoring.rst` & `aleksis_core-3.1.3/docs/admin/31_monitoring.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/admin/32_tasks.rst` & `aleksis_core-3.1.3/docs/admin/32_tasks.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/admin/33_data_checks.rst` & `aleksis_core-3.1.3/docs/admin/33_data_checks.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/admin/50_dashboard.rst` & `aleksis_core-3.1.3/docs/admin/50_dashboard.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/conf.py` & `aleksis_core-3.1.3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 project = "AlekSIS-Core"
 copyright = "2019-2023 The AlekSIS team"
 author = "The AlekSIS Team"
 
 # The short X.Y version
 version = "3.1"
 # The full version, including alpha/beta/rc tags
-release = "3.1.2"
+release = "3.1.3"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `aleksis_core-3.1.2/docs/dev/01_setup.rst` & `aleksis_core-3.1.3/docs/dev/01_setup.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/dev/02_install_apps.rst` & `aleksis_core-3.1.3/docs/dev/02_install_apps.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/dev/03_run_tests.rst` & `aleksis_core-3.1.3/docs/dev/03_run_tests.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/dev/04_materialize_templates.rst` & `aleksis_core-3.1.3/docs/dev/04_materialize_templates.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/dev/06_merging_app_settings.rst` & `aleksis_core-3.1.3/docs/dev/06_merging_app_settings.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/dev/10_dashboard_widgets.rst` & `aleksis_core-3.1.3/docs/dev/10_dashboard_widgets.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/index.rst` & `aleksis_core-3.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/make.bat` & `aleksis_core-3.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/ref/core/09_utils.rst` & `aleksis_core-3.1.3/docs/ref/core/09_utils.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/user/01_registration.rst` & `aleksis_core-3.1.3/docs/user/01_registration.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/user/02_personal_account.rst` & `aleksis_core-3.1.3/docs/user/02_personal_account.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/user/10_dashboard.rst` & `aleksis_core-3.1.3/docs/user/10_dashboard.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/docs/user/20_pwa.rst` & `aleksis_core-3.1.3/docs/user/20_pwa.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/pyproject.toml` & `aleksis_core-3.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-Core"
-version = "3.1.2"
+version = "3.1.3"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
@@ -123,14 +123,15 @@
 django-cte = "^1.1.5"
 pycountry = "^22.0.0"
 django-iconify = "^0.3"
 customidenticon = "^0.1.5"
 graphene-django = "^3.0.0"
 selenium = "^4.4.3"
 django-vite = "^2.0.2"
+graphene-django-cud = "^0.11.0"
 uwsgi = "^2.0.21"
 
 [tool.poetry.extras]
 ldap = ["django-auth-ldap"]
 s3 = ["boto3", "django-storages"]
 sentry = ["sentry-sdk"]
```

### Comparing `aleksis_core-3.1.2/tox.ini` & `aleksis_core-3.1.3/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.2/PKG-INFO` & `aleksis_core-3.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis-core
-Version: 3.1.2
+Version: 3.1.3
 Summary: AlekSIS (School Information System) — Core
 Home-page: https://aleksis.org
 License: EUPL-1.2-or-later
 Keywords: SIS,education,school,digitisation,school apps
 Author: Dominik George
 Author-email: dominik.george@teckids.org
 Maintainer: Jonathan Weth
@@ -82,14 +82,15 @@
 Requires-Dist: django-vite (>=2.0.2,<3.0.0)
 Requires-Dist: django-yarnpkg (>=6.0,<7.0)
 Requires-Dist: django_select2 (>=8.0,<9.0)
 Requires-Dist: django_widget_tweaks (>=1.4.5,<2.0.0)
 Requires-Dist: djangorestframework (>=3.12.4,<4.0.0)
 Requires-Dist: dynaconf[ini,toml,yaml] (>=3.1,<4.0)
 Requires-Dist: graphene-django (>=3.0.0,<4.0.0)
+Requires-Dist: graphene-django-cud (>=0.11.0,<0.12.0)
 Requires-Dist: haystack-redis (>=0.0.1,<0.0.2)
 Requires-Dist: html2text (>=2020.0.0,<2021.0.0)
 Requires-Dist: ipython (>=8.0.0,<9.0.0)
 Requires-Dist: libsass (>=0.22.0,<0.23.0)
 Requires-Dist: license-expression (>=30.0,<31.0)
 Requires-Dist: psutil (>=5.7.0,<6.0.0)
 Requires-Dist: psycopg2 (>=2.8,<3.0)
```

