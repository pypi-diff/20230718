# Comparing `tmp/NEMO-4.5.5.tar.gz` & `tmp/NEMO-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NEMO-4.5.5.tar", last modified: Tue May 16 14:04:38 2023, max compression
+gzip compressed data, was "NEMO-4.6.0.tar", last modified: Tue Jul 18 17:03:24 2023, max compression
```

## Comparing `NEMO-4.5.5.tar` & `NEMO-4.6.0.tar`

### file list

```diff
@@ -1,482 +1,512 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.621849 NEMO-4.5.5/
--rw-rw-rw-   0 root         (0) root         (0)     1865 2023-05-16 14:04:26.000000 NEMO-4.5.5/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-05-16 14:04:26.000000 NEMO-4.5.5/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.557849 NEMO-4.5.5/NEMO/
--rw-rw-rw-   0 root         (0) root         (0)     1254 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4594 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/actions.py
--rw-rw-rw-   0 root         (0) root         (0)    48729 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.558849 NEMO-4.5.5/NEMO/apps/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.559849 NEMO-4.5.5/NEMO/apps/area_access/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.545849 NEMO-4.5.5/NEMO/apps/area_access/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.559849 NEMO-4.5.5/NEMO/apps/area_access/static/area_access/
--rw-rw-rw-   0 root         (0) root         (0)      304 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/static/area_access/area_access.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.545849 NEMO-4.5.5/NEMO/apps/area_access/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.561849 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/
--rw-rw-rw-   0 root         (0) root         (0)     1531 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/already_logged_in.html
--rw-rw-rw-   0 root         (0) root         (0)      349 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/badge_not_found.html
--rw-rw-rw-   0 root         (0) root         (0)     9006 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/base.html
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/choose_project.html
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/door_is_open.html
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/farewell_screen.html
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/inactive.html
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/login_success.html
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/logout_success.html
--rw-rw-rw-   0 root         (0) root         (0)      666 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/logout_warning.html
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/no_active_projects.html
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/not_logged_in.html
--rw-rw-rw-   0 root         (0) root         (0)      210 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/physical_access_denied.html
--rw-rw-rw-   0 root         (0) root         (0)      566 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/resource_unavailable.html
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/welcome_screen.html
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    12271 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.561849 NEMO-4.5.5/NEMO/apps/kiosk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.545849 NEMO-4.5.5/NEMO/apps/kiosk/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.562849 NEMO-4.5.5/NEMO/apps/kiosk/static/kiosk/
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/static/kiosk/kiosk.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.546849 NEMO-4.5.5/NEMO/apps/kiosk/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.564849 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/acknowledgement.html
--rw-rw-rw-   0 root         (0) root         (0)     2125 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/category_choices.html
--rw-rw-rw-   0 root         (0) root         (0)     2012 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/choices.html
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/error.html
--rw-rw-rw-   0 root         (0) root         (0)     2923 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)    12510 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/kiosk.html
--rw-rw-rw-   0 root         (0) root         (0)      901 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/success.html
--rw-rw-rw-   0 root         (0) root         (0)    16575 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/tool_information.html
--rw-rw-rw-   0 root         (0) root         (0)     1108 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html
--rw-rw-rw-   0 root         (0) root         (0)     4472 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    13059 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.565849 NEMO-4.5.5/NEMO/apps/sensors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7165 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/customizations.py
--rw-rw-rw-   0 root         (0) root         (0)     5237 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/evaluators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.565849 NEMO-4.5.5/NEMO/apps/sensors/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.565849 NEMO-4.5.5/NEMO/apps/sensors/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/management/commands/manage_sensor_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.566849 NEMO-4.5.5/NEMO/apps/sensors/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     7794 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12955 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/models.py
--rw-rw-rw-   0 root         (0) root         (0)     4564 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/sensors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.546849 NEMO-4.5.5/NEMO/apps/sensors/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.567849 NEMO-4.5.5/NEMO/apps/sensors/static/sensors/
--rw-rw-rw-   0 root         (0) root         (0)   408236 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/static/sensors/chart.js
--rw-rw-rw-   0 root         (0) root         (0)   195090 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/static/sensors/chart.min.js
--rw-rw-rw-   0 root         (0) root         (0)     1376 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js
--rw-rw-rw-   0 root         (0) root         (0)     7659 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/static/sensors/daterangepicker.css
--rw-rw-rw-   0 root         (0) root         (0)    66305 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/static/sensors/daterangepicker.js
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/static/sensors/sensors.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.546849 NEMO-4.5.5/NEMO/apps/sensors/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.567849 NEMO-4.5.5/NEMO/apps/sensors/templates/customizations/
--rw-rw-rw-   0 root         (0) root         (0)     3701 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/templates/customizations/customizations_sensors.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.568849 NEMO-4.5.5/NEMO/apps/sensors/templates/sensors/
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/templates/sensors/sensor_alerts.html
--rw-rw-rw-   0 root         (0) root         (0)    15165 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/templates/sensors/sensor_data.html
--rw-rw-rw-   0 root         (0) root         (0)     2615 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/templates/sensors/sensors.html
--rw-rw-rw-   0 root         (0) root         (0)      790 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     5069 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/views.py
--rw-rw-rw-   0 root         (0) root         (0)     3966 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/context_processors.py
--rw-rw-rw-   0 root         (0) root         (0)     5778 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3833 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/fields.py
--rw-rw-rw-   0 root         (0) root         (0)    12935 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/forms.py
--rw-rw-rw-   0 root         (0) root         (0)    17784 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/interlocks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.568849 NEMO-4.5.5/NEMO/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.570849 NEMO-4.5.5/NEMO/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/cancel_unused_reservations.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/create_closure_alerts.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/manage_recurring_charges.py
--rw-rw-rw-   0 root         (0) root         (0)      431 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/manage_tool_qualifications.py
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/send_email_out_of_time_reservation_notification.py
--rw-rw-rw-   0 root         (0) root         (0)      415 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/send_email_reservation_ending_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/send_email_reservation_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/send_email_usage_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      456 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/send_email_user_access_expiration_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/send_email_weekend_access_notification.py
--rw-rw-rw-   0 root         (0) root         (0)     5578 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.575849 NEMO-4.5.5/NEMO/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    50307 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0001_version_1_0_0.py
--rw-rw-rw-   0 root         (0) root         (0)    32962 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0002_version_1_0_0_squashed.py
--rw-rw-rw-   0 root         (0) root         (0)     7988 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0012_version_2_0_0_squashed.py
--rw-rw-rw-   0 root         (0) root         (0)     9904 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0020_version_3_0_0.py
--rw-rw-rw-   0 root         (0) root         (0)     1712 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0021_version_3_1_0.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0022_version_3_3_0.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0023_badgereader.py
--rw-rw-rw-   0 root         (0) root         (0)      705 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0024_contactinformation_user.py
--rw-rw-rw-   0 root         (0) root         (0)     2674 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0025_version_3_6_0.py
--rw-rw-rw-   0 root         (0) root         (0)     5405 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0026_version_3_7_0.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0027_version_3_8_0.py
--rw-rw-rw-   0 root         (0) root         (0)     2233 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0028_version_3_9_0.py
--rw-rw-rw-   0 root         (0) root         (0)     1127 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0030_version_3_9_2.py
--rw-rw-rw-   0 root         (0) root         (0)     2785 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0031_version_3_10_0.py
--rw-rw-rw-   0 root         (0) root         (0)     3166 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0032_version_3_11_0.py
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0033_version_3_12_0.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0034_version_3_13_0.py
--rw-rw-rw-   0 root         (0) root         (0)     6747 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0035_version_3_14_0.py
--rw-rw-rw-   0 root         (0) root         (0)     7792 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0036_version_3_15_0.py
--rw-rw-rw-   0 root         (0) root         (0)     3717 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0037_version_3_16_0.py
--rw-rw-rw-   0 root         (0) root         (0)      935 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0038_version_4_0_0.py
--rw-rw-rw-   0 root         (0) root         (0)     3601 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0039_version_4_1_0.py
--rw-rw-rw-   0 root         (0) root         (0)     2444 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0040_version_4_2_0.py
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0041_version_4_2_1.py
--rw-rw-rw-   0 root         (0) root         (0)    16454 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0042_version_4_3_0.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0043_version_4_3_2.py
--rw-rw-rw-   0 root         (0) root         (0)     5420 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0044_version_4_4_0.py
--rw-rw-rw-   0 root         (0) root         (0)    13447 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0045_version_4_5_0.py
--rw-rw-rw-   0 root         (0) root         (0)     2037 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0045_version_4_5_5.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2269 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5874 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     3855 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/model_tree.py
--rw-rw-rw-   0 root         (0) root         (0)   152793 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1429 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)    49395 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/policy.py
--rw-rw-rw-   0 root         (0) root         (0)     9943 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/provisioning.py
--rw-rw-rw-   0 root         (0) root         (0)     5646 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/rates.py
--rw-rw-rw-   0 root         (0) root         (0)     1037 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/rest_filter_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     9391 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/serializers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.579849 NEMO-4.5.5/NEMO/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.579849 NEMO-4.5.5/NEMO/static/admin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.579849 NEMO-4.5.5/NEMO/static/admin/physical_access_level/
--rw-rw-rw-   0 root         (0) root         (0)      607 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/admin/physical_access_level/access_level.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.580849 NEMO-4.5.5/NEMO/static/admin/questions_preview/
--rw-rw-rw-   0 root         (0) root         (0)     4122 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/admin/questions_preview/questions_preview.css
--rw-rw-rw-   0 root         (0) root         (0)     1372 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/admin/questions_preview/questions_preview.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.580849 NEMO-4.5.5/NEMO/static/admin/reservation_questions/
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/admin/reservation_questions/reservation_questions.js
--rw-rw-rw-   0 root         (0) root         (0)     1225 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/admin/time_options_override.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.580849 NEMO-4.5.5/NEMO/static/admin/tool/
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/admin/tool/tool.js
--rw-rw-rw-   0 root         (0) root         (0)     1278 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/badge_reader.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.548849 NEMO-4.5.5/NEMO/static/bootstrap/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.582849 NEMO-4.5.5/NEMO/static/bootstrap/css/
--rw-rw-rw-   0 root         (0) root         (0)    22608 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap-theme.css
--rw-rw-rw-   0 root         (0) root         (0)    43339 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap-theme.css.map
--rw-rw-rw-   0 root         (0) root         (0)    19963 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap-theme.min.css
--rw-rw-rw-   0 root         (0) root         (0)   141622 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap.css
--rw-rw-rw-   0 root         (0) root         (0)   380986 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap.css.map
--rw-rw-rw-   0 root         (0) root         (0)   117305 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.583849 NEMO-4.5.5/NEMO/static/bootstrap/fonts/
--rw-rw-rw-   0 root         (0) root         (0)    20127 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0 root         (0) root         (0)   108738 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0 root         (0) root         (0)    45404 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)    23424 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-rw-rw-   0 root         (0) root         (0)    18028 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.583849 NEMO-4.5.5/NEMO/static/bootstrap/js/
--rw-rw-rw-   0 root         (0) root         (0)    67546 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/js/bootstrap.js
--rw-rw-rw-   0 root         (0) root         (0)    35951 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.583849 NEMO-4.5.5/NEMO/static/datetimepicker/
--rw-rw-rw-   0 root         (0) root         (0)     9020 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/datetimepicker/bootstrap-datetimepicker.css
--rw-rw-rw-   0 root         (0) root         (0)   105978 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/datetimepicker/bootstrap-datetimepicker.js
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.585849 NEMO-4.5.5/NEMO/static/fullcalendar/
--rw-rw-rw-   0 root         (0) root         (0)    28531 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/fullcalendar/fullcalendar.css
--rw-rw-rw-   0 root         (0) root         (0)   357749 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/fullcalendar/fullcalendar.js
--rw-rw-rw-   0 root         (0) root         (0)    13687 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/fullcalendar/fullcalendar.min.css
--rw-rw-rw-   0 root         (0) root         (0)   168700 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/fullcalendar/fullcalendar.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.585849 NEMO-4.5.5/NEMO/static/icons/
--rw-rw-rw-   0 root         (0) root         (0)    24065 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/icons/agreement.png
--rw-rw-rw-   0 root         (0) root         (0)    16685 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/icons/caution.png
--rw-rw-rw-   0 root         (0) root         (0)     4664 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/icons/preferences.png
--rw-rw-rw-   0 root         (0) root         (0)   247387 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/jquery.js
--rw-rw-rw-   0 root         (0) root         (0)    84320 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/jquery.min.js
--rw-rw-rw-   0 root         (0) root         (0)  1183392 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/jumbotron_watermark.bmp
--rw-rw-rw-   0 root         (0) root         (0)     1017 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/mobile.js
--rw-rw-rw-   0 root         (0) root         (0)   174603 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/moment.js
--rw-rw-rw-   0 root         (0) root         (0)    58102 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/moment.min.js
--rw-rw-rw-   0 root         (0) root         (0)    86041 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/moment.min.js.map
--rw-rw-rw-   0 root         (0) root         (0)    15594 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/nemo.css
--rw-rw-rw-   0 root         (0) root         (0)    20182 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/nemo.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.586849 NEMO-4.5.5/NEMO/static/numpad/
--rw-rw-rw-   0 root         (0) root         (0)    12285 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/numpad/custom_numpad.jquery.js
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/numpad/numpad.jquery.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.587849 NEMO-4.5.5/NEMO/static/pickadate/
--rw-rw-rw-   0 root         (0) root         (0)     3795 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/pickadate/default.css
--rw-rw-rw-   0 root         (0) root         (0)     6040 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/pickadate/default.date.css
--rw-rw-rw-   0 root         (0) root         (0)     2785 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/pickadate/default.time.css
--rw-rw-rw-   0 root         (0) root         (0)    48215 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/pickadate/picker.date.js
--rw-rw-rw-   0 root         (0) root         (0)    36941 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/pickadate/picker.js
--rw-rw-rw-   0 root         (0) root         (0)    31899 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/pickadate/picker.time.js
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/robots.txt
--rw-rw-rw-   0 root         (0) root         (0)    48446 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/typeahead.jquery.js
--rw-rw-rw-   0 root         (0) root         (0)    20748 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/typeahead.jquery.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.588849 NEMO-4.5.5/NEMO/static/virtualkeyboard/
--rw-rw-rw-   0 root         (0) root         (0)   113008 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/virtualkeyboard/jquery.keyboard.js
--rw-rw-rw-   0 root         (0) root         (0)    47325 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/virtualkeyboard/jquery.keyboard.min.js
--rw-rw-rw-   0 root         (0) root         (0)     7848 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/virtualkeyboard/keyboard-basic.css
--rw-rw-rw-   0 root         (0) root         (0)     5889 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/virtualkeyboard/keyboard-basic.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.590849 NEMO-4.5.5/NEMO/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.590849 NEMO-4.5.5/NEMO/templates/abuse/
--rw-rw-rw-   0 root         (0) root         (0)     4059 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/abuse/abuse.html
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/abuse/user_drill_down.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.591849 NEMO-4.5.5/NEMO/templates/accounts_and_projects/
--rw-rw-rw-   0 root         (0) root         (0)     7380 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/accounts_and_projects/account_and_projects.html
--rw-rw-rw-   0 root         (0) root         (0)     6415 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/accounts_and_projects/accounts_and_projects.html
--rw-rw-rw-   0 root         (0) root         (0)     2843 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/accounts_and_projects/create_account.html
--rw-rw-rw-   0 root         (0) root         (0)     5002 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/accounts_and_projects/create_project.html
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/accounts_and_projects/documents_for_project.html
--rw-rw-rw-   0 root         (0) root         (0)     3530 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/accounts_and_projects/projects.html
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/accounts_and_projects/users_for_project.html
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/acknowledgement.html
--rw-rw-rw-   0 root         (0) root         (0)     4694 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/alerts.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.593849 NEMO-4.5.5/NEMO/templates/area_access/
--rw-rw-rw-   0 root         (0) root         (0)     2951 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/area_access/area_access.html
--rw-rw-rw-   0 root         (0) root         (0)     1687 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/area_access/calendar_self_login.html
--rw-rw-rw-   0 root         (0) root         (0)     1111 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/area_access/change_project.html
--rw-rw-rw-   0 root         (0) root         (0)     1141 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/area_access/login_areas.html
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/area_access/new_area_access_record.html
--rw-rw-rw-   0 root         (0) root         (0)     1938 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/area_access/new_area_access_record_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1454 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/area_access/self_login.html
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/authorization_failed.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.594849 NEMO-4.5.5/NEMO/templates/base/
--rw-rw-rw-   0 root         (0) root         (0)      308 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/base/footer.html
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/base/impersonate_header.html
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/base/navbar.html
--rw-rw-rw-   0 root         (0) root         (0)     7673 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/base/navbar_base.html
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/base/popup.html
--rw-rw-rw-   0 root         (0) root         (0)     5811 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.596849 NEMO-4.5.5/NEMO/templates/calendar/
--rw-rw-rw-   0 root         (0) root         (0)    24260 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/calendar.html
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/configuration.html
--rw-rw-rw-   0 root         (0) root         (0)     2834 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/configuration_helper.html
--rw-rw-rw-   0 root         (0) root         (0)     1254 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/policy_dialog.html
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/project_choice.html
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/proxy_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)     1862 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/reservation_event_feed.html
--rw-rw-rw-   0 root         (0) root         (0)     1619 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/reservation_questions.html
--rw-rw-rw-   0 root         (0) root         (0)     1285 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/reservation_warning.html
--rw-rw-rw-   0 root         (0) root         (0)     4094 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/scheduled_outage_information.html
--rw-rw-rw-   0 root         (0) root         (0)     2011 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/specific_user_feed.html
--rw-rw-rw-   0 root         (0) root         (0)     2543 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/usage_event_feed.html
--rw-rw-rw-   0 root         (0) root         (0)     6530 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/configuration_agenda.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.596849 NEMO-4.5.5/NEMO/templates/consumables/
--rw-rw-rw-   0 root         (0) root         (0)     8048 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/consumables/consumables.html
--rw-rw-rw-   0 root         (0) root         (0)     1518 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/consumables/consumables_order.html
--rw-rw-rw-   0 root         (0) root         (0)    11695 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/consumables/recurring_charge.html
--rw-rw-rw-   0 root         (0) root         (0)     5491 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/consumables/recurring_charges.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.597849 NEMO-4.5.5/NEMO/templates/contact/
--rw-rw-rw-   0 root         (0) root         (0)      692 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/contact/contact_staff.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.599849 NEMO-4.5.5/NEMO/templates/customizations/
--rw-rw-rw-   0 root         (0) root         (0)     1848 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations.html
--rw-rw-rw-   0 root         (0) root         (0)     2318 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_application.html
--rw-rw-rw-   0 root         (0) root         (0)     7799 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_calendar.html
--rw-rw-rw-   0 root         (0) root         (0)     7324 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_dashboard.html
--rw-rw-rw-   0 root         (0) root         (0)     4202 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_emails.html
--rw-rw-rw-   0 root         (0) root         (0)     2545 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_interlock.html
--rw-rw-rw-   0 root         (0) root         (0)     5553 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_projects_and_accounts.html
--rw-rw-rw-   0 root         (0) root         (0)     2224 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_rates.html
--rw-rw-rw-   0 root         (0) root         (0)     3519 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_recurring_charges.html
--rw-rw-rw-   0 root         (0) root         (0)     2183 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_remote_work.html
--rw-rw-rw-   0 root         (0) root         (0)    16712 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     3678 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_safety.html
--rw-rw-rw-   0 root         (0) root         (0)    27806 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_templates.html
--rw-rw-rw-   0 root         (0) root         (0)     8661 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_tool.html
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_upload.html
--rw-rw-rw-   0 root         (0) root         (0)     5214 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_user.html
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/display_success_and_redirect.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.600849 NEMO-4.5.5/NEMO/templates/email/
--rw-rw-rw-   0 root         (0) root         (0)     7800 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/email/compose_email.html
--rw-rw-rw-   0 root         (0) root         (0)     3153 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/email/email_broadcast.html
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/email/email_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.600849 NEMO-4.5.5/NEMO/templates/event_details/
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/event_details/area_access_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1347 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/event_details/outage_details.html
--rw-rw-rw-   0 root         (0) root         (0)     9603 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/event_details/reservation_details.html
--rw-rw-rw-   0 root         (0) root         (0)      589 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/event_details/usage_details.html
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/facility_rules.html
--rw-rw-rw-   0 root         (0) root         (0)     1247 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/feedback.html
--rw-rw-rw-   0 root         (0) root         (0)      937 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/history.html
--rw-rw-rw-   0 root         (0) root         (0)     1217 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/impersonate.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.600849 NEMO-4.5.5/NEMO/templates/jumbotron/
--rw-rw-rw-   0 root         (0) root         (0)     2059 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/jumbotron/jumbotron.html
--rw-rw-rw-   0 root         (0) root         (0)     3635 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/jumbotron/jumbotron_content.html
--rw-rw-rw-   0 root         (0) root         (0)     8671 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/landing.html
--rw-rw-rw-   0 root         (0) root         (0)     3496 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/login.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.601849 NEMO-4.5.5/NEMO/templates/maintenance/
--rw-rw-rw-   0 root         (0) root         (0)     1558 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/maintenance/closed_task_details.html
--rw-rw-rw-   0 root         (0) root         (0)     5566 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/maintenance/maintenance.html
--rw-rw-rw-   0 root         (0) root         (0)     7450 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/maintenance/pending_task_details.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.602849 NEMO-4.5.5/NEMO/templates/mobile/
--rw-rw-rw-   0 root         (0) root         (0)      762 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/mobile/cancellation_result.html
--rw-rw-rw-   0 root         (0) root         (0)     1916 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/mobile/choose_item.html
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/mobile/error.html
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/mobile/individual_outage.html
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/mobile/individual_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)     5899 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/mobile/new_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/mobile/no_active_projects.html
--rw-rw-rw-   0 root         (0) root         (0)      777 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/mobile/reservation_success.html
--rw-rw-rw-   0 root         (0) root         (0)     1442 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/mobile/view_calendar.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.603849 NEMO-4.5.5/NEMO/templates/news/
--rw-rw-rw-   0 root         (0) root         (0)      981 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/news/archived_news.html
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/news/new_news_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1198 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/news/news_update_form.html
--rw-rw-rw-   0 root         (0) root         (0)     2038 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/news/recent_news.html
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/no_project.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.604849 NEMO-4.5.5/NEMO/templates/occupancy/
--rw-rw-rw-   0 root         (0) root         (0)      408 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/occupancy/occupancy.html
--rw-rw-rw-   0 root         (0) root         (0)     1841 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/occupancy/occupancy_content.html
--rw-rw-rw-   0 root         (0) root         (0)     1147 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/occupancy/occupancy_count.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.604849 NEMO-4.5.5/NEMO/templates/pagination/
--rw-rw-rw-   0 root         (0) root         (0)      865 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/pagination/pagination_base.html
--rw-rw-rw-   0 root         (0) root         (0)      521 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/pagination/pagination_column.html
--rw-rw-rw-   0 root         (0) root         (0)      673 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/pagination/pagination_pages.html
--rw-rw-rw-   0 root         (0) root         (0)      642 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/pagination/pagination_selector.html
--rw-rw-rw-   0 root         (0) root         (0)     2841 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/qualifications.html
--rw-rw-rw-   0 root         (0) root         (0)     5462 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/refresh_sidebar_icons.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.604849 NEMO-4.5.5/NEMO/templates/remote_work/
--rw-rw-rw-   0 root         (0) root         (0)    10648 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/remote_work/remote_work.html
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/remote_work/remote_work_base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.605849 NEMO-4.5.5/NEMO/templates/requests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.605849 NEMO-4.5.5/NEMO/templates/requests/access_requests/
--rw-rw-rw-   0 root         (0) root         (0)     7754 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/requests/access_requests/access_request.html
--rw-rw-rw-   0 root         (0) root         (0)     3450 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/requests/access_requests/access_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     3480 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/requests/access_requests/access_requests_table.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.606849 NEMO-4.5.5/NEMO/templates/requests/adjustment_requests/
--rw-rw-rw-   0 root         (0) root         (0)     8607 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/requests/adjustment_requests/adjustment_request.html
--rw-rw-rw-   0 root         (0) root         (0)     3733 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/requests/adjustment_requests/adjustment_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     7180 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.606849 NEMO-4.5.5/NEMO/templates/requests/buddy_requests/
--rw-rw-rw-   0 root         (0) root         (0)     3910 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/requests/buddy_requests/buddy_request.html
--rw-rw-rw-   0 root         (0) root         (0)     5602 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/requests/buddy_requests/buddy_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     4246 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/requests/user_requests.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.606849 NEMO-4.5.5/NEMO/templates/resources/
--rw-rw-rw-   0 root         (0) root         (0)     2950 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/resources/modify_resource.html
--rw-rw-rw-   0 root         (0) root         (0)     3846 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/resources/resource_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/resources/resources.html
--rw-rw-rw-   0 root         (0) root         (0)     3807 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/resources/scheduled_outage.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.607849 NEMO-4.5.5/NEMO/templates/rest_framework/
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/rest_framework/api.html
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/rest_framework/custom_error.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.608849 NEMO-4.5.5/NEMO/templates/safety/
--rw-rw-rw-   0 root         (0) root         (0)     3112 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/safety/safety.html
--rw-rw-rw-   0 root         (0) root         (0)     1831 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/safety/safety_base.html
--rw-rw-rw-   0 root         (0) root         (0)     7754 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/safety/safety_data_sheets.html
--rw-rw-rw-   0 root         (0) root         (0)     1990 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/safety/safety_issues.html
--rw-rw-rw-   0 root         (0) root         (0)     1723 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/safety/safety_issues_create.html
--rw-rw-rw-   0 root         (0) root         (0)     1722 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/safety/safety_issues_resolved.html
--rw-rw-rw-   0 root         (0) root         (0)     1762 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/safety/safety_issues_update.html
--rw-rw-rw-   0 root         (0) root         (0)     1713 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/safety/safety_items.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.608849 NEMO-4.5.5/NEMO/templates/snippets/
--rw-rw-rw-   0 root         (0) root         (0)      516 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/snippets/button.html
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/snippets/contact_person.html
--rw-rw-rw-   0 root         (0) root         (0)     1128 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/snippets/embedded_document.html
--rw-rw-rw-   0 root         (0) root         (0)     1673 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/snippets/tool_info.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.609849 NEMO-4.5.5/NEMO/templates/staff_charges/
--rw-rw-rw-   0 root         (0) root         (0)      860 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/staff_charges/change_status.html
--rw-rw-rw-   0 root         (0) root         (0)     1242 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/staff_charges/choose_project.html
--rw-rw-rw-   0 root         (0) root         (0)      498 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/staff_charges/end_area_charge.html
--rw-rw-rw-   0 root         (0) root         (0)     1198 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/staff_charges/new_staff_charge.html
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/staff_charges/reminder.html
--rw-rw-rw-   0 root         (0) root         (0)     1854 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/staff_charges/staff_charges_base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.610849 NEMO-4.5.5/NEMO/templates/status_dashboard/
--rw-rw-rw-   0 root         (0) root         (0)     1554 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/status_dashboard/occupancy.html
--rw-rw-rw-   0 root         (0) root         (0)     8659 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/status_dashboard/staff.html
--rw-rw-rw-   0 root         (0) root         (0)     7728 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/status_dashboard/staff_absence.html
--rw-rw-rw-   0 root         (0) root         (0)     5799 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/status_dashboard/status_dashboard.html
--rw-rw-rw-   0 root         (0) root         (0)     3557 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/status_dashboard/tools.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.610849 NEMO-4.5.5/NEMO/templates/tasks/
--rw-rw-rw-   0 root         (0) root         (0)     2542 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/tasks/resolve.html
--rw-rw-rw-   0 root         (0) root         (0)     5037 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/tasks/update.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.611849 NEMO-4.5.5/NEMO/templates/tool_control/
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/tool_control/get_projects.html
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/tool_control/interlock_error.html
--rw-rw-rw-   0 root         (0) root         (0)     3502 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/tool_control/past_tasks_and_comments.html
--rw-rw-rw-   0 root         (0) root         (0)     2472 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/tool_control/qualified_users.html
--rw-rw-rw-   0 root         (0) root         (0)    15560 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/tool_control/tool_control.html
--rw-rw-rw-   0 root         (0) root         (0)    36294 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/tool_control/tool_status.html
--rw-rw-rw-   0 root         (0) root         (0)     6142 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/tool_control/usage_data.html
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/tool_control/use_tool_for_other.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.612849 NEMO-4.5.5/NEMO/templates/training/
--rw-rw-rw-   0 root         (0) root         (0)      512 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/training/get_projects.html
--rw-rw-rw-   0 root         (0) root         (0)     4964 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/training/training.html
--rw-rw-rw-   0 root         (0) root         (0)     1596 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/training/training_entry.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.612849 NEMO-4.5.5/NEMO/templates/usage/
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/usage/adjustment_request_button.html
--rw-rw-rw-   0 root         (0) root         (0)     3573 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/usage/billing.html
--rw-rw-rw-   0 root         (0) root         (0)     9302 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/usage/usage.html
--rw-rw-rw-   0 root         (0) root         (0)     6781 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/usage/usage_base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.613849 NEMO-4.5.5/NEMO/templates/users/
--rw-rw-rw-   0 root         (0) root         (0)    20751 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/users/create_or_modify_user.html
--rw-rw-rw-   0 root         (0) root         (0)     8054 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/users/preferences.html
--rw-rw-rw-   0 root         (0) root         (0)     3758 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/users/safe_deactivation.html
--rw-rw-rw-   0 root         (0) root         (0)     4160 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/users/users.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.613849 NEMO-4.5.5/NEMO/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7825 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templatetags/custom_tags_and_filters.py
--rw-rw-rw-   0 root         (0) root         (0)    25690 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    23501 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.620849 NEMO-4.5.5/NEMO/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4308 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/abuse.py
--rw-rw-rw-   0 root         (0) root         (0)    14736 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/access_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     8275 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/accounts_and_projects.py
--rw-rw-rw-   0 root         (0) root         (0)    17416 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/adjustment_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     1812 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/alerts.py
--rw-rw-rw-   0 root         (0) root         (0)    13935 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/api.py
--rw-rw-rw-   0 root         (0) root         (0)    12115 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/api_billing.py
--rw-rw-rw-   0 root         (0) root         (0)     2013 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/api_file_import.py
--rw-rw-rw-   0 root         (0) root         (0)    18830 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/area_access.py
--rw-rw-rw-   0 root         (0) root         (0)    11992 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     6625 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/buddy_requests.py
--rw-rw-rw-   0 root         (0) root         (0)    68771 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/calendar.py
--rw-rw-rw-   0 root         (0) root         (0)     2149 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/charge_validation.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/configuration_agenda.py
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    10021 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/consumables.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/contact_staff.py
--rw-rw-rw-   0 root         (0) root         (0)    17761 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/customization.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/documents.py
--rw-rw-rw-   0 root         (0) root         (0)     9978 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/email.py
--rw-rw-rw-   0 root         (0) root         (0)     1973 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/event_details.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/feedback.py
--rw-rw-rw-   0 root         (0) root         (0)     1672 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/get_projects.py
--rw-rw-rw-   0 root         (0) root         (0)     4168 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/history.py
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/jumbotron.py
--rw-rw-rw-   0 root         (0) root         (0)     3293 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/landing.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/maintenance.py
--rw-rw-rw-   0 root         (0) root         (0)     8059 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/mobile.py
--rw-rw-rw-   0 root         (0) root         (0)     3356 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/news.py
--rw-rw-rw-   0 root         (0) root         (0)     5188 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/notifications.py
--rw-rw-rw-   0 root         (0) root         (0)     1326 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)     4822 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/qualifications.py
--rw-rw-rw-   0 root         (0) root         (0)     9504 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/remote_work.py
--rw-rw-rw-   0 root         (0) root         (0)     3700 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/resources.py
--rw-rw-rw-   0 root         (0) root         (0)     8877 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/safety.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/sidebar.py
--rw-rw-rw-   0 root         (0) root         (0)    19900 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/status_dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)    12963 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)    23605 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/tool_control.py
--rw-rw-rw-   0 root         (0) root         (0)     5953 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/training.py
--rw-rw-rw-   0 root         (0) root         (0)     1909 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/tutorials.py
--rw-rw-rw-   0 root         (0) root         (0)    18636 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/usage.py
--rw-rw-rw-   0 root         (0) root         (0)     1049 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/user_requests.py
--rw-rw-rw-   0 root         (0) root         (0)    20715 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/users.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.621849 NEMO-4.5.5/NEMO/widgets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2968 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/widgets/configuration_editor.py
--rw-rw-rw-   0 root         (0) root         (0)    26360 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/widgets/dynamic_form.py
--rw-rw-rw-   0 root         (0) root         (0)     8029 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/widgets/item_tree.py
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.558849 NEMO-4.5.5/NEMO.egg-info/
--rw-r--r--   0 root         (0) root         (0)      904 2023-05-16 14:04:38.000000 NEMO-4.5.5/NEMO.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16413 2023-05-16 14:04:38.000000 NEMO-4.5.5/NEMO.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 14:04:38.000000 NEMO-4.5.5/NEMO.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-16 14:04:38.000000 NEMO-4.5.5/NEMO.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      263 2023-05-16 14:04:38.000000 NEMO-4.5.5/NEMO.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 14:04:38.000000 NEMO-4.5.5/NEMO.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      904 2023-05-16 14:04:38.621849 NEMO-4.5.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4066 2023-05-16 14:04:26.000000 NEMO-4.5.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.621849 NEMO-4.5.5/resources/
--rw-rw-rw-   0 root         (0) root         (0)     3957 2023-05-16 14:04:26.000000 NEMO-4.5.5/resources/splash_pad_settings.py
--rw-r--r--   0 root         (0) root         (0)      109 2023-05-16 14:04:38.622849 NEMO-4.5.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1460 2023-05-16 14:04:26.000000 NEMO-4.5.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.973250 NEMO-4.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1865 2023-07-18 17:03:12.000000 NEMO-4.6.0/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-18 17:03:12.000000 NEMO-4.6.0/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.906249 NEMO-4.6.0/NEMO/
+-rw-rw-rw-   0 root         (0) root         (0)     1254 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4594 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)    49666 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.907250 NEMO-4.6.0/NEMO/apps/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.908249 NEMO-4.6.0/NEMO/apps/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.893249 NEMO-4.6.0/NEMO/apps/area_access/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.908249 NEMO-4.6.0/NEMO/apps/area_access/static/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/static/area_access/area_access.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.894249 NEMO-4.6.0/NEMO/apps/area_access/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.910250 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/already_logged_in.html
+-rw-rw-rw-   0 root         (0) root         (0)      349 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/badge_not_found.html
+-rw-rw-rw-   0 root         (0) root         (0)     9006 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/choose_project.html
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/door_is_open.html
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/farewell_screen.html
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/inactive.html
+-rw-rw-rw-   0 root         (0) root         (0)      397 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/login_success.html
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/logout_success.html
+-rw-rw-rw-   0 root         (0) root         (0)      666 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/logout_warning.html
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/no_active_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/not_logged_in.html
+-rw-rw-rw-   0 root         (0) root         (0)      210 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/physical_access_denied.html
+-rw-rw-rw-   0 root         (0) root         (0)      566 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/resource_unavailable.html
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/welcome_screen.html
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    12663 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.912249 NEMO-4.6.0/NEMO/apps/contracts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4147 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      212 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/customization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.912249 NEMO-4.6.0/NEMO/apps/contracts/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.912249 NEMO-4.6.0/NEMO/apps/contracts/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/management/commands/send_email_contract_reminders.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.912249 NEMO-4.6.0/NEMO/apps/contracts/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     5839 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5550 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.894249 NEMO-4.6.0/NEMO/apps/contracts/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.913250 NEMO-4.6.0/NEMO/apps/contracts/templates/contracts/
+-rw-rw-rw-   0 root         (0) root         (0)     4319 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/templates/contracts/contractors.html
+-rw-rw-rw-   0 root         (0) root         (0)     4204 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/templates/contracts/contracts_and_procurements.html
+-rw-rw-rw-   0 root         (0) root         (0)     3726 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/templates/contracts/procurements.html
+-rw-rw-rw-   0 root         (0) root         (0)     5069 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/templates/contracts/service_contracts.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.913250 NEMO-4.6.0/NEMO/apps/contracts/templates/customizations/
+-rw-rw-rw-   0 root         (0) root         (0)     2580 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/templates/customizations/customizations_contracts.html
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.914250 NEMO-4.6.0/NEMO/apps/contracts/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10827 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/views/contracts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.914250 NEMO-4.6.0/NEMO/apps/kiosk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.895249 NEMO-4.6.0/NEMO/apps/kiosk/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.915249 NEMO-4.6.0/NEMO/apps/kiosk/static/kiosk/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/static/kiosk/kiosk.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.895249 NEMO-4.6.0/NEMO/apps/kiosk/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.916250 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/acknowledgement.html
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/category_choices.html
+-rw-rw-rw-   0 root         (0) root         (0)     2044 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/choices.html
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/error.html
+-rw-rw-rw-   0 root         (0) root         (0)     2923 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)    12592 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/kiosk.html
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/success.html
+-rw-rw-rw-   0 root         (0) root         (0)    17312 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/tool_information.html
+-rw-rw-rw-   0 root         (0) root         (0)     1108 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html
+-rw-rw-rw-   0 root         (0) root         (0)     4472 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    13386 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.917250 NEMO-4.6.0/NEMO/apps/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7128 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/customizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5237 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/evaluators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.917250 NEMO-4.6.0/NEMO/apps/sensors/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.918250 NEMO-4.6.0/NEMO/apps/sensors/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/management/commands/manage_sensor_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.918250 NEMO-4.6.0/NEMO/apps/sensors/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     7794 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13007 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4906 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/sensors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.895249 NEMO-4.6.0/NEMO/apps/sensors/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.920250 NEMO-4.6.0/NEMO/apps/sensors/static/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)   408236 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/static/sensors/chart.js
+-rw-rw-rw-   0 root         (0) root         (0)   195090 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/static/sensors/chart.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     1376 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js
+-rw-rw-rw-   0 root         (0) root         (0)     7659 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/static/sensors/daterangepicker.css
+-rw-rw-rw-   0 root         (0) root         (0)    66305 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/static/sensors/daterangepicker.js
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/static/sensors/sensors.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.896249 NEMO-4.6.0/NEMO/apps/sensors/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.920250 NEMO-4.6.0/NEMO/apps/sensors/templates/customizations/
+-rw-rw-rw-   0 root         (0) root         (0)     4718 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/templates/customizations/customizations_sensors.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.920250 NEMO-4.6.0/NEMO/apps/sensors/templates/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/templates/sensors/sensor_alerts.html
+-rw-rw-rw-   0 root         (0) root         (0)    15165 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/templates/sensors/sensor_data.html
+-rw-rw-rw-   0 root         (0) root         (0)     3879 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/templates/sensors/sensors.html
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     5650 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     3966 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/context_processors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5776 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3833 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    14224 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)    17784 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/interlocks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.920250 NEMO-4.6.0/NEMO/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.922250 NEMO-4.6.0/NEMO/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/cancel_unused_reservations.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/create_closure_alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/manage_recurring_charges.py
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/manage_tool_qualifications.py
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/send_email_out_of_time_reservation_notification.py
+-rw-rw-rw-   0 root         (0) root         (0)      415 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/send_email_reservation_ending_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/send_email_reservation_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/send_email_usage_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      456 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/send_email_user_access_expiration_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/send_email_weekend_access_notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     5578 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.927250 NEMO-4.6.0/NEMO/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    50307 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0001_version_1_0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)    32962 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0002_version_1_0_0_squashed.py
+-rw-rw-rw-   0 root         (0) root         (0)     7988 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0012_version_2_0_0_squashed.py
+-rw-rw-rw-   0 root         (0) root         (0)     9904 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0020_version_3_0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1712 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0021_version_3_1_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0022_version_3_3_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0023_badgereader.py
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0024_contactinformation_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     2674 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0025_version_3_6_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     5405 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0026_version_3_7_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0027_version_3_8_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     2231 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0028_version_3_9_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0030_version_3_9_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0031_version_3_10_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     3166 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0032_version_3_11_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0033_version_3_12_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0034_version_3_13_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     6747 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0035_version_3_14_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     7792 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0036_version_3_15_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     3717 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0037_version_3_16_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      935 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0038_version_4_0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     3601 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0039_version_4_1_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     2444 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0040_version_4_2_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0041_version_4_2_1.py
+-rw-rw-rw-   0 root         (0) root         (0)    16447 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0042_version_4_3_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0043_version_4_3_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5416 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0044_version_4_4_0.py
+-rw-rw-rw-   0 root         (0) root         (0)    13447 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0045_version_4_5_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     2037 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0045_version_4_5_5.py
+-rw-rw-rw-   0 root         (0) root         (0)     2997 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0046_version_4_6_0.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2299 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     7993 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/model_tree.py
+-rw-rw-rw-   0 root         (0) root         (0)   148191 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1429 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)    49662 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/policy.py
+-rw-rw-rw-   0 root         (0) root         (0)     9943 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/provisioning.py
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/rates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1037 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/rest_filter_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)    11173 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.931250 NEMO-4.6.0/NEMO/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.931250 NEMO-4.6.0/NEMO/static/admin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.931250 NEMO-4.6.0/NEMO/static/admin/physical_access_level/
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/admin/physical_access_level/access_level.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.932250 NEMO-4.6.0/NEMO/static/admin/questions_preview/
+-rw-rw-rw-   0 root         (0) root         (0)     4122 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/admin/questions_preview/questions_preview.css
+-rw-rw-rw-   0 root         (0) root         (0)     1372 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/admin/questions_preview/questions_preview.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.932250 NEMO-4.6.0/NEMO/static/admin/reservation_questions/
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/admin/reservation_questions/reservation_questions.js
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/admin/time_options_override.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.932250 NEMO-4.6.0/NEMO/static/admin/tool/
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/admin/tool/tool.js
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/badge_reader.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.897249 NEMO-4.6.0/NEMO/static/bootstrap/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.934250 NEMO-4.6.0/NEMO/static/bootstrap/css/
+-rw-rw-rw-   0 root         (0) root         (0)    22608 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap-theme.css
+-rw-rw-rw-   0 root         (0) root         (0)    43339 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap-theme.css.map
+-rw-rw-rw-   0 root         (0) root         (0)    19963 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap-theme.min.css
+-rw-rw-rw-   0 root         (0) root         (0)   141622 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap.css
+-rw-rw-rw-   0 root         (0) root         (0)   380986 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap.css.map
+-rw-rw-rw-   0 root         (0) root         (0)   117305 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.935250 NEMO-4.6.0/NEMO/static/bootstrap/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)    20127 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0 root         (0) root         (0)   108738 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0 root         (0) root         (0)    45404 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    23424 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-rw-rw-   0 root         (0) root         (0)    18028 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.935250 NEMO-4.6.0/NEMO/static/bootstrap/js/
+-rw-rw-rw-   0 root         (0) root         (0)    67546 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/js/bootstrap.js
+-rw-rw-rw-   0 root         (0) root         (0)    35951 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.935250 NEMO-4.6.0/NEMO/static/datetimepicker/
+-rw-rw-rw-   0 root         (0) root         (0)     9020 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/datetimepicker/bootstrap-datetimepicker.css
+-rw-rw-rw-   0 root         (0) root         (0)   105978 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/datetimepicker/bootstrap-datetimepicker.js
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.937250 NEMO-4.6.0/NEMO/static/fullcalendar/
+-rw-rw-rw-   0 root         (0) root         (0)    28531 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/fullcalendar/fullcalendar.css
+-rw-rw-rw-   0 root         (0) root         (0)   357749 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/fullcalendar/fullcalendar.js
+-rw-rw-rw-   0 root         (0) root         (0)    13687 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/fullcalendar/fullcalendar.min.css
+-rw-rw-rw-   0 root         (0) root         (0)   168700 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/fullcalendar/fullcalendar.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.937250 NEMO-4.6.0/NEMO/static/icons/
+-rw-rw-rw-   0 root         (0) root         (0)    24065 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/icons/agreement.png
+-rw-rw-rw-   0 root         (0) root         (0)    16685 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/icons/caution.png
+-rw-rw-rw-   0 root         (0) root         (0)     4664 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/icons/preferences.png
+-rw-rw-rw-   0 root         (0) root         (0)   247387 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)    84320 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/jquery.min.js
+-rw-rw-rw-   0 root         (0) root         (0)  1183392 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/jumbotron_watermark.bmp
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/mobile.js
+-rw-rw-rw-   0 root         (0) root         (0)   174603 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/moment.js
+-rw-rw-rw-   0 root         (0) root         (0)    58102 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/moment.min.js
+-rw-rw-rw-   0 root         (0) root         (0)    86041 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/moment.min.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    17874 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/nemo.css
+-rw-rw-rw-   0 root         (0) root         (0)    21828 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/nemo.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.938250 NEMO-4.6.0/NEMO/static/numpad/
+-rw-rw-rw-   0 root         (0) root         (0)    12285 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/numpad/custom_numpad.jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/numpad/numpad.jquery.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.939250 NEMO-4.6.0/NEMO/static/pickadate/
+-rw-rw-rw-   0 root         (0) root         (0)     3795 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/pickadate/default.css
+-rw-rw-rw-   0 root         (0) root         (0)     6040 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/pickadate/default.date.css
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/pickadate/default.time.css
+-rw-rw-rw-   0 root         (0) root         (0)    48215 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/pickadate/picker.date.js
+-rw-rw-rw-   0 root         (0) root         (0)    36941 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/pickadate/picker.js
+-rw-rw-rw-   0 root         (0) root         (0)    31899 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/pickadate/picker.time.js
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/robots.txt
+-rw-rw-rw-   0 root         (0) root         (0)    48446 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/typeahead.jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)    20748 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/typeahead.jquery.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.939250 NEMO-4.6.0/NEMO/static/virtualkeyboard/
+-rw-rw-rw-   0 root         (0) root         (0)   113008 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/virtualkeyboard/jquery.keyboard.js
+-rw-rw-rw-   0 root         (0) root         (0)    47325 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/virtualkeyboard/jquery.keyboard.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     7848 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/virtualkeyboard/keyboard-basic.css
+-rw-rw-rw-   0 root         (0) root         (0)     5889 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/virtualkeyboard/keyboard-basic.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.942250 NEMO-4.6.0/NEMO/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.942250 NEMO-4.6.0/NEMO/templates/abuse/
+-rw-rw-rw-   0 root         (0) root         (0)     4059 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/abuse/abuse.html
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/abuse/user_drill_down.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.943250 NEMO-4.6.0/NEMO/templates/accounts_and_projects/
+-rw-rw-rw-   0 root         (0) root         (0)     7665 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/accounts_and_projects/account_and_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)     6409 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/accounts_and_projects/accounts_and_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)     2843 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/accounts_and_projects/create_account.html
+-rw-rw-rw-   0 root         (0) root         (0)     6693 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/accounts_and_projects/create_project.html
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/accounts_and_projects/documents_for_project.html
+-rw-rw-rw-   0 root         (0) root         (0)     3544 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/accounts_and_projects/projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/accounts_and_projects/users_for_project.html
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/acknowledgement.html
+-rw-rw-rw-   0 root         (0) root         (0)     4694 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/alerts.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.944250 NEMO-4.6.0/NEMO/templates/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)     2951 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/area_access/area_access.html
+-rw-rw-rw-   0 root         (0) root         (0)     1748 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/area_access/calendar_self_login.html
+-rw-rw-rw-   0 root         (0) root         (0)     1111 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/area_access/change_project.html
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/area_access/login_areas.html
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/area_access/new_area_access_record.html
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/area_access/new_area_access_record_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/area_access/self_login.html
+-rw-rw-rw-   0 root         (0) root         (0)      837 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/authorization_failed.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.945250 NEMO-4.6.0/NEMO/templates/base/
+-rw-rw-rw-   0 root         (0) root         (0)      308 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/base/footer.html
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/base/impersonate_header.html
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/base/navbar.html
+-rw-rw-rw-   0 root         (0) root         (0)     8117 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/base/navbar_base.html
+-rw-rw-rw-   0 root         (0) root         (0)      308 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/base/popup.html
+-rw-rw-rw-   0 root         (0) root         (0)     6174 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.947250 NEMO-4.6.0/NEMO/templates/calendar/
+-rw-rw-rw-   0 root         (0) root         (0)    24673 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/calendar.html
+-rw-rw-rw-   0 root         (0) root         (0)     1442 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/configuration.html
+-rw-rw-rw-   0 root         (0) root         (0)     2834 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/configuration_helper.html
+-rw-rw-rw-   0 root         (0) root         (0)     1315 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/policy_dialog.html
+-rw-rw-rw-   0 root         (0) root         (0)     1361 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/project_choice.html
+-rw-rw-rw-   0 root         (0) root         (0)     1512 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/proxy_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)     1862 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/reservation_event_feed.html
+-rw-rw-rw-   0 root         (0) root         (0)     1680 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/reservation_questions.html
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/reservation_warning.html
+-rw-rw-rw-   0 root         (0) root         (0)     4410 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/scheduled_outage_information.html
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/specific_user_feed.html
+-rw-rw-rw-   0 root         (0) root         (0)     2543 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/usage_event_feed.html
+-rw-rw-rw-   0 root         (0) root         (0)     6530 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/configuration_agenda.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.948250 NEMO-4.6.0/NEMO/templates/consumables/
+-rw-rw-rw-   0 root         (0) root         (0)     8224 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/consumables/consumables.html
+-rw-rw-rw-   0 root         (0) root         (0)     1538 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/consumables/consumables_order.html
+-rw-rw-rw-   0 root         (0) root         (0)    11695 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/consumables/recurring_charge.html
+-rw-rw-rw-   0 root         (0) root         (0)     5473 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/consumables/recurring_charges.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.948250 NEMO-4.6.0/NEMO/templates/contact/
+-rw-rw-rw-   0 root         (0) root         (0)      692 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/contact/contact_staff.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.950250 NEMO-4.6.0/NEMO/templates/customizations/
+-rw-rw-rw-   0 root         (0) root         (0)     1848 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations.html
+-rw-rw-rw-   0 root         (0) root         (0)     4324 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_application.html
+-rw-rw-rw-   0 root         (0) root         (0)     7799 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_calendar.html
+-rw-rw-rw-   0 root         (0) root         (0)     7634 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_dashboard.html
+-rw-rw-rw-   0 root         (0) root         (0)     4202 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_emails.html
+-rw-rw-rw-   0 root         (0) root         (0)     2545 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_interlock.html
+-rw-rw-rw-   0 root         (0) root         (0)     5553 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_projects_and_accounts.html
+-rw-rw-rw-   0 root         (0) root         (0)     2224 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_rates.html
+-rw-rw-rw-   0 root         (0) root         (0)     3519 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_recurring_charges.html
+-rw-rw-rw-   0 root         (0) root         (0)     2183 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_remote_work.html
+-rw-rw-rw-   0 root         (0) root         (0)    16717 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     3678 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_safety.html
+-rw-rw-rw-   0 root         (0) root         (0)    27806 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_templates.html
+-rw-rw-rw-   0 root         (0) root         (0)     9253 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_tool.html
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_upload.html
+-rw-rw-rw-   0 root         (0) root         (0)     5214 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_user.html
+-rw-rw-rw-   0 root         (0) root         (0)      502 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/display_success_and_redirect.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.951250 NEMO-4.6.0/NEMO/templates/email/
+-rw-rw-rw-   0 root         (0) root         (0)     7825 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/email/compose_email.html
+-rw-rw-rw-   0 root         (0) root         (0)     3153 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/email/email_broadcast.html
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/email/email_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.951250 NEMO-4.6.0/NEMO/templates/event_details/
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/event_details/area_access_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     1376 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/event_details/outage_details.html
+-rw-rw-rw-   0 root         (0) root         (0)    12242 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/event_details/reservation_details.html
+-rw-rw-rw-   0 root         (0) root         (0)      589 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/event_details/usage_details.html
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/facility_rules.html
+-rw-rw-rw-   0 root         (0) root         (0)     1247 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/feedback.html
+-rw-rw-rw-   0 root         (0) root         (0)      937 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/history.html
+-rw-rw-rw-   0 root         (0) root         (0)     1260 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/impersonate.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.952250 NEMO-4.6.0/NEMO/templates/jumbotron/
+-rw-rw-rw-   0 root         (0) root         (0)     2059 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/jumbotron/jumbotron.html
+-rw-rw-rw-   0 root         (0) root         (0)     3635 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/jumbotron/jumbotron_content.html
+-rw-rw-rw-   0 root         (0) root         (0)     8670 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/landing.html
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/login.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.952250 NEMO-4.6.0/NEMO/templates/maintenance/
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/maintenance/closed_task_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     5566 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/maintenance/maintenance.html
+-rw-rw-rw-   0 root         (0) root         (0)     7450 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/maintenance/pending_task_details.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.953250 NEMO-4.6.0/NEMO/templates/mobile/
+-rw-rw-rw-   0 root         (0) root         (0)      762 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/mobile/cancellation_result.html
+-rw-rw-rw-   0 root         (0) root         (0)     1916 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/mobile/choose_item.html
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/mobile/error.html
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/mobile/individual_outage.html
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/mobile/individual_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)     5899 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/mobile/new_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/mobile/no_active_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      777 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/mobile/reservation_success.html
+-rw-rw-rw-   0 root         (0) root         (0)     1442 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/mobile/view_calendar.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.954250 NEMO-4.6.0/NEMO/templates/news/
+-rw-rw-rw-   0 root         (0) root         (0)      981 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/news/archived_news.html
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/news/new_news_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/news/news_update_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/news/recent_news.html
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/no_project.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.954250 NEMO-4.6.0/NEMO/templates/occupancy/
+-rw-rw-rw-   0 root         (0) root         (0)      408 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/occupancy/occupancy.html
+-rw-rw-rw-   0 root         (0) root         (0)     1841 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/occupancy/occupancy_content.html
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/occupancy/occupancy_count.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.955250 NEMO-4.6.0/NEMO/templates/pagination/
+-rw-rw-rw-   0 root         (0) root         (0)      865 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/pagination/pagination_base.html
+-rw-rw-rw-   0 root         (0) root         (0)      521 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/pagination/pagination_column.html
+-rw-rw-rw-   0 root         (0) root         (0)      673 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/pagination/pagination_pages.html
+-rw-rw-rw-   0 root         (0) root         (0)      642 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/pagination/pagination_selector.html
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/qualifications.html
+-rw-rw-rw-   0 root         (0) root         (0)     5462 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/refresh_sidebar_icons.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.955250 NEMO-4.6.0/NEMO/templates/remote_work/
+-rw-rw-rw-   0 root         (0) root         (0)    10616 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/remote_work/remote_work.html
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/remote_work/remote_work_base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.955250 NEMO-4.6.0/NEMO/templates/requests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.956250 NEMO-4.6.0/NEMO/templates/requests/access_requests/
+-rw-rw-rw-   0 root         (0) root         (0)     7754 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/requests/access_requests/access_request.html
+-rw-rw-rw-   0 root         (0) root         (0)     3450 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/requests/access_requests/access_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     3480 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/requests/access_requests/access_requests_table.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.956250 NEMO-4.6.0/NEMO/templates/requests/adjustment_requests/
+-rw-rw-rw-   0 root         (0) root         (0)     8607 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/requests/adjustment_requests/adjustment_request.html
+-rw-rw-rw-   0 root         (0) root         (0)     3733 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/requests/adjustment_requests/adjustment_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     7257 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.957250 NEMO-4.6.0/NEMO/templates/requests/buddy_requests/
+-rw-rw-rw-   0 root         (0) root         (0)     3910 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/requests/buddy_requests/buddy_request.html
+-rw-rw-rw-   0 root         (0) root         (0)     5602 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/requests/buddy_requests/buddy_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     4246 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/requests/user_requests.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.957250 NEMO-4.6.0/NEMO/templates/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     2950 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/resources/modify_resource.html
+-rw-rw-rw-   0 root         (0) root         (0)     3846 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/resources/resource_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/resources/resources.html
+-rw-rw-rw-   0 root         (0) root         (0)     3898 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/resources/scheduled_outage.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.957250 NEMO-4.6.0/NEMO/templates/rest_framework/
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/rest_framework/api.html
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/rest_framework/custom_error.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.959250 NEMO-4.6.0/NEMO/templates/safety/
+-rw-rw-rw-   0 root         (0) root         (0)     3112 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/safety/safety.html
+-rw-rw-rw-   0 root         (0) root         (0)     1733 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/safety/safety_base.html
+-rw-rw-rw-   0 root         (0) root         (0)     7807 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/safety/safety_data_sheets.html
+-rw-rw-rw-   0 root         (0) root         (0)     1976 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/safety/safety_issues.html
+-rw-rw-rw-   0 root         (0) root         (0)     1723 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/safety/safety_issues_create.html
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/safety/safety_issues_resolved.html
+-rw-rw-rw-   0 root         (0) root         (0)     1762 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/safety/safety_issues_update.html
+-rw-rw-rw-   0 root         (0) root         (0)     1877 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/safety/safety_items.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.959250 NEMO-4.6.0/NEMO/templates/snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      516 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/snippets/button.html
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/snippets/contact_person.html
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/snippets/document_list.html
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/snippets/embedded_document.html
+-rw-rw-rw-   0 root         (0) root         (0)     1673 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/snippets/tool_info.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.960250 NEMO-4.6.0/NEMO/templates/staff_charges/
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/staff_charges/change_status.html
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/staff_charges/choose_project.html
+-rw-rw-rw-   0 root         (0) root         (0)      498 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/staff_charges/end_area_charge.html
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/staff_charges/new_staff_charge.html
+-rw-rw-rw-   0 root         (0) root         (0)     1014 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/staff_charges/reminder.html
+-rw-rw-rw-   0 root         (0) root         (0)     1854 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/staff_charges/staff_charges_base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.961250 NEMO-4.6.0/NEMO/templates/status_dashboard/
+-rw-rw-rw-   0 root         (0) root         (0)     1554 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/status_dashboard/occupancy.html
+-rw-rw-rw-   0 root         (0) root         (0)     9771 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/status_dashboard/staff.html
+-rw-rw-rw-   0 root         (0) root         (0)     7709 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/status_dashboard/staff_absence.html
+-rw-rw-rw-   0 root         (0) root         (0)     6650 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/status_dashboard/status_dashboard.html
+-rw-rw-rw-   0 root         (0) root         (0)     3602 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/status_dashboard/tools.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.961250 NEMO-4.6.0/NEMO/templates/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)     2542 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/tasks/resolve.html
+-rw-rw-rw-   0 root         (0) root         (0)     5037 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/tasks/update.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.962250 NEMO-4.6.0/NEMO/templates/tool_control/
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/tool_control/get_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      737 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/tool_control/interlock_error.html
+-rw-rw-rw-   0 root         (0) root         (0)     3502 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/tool_control/past_tasks_and_comments.html
+-rw-rw-rw-   0 root         (0) root         (0)     2466 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/tool_control/qualified_users.html
+-rw-rw-rw-   0 root         (0) root         (0)    15303 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/tool_control/tool_control.html
+-rw-rw-rw-   0 root         (0) root         (0)    37737 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/tool_control/tool_status.html
+-rw-rw-rw-   0 root         (0) root         (0)     6142 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/tool_control/usage_data.html
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/tool_control/use_tool_for_other.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.963250 NEMO-4.6.0/NEMO/templates/training/
+-rw-rw-rw-   0 root         (0) root         (0)      512 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/training/get_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)     4971 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/training/training.html
+-rw-rw-rw-   0 root         (0) root         (0)     1962 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/training/training_entry.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.963250 NEMO-4.6.0/NEMO/templates/usage/
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/usage/adjustment_request_button.html
+-rw-rw-rw-   0 root         (0) root         (0)     3573 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/usage/billing.html
+-rw-rw-rw-   0 root         (0) root         (0)     9218 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/usage/usage.html
+-rw-rw-rw-   0 root         (0) root         (0)     7812 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/usage/usage_base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.964250 NEMO-4.6.0/NEMO/templates/users/
+-rw-rw-rw-   0 root         (0) root         (0)    20776 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/users/create_or_modify_user.html
+-rw-rw-rw-   0 root         (0) root         (0)    18558 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/users/preferences.html
+-rw-rw-rw-   0 root         (0) root         (0)     3758 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/users/safe_deactivation.html
+-rw-rw-rw-   0 root         (0) root         (0)     4181 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/users/users.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.964250 NEMO-4.6.0/NEMO/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8447 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templatetags/custom_tags_and_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    26303 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    24642 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.972250 NEMO-4.6.0/NEMO/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4308 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/abuse.py
+-rw-rw-rw-   0 root         (0) root         (0)    14733 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/access_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     8275 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/accounts_and_projects.py
+-rw-rw-rw-   0 root         (0) root         (0)    18760 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/adjustment_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     1812 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)    14004 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    12252 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/api_billing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2415 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/api_file_import.py
+-rw-rw-rw-   0 root         (0) root         (0)    19042 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/area_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    12070 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     6625 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/buddy_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    71717 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/calendar.py
+-rw-rw-rw-   0 root         (0) root         (0)     2334 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/charge_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/configuration_agenda.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    10947 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/consumables.py
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/contact_staff.py
+-rw-rw-rw-   0 root         (0) root         (0)    18708 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/customization.py
+-rw-rw-rw-   0 root         (0) root         (0)     3442 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/documents.py
+-rw-rw-rw-   0 root         (0) root         (0)    10015 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/email.py
+-rw-rw-rw-   0 root         (0) root         (0)     1973 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/event_details.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/feedback.py
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/get_projects.py
+-rw-rw-rw-   0 root         (0) root         (0)     4168 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/history.py
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/jumbotron.py
+-rw-rw-rw-   0 root         (0) root         (0)     3293 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/landing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/maintenance.py
+-rw-rw-rw-   0 root         (0) root         (0)     8072 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/mobile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3356 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/news.py
+-rw-rw-rw-   0 root         (0) root         (0)     5459 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/notifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)     4822 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/qualifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     9506 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/remote_work.py
+-rw-rw-rw-   0 root         (0) root         (0)     3700 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     8877 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/safety.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/sidebar.py
+-rw-rw-rw-   0 root         (0) root         (0)    20146 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/status_dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)    13615 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)    23995 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/tool_control.py
+-rw-rw-rw-   0 root         (0) root         (0)     6043 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/training.py
+-rw-rw-rw-   0 root         (0) root         (0)     1909 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/tutorials.py
+-rw-rw-rw-   0 root         (0) root         (0)    18360 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1049 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/user_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    20715 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/users.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.972250 NEMO-4.6.0/NEMO/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2968 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/widgets/configuration_editor.py
+-rw-rw-rw-   0 root         (0) root         (0)    26383 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/widgets/dynamic_form.py
+-rw-rw-rw-   0 root         (0) root         (0)     8029 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/widgets/item_tree.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.907250 NEMO-4.6.0/NEMO.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      904 2023-07-18 17:03:24.000000 NEMO-4.6.0/NEMO.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17375 2023-07-18 17:03:24.000000 NEMO-4.6.0/NEMO.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 17:03:24.000000 NEMO-4.6.0/NEMO.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-18 17:03:24.000000 NEMO-4.6.0/NEMO.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      264 2023-07-18 17:03:24.000000 NEMO-4.6.0/NEMO.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-18 17:03:24.000000 NEMO-4.6.0/NEMO.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      904 2023-07-18 17:03:24.973250 NEMO-4.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4066 2023-07-18 17:03:12.000000 NEMO-4.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.973250 NEMO-4.6.0/resources/
+-rw-rw-rw-   0 root         (0) root         (0)    17135 2023-07-18 17:03:12.000000 NEMO-4.6.0/resources/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     3981 2023-07-18 17:03:12.000000 NEMO-4.6.0/resources/splash_pad_settings.py
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-18 17:03:24.974250 NEMO-4.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-07-18 17:03:12.000000 NEMO-4.6.0/setup.py
```

### Comparing `NEMO-4.5.5/LICENSE.md` & `NEMO-4.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/__init__.py` & `NEMO-4.6.0/NEMO/__init__.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/actions.py` & `NEMO-4.6.0/NEMO/actions.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/admin.py` & `NEMO-4.6.0/NEMO/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from django.contrib.admin.decorators import display
 from django.contrib.admin.widgets import FilteredSelectMultiple
 from django.contrib.auth.models import Permission
 from django.contrib.contenttypes.admin import GenericStackedInline
 from django.db.models import Q
 from django.db.models.fields.files import FieldFile
 from django.forms import BaseInlineFormSet
+from django.shortcuts import redirect
 from django.template.defaultfilters import linebreaksbr, urlencode
 from django.utils.safestring import mark_safe
 from mptt.admin import DraggableMPTTAdmin, MPTTAdminForm, TreeRelatedFieldListFilter
 
 from NEMO.actions import (
 	access_requests_export_csv,
 	adjustment_requests_export_csv,
@@ -102,18 +103,37 @@
 	UserPreferences,
 	UserType,
 	record_active_state,
 	record_local_many_to_many_changes,
 	record_remote_many_to_many_changes_and_save,
 )
 from NEMO.utilities import admin_get_item, format_daterange
+from NEMO.views.constants import NEXT_PARAMETER_NAME
 from NEMO.views.customization import ProjectsAccountsCustomization
 from NEMO.widgets.dynamic_form import DynamicForm, PostUsageFloatFieldQuestion, PostUsageNumberFieldQuestion
 
 
+# Admin class to allow redirect after add or change
+class ModelAdminRedirect(admin.ModelAdmin):
+
+	def response_post_save_add(self, request, obj):
+		return self.response_redirect(request, super().response_post_save_add(request, obj))
+
+	def response_post_save_change(self, request, obj):
+		return self.response_redirect(request, super().response_post_save_change(request, obj))
+
+	def response_delete(self, request, obj_display, obj_id):
+		return self.response_redirect(request, super().response_delete(request, obj_display, obj_id))
+
+	def response_redirect(self, request, original_response):
+		if NEXT_PARAMETER_NAME in request.GET:
+			return redirect(request.GET[NEXT_PARAMETER_NAME])
+		return original_response
+
+
 # Formset to require at least one inline form
 class AtLeastOneRequiredInlineFormSet(BaseInlineFormSet):
 	def clean(self):
 		super().clean()
 		if any(self.errors):
 			return
 		if not any(cleaned_data and not cleaned_data.get("DELETE", False) for cleaned_data in self.cleaned_data):
@@ -204,14 +224,15 @@
 			None,
 			{
 				"fields": (
 					"name",
 					"parent_tool",
 					"_category",
 					"qualified_users",
+					"_qualifications_never_expire",
 					"_post_usage_questions",
 					"_post_usage_preview",
 				)
 			},
 		),
 		("Additional Information", {"fields": ("_description", "_serial", "_image", "_tool_calendar_color")}),
 		("Current state", {"fields": ("visible", "_operational")}),
@@ -399,22 +420,22 @@
 		""" We only want staff user and tool superusers to be possible trainers """
 		if db_field.name == "trainer":
 			kwargs["queryset"] = User.objects.filter(Q(is_staff=True) | Q(superuser_for_tools__isnull=False)).distinct()
 		return super().formfield_for_foreignkey(db_field, request, **kwargs)
 
 
 @register(StaffCharge)
-class StaffChargeAdmin(admin.ModelAdmin):
+class StaffChargeAdmin(ModelAdminRedirect):
 	list_display = ("id", "staff_member", "customer", "start", "end")
 	list_filter = ("start", ("customer", admin.RelatedOnlyFieldListFilter), ("staff_member", admin.RelatedOnlyFieldListFilter))
 	date_hierarchy = "start"
 
 
 @register(AreaAccessRecord)
-class AreaAccessRecordAdmin(admin.ModelAdmin):
+class AreaAccessRecordAdmin(ModelAdminRedirect):
 	list_display = ("id", "customer", "area", "project", "start", "end")
 	list_filter = (("area", TreeRelatedFieldListFilter), "start")
 	date_hierarchy = "start"
 
 
 @register(Configuration)
 class ConfigurationAdmin(admin.ModelAdmin):
@@ -522,15 +543,15 @@
 		record_active_state(request, obj, form, "active", not change)
 
 		if "principal_investigators" in form.changed_data:
 			obj.manager_set.set(form.cleaned_data["principal_investigators"])
 
 
 @register(Reservation)
-class ReservationAdmin(admin.ModelAdmin):
+class ReservationAdmin(ModelAdminRedirect):
 	list_display = (
 		"id",
 		"user",
 		"creator",
 		"tool",
 		"area",
 		"project",
@@ -626,15 +647,15 @@
 			'<div class="questions_preview">{}{}</div><div class="help questions_preview_help">Save form to preview reservation questions</div>'.format(
 				rendered_form, form_validity_div
 			)
 		)
 
 
 @register(UsageEvent)
-class UsageEventAdmin(admin.ModelAdmin):
+class UsageEventAdmin(ModelAdminRedirect):
 	list_display = ("id", "tool", "user", "operator", "project", "start", "end", "duration", "remote_work")
 	list_filter = ("remote_work", "start", "end", ("tool", admin.RelatedOnlyFieldListFilter))
 	date_hierarchy = "start"
 
 
 @register(Consumable)
 class ConsumableAdmin(admin.ModelAdmin):
@@ -847,14 +868,15 @@
 	list_display = ("name",)
 
 
 @register(UserPreferences)
 class UserPreferencesAdmin(admin.ModelAdmin):
 	list_display = ("user",)
 	search_fields = ["user_preferences__user__first_name", "user_preferences__user__last_name", "user_preferences__user__username"]
+	filter_horizontal = ["tool_freed_time_notifications", "tool_adjustment_notifications"]
 	form = UserPreferencesForm
 
 
 class UserAdminForm(forms.ModelForm):
 	class Meta:
 		model = User
 		fields = "__all__"
```

### Comparing `NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/already_logged_in.html` & `NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/already_logged_in.html`

 * *Files 9% similar despite different names*

```diff
@@ -8,25 +8,28 @@
 		<h2>However, a scheduled outage is in effect in the {{ scheduled_outage_in_progress.area }}</h2>
 	{% endif %}
 {% elif reservation_requirement_failed %}
 	<h2>However, you cannot enter since you don't have a current reservation for this area.</h2>
 {% endif %}
 <h2>Please visit the {{ facility_name}} staff if you believe this is an error.</h2>
 {% if not reservation_requirement_failed and not max_capacity_reached and not scheduled_outage_in_progress %}
-<h2>What would you like to do?</h2>
-<p>
-	<a href="javascript:void(0)" role="button" class="btn btn-success btn-lg btn-block btn-extra-large" onclick="revert_to_default_content()">
-		Do nothing and keep me logged in
-	</a>
-</p>
-<p>
-	<a href="javascript:void(0)" role="button" class="btn btn-success btn-lg btn-block btn-extra-large" onclick="just_open_the_door('{{ badge_number }}')">
-		Open the door and keep me logged in
-	</a>
-</p>
+    <h2>What would you like to do?</h2>
+    <p>
+        <a href="javascript:void(0)" role="button" class="btn btn-success btn-lg btn-block btn-extra-large" onclick="revert_to_default_content()">
+            Do nothing and keep me logged in
+        </a>
+    </p>
+    {# Don't offer to open the door if there is no interlock #}
+    {% if door.interlock %}
+        <p>
+            <a href="javascript:void(0)" role="button" class="btn btn-success btn-lg btn-block btn-extra-large" onclick="just_open_the_door('{{ badge_number }}')">
+                Open the door and keep me logged in
+            </a>
+        </p>
+    {% endif %}
 {% endif %}
 <p>
 	<a href="javascript:void(0)" role="button" class="btn btn-success btn-lg btn-block btn-extra-large" onclick="exit_area('{{ badge_number }}')">
 		Log out of the {{ area }}
 	</a>
 </p>
 <script>revert(15);</script>
```

#### html2text {}

```diff
@@ -14,10 +14,12 @@
 {% endif %}
 ***** Please visit the {{ facility_name}} staff if you believe this is an
 error. *****
 {% if not reservation_requirement_failed and not max_capacity_reached and not
 scheduled_outage_in_progress %}
 ***** What would you like to do? *****
 Do_nothing_and_keep_me_logged_in
+{# Don't offer to open the door if there is no interlock #} {% if
+door.interlock %}
 Open_the_door_and_keep_me_logged_in
-{% endif %}
+{% endif %} {% endif %}
 Log_out_of_the_{{_area_}}
```

### Comparing `NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/base.html` & `NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/choose_project.html` & `NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/choose_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/logout_warning.html` & `NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/logout_warning.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/resource_unavailable.html` & `NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/resource_unavailable.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/area_access/urls.py` & `NEMO-4.6.0/NEMO/apps/area_access/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/area_access/views.py` & `NEMO-4.6.0/NEMO/apps/area_access/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,53 +17,60 @@
 	NoPhysicalAccessUserError,
 	PhysicalAccessExpiredUserError,
 	ProjectChargeException,
 	ReservationRequiredUserError,
 	ScheduledOutageInProgressError,
 	UnavailableResourcesUserError,
 )
-from NEMO.models import (BadgeReader, Door, PhysicalAccessLog, PhysicalAccessType, Project, UsageEvent, User)
+from NEMO.models import (
+	AreaAccessRecord,
+	BadgeReader,
+	Door,
+	PhysicalAccessLog,
+	PhysicalAccessType,
+	Project,
+	UsageEvent,
+	User,
+)
 from NEMO.policy import policy_class as policy
 from NEMO.views.area_access import log_in_user_to_area, log_out_user
 from NEMO.views.customization import ApplicationCustomization, InterlockCustomization
 from NEMO.views.tool_control import interlock_bypass_allowed
 
 
 @login_required
 @permission_required("NEMO.add_areaaccessrecord")
 @require_GET
 def welcome_screen(request, door_id):
 	door = get_object_or_404(Door, id=door_id)
-	reader_id = request.GET.get("reader_id")
-	badge_reader = BadgeReader.objects.get(id=reader_id) if reader_id else BadgeReader.default()
+	dictionary = {"area": door.area, "door": door, "badge_reader": get_badge_reader(request)}
 	return render(
-		request, "area_access/welcome_screen.html", {"area": door.area, "door": door, "badge_reader": badge_reader}
+		request,
+		"area_access/welcome_screen.html",
+		dictionary,
 	)
 
 
 @login_required
 @permission_required("NEMO.change_areaaccessrecord")
 @require_GET
 def farewell_screen(request, door_id):
 	door = get_object_or_404(Door, id=door_id)
-	reader_id = request.GET.get("reader_id")
-	badge_reader = BadgeReader.objects.get(id=reader_id) if reader_id else BadgeReader.default()
-	return render(
-		request, "area_access/farewell_screen.html", {"area": door.area, "door": door, "badge_reader": badge_reader}
-	)
+	dictionary = {"area": door.area, "door": door, "badge_reader": get_badge_reader(request)}
+	return render(request, "area_access/farewell_screen.html", dictionary)
 
 
 @login_required
 @permission_required("NEMO.add_areaaccessrecord")
 @require_POST
 def login_to_area(request, door_id):
 	door = get_object_or_404(Door, id=door_id)
 
 	badge_number = request.POST.get("badge_number")
-	bypass_interlock = request.POST.get("bypass", 'False') == 'True'
+	bypass_interlock = request.POST.get("bypass", "False") == "True"
 	if not badge_number:
 		return render(request, "area_access/badge_not_found.html")
 	try:
 		user = User.objects.get(badge_number=badge_number)
 	except User.DoesNotExist:
 		return render(request, "area_access/badge_not_found.html")
 
@@ -135,20 +142,23 @@
 
 	except ReservationRequiredUserError:
 		# deal with this error after checking if the user is already logged in
 		reservation_requirement_failed = True
 
 	current_area_access_record = user.area_access_record()
 	if current_area_access_record and current_area_access_record.area == door.area:
+		if ApplicationCustomization.get_bool("area_logout_already_logged_in"):
+			return logout_of_area(request, door_id)
 		# No log entry necessary here because all validation checks passed.
 		# The log entry is captured when the subsequent choice is made by the user.
 		return render(
 			request,
 			"area_access/already_logged_in.html",
 			{
+				"door": door,
 				"area": door.area,
 				"project": current_area_access_record.project,
 				"badge_number": user.badge_number,
 				"reservation_requirement_failed": reservation_requirement_failed,
 				"max_capacity_reached": max_capacity_reached,
 				"scheduled_outage_in_progress": scheduled_outage_in_progress,
 			},
@@ -182,17 +192,19 @@
 			if not project_id:
 				# No log entry necessary here because all validation checks passed, and the user must indicate which project
 				# the wish to login under. The log entry is captured when the subsequent choice is made by the user.
 				return render(request, "area_access/choose_project.html", {"area": door.area, "user": user})
 			else:
 				project = get_object_or_404(Project, id=project_id)
 				try:
-					policy.check_billing_to_project(project, user, door.area)
+					policy.check_billing_to_project(project, user, door.area, AreaAccessRecord(area=door.area, project=project, customer=user))
 				except ProjectChargeException as e:
-					log.details = "The user attempted to bill the project named {} but got error: {}".format(project.name, e.msg)
+					log.details = "The user attempted to bill the project named {} but got error: {}".format(
+						project.name, e.msg
+					)
 					log.save()
 					return render(request, "area_access/physical_access_denied.html", {"message": e.msg})
 
 		log.result = PhysicalAccessType.ALLOW
 		log.save()
 
 		# Automatically log the user out of any previous area before logging them in to the new area.
@@ -209,19 +221,23 @@
 				else:
 					return interlock_error("Login", user)
 
 			delay_lock_door(door.id)
 
 		log_in_user_to_area(door.area, user, project)
 
-		return render(
-			request,
-			"area_access/login_success.html",
-			{"area": door.area, "name": user.first_name, "project": project, "previous_area": previous_area},
-		)
+		dictionary = {
+			"door": door,
+			"area": door.area,
+			"name": user.first_name,
+			"project": project,
+			"previous_area": previous_area,
+		}
+
+		return render(request, "area_access/login_success.html", dictionary)
 
 
 @postpone
 def delay_lock_door(door_id):
 	door = Door.objects.get(id=door_id)
 	sleep(8)
 	door.interlock.lock()
@@ -288,15 +304,20 @@
 				return interlock_error(bypass_allowed=False)
 			delay_lock_door(door.id)
 		return render(request, "area_access/door_is_open.html")
 	return render(request, "area_access/not_logged_in.html", {"area": door.area})
 
 
 def interlock_error(action: str = None, user: User = None, bypass_allowed: bool = None):
-	error_message = InterlockCustomization.get('door_interlock_failure_message')
+	error_message = InterlockCustomization.get("door_interlock_failure_message")
 	bypass_allowed = interlock_bypass_allowed(user) if bypass_allowed is None else bypass_allowed
-	dictionary = {
-		"message": linebreaksbr(error_message),
-		"bypass_allowed": bypass_allowed,
-		"action": action
-	}
+	dictionary = {"message": linebreaksbr(error_message), "bypass_allowed": bypass_allowed, "action": action}
 	return JsonResponse(dictionary, status=501)
+
+
+def get_badge_reader(request) -> BadgeReader:
+	reader_id = request.GET.get("reader_id") or ApplicationCustomization.get_int("default_badge_reader_id")
+	try:
+		badge_reader = BadgeReader.objects.get(id=reader_id)
+	except BadgeReader.DoesNotExist:
+		badge_reader = BadgeReader.default()
+	return badge_reader
```

### Comparing `NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/category_choices.html` & `NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/category_choices.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/choices.html` & `NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/choices.html`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 		</div>
 	</div>
 </div>
 
 {% if messages %}
     {% for message in messages %}
         <div class="alert alert-{{ message.level_tag }} alert-dismissible show-on-load" {% if message.extra_tags %}{{ message.extra_tags }}{% endif %} style="display: none; margin-top: 15px">
-            <button type="button" class="close" data-dismiss="alert">&times;</button>
+            <button type="button" class="close" data-dismiss="alert" aria-label="Modal close button">&times;</button>
             {{message}}
         </div>
     {% endfor %}
 {% endif %}
 
 {% if usage_events %}
 	<h1>Current {{ facility_name }} usage</h1>
```

### Comparing `NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/error.html` & `NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/error.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html` & `NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/kiosk.html` & `NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/kiosk.html`

 * *Files 2% similar despite different names*

```diff
@@ -246,20 +246,21 @@
 			if (tool_id)
 			{
 				data += '&tool_id=' + tool_id;
 			}
 			status_element.html("<h1>Enabling tool...</h1>").show();
 			try_post_catch_interlock_error('{% url 'enable_tool_from_kiosk' %}', data);
 		}
-		function disable_tool()
+		function disable_tool(shorten)
 		{
 			default_content_element.hide();
 			error_element.hide();
 			error_interlock_element.hide();
 			let data = $('#tool_control').serialize();
+            if (shorten !== undefined && shorten) data += '&shorten=True';
 			status_element.html("<h1>Disabling tool...</h1>").show();
 			try_post_catch_interlock_error('{% url 'disable_tool_from_kiosk' %}', data);
 		}
 		function interlock_success_callback(response, status, xml_http_request)
         {
             error_interlock_element.hide();
             status_element.html(response).show();
```

### Comparing `NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/success.html` & `NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/success.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/tool_information.html` & `NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/tool_information.html`

 * *Files 7% similar despite different names*

```diff
@@ -227,20 +227,27 @@
 					Use the following field to prevent others from using the tool for <input id="downtime" type="number" name="downtime" class="form-control" style="display:inline; width:auto" min="5" max="120" inputmode="numeric" pattern="[0-9]*" placeholder="0"> minutes after disabling the tool.
 					<a id="delayed_logoff_help" class="pointer" tabindex="0" data-toggle="popover" data-placement="bottom" data-trigger="focus" data-content="Some tools may require downtime after you finish using them. (For example, to perform automated cleaning or pump-down). Once you click &quot;Stop using the {{ tool.name_or_child_in_use_name }}&quot; the tool interlock will immediately disable the tool and it will remain unusable for the specified duration. Leave the duration blank to indicate that no post-usage downtime is required.">What's this?</a>
 				</div>
 			{% endif %}
 			<div class="row">
 				<div class="col-xs-offset-3 col-xs-6" style="margin-top:30px">
 					<h2 id="answer_to_proceed" style="text-align:center">Please answer the required questions (above) to stop using the {{ tool.name_or_child_in_use_name }}</h2>
-					<div id="stop_button" class="alert alert-danger" style="text-align:center; margin-bottom:0; font-size:x-large" onclick="disable_tool()">
-						<span class="glyphicon glyphicon-stop"></span> Stop using the {{ tool.name_or_child_in_use_name }}
-						{% if remaining_reservation_duration %}
-							and relinquish the remaining {{ remaining_reservation_duration }} minutes of your reservation
-						{% endif %}
-					</div>
+					<div id="stop_button">
+                        <div class="alert alert-danger" style="text-align:center; margin-bottom:0; font-size:x-large" onclick="disable_tool()">
+                            <span class="glyphicon glyphicon-stop"></span> Stop using the {{ tool.name_or_child_in_use_name }}
+                            {% if not user.is_staff and remaining_reservation_duration %}
+                                and relinquish the remaining {{ remaining_reservation_duration }} minutes of your reservation
+                            {% endif %}
+                        </div>
+                        {% if remaining_reservation_duration and user.is_staff %}
+                            <div class="alert alert-danger" style="text-align:center; margin-bottom:0; margin-top: 10px; font-size:x-large" onclick="disable_tool(true)">
+                                <span class="glyphicon glyphicon-stop"></span> Stop using the {{ tool.name_or_child_in_use_name }} and relinquish the remaining {{ remaining_reservation_duration }} minutes of your reservation
+                            </div>
+                        {% endif %}
+                    </div>
 				</div>
 			</div>
 		{% endif %}
 		<div style="width: 100%;padding-top: 40px;border-bottom: 1px dashed lightgray"></div>
 		<h1>Make a reservation</h1>
 		{% include 'kiosk/tool_project_selection_snippet.html' with active_projects=customer.active_projects tool=tool %}
 		<div id="start_reserve" class="col-xs-offset-3 col-xs-6" style="display: none;margin-top:30px">
```

#### html2text {}

```diff
@@ -93,17 +93,21 @@
 tool.delayed_logoff_in_progress %}
 ***** Delayed logoff *****
 Use the following field to prevent others from using the tool for [Unknown
 INPUT type] minutes after disabling the tool. What's this?
 {% endif %}
 ***** Please answer the required questions (above) to stop using the {
 { tool.name_or_child_in_use_name }} *****
- Stop using the {{ tool.name_or_child_in_use_name }} {% if
-remaining_reservation_duration %} and relinquish the remaining {
+ Stop using the {{ tool.name_or_child_in_use_name }} {% if not user.is_staff
+and remaining_reservation_duration %} and relinquish the remaining {
 { remaining_reservation_duration }} minutes of your reservation {% endif %}
+{% if remaining_reservation_duration and user.is_staff %}
+ Stop using the {{ tool.name_or_child_in_use_name }} and relinquish the
+remaining {{ remaining_reservation_duration }} minutes of your reservation
+{% endif %}
 {% endif %}
 ****** Make a reservation ******
 {% include 'kiosk/tool_project_selection_snippet.html' with
 active_projects=customer.active_projects tool=tool %}
  Reserve the {{ tool.name }}
 {% else %} {% if customer.is_staff or customer.is_service_personnel and tool in
 customer.qualifications.all or tool.ready_to_use and tool in
```

### Comparing `NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html` & `NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html` & `NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/kiosk/urls.py` & `NEMO-4.6.0/NEMO/apps/kiosk/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/kiosk/views.py` & `NEMO-4.6.0/NEMO/apps/kiosk/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from NEMO.views.calendar import (
 	cancel_the_reservation,
 	extract_configuration,
 	extract_reservation_questions,
 	render_reservation_questions,
 	shorten_reservation,
 )
+from NEMO.views.customization import ApplicationCustomization
 from NEMO.views.status_dashboard import create_tool_summary
 from NEMO.views.tool_control import (
 	email_managers_required_questions_disable_tool,
 	interlock_bypass_allowed,
 	interlock_error,
 )
 from NEMO.widgets.dynamic_form import DynamicForm
@@ -38,15 +39,15 @@
 @synchronized("tool_id")
 def do_enable_tool(request, tool_id):
 	tool = Tool.objects.get(id=tool_id)
 	customer = User.objects.get(id=request.POST["customer_id"])
 	project = Project.objects.get(id=request.POST["project_id"])
 	bypass_interlock = request.POST.get("bypass", "False") == "True"
 
-	response = policy.check_to_enable_tool(tool, operator=customer, user=customer, project=project, staff_charge=False)
+	response = policy.check_to_enable_tool(tool, operator=customer, user=customer, project=project, staff_charge=False, remote_work=False)
 	if response.status_code != HTTPStatus.OK:
 		dictionary = {
 			"message": "You are not authorized to enable this tool. {}".format(response.content.decode()),
 			"delay": 10,
 		}
 		return render(request, "kiosk/acknowledgement.html", dictionary)
 
@@ -91,15 +92,16 @@
 	if tool.interlock and not tool.interlock.lock():
 		if bypass_interlock and interlock_bypass_allowed(customer):
 			pass
 		else:
 			return interlock_error("Disable", customer)
 
 	# Shorten the user's tool reservation since we are now done using the tool
-	shorten_reservation(user=customer, item=tool, new_end=timezone.now() + downtime)
+	staff_shortening = request.POST.get("shorten", False)
+	shorten_reservation(user=customer, item=tool, new_end=timezone.now() + downtime, force=staff_shortening)
 
 	# End the current usage event for the tool and save it.
 	current_usage_event = tool.get_current_usage_event()
 	current_usage_event.end = timezone.now() + downtime
 
 	# Collect post-usage questions
 	dynamic_form = DynamicForm(tool.post_usage_questions)
@@ -177,28 +179,30 @@
 	reservation.additional_information, reservation.self_configuration = extract_configuration(request)
 	# Reservation can't be short notice if the user is configuring the tool themselves.
 	if reservation.self_configuration:
 		reservation.short_notice = False
 
 	# Reservation questions if applicable
 	try:
-		reservation.question_data = extract_reservation_questions(request, ReservationItemType.TOOL, tool.id, reservation.project)
+		reservation.question_data = extract_reservation_questions(
+			request, ReservationItemType.TOOL, tool.id, reservation.project
+		)
 	except RequiredUnansweredQuestionsException as e:
 		error_dictionary["message"] = str(e)
 		return render(request, "kiosk/error.html", error_dictionary)
 
 	reservation.save_and_notify()
 	return render(request, "kiosk/success.html", {"new_reservation": reservation, "customer": customer})
 
 
 @login_required
 @permission_required("NEMO.kiosk")
 @require_POST
 def cancel_reservation(request, reservation_id):
-	""" Cancel a reservation for a user. """
+	"""Cancel a reservation for a user."""
 	reservation = Reservation.objects.get(id=reservation_id)
 	customer = User.objects.get(id=request.POST["customer_id"])
 
 	response = cancel_the_reservation(reservation=reservation, user_cancelling_reservation=customer, reason=None)
 
 	if response.status_code == HTTPStatus.OK:
 		return render(request, "kiosk/success.html", {"cancelled_reservation": reservation, "customer": customer})
@@ -264,15 +268,16 @@
 
 	categories = [
 		t[0] for t in Tool.objects.filter(visible=True).order_by("_category").values_list("_category").distinct()
 	]
 	unqualified_categories = [
 		category
 		for category in categories
-		if not customer.is_staff and not Tool.objects.filter(
+		if not customer.is_staff
+		   and not Tool.objects.filter(
 			visible=True, _category=category, id__in=customer.qualifications.all().values_list("id")
 		).exists()
 	]
 	dictionary = {
 		"now": timezone.now(),
 		"customer": customer,
 		"usage_events": list(usage_events),
@@ -332,23 +337,28 @@
 			shortened=False,
 			user=customer,
 			tool=tool,
 		)
 		remaining_reservation_duration = int((current_reservation.end - timezone.now()).total_seconds() / 60)
 		# We don't need to bother telling the user their reservation will be shortened if there's less than two minutes left.
 		# Staff are exempt from reservation shortening.
-		if remaining_reservation_duration > 2 and not customer.is_staff:
+		if remaining_reservation_duration > 2:
 			dictionary["remaining_reservation_duration"] = remaining_reservation_duration
 	except Reservation.DoesNotExist:
 		pass
 	return render(request, "kiosk/tool_information.html", dictionary)
 
 
 @login_required
 @permission_required("NEMO.kiosk")
 @require_GET
 def kiosk(request, location=None):
-	reader_id = request.GET.get("reader_id")
-	dictionary = {
-		"badge_reader": BadgeReader.objects.get(id=reader_id) if reader_id else BadgeReader.default(),
-	}
-	return render(request, "kiosk/kiosk.html", dictionary)
+	return render(request, "kiosk/kiosk.html", {"badge_reader": get_badge_reader(request)})
+
+
+def get_badge_reader(request) -> BadgeReader:
+	reader_id = request.GET.get("reader_id") or ApplicationCustomization.get_int("default_badge_reader_id")
+	try:
+		badge_reader = BadgeReader.objects.get(id=reader_id)
+	except BadgeReader.DoesNotExist:
+		badge_reader = BadgeReader.default()
+	return badge_reader
```

### Comparing `NEMO-4.5.5/NEMO/apps/sensors/admin.py` & `NEMO-4.6.0/NEMO/apps/sensors/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,14 @@
 	def get_display_value(self, obj: SensorData):
 		return obj.display_value()
 
 
 @register(SensorAlertEmail)
 class SensorAlertEmailAdmin(admin.ModelAdmin):
 	list_display = ("sensor", "enabled", "trigger_condition", "trigger_no_data", "additional_emails", "triggered_on")
-	readonly_fields = ("triggered_on",)
 
 
 @register(SensorAlertLog)
 class SensorAlertLogAdmin(admin.ModelAdmin):
 	list_display = ["id", "time", "sensor", "reset", "value"]
 	list_filter = [("sensor", admin.RelatedOnlyFieldListFilter), "value", "reset"]
 	date_hierarchy = "time"
```

### Comparing `NEMO-4.5.5/NEMO/apps/sensors/evaluators.py` & `NEMO-4.6.0/NEMO/apps/sensors/evaluators.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/sensors/migrations/0001_initial.py` & `NEMO-4.6.0/NEMO/apps/sensors/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/sensors/models.py` & `NEMO-4.6.0/NEMO/apps/sensors/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+from __future__ import annotations
+
 import datetime
 import random
 from logging import getLogger
 from typing import List, Optional
 
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ValidationError
 from django.core.validators import MaxValueValidator, MinValueValidator
 from django.db import models
-from django.db.models import QuerySet
 from django.utils import timezone
 from django.utils.safestring import mark_safe
 
 from NEMO.apps.sensors.customizations import SensorCustomization
 from NEMO.apps.sensors.evaluators import evaluate_boolean_expression
 from NEMO.fields import MultiEmailField
 from NEMO.models import BaseModel, InterlockCard
+from NEMO.typing import QuerySetType
 from NEMO.utilities import EmailCategory, format_datetime, get_email_from_settings, send_mail
 
 models_logger = getLogger(__name__)
 
 
 class SensorCardCategory(BaseModel):
 	name = models.CharField(max_length=200, help_text="The name for this sensor card category")
@@ -295,15 +297,15 @@
 		pass
 
 	def trigger_alert(self, alert_time: datetime.datetime, value: float = None):
 		# This should be implemented in children of this class
 		pass
 
 	@classmethod
-	def sensor_alert_filter(cls, enabled=True, sensor=None) -> List[QuerySet]:
+	def sensor_alert_filter(cls, enabled=True, sensor=None) -> List[QuerySetType[SensorAlert]]:
 		sensor_alert_qs = []
 		for sub_class in cls.__subclasses__():
 			sub_filter = sub_class.objects.all()
 			if enabled is not None:
 				sub_filter = sub_filter.filter(enabled=enabled)
 			if sensor:
 				sub_filter = sub_filter.filter(sensor=sensor)
```

### Comparing `NEMO-4.5.5/NEMO/apps/sensors/sensors.py` & `NEMO-4.6.0/NEMO/apps/sensors/sensors.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Dict, List
 
 from django.core.exceptions import ValidationError
 from django.utils.translation import gettext_lazy as _
 from pymodbus.client import ModbusTcpClient
 
 from NEMO.apps.sensors.admin import SensorAdminForm, SensorCardAdminForm
+from NEMO.apps.sensors.customizations import SensorCustomization
 from NEMO.apps.sensors.evaluators import evaluate_expression, evaluate_modbus_expression
 from NEMO.apps.sensors.models import Sensor as Sensor_model, SensorAlert, SensorCardCategory, SensorData
 
 sensors_logger = getLogger(__name__)
 
 
 class Sensor(ABC):
@@ -33,15 +34,26 @@
 		if not sensor.card.enabled:
 			warning_message = f"{sensor.name} sensor interface mocked out because sensor card is disabled."
 			sensors_logger.warning(warning_message)
 			return warning_message
 
 		data = None
 		try:
-			registers = self.do_read_values(sensor)
+			retries = SensorCustomization.get_int("sensor_read_retries")
+			total_tries = 1 + retries
+			# Handle retries
+			for attempt_number in range(total_tries):
+				try:
+					registers = self.do_read_values(sensor)
+					break
+				except:
+					if attempt_number == total_tries - 1:
+						raise
+					else:
+						continue
 			data_value = self.evaluate_sensor(sensor, registers=registers)
 			if data_value:
 				data = SensorData.objects.create(sensor=sensor, value=data_value)
 				process_alerts(sensor, data)
 				return data
 		except Exception as error:
 			sensors_logger.error(error)
@@ -82,15 +94,15 @@
 
 
 class ModbusTcpSensor(Sensor):
 	def clean_sensor(self, sensor_form: SensorAdminForm):
 		read_address = sensor_form.cleaned_data["read_address"]
 		number_of_values = sensor_form.cleaned_data["number_of_values"]
 		error = {}
-		if not read_address:
+		if read_address is None:
 			error["read_address"] = _("This field is required.")
 		if not number_of_values:
 			error["number_of_values"] = _("This field is required.")
 		if error:
 			raise ValidationError(error)
 
 	def do_read_values(self, sensor: Sensor_model) -> List:
```

### Comparing `NEMO-4.5.5/NEMO/apps/sensors/static/sensors/chart.js` & `NEMO-4.6.0/NEMO/apps/sensors/static/sensors/chart.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/sensors/static/sensors/chart.min.js` & `NEMO-4.6.0/NEMO/apps/sensors/static/sensors/chart.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js` & `NEMO-4.6.0/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/sensors/static/sensors/daterangepicker.css` & `NEMO-4.6.0/NEMO/apps/sensors/static/sensors/daterangepicker.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/sensors/static/sensors/daterangepicker.js` & `NEMO-4.6.0/NEMO/apps/sensors/static/sensors/daterangepicker.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/sensors/static/sensors/sensors.css` & `NEMO-4.6.0/NEMO/apps/sensors/static/sensors/sensors.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/sensors/templates/customizations/customizations_sensors.html` & `NEMO-4.6.0/NEMO/apps/sensors/templates/customizations/customizations_sensors.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,56 @@
 {% load custom_tags_and_filters %}
 <div class="panel-body">
     <h3 class="customization-section-title">Sensor data settings</h3>
     <form method="POST" action="{% url 'customize' 'sensors' %}" class="form-horizontal">
         {% csrf_token %}
+        <div class="form-group {% if errors.sensor_read_retries %}has-error{% endif %}">
+            <label class="control-label col-md-3" for="sensor_read_retries">Retry reading data</label>
+            <div class="col-md-3">
+                <div class="input-group">
+                    <input type="number" min="0" id="sensor_read_retries" name="sensor_read_retries" class="form-control text-right" value="{% if errors.sensor_read_retries %}{{ errors.sensor_read_retries.value }}{% else %}{{ sensor_read_retries }}{% endif %}"/>
+                    <span class="input-group-addon">time(s)</span>
+                </div>
+            </div>
+            <div class="col-md-offset-3 col-md-9 help-block light-grey">
+                {% if errors.sensor_read_retries %}
+                    {{ errors.sensor_read_retries.error }}
+                {% else %}
+                    The number of times to retry reading data from sensors before raising an error. Set to 0 to never retry.
+                {% endif %}
+            </div>
+        </div>
         <div class="form-group {% if errors.sensor_alert_emails %}has-error{% endif %}">
-            <label class="control-label col-md-2" for="sensor_alert_emails">Sensor alert email(s)</label>
+            <label class="control-label col-md-3" for="sensor_alert_emails">Sensor alert email(s)</label>
             <div class="col-md-5">
                 <input type="text" id="sensor_alert_emails" name="sensor_alert_emails" class="form-control" value="{% if errors.sensor_alert_emails %}{{ errors.sensor_alert_emails.value }}{% else %}{{ sensor_alert_emails }}{% endif %}" placeholder="sensor_alerts@example.org"/>
             </div>
-            <div class="col-md-5 help-block light-grey">
+            <div class="col-md-offset-3 col-md-9 help-block light-grey">
                 {% if errors.sensor_alert_emails %}
                     {{ errors.sensor_alert_emails.error }}
                 {% else %}
                     The email(s) to notify when a sensor alert is raised or reset. A comma-separated list can be used.
                 {% endif %}
             </div>
         </div>
         <div class="form-group">
-            <label class="control-label col-md-2 col-sm-2" for="sensor_default_daterange">Default daterange</label>
-            <div class="col-md-10 col-sm-10">
+            <label class="control-label col-md-3" for="sensor_default_daterange">Default daterange</label>
+            <div class="col-md-9">
                 <div class="radio">
                     <label><input type="radio" id="sensor_default_daterange" name="sensor_default_daterange" {% if not sensor_default_daterange %}checked{% endif %} value=""> Last 24 hrs</label>
                     <label><input type="radio" name="sensor_default_daterange" {% if sensor_default_daterange == 'last_72hrs' %}checked{% endif %} value="last_72hrs"> Last 72 hrs</label>
                     <label><input type="radio" name="sensor_default_daterange" {% if sensor_default_daterange == 'last_week' %}checked{% endif %} value="last_week"> Last week</label>
                     <label><input type="radio" name="sensor_default_daterange" {% if sensor_default_daterange == 'last_month' %}checked{% endif %} value="last_month"> Last month</label>
                     <label><input type="radio" name="sensor_default_daterange" {% if sensor_default_daterange == 'last_year' %}checked{% endif %} value="last_year"> Last year</label>
                 </div>
             </div>
         </div>
         <div class="form-group">
-            <label class="control-label col-md-2 col-sm-2" for="refresh-rate">Default refresh rate:</label>
-            <div class="col-md-3 col-sm-4">
+            <label class="control-label col-md-3" for="refresh-rate">Default refresh rate:</label>
+            <div class="col-md-3">
                 <select class="form-control" name="sensor_default_refresh_rate" id="refresh-rate">
                     <option value="" {% if not sensor_default_refresh_rate %}selected{% endif %}>no refresh</option>
                     <option value="1000" {% if sensor_default_refresh_rate == "1000" %}selected{% endif %}>every second</option>
                     <option value="5000" {% if sensor_default_refresh_rate == "5000" %}selected{% endif %}>every 5 seconds</option>
                     <option value="30000" {% if sensor_default_refresh_rate == "30000" %}selected{% endif %}>every 30 seconds</option>
                     <option value="60000" {% if sensor_default_refresh_rate == "60000" %}selected{% endif %}>every minute</option>
                     <option value="300000" {% if sensor_default_refresh_rate == "300000" %}selected{% endif %}>every 5 minutes</option>
```

### Comparing `NEMO-4.5.5/NEMO/apps/sensors/templates/sensors/sensor_data.html` & `NEMO-4.6.0/NEMO/apps/sensors/templates/sensors/sensor_data.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/sensors/templates/sensors/sensors.html` & `NEMO-4.6.0/NEMO/apps/sensors/templates/sensors/sensors.html`

 * *Files 19% similar despite different names*

```diff
@@ -43,9 +43,33 @@
                         <a href="{% url 'admin:app_list' 'sensors' %}">
                             Administration -> Detailed Administration -> Sensors
                         </a>
                     {% endif %}
                 </div>
             {% endif %}
         </ul>
+        {% if sensors or categories %}
+            {%if selected_category or alert_logs %}
+                <div class="panel-body">
+                    <ul class="nav nav-tabs" id="tabs">
+                        <li class="active">
+                            <a>Alert log</a>
+                        </li>
+                    </ul>
+                    <div id="no-sensor-data" class="tab-content panel panel-default panel-tab-content" style="margin-bottom: 0">
+                        <div class="panel-body">
+                            {% if alert_logs %}
+                                <ul style="margin-top: 10px;">
+                                    {% for alert in alert_logs %}
+                                        <li class="{% if alert.reset %}success-highlight{% else %}danger-highlight{% endif %}">[{{ alert.sensor.name }}] {{ alert.description }}</li>
+                                    {% endfor %}
+                                </ul>
+                            {% else %}
+                                <i>There are no alerts for sensors in the {{ selected_category }}.</i>
+                            {% endif %}
+                        </div>
+                    </div>
+                </div>
+            {% endif %}
+        {% endif %}
     </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -21,8 +21,17 @@
     * {% endfor %} {% endif %} {% if not sensors and not categories %}
       no items to display. {% if user.is_superuser and not selected_category
       and "django.contrib.admin"|app_installed %}
 
       You can add sensors, categories and alerts by navigating to
       Administration_->_Detailed_Administration_->_Sensors {% endif %}
     * {% endif %}
+{% if sensors or categories %} {%if selected_category or alert_logs %}
+    * Alert log
+{% if alert_logs %}
+    * {% for alert in alert_logs %}
+    * [{{ alert.sensor.name }}] {{ alert.description }}
+    * {% endfor %}
+{% else %} There are no alerts for sensors in the {{ selected_category }}. {%
+endif %}
+{% endif %} {% endif %}
 {% endblock %}
```

### Comparing `NEMO-4.5.5/NEMO/apps/sensors/urls.py` & `NEMO-4.6.0/NEMO/apps/sensors/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/apps/sensors/views.py` & `NEMO-4.6.0/NEMO/apps/sensors/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from datetime import datetime, timedelta
 from math import floor
+from typing import Set
 
 from django.contrib.auth.decorators import login_required, permission_required
-from django.db.models import QuerySet
 from django.http import HttpResponse, JsonResponse
 from django.shortcuts import get_object_or_404, render
 from django.utils import timezone
 from django.utils.text import slugify
 from django.views.decorators.http import require_GET
 
 from NEMO.apps.sensors.customizations import SensorCustomization
 from NEMO.apps.sensors.models import Sensor, SensorAlertLog, SensorCategory, SensorData
 from NEMO.decorators import disable_session_expiry_refresh, postpone, staff_member_required
+from NEMO.typing import QuerySetType
 from NEMO.utilities import (
 	BasicDisplayTable,
 	beginning_of_the_day,
 	export_format_datetime,
 	extract_times,
 	format_datetime,
 )
@@ -25,19 +26,22 @@
 @require_GET
 def sensors(request, category_id=None):
 	selected_category = None
 	if category_id:
 		selected_category = get_object_or_404(SensorCategory, pk=category_id)
 	categories = SensorCategory.objects.filter(parent=category_id)
 	sensor_list = Sensor.objects.filter(visible=True, sensor_category_id=category_id).order_by("name")
-	return render(
-		request,
-		"sensors/sensors.html",
-		{"selected_category": selected_category, "categories": categories, "sensors": sensor_list},
-	)
+	alert_logs = SensorAlertLog.objects.filter(sensor__in=recursive_sensors(category_id))[:30]
+	dictionary = {
+		"selected_category": selected_category,
+		"categories": categories,
+		"sensors": sensor_list,
+		"alert_logs": alert_logs
+	}
+	return render(request, "sensors/sensors.html", dictionary)
 
 
 @login_required
 @require_GET
 def sensor_details(request, sensor_id, tab: str = None):
 	sensor = get_object_or_404(Sensor, pk=sensor_id)
 	chart_step = int(request.GET.get("chart_step", 1))
@@ -99,15 +103,15 @@
 def sensor_alert_log(request, sensor_id):
 	sensor = get_object_or_404(Sensor, pk=sensor_id)
 	sensor_data, start, end = get_sensor_data(request, sensor)
 	alert_log_entries = SensorAlertLog.objects.filter(sensor=sensor, time__gte=start, time__lte=end or timezone.now())
 	return render(request, "sensors/sensor_alerts.html", {"alerts": alert_log_entries})
 
 
-def get_sensor_data(request, sensor) -> (QuerySet, datetime, datetime):
+def get_sensor_data(request, sensor) -> (QuerySetType[SensorData], datetime, datetime):
 	start, end = extract_times(request.GET, start_required=False, end_required=False)
 	sensor_data = SensorData.objects.filter(sensor=sensor)
 	now = timezone.now().replace(second=0, microsecond=0).astimezone()
 	sensor_default_daterange = SensorCustomization.get("sensor_default_daterange")
 	if not start:
 		if sensor_default_daterange == "last_year":
 			start = now - timedelta(days=365)
@@ -118,14 +122,23 @@
 		elif sensor_default_daterange == "last_72hrs":
 			start = now - timedelta(days=3)
 		else:
 			start = now - timedelta(days=1)
 	return sensor_data.filter(created_date__gte=start, created_date__lte=(end or now)), start, end
 
 
+def recursive_sensors(category_id, sensor_list: Set[Sensor] = None) -> Set[Sensor]:
+	if sensor_list is None:
+		sensor_list = set()
+	sensor_list.update([sensor for sensor in Sensor.objects.filter(visible=True, sensor_category_id=category_id)])
+	for category in SensorCategory.objects.filter(parent=category_id):
+		sensor_list.update(recursive_sensors(category.id, sensor_list))
+	return sensor_list
+
+
 @login_required
 @require_GET
 @permission_required("NEMO.trigger_timed_services", raise_exception=True)
 def manage_sensor_data(request):
 	return do_manage_sensor_data()
```

### Comparing `NEMO-4.5.5/NEMO/context_processors.py` & `NEMO-4.6.0/NEMO/context_processors.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/decorators.py` & `NEMO-4.6.0/NEMO/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 staff_member_required = permission_decorator(lambda u: u.is_active and (u.is_staff or u.is_superuser))
 user_office_required = permission_decorator(lambda u: u.is_active and (u.is_user_office or u.is_superuser))
 accounting_required = permission_decorator(lambda u: u.is_active and (u.is_accounting_officer or u.is_superuser))
 staff_member_or_tool_superuser_required = permission_decorator(lambda u: u.is_active and (u.is_staff or u.is_tool_superuser or u.is_superuser))
 staff_member_or_user_office_required = permission_decorator(lambda u: u.is_active and (u.is_staff or u.is_user_office or u.is_superuser))
 accounting_or_user_office_or_manager_required = permission_decorator(lambda u: u.is_active and (u.is_accounting_officer or u.is_user_office or u.is_facility_manager or u.is_superuser))
 user_office_or_manager_required = permission_decorator(lambda u: u.is_active and (u.is_user_office or u.is_facility_manager or u.is_superuser))
-any_staff_required = permission_decorator(lambda u: u.is_active and (u.is_any_part_of_staff))
+any_staff_required = permission_decorator(lambda u: u.is_active and u.is_any_part_of_staff)
 accounting_or_manager_required = permission_decorator(lambda u: u.is_active and (u.is_accounting_officer or u.is_facility_manager or u.is_superuser))
 
 
 # Use this decorator annotation to replace another existing function. The first parameter of
 # the new function should be "old_function" which will contain the function being replaced
 # For example, to replace NEMO.views.policy.check_policy_to_save_reservation(arg1, arg2)
 # @replace_function("NEMO.views.policy.check_policy_to_save_reservation")
```

### Comparing `NEMO-4.5.5/NEMO/exceptions.py` & `NEMO-4.6.0/NEMO/exceptions.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/fields.py` & `NEMO-4.6.0/NEMO/fields.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/forms.py` & `NEMO-4.6.0/NEMO/forms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from datetime import datetime
 
+from django.contrib.admin.widgets import FilteredSelectMultiple
 from django.core.exceptions import NON_FIELD_ERRORS, ValidationError
 from django.forms import (
 	BaseForm,
 	BooleanField,
 	CharField,
 	ChoiceField,
 	DateField,
 	Form,
 	ImageField,
 	IntegerField,
 	ModelChoiceField,
 	ModelForm,
+	ModelMultipleChoiceField,
 )
 from django.forms.utils import ErrorDict, ErrorList
 from django.utils import timezone
 
 from NEMO.models import (
 	Account,
 	AdjustmentRequest,
@@ -31,14 +33,15 @@
 	SafetyIssue,
 	ScheduledOutage,
 	StaffAbsence,
 	Task,
 	TaskCategory,
 	TaskImages,
 	TemporaryPhysicalAccessRequest,
+	Tool,
 	User,
 	UserPreferences,
 )
 from NEMO.utilities import bootstrap_primary_color, format_datetime, quiet_int
 from NEMO.views.customization import UserRequestsCustomization
 
 
@@ -61,14 +64,35 @@
 
 
 class ProjectForm(ModelForm):
 	class Meta:
 		model = Project
 		exclude = ["only_allow_tools", "allow_consumable_withdrawals"]
 
+	principal_investigators = ModelMultipleChoiceField(
+		queryset=User.objects.all(),
+		required=False,
+		widget=FilteredSelectMultiple(verbose_name="Principal investigators", is_stacked=False),
+	)
+
+	def __init__(self, *args, **kwargs):
+		super().__init__(*args, **kwargs)
+		if self.instance.pk:
+			self.fields["principal_investigators"].initial = self.instance.manager_set.all()
+
+	def _save_m2m(self):
+		super()._save_m2m()
+		exclude = self._meta.exclude
+		fields = self._meta.fields
+		# Check for fields and exclude
+		if fields and "principal_investigators" not in fields or exclude and "principal_investigators" in exclude:
+			return
+		if "principal_investigators" in self.cleaned_data:
+			self.instance.manager_set.set(self.cleaned_data["principal_investigators"])
+
 
 class AccountForm(ModelForm):
 	class Meta:
 		model = Account
 		fields = "__all__"
 
 
@@ -355,14 +379,20 @@
 
 
 class UserPreferencesForm(ModelForm):
 	class Meta:
 		model = UserPreferences
 		fields = "__all__"
 
+	def __init__(self, *args, **kwargs):
+		super().__init__(*args, **kwargs)
+		self.fields["tool_freed_time_notifications"].queryset = Tool.objects.filter(visible=True, parent_tool__isnull=True)
+		self.fields["tool_adjustment_notifications"].queryset = Tool.objects.filter(visible=True, parent_tool__isnull=True)
+		self.fields["tool_task_notifications"].queryset = Tool.objects.filter(visible=True, parent_tool__isnull=True)
+
 	def clean_recurring_charges_reminder_days(self):
 		recurring_charges_reminder_days = self.cleaned_data["recurring_charges_reminder_days"]
 		try:
 			for reminder_days in recurring_charges_reminder_days.split(","):
 				try:
 					int(reminder_days)
 				except ValueError:
```

### Comparing `NEMO-4.5.5/NEMO/interlocks.py` & `NEMO-4.6.0/NEMO/interlocks.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/management/commands/send_email_usage_reminders.py` & `NEMO-4.6.0/NEMO/management/commands/send_email_usage_reminders.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/middleware.py` & `NEMO-4.6.0/NEMO/middleware.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0001_version_1_0_0.py` & `NEMO-4.6.0/NEMO/migrations/0001_version_1_0_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0002_version_1_0_0_squashed.py` & `NEMO-4.6.0/NEMO/migrations/0002_version_1_0_0_squashed.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0012_version_2_0_0_squashed.py` & `NEMO-4.6.0/NEMO/migrations/0012_version_2_0_0_squashed.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0020_version_3_0_0.py` & `NEMO-4.6.0/NEMO/migrations/0020_version_3_0_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0021_version_3_1_0.py` & `NEMO-4.6.0/NEMO/migrations/0021_version_3_1_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0022_version_3_3_0.py` & `NEMO-4.6.0/NEMO/migrations/0022_version_3_3_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0023_badgereader.py` & `NEMO-4.6.0/NEMO/migrations/0023_badgereader.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0024_contactinformation_user.py` & `NEMO-4.6.0/NEMO/migrations/0024_contactinformation_user.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0025_version_3_6_0.py` & `NEMO-4.6.0/NEMO/migrations/0025_version_3_6_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0026_version_3_7_0.py` & `NEMO-4.6.0/NEMO/migrations/0026_version_3_7_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0028_version_3_9_0.py` & `NEMO-4.6.0/NEMO/migrations/0028_version_3_9_0.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             name='value',
             field=models.FloatField(default=0, help_text='The current value of this counter'),
         ),
         migrations.CreateModel(
             name='ToolDocuments',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('document', models.FileField(null=True, blank=True, upload_to=NEMO.utilities.get_tool_document_filename, verbose_name='Document')),
+                ('document', models.FileField(null=True, blank=True, upload_to=NEMO.utilities.document_filename_upload, verbose_name='Document')),
                 ('uploaded_at', models.DateTimeField(auto_now_add=True)),
                 ('name', models.CharField(blank=True, help_text='The optional name to display for this document', max_length=200, null=True)),
                 ('url', models.CharField(blank=True, max_length=200, null=True, verbose_name='URL')),
                 ('tool', models.ForeignKey(on_delete=models.deletion.CASCADE, to='NEMO.Tool')),
             ],
             options={
                 'verbose_name_plural': 'Tool documents',
```

### Comparing `NEMO-4.5.5/NEMO/migrations/0030_version_3_9_2.py` & `NEMO-4.6.0/NEMO/migrations/0030_version_3_9_2.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0031_version_3_10_0.py` & `NEMO-4.6.0/NEMO/migrations/0031_version_3_10_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0032_version_3_11_0.py` & `NEMO-4.6.0/NEMO/migrations/0032_version_3_11_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0035_version_3_14_0.py` & `NEMO-4.6.0/NEMO/migrations/0035_version_3_14_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0036_version_3_15_0.py` & `NEMO-4.6.0/NEMO/migrations/0036_version_3_15_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0037_version_3_16_0.py` & `NEMO-4.6.0/NEMO/migrations/0037_version_3_16_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0038_version_4_0_0.py` & `NEMO-4.6.0/NEMO/migrations/0038_version_4_0_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0039_version_4_1_0.py` & `NEMO-4.6.0/NEMO/migrations/0039_version_4_1_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0040_version_4_2_0.py` & `NEMO-4.6.0/NEMO/migrations/0040_version_4_2_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0042_version_4_3_0.py` & `NEMO-4.6.0/NEMO/migrations/0042_version_4_3_0.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
                 'ordering': ['display_order', 'name'],
             },
         ),
         migrations.CreateModel(
             name='ProjectDocuments',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('document', models.FileField(blank=True, null=True, upload_to=NEMO.utilities.get_project_document_filename, verbose_name='Document')),
+                ('document', models.FileField(blank=True, null=True, upload_to=NEMO.utilities.document_filename_upload, verbose_name='Document')),
                 ('url', models.CharField(blank=True, max_length=200, null=True, verbose_name='URL')),
                 ('name', models.CharField(blank=True, help_text='The optional name to display for this document', max_length=200, null=True)),
                 ('uploaded_at', models.DateTimeField(auto_now_add=True)),
                 ('project', models.ForeignKey(related_name="project_documents", on_delete=django.db.models.deletion.CASCADE, to='NEMO.project')),
             ],
             options={
                 'verbose_name_plural': 'Project documents',
@@ -242,15 +242,15 @@
             name='discipline',
             field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to='NEMO.discipline'),
         ),
         migrations.CreateModel(
             name='UserDocuments',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('document', models.FileField(blank=True, null=True, upload_to=NEMO.utilities.get_user_document_filename, verbose_name='Document')),
+                ('document', models.FileField(blank=True, null=True, upload_to=NEMO.utilities.document_filename_upload, verbose_name='Document')),
                 ('url', models.CharField(blank=True, max_length=200, null=True, verbose_name='URL')),
                 ('name', models.CharField(blank=True, help_text='The optional name to display for this document', max_length=200, null=True)),
                 ('uploaded_at', models.DateTimeField(auto_now_add=True)),
                 ('user', models.ForeignKey(related_name="user_documents", on_delete=django.db.models.deletion.CASCADE, to='NEMO.user')),
             ],
             options={
                 'verbose_name_plural': 'User documents',
```

### Comparing `NEMO-4.5.5/NEMO/migrations/0043_version_4_3_2.py` & `NEMO-4.6.0/NEMO/migrations/0043_version_4_3_2.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0044_version_4_4_0.py` & `NEMO-4.6.0/NEMO/migrations/0044_version_4_4_0.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                 'abstract': False,
             },
         ),
         migrations.CreateModel(
             name='SafetyItemDocuments',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('document', models.FileField(blank=True, null=True, upload_to=NEMO.utilities.get_safety_document_filename, verbose_name='Document')),
+                ('document', models.FileField(blank=True, null=True, upload_to=NEMO.utilities.document_filename_upload, verbose_name='Document')),
                 ('url', models.CharField(blank=True, max_length=200, null=True, verbose_name='URL')),
                 ('name', models.CharField(blank=True, help_text='The optional name to display for this document', max_length=200, null=True)),
                 ('uploaded_at', models.DateTimeField(auto_now_add=True)),
                 ('safety_item', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='NEMO.safetyitem')),
             ],
             options={
                 'verbose_name_plural': 'Safety item documents',
```

### Comparing `NEMO-4.5.5/NEMO/migrations/0045_version_4_5_0.py` & `NEMO-4.6.0/NEMO/migrations/0045_version_4_5_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations/0045_version_4_5_5.py` & `NEMO-4.6.0/NEMO/migrations/0045_version_4_5_5.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/migrations_utils.py` & `NEMO-4.6.0/NEMO/migrations_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,16 @@
         now = timezone.now()
         story = News()
         story.title = f"What's new in NEMO {version}?"
         content = f"Thank you for updating to NEMO {version}.\n"
         if extra_content:
             content += extra_content + "\n"
         content += (
-            f"\nClick on the following links to consult the <a href='https://github.com/usnistgov/NEMO/releases/tag/{version}' target='_blank'>Release Notes</a> "
-            f"and the <a href='https://www.nist.gov/document/nemofeaturemanualpdf' target='_blank'>Feature manual</a>"
+            f"\nClick on the following links to consult the <a href='https://github.com/usnistgov/NEMO/releases/tag/{version}' target='_blank'>NEMO {version} Release Notes</a> "
+            f"and the <a href='https://www.nist.gov/document/nemofeaturemanualpdf' target='_blank'>NEMO {version} Feature manual</a>"
         )
         content = f"Originally published on {migration_format_datetime(now)} by NEMO:\n" + content.strip()
         story.original_content = content
         story.created = now
         story.all_content = content
         story.last_updated = now
         story.last_update_content = content
```

### Comparing `NEMO-4.5.5/NEMO/model_tree.py` & `NEMO-4.6.0/NEMO/model_tree.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/models.py` & `NEMO-4.6.0/NEMO/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from enum import Enum
 from html import escape
 from json import loads
 from logging import getLogger
 from re import match
 from typing import List, Optional, Set, Union
 
-from dateutil import rrule
 from django.conf import settings
 from django.contrib import auth
 from django.contrib.auth.models import BaseUserManager, Group, Permission, PermissionsMixin
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import NON_FIELD_ERRORS, ValidationError
 from django.core.validators import MinValueValidator
@@ -31,38 +30,35 @@
 from django.utils import timezone
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 from mptt.fields import TreeForeignKey
 from mptt.models import MPTTModel
 
 from NEMO import fields
-from NEMO.mixins import BillableItemMixin, CalendarDisplayMixin
+from NEMO.mixins import BillableItemMixin, CalendarDisplayMixin, RecurrenceMixin
+from NEMO.typing import QuerySetType
 from NEMO.utilities import (
 	EmailCategory,
 	RecurrenceFrequency,
 	as_timezone,
-	beginning_of_the_day,
 	bootstrap_primary_color,
 	distinct_qs_value_list,
+	document_filename_upload,
 	format_daterange,
 	format_datetime,
 	get_chemical_document_filename,
+	get_full_url,
 	get_hazard_logo_filename,
-	get_project_document_filename,
-	get_recurring_rule,
-	get_safety_document_filename,
 	get_task_image_filename,
-	get_tool_document_filename,
 	get_tool_image_filename,
-	get_user_document_filename,
 	render_email_template,
 	send_mail,
+	supported_embedded_extensions,
 )
-from NEMO.views.constants import ADDITIONAL_INFORMATION_MAXIMUM_LENGTH
-from NEMO.views.documents import supported_embedded_extensions
+from NEMO.views.constants import ADDITIONAL_INFORMATION_MAXIMUM_LENGTH, CHAR_FIELD_MAXIMUM_LENGTH
 from NEMO.widgets.configuration_editor import ConfigurationEditor
 
 models_logger = getLogger(__name__)
 
 
 class BaseQuerySet(models.query.QuerySet):
 
@@ -143,14 +139,81 @@
 		abstract = True
 		ordering = ["display_order", "name"]
 
 	def __str__(self):
 		return str(self.name)
 
 
+class BaseDocumentModel(BaseModel):
+	document = models.FileField(null=True, blank=True, upload_to=document_filename_upload, verbose_name='Document')
+	url = models.CharField(null=True, blank=True, max_length=200, verbose_name='URL')
+	name = models.CharField(null=True, blank=True, max_length=200, help_text="The optional name to display for this document")
+	uploaded_at = models.DateTimeField(auto_now_add=True)
+
+	def get_filename_upload(self, filename):
+		raise NotImplementedError("subclasses must provide a filename for upload")
+
+	def filename(self):
+		return self.name if self.name else os.path.basename(self.document.name) if self.document else self.url.rsplit('/', 1)[-1] if self.url else ""
+
+	def link(self):
+		return self.document.url if self.document else self.url
+
+	def full_link(self, request=None):
+		return get_full_url(self.document.url, request) if self.document else self.url
+
+	def can_be_embedded(self):
+		return any([self.link().lower().endswith(ext) for ext in supported_embedded_extensions])
+
+	def __str__(self):
+		return self.filename()
+
+	def clean(self):
+		if not self.document and not self.url:
+			raise ValidationError({'document': 'Either document or URL should be provided.'})
+		elif self.document and self.url:
+			raise ValidationError({'document': 'Choose either document or URL but not both.'})
+
+	class Meta:
+		ordering = ['-uploaded_at']
+		abstract = True
+
+
+# These two auto-delete documents from filesystem when they are unneeded:
+@receiver(models.signals.post_delete)
+def auto_delete_file_on_document_delete(sender, instance: BaseDocumentModel, **kwargs):
+	if not issubclass(sender, BaseDocumentModel):
+		return
+	"""	Deletes file from filesystem when corresponding `SafetyItemDocuments` object is deleted.	"""
+	if instance.document:
+		if os.path.isfile(instance.document.path):
+			os.remove(instance.document.path)
+
+
+@receiver(models.signals.pre_save)
+def auto_delete_file_on_document_change(sender, instance: BaseDocumentModel, **kwargs):
+	if not issubclass(sender, BaseDocumentModel):
+		return
+	"""	Deletes old file from filesystem when corresponding `SafetyItemDocuments` object is updated with new file. """
+	if not instance.pk:
+		return False
+
+	model_class = type(instance)
+
+	try:
+		old_file = model_class.objects.get(pk=instance.pk).document
+	except model_class.DoesNotExist:
+		return False
+
+	new_file = instance.document
+	if old_file and not old_file == new_file:
+		if os.path.isfile(old_file.path):
+			os.remove(old_file.path)
+
+
 class ReservationItemType(Enum):
 	TOOL = 'tool'
 	AREA = 'area'
 	NONE = ''
 
 	def get_object_class(self):
 		if self == ReservationItemType.AREA:
@@ -228,14 +291,19 @@
 	email_send_access_expiration_emails = models.PositiveIntegerField(default=EmailNotificationType.BOTH_EMAILS, choices=EmailNotificationType.on_choices(), help_text="Access expiration reminders")
 	email_send_tool_qualification_expiration_emails = models.PositiveIntegerField(default=EmailNotificationType.BOTH_EMAILS, choices=EmailNotificationType.on_choices(), help_text="Tool qualification expiration reminders")
 	email_send_usage_reminders = models.PositiveIntegerField(default=EmailNotificationType.BOTH_EMAILS, choices=EmailNotificationType.Choices, help_text="Usage reminders")
 	email_send_reservation_reminders = models.PositiveIntegerField(default=EmailNotificationType.BOTH_EMAILS, choices=EmailNotificationType.Choices, help_text="Reservation reminders")
 	email_send_reservation_ending_reminders = models.PositiveIntegerField(default=EmailNotificationType.BOTH_EMAILS, choices=EmailNotificationType.Choices, help_text="Reservation ending reminders")
 	recurring_charges_reminder_days = models.CharField(null=True, blank=True, default="60,7", max_length=200, help_text="The number of days to send a reminder before a recurring charge is due. A comma-separated list can be used for multiple reminders.")
 	email_send_recurring_charges_reminder_emails = models.PositiveIntegerField(default=EmailNotificationType.BOTH_EMAILS, choices=EmailNotificationType.Choices, help_text="Recurring charges reminders")
+	tool_freed_time_notifications = models.ManyToManyField("Tool", blank=True, help_text="Tools to receive notification when reservation time is freed.")
+	tool_freed_time_notifications_min_time = models.PositiveIntegerField(default=120, help_text="Minimum amount of minutes freed to receive a notification.")
+	tool_freed_time_notifications_max_future_days = models.PositiveIntegerField(default=7, help_text="Maximum number of days in the future to receive a notification for.")
+	tool_adjustment_notifications = models.ManyToManyField("Tool", related_name="+", blank=True, help_text="Tools to see/receive adjustment notifications for. If empty all notifications will be received.")
+	tool_task_notifications = models.ManyToManyField("Tool", related_name="+", blank=True, help_text="Tools to see maintenance records and receive task notifications for. If empty all notifications will be received.")
 
 	def get_recurring_charges_days(self) -> List[int]:
 		return [int(days) for days in self.recurring_charges_reminder_days.split(",") if self.recurring_charges_reminder_days]
 
 	def __str__(self):
 		return f"{self.user.username}'s preferences"
 
@@ -387,15 +455,15 @@
 			raise ValidationError({"end_time": "The end time must be later than the start time"})
 
 	class Meta:
 		ordering = ['-creation_time']
 
 
 class Closure(BaseModel):
-	name = models.CharField(max_length=255, help_text="The name of this closure, that will be displayed as the policy problem and alert (if applicable).")
+	name = models.CharField(max_length=CHAR_FIELD_MAXIMUM_LENGTH, help_text="The name of this closure, that will be displayed as the policy problem and alert (if applicable).")
 	alert_days_before = models.PositiveIntegerField(null=True, blank=True, help_text="Enter the number of days before the closure when an alert should automatically be created. Leave blank for no alert.")
 	alert_template = models.TextField(null=True, blank=True, help_text=mark_safe("The template to create the alert with. The following variables are provided (when applicable): <b>name</b>, <b>start_time</b>, <b>end_time</b>, <b>areas</b>."))
 	notify_managers_last_occurrence = models.BooleanField(default=True, help_text="Check this box to notify facility managers on the last occurrence of this closure.")
 	staff_absent = models.BooleanField(default=True, help_text="Check this box and all staff members will be marked absent during this closure in staff status.")
 	physical_access_levels = models.ManyToManyField('PhysicalAccessLevel', blank=True, help_text="Select access levels this closure applies to.")
 
 	def __str__(self):
@@ -484,15 +552,15 @@
 	# Permissions
 	is_active = models.BooleanField('active', default=True, help_text='Designates whether this user can log in. Unselect this instead of deleting accounts.')
 	is_staff = models.BooleanField('staff', default=False, help_text='Designates this user as technical staff. Technical staff can start remote projects, check maintenance, change configuration, train users etc.')
 	is_user_office = models.BooleanField('user office', default=False, help_text='Designates this user as part of the User Office. User Office staff can create and manage users and projects, charge supplies, check usage etc.')
 	is_accounting_officer = models.BooleanField('accounting officer', default=False, help_text='Designates this user as Accounting officer. Accounting officers can manage projects, view user details, and check usage/billing.')
 	is_service_personnel = models.BooleanField('service personnel', default=False, help_text='Designates this user as service personnel. Service personnel can operate qualified tools without a reservation even when they are shutdown or during an outage and can access authorized areas without a reservation.')
 	is_technician = models.BooleanField('technician', default=False, help_text='Specifies how to bill staff time for this user. When checked, customers are billed at technician rates.')
-	is_facility_manager = models.BooleanField('facility manager', default=False, help_text='Designates this user as facility manager. Facility managers receive updates on all reported problems in the facility and can also review access requests.')
+	is_facility_manager = models.BooleanField('facility manager', default=False, help_text='Designates this user as facility manager. Facility managers receive updates on all reported problems in the facility and also review access and adjustment requests.')
 	is_superuser = models.BooleanField('administrator', default=False, help_text='Designates that this user has all permissions without explicitly assigning them.')
 	training_required = models.BooleanField('facility rules tutorial required', default=True, help_text='When selected, the user is blocked from all reservation and tool usage capabilities.')
 	groups = models.ManyToManyField(Group, blank=True, help_text='The groups this user belongs to. A user will get all permissions granted to each of his/her group.')
 	user_permissions = models.ManyToManyField(Permission, blank=True, help_text='Specific permissions for this user.')
 
 	# Important dates
 	date_joined = models.DateTimeField(default=timezone.now)
@@ -711,65 +779,25 @@
 			("kiosk", "Kiosk services"),
 		)
 
 	def __str__(self):
 		return self.get_full_name()
 
 
-class UserDocuments(BaseModel):
+class UserDocuments(BaseDocumentModel):
 	user = models.ForeignKey(User, related_name="user_documents", on_delete=models.CASCADE)
-	document = models.FileField(null=True, blank=True, upload_to=get_user_document_filename, verbose_name='Document')
-	url = models.CharField(null=True, blank=True, max_length=200, verbose_name='URL')
-	name = models.CharField(null=True, blank=True, max_length=200, help_text="The optional name to display for this document")
-	uploaded_at = models.DateTimeField(auto_now_add=True)
 
-	def filename(self):
-		return self.name if self.name else os.path.basename(self.document.name) if self.document else self.url.rsplit('/', 1)[-1]
+	def get_filename_upload(self, filename):
+		from django.template.defaultfilters import slugify
 
-	def link(self):
-		return self.document.url if self.document else self.url
+		username = slugify(self.user.username)
+		return f"user_documents/{username}/{filename}"
 
-	def __str__(self):
-		return self.filename()
-
-	def clean(self):
-		if not self.document and not self.url:
-			raise ValidationError({'document': 'Either document or URL should be provided.'})
-		elif self.document and self.url:
-			raise ValidationError({'document': 'Choose either document or URL but not both.'})
-
-	class Meta:
+	class Meta(BaseDocumentModel.Meta):
 		verbose_name_plural = "User documents"
-		ordering = ['-uploaded_at']
-
-
-# These two auto-delete project documents from filesystem when they are unneeded:
-@receiver(models.signals.post_delete, sender=UserDocuments)
-def auto_delete_file_on_user_document_delete(sender, instance: UserDocuments, **kwargs):
-	"""	Deletes file from filesystem when corresponding `UserDocuments` object is deleted.	"""
-	if instance.document:
-		if os.path.isfile(instance.document.path):
-			os.remove(instance.document.path)
-
-
-@receiver(models.signals.pre_save, sender=UserDocuments)
-def auto_delete_file_on_user_document_change(sender, instance: UserDocuments, **kwargs):
-	"""	Deletes old file from filesystem when corresponding `UserDocuments` object is updated with new file. """
-	if not instance.pk:
-		return False
-
-	try:
-		old_file = UserDocuments.objects.get(pk=instance.pk).document
-	except UserDocuments.DoesNotExist:
-		return False
-
-	new_file = instance.document
-	if not old_file == new_file:
-		if os.path.isfile(old_file.path):
-			os.remove(old_file.path)
 
 
 class Tool(SerializationByNameModel):
 	name = models.CharField(max_length=100, unique=True)
 	parent_tool = models.ForeignKey('Tool', related_name="tool_children_set", null=True, blank=True, help_text='Select a parent tool to allow alternate usage', on_delete=models.CASCADE)
 	visible = models.BooleanField(default=True, help_text="Specifies whether this tool is visible to users.")
 	_description = models.TextField(db_column="description", null=True, blank=True, help_text="HTML syntax could be used")
@@ -781,14 +809,15 @@
 	_primary_owner = models.ForeignKey(User, db_column="primary_owner_id", null=True, blank=True, related_name="primary_tool_owner", help_text="The staff member who is responsible for administration of this tool.", on_delete=models.PROTECT)
 	_backup_owners = models.ManyToManyField(User, db_table='NEMO_tool_backup_owners', blank=True, related_name="backup_for_tools", help_text="Alternate staff members who are responsible for administration of this tool when the primary owner is unavailable.")
 	_superusers = models.ManyToManyField(User, db_table='NEMO_tool_superusers', blank=True, related_name="superuser_for_tools", help_text="Superusers who can train users on this tool.")
 	_location = models.CharField(db_column="location", null=True, blank=True, max_length=100)
 	_phone_number = models.CharField(db_column="phone_number", null=True, blank=True, max_length=100)
 	_notification_email_address = models.EmailField(db_column="notification_email_address", blank=True, null=True, help_text="Messages that relate to this tool (such as comments, problems, and shutdowns) will be forwarded to this email address. This can be a normal email address or a mailing list address.")
 	_interlock = models.OneToOneField('Interlock', db_column="interlock_id", blank=True, null=True, on_delete=models.SET_NULL)
+	_qualifications_never_expire = models.BooleanField(default=False, db_column="qualifications_never_expire", help_text="Check this box if qualifications for this tool should never expire (even if the tool qualification expiration feature is enabled).")
 	# Policy fields:
 	_requires_area_access = TreeForeignKey('Area', db_column="requires_area_access_id", null=True, blank=True, help_text="Indicates that this tool is physically located in a billable area and requires an active area access record in order to be operated.", on_delete=models.PROTECT)
 	_grant_physical_access_level_upon_qualification = models.ForeignKey('PhysicalAccessLevel', db_column="grant_physical_access_level_upon_qualification_id", null=True, blank=True, help_text="The designated physical access level is granted to the user upon qualification for this tool.", on_delete=models.PROTECT)
 	_grant_badge_reader_access_upon_qualification = models.CharField(db_column="grant_badge_reader_access_upon_qualification", max_length=100, null=True, blank=True, help_text="Badge reader access is granted to the user upon qualification for this tool.")
 	_reservation_horizon = models.PositiveIntegerField(db_column="reservation_horizon", default=14, null=True, blank=True, help_text="Users may create reservations this many days in advance. Leave this field blank to indicate that no reservation horizon exists for this tool.")
 	_minimum_usage_block_time = models.PositiveIntegerField(db_column="minimum_usage_block_time", null=True, blank=True, help_text="The minimum amount of time (in minutes) that a user must reserve this tool for a single reservation. Leave this field blank to indicate that no minimum usage block time exists for this tool.")
 	_maximum_usage_block_time = models.PositiveIntegerField(db_column="maximum_usage_block_time", null=True, blank=True, help_text="The maximum amount of time (in minutes) that a user may reserve this tool for a single reservation. Leave this field blank to indicate that no maximum usage block time exists for this tool.")
@@ -812,14 +841,23 @@
 
 	@category.setter
 	def category(self, value):
 		self.raise_setter_error_if_child_tool("category")
 		self._category = value
 
 	@property
+	def qualifications_never_expire(self):
+		return self.parent_tool.qualifications_never_expire if self.is_child_tool() else self._qualifications_never_expire
+
+	@qualifications_never_expire.setter
+	def qualifications_never_expire(self, value):
+		self.raise_setter_error_if_child_tool("qualifications_never_expire")
+		self._qualifications_never_expire = value
+
+	@property
 	def description(self):
 		return self.parent_tool.description if self.is_child_tool() else self._description
 
 	@description.setter
 	def description(self, value):
 		self.raise_setter_error_if_child_tool("description")
 		self._description = value
@@ -857,24 +895,24 @@
 
 	@primary_owner.setter
 	def primary_owner(self, value):
 		self.raise_setter_error_if_child_tool("primary_owner")
 		self._primary_owner = value
 
 	@property
-	def backup_owners(self) -> QuerySet:
+	def backup_owners(self) -> QuerySetType[User]:
 		return self.parent_tool.backup_owners if self.is_child_tool() else self._backup_owners
 
 	@backup_owners.setter
 	def backup_owners(self, value):
 		self.raise_setter_error_if_child_tool("backup_owners")
 		self._backup_owners = value
 
 	@property
-	def superusers(self) -> QuerySet:
+	def superusers(self) -> QuerySetType[User]:
 		return self.parent_tool.superusers if self.is_child_tool() else self._superusers
 
 	@superusers.setter
 	def superusers(self, value):
 		self.raise_setter_error_if_child_tool("superusers")
 		self._superusers = value
 
@@ -1299,65 +1337,25 @@
 		if self.parent_tool_id:
 			# in case of alternate tool, recreate a new tool with only parent_tool and name (never visible)
 			fresh_tool = Tool(id=self.id, parent_tool=self.parent_tool, name=self.name, visible=False)
 			self.__dict__.update(fresh_tool.__dict__)
 		super().save(force_insert, force_update, using, update_fields)
 
 
-class ToolDocuments(BaseModel):
+class ToolDocuments(BaseDocumentModel):
 	tool = models.ForeignKey(Tool, on_delete=models.CASCADE)
-	document = models.FileField(null=True, blank=True, upload_to=get_tool_document_filename, verbose_name='Document')
-	url = models.CharField(null=True, blank=True, max_length=200, verbose_name='URL')
-	name = models.CharField(null=True, blank=True, max_length=200, help_text="The optional name to display for this document")
-	uploaded_at = models.DateTimeField(auto_now_add=True)
-
-	def filename(self):
-		return self.name if self.name else os.path.basename(self.document.name) if self.document else self.url.rsplit('/', 1)[-1]
-
-	def link(self):
-		return self.document.url if self.document else self.url
 
-	def __str__(self):
-		return self.filename()
+	def get_filename_upload(self, filename):
+		from django.template.defaultfilters import slugify
 
-	def clean(self):
-		if not self.document and not self.url:
-			raise ValidationError({'document': 'Either document or URL should be provided.'})
-		elif self.document and self.url:
-			raise ValidationError({'document': 'Choose either document or URL but not both.'})
+		tool_name = slugify(self.tool.name)
+		return f"tool_documents/{tool_name}/{filename}"
 
-	class Meta:
+	class Meta(BaseDocumentModel.Meta):
 		verbose_name_plural = "Tool documents"
-		ordering = ['-uploaded_at']
-
-
-# These two auto-delete tool documents from filesystem when they are unneeded:
-@receiver(models.signals.post_delete, sender=ToolDocuments)
-def auto_delete_file_on_tool_document_delete(sender, instance: ToolDocuments, **kwargs):
-	"""	Deletes file from filesystem when corresponding `ToolDocuments` object is deleted.	"""
-	if instance.document:
-		if os.path.isfile(instance.document.path):
-			os.remove(instance.document.path)
-
-
-@receiver(models.signals.pre_save, sender=ToolDocuments)
-def auto_delete_file_on_tool_document_change(sender, instance: ToolDocuments, **kwargs):
-	"""	Deletes old file from filesystem when corresponding `ToolDocuments` object is updated with new file. """
-	if not instance.pk:
-		return False
-
-	try:
-		old_file = ToolDocuments.objects.get(pk=instance.pk).document
-	except ToolDocuments.DoesNotExist:
-		return False
-
-	new_file = instance.document
-	if not old_file == new_file:
-		if os.path.isfile(old_file.path):
-			os.remove(old_file.path)
 
 
 class ToolQualificationGroup(SerializationByNameModel):
 	name = models.CharField(max_length=200, unique=True, help_text="The name of this tool group")
 	tools = models.ManyToManyField(Tool, blank=False)
 
 	def __str__(self):
@@ -1664,65 +1662,25 @@
 	class Meta:
 		ordering = ["name"]
 
 	def __str__(self):
 		return str(self.name)
 
 
-class ProjectDocuments(BaseModel):
+class ProjectDocuments(BaseDocumentModel):
 	project = models.ForeignKey(Project, related_name="project_documents", on_delete=models.CASCADE)
-	document = models.FileField(null=True, blank=True, upload_to=get_project_document_filename, verbose_name='Document')
-	url = models.CharField(null=True, blank=True, max_length=200, verbose_name='URL')
-	name = models.CharField(null=True, blank=True, max_length=200, help_text="The optional name to display for this document")
-	uploaded_at = models.DateTimeField(auto_now_add=True)
 
-	def filename(self):
-		return self.name if self.name else os.path.basename(self.document.name) if self.document else self.url.rsplit('/', 1)[-1]
+	def get_filename_upload(self, filename):
+		from django.template.defaultfilters import slugify
 
-	def link(self):
-		return self.document.url if self.document else self.url
-
-	def __str__(self):
-		return self.filename()
-
-	def clean(self):
-		if not self.document and not self.url:
-			raise ValidationError({'document': 'Either document or URL should be provided.'})
-		elif self.document and self.url:
-			raise ValidationError({'document': 'Choose either document or URL but not both.'})
+		project_name = slugify(self.project.name)
+		return f"project_documents/{project_name}/{filename}"
 
-	class Meta:
+	class Meta(BaseDocumentModel.Meta):
 		verbose_name_plural = "Project documents"
-		ordering = ['-uploaded_at']
-
-
-# These two auto-delete project documents from filesystem when they are unneeded:
-@receiver(models.signals.post_delete, sender=ProjectDocuments)
-def auto_delete_file_on_project_document_delete(sender, instance: ProjectDocuments, **kwargs):
-	"""	Deletes file from filesystem when corresponding `ProjectDocuments` object is deleted.	"""
-	if instance.document:
-		if os.path.isfile(instance.document.path):
-			os.remove(instance.document.path)
-
-
-@receiver(models.signals.pre_save, sender=ProjectDocuments)
-def auto_delete_file_on_project_document_change(sender, instance: ProjectDocuments, **kwargs):
-	"""	Deletes old file from filesystem when corresponding `ProjectDocuments` object is updated with new file. """
-	if not instance.pk:
-		return False
-
-	try:
-		old_file = ProjectDocuments.objects.get(pk=instance.pk).document
-	except ProjectDocuments.DoesNotExist:
-		return False
-
-	new_file = instance.document
-	if not old_file == new_file:
-		if os.path.isfile(old_file.path):
-			os.remove(old_file.path)
 
 
 def pre_delete_entity(sender, instance, using, **kwargs):
 	""" Remove activity history and membership history when an account, project, tool, or user is deleted. """
 	content_type = ContentType.objects.get_for_model(sender)
 	ActivityHistory.objects.filter(object_id=instance.id, content_type=content_type).delete()
 	MembershipHistory.objects.filter(parent_object_id=instance.id, parent_content_type=content_type).delete()
@@ -1923,14 +1881,15 @@
 class ConsumableWithdraw(BaseModel, BillableItemMixin):
 	customer = models.ForeignKey(User, related_name="consumable_user", help_text="The user who will use the consumable item.", on_delete=models.CASCADE)
 	merchant = models.ForeignKey(User, related_name="consumable_merchant", help_text="The staff member that performed the withdraw.", on_delete=models.CASCADE)
 	consumable = models.ForeignKey(Consumable, on_delete=models.CASCADE)
 	quantity = models.PositiveIntegerField()
 	project = models.ForeignKey(Project, help_text="The withdraw will be billed to this project.", on_delete=models.CASCADE)
 	date = models.DateTimeField(default=timezone.now, help_text="The date and time when the user withdrew the consumable.")
+	tool_usage = models.BooleanField(default=False, help_text="Whether this withdraw is from tool usage")
 	validated = models.BooleanField(default=False)
 	validated_by = models.ForeignKey(User, null=True, blank=True, related_name="consumable_withdrawal_validated_set", on_delete=models.CASCADE)
 
 	class Meta:
 		ordering = ['-date']
 
 	def clean(self):
@@ -1950,25 +1909,25 @@
 		if self.consumable_id:
 			if not self.consumable.reusable and self.quantity > self.consumable.quantity:
 				errors[NON_FIELD_ERRORS] = f'There are not enough "{self.consumable.name}". (The current quantity in stock is {str(self.consumable.quantity)}). Please order more as soon as possible.'
 		if self.customer_id and self.consumable_id and self.project_id:
 			from NEMO.exceptions import ProjectChargeException
 			from NEMO.policy import policy_class as policy
 			try:
-				policy.check_billing_to_project(self.project, self.customer, self.consumable)
+				policy.check_billing_to_project(self.project, self.customer, self.consumable, self)
 			except ProjectChargeException as e:
 				errors["project"] = e.msg
 		if errors:
 			raise ValidationError(errors)
 
 	def __str__(self):
 		return str(self.id)
 
 
-class RecurringConsumableCharge(BaseModel):
+class RecurringConsumableCharge(BaseModel, RecurrenceMixin):
 	name = models.CharField(max_length=200, help_text="The name/identifier for this recurring charge.")
 	customer = models.ForeignKey(User, null=True, blank=True, related_name="recurring_charge_customer", help_text="The user who will be charged.", on_delete=models.CASCADE)
 	consumable = models.ForeignKey(Consumable, on_delete=models.CASCADE)
 	quantity = models.PositiveIntegerField(default=1, validators=[MinValueValidator(1)], help_text="The number of consumables to charge.")
 	project = models.ForeignKey(Project, null=True, blank=True, help_text="The project to bill.", on_delete=models.CASCADE)
 	last_charge = models.DateTimeField(null=True, blank=True, help_text="The date and time when the user was last charged.")
 	# Recurring schedule. TODO: think about extracting into its own model if used anywhere else
@@ -1980,22 +1939,16 @@
 	# Audit
 	last_updated = models.DateTimeField(help_text="The time this charge was last modified.")
 	last_updated_by = models.ForeignKey("User", related_name="recurring_charge_updated", help_text="The user who last modified this charge (and will be used as merchant on the charge).", on_delete=models.PROTECT)
 
 	class Meta:
 		ordering = ["name"]
 
-	@property
-	def get_rec_frequency_enum(self):
-		return RecurrenceFrequency(self.rec_frequency)
-
 	def next_charge(self, inc=False) -> datetime:
-		today = beginning_of_the_day(datetime.datetime.now(), in_local_timezone=False)
-		recurrence = self.get_recurrence()
-		return recurrence.after(today, inc=inc) if recurrence else None
+		return self.next_recurrence(inc)
 
 	def invalid_customer(self):
 		from NEMO.views.customization import RecurringChargesCustomization
 		skip_customer = RecurringChargesCustomization.get_bool("recurring_charges_skip_customer_validation")
 		if self.customer and not skip_customer:
 			if not self.customer.is_active:
 				return "This user is inactive"
@@ -2010,42 +1963,14 @@
 				return "The account for this project is inactive"
 			if not self.project.allow_consumable_withdrawals:
 				return "This project doesn't allow consumable charges"
 		if self.customer and self.project:
 			if self.project not in self.customer.active_projects():
 				return "The user does not belong to this project"
 
-	def get_recurrence(self) -> rrule:
-		if self.rec_start and self.rec_frequency:
-			return get_recurring_rule(self.rec_start, self.get_rec_frequency_enum, self.rec_until, self.rec_interval, self.rec_count)
-
-	def get_recurrence_interval_display(self) -> str:
-		if not self.rec_start or not self.rec_frequency:
-			return ""
-		interval = f"{self.rec_interval} " if self.rec_interval != 1 else ""
-		f_enum = self.get_rec_frequency_enum
-		frequency = f"{f_enum.display_text}s" if self.rec_interval != 1 else f_enum.display_text
-		return f"Every {interval}{frequency}"
-
-	def get_recurrence_display(self) -> str:
-		rec_display = ""
-		if self.rec_start and self.rec_frequency:
-			start = f", starting {format_datetime(self.rec_start, 'SHORT_DATE_FORMAT')}"
-			end = ""
-			if self.rec_until or self.rec_count:
-				end = f" and ending "
-				if self.rec_until:
-					end += f"on {format_datetime(self.rec_until, 'SHORT_DATE_FORMAT')}"
-				elif self.rec_count:
-					end += f"after {self.rec_count} iterations" if self.rec_count != 1 else f"after one time"
-					if self.get_recurrence():
-						end += f" on {format_datetime(list(self.get_recurrence())[-1], 'SHORT_DATE_FORMAT')}"
-			return f"{self.get_recurrence_interval_display()}{start}{end}"
-		return rec_display
-
 	def charge(self):
 		# Cannot charge twice the same day
 		if self.last_charge and as_timezone(self.last_charge).date() == datetime.date.today():
 			return
 		else:
 			from NEMO.views.consumables import make_withdrawal
 			self.full_clean()
@@ -2065,20 +1990,15 @@
 	def clean(self):
 		if not self.is_empty():
 			errors = {}
 			if not self.customer:
 				errors["customer"] = "This field is required."
 			if not self.project:
 				errors["project"] = "This field is required."
-			if not self.rec_start:
-				errors["rec_start"] = "This field is required."
-			if not self.rec_frequency:
-				errors["rec_frequency"] = "This field is required."
-			if self.rec_until and self.rec_count:
-				errors[NON_FIELD_ERRORS] = "'count' and 'until' cannot be used at the same time."
+			errors.update(self.clean_recurrence())
 			# Validate needed fields are present
 			if errors:
 				raise ValidationError(errors)
 			# Validate if we have everything to charge
 			from NEMO.forms import ConsumableWithdrawForm
 			from NEMO.views.customization import RecurringChargesCustomization
 			skip_customer = RecurringChargesCustomization.get_bool("recurring_charges_skip_customer_validation")
@@ -2527,68 +2447,25 @@
 	description = models.TextField(null=True, blank=True, help_text="The description for this safety item. HTML can be used.")
 	category = models.ForeignKey(SafetyCategory, null=True, blank=True, help_text="The category for this safety item.", on_delete=models.SET_NULL)
 
 	def __str__(self):
 		return self.name
 
 
-class SafetyItemDocuments(BaseModel):
+class SafetyItemDocuments(BaseDocumentModel):
 	safety_item = models.ForeignKey(SafetyItem, on_delete=models.CASCADE)
-	document = models.FileField(null=True, blank=True, upload_to=get_safety_document_filename, verbose_name='Document')
-	url = models.CharField(null=True, blank=True, max_length=200, verbose_name='URL')
-	name = models.CharField(null=True, blank=True, max_length=200, help_text="The optional name to display for this document")
-	uploaded_at = models.DateTimeField(auto_now_add=True)
 
-	def filename(self):
-		return self.name if self.name else os.path.basename(self.document.name) if self.document else self.url.rsplit('/', 1)[-1] if self.url else ""
-
-	def link(self):
-		return self.document.url if self.document else self.url
-
-	def can_be_embedded(self):
-		return any([self.link().lower().endswith(ext) for ext in supported_embedded_extensions])
+	def get_filename_upload(self, filename):
+		from django.template.defaultfilters import slugify
 
-	def __str__(self):
-		return self.filename()
+		item_name = slugify(self.safety_item.name)
+		return f"safety_item/{item_name}/{filename}"
 
-	def clean(self):
-		if not self.document and not self.url:
-			raise ValidationError({'document': 'Either document or URL should be provided.'})
-		elif self.document and self.url:
-			raise ValidationError({'document': 'Choose either document or URL but not both.'})
-
-	class Meta:
+	class Meta(BaseDocumentModel.Meta):
 		verbose_name_plural = "Safety item documents"
-		ordering = ['-uploaded_at']
-
-
-# These two auto-delete safety item documents from filesystem when they are unneeded:
-@receiver(models.signals.post_delete, sender=SafetyItemDocuments)
-def auto_delete_file_on_safety_item_document_delete(sender, instance: SafetyItemDocuments, **kwargs):
-	"""	Deletes file from filesystem when corresponding `SafetyItemDocuments` object is deleted.	"""
-	if instance.document:
-		if os.path.isfile(instance.document.path):
-			os.remove(instance.document.path)
-
-
-@receiver(models.signals.pre_save, sender=SafetyItemDocuments)
-def auto_delete_file_on_safety_item_document_change(sender, instance: SafetyItemDocuments, **kwargs):
-	"""	Deletes old file from filesystem when corresponding `SafetyItemDocuments` object is updated with new file. """
-	if not instance.pk:
-		return False
-
-	try:
-		old_file = SafetyItemDocuments.objects.get(pk=instance.pk).document
-	except SafetyItemDocuments.DoesNotExist:
-		return False
-
-	new_file = instance.document
-	if not old_file == new_file:
-		if os.path.isfile(old_file.path):
-			os.remove(old_file.path)
 
 
 class AlertCategory(BaseModel):
 	name = models.CharField(max_length=200)
 
 	class Meta:
 		ordering = ["name"]
@@ -2850,15 +2727,15 @@
 	deleted = models.BooleanField(default=False, help_text="Indicates the request has been deleted and won't be shown anymore.")
 
 	@property
 	def creator(self) -> User:
 		return self.user
 
 	@property
-	def replies(self) -> QuerySet:
+	def replies(self) -> QuerySetType[RequestMessage]:
 		return RequestMessage.objects.filter(object_id=self.id, content_type=ContentType.objects.get_for_model(self))
 
 	def creator_and_reply_users(self) -> List[User]:
 		result = {self.user}
 		for reply in self.replies:
 			result.add(reply.author)
 		return list(result)
@@ -2880,15 +2757,15 @@
 	new_start = models.DateTimeField(null=True, blank=True)
 	new_end = models.DateTimeField(null=True, blank=True)
 	status = models.IntegerField(choices=RequestStatus.choices_without_expired(), default=RequestStatus.PENDING)
 	reviewer = models.ForeignKey("User", null=True, blank=True, related_name='adjustment_requests_reviewed', on_delete=models.CASCADE)
 	deleted = models.BooleanField(default=False, help_text="Indicates the request has been deleted and won't be shown anymore.")
 
 	@property
-	def replies(self) -> QuerySet:
+	def replies(self) -> QuerySetType[RequestMessage]:
 		return RequestMessage.objects.filter(object_id=self.id, content_type=ContentType.objects.get_for_model(self))
 
 	def get_new_start(self) -> Optional[datetime]:
 		# Returns the new start if different from the item's start (not counting seconds and microseconds)
 		return self.new_start if self.new_start and self.item and self.item.start and self.item.start.replace(microsecond=0, second=0) != self.new_start else None
 
 	def get_new_end(self) -> Optional[datetime]:
@@ -2940,16 +2817,16 @@
 	content = models.TextField()
 
 	class Meta:
 		ordering = ['creation_date']
 
 
 class StaffAbsenceType(BaseModel):
-	name = models.CharField(max_length=255, help_text="The name of this absence type.")
-	description = models.CharField(max_length=255, help_text="The description for this absence type.")
+	name = models.CharField(max_length=CHAR_FIELD_MAXIMUM_LENGTH, help_text="The name of this absence type.")
+	description = models.CharField(max_length=CHAR_FIELD_MAXIMUM_LENGTH, help_text="The description for this absence type.")
 
 	def __str__(self):
 		description = f" ({self.description})" if self.description else ''
 		return f"{self.name}{description}"
 
 	class Meta:
 		ordering = ["name"]
```

### Comparing `NEMO-4.5.5/NEMO/parsers.py` & `NEMO-4.6.0/NEMO/parsers.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/permissions.py` & `NEMO-4.6.0/NEMO/permissions.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/policy.py` & `NEMO-4.6.0/NEMO/policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,21 +21,23 @@
     UnavailableResourcesUserError,
 )
 from NEMO.models import (
     Area,
     AreaAccessRecord,
     ClosureTime,
     Consumable,
+    ConsumableWithdraw,
     PhysicalAccessLevel,
     Project,
     Reservation,
     ReservationItemType,
     ScheduledOutage,
     StaffCharge,
     Tool,
+    UsageEvent,
     User,
 )
 from NEMO.utilities import (
     EmailCategory,
     distinct_qs_value_list,
     format_daterange,
     format_datetime,
@@ -43,15 +45,15 @@
     render_email_template,
     send_mail,
 )
 from NEMO.views.customization import ApplicationCustomization, EmailsCustomization, get_media_file_contents
 
 
 class NEMOPolicy:
-    def check_to_enable_tool(self, tool: Tool, operator: User, user: User, project: Project, staff_charge: bool):
+    def check_to_enable_tool(self, tool: Tool, operator: User, user: User, project: Project, staff_charge: bool, remote_work=False):
         """
         Check that the user is allowed to enable the tool. Enable the tool if the policy checks pass.
         """
         facility_name = ApplicationCustomization.get("facility_name")
 
         # The tool must be visible (or the parent if it's a child tool) to users.
         visible = tool.parent_tool.visible if tool.is_child_tool() else tool.visible
@@ -135,20 +137,20 @@
         # Staff may only charge staff time for one user at a time.
         if staff_charge and operator.charging_staff_time():
             return HttpResponseBadRequest(
                 "You are already charging staff time. You must end the current staff charge before you being another."
             )
 
         # Staff may not bill staff time to themselves.
-        if staff_charge and operator == user:
+        if (staff_charge or remote_work) and operator == user:
             return HttpResponseBadRequest("You cannot charge staff time to yourself.")
 
         # Check if we are allowed to bill to project
         try:
-            self.check_billing_to_project(project, user, tool)
+            self.check_billing_to_project(project, user, tool, UsageEvent(tool=tool, project=project, remote_work=remote_work, user=user))
         except ProjectChargeException as e:
             return HttpResponseBadRequest(e.msg)
 
         # The tool operator must not have a lock on usage
         if operator.training_required:
             return HttpResponseBadRequest(
                 f"You are blocked from using all tools in the {facility_name}. Please complete the {facility_name} rules tutorial in order to use tools."
@@ -246,15 +248,15 @@
             else:
                 policy_problems.append(
                     str(user) + " does not belong to any active projects and cannot have reservations."
                 )
 
         # Check if we are allowed to bill to project
         try:
-            self.check_billing_to_project(new_reservation.project, user, new_reservation.reservation_item)
+            self.check_billing_to_project(new_reservation.project, user, new_reservation.reservation_item, new_reservation)
         except ProjectChargeException as e:
             policy_problems.append(e.msg)
 
         # If the user is a staff member or there's an explicit policy override then the policy check is finished.
         if user.is_staff or explicit_policy_override:
             return policy_problems, overridable
 
@@ -842,15 +844,15 @@
                 if a.maximum_capacity and 0 < a.maximum_capacity <= a.occupancy_count():
                     raise MaximumCapacityReachedError(user=user, area=a)
 
             if area.requires_reservation and not area.get_current_reservation_for_user(user):
                 raise ReservationRequiredUserError(user=user, area=area)
 
     def check_billing_to_project(
-        self, project: Project, user: User, item: Union[Tool, Area, Consumable, StaffCharge] = None
+        self, project: Project, user: User, item: Union[Tool, Area, Consumable, StaffCharge] = None, charge: Union[UsageEvent, AreaAccessRecord, ConsumableWithdraw, StaffCharge, Reservation] = None
     ):
         if project:
             if project not in user.active_projects():
                 raise NotAllowedToChargeProjectException(project=project, user=user)
 
             if item:
                 # Check if project only allows billing for certain tools
```

### Comparing `NEMO-4.5.5/NEMO/provisioning.py` & `NEMO-4.6.0/NEMO/provisioning.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/rates.py` & `NEMO-4.6.0/NEMO/rates.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/rest_filter_backend.py` & `NEMO-4.6.0/NEMO/rest_filter_backend.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/serializers.py` & `NEMO-4.6.0/NEMO/serializers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from copy import deepcopy
 
 from django.contrib.auth.models import Group, Permission
 from django.contrib.contenttypes.models import ContentType
+from django.core import validators
 from rest_flex_fields.serializers import FlexFieldsSerializerMixin
 from rest_framework import serializers
 from rest_framework.fields import CharField, ChoiceField, DateTimeField, DecimalField, IntegerField
 from rest_framework.utils import model_meta
 
 from NEMO.models import (
 	Account,
@@ -40,36 +41,74 @@
 		# Remove many-to-many relationships from attributes_data, so we can properly validate.
 		info = model_meta.get_field_info(ModelClass)
 		for field_name, relation_info in info.relations.items():
 			if relation_info.to_many and (field_name in attributes_data):
 				attributes_data.pop(field_name)
 		for attr, value in attributes_data.items():
 			setattr(instance, attr, value)
-		self.full_clean(instance)
+		exclude = self.get_validation_exclusions(instance, attributes_data)
+		self.full_clean(instance, exclude)
 		return attrs
 
+	def get_validation_exclusions(self, instance, attributes_data):
+		exclude = []
+		# Build up a list of fields that should be excluded from model field
+		# validation and unique checks.
+		for f in instance._meta.fields:
+			field = f.name
+			meta_fields = getattr(self.Meta, 'fields', None)
+			meta_exclude = getattr(self.Meta, 'exclude', None)
+
+			# Exclude fields that aren't on the serializer.
+			if field not in self.fields:
+				exclude.append(f.name)
+
+			# Don't perform model validation on fields that were defined
+			# manually on the form and excluded via the Serializer's Meta
+			# class.
+			elif meta_fields and field not in meta_fields:
+				exclude.append(f.name)
+			elif meta_exclude and field in meta_exclude:
+				exclude.append(f.name)
+
+			# Exclude empty fields that are not required by the serializer, if
+			# the underlying model field is required. This keeps the model field
+			# from raising a required error. Note: don't exclude the field from
+			# validation if the model field allows blanks. If it does, the blank
+			# value may be included in a unique check, so cannot be excluded
+			# from validation.
+			else:
+				form_field = self.fields[field]
+				field_value = attributes_data.get(field)
+				if not f.blank and not form_field.required and field_value in list(validators.EMPTY_VALUES):
+					exclude.append(f.name)
+		return exclude
+
 	def full_clean(self, instance, exclude=None, validate_unique=True):
 		instance.full_clean(exclude, validate_unique)
 
 
-class UserSerializer(ModelSerializer):
+class UserSerializer(FlexFieldsSerializerMixin, ModelSerializer):
 	class Meta:
 		model = User
-		fields = "__all__"
+		exclude = ["preferences"]
+		expandable_fields = {
+			"projects": ("NEMO.serializers.ProjectSerializer", {'many': True}),
+			"managed_projects": ("NEMO.serializers.ProjectSerializer", {'many': True}),
+			"groups": ("NEMO.serializers.GroupSerializer", {'many': True}),
+			"user_permissions": ("NEMO.serializers.PermissionSerializer", {'many': True}),
+		}
 
-	# Special handling to exclude OneToOne user preferences here and add it in create
-	def full_clean(self, instance, exclude=None, validate_unique=True):
-		if not instance or not instance.id:
-			exclude = ["preferences"]
-		super().full_clean(instance, exclude, validate_unique)
-
-	def create(self, validated_data):
-		instance: User = super().create(validated_data)
-		instance.get_preferences()
-		return instance
+	def to_internal_value(self, data):
+		# Unique and nullable field conflict if passed the empty string so set
+		# it to None instead. Very specific case for nullable unique CharField
+		if data.get("badge_number", None) == "":
+			data = data.copy()
+			data["badge_number"] = None
+		return super().to_internal_value(data)
 
 
 class ProjectDisciplineSerializer(ModelSerializer):
 	class Meta:
 		model = ProjectDiscipline
 		fields = "__all__"
 
@@ -291,14 +330,15 @@
 
 
 class BillableItemSerializer(serializers.Serializer):
 	type = ChoiceField(
 		["missed_reservation", "tool_usage", "area_access", "consumable", "staff_charge", "training_session"]
 	)
 	name = CharField(max_length=200, read_only=True)
+	item_id = IntegerField(read_only=True)
 	details = CharField(max_length=500, read_only=True)
 	account = CharField(max_length=200, read_only=True)
 	account_id = IntegerField(read_only=True)
 	project = CharField(max_length=200, read_only=True)
 	project_id = IntegerField(read_only=True)
 	application = CharField(max_length=200, read_only=True)
 	user = CharField(max_length=255, read_only=True)
```

### Comparing `NEMO-4.5.5/NEMO/static/admin/physical_access_level/access_level.js` & `NEMO-4.6.0/NEMO/static/admin/physical_access_level/access_level.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/admin/questions_preview/questions_preview.css` & `NEMO-4.6.0/NEMO/static/admin/questions_preview/questions_preview.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/admin/questions_preview/questions_preview.js` & `NEMO-4.6.0/NEMO/static/admin/questions_preview/questions_preview.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/admin/time_options_override.js` & `NEMO-4.6.0/NEMO/static/admin/time_options_override.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/admin/tool/tool.js` & `NEMO-4.6.0/NEMO/static/admin/tool/tool.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/badge_reader.js` & `NEMO-4.6.0/NEMO/static/badge_reader.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,28 +1,30 @@
 BadgeReader = function(on_success, send_key, record_key) {
 
     $(window).keypress(on_keypress).keydown(on_keydown);
-    var record_badge_number = false;
-    var badge_number = "";
+    let record_badge_number = false;
+    let badge_number = "";
 
     // Note that keydown and keyup provide a code indicating which key is pressed, while keypress indicates which character was entered. For example, a lowercase "a" will be reported as 65 by keydown and keyup, but as 97 by keypress. An uppercase "A" is reported as 65 by all events. Because of this distinction, when catching special keystrokes such as F2, .keydown() or .keyup() is a better choice.
 
     function on_keypress(event) {
-        if (record_key && record_badge_number || !record_key) {
+        // Don't write send and record keys
+        if (event.key !== send_key && event.key !== record_key && (record_key && record_badge_number || !record_key)) {
             badge_number += String.fromCharCode(event.which);
             $("#badge_number").html(badge_number);
         }
     }
 
     function on_keydown(event) {
-        if (event.key === record_key) {
-            // Activate badge number recording
-            record_badge_number = !record_badge_number;
-        }
-        if (event.key === send_key && !record_badge_number) {
+        // First priority is sending the badge number if send key is pressed
+        if (event.key === send_key && (record_key && record_badge_number || !record_key)) {
             // Sending badge number
             on_success(badge_number);
             $("#badge_number").html(badge_number + ", sent");
             badge_number = "";
+            record_badge_number = false;
+        } else if (event.key === record_key) {
+            // Activate badge number recording
+            record_badge_number = true;
         }
     }
 };
```

### Comparing `NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap-theme.css` & `NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap-theme.css.map` & `NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap-theme.min.css` & `NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap.css` & `NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap.css.map` & `NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap.min.css` & `NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot` & `NEMO-4.6.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg` & `NEMO-4.6.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `NEMO-4.6.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff` & `NEMO-4.6.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2` & `NEMO-4.6.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/bootstrap/js/bootstrap.js` & `NEMO-4.6.0/NEMO/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/bootstrap/js/bootstrap.min.js` & `NEMO-4.6.0/NEMO/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/datetimepicker/bootstrap-datetimepicker.css` & `NEMO-4.6.0/NEMO/static/datetimepicker/bootstrap-datetimepicker.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/datetimepicker/bootstrap-datetimepicker.js` & `NEMO-4.6.0/NEMO/static/datetimepicker/bootstrap-datetimepicker.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/favicon.ico` & `NEMO-4.6.0/NEMO/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/fullcalendar/fullcalendar.css` & `NEMO-4.6.0/NEMO/static/fullcalendar/fullcalendar.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/fullcalendar/fullcalendar.js` & `NEMO-4.6.0/NEMO/static/fullcalendar/fullcalendar.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/fullcalendar/fullcalendar.min.css` & `NEMO-4.6.0/NEMO/static/fullcalendar/fullcalendar.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/fullcalendar/fullcalendar.min.js` & `NEMO-4.6.0/NEMO/static/fullcalendar/fullcalendar.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/icons/agreement.png` & `NEMO-4.6.0/NEMO/static/icons/agreement.png`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/icons/caution.png` & `NEMO-4.6.0/NEMO/static/icons/caution.png`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/icons/preferences.png` & `NEMO-4.6.0/NEMO/static/icons/preferences.png`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/jquery.js` & `NEMO-4.6.0/NEMO/static/jquery.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/jquery.min.js` & `NEMO-4.6.0/NEMO/static/jquery.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/jumbotron_watermark.bmp` & `NEMO-4.6.0/NEMO/static/jumbotron_watermark.bmp`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/mobile.js` & `NEMO-4.6.0/NEMO/static/mobile.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/moment.js` & `NEMO-4.6.0/NEMO/static/moment.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/moment.min.js` & `NEMO-4.6.0/NEMO/static/moment.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/moment.min.js.map` & `NEMO-4.6.0/NEMO/static/moment.min.js.map`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/nemo.css` & `NEMO-4.6.0/NEMO/static/nemo.css`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+a
+{
+	color: #1067b4;
+}
+
 label
 {
 	font-weight: normal !important;
 }
 
 .application-sidebar
 {
@@ -147,40 +152,60 @@
 .small-icon
 {
 	margin-right: 5px;
 }
 
 .primary-highlight
 {
-	color: #428bca;
+	color: #3477b4;
+}
+
+.label-primary
+{
+	background-color: #3477b4;
 }
 
 .success-highlight
 {
-	color: #22b14c;
+	color: #008000;
+}
+
+.label-success
+{
+	background-color: #008000;
 }
 
 .warning-highlight
 {
-	color: #f0ad4e;
+	color: #eb9316;
+}
+
+.label-warning
+{
+	background-color: #eb9316;
 }
 
 .danger-highlight
 {
-	color: red;
+	color: #dc143c;
+}
+
+.label-danger
+{
+	background-color: #dc143c;
 }
 
 .grey
 {
 	color: grey;
 }
 
 .light-grey
 {
-	color: lightgrey;
+	color: #6F6F6F;
 }
 
 .hover-black:hover
 {
 	color: black;
 }
 
@@ -276,14 +301,23 @@
 }
 
 /* Add extra space on the right of the calendar header where the buttons are */
 .fc-toolbar .fc-right {
 	margin-right: 15px;
 }
 
+/* Override Bootstrap's media and media-body CSS settings so that the
+Twitter Typeahead autocomplete dropdown menu isn't chopped off. */
+.media, .media-body
+{
+	overflow: visible;
+	min-height: 35px;
+}
+
+
 /* Twitter typeahead styles */
 .twitter-typeahead
 {
 	display: block !important;
 }
 
 /* The hint is the portion of text that comes after what you've typed to suggest word completion. */
@@ -301,22 +335,14 @@
 	border: 1px solid #cccccc;
 	border-radius: 4px;
 	box-shadow: 0 5px 10px rgba(0, 0, 0, .2);
 	max-height: 150px;
 	overflow-y: auto;
 }
 
-/* Override Bootstrap's media and media-body CSS settings so that the
-Twitter Typeahead autocomplete dropdown menu isn't chopped off. */
-.media, .media-body
-{
-	overflow: visible;
-	min-height: 35px;
-}
-
 /* The suggestion style encases the matching part of the query in each of the search results. */
 /* Zero out some padding and margin properties. */
 .tt-suggestion
 {
 	padding: 3px 20px;
 	line-height: 20px;
 	cursor: pointer;
@@ -872,27 +898,43 @@
 .pagination-column .glyphicon
 {
 	font-size: 10px;
 	padding-left: 5px;
 	vertical-align: middle;
 }
 
+/* No bottom margin when using pagination inside a panel */
+.panel-body .pagination:last-of-type
+{
+	margin-bottom: 0;
+}
+
 /* Badge display on top right corner */
+.badge
+{
+	background-color: #6e6e6e;
+}
+
 .badge.badge-tab-top
 {
 	z-index: 5;
 	position: absolute;
 	top: -0.5em;
 	right: -0.5em;
 }
 
-.active > a > .badge.badge-tab-top
+.badge.active
+{
+	vertical-align: top;
+}
+
+.active > a > .badge.badge-tab-top, .badge.active
 {
 	color: #fff !important;
-	background-color: red !important;
+	background-color: #ee0000 !important;
 }
 
 .nav-pills.nav-pills-spacer > li + li
 {
 	margin-left: 8px;
 }
 
@@ -918,15 +960,14 @@
 
 .sticky
 {
 	position: sticky;
 	position: -webkit-sticky;
 	left: 0;
 	top:0;
-	background-color: #fff;
 	z-index: 5;
 }
 
 /* Staff status styles */
 .staff-status-contact, .staff-status-add
 {
 	width: 100%;
@@ -1035,7 +1076,84 @@
 	padding-top: 20px;
 }
 
 .adjustment-request-reply-textarea
 {
 	padding-top: 5px;
 }
+
+.usage-charge
+{
+	position: relative;
+}
+
+.usage-charge-adjustment-button
+{
+	position: absolute;
+	top: 15px;
+	right: 15px;
+}
+
+/* Table default color enforcing (useful when using sticky columns) */
+.table > thead > tr > td.default,
+.table > tbody > tr > td.default,
+.table > tfoot > tr > td.default,
+.table > thead > tr > th.default,
+.table > tbody > tr > th.default,
+.table > tfoot > tr > th.default,
+.table > thead > tr.default > td,
+.table > tbody > tr.default > td,
+.table > tfoot > tr.default > td,
+.table > thead > tr.default > th,
+.table > tbody > tr.default > th,
+.table > tfoot > tr.default > th
+{
+  	background-color: #ffffff;
+}
+
+.table-striped > thead > tr:nth-of-type(odd) > td.default,
+.table-striped > tbody > tr:nth-of-type(odd) > td.default,
+.table-striped > tfoot > tr:nth-of-type(odd) > td.default,
+.table-striped > thead > tr:nth-of-type(odd) > th.default,
+.table-striped > tbody > tr:nth-of-type(odd) > th.default,
+.table-striped > tfoot > tr:nth-of-type(odd) > th.default,
+.table-striped > thead > tr.default:nth-of-type(odd) > td,
+.table-striped > tbody > tr.default:nth-of-type(odd) > td,
+.table-striped > tfoot > tr.default:nth-of-type(odd) > td,
+.table-striped > thead > tr.default:nth-of-type(odd) > th,
+.table-striped > tbody > tr.default:nth-of-type(odd) > th,
+.table-striped > tfoot > tr.default:nth-of-type(odd) > th
+{
+  	background-color: #f9f9f9;
+}
+
+.table-hover > tbody > tr > td.default:hover,
+.table-hover > tbody > tr > th.default:hover,
+.table-hover > tbody > tr.default:hover > td,
+.table-hover > tbody > tr:hover > .default,
+.table-hover > tbody > tr.default:hover > th
+{
+  	background-color: #f5f5f5;
+}
+
+.strikethrough
+{
+	text-decoration: line-through;
+}
+
+#safety-tabs
+{
+	margin-top: 0;
+	margin-bottom: 15px;
+}
+
+.safety-title
+{
+	margin-top: 0;
+	margin-right: 20px;
+}
+
+.safety-tabs-nav
+{
+	display: inline-block;
+	float: right;
+}
```

### Comparing `NEMO-4.5.5/NEMO/static/nemo.js` & `NEMO-4.6.0/NEMO/static/nemo.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -36,15 +36,15 @@
     }
 }
 
 // This function allows any page to switch between content tabs in
 // the Bootstrap framework. It is generally called upon loading the page.
 function switch_tab(element) {
     element.preventDefault();
-    $(this).tab('show')
+    $(this).tab('show');
 }
 
 function set_item_link_callback(callback) {
     $("a[data-item-type='tool'], a[data-item-type='area']").each(function() {
         $(this).click({
             "callback": callback
         }, callback);
@@ -67,30 +67,40 @@
     expand_to_item(search_selection.id, search_selection.type);
 }
 
 // This function toggles all parent categories of a tool/area and selects the tool.
 function expand_to_item(id, type) {
     $("#sidebar a").removeClass('selected');
     $("#" + type + "-" + id).addClass('selected').click().parents('ul.tree').show();
+    $("#sidebar").attr("aria-expanded", true);
     save_sidebar_state();
 }
 
+function toggle_categories() {
+    let sidebar_expanded = $("#sidebar").attr("aria-expanded") || "false";
+    sidebar_expanded === "true" ? collapse_all_categories() : expand_all_categories();
+}
+
 // This function expands all tool category branches for the sidebar in the calendar & tool control pages.
 function expand_all_categories() {
     $(".item_tree ul.tree.area-list").show();
     $(".item_tree ul.tree.tool-list").show();
     $("#search").focus();
+    $("#sidebar").attr("aria-expanded", true);
+    $("#expand_collapse_icon").removeClass("glyphicon-resize-full").removeClass("glyphicon-resize-small").addClass("glyphicon-resize-small");
     save_sidebar_state();
 }
 
 // This function collapses all tool category branches for the sidebar in the calendar & tool control pages.
 function collapse_all_categories() {
     $(".item_tree ul.tree.tool-list").hide();
     $(".item_tree ul.tree.area-list").hide();
     $("#search").focus();
+    $("#sidebar").attr("aria-expanded", false);
+    $("#expand_collapse_icon").removeClass("glyphicon-resize-full").removeClass("glyphicon-resize-small").addClass("glyphicon-resize-full");
     save_sidebar_state();
 }
 
 function toggle_qualified_tools(user_qualifications) {
     // Toggle local storage data value
     if (localStorage.getItem("showQualifiedTools") === "true") {
         localStorage.setItem("showQualifiedTools", "false");
@@ -214,14 +224,15 @@
     }
 }
 
 function save_sidebar_state() {
     let showQualifiedTools = localStorage.getItem("showQualifiedTools");
 
     localStorage.clear();
+    localStorage["sidebarExpanded"] = $("#sidebar").attr("aria-expanded") || "false";
     let categories = $(".item_tree ul.tree");
     for (let c = 0; c < categories.length; c++) {
         let category = categories[c].getAttribute('data-category');
         localStorage[category] = $(categories[c]).is(':visible');
     }
     let selected_item = get_selected_item();
     if (selected_item) {
@@ -230,14 +241,21 @@
 
     if (showQualifiedTools !== null) {
         localStorage.setItem("showQualifiedTools", showQualifiedTools)
     }
 }
 
 function load_sidebar_state() {
+    let sidebar_expanded = localStorage.getItem("sidebarExpanded");
+    if (sidebar_expanded === "true") {
+        $("#expand_collapse_icon").addClass("glyphicon-resize-small");
+    } else {
+        $("#expand_collapse_icon").addClass("glyphicon-resize-full");
+    }
+    $("#sidebar").attr("aria-expanded", sidebar_expanded);
     let categories = $(".item_tree ul.tree");
     for (let c = 0; c < categories.length; c++) {
         let category = categories[c];
         let name = category.getAttribute('data-category');
         let state = localStorage[name];
         if (state === "true") {
             $(category).show();
@@ -283,16 +301,16 @@
 // Use this function with ajax_get(), ajax_post() or other similar functions.
 function ajax_failure_callback(title, preface) {
     preface = preface || "";
 
     function callback(xml_http_request, status, exception) {
         let dialog_contents =
             "<div class='modal-header'>" +
-            "<button type='button' class='close' data-dismiss='modal'>&times;</button>" +
-            "<h4 class='modal-title'>" + title + "</h4>" +
+            "<button type='button' class='close' data-dismiss='modal' aria-label='Modal close button'>&times;</button>" +
+            "<h4 id='modal-description-label' class='modal-title'>" + title + "</h4>" +
             "</div>" +
             "<div class='modal-body'>" + [preface, xml_http_request.responseText].join(" ") +
             "</div>";
         $("#dialog .modal-content").html(dialog_contents);
         $("#dialog").modal('show');
     }
 
@@ -304,16 +322,16 @@
 
     function callback(response, status, xml_header_request) {
         if (status !== "error") {
             return;
         }
         let dialog_contents =
             "<div class='modal-header'>" +
-            "<button type='button' class='close' data-dismiss='modal'>&times;</button>" +
-            "<h4 class='modal-title'>" + title + "</h4>" +
+            "<button type='button' class='close' data-dismiss='modal' aria-label='Modal close button'>&times;</button>" +
+            "<h4 id='modal-description-label' class='modal-title'>" + title + "</h4>" +
             "</div>" +
             "<div class='modal-body'>" + [preface, xml_header_request.responseText].join(" ") +
             "</div>";
         $("#dialog .modal-content").html(dialog_contents);
         $("#dialog").modal('show');
     }
 
@@ -603,8 +621,28 @@
             }
         }
         if (shouldSwitch) {
             b[i].parentNode.insertBefore(b[i + 1], b[i]);
             switching = true;
         }
     }
+}
+
+function wait_for_element(selector) {
+    return new Promise(resolve => {
+        if (document.querySelector(selector)) {
+            return resolve(document.querySelector(selector));
+        }
+
+        const observer = new MutationObserver(mutations => {
+            if (document.querySelector(selector)) {
+                resolve(document.querySelector(selector));
+                observer.disconnect();
+            }
+        });
+
+        observer.observe(document.body, {
+            childList: true,
+            subtree: true
+        });
+    });
 }
```

### Comparing `NEMO-4.5.5/NEMO/static/numpad/custom_numpad.jquery.js` & `NEMO-4.6.0/NEMO/static/numpad/custom_numpad.jquery.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/pickadate/default.css` & `NEMO-4.6.0/NEMO/static/pickadate/default.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/pickadate/default.date.css` & `NEMO-4.6.0/NEMO/static/pickadate/default.date.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/pickadate/default.time.css` & `NEMO-4.6.0/NEMO/static/pickadate/default.time.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/pickadate/picker.date.js` & `NEMO-4.6.0/NEMO/static/pickadate/picker.date.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/pickadate/picker.js` & `NEMO-4.6.0/NEMO/static/pickadate/picker.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/pickadate/picker.time.js` & `NEMO-4.6.0/NEMO/static/pickadate/picker.time.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/typeahead.jquery.js` & `NEMO-4.6.0/NEMO/static/typeahead.jquery.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/typeahead.jquery.min.js` & `NEMO-4.6.0/NEMO/static/typeahead.jquery.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/virtualkeyboard/jquery.keyboard.js` & `NEMO-4.6.0/NEMO/static/virtualkeyboard/jquery.keyboard.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/virtualkeyboard/jquery.keyboard.min.js` & `NEMO-4.6.0/NEMO/static/virtualkeyboard/jquery.keyboard.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/virtualkeyboard/keyboard-basic.css` & `NEMO-4.6.0/NEMO/static/virtualkeyboard/keyboard-basic.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/static/virtualkeyboard/keyboard-basic.min.css` & `NEMO-4.6.0/NEMO/static/virtualkeyboard/keyboard-basic.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/abuse/abuse.html` & `NEMO-4.6.0/NEMO/templates/abuse/abuse.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/abuse/user_drill_down.html` & `NEMO-4.6.0/NEMO/templates/abuse/user_drill_down.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/accounts_and_projects/account_and_projects.html` & `NEMO-4.6.0/NEMO/templates/accounts_and_projects/account_and_projects.html`

 * *Files 4% similar despite different names*

```diff
@@ -42,44 +42,50 @@
                                 <a onclick="$(this).closest('form').submit()" class="label {% if project.active %}label-success{% else %}label-danger{% endif %}" style="vertical-align:50%; font-size:small">
                                     {% if project.active %}Active{% else %}Inactive{% endif %}
                                 </a>
                             </form>
                         </div>
                         <div style="margin-left:34px">
                             {% if selected_project %}<label class="control-label">Account:</label> <a href="{% url 'account' project.account.id %}">{{ project.account }}</a>{% endif %}
+                            {% if project.manager_set.all %}
+                                <div>
+                                    <span class="control-label">PIs:</span>
+                                    <span>{{ project.manager_set.all|join:", " }}</span>
+                                </div>
+                            {% endif %}
                             <div id="project_{{ project.id }}_details" class="collapse {% if selected_project %}in{% endif %}">
                                 <div>
-                                    <label class="control-label">{{ "projects_and_accounts"|customization:"project_application_identifier_name" }}:</label>
-                                    <span class="grey">{{ project.application_identifier }}</span>
+                                    <span class="control-label">{{ "projects_and_accounts"|customization:"project_application_identifier_name" }}:</span>
+                                    <span>{{ project.application_identifier }}</span>
                                 </div>
 								{% if project.discipline %}
 									<div>
-										<label class="control-label">Discipline:</label>
-										<span class="grey">{{ project.discipline }}</span>
+										<span class="control-label">Discipline:</span>
+										<span>{{ project.discipline }}</span>
 									</div>
 								{% endif %}
                                 {% if project.start_date %}
                                     <div>
-                                        <label class="control-label">Start Date:</label>
-                                        <span class="grey">{{ project.start_date }}</span>
+                                        <span class="control-label">Start Date:</span>
+                                        <span>{{ project.start_date }}</span>
                                     </div>
                                 {% endif %}
                                 <div id="project_{{ project.id }}_users">
                                     {% include 'accounts_and_projects/users_for_project.html' with users=project.user_set.all %}
                                 </div>
 								{% if allow_document_upload or project.project_documents.all %}
 									<div id="project_{{ project.id }}_documents">
 										{% include 'accounts_and_projects/documents_for_project.html' with documents=project.project_documents.all %}
 									</div>
 								{% endif %}
                             </div>
                         </div>
                     {% endif %}
 				{% empty %}
-					<h4 class="grey">This account does not have any projects</h4>
+					<h4>This account does not have any projects</h4>
 				{% endfor %}
 			</div>
 		</div>
 	{% endif %}
 	<script>
 		function get_account(jquery_event, search_selection, dataset_name)
 		{
```

#### html2text {}

```diff
@@ -14,15 +14,18 @@
 {% endif %} {% for project in account.project_set.all %} {% if not
 selected_project or project == selected_project %}
  {{ project }}
 {% csrf_token %} {# Using an 'input submit' element would be preferable to an
 anchor on the following line, but Bootstrap can't style a 'submit' as a label
 so you have to use an anchor. #} {% if project.active %}Active{% else
 %}Inactive{% endif %}
-{% if selected_project %}Account: {{_project.account_}}{% endif %}
+{% if selected_project %}Account: {{_project.account_}}{% endif %} {% if
+project.manager_set.all %}
+PIs: {{ project.manager_set.all|join:", " }}
+{% endif %}
 {{ "projects_and_accounts"|customization:"project_application_identifier_name"
 }}: {{ project.application_identifier }}
 {% if project.discipline %}
 Discipline: {{ project.discipline }}
 {% endif %} {% if project.start_date %}
 Start Date: {{ project.start_date }}
 {% endif %}
```

### Comparing `NEMO-4.5.5/NEMO/templates/accounts_and_projects/accounts_and_projects.html` & `NEMO-4.6.0/NEMO/templates/accounts_and_projects/accounts_and_projects.html`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 	<table class="table table-bordered table-condensed table-hover table-align-middle thead-light">
 			<thead>
 				<tr>
 					<th>{% include 'pagination/pagination_column.html' with order_by='name' name='Name' %}</th>
 					{% if account_types %}<th>{% include 'pagination/pagination_column.html' with order_by='type' name='Account type' %}</th>{% endif %}
 					<th>{{ "projects_and_accounts"|customization:"project_application_identifier_name" }}</th>
 					<th class="button-column-minimum">{% include 'pagination/pagination_column.html' with order_by='active' name='Active' %}</th>
-					<th class="button-column-minimum"></th>
+					<th class="button-column-minimum" aria-label="Action"></th>
 				</tr>
 			</thead>
 			<tbody>
 				{% for account in page %}
 					<tr style="background-color: #f9f9f9">
 						<td id="chevron_{{ account.id }}" data-toggle="collapse" data-target=".projects_{{ account.id }}" onclick="toggle_details($('#chevron_{{ account.id }}'))" style="font-weight: bold">
 							<span class="glyphicon glyphicon-chevron-{% if account_list_collapse %}right{% else %}down{% endif %} pull-left chevron"></span>
@@ -50,15 +50,15 @@
                             {% button type="view" size="small" value="View" title="View account" url=account_url %}
 						</td>
 					</tr>
                     {% regroup account.sorted_projects by active as active_inactive_projects %}
                     {% if active_inactive_projects|length_is:1 and not active_inactive_projects.0.grouper and project_list_active_only %}
                         <tr class="collapse {% if not account_list_collapse %}in{% endif %} projects_{{ account.id }}">
 							<td colspan="4" style="padding-left: 28px">
-								<span class="grey">This account does not have any active projects</span>
+								<span>This account does not have any active projects</span>
 							</td>
 						</tr>
                     {% endif %}
 					{% for project_list in active_inactive_projects %}
                         {% if project_list.grouper or not project_list_active_only %}
                             {% for project in project_list.list %}
                                 <tr class="collapse {% if not account_list_collapse %}in{% endif %} projects_{{ account.id }}">
@@ -81,15 +81,15 @@
                                     </td>
                                 </tr>
                             {% endfor %}
                         {% endif %}
                     {% empty %}
 						<tr class="collapse {% if not account_list_collapse %}in{% endif %} projects_{{ account.id }}">
 							<td colspan="4" style="padding-left: 28px">
-								<span class="grey">This account does not have any projects</span>
+								<span>This account does not have any projects</span>
 							</td>
 						</tr>
                     {% endfor %}
 				{% endfor %}
 			</tbody>
 		</table>
 {% endblock %}
```

### Comparing `NEMO-4.5.5/NEMO/templates/accounts_and_projects/create_account.html` & `NEMO-4.6.0/NEMO/templates/accounts_and_projects/create_account.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/accounts_and_projects/create_project.html` & `NEMO-4.6.0/NEMO/templates/accounts_and_projects/create_project.html`

 * *Files 26% similar despite different names*

```diff
@@ -64,14 +64,25 @@
             <div class="col-sm-4">
 				<input type="text" id="start_date" name="start_date" class="form-control" placeholder="Choose a date" value="{{ form.start_date.value|input_date_format }}">
             </div>
             <div class="col-sm-6 form-control-static danger-highlight">
 				{{ form.start_date.errors|striptags }}
 			</div>
         </div>
+        <div class="form-group">
+            <label class="control-label col-sm-2" for="pi_search">PIs</label>
+            <div class="col-sm-4">
+                <input id="pi_search" type="text" autocomplete="off" class="form-control" placeholder="Add a principal investigator">
+            </div>
+        </div>
+        <div class="form-group">
+            <div id="pi-list" class="col-sm-offset-2 col-sm-4">
+                This project has no principal investigators.
+            </div>
+        </div>
 		{% if allow_document_upload %}
 			<div class="form-group">
 				<label for="project_documents" class="control-label col-sm-2">Documents</label>
                 <div class="col-sm-4">
 					<input type="file" id="project_documents" name="project_documents" class="form-control-static" multiple>
 				</div>
 				<div class="col-sm-6 form-control-static danger-highlight">
@@ -91,24 +102,44 @@
 		<div class="form-group">
 			<div class="col-sm-offset-2 col-sm-10">
                 {% button type="save" value="Create new project" %}
 			</div>
 		</div>
 	</form>
 	<script>
+        function select_pi(jquery_event, search_selection, dataset_name)
+        {
+            add_to_list("#pi-list", "remove_pi", search_selection.id, search_selection.name, "remove " + search_selection.name + " as principal investigator", "principal_investigators");
+            $("#pi_search").typeahead('val', '');
+        }
+        function remove_pi(id)
+        {
+            remove_from_list("#pi-list", "#principal_investigators_" + id, "This project has no principal investigators.")
+        }
 		function select_account(jquery_event, search_selection, dataset_name)
 		{
 			$('#account_search').prop('required', false).typeahead('val', search_selection.id).hide();
 			$("#selected_account").val(search_selection.name).show();
 		}
 		function clear_account_selection()
 		{
 			$("#selected_account").hide();
 			$('#account_search').prop('required', true).typeahead('val', '').show().focus();
 		}
 		window.addEventListener("load", function ()
 		{
 		    $('#start_date').datetimepicker({format: '{{ date_input_js_format }}'});
+            $('#pi_search').autocomplete('pis', select_pi, {{ user_list|json_search_base }});
 			$('#account_search').autocomplete('account', select_account, {{ account_list|json_search_base }});
+            {% if form.account.value %}
+                {% for account in account_list %}
+                    {% if account.id == form.account.value|to_int %}select_account(null, {"id": "{{ account.id }}", "name": "{{ account.name }}"});{% endif %}
+                {% endfor %}
+            {% endif %}
+            {% for pi in form.principal_investigators.value %}
+                {% for user in user_list %}
+                    {% if user.id == pi|to_int %}select_pi(null, {"id": "{{ user.id }}", "name": "{{ user }}"});{% endif %}
+                {% endfor %}
+            {% endfor %}
 		});
 	</script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -25,14 +25,17 @@
 { discipline_name|default_if_none:'' }}
 {% endfor %}
 {{ form.discipline.errors|striptags }}
 {% endif %}
 Start date
 [{{ form.start_date.value|input_date_format }}]
 {{ form.start_date.errors|striptags }}
+PIs
+[                    ]
+This project has no principal investigators.
 {% if allow_document_upload %}
 Documents
 [File]
 {{ form.project_documents.errors|striptags }}
 {% endif %}
 
 % if form.active.value %}checked{% endif %}> Active
```

### Comparing `NEMO-4.5.5/NEMO/templates/accounts_and_projects/documents_for_project.html` & `NEMO-4.6.0/NEMO/templates/accounts_and_projects/documents_for_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/accounts_and_projects/projects.html` & `NEMO-4.6.0/NEMO/templates/accounts_and_projects/projects.html`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 					<div>
 						<label class="control-label">Users:</label>
 					</div>
 					<div>
 						{% if project.user_set.all %}
 							<ul>
 							{% for u in project.user_set.all %}
-								<li class="{% if not u.is_active %}light-grey{% endif %}">{{ u }}</li>
+								<li class="{% if not u.is_active %}strikethrough light-grey{% endif %}">{{ u }}</li>
 							{% endfor %}
 							</ul>
 						{% else %}
 							<span class="grey">This project does not have any members.</span>
 						{% endif %}
 					</div>
 				{% endif %}
```

### Comparing `NEMO-4.5.5/NEMO/templates/accounts_and_projects/users_for_project.html` & `NEMO-4.6.0/NEMO/templates/accounts_and_projects/users_for_project.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <div style="height:10px"></div>
 <div id="add_user_to_project_{{ project.id }}">
 	<label class="control-label">Users:<input id="search_user_for_project_{{ project.id }}" type="text" class="form-control user_search" placeholder="Search for a user to add" data-project-id="{{ project.id }}" style="min-width: 250px;"></label>
 </div>
 <div>
 	{% for u in users %}
-		<a href="javascript:remove_user_from_project('{{ u.id }}', '{{ project.id }}')" class="{% if u.is_active %}grey{% else %}light-grey{% endif %} hover-black" title="Remove {{ u.first_name }}"><span class="glyphicon glyphicon-remove-circle"></span></a> {% if u.is_active %}{{ u }}{% else %}<span class="light-grey">{{ u }}</span>{% endif %}<br>
+		<a href="javascript:remove_user_from_project('{{ u.id }}', '{{ project.id }}')" class="grey hover-black" title="Remove {{ u.first_name }}"><span class="glyphicon glyphicon-remove-circle"></span></a> {% if u.is_active %}{{ u }}{% else %}<span class="strikethrough light-grey" title="This user is inactive">{{ u }}</span>{% endif %}<br>
 	{% empty %}
 		This project does not have any members.
 	{% endfor %}
 </div>
 
 <script>
     $(function()
```

### Comparing `NEMO-4.5.5/NEMO/templates/alerts.html` & `NEMO-4.6.0/NEMO/templates/alerts.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/area_access/area_access.html` & `NEMO-4.6.0/NEMO/templates/area_access/area_access.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/area_access/calendar_self_login.html` & `NEMO-4.6.0/NEMO/templates/area_access/calendar_self_login.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% load custom_tags_and_filters %}
 <div class="modal-header">
-	<button type="button" class="close" data-dismiss="modal">&times;</button>
-	<h4 class="modal-title">{% if error_message %}Error trying {% else %}You are about {% endif %}to login to the {{ area }}</h4>
+	<button type="button" class="close" data-dismiss="modal" aria-label="Modal close button">&times;</button>
+	<h4 id="modal-description-label" class="modal-title">{% if error_message %}Error trying {% else %}You are about {% endif %}to login to the {{ area }}</h4>
 </div>
 
 <div class="modal-body">
 	<input type="hidden" id="dialog_cancelled" value="true">
 	{% if error_message %}
 		<div class="alert alert-danger">
 			{{ error_message }}
```

### Comparing `NEMO-4.5.5/NEMO/templates/area_access/change_project.html` & `NEMO-4.6.0/NEMO/templates/area_access/change_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/area_access/login_areas.html` & `NEMO-4.6.0/NEMO/templates/area_access/login_areas.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/area_access/new_area_access_record.html` & `NEMO-4.6.0/NEMO/templates/area_access/new_area_access_record.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/area_access/new_area_access_record_details.html` & `NEMO-4.6.0/NEMO/templates/area_access/new_area_access_record_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/area_access/self_login.html` & `NEMO-4.6.0/NEMO/templates/area_access/self_login.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/authorization_failed.html` & `NEMO-4.6.0/NEMO/templates/authorization_failed.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/base/navbar_base.html` & `NEMO-4.6.0/NEMO/templates/base/navbar_base.html`

 * *Files 12% similar despite different names*

```diff
@@ -22,23 +22,23 @@
                             <li><a href="{% url 'status_dashboard_tab' 'tools' %}">Status dashboard</a></li>
                         {% endif %}
                     {% endif %}
                     {% if buddy_system_areas_exist or access_user_request_allowed_exist and facility_managers_exist or adjustment_request_allowed and facility_managers_exist %}
                         <li><a href="{% url 'user_requests' %}">
                             Requests
                             {% if buddy_notification_count or temporary_access_notification_count or adjustment_notification_count %}
-                                <span class="badge" style="vertical-align:middle; background-color:red">{{ buddy_notification_count|add:temporary_access_notification_count|add:adjustment_notification_count }}</span>
+                                <span class="badge active">{{ buddy_notification_count|add:temporary_access_notification_count|add:adjustment_notification_count }}</span>
                             {% endif %}
                         </a></li>
                     {% endif %}
                     {% if safety_menu_item %}
                         <li><a href="{% url 'safety' %}">
                             Safety
                             {% if safety_notification_count %}
-                                <span class="badge" style="vertical-align:middle; background-color:red">{{ safety_notification_count }}</span>
+                                <span class="badge active">{{ safety_notification_count }}</span>
                             {% endif %}
                         </a></li>
                     {% endif %}
                 {% endblock %}
 				{% if user.is_any_part_of_staff or user.is_tool_superuser or user.is_project_pi or user.get_all_permissions and "django.contrib.admin"|app_installed %}
 					<li class="dropdown">
 						<a href="#" class="dropdown-toggle" data-toggle="dropdown">Administration <b class="caret"></b></a>
@@ -50,14 +50,17 @@
                                 {% if user.is_any_part_of_staff %}
                                     {% navigation_url 'abuse' 'Abuse' user.is_facility_manager user.is_superuser %}
                                     {% navigation_url 'accounts_and_projects' 'Accounts and projects' user.is_accounting_officer user.is_user_office user.is_facility_manager user.is_superuser %}
                                     {% navigation_url 'alerts' 'Alerts' user.is_staff user.is_user_office user.is_superuser %}
                                     {% navigation_url 'api-root' 'API' user.is_superuser %}
                                     {% if areas_exist %}{% navigation_url 'area_access' 'Area access' user.is_staff user.is_user_office user.is_superuser %}{% endif %}
                                     {% if tools_exist %}{% navigation_url 'configuration_agenda' 'Configuration agenda' user.is_staff user.is_superuser %}{% endif %}
+                                    {% if user.is_facility_manager or user.is_superuser or user.is_staff and "contracts"|customization:"contracts_view_staff" == "enabled" or user.is_user_office and "contracts"|customization:"contracts_view_user_office" == "enabled" or user.is_accounting_officer and "contracts"|customization:"contracts_view_accounting_officer" == "enabled" %}
+                                        {% navigation_url 'service_contracts' 'Contracts & procurements' %}
+                                    {% endif %}
                                     {% navigation_url 'customization' 'Customization' user.is_superuser %}
                                     {% navigation_url 'email_broadcast' 'Email' %}
                                     {% navigation_url 'impersonate' 'Impersonate' user.is_superuser %}
                                     {% if tools_exist %}{% navigation_url 'maintenance' 'Maintenance' user.is_staff  user.is_superuser %}{% endif %}
                                     {% navigation_url 'project_billing' 'Project billing' user.is_accounting_officer user.is_user_office user.is_superuser %}
                                     {% if tools_exist %}{% navigation_url 'qualifications' 'Qualifications' user.is_staff user.is_superuser %}{% endif %}
                                     {% navigation_url 'recurring_charges' recurring_charges_name user.is_user_office user.is_facility_manager user.is_superuser %}
```

#### html2text {}

```diff
@@ -34,15 +34,22 @@
             {% navigation_url 'alerts' 'Alerts' user.is_staff
             user.is_user_office user.is_superuser %} {% navigation_url 'api-
             root' 'API' user.is_superuser %} {% if areas_exist %}{%
             navigation_url 'area_access' 'Area access' user.is_staff
             user.is_user_office user.is_superuser %}{% endif %} {% if
             tools_exist %}{% navigation_url 'configuration_agenda'
             'Configuration agenda' user.is_staff user.is_superuser %}{% endif
-            %} {% navigation_url 'customization' 'Customization'
+            %} {% if user.is_facility_manager or user.is_superuser or
+            user.is_staff and "contracts"|customization:"contracts_view_staff"
+            == "enabled" or user.is_user_office and "contracts"|customization:
+            "contracts_view_user_office" == "enabled" or
+            user.is_accounting_officer and "contracts"|customization:
+            "contracts_view_accounting_officer" == "enabled" %} {%
+            navigation_url 'service_contracts' 'Contracts & procurements' %} {%
+            endif %} {% navigation_url 'customization' 'Customization'
             user.is_superuser %} {% navigation_url 'email_broadcast' 'Email' %}
             {% navigation_url 'impersonate' 'Impersonate' user.is_superuser %}
             {% if tools_exist %}{% navigation_url 'maintenance' 'Maintenance'
             user.is_staff user.is_superuser %}{% endif %} {% navigation_url
             'project_billing' 'Project billing' user.is_accounting_officer
             user.is_user_office user.is_superuser %} {% if tools_exist %}{%
             navigation_url 'qualifications' 'Qualifications' user.is_staff
```

### Comparing `NEMO-4.5.5/NEMO/templates/base.html` & `NEMO-4.6.0/NEMO/templates/base.html`

 * *Files 7% similar despite different names*

```diff
@@ -53,32 +53,33 @@
 	<link rel="stylesheet" type="text/css" href="{% static "nemo.css" %}"/>
 
 	{% block extrahead %}{% endblock %}
 
 	<title>{% block title %}{% endblock %}</title>
 </head>
 <body class="{% if request.session.impersonate_id %}impersonating{% endif %}">
+<a class="sr-only sr-only-focusable" href="#main-content">Skip to main content</a>
 {% if request.session.impersonate_id %}
 	{% include 'base/impersonate_header.html' %}
 {% endif %}
 {% if no_header %}
 	<div style="height: 15px;"></div>
 {% else %}
 	{% include 'base/navbar.html' %}
 {% endif %}
 {% block body %}
     <div class="body-container">
         <div id="loading-div-page" class="spinner-full-page spinner-container" style="display: none">
             <div class="glyphicon glyphicon-repeat normal-right-spinner"></div>
         </div>
-        <div class="container">
+        <div class="container" id="main-content">
 			{% if messages %}
 				{% for message in messages %}
 					<div class="alert alert-{% if message.level_tag == 'error' %}danger{% else %}{{ message.level_tag }}{% endif %} alert-dismissible show-on-load" {% if message.extra_tags %}{{ message.extra_tags }}{% endif %} style="display: none">
-						<button type="button" class="close" data-dismiss="alert">&times;</button>
+						<button type="button" class="close" data-dismiss="alert" aria-label="Modal close button">&times;</button>
 						{{ message }}
 					</div>
 				{% endfor %}
 			{% endif %}
             {# Content goes here #}
             {% block content %}{% endblock %}
         </div>
@@ -86,16 +87,16 @@
             <div style="height: 200px"></div>
         {% endblock %}
     </div>
     {% include 'base/footer.html' %}
 {% endblock %}
 
 {# This division is used to display dialog messages via Bootstrap. #}
-<div class="modal fade" id="dialog" tabindex="-1" role="dialog">
-	<div class="modal-dialog">
+<div class="modal fade" id="dialog" tabindex="-1">
+	<div class="modal-dialog" role="dialog" aria-modal="true">
 		<div class="modal-content">
 		</div>
 	</div>
 </div>
 
 <script>
 	function csrf_token()
@@ -144,15 +145,19 @@
         {# sent to the logoff page, which then redirects them back to the login page. #}
         {% if logout_allowed %}
             $(document).ajaxComplete(function (event, xhr, status, error){navigate_to_login_on_session_expiration('{% url 'logout' %}', event, xhr, status, error)});
         {% endif %}
 
         {# Remove all size classes from the modal on close, to revert to default medium size #}
         $("#dialog").on("hidden.bs.modal", function () {
-            $('#dialog .modal-dialog').removeClass('modal-lg', 'modal-sm');
+            $("#dialog .modal-dialog").removeClass("modal-lg", "modal-sm");
+        });
+        {# Set described by on when showing modal #}
+        $("#dialog").on("shown.bs.modal", function () {
+            $("#dialog .modal-dialog").attr("aria-labelledby", "modal-description-label");
         });
     }, false);
 
     {# Hide spinner on page show, just in case for some browser back button reloading it #}
     window.addEventListener('pageshow', function()
     {
         hide_spinner();
```

### Comparing `NEMO-4.5.5/NEMO/templates/calendar/calendar.html` & `NEMO-4.6.0/NEMO/templates/calendar/calendar.html`

 * *Files 3% similar despite different names*

```diff
@@ -3,42 +3,40 @@
 {% block title %}Calendar{% endblock %}
 {% block extrahead %}
 	{% load static %}
 	<link rel="stylesheet" type="text/css" href="{% static "fullcalendar/fullcalendar.min.css" %}" />
 	<script type="text/javascript" src="{% static "fullcalendar/fullcalendar.min.js" %}"></script>
 {% endblock %}
 {% block body %}
-
+<div id="main-content">
 <div id="sidebar" class="application-sidebar">
 	<div class="btn-group sidebar-item">
 		<button type="button" class="btn btn-default dropdown-toggle" style="width:100%" data-toggle="dropdown">
 			<span id="event_type">Reservations</span>
 			<span class="caret"></span>
 		</button>
 		<ul class="dropdown-menu">
-			<li class="dropdown-header">Which type of events would you like<br>to view on the calendar?</li>
-			<li data-toggle="tooltip" data-placement="right" title="Displays {% if tools and areas %}tool and area{% elif tools %}tool{% elif areas %}area{% endif %} reservations. While viewing reservations, the 'Personal schedule' link shows your reservations for all {% if tools and areas %}tools and areas{% elif tools %}tools{% elif areas %}areas{% endif %}. Select a {% if tools and areas %}tool or area{% elif tools %}tool{% elif areas %}area{% endif %} to view everyone's reservations for that {% if tools and areas %}tool or area{% elif tools %}tool{% elif areas %}area{% endif %}."><a href="javascript:void(0)" onclick="change_calendar_event_type(this)">Reservations</a></li>
-			<li data-toggle="tooltip" data-placement="right" title="Displays your {{ facility_name }} usage. This includes{% if areas %} area access,{% endif %}{% if tools %} tool usage,{% endif %} and missed reservations (which are all billable items)."><a href="javascript:void(0)" onclick="change_calendar_event_type(this)">{{ facility_name }} usage</a></li>
+			<li class="dropdown-header" id="event_type_help">Which type of events would you like<br>to view on the calendar?</li>
+			<li data-toggle="tooltip" data-placement="right" title="Displays {% if tools and areas %}tool and area{% elif tools %}tool{% elif areas %}area{% endif %} reservations. While viewing reservations, the 'Personal schedule' link shows your reservations for all {% if tools and areas %}tools and areas{% elif tools %}tools{% elif areas %}areas{% endif %}. Select a {% if tools and areas %}tool or area{% elif tools %}tool{% elif areas %}area{% endif %} to view everyone's reservations for that {% if tools and areas %}tool or area{% elif tools %}tool{% elif areas %}area{% endif %}."><a aria-describedby="event_type_help" href="javascript:void(0)" onclick="change_calendar_event_type(this)">Reservations</a></li>
+			<li data-toggle="tooltip" data-placement="right" title="Displays your {{ facility_name }} usage. This includes{% if areas %} area access,{% endif %}{% if tools %} tool usage,{% endif %} and missed reservations (which are all billable items)."><a aria-describedby="event_type_help" href="javascript:void(0)" onclick="change_calendar_event_type(this)">{{ facility_name }} usage</a></li>
 			{% if user.is_staff %}
-				<li data-toggle="tooltip" data-placement="right" title="Displays {{ facility_name }} reservations and usage for a specific user. This includes reservations, area access, tool usage, and missed reservations."><a href="javascript:void(0)" onclick="change_calendar_event_type(this)">Specific user</a></li>
+				<li data-toggle="tooltip" data-placement="right" title="Displays {{ facility_name }} reservations and usage for a specific user. This includes reservations, area access, tool usage, and missed reservations."><a aria-describedby="event_type_help" href="javascript:void(0)" onclick="change_calendar_event_type(this)">Specific user</a></li>
 			{% endif %}
 		</ul>
 	</div>
 	<div id="expand-collapse" class="btn-group sidebar-item">
-        {% if calendar_qualified_tools and not user.is_staff  %}
-            <button type="button" class="btn btn-default" style="width:33%" onclick="expand_all_categories()" title="Expand all categories"><span class="glyphicon glyphicon-resize-full"></span></button>
-            <button type="button" class="btn btn-default" style="width:33%" onclick="collapse_all_categories()" title="Collapse all categories"><span class="glyphicon glyphicon-resize-small"></span></button>
-            <button type="button" class="btn btn-default" id="qualified_tools_btn" style="width:34%" onclick="toggle_qualified_tools(retrieve_user_qualifications())" title="Only show qualified tools"><span class="glyphicon glyphicon-check"></span></button>
+        {% if calendar_qualified_tools and not user.is_staff %}
+            <button type="button" class="btn btn-default" style="width:50%" onclick="toggle_categories()" title="Expand/collapse all categories"><span id="expand_collapse_icon" class="glyphicon glyphicon"></span></button>
+            <button type="button" class="btn btn-default" id="qualified_tools_btn" style="width:50%" onclick="toggle_qualified_tools(retrieve_user_qualifications())" title="Only show qualified tools"><span class="glyphicon glyphicon-check"></span></button>
         {% else %}
-            <button type="button" class="btn btn-default" style="width:50%" onclick="expand_all_categories()" title="Expand all categories"><span class="glyphicon glyphicon-resize-full"></span></button>
-            <button type="button" class="btn btn-default" style="width:50%" onclick="collapse_all_categories()" title="Collapse all categories"><span class="glyphicon glyphicon-resize-small"></span></button>
+            <button type="button" class="btn btn-default" style="width:100%" onclick="toggle_categories()" title="Expand/collapse all categories"><span id="expand_collapse_icon" class="glyphicon glyphicon"></span></button>
         {% endif %}
 	</div>
-	<input type="text" id="item_search" placeholder="Search for{% if tools %} a tool{% endif %}{% if tools and areas %} or{% endif %}{% if areas %} an area{% endif %}" class="form-control sidebar-item" autocomplete="off">
-	<input type="text" id="user_search" placeholder="Search for a user" class="form-control sidebar-item" autocomplete="off" style="display:none">
+	<input aria-label="Search for a tool or area" type="search" id="item_search" placeholder="Search for{% if tools %} a tool{% endif %}{% if tools and areas %} or{% endif %}{% if areas %} an area{% endif %}" class="form-control sidebar-item" autocomplete="off">
+	<input aria-label="Search for a user" type="search" id="user_search" placeholder="Search for a user" class="form-control sidebar-item" autocomplete="off" style="display:none">
 	<button id="chosen_user_button" type="button" class="btn btn-default" style="width:100%; display:none" onclick="clear_specific_user()"></button>
 
 	{# The following menu tree code was take from an example at http://www.bootply.com/120625 #}
 	<ul id="extra-links" class="nav nav-list" style="margin-top: 10px; margin-bottom: 8px;">
 		<li><a href="javascript:void(0)" class="selected personal_schedule" data-item-id="personal_schedule" onclick="set_selected_item(this); update_event_sources()">Personal schedule</a></li>
 		{% if calendar_all_tools %}
 		<li><a href="javascript:void(0)" class="all_tools" data-item-id="all_tools" onclick="set_selected_item(this); update_event_sources()">All tools</a></li>
@@ -93,15 +91,15 @@
 		}
 	};
 
 	if(event_type === 'reservations' || event_type === '{{ facility_name|lower }} usage')
 	{
 		let item = get_selected_item();
 		let scheduled_outage_button = $(".fc-scheduledOutage-button")[0];
-		$(scheduled_outage_button).addClass('fc-state-disabled');
+		$(scheduled_outage_button).attr("disabled", "true").addClass('fc-state-disabled');
 		if(item === 'personal_schedule')
 		{
 			item_event_source.data.personal_schedule = true;
 		}
 		else if(item === 'all_tools')
 		{
 			item_event_source.data.all_tools = true;
@@ -115,15 +113,15 @@
 			item_event_source.data.all_areastools = true;
 		}
 		else if(item)
 		{
 			item = JSON.parse(item)
 			item_event_source.data.item_id = item.id;
 			item_event_source.data.item_type = item.type;
-			$(scheduled_outage_button).removeClass('fc-state-disabled');
+			$(scheduled_outage_button).removeAttr("disabled").removeClass('fc-state-disabled');
 		}
 	}
 	else if(event_type === 'specific user')
 	{
 		let user_search = $("#user_search");
 		if(user_search.typeahead('val'))
 			item_event_source.data.user = user_search.typeahead('val');
@@ -354,14 +352,28 @@
 
 function set_reservation_title(url, reservation_id, title)
 {
 	let failure_dialog = ajax_failure_callback("Unable to set reservation title");
 	ajax_post(url, {'title': title}, refresh_calendar_and_sidebar, [failure_dialog, refresh_calendar_and_sidebar]);
 }
 
+function change_reservation_date(url, reservation_id, param, value)
+{
+    let data = {'id': reservation_id};
+    data[param] = value;
+    let post_data =
+    {
+        "url": url,
+        "data": data,
+        "type": "POST",
+        "dataType": "html"
+    };
+    ajax_post(url, data, function(response, status, xml_http_request) { return event_creation_success_callback(response, status, xml_http_request, post_data) }, [ajax_failure_callback("Reservation date changed failed")], refresh_calendar_and_sidebar)
+}
+
 function change_reservation_project(url, project_id)
 {
 	let failure_dialog = ajax_failure_callback("Unable to change reservation project");
 	ajax_post(url, {'project_id': project_id}, refresh_calendar_and_sidebar, [failure_dialog, refresh_calendar_and_sidebar]);
 }
 
 function on_browser_resize()
@@ -670,9 +682,9 @@
 	$('[data-toggle~="tooltip"]').tooltip({ container: 'body' });
 	refresh_calendar_login();
 }
 
 $(on_load);
 
 </script>
-
+</div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -7,22 +7,22 @@
     * Which type of events would you like
       to view on the calendar?
     * Reservations
     * {{_facility_name_}}_usage
     * {% if user.is_staff %}
     * Specific_user
     * {% endif %}
-{% if calendar_qualified_tools and not user.is_staff %}    {% else %}   {%
-endif %}
-[                    ] [                    ]  {# The following menu tree code
-was take from an example at http://www.bootply.com/120625 #}
+{% if calendar_qualified_tools and not user.is_staff %}   {% else %}  {% endif
+%}
+[Unknown INPUT type] [Unknown INPUT type]  {# The following menu tree code was
+take from an example at http://www.bootply.com/120625 #}
     * Personal_schedule
     * {% if calendar_all_tools %}
     * All_tools
     * {% endif %} {% if calendar_all_areas %}
     * All_areas
     * {% endif %} {% if calendar_all_areastools %}
     * All_areas_and_tools
     * {% endif %}
 {# The item tree has the HTML class tag "item_tree". See the widgets/
 item_tree.py file for more information. #} {{ rendered_item_tree_html }}
- {% endblock %}
+{% endblock %}
```

### Comparing `NEMO-4.5.5/NEMO/templates/calendar/configuration.html` & `NEMO-4.6.0/NEMO/templates/calendar/configuration.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% load custom_tags_and_filters %}
 <div class="modal-header">
-	<button type="button" class="close" data-dismiss="modal">&times;</button>
-	<h4 class="modal-title">Choose tool configuration</h4>
+	<button type="button" class="close" data-dismiss="modal" aria-label="Modal close button">&times;</button>
+	<h4 id="modal-description-label" class="modal-title">Choose tool configuration</h4>
 </div>
 
 <div class="modal-body">
 	{# Assume the dialog is cancelled by default, preventing the reservation request from being processed further. #}
 	{# When a button is clicked this value is set to false, enabling further processing. #}
 	{# Hiding the dialog using the X in the top right, or clicking outside of it, will stop processing. #}
 	<input type="hidden" id="dialog_cancelled" value="true">
```

### Comparing `NEMO-4.5.5/NEMO/templates/calendar/configuration_helper.html` & `NEMO-4.6.0/NEMO/templates/calendar/configuration_helper.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/calendar/policy_dialog.html` & `NEMO-4.6.0/NEMO/templates/calendar/policy_dialog.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% load custom_tags_and_filters %}
 <div class="modal-header">
-	<button type="button" class="close" data-dismiss="modal">&times;</button>
-	<h4 class="modal-title">{{ facility_name }} policy conflict</h4>
+	<button type="button" class="close" data-dismiss="modal" aria-label="Modal close button">&times;</button>
+	<h4 id="modal-description-label" class="modal-title">{{ facility_name }} policy conflict</h4>
 </div>
 
 <div class="modal-body">
 	<p>This reservation conflicts with {{ facility_name }} policy.{% if overridable %} The policy <span style="font-weight:bold">can</span> be overridden.{% endif %}</p>
 	<ul>
 		{% for reason in policy_problems %}
 			<li>{{ reason }}</li>
```

### Comparing `NEMO-4.5.5/NEMO/templates/calendar/project_choice.html` & `NEMO-4.6.0/NEMO/templates/calendar/project_choice.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% load custom_tags_and_filters %}
 <div class="modal-header">
-	<button type="button" class="close" data-dismiss="modal">&times;</button>
-	<h4 class="modal-title">Which project is this for?</h4>
+	<button type="button" class="close" data-dismiss="modal" aria-label="Modal close button">&times;</button>
+	<h4 id="modal-description-label" class="modal-title">Which project is this for?</h4>
 </div>
 
 <div class="modal-body">
 	{# Assume the dialog is cancelled by default, preventing the reservation request from being processed further. #}
 	{# When a button is clicked this value is set to true, enabling further processing. #}
 	{# Hiding the dialog using the X in the top right, or clicking outside of it, will stop processing. #}
 	<input type="hidden" id="dialog_cancelled" value="true">
```

### Comparing `NEMO-4.5.5/NEMO/templates/calendar/proxy_reservation.html` & `NEMO-4.6.0/NEMO/templates/calendar/proxy_reservation.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 {% load custom_tags_and_filters %}
-
 <div class="modal-header">
-	<button type="button" class="close" data-dismiss="modal">&times;</button>
-	<h4 class="modal-title">Make a reservation for someone else</h4>
+	<button type="button" class="close" data-dismiss="modal" aria-label="Modal close button">&times;</button>
+	<h4 id="modal-description-label" class="modal-title">Make a reservation for someone else</h4>
 </div>
 
 <div class="modal-body">
-	<p>
+	<p id="proxy-reservation-description">
 		You can make reservations for another user by searching for and selecting the user below. Any reservations you make after that will be made for the selected user.
 		When you are done making reservations for another user, click the button that says &quot;Reserving as [user]&quot; at the top of the calendar.
 	</p>
 	<p>
 		While you are making reservations for someone else, all validation checks apply as if you are that user.
 		Likewise, error messages are displayed as if you are that person.
 	</p>
-	<input id="proxy_reservation" type="text" class="form-control" placeholder="Search for a user">
+	<input aria-label="Search for a user" aria-describedby="proxy-reservation-description" id="proxy_reservation" type="search" class="form-control" placeholder="Search for a user">
 </div>
 
 <script>
 	$("#proxy_reservation").autocomplete('users', proxy_reservation, {{ users|json_search_base }});
 	autofocus('#proxy_reservation');
 	function proxy_reservation(jquery_event, search_selection)
 	{
```

#### html2text {}

```diff
@@ -4,8 +4,8 @@
 You can make reservations for another user by searching for and selecting the
 user below. Any reservations you make after that will be made for the selected
 user. When you are done making reservations for another user, click the button
 that says "Reserving as [user]" at the top of the calendar.
 While you are making reservations for someone else, all validation checks apply
 as if you are that user. Likewise, error messages are displayed as if you are
 that person.
-[                    ]
+[Unknown INPUT type]
```

### Comparing `NEMO-4.5.5/NEMO/templates/calendar/reservation_event_feed.html` & `NEMO-4.6.0/NEMO/templates/calendar/reservation_event_feed.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/calendar/reservation_questions.html` & `NEMO-4.6.0/NEMO/templates/calendar/reservation_questions.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% load custom_tags_and_filters %}
 <div class="modal-header">
-	<button type="button" class="close" data-dismiss="modal">&times;</button>
-	<h4 class="modal-title">Reservation questions</h4>
+	<button type="button" class="close" data-dismiss="modal" aria-label="Modal close button">&times;</button>
+	<h4 id="modal-description-label" class="modal-title">Reservation questions</h4>
 </div>
 
 <div class="modal-body">
 	<p>This reservation requires extra information to be provided:</p>
     {% if error %}
         <div class="alert alert-danger">
 			Oops! Something went wrong. Please correct the errors highlighted below.<br><br>
```

### Comparing `NEMO-4.5.5/NEMO/templates/calendar/reservation_warning.html` & `NEMO-4.6.0/NEMO/templates/calendar/reservation_warning.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/calendar/scheduled_outage_information.html` & `NEMO-4.6.0/NEMO/templates/calendar/scheduled_outage_information.html`

 * *Files 6% similar despite different names*

```diff
@@ -2,43 +2,46 @@
 {% load custom_tags_and_filters %}
 {% block extrahead %}
     <script type="text/javascript" src="{% static "datetimepicker/bootstrap-datetimepicker.js" %}"></script>
 	<link rel="stylesheet" type="text/css" href="{% static "datetimepicker/bootstrap-datetimepicker.css" %}"/>
 {% endblock %}
 
 <div class="modal-header">
-	<button type="button" class="close" data-dismiss="modal">&times;</button>
-	<h4 class="modal-title">Schedule an outage</h4>
+	<button type="button" class="close" data-dismiss="modal" aria-label="Modal close button">&times;</button>
+	<h4 id="modal-description-label" class="modal-title">Schedule an outage</h4>
 </div>
 
 <div class="modal-body clearfix">
 	{# Assume the dialog is cancelled by default, preventing the scheduled outage request from being processed further. #}
 	{# When a button is clicked this value is set to false, enabling further processing. #}
 	{# Hiding the dialog using the X in the top right, or clicking outside of it, will stop processing. #}
 	<input type="hidden" id="dialog_cancelled" value="true">
 	<form id="additional_event_parameters" onsubmit="return false">
 		<input type="hidden" id="configured" name="configured" value="true">
 		<div class="form-group col-sm-12">
 			<label for="title">Title</label>
-			<input id="title" name="title" type="text" maxlength="100" class="form-control" autocomplete="off" placeholder="You must provide a title to create a scheduled outage">
+			<input aria-labelledby="outage_title_help" id="title" name="title" type="text" maxlength="100" class="form-control" autocomplete="off">
+            <div id="outage_title_help" class="light-grey">You must provide a title to create a scheduled outage</div>
 		</div>
 		{% if categories %}
 			<div class="form-group col-sm-12">
-				<label for="category">Category</label><span class="light-grey"> - is there a category for this outage? This is useful for data and trend analysis</span>
-				<select class="form-control" name="category" id="category">
+				<label for="category">Category</label>
+				<select aria-labelledby="outage_category_help" class="form-control" name="category" id="category">
 					<option></option>
 					{% for c in categories %}
 						<option>{{ c }}</option>
 					{% endfor %}
 				</select>
+                <div id="outage_category_help" class="light-grey">Is there a category for this outage? This is useful for data and trend analysis</div>
 			</div>
 		{% endif %}
 		<div class="form-group col-sm-12">
 			<label for="details">Details</label>
-			<textarea name="details" id="details" rows="7" maxlength="3000" class="form-control" placeholder="Please provide any additional details for the scheduled outage. Be descriptive so that users understand why there is a scheduled outage."></textarea>
+			<textarea aria-labelledby="outage_details_help" name="details" id="details" rows="7" maxlength="3000" class="form-control"></textarea>
+            <div id="outage_details_help" class="light-grey">Please provide any additional details for the scheduled outage. Be descriptive so that users understand why there is a scheduled outage.</div>
 		</div>
 		<div class="col-sm-12">
 			<a onclick="toggle_details(this)" data-toggle="collapse" data-target="#recurrence" class="pointer" style="text-decoration: none">
 				<input type="checkbox" id="recurring_outage" name="recurring_outage"/>
 			</a>
 			<label for="recurring_outage" style="padding-left: 5px">Create more than one occurrence of this outage</label>
 		</div>
```

#### html2text {}

```diff
@@ -4,19 +4,23 @@
 ×
 *** Schedule an outage ***
 {# Assume the dialog is cancelled by default, preventing the scheduled outage
 request from being processed further. #} {# When a button is clicked this value
 is set to false, enabling further processing. #} {# Hiding the dialog using the
 X in the top right, or clicking outside of it, will stop processing. #}
 Title [title               ]
+You must provide a title to create a scheduled outage
 {% if categories %}
 {% for c in categories %}
 {{ c }}
 {% endfor %}
+Is there a category for this outage? This is useful for data and trend analysis
 {% endif %}
+Please provide any additional details for the scheduled outage. Be descriptive
+so that users understand why there is a scheduled outage.
 ⁰ Create more than one occurrence of this outage
 Every [Unknown INPUT type]
 {% for choice in recurrence_intervals %}
 {{ choice.1 }}
 {% endfor %}
 Until: [recurrence_until    ]
 {% button id="schedule_outage" type="save" disabled="disabled" submit=False
```

### Comparing `NEMO-4.5.5/NEMO/templates/calendar/specific_user_feed.html` & `NEMO-4.6.0/NEMO/templates/calendar/specific_user_feed.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/calendar/usage_event_feed.html` & `NEMO-4.6.0/NEMO/templates/calendar/usage_event_feed.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/configuration_agenda.html` & `NEMO-4.6.0/NEMO/templates/configuration_agenda.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/consumables/consumables.html` & `NEMO-4.6.0/NEMO/templates/consumables/consumables.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 {% extends 'base.html' %}
 {% load custom_tags_and_filters %}
 {% block title %}Withdraw consumables{% endblock %}
 {% block content %}
 	<h1>Withdraw consumables</h1>
     <div style="height: 15px"></div>
     <div class="col-md-5">
-        <p>Use this form to charge users for consumable items & supplies.</p>
+        <p>Use this form to {% if self_checkout %}checkout{% else %}charge users for{% endif %} consumable items & supplies.</p>
         <form id="withdrawal_form_order" action="{% url 'consumables' %}" class="form-horizontal" method="post">
             {% csrf_token %}
-
-            <div class="form-group">
-                <label class="control-label col-md-3" for="customer_search">Customer</label>
-                <div class="col-md-9">
-                    <input type="text" class="form-control" id="customer_search" placeholder="Search for a customer" required>
-                    <input type="button" id="chosen_customer" class="btn btn-default" style="display:none" onclick="clear_selected_customer()">
-                    <input type="hidden" id="customer" name="customer">
+            {% if not self_checkout %}
+                <div class="form-group">
+                    <label class="control-label col-md-3" for="customer_search">Customer</label>
+                    <div class="col-md-9">
+                        <input type="text" class="form-control" id="customer_search" placeholder="Search for a customer" required>
+                        <input type="button" id="chosen_customer" class="btn btn-default" style="display:none" onclick="clear_selected_customer()" aria-label="Selected customer">
+                        <input type="hidden" id="customer" name="customer">
+                    </div>
                 </div>
-            </div>
+            {% endif %}
 
             <div class="form-group">
                 <label class="control-label col-md-3" for="project">Project</label>
                 <div class="col-md-9">
                     <select id="project" name="project" class="form-control" {% if not projects %}disabled{% endif %} required>
                         {% if projects|length == 0 %}
                             <option></option>
```

### Comparing `NEMO-4.5.5/NEMO/templates/consumables/consumables_order.html` & `NEMO-4.6.0/NEMO/templates/consumables/consumables_order.html`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     <table class="table table-condensed table-striped thead-light">
         <thead>
             <tr>
                 <th>Customer</th>
                 <th>Project</th>
                 <th>Consumable</th>
                 <th>Quantity</th>
-                <th></th>
+                <th aria-label="Action"></th>
             </tr>
         </thead>
         {% for withdraw in request.session.withdrawals %}
             <tr>
                 <td>{{ withdraw.customer }}</td>
                 <td>{{ withdraw.project }}</td>
                 <td>{{ withdraw.consumable }}</td>
```

### Comparing `NEMO-4.5.5/NEMO/templates/consumables/recurring_charge.html` & `NEMO-4.6.0/NEMO/templates/consumables/recurring_charge.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/consumables/recurring_charges.html` & `NEMO-4.6.0/NEMO/templates/consumables/recurring_charges.html`

 * *Files 2% similar despite different names*

```diff
@@ -34,20 +34,20 @@
                 <th>Next charge</th>
                 <th>Actions</th>
             </tr>
         </thead>
         <tbody>
             {% now "Y-m-d" as today_date %}
             {% for recurring_charge in page %}
-                <tr {% if not recurring_charge.is_empty and not recurring_charge.next_charge %}class="alert-danger" data-toggle="tooltip" data-title="This item expired"{% endif %}>
+                <tr {% if not recurring_charge.is_empty and not recurring_charge.next_charge %}class="danger" data-toggle="tooltip" data-title="This item expired"{% endif %}>
                     <td>{{ recurring_charge.name }}</td>
                     {% if different_quantities|length != 1 or page.0.quantity != 1 %}<td>{{ recurring_charge.quantity }}</td>{% endif %}
                     <td>{{ recurring_charge.consumable }}</td>
-                    <td {% if recurring_charge.invalid_customer %}class="alert-danger" data-toggle="tooltip" data-title="{{ recurring_charge.invalid_customer|default:'' }}"{% endif %}>{{ recurring_charge.customer|default_if_none:"" }}</td>
-                    <td {% if recurring_charge.invalid_project %}class="alert-danger" data-toggle="tooltip" data-title="{{ recurring_charge.invalid_project|default:'' }}"{% endif %}>{{ recurring_charge.project|default_if_none:"" }}</td>
+                    <td {% if recurring_charge.invalid_customer %}class="danger" data-toggle="tooltip" data-title="{{ recurring_charge.invalid_customer|default:'' }}"{% endif %}>{{ recurring_charge.customer|default_if_none:"" }}</td>
+                    <td {% if recurring_charge.invalid_project %}class="danger" data-toggle="tooltip" data-title="{{ recurring_charge.invalid_project|default:'' }}"{% endif %}>{{ recurring_charge.project|default_if_none:"" }}</td>
                     <td style="white-space: nowrap;">{% if recurring_charge.get_recurrence_interval_display %}{{ recurring_charge.get_recurrence_interval_display }} <span class="glyphicon glyphicon-info-sign primary-highlight" style="vertical-align: text-bottom" data-toggle="tooltip" data-title="{{ recurring_charge.get_recurrence_display|default_if_none:'' }}"></span>{% endif %}</td>
                     <td>{{ recurring_charge.last_charge|date:'SHORT_DATE_FORMAT' }}</td>
                     <td>{{ recurring_charge.next_charge|date:'SHORT_DATE_FORMAT' }}</td>
                     <td class="button-column-minimum">
                         {% url "edit_recurring_charge" recurring_charge.id as edit_charge %}
                         {% url "clear_recurring_charge" recurring_charge.id as clear_charge %}
                         {% url "delete_recurring_charge" recurring_charge.id as delete_charge %}
```

### Comparing `NEMO-4.5.5/NEMO/templates/contact/contact_staff.html` & `NEMO-4.6.0/NEMO/templates/contact/contact_staff.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/customizations/customizations.html` & `NEMO-4.6.0/NEMO/templates/customizations/customizations.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/customizations/customizations_application.html` & `NEMO-4.6.0/NEMO/templates/rest_framework/api.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,145 +1,171 @@
-00000000: 7b25 206c 6f61 6420 6375 7374 6f6d 5f74  {% load custom_t
-00000010: 6167 735f 616e 645f 6669 6c74 6572 7320  ags_and_filters 
-00000020: 257d 0a3c 6469 7620 636c 6173 733d 2270  %}.<div class="p
-00000030: 616e 656c 2d62 6f64 7922 3e0a 2020 2020  anel-body">.    
-00000040: 3c68 3320 636c 6173 733d 2263 7573 746f  <h3 class="custo
-00000050: 6d69 7a61 7469 6f6e 2d73 6563 7469 6f6e  mization-section
-00000060: 2d74 6974 6c65 223e 4170 706c 6963 6174  -title">Applicat
-00000070: 696f 6e20 7365 7474 696e 6773 3c2f 6833  ion settings</h3
-00000080: 3e0a 2020 2020 3c66 6f72 6d20 6d65 7468  >.    <form meth
-00000090: 6f64 3d22 504f 5354 2220 6163 7469 6f6e  od="POST" action
-000000a0: 3d22 7b25 2075 726c 2027 6375 7374 6f6d  ="{% url 'custom
-000000b0: 697a 6527 2027 6170 706c 6963 6174 696f  ize' 'applicatio
-000000c0: 6e27 2025 7d22 2063 6c61 7373 3d22 666f  n' %}" class="fo
-000000d0: 726d 2d68 6f72 697a 6f6e 7461 6c22 3e0a  rm-horizontal">.
-000000e0: 2020 2020 2020 2020 7b25 2063 7372 665f          {% csrf_
-000000f0: 746f 6b65 6e20 257d 0a20 2020 2020 2020  token %}.       
-00000100: 203c 6469 7620 636c 6173 733d 2266 6f72   <div class="for
-00000110: 6d2d 6772 6f75 7022 3e0a 2020 2020 2020  m-group">.      
-00000120: 2020 2020 2020 3c6c 6162 656c 2063 6c61        <label cla
-00000130: 7373 3d22 636f 6e74 726f 6c2d 6c61 6265  ss="control-labe
-00000140: 6c20 636f 6c2d 6d64 2d32 2220 666f 723d  l col-md-2" for=
-00000150: 2266 6163 696c 6974 795f 6e61 6d65 223e  "facility_name">
-00000160: 4661 6369 6c69 7479 206e 616d 653c 2f6c  Facility name</l
-00000170: 6162 656c 3e0a 2020 2020 2020 2020 2020  abel>.          
-00000180: 2020 3c64 6976 2063 6c61 7373 3d22 636f    <div class="co
-00000190: 6c2d 6d64 2d35 223e 0a20 2020 2020 2020  l-md-5">.       
-000001a0: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
-000001b0: 7479 7065 3d22 7465 7874 2220 6964 3d22  type="text" id="
-000001c0: 6661 6369 6c69 7479 5f6e 616d 6522 206e  facility_name" n
-000001d0: 616d 653d 2266 6163 696c 6974 795f 6e61  ame="facility_na
-000001e0: 6d65 2220 636c 6173 733d 2266 6f72 6d2d  me" class="form-
-000001f0: 636f 6e74 726f 6c22 2076 616c 7565 3d22  control" value="
-00000200: 7b7b 2066 6163 696c 6974 795f 6e61 6d65  {{ facility_name
-00000210: 207d 7d22 3e0a 2020 2020 2020 2020 2020   }}">.          
-00000220: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-00000230: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00000240: 2263 6f6c 2d6d 642d 3520 6865 6c70 2d62  "col-md-5 help-b
-00000250: 6c6f 636b 206c 6967 6874 2d67 7265 7922  lock light-grey"
-00000260: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000270: 2020 5468 6520 6e61 6d65 206f 6620 7468    The name of th
-00000280: 6520 6661 6369 6c69 7479 2074 6f20 7573  e facility to us
-00000290: 6520 696e 2061 6c6c 2074 656d 706c 6174  e in all templat
-000002a0: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
-000002b0: 3c2f 6469 763e 0a20 2020 2020 2020 203c  </div>.        <
-000002c0: 2f64 6976 3e0a 2020 2020 2020 2020 3c64  /div>.        <d
-000002d0: 6976 2063 6c61 7373 3d22 666f 726d 2d67  iv class="form-g
-000002e0: 726f 7570 223e 0a20 2020 2020 2020 2020  roup">.         
-000002f0: 2020 203c 6c61 6265 6c20 636c 6173 733d     <label class=
-00000300: 2263 6f6e 7472 6f6c 2d6c 6162 656c 2063  "control-label c
-00000310: 6f6c 2d6d 642d 3222 2066 6f72 3d22 7369  ol-md-2" for="si
-00000320: 7465 5f74 6974 6c65 223e 5369 7465 2074  te_title">Site t
-00000330: 6974 6c65 3c2f 6c61 6265 6c3e 0a20 2020  itle</label>.   
-00000340: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00000350: 6173 733d 2263 6f6c 2d6d 642d 3522 3e0a  ass="col-md-5">.
-00000360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000370: 3c69 6e70 7574 2074 7970 653d 2274 6578  <input type="tex
-00000380: 7422 2069 643d 2273 6974 655f 7469 746c  t" id="site_titl
-00000390: 6522 206e 616d 653d 2273 6974 655f 7469  e" name="site_ti
-000003a0: 746c 6522 2063 6c61 7373 3d22 666f 726d  tle" class="form
-000003b0: 2d63 6f6e 7472 6f6c 2220 7661 6c75 653d  -control" value=
-000003c0: 227b 7b20 7369 7465 5f74 6974 6c65 207d  "{{ site_title }
-000003d0: 7d22 3e0a 2020 2020 2020 2020 2020 2020  }">.            
-000003e0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-000003f0: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
-00000400: 6f6c 2d6d 642d 3520 6865 6c70 2d62 6c6f  ol-md-5 help-blo
-00000410: 636b 206c 6967 6874 2d67 7265 7922 3e0a  ck light-grey">.
-00000420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000430: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
-00000440: 7369 7465 2074 6f20 7573 6520 696e 2061  site to use in a
-00000450: 6c6c 2074 656d 706c 6174 6573 2f68 6561  ll templates/hea
-00000460: 6465 7273 2e0a 2020 2020 2020 2020 2020  ders..          
-00000470: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-00000480: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00000490: 3c64 6976 2063 6c61 7373 3d22 666f 726d  <div class="form
-000004a0: 2d67 726f 7570 223e 0a20 2020 2020 2020  -group">.       
-000004b0: 2020 2020 203c 6c61 6265 6c20 636c 6173       <label clas
-000004c0: 733d 2263 6f6e 7472 6f6c 2d6c 6162 656c  s="control-label
-000004d0: 2063 6f6c 2d6d 642d 3222 3e41 7265 6120   col-md-2">Area 
-000004e0: 6c6f 6769 6e2f 6c6f 676f 7574 3c2f 6c61  login/logout</la
-000004f0: 6265 6c3e 0a20 2020 2020 2020 2020 2020  bel>.           
-00000500: 203c 6469 7620 636c 6173 733d 2263 6f6c   <div class="col
-00000510: 2d6d 642d 3130 223e 0a20 2020 2020 2020  -md-10">.       
-00000520: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00000530: 6173 733d 2263 6865 636b 626f 7822 3e0a  ass="checkbox">.
-00000540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000550: 2020 2020 3c6c 6162 656c 3e3c 696e 7075      <label><inpu
-00000560: 7420 7479 7065 3d22 6368 6563 6b62 6f78  t type="checkbox
-00000570: 2220 6e61 6d65 3d22 7365 6c66 5f6c 6f67  " name="self_log
-00000580: 5f69 6e22 207b 2520 6966 2073 656c 665f  _in" {% if self_
-00000590: 6c6f 675f 696e 2025 7d63 6865 636b 6564  log_in %}checked
-000005a0: 7b25 2065 6e64 6966 2025 7d20 7661 6c75  {% endif %} valu
-000005b0: 653d 2265 6e61 626c 6564 223e 416c 6c6f  e="enabled">Allo
-000005c0: 7720 7573 6572 7320 746f 206c 6f67 2074  w users to log t
-000005d0: 6865 6d73 656c 7665 7320 696e 746f 2061  hemselves into a
-000005e0: 6363 6573 7320 636f 6e74 726f 6c6c 6564  ccess controlled
-000005f0: 2061 7265 6173 2066 726f 6d20 7468 6520   areas from the 
-00000600: 6c61 6e64 696e 6720 7061 6765 3c2f 6c61  landing page</la
-00000610: 6265 6c3e 3c62 722f 3e0a 2020 2020 2020  bel><br/>.      
-00000620: 2020 2020 2020 2020 2020 2020 2020 3c6c                <l
-00000630: 6162 656c 3e3c 696e 7075 7420 7479 7065  abel><input type
-00000640: 3d22 6368 6563 6b62 6f78 2220 6e61 6d65  ="checkbox" name
-00000650: 3d22 7365 6c66 5f6c 6f67 5f6f 7574 2220  ="self_log_out" 
-00000660: 7b25 2069 6620 7365 6c66 5f6c 6f67 5f6f  {% if self_log_o
-00000670: 7574 2025 7d63 6865 636b 6564 7b25 2065  ut %}checked{% e
-00000680: 6e64 6966 2025 7d20 7661 6c75 653d 2265  ndif %} value="e
-00000690: 6e61 626c 6564 223e 416c 6c6f 7720 7573  nabled">Allow us
-000006a0: 6572 7320 746f 206c 6f67 2074 6865 6d73  ers to log thems
-000006b0: 656c 7665 7320 6f75 7420 6f66 2061 6363  elves out of acc
-000006c0: 6573 7320 636f 6e74 726f 6c6c 6564 2061  ess controlled a
-000006d0: 7265 6173 2066 726f 6d20 7468 6520 6c61  reas from the la
-000006e0: 6e64 696e 6720 7061 6765 3c2f 6c61 6265  nding page</labe
-000006f0: 6c3e 3c62 722f 3e0a 2020 2020 2020 2020  l><br/>.        
-00000700: 2020 2020 2020 2020 2020 2020 3c6c 6162              <lab
-00000710: 656c 3e3c 696e 7075 7420 7479 7065 3d22  el><input type="
-00000720: 6368 6563 6b62 6f78 2220 6e61 6d65 3d22  checkbox" name="
-00000730: 6361 6c65 6e64 6172 5f6c 6f67 696e 5f6c  calendar_login_l
-00000740: 6f67 6f75 7422 207b 2520 6966 2063 616c  ogout" {% if cal
-00000750: 656e 6461 725f 6c6f 6769 6e5f 6c6f 676f  endar_login_logo
-00000760: 7574 2025 7d63 6865 636b 6564 7b25 2065  ut %}checked{% e
-00000770: 6e64 6966 2025 7d20 7661 6c75 653d 2265  ndif %} value="e
-00000780: 6e61 626c 6564 223e 5368 6f77 2061 6363  nabled">Show acc
-00000790: 6573 7320 636f 6e74 726f 6c6c 6564 2061  ess controlled a
-000007a0: 7265 6120 6c6f 6769 6e2f 6c6f 676f 7574  rea login/logout
-000007b0: 2062 7574 746f 6e20 6f6e 2063 616c 656e   button on calen
-000007c0: 6461 7220 7669 6577 2028 7265 7175 6972  dar view (requir
-000007d0: 6573 206c 6f67 696e 2061 6e64 2f6f 7220  es login and/or 
-000007e0: 6c6f 676f 7574 2066 6561 7475 7265 2065  logout feature e
-000007f0: 6e61 626c 6564 2061 626f 7665 293c 2f6c  nabled above)</l
-00000800: 6162 656c 3e0a 2020 2020 2020 2020 2020  abel>.          
-00000810: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-00000820: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00000830: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00000840: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00000850: 733d 2263 7573 746f 6d69 7a61 7469 6f6e  s="customization
-00000860: 2d73 6570 6172 6174 696f 6e22 2073 7479  -separation" sty
-00000870: 6c65 3d22 6d61 7267 696e 2d62 6f74 746f  le="margin-botto
-00000880: 6d3a 2031 3570 7822 3e3c 2f64 6976 3e0a  m: 15px"></div>.
-00000890: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-000008a0: 7373 3d22 7465 7874 2d63 656e 7465 7222  ss="text-center"
-000008b0: 3e0a 2020 2020 2020 2020 2020 2020 7b25  >.            {%
-000008c0: 2062 7574 746f 6e20 7479 7065 3d22 7361   button type="sa
-000008d0: 7665 2220 7661 6c75 653d 2253 6176 6520  ve" value="Save 
-000008e0: 7365 7474 696e 6773 2220 257d 0a20 2020  settings" %}.   
-000008f0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-00000900: 3c2f 666f 726d 3e0a 3c2f 6469 763e       </form>.</div>
+00000000: 7b25 2065 7874 656e 6473 2022 7265 7374  {% extends "rest
+00000010: 5f66 7261 6d65 776f 726b 2f62 6173 652e  _framework/base.
+00000020: 6874 6d6c 2220 257d 0a20 2020 207b 2520  html" %}.    {% 
+00000030: 626c 6f63 6b20 636f 6e74 656e 7420 257d  block content %}
+00000040: 0a20 2020 2020 2020 207b 7b20 626c 6f63  .        {{ bloc
+00000050: 6b2e 7375 7065 7220 7d7d 0a20 2020 2020  k.super }}.     
+00000060: 2020 207b 2520 6966 2022 504f 5354 2220     {% if "POST" 
+00000070: 696e 2061 6c6c 6f77 6564 5f6d 6574 686f  in allowed_metho
+00000080: 6473 2061 6e64 2072 6177 5f64 6174 615f  ds and raw_data_
+00000090: 706f 7374 5f66 6f72 6d20 257d 0a20 2020  post_form %}.   
+000000a0: 2020 2020 2020 2020 203c 6469 7620 7374           <div st
+000000b0: 796c 653d 2264 6973 706c 6179 3a6e 6f6e  yle="display:non
+000000c0: 6522 3e0a 2020 2020 2020 2020 2020 2020  e">.            
+000000d0: 2020 2020 3c6c 6920 6964 3d22 6669 6c65      <li id="file
+000000e0: 2d69 6d70 6f72 742d 6e61 762d 7461 6222  -import-nav-tab"
+000000f0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000100: 2020 2020 2020 3c61 2069 643d 2766 696c        <a id='fil
+00000110: 652d 696d 706f 7274 2d74 6162 2720 6872  e-import-tab' hr
+00000120: 6566 3d22 2366 696c 652d 696d 706f 7274  ef="#file-import
+00000130: 2d66 6f72 6d22 2064 6174 612d 746f 6767  -form" data-togg
+00000140: 6c65 3d22 7461 6222 3e46 696c 6520 696d  le="tab">File im
+00000150: 706f 7274 3c2f 613e 0a20 2020 2020 2020  port</a>.       
+00000160: 2020 2020 2020 2020 203c 2f6c 693e 0a0a           </li>..
+00000170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000180: 3c64 6976 2063 6c61 7373 3d22 7461 622d  <div class="tab-
+00000190: 7061 6e65 2220 6964 3d22 6669 6c65 2d69  pane" id="file-i
+000001a0: 6d70 6f72 742d 666f 726d 223e 0a20 2020  mport-form">.   
+000001b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001c0: 203c 666f 726d 2061 6374 696f 6e3d 227b   <form action="{
+000001d0: 2520 7572 6c20 2761 7069 5f66 696c 655f  % url 'api_file_
+000001e0: 696d 706f 7274 2720 257d 2220 656e 6374  import' %}" enct
+000001f0: 7970 653d 226d 756c 7469 7061 7274 2f66  ype="multipart/f
+00000200: 6f72 6d2d 6461 7461 2220 636c 6173 733d  orm-data" class=
+00000210: 2266 6f72 6d2d 686f 7269 7a6f 6e74 616c  "form-horizontal
+00000220: 2220 6d65 7468 6f64 3d22 504f 5354 2220  " method="POST" 
+00000230: 6e6f 7661 6c69 6461 7465 3e0a 2020 2020  novalidate>.    
+00000240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000250: 2020 2020 3c66 6965 6c64 7365 743e 0a20      <fieldset>. 
+00000260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000270: 2020 2020 2020 2020 2020 207b 2520 6373             {% cs
+00000280: 7266 5f74 6f6b 656e 2025 7d0a 2020 2020  rf_token %}.    
+00000290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002a0: 2020 2020 2020 2020 3c69 6e70 7574 2074          <input t
+000002b0: 7970 653d 2268 6964 6465 6e22 206e 616d  ype="hidden" nam
+000002c0: 653d 2272 6571 7565 7374 5f75 726c 2220  e="request_url" 
+000002d0: 7661 6c75 653d 227b 7b20 7265 7175 6573  value="{{ reques
+000002e0: 742e 6765 745f 6675 6c6c 5f70 6174 6820  t.get_full_path 
+000002f0: 7d7d 222f 3e0a 2020 2020 2020 2020 2020  }}"/>.          
+00000300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000310: 2020 3c64 6976 2063 6c61 7373 3d22 666f    <div class="fo
+00000320: 726d 2d67 726f 7570 223e 0a20 2020 2020  rm-group">.     
+00000330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000340: 2020 2020 2020 2020 2020 203c 6c61 6265             <labe
+00000350: 6c20 666f 723d 2266 696c 655f 666f 726d  l for="file_form
+00000360: 6174 7322 2063 6c61 7373 3d22 636f 6c2d  ats" class="col-
+00000370: 6c67 2d32 2063 6f6c 2d73 6d2d 3320 636f  lg-2 col-sm-3 co
+00000380: 6e74 726f 6c2d 6c61 6265 6c22 3e41 6363  ntrol-label">Acc
+00000390: 6570 7465 6420 6669 6c65 2066 6f72 6d61  epted file forma
+000003a0: 7473 3c2f 6c61 6265 6c3e 0a20 2020 2020  ts</label>.     
+000003b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003c0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+000003d0: 636c 6173 733d 2263 6f6c 2d6c 672d 3130  class="col-lg-10
+000003e0: 2063 6f6c 2d73 6d2d 3922 3e0a 2020 2020   col-sm-9">.    
+000003f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000410: 3c64 6976 2063 6c61 7373 3d22 666f 726d  <div class="form
+00000420: 2d63 6f6e 7472 6f6c 2d73 7461 7469 6322  -control-static"
+00000430: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000450: 2020 2020 2020 2020 2020 7b25 2066 6f72            {% for
+00000460: 2070 6172 7365 7220 696e 2061 7069 5f73   parser in api_s
+00000470: 6574 7469 6e67 732e 4445 4641 554c 545f  ettings.DEFAULT_
+00000480: 5041 5253 4552 5f43 4c41 5353 4553 2025  PARSER_CLASSES %
+00000490: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+000004a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004b0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+000004c0: 2069 6620 7061 7273 6572 2e6d 6564 6961   if parser.media
+000004d0: 5f74 7970 6520 213d 2022 6d75 6c74 6970  _type != "multip
+000004e0: 6172 742f 666f 726d 2d64 6174 6122 2025  art/form-data" %
+000004f0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00000500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000520: 2020 7b7b 2070 6172 7365 722e 6d65 6469    {{ parser.medi
+00000530: 615f 7479 7065 207d 7d7b 2520 6966 206e  a_type }}{% if n
+00000540: 6f74 2066 6f72 6c6f 6f70 2e6c 6173 7420  ot forloop.last 
+00000550: 257d 2c20 7b25 2065 6e64 6966 2025 7d0a  %}, {% endif %}.
+00000560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000580: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+00000590: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
+000005a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005c0: 7b25 2065 6e64 666f 7220 257d 0a20 2020  {% endfor %}.   
+000005d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005f0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+00000600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000610: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00000620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000630: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00000640: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000650: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00000660: 6976 2063 6c61 7373 3d22 666f 726d 2d67  iv class="form-g
+00000670: 726f 7570 223e 0a20 2020 2020 2020 2020  roup">.         
+00000680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000690: 2020 2020 2020 203c 6c61 6265 6c20 666f         <label fo
+000006a0: 723d 2269 6d70 6f72 745f 6669 6c65 2220  r="import_file" 
+000006b0: 636c 6173 733d 2263 6f6c 2d6c 672d 3220  class="col-lg-2 
+000006c0: 636f 6c2d 736d 2d33 2063 6f6e 7472 6f6c  col-sm-3 control
+000006d0: 2d6c 6162 656c 223e 4669 6c65 2074 6f20  -label">File to 
+000006e0: 696d 706f 7274 3c2f 6c61 6265 6c3e 0a20  import</label>. 
+000006f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000700: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000710: 6469 7620 636c 6173 733d 2263 6f6c 2d6c  div class="col-l
+00000720: 672d 3130 2063 6f6c 2d73 6d2d 3922 3e0a  g-10 col-sm-9">.
+00000730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000750: 2020 2020 3c69 6e70 7574 2074 7970 653d      <input type=
+00000760: 2266 696c 6522 2069 643d 2269 6d70 6f72  "file" id="impor
+00000770: 745f 6669 6c65 2220 6e61 6d65 3d22 696d  t_file" name="im
+00000780: 706f 7274 5f66 696c 6522 2063 6c61 7373  port_file" class
+00000790: 3d22 666f 726d 2d63 6f6e 7472 6f6c 2d73  ="form-control-s
+000007a0: 7461 7469 6322 2073 7479 6c65 3d22 626f  tatic" style="bo
+000007b0: 7264 6572 3a20 6e6f 6e65 3b20 626f 782d  rder: none; box-
+000007c0: 7368 6164 6f77 3a20 6e6f 6e65 3b20 6261  shadow: none; ba
+000007d0: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a20  ckground-color: 
+000007e0: 7472 616e 7370 6172 656e 7422 3e0a 2020  transparent">.  
+000007f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000800: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00000810: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00000820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000830: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+00000840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000850: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00000860: 666f 726d 2d61 6374 696f 6e73 223e 0a20  form-actions">. 
+00000870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000880: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000890: 6275 7474 6f6e 2063 6c61 7373 3d22 6274  button class="bt
+000008a0: 6e20 6274 6e2d 7072 696d 6172 7920 6a73  n btn-primary js
+000008b0: 2d74 6f6f 6c74 6970 2220 7469 746c 653d  -tooltip" title=
+000008c0: 224d 616b 6520 6120 504f 5354 2072 6571  "Make a POST req
+000008d0: 7565 7374 206f 6e20 7468 6520 7b7b 206e  uest on the {{ n
+000008e0: 616d 6520 7d7d 2072 6573 6f75 7263 6522  ame }} resource"
+000008f0: 3e50 4f53 543c 2f62 7574 746f 6e3e 0a20  >POST</button>. 
+00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000910: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00000920: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000930: 2020 2020 2020 2020 2020 3c2f 6669 656c            </fiel
+00000940: 6473 6574 3e0a 2020 2020 2020 2020 2020  dset>.          
+00000950: 2020 2020 2020 2020 2020 3c2f 666f 726d            </form
+00000960: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000970: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00000980: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00000990: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
+000009a0: 2020 2020 7b25 2065 6e64 626c 6f63 6b20      {% endblock 
+000009b0: 257d 0a20 2020 207b 2520 626c 6f63 6b20  %}.    {% block 
+000009c0: 7363 7269 7074 2025 7d0a 2020 2020 2020  script %}.      
+000009d0: 2020 7b7b 2062 6c6f 636b 2e73 7570 6572    {{ block.super
+000009e0: 207d 7d0a 2020 2020 2020 2020 3c73 6372   }}.        <scr
+000009f0: 6970 743e 0a20 2020 2020 2020 2020 2020  ipt>.           
+00000a00: 2024 2822 756c 2e6e 6176 2e6e 6176 2d74   $("ul.nav.nav-t
+00000a10: 6162 732e 666f 726d 2d73 7769 7463 6865  abs.form-switche
+00000a20: 7222 292e 7072 6570 656e 6428 2428 2223  r").prepend($("#
+00000a30: 6669 6c65 2d69 6d70 6f72 742d 6e61 762d  file-import-nav-
+00000a40: 7461 6222 2929 0a20 2020 2020 2020 2020  tab")).         
+00000a50: 2020 2024 2822 6469 762e 7765 6c6c 2e74     $("div.well.t
+00000a60: 6162 2d63 6f6e 7465 6e74 2229 2e61 7070  ab-content").app
+00000a70: 656e 6428 2428 2223 6669 6c65 2d69 6d70  end($("#file-imp
+00000a80: 6f72 742d 666f 726d 2229 290a 2020 2020  ort-form")).    
+00000a90: 2020 2020 3c2f 7363 7269 7074 3e0a 2020      </script>.  
+00000aa0: 2020 7b25 2065 6e64 626c 6f63 6b20 257d    {% endblock %}
```

### Comparing `NEMO-4.5.5/NEMO/templates/customizations/customizations_calendar.html` & `NEMO-4.6.0/NEMO/templates/customizations/customizations_calendar.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/customizations/customizations_emails.html` & `NEMO-4.6.0/NEMO/templates/customizations/customizations_emails.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/customizations/customizations_interlock.html` & `NEMO-4.6.0/NEMO/templates/customizations/customizations_interlock.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/customizations/customizations_projects_and_accounts.html` & `NEMO-4.6.0/NEMO/templates/customizations/customizations_projects_and_accounts.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/customizations/customizations_rates.html` & `NEMO-4.6.0/NEMO/templates/customizations/customizations_rates.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/customizations/customizations_recurring_charges.html` & `NEMO-4.6.0/NEMO/templates/customizations/customizations_recurring_charges.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/customizations/customizations_remote_work.html` & `NEMO-4.6.0/NEMO/templates/customizations/customizations_remote_work.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/customizations/customizations_requests.html` & `NEMO-4.6.0/NEMO/templates/customizations/customizations_requests.html`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                     {{ errors.adjustment_requests_time_limit_frequency.error }}
                 {% else %}
                     The timeframe for users to be able to request adjustment on charges.
                 {% endif %}
             </div>
         </div>
         <div class="form-group">
-            <label class="control-label col-md-4">Approved charges</label>
+            <label class="control-label col-md-4">Edit approved charges</label>
             <div class="col-md-8">
                 <div class="checkbox">
                     <label><input type="checkbox" name="adjustment_requests_edit_charge_button" {% if adjustment_requests_edit_charge_button %}checked{% endif %} value="enabled">Check this box to show a link to edit the original charge after approval</label><br/>
                 </div>
             </div>
             <div class="col-md-offset-4 col-md-8 help-block light-grey">
                 This does not apply to general charges.
```

### Comparing `NEMO-4.5.5/NEMO/templates/customizations/customizations_safety.html` & `NEMO-4.6.0/NEMO/templates/customizations/customizations_safety.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/customizations/customizations_templates.html` & `NEMO-4.6.0/NEMO/templates/customizations/customizations_templates.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/customizations/customizations_tool.html` & `NEMO-4.6.0/NEMO/templates/customizations/customizations_tool.html`

 * *Files 6% similar despite different names*

```diff
@@ -88,455 +88,492 @@
 00000570: 636b 6564 7b25 2065 6e64 6966 2025 7d20  cked{% endif %} 
 00000580: 7661 6c75 653d 2265 6e61 626c 6564 223e  value="enabled">
 00000590: 2052 6571 7569 7265 643c 2f6c 6162 656c   Required</label
 000005a0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
 000005b0: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
 000005c0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
 000005d0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-000005e0: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
-000005f0: 7573 746f 6d69 7a61 7469 6f6e 2d73 6570  ustomization-sep
-00000600: 6172 6174 696f 6e22 2073 7479 6c65 3d22  aration" style="
-00000610: 6d61 7267 696e 2d62 6f74 746f 6d3a 2031  margin-bottom: 1
-00000620: 3570 7822 3e3c 2f64 6976 3e0a 2020 2020  5px"></div>.    
-00000630: 2020 2020 3c68 3320 636c 6173 733d 2263      <h3 class="c
-00000640: 7573 746f 6d69 7a61 7469 6f6e 2d73 6563  ustomization-sec
-00000650: 7469 6f6e 2d74 6974 6c65 223e 546f 6f6c  tion-title">Tool
-00000660: 2063 6f6e 7472 6f6c 3c2f 6833 3e0a 2020   control</h3>.  
-00000670: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00000680: 3d22 666f 726d 2d67 726f 7570 207b 2520  ="form-group {% 
-00000690: 6966 2065 7272 6f72 732e 746f 6f6c 5f63  if errors.tool_c
-000006a0: 6f6e 7472 6f6c 5f63 6f6e 6669 6775 7261  ontrol_configura
-000006b0: 7469 6f6e 5f73 6574 7469 6e67 5f74 656d  tion_setting_tem
-000006c0: 706c 6174 6520 257d 6861 732d 6572 726f  plate %}has-erro
-000006d0: 727b 2520 656e 6469 6620 257d 223e 0a20  r{% endif %}">. 
-000006e0: 2020 2020 2020 2020 2020 203c 6c61 6265             <labe
-000006f0: 6c20 636c 6173 733d 2263 6f6e 7472 6f6c  l class="control
-00000700: 2d6c 6162 656c 2063 6f6c 2d6d 642d 3322  -label col-md-3"
-00000710: 2066 6f72 3d22 746f 6f6c 5f63 6f6e 7472   for="tool_contr
-00000720: 6f6c 5f63 6f6e 6669 6775 7261 7469 6f6e  ol_configuration
-00000730: 5f73 6574 7469 6e67 5f74 656d 706c 6174  _setting_templat
-00000740: 6522 3e43 6f6e 6669 6775 7261 7469 6f6e  e">Configuration
-00000750: 2074 656d 706c 6174 653c 2f6c 6162 656c   template</label
-00000760: 3e0a 2020 2020 2020 2020 2020 2020 3c64  >.            <d
-00000770: 6976 2063 6c61 7373 3d22 636f 6c2d 6d64  iv class="col-md
-00000780: 2d37 223e 0a20 2020 2020 2020 2020 2020  -7">.           
-00000790: 2020 2020 203c 7465 7874 6172 6561 206f       <textarea o
-000007a0: 6e69 6e70 7574 3d22 6175 746f 5f73 697a  ninput="auto_siz
-000007b0: 655f 7465 7874 6172 6561 2874 6869 7329  e_textarea(this)
-000007c0: 3b22 2069 643d 2274 6f6f 6c5f 636f 6e74  ;" id="tool_cont
-000007d0: 726f 6c5f 636f 6e66 6967 7572 6174 696f  rol_configuratio
-000007e0: 6e5f 7365 7474 696e 675f 7465 6d70 6c61  n_setting_templa
-000007f0: 7465 2220 6e61 6d65 3d22 746f 6f6c 5f63  te" name="tool_c
-00000800: 6f6e 7472 6f6c 5f63 6f6e 6669 6775 7261  ontrol_configura
-00000810: 7469 6f6e 5f73 6574 7469 6e67 5f74 656d  tion_setting_tem
-00000820: 706c 6174 6522 2063 6c61 7373 3d22 666f  plate" class="fo
-00000830: 726d 2d63 6f6e 7472 6f6c 223e 7b25 2069  rm-control">{% i
-00000840: 6620 6572 726f 7273 2e74 6f6f 6c5f 636f  f errors.tool_co
-00000850: 6e74 726f 6c5f 636f 6e66 6967 7572 6174  ntrol_configurat
-00000860: 696f 6e5f 7365 7474 696e 675f 7465 6d70  ion_setting_temp
-00000870: 6c61 7465 2025 7d7b 7b20 6572 726f 7273  late %}{{ errors
-00000880: 2e74 6f6f 6c5f 636f 6e74 726f 6c5f 636f  .tool_control_co
-00000890: 6e66 6967 7572 6174 696f 6e5f 7365 7474  nfiguration_sett
-000008a0: 696e 675f 7465 6d70 6c61 7465 2e76 616c  ing_template.val
-000008b0: 7565 207d 7d7b 2520 656c 7365 2025 7d7b  ue }}{% else %}{
-000008c0: 7b20 746f 6f6c 5f63 6f6e 7472 6f6c 5f63  { tool_control_c
-000008d0: 6f6e 6669 6775 7261 7469 6f6e 5f73 6574  onfiguration_set
-000008e0: 7469 6e67 5f74 656d 706c 6174 6520 7d7d  ting_template }}
-000008f0: 7b25 2065 6e64 6966 2025 7d3c 2f74 6578  {% endif %}</tex
-00000900: 7461 7265 613e 0a20 2020 2020 2020 2020  tarea>.         
-00000910: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-00000920: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00000930: 3d22 636f 6c2d 6d64 2d6f 6666 7365 742d  ="col-md-offset-
-00000940: 3320 636f 6c2d 6d64 2d39 2068 656c 702d  3 col-md-9 help-
-00000950: 626c 6f63 6b20 6c69 6768 742d 6772 6579  block light-grey
-00000960: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00000970: 2020 207b 2520 6966 2065 7272 6f72 732e     {% if errors.
-00000980: 746f 6f6c 5f63 6f6e 7472 6f6c 5f63 6f6e  tool_control_con
-00000990: 6669 6775 7261 7469 6f6e 5f73 6574 7469  figuration_setti
-000009a0: 6e67 5f74 656d 706c 6174 6520 257d 0a20  ng_template %}. 
-000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009c0: 2020 207b 7b20 6572 726f 7273 2e74 6f6f     {{ errors.too
-000009d0: 6c5f 636f 6e74 726f 6c5f 636f 6e66 6967  l_control_config
-000009e0: 7572 6174 696f 6e5f 7365 7474 696e 675f  uration_setting_
-000009f0: 7465 6d70 6c61 7465 2e65 7272 6f72 207d  template.error }
-00000a00: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00000a10: 2020 7b25 2065 6c73 6520 257d 0a20 2020    {% else %}.   
-00000a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a30: 2054 6865 2064 6a61 6e67 6f20 7465 6d70   The django temp
-00000a40: 6c61 7465 2075 7365 6420 666f 7220 7265  late used for re
-00000a50: 6e64 6572 696e 6720 6375 7272 656e 7420  ndering current 
-00000a60: 636f 6e66 6967 7572 6174 696f 6e20 7365  configuration se
-00000a70: 7474 696e 672e 2054 6865 2063 6f6e 7465  tting. The conte
-00000a80: 7874 2076 6172 6961 626c 6520 3c62 3e63  xt variable <b>c
-00000a90: 7572 7265 6e74 5f73 6574 7469 6e67 3c2f  urrent_setting</
-00000aa0: 623e 2069 7320 7072 6f76 6964 6564 2e0a  b> is provided..
-00000ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ac0: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
-00000ad0: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00000ae0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-00000af0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00000b00: 3d22 666f 726d 2d67 726f 7570 223e 0a20  ="form-group">. 
-00000b10: 2020 2020 2020 2020 2020 203c 6c61 6265             <labe
-00000b20: 6c20 636c 6173 733d 2263 6f6e 7472 6f6c  l class="control
-00000b30: 2d6c 6162 656c 2063 6f6c 2d73 6d2d 3420  -label col-sm-4 
-00000b40: 636f 6c2d 6d64 2d33 223e 5573 6167 6520  col-md-3">Usage 
-00000b50: 6461 7461 2068 6973 746f 7279 3c2f 6c61  data history</la
-00000b60: 6265 6c3e 0a20 2020 2020 2020 2020 2020  bel>.           
-00000b70: 203c 6469 7620 636c 6173 733d 2263 6f6c   <div class="col
-00000b80: 2d73 6d2d 3820 636f 6c2d 6d64 2d39 223e  -sm-8 col-md-9">
-00000b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000ba0: 203c 6469 7620 636c 6173 733d 2263 6865   <div class="che
-00000bb0: 636b 626f 7822 3e0a 2020 2020 2020 2020  ckbox">.        
-00000bc0: 2020 2020 2020 2020 2020 2020 3c6c 6162              <lab
-00000bd0: 656c 3e3c 696e 7075 7420 7479 7065 3d22  el><input type="
-00000be0: 6368 6563 6b62 6f78 2220 6964 3d22 746f  checkbox" id="to
-00000bf0: 6f6c 5f63 6f6e 7472 6f6c 5f68 6964 655f  ol_control_hide_
-00000c00: 6461 7461 5f68 6973 746f 7279 5f75 7365  data_history_use
-00000c10: 7273 2220 6e61 6d65 3d22 746f 6f6c 5f63  rs" name="tool_c
-00000c20: 6f6e 7472 6f6c 5f68 6964 655f 6461 7461  ontrol_hide_data
-00000c30: 5f68 6973 746f 7279 5f75 7365 7273 2220  _history_users" 
-00000c40: 7b25 2069 6620 746f 6f6c 5f63 6f6e 7472  {% if tool_contr
-00000c50: 6f6c 5f68 6964 655f 6461 7461 5f68 6973  ol_hide_data_his
-00000c60: 746f 7279 5f75 7365 7273 2025 7d63 6865  tory_users %}che
-00000c70: 636b 6564 7b25 2065 6e64 6966 2025 7d20  cked{% endif %} 
-00000c80: 7661 6c75 653d 2265 6e61 626c 6564 223e  value="enabled">
-00000c90: 2063 6865 636b 2074 6f20 6f6e 6c79 2073   check to only s
-00000ca0: 686f 7720 7573 6167 6520 6461 7461 2068  how usage data h
-00000cb0: 6973 746f 7279 2074 6162 2066 6f72 2073  istory tab for s
-00000cc0: 7461 6666 206d 656d 6265 7273 3c2f 6c61  taff members</la
-00000cd0: 6265 6c3e 0a20 2020 2020 2020 2020 2020  bel>.           
-00000ce0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-00000cf0: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00000d00: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-00000d10: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00000d20: 3d22 6375 7374 6f6d 697a 6174 696f 6e2d  ="customization-
-00000d30: 7365 7061 7261 7469 6f6e 2220 7374 796c  separation" styl
-00000d40: 653d 226d 6172 6769 6e2d 626f 7474 6f6d  e="margin-bottom
-00000d50: 3a20 3135 7078 223e 3c2f 6469 763e 0a20  : 15px"></div>. 
-00000d60: 2020 2020 2020 203c 6833 2063 6c61 7373         <h3 class
-00000d70: 3d22 6375 7374 6f6d 697a 6174 696f 6e2d  ="customization-
-00000d80: 7365 6374 696f 6e2d 7469 746c 6522 3e54  section-title">T
-00000d90: 6f6f 6c20 7175 616c 6966 6963 6174 696f  ool qualificatio
-00000da0: 6e20 6578 7069 7261 7469 6f6e 3c2f 6833  n expiration</h3
-00000db0: 3e0a 2020 2020 2020 2020 3c70 3e49 6620  >.        <p>If 
-00000dc0: 6163 7469 7665 2c20 7468 6973 2066 6561  active, this fea
-00000dd0: 7475 7265 2077 696c 6c20 7265 6d6f 7665  ture will remove
-00000de0: 2074 6f6f 6c20 7175 616c 6966 6963 6174   tool qualificat
-00000df0: 696f 6e20 6672 6f6d 2061 2075 7365 7220  ion from a user 
-00000e00: 6966 2074 6865 2075 7365 7220 6861 7320  if the user has 
-00000e10: 6e6f 7420 7573 6564 2074 6865 2074 6f6f  not used the too
-00000e20: 6c20 6166 7465 7220 6120 7768 696c 6520  l after a while 
-00000e30: 6f72 206e 6576 6572 2075 7365 6420 6974  or never used it
-00000e40: 2073 696e 6365 2071 7561 6c69 6669 6564   since qualified
-00000e50: 2028 636f 6e66 6967 7572 6564 2073 6570   (configured sep
-00000e60: 6172 6174 656c 7929 2e0a 2020 2020 2020  arately)..      
-00000e70: 2020 3c70 3e54 6865 203c 6120 6872 6566    <p>The <a href
-00000e80: 3d22 7b25 2075 726c 2027 6375 7374 6f6d  ="{% url 'custom
-00000e90: 697a 6174 696f 6e27 2027 7465 6d70 6c61  ization' 'templa
-00000ea0: 7465 7327 2025 7d3f 2374 6f6f 6c5f 7175  tes' %}?#tool_qu
-00000eb0: 616c 6966 6963 6174 696f 6e5f 6578 7069  alification_expi
-00000ec0: 7261 7469 6f6e 5f65 6d61 696c 5f69 6422  ration_email_id"
-00000ed0: 3e75 7365 7220 746f 6f6c 2071 7561 6c69  >user tool quali
-00000ee0: 6669 6361 7469 6f6e 2065 7870 6972 6174  fication expirat
-00000ef0: 696f 6e20 656d 6169 6c3c 2f61 3e20 6e65  ion email</a> ne
-00000f00: 6564 2074 6f20 6265 2073 6574 2074 6f20  ed to be set to 
-00000f10: 656e 6162 6c65 2074 6869 7320 6665 6174  enable this feat
-00000f20: 7572 652e 3c2f 703e 3c62 722f 3e0a 2020  ure.</p><br/>.  
-00000f30: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00000f40: 3d22 666f 726d 2d67 726f 7570 207b 2520  ="form-group {% 
-00000f50: 6966 2065 7272 6f72 732e 746f 6f6c 5f71  if errors.tool_q
-00000f60: 7561 6c69 6669 6361 7469 6f6e 5f72 656d  ualification_rem
-00000f70: 696e 6465 725f 6461 7973 2025 7d68 6173  inder_days %}has
-00000f80: 2d65 7272 6f72 7b25 2065 6e64 6966 2025  -error{% endif %
-00000f90: 7d22 3e0a 2020 2020 2020 2020 2020 2020  }">.            
-00000fa0: 3c6c 6162 656c 2063 6c61 7373 3d22 636f  <label class="co
-00000fb0: 6e74 726f 6c2d 6c61 6265 6c20 636f 6c2d  ntrol-label col-
-00000fc0: 6d64 2d33 2220 666f 723d 2274 6f6f 6c5f  md-3" for="tool_
-00000fd0: 7175 616c 6966 6963 6174 696f 6e5f 7265  qualification_re
-00000fe0: 6d69 6e64 6572 5f64 6179 7322 3e52 656d  minder_days">Rem
-00000ff0: 696e 6465 7220 6461 7973 3c2f 6c61 6265  inder days</labe
-00001000: 6c3e 0a20 2020 2020 2020 2020 2020 203c  l>.            <
-00001010: 6469 7620 636c 6173 733d 2263 6f6c 2d6d  div class="col-m
-00001020: 642d 3522 3e0a 2020 2020 2020 2020 2020  d-5">.          
-00001030: 2020 2020 2020 3c69 6e70 7574 2074 7970        <input typ
-00001040: 653d 2274 6578 7422 2069 643d 2274 6f6f  e="text" id="too
-00001050: 6c5f 7175 616c 6966 6963 6174 696f 6e5f  l_qualification_
-00001060: 7265 6d69 6e64 6572 5f64 6179 7322 206e  reminder_days" n
-00001070: 616d 653d 2274 6f6f 6c5f 7175 616c 6966  ame="tool_qualif
-00001080: 6963 6174 696f 6e5f 7265 6d69 6e64 6572  ication_reminder
-00001090: 5f64 6179 7322 2063 6c61 7373 3d22 666f  _days" class="fo
-000010a0: 726d 2d63 6f6e 7472 6f6c 2220 7661 6c75  rm-control" valu
-000010b0: 653d 227b 2520 6966 2065 7272 6f72 732e  e="{% if errors.
-000010c0: 746f 6f6c 5f71 7561 6c69 6669 6361 7469  tool_qualificati
-000010d0: 6f6e 5f72 656d 696e 6465 725f 6461 7973  on_reminder_days
-000010e0: 2025 7d7b 7b20 6572 726f 7273 2e74 6f6f   %}{{ errors.too
-000010f0: 6c5f 7175 616c 6966 6963 6174 696f 6e5f  l_qualification_
-00001100: 7265 6d69 6e64 6572 5f64 6179 732e 7661  reminder_days.va
-00001110: 6c75 6520 7d7d 7b25 2065 6c73 6520 257d  lue }}{% else %}
-00001120: 7b7b 2074 6f6f 6c5f 7175 616c 6966 6963  {{ tool_qualific
-00001130: 6174 696f 6e5f 7265 6d69 6e64 6572 5f64  ation_reminder_d
-00001140: 6179 7320 7d7d 7b25 2065 6e64 6966 2025  ays }}{% endif %
-00001150: 7d22 2f3e 0a20 2020 2020 2020 2020 2020  }"/>.           
-00001160: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00001170: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00001180: 636f 6c2d 6d64 2d6f 6666 7365 742d 3320  col-md-offset-3 
-00001190: 636f 6c2d 6d64 2d39 2068 656c 702d 626c  col-md-9 help-bl
-000011a0: 6f63 6b20 6c69 6768 742d 6772 6579 223e  ock light-grey">
-000011b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000011c0: 207b 2520 6966 2065 7272 6f72 732e 746f   {% if errors.to
-000011d0: 6f6c 5f71 7561 6c69 6669 6361 7469 6f6e  ol_qualification
-000011e0: 5f72 656d 696e 6465 725f 6461 7973 2025  _reminder_days %
-000011f0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00001200: 2020 2020 2020 7b7b 2065 7272 6f72 732e        {{ errors.
-00001210: 746f 6f6c 5f71 7561 6c69 6669 6361 7469  tool_qualificati
-00001220: 6f6e 5f72 656d 696e 6465 725f 6461 7973  on_reminder_days
-00001230: 2e65 7272 6f72 207d 7d0a 2020 2020 2020  .error }}.      
-00001240: 2020 2020 2020 2020 2020 7b25 2065 6c73            {% els
-00001250: 6520 257d 0a20 2020 2020 2020 2020 2020  e %}.           
-00001260: 2020 2020 2020 2020 2054 6865 2028 6f70           The (op
-00001270: 7469 6f6e 616c 2920 6e75 6d62 6572 206f  tional) number o
-00001280: 6620 6461 7973 2074 6f20 7365 6e64 2061  f days to send a
-00001290: 2072 656d 696e 6465 7220 7072 696f 7220   reminder prior 
-000012a0: 746f 2074 6865 2075 7365 7227 7320 746f  to the user's to
-000012b0: 6f6c 2071 7561 6c69 6669 6361 7469 6f6e  ol qualification
-000012c0: 2065 7870 6972 6174 696f 6e20 2862 656c   expiration (bel
-000012d0: 6f77 292e 2041 2063 6f6d 6d61 2d73 6570  ow). A comma-sep
-000012e0: 6172 6174 6564 206c 6973 7420 6361 6e20  arated list can 
-000012f0: 6265 2075 7365 6420 666f 7220 6d75 6c74  be used for mult
-00001300: 6970 6c65 2072 656d 696e 6465 7273 2e20  iple reminders. 
-00001310: 5468 6973 2061 7070 6c69 6573 2074 6f20  This applies to 
-00001320: 626f 7468 2065 7870 6972 6174 696f 6e20  both expiration 
-00001330: 6361 7365 732e 0a20 2020 2020 2020 2020  cases..         
-00001340: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
-00001350: 257d 0a20 2020 2020 2020 2020 2020 203c  %}.            <
-00001360: 2f64 6976 3e0a 2020 2020 2020 2020 3c2f  /div>.        </
-00001370: 6469 763e 0a20 2020 2020 2020 203c 6469  div>.        <di
-00001380: 7620 636c 6173 733d 2266 6f72 6d2d 6772  v class="form-gr
-00001390: 6f75 7020 7b25 2069 6620 6572 726f 7273  oup {% if errors
-000013a0: 2e74 6f6f 6c5f 7175 616c 6966 6963 6174  .tool_qualificat
-000013b0: 696f 6e5f 6578 7069 7261 7469 6f6e 5f64  ion_expiration_d
-000013c0: 6179 7320 257d 6861 732d 6572 726f 727b  ays %}has-error{
-000013d0: 2520 656e 6469 6620 257d 223e 0a20 2020  % endif %}">.   
-000013e0: 2020 2020 2020 2020 203c 6c61 6265 6c20           <label 
-000013f0: 636c 6173 733d 2263 6f6e 7472 6f6c 2d6c  class="control-l
-00001400: 6162 656c 2063 6f6c 2d6d 642d 3322 2066  abel col-md-3" f
-00001410: 6f72 3d22 746f 6f6c 5f71 7561 6c69 6669  or="tool_qualifi
-00001420: 6361 7469 6f6e 5f65 7870 6972 6174 696f  cation_expiratio
-00001430: 6e5f 6461 7973 223e 4578 7069 7261 7469  n_days">Expirati
-00001440: 6f6e 2064 6179 7320 2870 7265 7669 6f75  on days (previou
-00001450: 7320 746f 6f6c 2075 7361 6765 293c 2f6c  s tool usage)</l
-00001460: 6162 656c 3e0a 2020 2020 2020 2020 2020  abel>.          
-00001470: 2020 3c64 6976 2063 6c61 7373 3d22 636f    <div class="co
-00001480: 6c2d 6d64 2d35 223e 0a20 2020 2020 2020  l-md-5">.       
-00001490: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
-000014a0: 7479 7065 3d22 6e75 6d62 6572 2220 7374  type="number" st
-000014b0: 6570 3d22 3122 2069 643d 2274 6f6f 6c5f  ep="1" id="tool_
-000014c0: 7175 616c 6966 6963 6174 696f 6e5f 6578  qualification_ex
-000014d0: 7069 7261 7469 6f6e 5f64 6179 7322 206e  piration_days" n
-000014e0: 616d 653d 2274 6f6f 6c5f 7175 616c 6966  ame="tool_qualif
-000014f0: 6963 6174 696f 6e5f 6578 7069 7261 7469  ication_expirati
-00001500: 6f6e 5f64 6179 7322 2063 6c61 7373 3d22  on_days" class="
-00001510: 666f 726d 2d63 6f6e 7472 6f6c 2220 7661  form-control" va
-00001520: 6c75 653d 227b 2520 6966 2065 7272 6f72  lue="{% if error
-00001530: 732e 746f 6f6c 5f71 7561 6c69 6669 6361  s.tool_qualifica
-00001540: 7469 6f6e 5f65 7870 6972 6174 696f 6e5f  tion_expiration_
-00001550: 6461 7973 2025 7d7b 7b20 6572 726f 7273  days %}{{ errors
-00001560: 2e74 6f6f 6c5f 7175 616c 6966 6963 6174  .tool_qualificat
-00001570: 696f 6e5f 6578 7069 7261 7469 6f6e 5f64  ion_expiration_d
-00001580: 6179 732e 7661 6c75 6520 7d7d 7b25 2065  ays.value }}{% e
-00001590: 6c73 6520 257d 7b7b 2074 6f6f 6c5f 7175  lse %}{{ tool_qu
-000015a0: 616c 6966 6963 6174 696f 6e5f 6578 7069  alification_expi
-000015b0: 7261 7469 6f6e 5f64 6179 7320 7d7d 7b25  ration_days }}{%
-000015c0: 2065 6e64 6966 2025 7d22 2f3e 0a20 2020   endif %}"/>.   
-000015d0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-000015e0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-000015f0: 2063 6c61 7373 3d22 636f 6c2d 6d64 2d6f   class="col-md-o
-00001600: 6666 7365 742d 3320 636f 6c2d 6d64 2d39  ffset-3 col-md-9
-00001610: 2068 656c 702d 626c 6f63 6b20 6c69 6768   help-block ligh
-00001620: 742d 6772 6579 223e 0a20 2020 2020 2020  t-grey">.       
-00001630: 2020 2020 2020 2020 207b 2520 6966 2065           {% if e
-00001640: 7272 6f72 732e 746f 6f6c 5f71 7561 6c69  rrors.tool_quali
-00001650: 6669 6361 7469 6f6e 5f65 7870 6972 6174  fication_expirat
-00001660: 696f 6e5f 6461 7973 2025 7d0a 2020 2020  ion_days %}.    
-00001670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001680: 7b7b 2065 7272 6f72 732e 746f 6f6c 5f71  {{ errors.tool_q
-00001690: 7561 6c69 6669 6361 7469 6f6e 5f65 7870  ualification_exp
-000016a0: 6972 6174 696f 6e5f 6461 7973 2e65 7272  iration_days.err
-000016b0: 6f72 207d 7d0a 2020 2020 2020 2020 2020  or }}.          
-000016c0: 2020 2020 2020 7b25 2065 6c73 6520 257d        {% else %}
-000016d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000016e0: 2020 2020 2054 6865 206e 756d 6265 7220       The number 
-000016f0: 6f66 2064 6179 7320 6265 666f 7265 2074  of days before t
-00001700: 6865 2075 7365 7227 7320 746f 6f6c 2071  he user's tool q
-00001710: 7561 6c69 6669 6361 7469 6f6e 2065 7870  ualification exp
-00001720: 6972 6573 2073 696e 6365 2074 6865 2075  ires since the u
-00001730: 7365 7220 6c61 7374 2075 7365 6420 7468  ser last used th
-00001740: 6520 746f 6f6c 2e0a 2020 2020 2020 2020  e tool..        
-00001750: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-00001760: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00001770: 3c2f 6469 763e 0a20 2020 2020 2020 203c  </div>.        <
-00001780: 2f64 6976 3e0a 2020 2020 2020 2020 3c64  /div>.        <d
-00001790: 6976 2063 6c61 7373 3d22 666f 726d 2d67  iv class="form-g
-000017a0: 726f 7570 207b 2520 6966 2065 7272 6f72  roup {% if error
-000017b0: 732e 746f 6f6c 5f71 7561 6c69 6669 6361  s.tool_qualifica
-000017c0: 7469 6f6e 5f65 7870 6972 6174 696f 6e5f  tion_expiration_
-000017d0: 6e65 7665 725f 7573 6564 5f64 6179 7320  never_used_days 
-000017e0: 257d 6861 732d 6572 726f 727b 2520 656e  %}has-error{% en
-000017f0: 6469 6620 257d 223e 0a20 2020 2020 2020  dif %}">.       
-00001800: 2020 2020 203c 6c61 6265 6c20 636c 6173       <label clas
-00001810: 733d 2263 6f6e 7472 6f6c 2d6c 6162 656c  s="control-label
-00001820: 2063 6f6c 2d6d 642d 3322 2066 6f72 3d22   col-md-3" for="
-00001830: 746f 6f6c 5f71 7561 6c69 6669 6361 7469  tool_qualificati
-00001840: 6f6e 5f65 7870 6972 6174 696f 6e5f 6e65  on_expiration_ne
-00001850: 7665 725f 7573 6564 5f64 6179 7322 3e45  ver_used_days">E
-00001860: 7870 6972 6174 696f 6e20 6461 7973 2028  xpiration days (
-00001870: 6e6f 2074 6f6f 6c20 7573 6167 6529 3c2f  no tool usage)</
-00001880: 6c61 6265 6c3e 0a20 2020 2020 2020 2020  label>.         
-00001890: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
-000018a0: 6f6c 2d6d 642d 3522 3e0a 2020 2020 2020  ol-md-5">.      
-000018b0: 2020 2020 2020 2020 2020 3c69 6e70 7574            <input
-000018c0: 2074 7970 653d 226e 756d 6265 7222 2073   type="number" s
-000018d0: 7465 703d 2231 2220 6964 3d22 746f 6f6c  tep="1" id="tool
-000018e0: 5f71 7561 6c69 6669 6361 7469 6f6e 5f65  _qualification_e
-000018f0: 7870 6972 6174 696f 6e5f 6e65 7665 725f  xpiration_never_
-00001900: 7573 6564 5f64 6179 7322 206e 616d 653d  used_days" name=
-00001910: 2274 6f6f 6c5f 7175 616c 6966 6963 6174  "tool_qualificat
-00001920: 696f 6e5f 6578 7069 7261 7469 6f6e 5f6e  ion_expiration_n
-00001930: 6576 6572 5f75 7365 645f 6461 7973 2220  ever_used_days" 
-00001940: 636c 6173 733d 2266 6f72 6d2d 636f 6e74  class="form-cont
-00001950: 726f 6c22 2076 616c 7565 3d22 7b25 2069  rol" value="{% i
-00001960: 6620 6572 726f 7273 2e74 6f6f 6c5f 7175  f errors.tool_qu
-00001970: 616c 6966 6963 6174 696f 6e5f 6578 7069  alification_expi
-00001980: 7261 7469 6f6e 5f6e 6576 6572 5f75 7365  ration_never_use
-00001990: 645f 6461 7973 2025 7d7b 7b20 6572 726f  d_days %}{{ erro
-000019a0: 7273 2e74 6f6f 6c5f 7175 616c 6966 6963  rs.tool_qualific
-000019b0: 6174 696f 6e5f 6578 7069 7261 7469 6f6e  ation_expiration
-000019c0: 5f6e 6576 6572 5f75 7365 645f 6461 7973  _never_used_days
-000019d0: 2e76 616c 7565 207d 7d7b 2520 656c 7365  .value }}{% else
-000019e0: 2025 7d7b 7b20 746f 6f6c 5f71 7561 6c69   %}{{ tool_quali
-000019f0: 6669 6361 7469 6f6e 5f65 7870 6972 6174  fication_expirat
-00001a00: 696f 6e5f 6e65 7665 725f 7573 6564 5f64  ion_never_used_d
-00001a10: 6179 7320 7d7d 7b25 2065 6e64 6966 2025  ays }}{% endif %
-00001a20: 7d22 2f3e 0a20 2020 2020 2020 2020 2020  }"/>.           
-00001a30: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00001a40: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00001a50: 636f 6c2d 6d64 2d6f 6666 7365 742d 3320  col-md-offset-3 
-00001a60: 636f 6c2d 6d64 2d39 2068 656c 702d 626c  col-md-9 help-bl
-00001a70: 6f63 6b20 6c69 6768 742d 6772 6579 223e  ock light-grey">
-00001a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001a90: 207b 2520 6966 2065 7272 6f72 732e 746f   {% if errors.to
-00001aa0: 6f6c 5f71 7561 6c69 6669 6361 7469 6f6e  ol_qualification
-00001ab0: 5f65 7870 6972 6174 696f 6e5f 6e65 7665  _expiration_neve
-00001ac0: 725f 7573 6564 5f64 6179 7320 257d 0a20  r_used_days %}. 
-00001ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ae0: 2020 207b 7b20 6572 726f 7273 2e74 6f6f     {{ errors.too
-00001af0: 6c5f 7175 616c 6966 6963 6174 696f 6e5f  l_qualification_
-00001b00: 6578 7069 7261 7469 6f6e 5f6e 6576 6572  expiration_never
-00001b10: 5f75 7365 645f 6461 7973 2e65 7272 6f72  _used_days.error
-00001b20: 207d 7d0a 2020 2020 2020 2020 2020 2020   }}.            
-00001b30: 2020 2020 7b25 2065 6c73 6520 257d 0a20      {% else %}. 
-00001b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b50: 2020 2054 6865 206e 756d 6265 7220 6f66     The number of
-00001b60: 2064 6179 7320 6265 666f 7265 2074 6865   days before the
-00001b70: 2075 7365 7227 7320 746f 6f6c 2071 7561   user's tool qua
-00001b80: 6c69 6669 6361 7469 6f6e 2065 7870 6972  lification expir
-00001b90: 6573 2073 696e 6365 2074 6865 2075 7365  es since the use
-00001ba0: 7220 7175 616c 6966 6965 6420 666f 7220  r qualified for 
-00001bb0: 7468 6520 6669 7273 7420 7469 6d65 2e0a  the first time..
-00001bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bd0: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
-00001be0: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00001bf0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-00001c00: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00001c10: 3d22 666f 726d 2d67 726f 7570 207b 2520  ="form-group {% 
-00001c20: 6966 2065 7272 6f72 732e 746f 6f6c 5f71  if errors.tool_q
-00001c30: 7561 6c69 6669 6361 7469 6f6e 5f63 6320  ualification_cc 
-00001c40: 257d 6861 732d 6572 726f 727b 2520 656e  %}has-error{% en
-00001c50: 6469 6620 257d 223e 0a20 2020 2020 2020  dif %}">.       
-00001c60: 2020 2020 203c 6c61 6265 6c20 636c 6173       <label clas
-00001c70: 733d 2263 6f6e 7472 6f6c 2d6c 6162 656c  s="control-label
-00001c80: 2063 6f6c 2d6d 642d 3322 2066 6f72 3d22   col-md-3" for="
-00001c90: 746f 6f6c 5f71 7561 6c69 6669 6361 7469  tool_qualificati
-00001ca0: 6f6e 5f63 6322 3e52 656d 696e 6465 722f  on_cc">Reminder/
-00001cb0: 6578 7069 7261 7469 6f6e 2043 433c 2f6c  expiration CC</l
-00001cc0: 6162 656c 3e0a 2020 2020 2020 2020 2020  abel>.          
-00001cd0: 2020 3c64 6976 2063 6c61 7373 3d22 636f    <div class="co
-00001ce0: 6c2d 6d64 2d35 223e 0a20 2020 2020 2020  l-md-5">.       
-00001cf0: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
-00001d00: 7479 7065 3d22 7465 7874 2220 6964 3d22  type="text" id="
-00001d10: 746f 6f6c 5f71 7561 6c69 6669 6361 7469  tool_qualificati
-00001d20: 6f6e 5f63 6322 206e 616d 653d 2274 6f6f  on_cc" name="too
-00001d30: 6c5f 7175 616c 6966 6963 6174 696f 6e5f  l_qualification_
-00001d40: 6363 2220 636c 6173 733d 2266 6f72 6d2d  cc" class="form-
-00001d50: 636f 6e74 726f 6c22 2076 616c 7565 3d22  control" value="
-00001d60: 7b25 2069 6620 6572 726f 7273 2e74 6f6f  {% if errors.too
-00001d70: 6c5f 7175 616c 6966 6963 6174 696f 6e5f  l_qualification_
-00001d80: 6363 2025 7d7b 7b20 6572 726f 7273 2e74  cc %}{{ errors.t
-00001d90: 6f6f 6c5f 7175 616c 6966 6963 6174 696f  ool_qualificatio
-00001da0: 6e5f 6363 2e76 616c 7565 207d 7d7b 2520  n_cc.value }}{% 
-00001db0: 656c 7365 2025 7d7b 7b20 746f 6f6c 5f71  else %}{{ tool_q
-00001dc0: 7561 6c69 6669 6361 7469 6f6e 5f63 6320  ualification_cc 
-00001dd0: 7d7d 7b25 2065 6e64 6966 2025 7d22 2070  }}{% endif %}" p
-00001de0: 6c61 6365 686f 6c64 6572 3d22 696e 666f  laceholder="info
-00001df0: 726d 6174 696f 6e40 6578 616d 706c 652e  rmation@example.
-00001e00: 6f72 6722 2f3e 0a20 2020 2020 2020 2020  org"/>.         
-00001e10: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-00001e20: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00001e30: 3d22 636f 6c2d 6d64 2d6f 6666 7365 742d  ="col-md-offset-
-00001e40: 3320 636f 6c2d 6d64 2d39 2068 656c 702d  3 col-md-9 help-
-00001e50: 626c 6f63 6b20 6c69 6768 742d 6772 6579  block light-grey
-00001e60: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00001e70: 2020 207b 2520 6966 2065 7272 6f72 732e     {% if errors.
-00001e80: 746f 6f6c 5f71 7561 6c69 6669 6361 7469  tool_qualificati
-00001e90: 6f6e 5f63 6320 257d 0a20 2020 2020 2020  on_cc %}.       
-00001ea0: 2020 2020 2020 2020 2020 2020 207b 7b20               {{ 
-00001eb0: 6572 726f 7273 2e74 6f6f 6c5f 7175 616c  errors.tool_qual
-00001ec0: 6966 6963 6174 696f 6e5f 6363 2e65 7272  ification_cc.err
-00001ed0: 6f72 207d 7d0a 2020 2020 2020 2020 2020  or }}.          
-00001ee0: 2020 2020 2020 7b25 2065 6c73 6520 257d        {% else %}
-00001ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001f00: 2020 2020 2045 7874 7261 2065 6d61 696c       Extra email
-00001f10: 2061 6464 7265 7373 2074 6f20 636f 7079   address to copy
-00001f20: 2077 6865 6e20 6120 7573 6572 2773 2074   when a user's t
-00001f30: 6f6f 6c20 7175 616c 6966 6963 6174 696f  ool qualificatio
-00001f40: 6e20 7265 6d69 6e64 6572 2f65 7870 6972  n reminder/expir
-00001f50: 6174 696f 6e20 656d 6169 6c20 6973 2073  ation email is s
-00001f60: 656e 742e 2041 2063 6f6d 6d61 2d73 6570  ent. A comma-sep
-00001f70: 6172 6174 6564 206c 6973 7420 6361 6e20  arated list can 
-00001f80: 6265 2075 7365 642e 0a20 2020 2020 2020  be used..       
-00001f90: 2020 2020 2020 2020 207b 2520 656e 6469           {% endi
-00001fa0: 6620 257d 0a20 2020 2020 2020 2020 2020  f %}.           
-00001fb0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00001fc0: 3c2f 6469 763e 0a20 2020 2020 2020 203c  </div>.        <
-00001fd0: 6469 7620 636c 6173 733d 2263 7573 746f  div class="custo
-00001fe0: 6d69 7a61 7469 6f6e 2d73 6570 6172 6174  mization-separat
-00001ff0: 696f 6e22 2073 7479 6c65 3d22 6d61 7267  ion" style="marg
-00002000: 696e 2d62 6f74 746f 6d3a 2031 3570 7822  in-bottom: 15px"
-00002010: 3e3c 2f64 6976 3e0a 2020 2020 2020 2020  ></div>.        
-00002020: 3c64 6976 2063 6c61 7373 3d22 7465 7874  <div class="text
-00002030: 2d63 656e 7465 7222 3e0a 2020 2020 2020  -center">.      
-00002040: 2020 2020 2020 7b25 2062 7574 746f 6e20        {% button 
-00002050: 7479 7065 3d22 7361 7665 2220 7661 6c75  type="save" valu
-00002060: 653d 2253 6176 6520 7365 7474 696e 6773  e="Save settings
-00002070: 2220 257d 0a20 2020 2020 2020 203c 2f64  " %}.        </d
-00002080: 6976 3e0a 2020 2020 3c2f 6469 763e 0a20  iv>.    </div>. 
-00002090: 2020 203c 7363 7269 7074 2074 7970 653d     <script type=
-000020a0: 2274 6578 742f 6a61 7661 7363 7269 7074  "text/javascript
-000020b0: 223e 0a20 2020 2020 2020 2024 2822 2374  ">.        $("#t
-000020c0: 6f6f 6c2d 7461 622d 6c69 6e6b 2229 2e63  ool-tab-link").c
-000020d0: 6c69 636b 2866 756e 6374 696f 6e28 2920  lick(function() 
-000020e0: 7b73 6574 5469 6d65 6f75 7428 6f6e 5f74  {setTimeout(on_t
-000020f0: 6f6f 6c5f 7461 625f 7368 6f77 2c20 3530  ool_tab_show, 50
-00002100: 297d 293b 0a20 2020 2020 2020 2066 756e  )});.        fun
-00002110: 6374 696f 6e20 6f6e 5f74 6f6f 6c5f 7461  ction on_tool_ta
-00002120: 625f 7368 6f77 2829 0a20 2020 2020 2020  b_show().       
-00002130: 207b 0a20 2020 2020 2020 2020 2020 2061   {.            a
-00002140: 7574 6f5f 7369 7a65 5f74 6578 7461 7265  uto_size_textare
-00002150: 6128 646f 6375 6d65 6e74 2e67 6574 456c  a(document.getEl
-00002160: 656d 656e 7442 7949 6428 2774 6f6f 6c5f  ementById('tool_
-00002170: 636f 6e74 726f 6c5f 636f 6e66 6967 7572  control_configur
-00002180: 6174 696f 6e5f 7365 7474 696e 675f 7465  ation_setting_te
-00002190: 6d70 6c61 7465 2729 290a 2020 2020 2020  mplate')).      
-000021a0: 2020 7d0a 2020 2020 2020 2020 6f6e 5f74    }.        on_t
-000021b0: 6f6f 6c5f 7461 625f 7368 6f77 2829 3b0a  ool_tab_show();.
-000021c0: 2020 2020 3c2f 7363 7269 7074 3e0a 3c2f      </script>.</
-000021d0: 666f 726d 3e                             form>
+000005e0: 2020 203c 6469 7620 636c 6173 733d 2266     <div class="f
+000005f0: 6f72 6d2d 6772 6f75 7022 3e0a 2020 2020  orm-group">.    
+00000600: 2020 2020 2020 2020 3c6c 6162 656c 2063          <label c
+00000610: 6c61 7373 3d22 636f 6e74 726f 6c2d 6c61  lass="control-la
+00000620: 6265 6c20 636f 6c2d 736d 2d34 2063 6f6c  bel col-sm-4 col
+00000630: 2d6d 642d 3322 3e54 6f6f 6c20 7072 6f62  -md-3">Tool prob
+00000640: 6c65 6d20 7570 6461 7465 733c 2f6c 6162  lem updates</lab
+00000650: 656c 3e0a 2020 2020 2020 2020 2020 2020  el>.            
+00000660: 3c64 6976 2063 6c61 7373 3d22 636f 6c2d  <div class="col-
+00000670: 736d 2d38 2063 6f6c 2d6d 642d 3922 3e0a  sm-8 col-md-9">.
+00000680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000690: 3c64 6976 2063 6c61 7373 3d22 6368 6563  <div class="chec
+000006a0: 6b62 6f78 223e 0a20 2020 2020 2020 2020  kbox">.         
+000006b0: 2020 2020 2020 2020 2020 203c 696e 7075             <inpu
+000006c0: 7420 7479 7065 3d22 6869 6464 656e 2220  t type="hidden" 
+000006d0: 6e61 6d65 3d22 746f 6f6c 5f74 6173 6b5f  name="tool_task_
+000006e0: 7570 6461 7465 735f 6661 6369 6c69 7479  updates_facility
+000006f0: 5f6d 616e 6167 6572 7322 2076 616c 7565  _managers" value
+00000700: 3d22 6f66 6622 2f3e 0a20 2020 2020 2020  ="off"/>.       
+00000710: 2020 2020 2020 2020 2020 2020 203c 6c61               <la
+00000720: 6265 6c3e 3c69 6e70 7574 2074 7970 653d  bel><input type=
+00000730: 2263 6865 636b 626f 7822 206e 616d 653d  "checkbox" name=
+00000740: 2274 6f6f 6c5f 7461 736b 5f75 7064 6174  "tool_task_updat
+00000750: 6573 5f66 6163 696c 6974 795f 6d61 6e61  es_facility_mana
+00000760: 6765 7273 2220 7b25 2069 6620 746f 6f6c  gers" {% if tool
+00000770: 5f74 6173 6b5f 7570 6461 7465 735f 6661  _task_updates_fa
+00000780: 6369 6c69 7479 5f6d 616e 6167 6572 7320  cility_managers 
+00000790: 213d 2027 6f66 6627 2025 7d63 6865 636b  != 'off' %}check
+000007a0: 6564 7b25 2065 6e64 6966 2025 7d20 7661  ed{% endif %} va
+000007b0: 6c75 653d 2222 3e53 656e 6420 616c 6c20  lue="">Send all 
+000007c0: 746f 6f6c 2070 726f 626c 656d 2075 7064  tool problem upd
+000007d0: 6174 6573 2074 6f20 6661 6369 6c69 7479  ates to facility
+000007e0: 206d 616e 6167 6572 733c 2f6c 6162 656c   managers</label
+000007f0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000800: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00000810: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00000820: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
+00000830: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
+00000840: 7573 746f 6d69 7a61 7469 6f6e 2d73 6570  ustomization-sep
+00000850: 6172 6174 696f 6e22 2073 7479 6c65 3d22  aration" style="
+00000860: 6d61 7267 696e 2d62 6f74 746f 6d3a 2031  margin-bottom: 1
+00000870: 3570 7822 3e3c 2f64 6976 3e0a 2020 2020  5px"></div>.    
+00000880: 2020 2020 3c68 3320 636c 6173 733d 2263      <h3 class="c
+00000890: 7573 746f 6d69 7a61 7469 6f6e 2d73 6563  ustomization-sec
+000008a0: 7469 6f6e 2d74 6974 6c65 223e 546f 6f6c  tion-title">Tool
+000008b0: 2063 6f6e 7472 6f6c 3c2f 6833 3e0a 2020   control</h3>.  
+000008c0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+000008d0: 3d22 666f 726d 2d67 726f 7570 207b 2520  ="form-group {% 
+000008e0: 6966 2065 7272 6f72 732e 746f 6f6c 5f63  if errors.tool_c
+000008f0: 6f6e 7472 6f6c 5f63 6f6e 6669 6775 7261  ontrol_configura
+00000900: 7469 6f6e 5f73 6574 7469 6e67 5f74 656d  tion_setting_tem
+00000910: 706c 6174 6520 257d 6861 732d 6572 726f  plate %}has-erro
+00000920: 727b 2520 656e 6469 6620 257d 223e 0a20  r{% endif %}">. 
+00000930: 2020 2020 2020 2020 2020 203c 6c61 6265             <labe
+00000940: 6c20 636c 6173 733d 2263 6f6e 7472 6f6c  l class="control
+00000950: 2d6c 6162 656c 2063 6f6c 2d6d 642d 3322  -label col-md-3"
+00000960: 2066 6f72 3d22 746f 6f6c 5f63 6f6e 7472   for="tool_contr
+00000970: 6f6c 5f63 6f6e 6669 6775 7261 7469 6f6e  ol_configuration
+00000980: 5f73 6574 7469 6e67 5f74 656d 706c 6174  _setting_templat
+00000990: 6522 3e43 6f6e 6669 6775 7261 7469 6f6e  e">Configuration
+000009a0: 2074 656d 706c 6174 653c 2f6c 6162 656c   template</label
+000009b0: 3e0a 2020 2020 2020 2020 2020 2020 3c64  >.            <d
+000009c0: 6976 2063 6c61 7373 3d22 636f 6c2d 6d64  iv class="col-md
+000009d0: 2d37 223e 0a20 2020 2020 2020 2020 2020  -7">.           
+000009e0: 2020 2020 203c 7465 7874 6172 6561 206f       <textarea o
+000009f0: 6e69 6e70 7574 3d22 6175 746f 5f73 697a  ninput="auto_siz
+00000a00: 655f 7465 7874 6172 6561 2874 6869 7329  e_textarea(this)
+00000a10: 3b22 2069 643d 2274 6f6f 6c5f 636f 6e74  ;" id="tool_cont
+00000a20: 726f 6c5f 636f 6e66 6967 7572 6174 696f  rol_configuratio
+00000a30: 6e5f 7365 7474 696e 675f 7465 6d70 6c61  n_setting_templa
+00000a40: 7465 2220 6e61 6d65 3d22 746f 6f6c 5f63  te" name="tool_c
+00000a50: 6f6e 7472 6f6c 5f63 6f6e 6669 6775 7261  ontrol_configura
+00000a60: 7469 6f6e 5f73 6574 7469 6e67 5f74 656d  tion_setting_tem
+00000a70: 706c 6174 6522 2063 6c61 7373 3d22 666f  plate" class="fo
+00000a80: 726d 2d63 6f6e 7472 6f6c 223e 7b25 2069  rm-control">{% i
+00000a90: 6620 6572 726f 7273 2e74 6f6f 6c5f 636f  f errors.tool_co
+00000aa0: 6e74 726f 6c5f 636f 6e66 6967 7572 6174  ntrol_configurat
+00000ab0: 696f 6e5f 7365 7474 696e 675f 7465 6d70  ion_setting_temp
+00000ac0: 6c61 7465 2025 7d7b 7b20 6572 726f 7273  late %}{{ errors
+00000ad0: 2e74 6f6f 6c5f 636f 6e74 726f 6c5f 636f  .tool_control_co
+00000ae0: 6e66 6967 7572 6174 696f 6e5f 7365 7474  nfiguration_sett
+00000af0: 696e 675f 7465 6d70 6c61 7465 2e76 616c  ing_template.val
+00000b00: 7565 207d 7d7b 2520 656c 7365 2025 7d7b  ue }}{% else %}{
+00000b10: 7b20 746f 6f6c 5f63 6f6e 7472 6f6c 5f63  { tool_control_c
+00000b20: 6f6e 6669 6775 7261 7469 6f6e 5f73 6574  onfiguration_set
+00000b30: 7469 6e67 5f74 656d 706c 6174 6520 7d7d  ting_template }}
+00000b40: 7b25 2065 6e64 6966 2025 7d3c 2f74 6578  {% endif %}</tex
+00000b50: 7461 7265 613e 0a20 2020 2020 2020 2020  tarea>.         
+00000b60: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00000b70: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00000b80: 3d22 636f 6c2d 6d64 2d6f 6666 7365 742d  ="col-md-offset-
+00000b90: 3320 636f 6c2d 6d64 2d39 2068 656c 702d  3 col-md-9 help-
+00000ba0: 626c 6f63 6b20 6c69 6768 742d 6772 6579  block light-grey
+00000bb0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00000bc0: 2020 207b 2520 6966 2065 7272 6f72 732e     {% if errors.
+00000bd0: 746f 6f6c 5f63 6f6e 7472 6f6c 5f63 6f6e  tool_control_con
+00000be0: 6669 6775 7261 7469 6f6e 5f73 6574 7469  figuration_setti
+00000bf0: 6e67 5f74 656d 706c 6174 6520 257d 0a20  ng_template %}. 
+00000c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c10: 2020 207b 7b20 6572 726f 7273 2e74 6f6f     {{ errors.too
+00000c20: 6c5f 636f 6e74 726f 6c5f 636f 6e66 6967  l_control_config
+00000c30: 7572 6174 696f 6e5f 7365 7474 696e 675f  uration_setting_
+00000c40: 7465 6d70 6c61 7465 2e65 7272 6f72 207d  template.error }
+00000c50: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00000c60: 2020 7b25 2065 6c73 6520 257d 0a20 2020    {% else %}.   
+00000c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c80: 2054 6865 2064 6a61 6e67 6f20 7465 6d70   The django temp
+00000c90: 6c61 7465 2075 7365 6420 666f 7220 7265  late used for re
+00000ca0: 6e64 6572 696e 6720 6375 7272 656e 7420  ndering current 
+00000cb0: 636f 6e66 6967 7572 6174 696f 6e20 7365  configuration se
+00000cc0: 7474 696e 672e 2054 6865 2063 6f6e 7465  tting. The conte
+00000cd0: 7874 2076 6172 6961 626c 6520 3c62 3e63  xt variable <b>c
+00000ce0: 7572 7265 6e74 5f73 6574 7469 6e67 3c2f  urrent_setting</
+00000cf0: 623e 2069 7320 7072 6f76 6964 6564 2e0a  b> is provided..
+00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d10: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+00000d20: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00000d30: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+00000d40: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00000d50: 3d22 666f 726d 2d67 726f 7570 223e 0a20  ="form-group">. 
+00000d60: 2020 2020 2020 2020 2020 203c 6c61 6265             <labe
+00000d70: 6c20 636c 6173 733d 2263 6f6e 7472 6f6c  l class="control
+00000d80: 2d6c 6162 656c 2063 6f6c 2d73 6d2d 3420  -label col-sm-4 
+00000d90: 636f 6c2d 6d64 2d33 223e 5573 6167 6520  col-md-3">Usage 
+00000da0: 6461 7461 2068 6973 746f 7279 3c2f 6c61  data history</la
+00000db0: 6265 6c3e 0a20 2020 2020 2020 2020 2020  bel>.           
+00000dc0: 203c 6469 7620 636c 6173 733d 2263 6f6c   <div class="col
+00000dd0: 2d73 6d2d 3820 636f 6c2d 6d64 2d39 223e  -sm-8 col-md-9">
+00000de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000df0: 203c 6469 7620 636c 6173 733d 2263 6865   <div class="che
+00000e00: 636b 626f 7822 3e0a 2020 2020 2020 2020  ckbox">.        
+00000e10: 2020 2020 2020 2020 2020 2020 3c6c 6162              <lab
+00000e20: 656c 3e3c 696e 7075 7420 7479 7065 3d22  el><input type="
+00000e30: 6368 6563 6b62 6f78 2220 6964 3d22 746f  checkbox" id="to
+00000e40: 6f6c 5f63 6f6e 7472 6f6c 5f68 6964 655f  ol_control_hide_
+00000e50: 6461 7461 5f68 6973 746f 7279 5f75 7365  data_history_use
+00000e60: 7273 2220 6e61 6d65 3d22 746f 6f6c 5f63  rs" name="tool_c
+00000e70: 6f6e 7472 6f6c 5f68 6964 655f 6461 7461  ontrol_hide_data
+00000e80: 5f68 6973 746f 7279 5f75 7365 7273 2220  _history_users" 
+00000e90: 7b25 2069 6620 746f 6f6c 5f63 6f6e 7472  {% if tool_contr
+00000ea0: 6f6c 5f68 6964 655f 6461 7461 5f68 6973  ol_hide_data_his
+00000eb0: 746f 7279 5f75 7365 7273 2025 7d63 6865  tory_users %}che
+00000ec0: 636b 6564 7b25 2065 6e64 6966 2025 7d20  cked{% endif %} 
+00000ed0: 7661 6c75 653d 2265 6e61 626c 6564 223e  value="enabled">
+00000ee0: 2063 6865 636b 2074 6f20 6f6e 6c79 2073   check to only s
+00000ef0: 686f 7720 7573 6167 6520 6461 7461 2068  how usage data h
+00000f00: 6973 746f 7279 2074 6162 2066 6f72 2073  istory tab for s
+00000f10: 7461 6666 206d 656d 6265 7273 3c2f 6c61  taff members</la
+00000f20: 6265 6c3e 0a20 2020 2020 2020 2020 2020  bel>.           
+00000f30: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00000f40: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00000f50: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+00000f60: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00000f70: 3d22 6375 7374 6f6d 697a 6174 696f 6e2d  ="customization-
+00000f80: 7365 7061 7261 7469 6f6e 2220 7374 796c  separation" styl
+00000f90: 653d 226d 6172 6769 6e2d 626f 7474 6f6d  e="margin-bottom
+00000fa0: 3a20 3135 7078 223e 3c2f 6469 763e 0a20  : 15px"></div>. 
+00000fb0: 2020 2020 2020 203c 6833 2063 6c61 7373         <h3 class
+00000fc0: 3d22 6375 7374 6f6d 697a 6174 696f 6e2d  ="customization-
+00000fd0: 7365 6374 696f 6e2d 7469 746c 6522 3e54  section-title">T
+00000fe0: 6f6f 6c20 7175 616c 6966 6963 6174 696f  ool qualificatio
+00000ff0: 6e20 6578 7069 7261 7469 6f6e 3c2f 6833  n expiration</h3
+00001000: 3e0a 2020 2020 2020 2020 3c70 3e49 6620  >.        <p>If 
+00001010: 6163 7469 7665 2c20 7468 6973 2066 6561  active, this fea
+00001020: 7475 7265 2077 696c 6c20 7265 6d6f 7665  ture will remove
+00001030: 2074 6f6f 6c20 7175 616c 6966 6963 6174   tool qualificat
+00001040: 696f 6e20 6672 6f6d 2061 2075 7365 7220  ion from a user 
+00001050: 6966 2074 6865 2075 7365 7220 6861 7320  if the user has 
+00001060: 6e6f 7420 7573 6564 2074 6865 2074 6f6f  not used the too
+00001070: 6c20 6166 7465 7220 6120 7768 696c 6520  l after a while 
+00001080: 6f72 206e 6576 6572 2075 7365 6420 6974  or never used it
+00001090: 2073 696e 6365 2071 7561 6c69 6669 6564   since qualified
+000010a0: 2028 636f 6e66 6967 7572 6564 2073 6570   (configured sep
+000010b0: 6172 6174 656c 7929 2e0a 2020 2020 2020  arately)..      
+000010c0: 2020 3c70 3e54 6865 203c 6120 6872 6566    <p>The <a href
+000010d0: 3d22 7b25 2075 726c 2027 6375 7374 6f6d  ="{% url 'custom
+000010e0: 697a 6174 696f 6e27 2027 7465 6d70 6c61  ization' 'templa
+000010f0: 7465 7327 2025 7d3f 2374 6f6f 6c5f 7175  tes' %}?#tool_qu
+00001100: 616c 6966 6963 6174 696f 6e5f 6578 7069  alification_expi
+00001110: 7261 7469 6f6e 5f65 6d61 696c 5f69 6422  ration_email_id"
+00001120: 3e75 7365 7220 746f 6f6c 2071 7561 6c69  >user tool quali
+00001130: 6669 6361 7469 6f6e 2065 7870 6972 6174  fication expirat
+00001140: 696f 6e20 656d 6169 6c3c 2f61 3e20 6e65  ion email</a> ne
+00001150: 6564 2074 6f20 6265 2073 6574 2074 6f20  ed to be set to 
+00001160: 656e 6162 6c65 2074 6869 7320 6665 6174  enable this feat
+00001170: 7572 652e 3c2f 703e 3c62 722f 3e0a 2020  ure.</p><br/>.  
+00001180: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00001190: 3d22 666f 726d 2d67 726f 7570 207b 2520  ="form-group {% 
+000011a0: 6966 2065 7272 6f72 732e 746f 6f6c 5f71  if errors.tool_q
+000011b0: 7561 6c69 6669 6361 7469 6f6e 5f72 656d  ualification_rem
+000011c0: 696e 6465 725f 6461 7973 2025 7d68 6173  inder_days %}has
+000011d0: 2d65 7272 6f72 7b25 2065 6e64 6966 2025  -error{% endif %
+000011e0: 7d22 3e0a 2020 2020 2020 2020 2020 2020  }">.            
+000011f0: 3c6c 6162 656c 2063 6c61 7373 3d22 636f  <label class="co
+00001200: 6e74 726f 6c2d 6c61 6265 6c20 636f 6c2d  ntrol-label col-
+00001210: 6d64 2d33 2220 666f 723d 2274 6f6f 6c5f  md-3" for="tool_
+00001220: 7175 616c 6966 6963 6174 696f 6e5f 7265  qualification_re
+00001230: 6d69 6e64 6572 5f64 6179 7322 3e52 656d  minder_days">Rem
+00001240: 696e 6465 7220 6461 7973 3c2f 6c61 6265  inder days</labe
+00001250: 6c3e 0a20 2020 2020 2020 2020 2020 203c  l>.            <
+00001260: 6469 7620 636c 6173 733d 2263 6f6c 2d6d  div class="col-m
+00001270: 642d 3522 3e0a 2020 2020 2020 2020 2020  d-5">.          
+00001280: 2020 2020 2020 3c69 6e70 7574 2074 7970        <input typ
+00001290: 653d 2274 6578 7422 2069 643d 2274 6f6f  e="text" id="too
+000012a0: 6c5f 7175 616c 6966 6963 6174 696f 6e5f  l_qualification_
+000012b0: 7265 6d69 6e64 6572 5f64 6179 7322 206e  reminder_days" n
+000012c0: 616d 653d 2274 6f6f 6c5f 7175 616c 6966  ame="tool_qualif
+000012d0: 6963 6174 696f 6e5f 7265 6d69 6e64 6572  ication_reminder
+000012e0: 5f64 6179 7322 2063 6c61 7373 3d22 666f  _days" class="fo
+000012f0: 726d 2d63 6f6e 7472 6f6c 2220 7661 6c75  rm-control" valu
+00001300: 653d 227b 2520 6966 2065 7272 6f72 732e  e="{% if errors.
+00001310: 746f 6f6c 5f71 7561 6c69 6669 6361 7469  tool_qualificati
+00001320: 6f6e 5f72 656d 696e 6465 725f 6461 7973  on_reminder_days
+00001330: 2025 7d7b 7b20 6572 726f 7273 2e74 6f6f   %}{{ errors.too
+00001340: 6c5f 7175 616c 6966 6963 6174 696f 6e5f  l_qualification_
+00001350: 7265 6d69 6e64 6572 5f64 6179 732e 7661  reminder_days.va
+00001360: 6c75 6520 7d7d 7b25 2065 6c73 6520 257d  lue }}{% else %}
+00001370: 7b7b 2074 6f6f 6c5f 7175 616c 6966 6963  {{ tool_qualific
+00001380: 6174 696f 6e5f 7265 6d69 6e64 6572 5f64  ation_reminder_d
+00001390: 6179 7320 7d7d 7b25 2065 6e64 6966 2025  ays }}{% endif %
+000013a0: 7d22 2f3e 0a20 2020 2020 2020 2020 2020  }"/>.           
+000013b0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+000013c0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+000013d0: 636f 6c2d 6d64 2d6f 6666 7365 742d 3320  col-md-offset-3 
+000013e0: 636f 6c2d 6d64 2d39 2068 656c 702d 626c  col-md-9 help-bl
+000013f0: 6f63 6b20 6c69 6768 742d 6772 6579 223e  ock light-grey">
+00001400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001410: 207b 2520 6966 2065 7272 6f72 732e 746f   {% if errors.to
+00001420: 6f6c 5f71 7561 6c69 6669 6361 7469 6f6e  ol_qualification
+00001430: 5f72 656d 696e 6465 725f 6461 7973 2025  _reminder_days %
+00001440: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00001450: 2020 2020 2020 7b7b 2065 7272 6f72 732e        {{ errors.
+00001460: 746f 6f6c 5f71 7561 6c69 6669 6361 7469  tool_qualificati
+00001470: 6f6e 5f72 656d 696e 6465 725f 6461 7973  on_reminder_days
+00001480: 2e65 7272 6f72 207d 7d0a 2020 2020 2020  .error }}.      
+00001490: 2020 2020 2020 2020 2020 7b25 2065 6c73            {% els
+000014a0: 6520 257d 0a20 2020 2020 2020 2020 2020  e %}.           
+000014b0: 2020 2020 2020 2020 2054 6865 2028 6f70           The (op
+000014c0: 7469 6f6e 616c 2920 6e75 6d62 6572 206f  tional) number o
+000014d0: 6620 6461 7973 2074 6f20 7365 6e64 2061  f days to send a
+000014e0: 2072 656d 696e 6465 7220 7072 696f 7220   reminder prior 
+000014f0: 746f 2074 6865 2075 7365 7227 7320 746f  to the user's to
+00001500: 6f6c 2071 7561 6c69 6669 6361 7469 6f6e  ol qualification
+00001510: 2065 7870 6972 6174 696f 6e20 2862 656c   expiration (bel
+00001520: 6f77 292e 2041 2063 6f6d 6d61 2d73 6570  ow). A comma-sep
+00001530: 6172 6174 6564 206c 6973 7420 6361 6e20  arated list can 
+00001540: 6265 2075 7365 6420 666f 7220 6d75 6c74  be used for mult
+00001550: 6970 6c65 2072 656d 696e 6465 7273 2e20  iple reminders. 
+00001560: 5468 6973 2061 7070 6c69 6573 2074 6f20  This applies to 
+00001570: 626f 7468 2065 7870 6972 6174 696f 6e20  both expiration 
+00001580: 6361 7365 732e 0a20 2020 2020 2020 2020  cases..         
+00001590: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+000015a0: 257d 0a20 2020 2020 2020 2020 2020 203c  %}.            <
+000015b0: 2f64 6976 3e0a 2020 2020 2020 2020 3c2f  /div>.        </
+000015c0: 6469 763e 0a20 2020 2020 2020 203c 6469  div>.        <di
+000015d0: 7620 636c 6173 733d 2266 6f72 6d2d 6772  v class="form-gr
+000015e0: 6f75 7020 7b25 2069 6620 6572 726f 7273  oup {% if errors
+000015f0: 2e74 6f6f 6c5f 7175 616c 6966 6963 6174  .tool_qualificat
+00001600: 696f 6e5f 6578 7069 7261 7469 6f6e 5f64  ion_expiration_d
+00001610: 6179 7320 257d 6861 732d 6572 726f 727b  ays %}has-error{
+00001620: 2520 656e 6469 6620 257d 223e 0a20 2020  % endif %}">.   
+00001630: 2020 2020 2020 2020 203c 6c61 6265 6c20           <label 
+00001640: 636c 6173 733d 2263 6f6e 7472 6f6c 2d6c  class="control-l
+00001650: 6162 656c 2063 6f6c 2d6d 642d 3322 2066  abel col-md-3" f
+00001660: 6f72 3d22 746f 6f6c 5f71 7561 6c69 6669  or="tool_qualifi
+00001670: 6361 7469 6f6e 5f65 7870 6972 6174 696f  cation_expiratio
+00001680: 6e5f 6461 7973 223e 4578 7069 7261 7469  n_days">Expirati
+00001690: 6f6e 2064 6179 7320 2870 7265 7669 6f75  on days (previou
+000016a0: 7320 746f 6f6c 2075 7361 6765 293c 2f6c  s tool usage)</l
+000016b0: 6162 656c 3e0a 2020 2020 2020 2020 2020  abel>.          
+000016c0: 2020 3c64 6976 2063 6c61 7373 3d22 636f    <div class="co
+000016d0: 6c2d 6d64 2d35 223e 0a20 2020 2020 2020  l-md-5">.       
+000016e0: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
+000016f0: 7479 7065 3d22 6e75 6d62 6572 2220 7374  type="number" st
+00001700: 6570 3d22 3122 2069 643d 2274 6f6f 6c5f  ep="1" id="tool_
+00001710: 7175 616c 6966 6963 6174 696f 6e5f 6578  qualification_ex
+00001720: 7069 7261 7469 6f6e 5f64 6179 7322 206e  piration_days" n
+00001730: 616d 653d 2274 6f6f 6c5f 7175 616c 6966  ame="tool_qualif
+00001740: 6963 6174 696f 6e5f 6578 7069 7261 7469  ication_expirati
+00001750: 6f6e 5f64 6179 7322 2063 6c61 7373 3d22  on_days" class="
+00001760: 666f 726d 2d63 6f6e 7472 6f6c 2220 7661  form-control" va
+00001770: 6c75 653d 227b 2520 6966 2065 7272 6f72  lue="{% if error
+00001780: 732e 746f 6f6c 5f71 7561 6c69 6669 6361  s.tool_qualifica
+00001790: 7469 6f6e 5f65 7870 6972 6174 696f 6e5f  tion_expiration_
+000017a0: 6461 7973 2025 7d7b 7b20 6572 726f 7273  days %}{{ errors
+000017b0: 2e74 6f6f 6c5f 7175 616c 6966 6963 6174  .tool_qualificat
+000017c0: 696f 6e5f 6578 7069 7261 7469 6f6e 5f64  ion_expiration_d
+000017d0: 6179 732e 7661 6c75 6520 7d7d 7b25 2065  ays.value }}{% e
+000017e0: 6c73 6520 257d 7b7b 2074 6f6f 6c5f 7175  lse %}{{ tool_qu
+000017f0: 616c 6966 6963 6174 696f 6e5f 6578 7069  alification_expi
+00001800: 7261 7469 6f6e 5f64 6179 7320 7d7d 7b25  ration_days }}{%
+00001810: 2065 6e64 6966 2025 7d22 2f3e 0a20 2020   endif %}"/>.   
+00001820: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00001830: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00001840: 2063 6c61 7373 3d22 636f 6c2d 6d64 2d6f   class="col-md-o
+00001850: 6666 7365 742d 3320 636f 6c2d 6d64 2d39  ffset-3 col-md-9
+00001860: 2068 656c 702d 626c 6f63 6b20 6c69 6768   help-block ligh
+00001870: 742d 6772 6579 223e 0a20 2020 2020 2020  t-grey">.       
+00001880: 2020 2020 2020 2020 207b 2520 6966 2065           {% if e
+00001890: 7272 6f72 732e 746f 6f6c 5f71 7561 6c69  rrors.tool_quali
+000018a0: 6669 6361 7469 6f6e 5f65 7870 6972 6174  fication_expirat
+000018b0: 696f 6e5f 6461 7973 2025 7d0a 2020 2020  ion_days %}.    
+000018c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018d0: 7b7b 2065 7272 6f72 732e 746f 6f6c 5f71  {{ errors.tool_q
+000018e0: 7561 6c69 6669 6361 7469 6f6e 5f65 7870  ualification_exp
+000018f0: 6972 6174 696f 6e5f 6461 7973 2e65 7272  iration_days.err
+00001900: 6f72 207d 7d0a 2020 2020 2020 2020 2020  or }}.          
+00001910: 2020 2020 2020 7b25 2065 6c73 6520 257d        {% else %}
+00001920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001930: 2020 2020 2054 6865 206e 756d 6265 7220       The number 
+00001940: 6f66 2064 6179 7320 6265 666f 7265 2074  of days before t
+00001950: 6865 2075 7365 7227 7320 746f 6f6c 2071  he user's tool q
+00001960: 7561 6c69 6669 6361 7469 6f6e 2065 7870  ualification exp
+00001970: 6972 6573 2073 696e 6365 2074 6865 2075  ires since the u
+00001980: 7365 7220 6c61 7374 2075 7365 6420 7468  ser last used th
+00001990: 6520 746f 6f6c 2e0a 2020 2020 2020 2020  e tool..        
+000019a0: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
+000019b0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+000019c0: 3c2f 6469 763e 0a20 2020 2020 2020 203c  </div>.        <
+000019d0: 2f64 6976 3e0a 2020 2020 2020 2020 3c64  /div>.        <d
+000019e0: 6976 2063 6c61 7373 3d22 666f 726d 2d67  iv class="form-g
+000019f0: 726f 7570 207b 2520 6966 2065 7272 6f72  roup {% if error
+00001a00: 732e 746f 6f6c 5f71 7561 6c69 6669 6361  s.tool_qualifica
+00001a10: 7469 6f6e 5f65 7870 6972 6174 696f 6e5f  tion_expiration_
+00001a20: 6e65 7665 725f 7573 6564 5f64 6179 7320  never_used_days 
+00001a30: 257d 6861 732d 6572 726f 727b 2520 656e  %}has-error{% en
+00001a40: 6469 6620 257d 223e 0a20 2020 2020 2020  dif %}">.       
+00001a50: 2020 2020 203c 6c61 6265 6c20 636c 6173       <label clas
+00001a60: 733d 2263 6f6e 7472 6f6c 2d6c 6162 656c  s="control-label
+00001a70: 2063 6f6c 2d6d 642d 3322 2066 6f72 3d22   col-md-3" for="
+00001a80: 746f 6f6c 5f71 7561 6c69 6669 6361 7469  tool_qualificati
+00001a90: 6f6e 5f65 7870 6972 6174 696f 6e5f 6e65  on_expiration_ne
+00001aa0: 7665 725f 7573 6564 5f64 6179 7322 3e45  ver_used_days">E
+00001ab0: 7870 6972 6174 696f 6e20 6461 7973 2028  xpiration days (
+00001ac0: 6e6f 2074 6f6f 6c20 7573 6167 6529 3c2f  no tool usage)</
+00001ad0: 6c61 6265 6c3e 0a20 2020 2020 2020 2020  label>.         
+00001ae0: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
+00001af0: 6f6c 2d6d 642d 3522 3e0a 2020 2020 2020  ol-md-5">.      
+00001b00: 2020 2020 2020 2020 2020 3c69 6e70 7574            <input
+00001b10: 2074 7970 653d 226e 756d 6265 7222 2073   type="number" s
+00001b20: 7465 703d 2231 2220 6964 3d22 746f 6f6c  tep="1" id="tool
+00001b30: 5f71 7561 6c69 6669 6361 7469 6f6e 5f65  _qualification_e
+00001b40: 7870 6972 6174 696f 6e5f 6e65 7665 725f  xpiration_never_
+00001b50: 7573 6564 5f64 6179 7322 206e 616d 653d  used_days" name=
+00001b60: 2274 6f6f 6c5f 7175 616c 6966 6963 6174  "tool_qualificat
+00001b70: 696f 6e5f 6578 7069 7261 7469 6f6e 5f6e  ion_expiration_n
+00001b80: 6576 6572 5f75 7365 645f 6461 7973 2220  ever_used_days" 
+00001b90: 636c 6173 733d 2266 6f72 6d2d 636f 6e74  class="form-cont
+00001ba0: 726f 6c22 2076 616c 7565 3d22 7b25 2069  rol" value="{% i
+00001bb0: 6620 6572 726f 7273 2e74 6f6f 6c5f 7175  f errors.tool_qu
+00001bc0: 616c 6966 6963 6174 696f 6e5f 6578 7069  alification_expi
+00001bd0: 7261 7469 6f6e 5f6e 6576 6572 5f75 7365  ration_never_use
+00001be0: 645f 6461 7973 2025 7d7b 7b20 6572 726f  d_days %}{{ erro
+00001bf0: 7273 2e74 6f6f 6c5f 7175 616c 6966 6963  rs.tool_qualific
+00001c00: 6174 696f 6e5f 6578 7069 7261 7469 6f6e  ation_expiration
+00001c10: 5f6e 6576 6572 5f75 7365 645f 6461 7973  _never_used_days
+00001c20: 2e76 616c 7565 207d 7d7b 2520 656c 7365  .value }}{% else
+00001c30: 2025 7d7b 7b20 746f 6f6c 5f71 7561 6c69   %}{{ tool_quali
+00001c40: 6669 6361 7469 6f6e 5f65 7870 6972 6174  fication_expirat
+00001c50: 696f 6e5f 6e65 7665 725f 7573 6564 5f64  ion_never_used_d
+00001c60: 6179 7320 7d7d 7b25 2065 6e64 6966 2025  ays }}{% endif %
+00001c70: 7d22 2f3e 0a20 2020 2020 2020 2020 2020  }"/>.           
+00001c80: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+00001c90: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00001ca0: 636f 6c2d 6d64 2d6f 6666 7365 742d 3320  col-md-offset-3 
+00001cb0: 636f 6c2d 6d64 2d39 2068 656c 702d 626c  col-md-9 help-bl
+00001cc0: 6f63 6b20 6c69 6768 742d 6772 6579 223e  ock light-grey">
+00001cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001ce0: 207b 2520 6966 2065 7272 6f72 732e 746f   {% if errors.to
+00001cf0: 6f6c 5f71 7561 6c69 6669 6361 7469 6f6e  ol_qualification
+00001d00: 5f65 7870 6972 6174 696f 6e5f 6e65 7665  _expiration_neve
+00001d10: 725f 7573 6564 5f64 6179 7320 257d 0a20  r_used_days %}. 
+00001d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d30: 2020 207b 7b20 6572 726f 7273 2e74 6f6f     {{ errors.too
+00001d40: 6c5f 7175 616c 6966 6963 6174 696f 6e5f  l_qualification_
+00001d50: 6578 7069 7261 7469 6f6e 5f6e 6576 6572  expiration_never
+00001d60: 5f75 7365 645f 6461 7973 2e65 7272 6f72  _used_days.error
+00001d70: 207d 7d0a 2020 2020 2020 2020 2020 2020   }}.            
+00001d80: 2020 2020 7b25 2065 6c73 6520 257d 0a20      {% else %}. 
+00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001da0: 2020 2054 6865 206e 756d 6265 7220 6f66     The number of
+00001db0: 2064 6179 7320 6265 666f 7265 2074 6865   days before the
+00001dc0: 2075 7365 7227 7320 746f 6f6c 2071 7561   user's tool qua
+00001dd0: 6c69 6669 6361 7469 6f6e 2065 7870 6972  lification expir
+00001de0: 6573 2073 696e 6365 2074 6865 2075 7365  es since the use
+00001df0: 7220 7175 616c 6966 6965 6420 666f 7220  r qualified for 
+00001e00: 7468 6520 6669 7273 7420 7469 6d65 2e0a  the first time..
+00001e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e20: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+00001e30: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00001e40: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+00001e50: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00001e60: 3d22 666f 726d 2d67 726f 7570 207b 2520  ="form-group {% 
+00001e70: 6966 2065 7272 6f72 732e 746f 6f6c 5f71  if errors.tool_q
+00001e80: 7561 6c69 6669 6361 7469 6f6e 5f63 6320  ualification_cc 
+00001e90: 257d 6861 732d 6572 726f 727b 2520 656e  %}has-error{% en
+00001ea0: 6469 6620 257d 223e 0a20 2020 2020 2020  dif %}">.       
+00001eb0: 2020 2020 203c 6c61 6265 6c20 636c 6173       <label clas
+00001ec0: 733d 2263 6f6e 7472 6f6c 2d6c 6162 656c  s="control-label
+00001ed0: 2063 6f6c 2d6d 642d 3322 2066 6f72 3d22   col-md-3" for="
+00001ee0: 746f 6f6c 5f71 7561 6c69 6669 6361 7469  tool_qualificati
+00001ef0: 6f6e 5f63 6322 3e52 656d 696e 6465 722f  on_cc">Reminder/
+00001f00: 6578 7069 7261 7469 6f6e 2043 433c 2f6c  expiration CC</l
+00001f10: 6162 656c 3e0a 2020 2020 2020 2020 2020  abel>.          
+00001f20: 2020 3c64 6976 2063 6c61 7373 3d22 636f    <div class="co
+00001f30: 6c2d 6d64 2d35 223e 0a20 2020 2020 2020  l-md-5">.       
+00001f40: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
+00001f50: 7479 7065 3d22 7465 7874 2220 6964 3d22  type="text" id="
+00001f60: 746f 6f6c 5f71 7561 6c69 6669 6361 7469  tool_qualificati
+00001f70: 6f6e 5f63 6322 206e 616d 653d 2274 6f6f  on_cc" name="too
+00001f80: 6c5f 7175 616c 6966 6963 6174 696f 6e5f  l_qualification_
+00001f90: 6363 2220 636c 6173 733d 2266 6f72 6d2d  cc" class="form-
+00001fa0: 636f 6e74 726f 6c22 2076 616c 7565 3d22  control" value="
+00001fb0: 7b25 2069 6620 6572 726f 7273 2e74 6f6f  {% if errors.too
+00001fc0: 6c5f 7175 616c 6966 6963 6174 696f 6e5f  l_qualification_
+00001fd0: 6363 2025 7d7b 7b20 6572 726f 7273 2e74  cc %}{{ errors.t
+00001fe0: 6f6f 6c5f 7175 616c 6966 6963 6174 696f  ool_qualificatio
+00001ff0: 6e5f 6363 2e76 616c 7565 207d 7d7b 2520  n_cc.value }}{% 
+00002000: 656c 7365 2025 7d7b 7b20 746f 6f6c 5f71  else %}{{ tool_q
+00002010: 7561 6c69 6669 6361 7469 6f6e 5f63 6320  ualification_cc 
+00002020: 7d7d 7b25 2065 6e64 6966 2025 7d22 2070  }}{% endif %}" p
+00002030: 6c61 6365 686f 6c64 6572 3d22 696e 666f  laceholder="info
+00002040: 726d 6174 696f 6e40 6578 616d 706c 652e  rmation@example.
+00002050: 6f72 6722 2f3e 0a20 2020 2020 2020 2020  org"/>.         
+00002060: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00002070: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00002080: 3d22 636f 6c2d 6d64 2d6f 6666 7365 742d  ="col-md-offset-
+00002090: 3320 636f 6c2d 6d64 2d39 2068 656c 702d  3 col-md-9 help-
+000020a0: 626c 6f63 6b20 6c69 6768 742d 6772 6579  block light-grey
+000020b0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+000020c0: 2020 207b 2520 6966 2065 7272 6f72 732e     {% if errors.
+000020d0: 746f 6f6c 5f71 7561 6c69 6669 6361 7469  tool_qualificati
+000020e0: 6f6e 5f63 6320 257d 0a20 2020 2020 2020  on_cc %}.       
+000020f0: 2020 2020 2020 2020 2020 2020 207b 7b20               {{ 
+00002100: 6572 726f 7273 2e74 6f6f 6c5f 7175 616c  errors.tool_qual
+00002110: 6966 6963 6174 696f 6e5f 6363 2e65 7272  ification_cc.err
+00002120: 6f72 207d 7d0a 2020 2020 2020 2020 2020  or }}.          
+00002130: 2020 2020 2020 7b25 2065 6c73 6520 257d        {% else %}
+00002140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002150: 2020 2020 2045 7874 7261 2065 6d61 696c       Extra email
+00002160: 2061 6464 7265 7373 2074 6f20 636f 7079   address to copy
+00002170: 2077 6865 6e20 6120 7573 6572 2773 2074   when a user's t
+00002180: 6f6f 6c20 7175 616c 6966 6963 6174 696f  ool qualificatio
+00002190: 6e20 7265 6d69 6e64 6572 2f65 7870 6972  n reminder/expir
+000021a0: 6174 696f 6e20 656d 6169 6c20 6973 2073  ation email is s
+000021b0: 656e 742e 2041 2063 6f6d 6d61 2d73 6570  ent. A comma-sep
+000021c0: 6172 6174 6564 206c 6973 7420 6361 6e20  arated list can 
+000021d0: 6265 2075 7365 642e 0a20 2020 2020 2020  be used..       
+000021e0: 2020 2020 2020 2020 207b 2520 656e 6469           {% endi
+000021f0: 6620 257d 0a20 2020 2020 2020 2020 2020  f %}.           
+00002200: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+00002210: 3c2f 6469 763e 0a20 2020 2020 2020 203c  </div>.        <
+00002220: 6469 7620 636c 6173 733d 2263 7573 746f  div class="custo
+00002230: 6d69 7a61 7469 6f6e 2d73 6570 6172 6174  mization-separat
+00002240: 696f 6e22 2073 7479 6c65 3d22 6d61 7267  ion" style="marg
+00002250: 696e 2d62 6f74 746f 6d3a 2031 3570 7822  in-bottom: 15px"
+00002260: 3e3c 2f64 6976 3e0a 2020 2020 2020 2020  ></div>.        
+00002270: 3c64 6976 2063 6c61 7373 3d22 7465 7874  <div class="text
+00002280: 2d63 656e 7465 7222 3e0a 2020 2020 2020  -center">.      
+00002290: 2020 2020 2020 7b25 2062 7574 746f 6e20        {% button 
+000022a0: 7479 7065 3d22 7361 7665 2220 7661 6c75  type="save" valu
+000022b0: 653d 2253 6176 6520 7365 7474 696e 6773  e="Save settings
+000022c0: 2220 257d 0a20 2020 2020 2020 203c 2f64  " %}.        </d
+000022d0: 6976 3e0a 2020 2020 3c2f 6469 763e 0a20  iv>.    </div>. 
+000022e0: 2020 203c 7363 7269 7074 2074 7970 653d     <script type=
+000022f0: 2274 6578 742f 6a61 7661 7363 7269 7074  "text/javascript
+00002300: 223e 0a20 2020 2020 2020 2024 2822 2374  ">.        $("#t
+00002310: 6f6f 6c2d 7461 622d 6c69 6e6b 2229 2e63  ool-tab-link").c
+00002320: 6c69 636b 2866 756e 6374 696f 6e28 2920  lick(function() 
+00002330: 7b73 6574 5469 6d65 6f75 7428 6f6e 5f74  {setTimeout(on_t
+00002340: 6f6f 6c5f 7461 625f 7368 6f77 2c20 3530  ool_tab_show, 50
+00002350: 297d 293b 0a20 2020 2020 2020 2066 756e  )});.        fun
+00002360: 6374 696f 6e20 6f6e 5f74 6f6f 6c5f 7461  ction on_tool_ta
+00002370: 625f 7368 6f77 2829 0a20 2020 2020 2020  b_show().       
+00002380: 207b 0a20 2020 2020 2020 2020 2020 2061   {.            a
+00002390: 7574 6f5f 7369 7a65 5f74 6578 7461 7265  uto_size_textare
+000023a0: 6128 646f 6375 6d65 6e74 2e67 6574 456c  a(document.getEl
+000023b0: 656d 656e 7442 7949 6428 2774 6f6f 6c5f  ementById('tool_
+000023c0: 636f 6e74 726f 6c5f 636f 6e66 6967 7572  control_configur
+000023d0: 6174 696f 6e5f 7365 7474 696e 675f 7465  ation_setting_te
+000023e0: 6d70 6c61 7465 2729 290a 2020 2020 2020  mplate')).      
+000023f0: 2020 7d0a 2020 2020 2020 2020 6f6e 5f74    }.        on_t
+00002400: 6f6f 6c5f 7461 625f 7368 6f77 2829 3b0a  ool_tab_show();.
+00002410: 2020 2020 3c2f 7363 7269 7074 3e0a 3c2f      </script>.</
+00002420: 666f 726d 3e                             form>
```

### Comparing `NEMO-4.5.5/NEMO/templates/customizations/customizations_upload.html` & `NEMO-4.6.0/NEMO/templates/customizations/customizations_upload.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/customizations/customizations_user.html` & `NEMO-4.6.0/NEMO/templates/customizations/customizations_user.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/email/compose_email.html` & `NEMO-4.6.0/NEMO/templates/email/compose_email.html`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 			<form action="{% url 'send_broadcast_email' %}" id="email_form" method="post">
 				{% csrf_token %}
 				<div class="col-sm-6">
                     <div class="row">
                         <div class="col-sm-6 h3">Recipients</div>
                         <div class="col-sm-6 h3">{% if user_emails %}{% button type="export" size="small" value="Export user list" onclick="export_user_emails();" %}{% endif %}</div>
                     </div>
-					Active users are listed below in black. Inactive users are <span style="color:lightgrey">gray</span>.
+					Active users are listed below in black. Inactive users are <span class="light-grey strikethrough">crossed out</span>.
 					<div class="checkbox">
 						<label><input type="checkbox" name="only_active_users" onclick="updated_email_link()" checked> Only send this email to active users</label>
 					</div>
 					<div class="checkbox">
 						<label><input type="checkbox" name="copy_me" onclick="updated_email_link()" checked> Send a copy of this email to myself</label>
 					</div>
 					{% for u in users %}
-						<span {% if not u.is_active %}style="color:lightgrey"{% endif %}>{{ u }} - {{ u.email }}</span><br>
+						<span {% if not u.is_active %}class="light-grey strikethrough"{% endif %}>{{ u }} - {{ u.email }}</span><br>
 					{% endfor %}
 				</div>
 				<div class="col-sm-6">
 					<h3>Email content</h3>
 					<input type="hidden" name="audience" value="{{ audience }}">
 					<input type="hidden" name="no_type" value="{{ no_type }}">
                     {% for selection_value in selection %}
```

### Comparing `NEMO-4.5.5/NEMO/templates/email/email_broadcast.html` & `NEMO-4.6.0/NEMO/templates/email/email_broadcast.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/email/email_form.html` & `NEMO-4.6.0/NEMO/templates/email/email_form.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/event_details/area_access_details.html` & `NEMO-4.6.0/NEMO/templates/event_details/area_access_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/event_details/outage_details.html` & `NEMO-4.6.0/NEMO/templates/event_details/outage_details.html`

 * *Files 13% similar despite different names*

```diff
@@ -16,13 +16,13 @@
     {% if outage.details %}
         Details:<br>
         {{ outage.details|linebreaksbr }}
     {% endif %}
 
     {# Allow the user to cancel the outage if they have that priviledge. only in popup view #}
     {% if user.is_staff and popup_view %}
-        <div class="modal-footer">
+        <div class="modal-footer" style="padding: 15px 0 0 0;">
             {% url 'cancel_outage' outage.id as cancel_outage_url %}
             {% button type="delete" value="Cancel this outage" dismiss="modal" onclick="$('#dialog').one('hidden.bs.modal', function() { cancel_outage('"|concat:cancel_outage_url|concat:"', 'Outage "|concat:outage.id|concat:"'); });" %}
         </div>
     {% endif %}
 {% endblock %}
```

### Comparing `NEMO-4.5.5/NEMO/templates/event_details/reservation_details.html` & `NEMO-4.6.0/NEMO/templates/event_details/reservation_details.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 {% extends popup_view|yesno:"base/popup.html,base.html" %}
 {% load custom_tags_and_filters %}
+{% load tz %}
 
 {% if not popup_view %}
 {% block extrahead %}
     <script type="text/javascript">
     function callback_success(){
         // if on a standalone page, reload the browser window to display the results of the change to the reservation
         location.reload()
@@ -23,14 +24,22 @@
 
     function set_reservation_title(url, reservation_id, title)
     {
         let failure_dialog = ajax_failure_callback("Unable to set reservation title");
         ajax_post(url, {'title': title}, callback_success, [failure_dialog]);
     }
 
+    function change_reservation_date(url, reservation_id, param, value)
+    {
+        let failure_dialog = ajax_failure_callback("Unable to change reservation date");
+        let data = {'id': reservation_id};
+        data[param] = value;
+        ajax_post(url, data, callback_success, [failure_dialog]);
+    }
+
     function change_reservation_project(url, project_id)
     {
         let failure_dialog = ajax_failure_callback("Unable to change reservation project");
         function callback_failure(){
             $('#reservation_project').show();
             $('#reservation_change_project').hide();
         }
@@ -53,18 +62,18 @@
 		<div class="alert alert-danger">This reservation was automatically removed from the calendar due to {{ reservation.reservation_item_type.value }} inactivity.</div>
 	{% endif %}
 
     <table class="table table-striped">
 
 	{% if user.is_staff %}
     <tr>
-        <td style="vertical-align: middle">Title:</td>
+        <td style="vertical-align: middle"><label for="title">Title:</label></td>
         <td>
             <div class="input-group">
-                <input type="text" id="title" aria-label="Reservation title" class="form-control" placeholder="{{ reservation.user }}" maxlength="200" value="{{ reservation.title }}">
+                <input type="text" id="title"  class="form-control" placeholder="{{ reservation.user }}" maxlength="200" value="{{ reservation.title }}">
                 <span class="input-group-btn">
                     <button type="button" class="btn btn-success" data-dismiss="modal" onclick="{% if popup_view %}$('#dialog').one('hidden.bs.modal', function() { {% endif %}set_reservation_title('{% url 'set_reservation_title' reservation.id %}', {{ reservation.id }}, $('#title').val()) {% if popup_view %}}){% endif %}">Set title</button>
                 </span>
             </div>
         </td>
     </tr>
 	{% elif reservation.title %}
@@ -103,15 +112,15 @@
             <td>
                 {{ reservation.project }}
                 {% if reservation_project_can_be_changed %}<span class="glyphicon glyphicon-pencil pull-right" title="Change the project" onclick="$('#reservation_project').hide();$('#reservation_change_project').show();"></span>{% endif %}
             </td>
         </tr>
         {% if reservation_project_can_be_changed %}
             <tr id="reservation_change_project" style="display: none;">
-                <td style="vertical-align: middle;">Project:</td>
+                <td style="vertical-align: middle;"><label for="change_project">Project:</label></td>
                 <td>
                     <div class="input-group">
                         <select id="change_project" name="project" aria-label="Reservation project" class="form-control">
                             {% for p in reservation.user.active_projects %}
                                 <option value="{{ p.id }}" {% if reservation.project.id == p.id %}selected{% endif %}>{% project_selection_display p %}</option>
                             {% endfor %}
                         </select>
@@ -120,20 +129,48 @@
                         </span>
                     </div>
                 </td>
             </tr>
         {% endif %}
 	{% endif %}
     <tr>
-        <td>Start:</td>
-        <td>{{ reservation.start }}</td>
+        {% if request.user == reservation.user and reservation.has_not_ended and reservation.has_not_started %}
+            <td style="vertical-align: middle"><label for="reservation_start" style="margin-bottom: 0">Start:</label></td>
+            <td id="reservation_display_start">
+                {{ reservation.start }}
+                <span class="glyphicon glyphicon-pencil pull-right" title="Change the start date" onclick="$('#reservation_display_start').hide();$('#reservation_change_start').show();"></span>
+            </td>
+            <td id="reservation_change_start" style="display: none">
+                <div class="input-group">
+                    <input type="text" id="reservation_start" class="form-control" value="{{ reservation.start|localtime|input_date_format }}">
+                    <span class="input-group-btn">
+                        <button type="button" class="btn btn-success" data-dismiss="modal" onclick="{% if popup_view %}$('#dialog').one('hidden.bs.modal', function() { {% endif %}change_reservation_date('{% url 'change_reservation_date' %}', {{ reservation.id }}, 'new_start', $('#reservation_start').val()) {% if popup_view %}}){% endif %}">Change start</button>
+                    </span>
+                </div>
+            </td>
+        {% else %}
+            <td>Start:</td>
+            <td>{{ reservation.start }}</td>
+        {% endif %}
     </tr>
     <tr>
-        <td>End:</td>
-        <td>{{ reservation.end }}</td>
+        {% if request.user == reservation.user and reservation.has_not_ended and reservation.has_not_started %}
+            <td style="vertical-align: middle"><label for="reservation_end">End:</label></td>
+            <td>
+                <div class="input-group">
+                    <input type="text" id="reservation_end" class="form-control" value="{{ reservation.end|localtime|input_date_format }}">
+                    <span class="input-group-btn">
+                        <button type="button" class="btn btn-success" data-dismiss="modal" onclick="{% if popup_view %}$('#dialog').one('hidden.bs.modal', function() { {% endif %}change_reservation_date('{% url 'change_reservation_date' %}', {{ reservation.id }}, 'new_end', $('#reservation_end').val()) {% if popup_view %}}){% endif %}">Change end</button>
+                    </span>
+                </div>
+            </td>
+        {% else %}
+            <td>End:</td>
+            <td>{{ reservation.end }}</td>
+        {% endif %}
     </tr>
     <tr>
         <td>Identifier:</td>
         <td>{{ reservation.id }}</td>
     </tr>
     {% if reservation.question_data_json.items %}
     <tr>
@@ -174,15 +211,15 @@
         </tr>
     {% endif %}
     </table>
 
     {# Allow the user to cancel the reservation if they have that priviledge. #}
     {% if not reservation.missed and not reservation.cancelled %}
         {% if reservation.user.id == user.id and reservation.has_not_ended or user.is_staff %}
-            <div class="modal-footer">
+            <div class="modal-footer" style="padding: 15px 0 0 0;">
                 {# You must provide a reason if you are cancelling someone else's reservation. #}
                 {% if reservation.user == user %}
                     <button type="button" class="btn btn-danger" data-dismiss="modal" onclick="{% if popup_view %}$('#dialog').one('hidden.bs.modal', function() { {% endif %}cancel_reservation('{% url 'cancel_reservation' reservation.id %}', 'Reservation {{ reservation.id }}') {% if popup_view %}}){% endif %}" title="Cancel this reservation"><i class="glyphicon glyphicon-trash"></i> Cancel this reservation</button>
                 {% else %}
                     <div class="input-group">
                         <input type="text" id="reason" class="form-control" placeholder="Reason for cancellation (required)" aria-label="Reason for cancellation (required)" maxlength="3000">
                         <span class="input-group-btn">
```

#### html2text {}

```diff
@@ -1,41 +1,53 @@
 {% extends popup_view|yesno:"base/popup.html,base.html" %} {% load
-custom_tags_and_filters %} {% if not popup_view %} {% block extrahead %}
+custom_tags_and_filters %} {% load tz %} {% if not popup_view %} {% block
+extrahead %}
  {% endblock %} {% endif %} {% block title %}{{ reservation.reservation_item }}
 reservation details{% endblock %} {% block content %} {% if not popup_view %}
 ****** {{ reservation.reservation_item }} reservation details ******
 {% endif %} {% if reservation.short_notice %}
 {{ facility_name }} staff were not given sufficient notice to configure this
 tool. There is no guarantee that this tool will be configured properly at time
 of use.
 {% endif %} {% if reservation.missed %}
 This reservation was automatically removed from the calendar due to {
 { reservation.reservation_item_type.value }} inactivity.
 {% endif %}
-Title:                  [{{ reservation.title }}]  Set title
-Title:                  {{ reservation.title }}
-User:                   {{_reservation.user_}}
-Created by:             {{ reservation.creator }}
-Created on:             {{ reservation.creation_time }}
-Tool:                   {{_reservation.tool_}}
-Area:                   {{ reservation.area }}
-Project:                {{ reservation.project }} {% if
-                        reservation_project_can_be_changed %}{% endif %}
-                        {% for p in reservation.user.active_projects %}
-                        % if reservation.project.id == p.id %}selected{% endif
-Project:                %}>{% project_selection_display p %}
-                        {% endfor %}
-                          Change project
-Start:                  {{ reservation.start }}
-End:                    {{ reservation.end }}
-Identifier:             {{ reservation.id }}
-Reservation questions:
-Self-configuration:     {{ reservation.user }} has opted to perform the tool
-                        configuration
-Additional information: {{ reservation.additional_information|linebreaksbr }}
+Title:         [{{ reservation.title }}]  Set title
+Title:         {{ reservation.title }}
+User:          {{_reservation.user_}}
+Created by:    {{ reservation.creator }}
+Created on:    {{ reservation.creation_time }}
+Tool:          {{_reservation.tool_}}
+Area:          {{ reservation.area }}
+               {{ reservation.project }} {% if
+Project:       reservation_project_can_be_changed %}{% endif
+               %}
+               {% for p in reservation.user.active_projects %}
+               % if reservation.project.id == p.id %}selected
+Project:       {% endif %}>{% project_selection_display p %}
+               {% endfor %}
+                 Change project
+                                                               [{                                                            {
+Start:         {{ reservation.start }}                         {                                             Start:          {
+                                                               reservation.start|localtime|input_date_format                 reservation.start
+                                                               }}]  Change start                                             }}
+                                                                                                             {
+End:           [{{ reservation.end|localtime|input_date_format End:                                          {
+               }}]  Change end                                                                               reservation.end
+                                                                                                             }}
+Identifier:    {{ reservation.id }}
+Reservation
+questions:
+Self-          {{ reservation.user }} has opted to perform the
+configuration: tool configuration
+               {
+Additional     {
+information:   reservation.additional_information|linebreaksbr
+               }}
 {# Allow the user to cancel the reservation if they have that priviledge. #} {%
 if not reservation.missed and not reservation.cancelled %} {% if
 reservation.user.id == user.id and reservation.has_not_ended or user.is_staff
 %}
 {# You must provide a reason if you are cancelling someone else's reservation.
 #} {% if reservation.user == user %}  Cancel this reservation {% else %}
 [                    ]   Cancel this reservation
```

### Comparing `NEMO-4.5.5/NEMO/templates/event_details/usage_details.html` & `NEMO-4.6.0/NEMO/templates/event_details/usage_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/feedback.html` & `NEMO-4.6.0/NEMO/templates/feedback.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/history.html` & `NEMO-4.6.0/NEMO/templates/history.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/impersonate.html` & `NEMO-4.6.0/NEMO/templates/impersonate.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 {% extends 'base.html' %}
 {% load custom_tags_and_filters %}
+{% block title %}Impersonate{% endblock %}
 
 {% block content %}
 	<form class="form-horizontal" action="{% url 'impersonate' %}" method="post">
 		{% csrf_token %}
 		<input id="user_id" name="user_id" type="hidden"/>
 		<p>This form allows you to impersonate any active user.</p>
 		<div class="form-group">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends 'base.html' %} {% load custom_tags_and_filters %} {% block content
-%}
+{% extends 'base.html' %} {% load custom_tags_and_filters %} {% block title
+%}Impersonate{% endblock %} {% block content %}
 {% csrf_token %}
 This form allows you to impersonate any active user.
 [                    ]
 {% button id="impersonate_submit" type="warn" submit=True value="Impersonate"
 icon="glyphicon-user" %}
 {% endblock %}
```

### Comparing `NEMO-4.5.5/NEMO/templates/jumbotron/jumbotron.html` & `NEMO-4.6.0/NEMO/templates/jumbotron/jumbotron.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/jumbotron/jumbotron_content.html` & `NEMO-4.6.0/NEMO/templates/jumbotron/jumbotron_content.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/landing.html` & `NEMO-4.6.0/NEMO/templates/landing.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 {% extends 'base.html' %}
 {% load static %}
 {% load custom_tags_and_filters %}
 
 {% block title %}{{ site_title }}{% endblock %}
 {% block content %}
+    <h1 class="sr-only">Main dashboard</h1>
 	{% if user.training_required %}
 		<div class="row">
 			<div class="col-lg-12">
 				<a href="{% url 'facility_rules' %}">
 					<div class="well clearfix">
 						<div class="col-lg-2 text-center"><img src="{% static 'icons/caution.png' %}" alt="Caution image" height="128" width="128"></div>
 						<div class="col-lg-8 text-center">
@@ -108,15 +109,15 @@
 					<a href="{{ choice.url }}" {% if choice.open_in_new_tab %}target="_blank" {% else %}onclick="show_spinner();"{% endif %} {% if choice.secure_referral %}rel="noopener noreferrer"{% endif %} style="text-decoration: none !important">
 						<img src="{{ choice.image.url }}" alt="{{ choice.name }} icon" height="128" width="128">
 						<h3 style="margin-top:0">
 							{{ choice.name }}
 							{% if choice.notifications %}
 								{% for type, count in notification_counts.items %}
 									{% if choice.notifications == type and count %}
-										<span class="badge" style="vertical-align:middle; background-color:red">{{ count }}</span>
+										<span class="badge active">{{ count }}</span>
 									{% endif %}
 								{% endfor %}
 							{% endif %}
 						</h3>
 					</a>
 				</div>
 			{% if forloop.counter|divisibleby:4 or forloop.last %}</div>{% endif %}
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 {% extends 'base.html' %} {% load static %} {% load custom_tags_and_filters %}
-{% block title %}{{ site_title }}{% endblock %} {% block content %} {% if
-user.training_required %}
+{% block title %}{{ site_title }}{% endblock %} {% block content %}
+****** Main dashboard ******
+{% if user.training_required %}
 [Caution_image]
 *****_{{_facility_name_}}_Rules_Tutorial_*****
 You_must_complete_your_{{_facility_name_}}_rules_tutorial_before_you_can_make
 reservations_or_use_{{_facility_name_}}_tools._Click_here_to_begin_the
 tutorial.
 [Agreement_icon]
 {% endif %}
```

### Comparing `NEMO-4.5.5/NEMO/templates/login.html` & `NEMO-4.6.0/NEMO/templates/login.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/maintenance/closed_task_details.html` & `NEMO-4.6.0/NEMO/templates/maintenance/closed_task_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/maintenance/maintenance.html` & `NEMO-4.6.0/NEMO/templates/maintenance/maintenance.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/maintenance/pending_task_details.html` & `NEMO-4.6.0/NEMO/templates/maintenance/pending_task_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/mobile/cancellation_result.html` & `NEMO-4.6.0/NEMO/templates/mobile/cancellation_result.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/mobile/choose_item.html` & `NEMO-4.6.0/NEMO/templates/mobile/choose_item.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/mobile/individual_outage.html` & `NEMO-4.6.0/NEMO/templates/mobile/individual_outage.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/mobile/individual_reservation.html` & `NEMO-4.6.0/NEMO/templates/mobile/individual_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/mobile/new_reservation.html` & `NEMO-4.6.0/NEMO/templates/mobile/new_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/mobile/reservation_success.html` & `NEMO-4.6.0/NEMO/templates/mobile/reservation_success.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/mobile/view_calendar.html` & `NEMO-4.6.0/NEMO/templates/mobile/view_calendar.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/news/archived_news.html` & `NEMO-4.6.0/NEMO/templates/news/archived_news.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/news/new_news_form.html` & `NEMO-4.6.0/NEMO/templates/news/new_news_form.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/news/news_update_form.html` & `NEMO-4.6.0/NEMO/templates/news/news_update_form.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/news/recent_news.html` & `NEMO-4.6.0/NEMO/templates/news/recent_news.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/occupancy/occupancy_content.html` & `NEMO-4.6.0/NEMO/templates/occupancy/occupancy_content.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/occupancy/occupancy_count.html` & `NEMO-4.6.0/NEMO/templates/occupancy/occupancy_count.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/pagination/pagination_base.html` & `NEMO-4.6.0/NEMO/templates/pagination/pagination_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/pagination/pagination_column.html` & `NEMO-4.6.0/NEMO/templates/pagination/pagination_column.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/pagination/pagination_pages.html` & `NEMO-4.6.0/NEMO/templates/pagination/pagination_pages.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/pagination/pagination_selector.html` & `NEMO-4.6.0/NEMO/templates/pagination/pagination_selector.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/qualifications.html` & `NEMO-4.6.0/NEMO/templates/qualifications.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/refresh_sidebar_icons.html` & `NEMO-4.6.0/NEMO/templates/refresh_sidebar_icons.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/remote_work/remote_work.html` & `NEMO-4.6.0/NEMO/templates/remote_work/remote_work.html`

 * *Files 6% similar despite different names*

```diff
@@ -90,43 +90,45 @@
 			<th>End</th>
 			{% if remote_work_validation %}<th>Validate</th>{% endif %}
 		</tr>
 		</thead>
 		<tbody>
 		{% for c in staff_charges %}
 			<tr class="staff_charge_row_{{ c.id }} {% if remote_work_validation and  c.validated %}success-highlight{% endif %}">
-				{% if "django.contrib.admin"|app_installed and perms.NEMO.change_staffcharge %}
-                    <td><a href="{% url 'admin:NEMO_staffcharge_change' c.id %}">{{ c.id }}</a></td>
+				{% admin_edit_url c request.build_absolute_uri as edit_url %}
+                {% if edit_url %}
+                    <td><a href="{{ edit_url }}">{{ c.id }}</a></td>
                 {% else %}
                     <td>{{ c.id }}</td>
                 {% endif %}
 				<td>{{ c.staff_member }}</td>
 				<td>{{ c.customer }}</td>
 				<td>{{ c.project }}</td>
 				<td>{{ c.start }}</td>
 				<td>{{ c.end|default_if_none:'' }}</td>
 				{% if remote_work_validation %}
                     <td {% if c.note and c.areaaccessrecord_set.exists %}rowspan="3" {% elif c.note or c.areaaccessrecord_set.exists %}rowspan="2"{% endif %} style="vertical-align: middle">
                         {% url 'validate_staff_charge' c.id as validate_staff_charge_url %}
-                        {% if not c.validated %}
+                        {% if c.end and not c.validated %}
                             {% button type="save" submit=False onclick="validate_charge('"|concat:validate_staff_charge_url|concat:"', this, '.staff_charge_row_"|concat:c.id|concat:"')" icon="glyphicon-ok-circle" value="Validate" %}
                         {% endif %}
                     </td>
                 {% endif %}
 			</tr>
             {% if c.note %}
                 <tr class="staff_charge_row_{{ c.id }} {% if remote_work_validation and c.validated %}success-highlight{% endif %}">
                     <td style="border: none; padding-top: 0"></td>
                     <td colspan="5" style="border:none; padding-top: 0">Charge note: {{ c.note|linebreaksbr }}<br></td>
                 </tr>
             {% endif %}
 			{% for area_access_record in c.areaaccessrecord_set.all %}
 				<tr class="staff_charge_row_{{ c.id }} {% if remote_work_validation and c.validated %}success-highlight{% endif %}" style="font-size: smaller">
-					{% if "django.contrib.admin"|app_installed and perms.NEMO.change_areaaccessrecord %}
-                        <td><a href="{% url 'admin:NEMO_areaaccessrecord_change' area_access_record.id %}">{{ area_access_record.id }}</a></td>
+					{% admin_edit_url area_access_record request.build_absolute_uri as edit_url %}
+                    {% if edit_url %}
+                        <td><a href="{{ edit_url }}">{{ area_access_record.id }}</a></td>
                     {% else %}
                         <td>{{ area_access_record.id }}</td>
                     {% endif %}
 					<td colspan="3" style="border-top-style: dotted">{{ area_access_record.area.name }} access</td>
 					<td style="border-top-style: dotted">{{ area_access_record.start }}</td>
 					<td style="border-top-style: dotted">{{ area_access_record.end|default_if_none:'' }}</td>
 				</tr>
@@ -154,29 +156,30 @@
 			<th>Tool</th>
 			{% if remote_work_validation %}<th>Validate</th>{% endif %}
 		</tr>
 		</thead>
 		<tbody>
 		{% for u in usage %}
 			<tr {% if remote_work_validation and u.validated %}class="success-highlight"{% endif %} id="usage_event_row_{{ forloop.counter }}">
-				{% if "django.contrib.admin"|app_installed and perms.NEMO.change_usageevent %}
-                    <td><a href="{% url 'admin:NEMO_usageevent_change' u.id %}">{{ u.id }}</a></td>
+				{% admin_edit_url u request.build_absolute_uri as edit_url %}
+                {% if edit_url %}
+                    <td><a href="{{ edit_url }}">{{ u.id }}</a></td>
                 {% else %}
                     <td>{{ u.id }}</td>
                 {% endif %}
 				<td>{{ u.operator }}</td>
 				<td>{{ u.user }}</td>
 				<td>{{ u.project }}</td>
 				<td>{{ u.start }}</td>
 				<td>{{ u.end|default_if_none:'' }}</td>
 				<td>{{ u.tool }}</td>
 				{% if remote_work_validation %}
                     <td>
                         {% url 'validate_usage_event' u.id as validate_usage_url %}
-                        {% if not u.validated %}
+                        {% if u.end and not u.validated %}
                             {% button type="save" submit=False onclick="validate_charge('"|concat:validate_usage_url|concat:"', this, '#usage_event_row_"|concat:forloop.counter|concat:"')" icon="glyphicon-ok-circle" value="Validate" %}
                         {% endif %}
                     </td>
                 {% endif %}
 			</tr>
         {% empty %}
             <tr><td colspan="8">
```

### Comparing `NEMO-4.5.5/NEMO/templates/remote_work/remote_work_base.html` & `NEMO-4.6.0/NEMO/templates/remote_work/remote_work_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/requests/access_requests/access_request.html` & `NEMO-4.6.0/NEMO/templates/requests/access_requests/access_request.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/requests/access_requests/access_requests.html` & `NEMO-4.6.0/NEMO/templates/requests/access_requests/access_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/requests/access_requests/access_requests_table.html` & `NEMO-4.6.0/NEMO/templates/requests/access_requests/access_requests_table.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/requests/adjustment_requests/adjustment_request.html` & `NEMO-4.6.0/NEMO/templates/requests/adjustment_requests/adjustment_request.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/requests/adjustment_requests/adjustment_requests.html` & `NEMO-4.6.0/NEMO/templates/requests/adjustment_requests/adjustment_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html` & `NEMO-4.6.0/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,17 @@
                 <td class="text-center" style="vertical-align: middle">{{ a_request.item.get_display }}</td>
                 <td class="text-center" style="vertical-align: middle">{{ a_request.get_new_start|date:'SHORT_DATETIME_FORMAT' }}</td>
                 <td class="text-center" style="vertical-align: middle">{{ a_request.get_new_end|date:'SHORT_DATETIME_FORMAT' }}</td>
                 <td class="text-center" style="vertical-align: middle">{{ a_request.get_time_difference|default_if_none:"" }}</td>
                 <td class="text-right text-nowrap" style="vertical-align: middle">
                     {% if request_status == 'approved' or request_status == 'denied' %}
                         {{ a_request.reviewer.get_name }}
-                        {% if request_status == 'approved' and a_request.editable_charge and "django.contrib.admin"|app_installed and "requests"|customization:"adjustment_requests_edit_charge_button" == "enabled" %}
-                            {% admin_edit_url a_request.item as edit_url %}
+                        {% if request_status == 'approved' and a_request.editable_charge and "requests"|customization:"adjustment_requests_edit_charge_button" == "enabled" %}
+                            {% url "user_requests" "adjustment" as redirect_adjustment_url %}
+                            {% admin_edit_url a_request.item redirect_adjustment_url as edit_url %}
                             {% if edit_url %}
                                 <br>{% button type="edit" size="small" value="Edit charge" url=edit_url %}
                             {% endif %}
                         {% endif %}
                     {% else %}
                         {% if request_status == 'pending' and user.is_facility_manager %}
                             <a class="btn btn-sm btn-default" title="Approve/Deny" href="{% url 'edit_adjustment_request' a_request.id %}"><i class="glyphicon glyphicon-ok-circle success-highlight"></i>&nbsp;&nbsp;<i class="glyphicon glyphicon-ban-circle danger-highlight"></i> Review</a>
```

#### html2text {}

```diff
@@ -5,27 +5,28 @@
                                                                                                                                                                                                    Approved by {% elif request_status ==
                                                                                                                                                                                                    'denied' %} Denied by {% endif %}
                                                                                                                                                                                                    {% if request_status == 'approved' or
                                                                                                                                                                                                    request_status == 'denied' %} {
                                                                                                                                                                                                    { a_request.reviewer.get_name }} {% if
                                                                                                                                                                                                    request_status == 'approved' and
                                                                                                                                                                                                    a_request.editable_charge and
-                                                                                                                                                                                                   "django.contrib.admin"|app_installed and
                                                                                                                                                                                                    "requests"|customization:
                                                                                                                                                                                                    "adjustment_requests_edit_charge_button"
-                                                                                                                                                                                                   == "enabled" %} {% admin_edit_url
-                                                                                                                                                                                                   a_request.item as edit_url %} {% if
-                                                                                                                                                                                                   edit_url %}
+                                                                                                                                                                                                   == "enabled" %} {% url "user_requests"
+                                                                                                                                                                                                   "adjustment" as redirect_adjustment_url
+                                                                                                                                                                                                   %} {% admin_edit_url a_request.item
+                                                                                                                                                                                                   redirect_adjustment_url as edit_url %}
+                                                                                                                                                                                                   {% if edit_url %}
                                                                                                                                                                                                    {% button type="edit" size="small"
                                                                                                                                                                                                    value="Edit charge" url=edit_url %} {%
-{% if a_request.id in                                                                                                                                                                              endif %} {% endif %} {% else %} {% if
+{% if a_request.id in               {                          {                          {                             {                           {                                              endif %} {% endif %} {% else %} {% if
 request_notifications %}New {%      {                          {                          {                             {                           {                                              request_status == 'pending' and
-endif %}{                           {                          {                          {                             {                           {                                              user.is_facility_manager %}
-{ a_request.creation_time|date:     a_request.creator.get_name a_request.item.get_display a_request.get_new_start|date: a_request.get_new_end|date: a_request.get_time_difference|default_if_none:   _Review
-'SHORT_DATETIME_FORMAT' }}          }}                         }}                         'SHORT_DATETIME_FORMAT' }}    'SHORT_DATETIME_FORMAT' }}  "" }}                                           {% endif %} {% if request_status ==
+endif %}{                           a_request.creator.get_name a_request.item.get_display a_request.get_new_start|date: a_request.get_new_end|date: a_request.get_time_difference|default_if_none: user.is_facility_manager %}
+{ a_request.creation_time|date:     }}                         }}                         'SHORT_DATETIME_FORMAT' }}    'SHORT_DATETIME_FORMAT' }}  "" }}                                            _Review
+'SHORT_DATETIME_FORMAT' }}                                                                                                                                                                          {% endif %} {% if request_status ==
                                                                                                                                                                                                    'pending' and a_request.creator == user
                                                                                                                                                                                                    %} {% url 'edit_adjustment_request'
                                                                                                                                                                                                    a_request.id as edit_request_url %} {%
                                                                                                                                                                                                    url 'delete_adjustment_request'
                                                                                                                                                                                                    a_request.id as delete_request_url %} {%
                                                                                                                                                                                                    button type="edit" size="small"
                                                                                                                                                                                                    value="Edit" title="Edit request"
```

### Comparing `NEMO-4.5.5/NEMO/templates/requests/buddy_requests/buddy_request.html` & `NEMO-4.6.0/NEMO/templates/requests/buddy_requests/buddy_request.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/requests/buddy_requests/buddy_requests.html` & `NEMO-4.6.0/NEMO/templates/requests/buddy_requests/buddy_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/requests/user_requests.html` & `NEMO-4.6.0/NEMO/templates/requests/user_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/resources/modify_resource.html` & `NEMO-4.6.0/NEMO/templates/resources/modify_resource.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/resources/resource_details.html` & `NEMO-4.6.0/NEMO/templates/resources/resource_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/resources/resources.html` & `NEMO-4.6.0/NEMO/templates/resources/resources.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/resources/scheduled_outage.html` & `NEMO-4.6.0/NEMO/templates/resources/scheduled_outage.html`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 						<option {% if oc.name == form.category.value %}selected{% endif %}>{{ oc }}</option>
 					{% endfor %}
 				</select>
 			</div>
 		{% endif %}
 		<div class="form-group">
 			<label for="details">Details</label>{% if form.details.errors %} - <span style="color:red">{{ form.details.errors|striptags }}</span>{% endif %}
-			<textarea class="form-control" rows="3" name="details" id="details" maxlength="{{ form.fields.details.max_length }}" placeholder="What is the reason for the outage? What other details will be relevant for users to know?">{{ form.details.value|default_if_none:"" }}</textarea>
+			<textarea aria-labelledby="outage_details_help" class="form-control" rows="3" name="details" id="details" maxlength="{{ form.fields.details.max_length }}">{{ form.details.value|default_if_none:"" }}</textarea>
+            <div class="light-grey" id="outage_details_help">What is the reason for the outage? What other details will be relevant for users to know?</div>
 		</div>
 		<div class="form-group">
 			<div class="row">
 				<div class="col-sm-6">
 					<label for="start">Start time</label>{% if form.start.errors %} - <span style="color:red">{{ form.start.errors|striptags }}</span>{% endif %}
 					<input type="text" class="form-control" name="start" id="start" value="{{ form.start.value|input_date_format }}">
 				</div>
```

#### html2text {}

```diff
@@ -27,13 +27,15 @@
 {% for oc in outage_categories %}
 % if oc.name == form.category.value %}selected{% endif %}>{{ oc }}
 {% endfor %}
 {% endif %}
 Details{% if form.details.errors %} - {{ form.details.errors|striptags }}{%
 endif %}
 {{ form.details.value|default_if_none:"" }}
+What is the reason for the outage? What other details will be relevant for
+users to know?
 Start time{% if form.start.errors %} - {{ form.start.errors|striptags }}{%
 endif %} [{{ form.start.value|input_date_format }}]
 End time{% if form.end.errors %} - {{ form.end.errors|striptags }}{% endif %} [
 {{ form.end.value|input_date_format }}]
 {% button type="save" value=editing|yesno:"Save changes,Create outage" %}
  {% endblock %}
```

### Comparing `NEMO-4.5.5/NEMO/templates/safety/safety.html` & `NEMO-4.6.0/NEMO/templates/safety/safety.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/safety/safety_base.html` & `NEMO-4.6.0/NEMO/templates/safety/safety_base.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends 'base.html' %}
 {% load custom_tags_and_filters %}
 {% block content %}
-    <div id="safety_tabs" class="clearfix" style="margin-top: 0;margin-bottom: 15px">
-        <h1 class="pull-left" style="margin-top: 0;margin-right: 20px">{% block safety_title %}Safety{% endblock %}</h1>
+    <div id="safety-tabs" class="clearfix">
+        <h1 class="safety-title pull-left">{% block safety_title %}Safety{% endblock %}</h1>
         {% if show_tabs > 1 %}
-            <ul class="nav nav-pills nav-pills-spacer" id="tabs" style="display: inline-block;float: right;">
+            <ul class="nav nav-pills nav-pills-spacer safety-tabs-nav" id="tabs">
                 {% if show_safety %}
                     <li class="{% if tab == 'safety' %}active{% endif %}">
                         <a href="#safety" onclick="location.href = '{% url "safety" %}'">Safety</a>
                     </li>
                 {% endif %}
                 {% if show_safety_issues %}
                     <li class="{% if tab == 'safety_issues' %}active{% endif %}">
```

### Comparing `NEMO-4.5.5/NEMO/templates/safety/safety_data_sheets.html` & `NEMO-4.6.0/NEMO/templates/safety/safety_data_sheets.html`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,19 @@
         </div>
     </div>
     {% if chemicals %}
         <div id="safety_data_sheets_container" class="container" style="bottom: 45px;top: 175px;position: absolute; max-height: 100%; overflow-y: auto;overflow-x: hidden; margin-top: 25px; padding: 0 30px 0 0;">
             <table class="table table-align-middle table-responsive table-bordered table-condensed table-hover thead-light" style="overflow: auto; height: 1px;table-layout: fixed;">
                 <thead class="sticky">
                     <tr>
-                        <th class="sds-box-shadow-bottom" style="border-left-style: hidden !important; border-top-style: hidden!important;background-color: white"></th>
+                        <th class="sds-box-shadow-bottom" style="border-left-style: hidden !important; border-top-style: hidden!important;background-color: white" aria-label="Empty cell"></th>
                         {% for hazard in hazards %}
                             <th class="text-center sds-box-shadow-bottom" style="width: calc(75%/{{ hazards|length }})"><img style="display:block; width: 100%;" alt="{{ hazard.name }} logo" src="{% get_media_prefix %}{{ hazard.logo }}"/></th>
                         {% endfor %}
-                        <th class="sds-box-shadow-bottom" style="display: none;border-right-style: hidden!important; border-top-style: hidden!important;background-color: white">
+                        <th class="sds-box-shadow-bottom" style="display: none;border-right-style: hidden!important; border-top-style: hidden!important;background-color: white" aria-label="Empty cell"></th>
                     </tr>
                     <tr>
                         <th class="text-center sds-box-shadow-top" style="overflow: hidden;vertical-align: middle">
                             <span class="pagination-column" style="white-space: inherit;display: inline">
                                 <a href="?o={% if order_by == "name" %}-{% endif %}name">Name<span class="{% if order_by != "name" and order_by != "-name" %}hidden{% endif %} glyphicon glyphicon-triangle-{% if hazard_order == "name" %}bottom{% else %}top{% endif %}"></span></a>
                             </span>
                         </th>
@@ -112,15 +112,15 @@
             {
                 rows.show();
             }
         });
 
         function resize_container()
         {
-            const safety_height = $(".navbar.navbar-default").outerHeight(true) + $("#safety_tabs").outerHeight(true) + $("#data_sheets_header").outerHeight(true) + 20;
+            const safety_height = $(".navbar.navbar-default").outerHeight(true) + $("#safety-tabs").outerHeight(true) + $("#data_sheets_header").outerHeight(true) + 20;
             $("#safety_data_sheets_container").css("top", safety_height + "px");
         }
         $(window).on("resize", resize_container);
         resize_container();
 
         if ({{ search_keywords|yesno:"true,false" }})
         {
```

### Comparing `NEMO-4.5.5/NEMO/templates/safety/safety_issues.html` & `NEMO-4.6.0/NEMO/templates/safety/safety_issues.html`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 				<a href="{% url 'update_safety_issue' ticket.id %}" style="text-decoration: none">
 			{% endif %}
 			<div class="panel panel-default">
 				<div class="panel-body">
 					<div class="form-group">
 						<h4>
 							{% if ticket.id in notifications %}
-								<span class="badge" style="vertical-align:middle; background-color:red">New</span>
+								<span class="badge active" style="vertical-align:middle;">New</span>
 							{% endif %}
 							Concern
 						</h4>
 						{{ ticket.concern|linebreaksbr }}
 					</div>
 					<div class="form-group">
 						{% if not ticket.visible %}<span class="glyphicon glyphicon-eye-close"></span> This issue is hidden from users<br>{% endif %}
```

### Comparing `NEMO-4.5.5/NEMO/templates/safety/safety_issues_create.html` & `NEMO-4.6.0/NEMO/templates/safety/safety_issues_create.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/safety/safety_issues_resolved.html` & `NEMO-4.6.0/NEMO/templates/safety/safety_issues_resolved.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/safety/safety_issues_update.html` & `NEMO-4.6.0/NEMO/templates/safety/safety_issues_update.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/safety/safety_items.html` & `NEMO-4.6.0/NEMO/templates/safety/safety_items.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+{% load custom_tags_and_filters %}
 <div class="tab-content panel panel-default">
     {% if safety_category %}
     <div class="panel-heading pointer" data-toggle="collapse" data-target="#items-{{ safety_category.id }}" onclick="toggle_details($(this).children(':first'))">
         <h3 class="panel-title pointer"><i class="glyphicon glyphicon-chevron-down chevron"></i> {{ safety_category }}</h3>
     </div>
     <div class="collapse in" id="items-{{ safety_category.id }}">
         <div class="panel-body">
@@ -12,15 +13,17 @@
                     <li id="safety_item_{{ safety_item.id }}" style="margin-bottom: 15px"><u>{{ safety_item.name }}:</u>
                         {% if safety_item.description %}
                             <div style="margin: 5px 0">{{ safety_item.description|safe|linebreaksbr }}</div>
                         {% endif %}
                         <ul>
                             {% for doc in safety_item.safetyitemdocuments_set.all %}
                                 {% if doc.can_be_embedded %}
-                                    <li><a href="#" onclick="open_doc('{% url 'media_view' 'true' 'safety_document' doc.id %}')">{{ doc.filename }}</a></li>
+                                    {% with content_type=doc|content_type %}
+                                        <li><a href="#" onclick="open_doc('{% url 'media_view' 'true' content_type.id doc.id %}')">{{ doc.filename }}</a></li>
+                                    {% endwith %}
                                 {% else %}
                                     <li><a href="{{ doc.link }}" target="_blank">{{ doc.filename }}</a></li>
                                 {% endif %}
                             {% endfor %}
                         </ul>
                     </li>
                 {% endfor %}
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
+{% load custom_tags_and_filters %}
 {% if safety_category %}
  {{ safety_category }}
 {% endif %}
     * {% for safety_item in safety_items %}
     * {{_safety_item.name_}}: {% if safety_item.description %}
       {{ safety_item.description|safe|linebreaksbr }}
       {% endif %}
           o {% for doc in safety_item.safetyitemdocuments_set.all %} {% if
-            doc.can_be_embedded %}
+            doc.can_be_embedded %} {% with content_type=doc|content_type %}
           o {{_doc.filename_}}
-          o {% else %}
+          o {% endwith %} {% else %}
           o {{_doc.filename_}}
           o {% endif %} {% endfor %}
     * {% endfor %}
 {% if safety_category %}
 {% endif %}
```

### Comparing `NEMO-4.5.5/NEMO/templates/snippets/button.html` & `NEMO-4.6.0/NEMO/templates/snippets/button.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/snippets/contact_person.html` & `NEMO-4.6.0/NEMO/templates/snippets/contact_person.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/snippets/embedded_document.html` & `NEMO-4.6.0/NEMO/templates/snippets/embedded_document.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/snippets/tool_info.html` & `NEMO-4.6.0/NEMO/templates/snippets/tool_info.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/staff_charges/change_status.html` & `NEMO-4.6.0/NEMO/templates/staff_charges/change_status.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/staff_charges/choose_project.html` & `NEMO-4.6.0/NEMO/templates/staff_charges/choose_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/staff_charges/new_staff_charge.html` & `NEMO-4.6.0/NEMO/templates/staff_charges/new_staff_charge.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/staff_charges/reminder.html` & `NEMO-4.6.0/NEMO/templates/staff_charges/reminder.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% load custom_tags_and_filters %}
 <div class="modal-header">
-	<button type="button" class="close" data-dismiss="modal">&times;</button>
-	<h4 class="modal-title">Would you like to end your staff charge?</h4>
+	<button type="button" class="close" data-dismiss="modal" aria-label="Modal close button">&times;</button>
+	<h4 id="modal-description-label" class="modal-title">Would you like to end your staff charge?</h4>
 </div>
 
 <div class="modal-body">
 	{% with user.get_staff_charge as staff_charge %}
 		You are charging staff time to {{ staff_charge.customer }} for the project named
 		{{ staff_charge.project }} since {{ staff_charge.start }}.
 		Now that you have finished using the {{ tool.name_or_child_in_use_name }} on this person's behalf, would you
```

### Comparing `NEMO-4.5.5/NEMO/templates/staff_charges/staff_charges_base.html` & `NEMO-4.6.0/NEMO/templates/staff_charges/staff_charges_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/status_dashboard/occupancy.html` & `NEMO-4.6.0/NEMO/templates/status_dashboard/occupancy.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/status_dashboard/staff.html` & `NEMO-4.6.0/NEMO/templates/status_dashboard/staff.html`

 * *Files 10% similar despite different names*

```diff
@@ -2,92 +2,97 @@
 {% load tz %}
 <style>
 .table-hover-first tr:hover td:is(:first-child)
 {
   background: #ddd !important;
 }
 </style>
+{% if staffs %}
 <div class="row" style="display: table-row;">
     <div style="display: table-cell;width: 100%">
         Staff availability is highlighted in <span style="display: inline-block; padding: 3px" class="alert-success">green</span><br>
         Staff partial availability is highlighted in <span style="display: inline-block; padding: 3px" class="alert-warning">orange</span><br>
         Staff absence is highlighted in <span style="display: inline-block; padding: 3px" class="alert-danger">red</span><br><br>
 
         Extra information (if available) can be found by hovering over a time block<br>
         Clicking on a staff member will display their contact information
     </div>
     {% if user_view != 'day' %}
         <div style="display: table-cell; vertical-align: bottom; width: 100%">
             <div style="display: inline-flex">
                 <div class="btn-group" role="group" style="display: inline-flex">
-                    <button type="button" class="btn btn-default {% if page_view == 'day' %}active{% endif %}" onclick="location.href = '?timestamp={{ page_timestamp }}&view=day'" {% if page_view == 'day' %}aria-pressed="true"{% endif %}>Day</button>
-                    <button type="button" class="btn btn-default {% if not page_view or page_view == 'week' %}active{% endif %}" onclick="location.href = '?timestamp={{ page_timestamp }}&view=week'" {% if not page_view or page_view == 'week' %}aria-pressed="true"{% endif %}>Week</button>
+                    <button type="button" class="btn btn-default {% if page_view == 'day' %}active{% endif %}" onclick="refresh_staff_status_dashboard('timestamp={{ page_timestamp }}&view=day');" {% if page_view == 'day' %}aria-pressed="true"{% endif %}>Day</button>
+                    <button type="button" class="btn btn-default {% if not page_view or page_view == 'week' %}active{% endif %}" onclick="refresh_staff_status_dashboard('timestamp={{ page_timestamp }}&view=week');" {% if not page_view or page_view == 'week' %}aria-pressed="true"{% endif %}>Week</button>
                     {% if not user_view %}
-                        <button type="button" class="btn btn-default {% if page_view == 'month' %}active{% endif %}" onclick="location.href = '?timestamp={{ page_timestamp }}&view=month'" {% if page_view == 'month' %}aria-pressed="true"{% endif %}>Month</button>
+                        <button type="button" class="btn btn-default {% if page_view == 'month' %}active{% endif %}" onclick="refresh_staff_status_dashboard('timestamp={{ page_timestamp }}&view=month');" {% if page_view == 'month' %}aria-pressed="true"{% endif %}>Month</button>
                     {% endif %}
                 </div>
                 {% if user.is_facility_manager %}
                     {% url 'status_dashboard_tab' 'staff' as staff_status_url %}
                     {% button style="margin-left: 10px" value="Export" type="export" url=staff_status_url|concat:"?timestamp="|concat:page_timestamp|concat:"&view="|concat:page_view|concat:"&csv=true" role="button" target="_blank" %}
                 {% endif %}
             </div>
         </div>
     {% endif %}
 </div>
 <div id="contact-info-tooltip-container" class="info-tooltip-container" style="overflow-x: auto; margin-top: 25px; margin-bottom: 20px; border: 1px solid #ddd;">
     <table class="table table-responsive table-hover-first" style="margin: 0;border-collapse: collapse">
         <thead>
             <tr class="no-border">
-                <th class="sticky" {% if days_length == 1 %}style="width:33%"{% endif %}></th>
+                <th class="sticky" style="background-color: white; {% if days_length == 1 %}width:33%{% endif %}" aria-label="Blank corner cell"></th>
                 {% if prev %}
-                    <th class="button-column-minimum" style="vertical-align: middle;">
-                        <a href="{% url 'status_dashboard_tab' 'staff' %}?timestamp={{ prev }}&view={{ page_view }}">
+                    <th class="button-column-minimum" style="vertical-align: middle;" aria-label="Previous page cell">
+                        <a style="cursor: pointer" onclick="refresh_staff_status_dashboard('timestamp={{ page_timestamp }}&view=week');" aria-label="Previous page button">
                             <i class="glyphicon glyphicon-chevron-left chevron" style="padding: 0"></i>
                         </a>
                     </th>
                 {% endif %}
                 {% for day in days %}
                     {% now 'Y-m-d' as today %}
                     <th class="text-center {% if day|date:'Y-m-d' == today %}alert-info{% endif %}">
                         <span {% if day|date:'Y-m-d' == today %}data-toggle='tooltip' data-title="Today's date"{% endif %}>{{ day|date:staff_date_format }}</span>
                     </th>
                 {% endfor %}
                 {% if next %}
-                    <th class="button-column-minimum" style="vertical-align: middle;">
-                        <a href="{% url 'status_dashboard_tab' 'staff' %}?timestamp={{ next }}&view={{ page_view }}">
+                    <th class="button-column-minimum" style="vertical-align: middle;" aria-label="Next page cell">
+                        <a style="cursor: pointer" onclick="refresh_staff_status_dashboard('timestamp={{ next }}&view={{ page_view }}')" aria-label="Next page button">
                             <i class="glyphicon glyphicon-chevron-right chevron" style="padding: 0"></i>
                         </a>
                     </th>
                 {% endif %}
             </tr>
         </thead>
         <tbody>
         {% regroup staffs by category as category_staff %}
             {% for category in category_staff %}
                 <tr>
                     <th colspan="{% if prev %}3{% else %}2{% endif %}" class="sticky">{{ category.grouper|default_if_none:'Other' }}</th>
-                    {% if next or days_length != 1 %}<th colspan="{% if next %}{{ days_length|add:'1' }}{% else %}{{ days_length }}{% endif %}"></th>{% endif %}
+                    {% if next or days_length != 1 %}<th aria-label="Staff category empty cells" colspan="{% if next %}{{ days_length|add:'1' }}{% else %}{{ days_length }}{% endif %}"></th>{% endif %}
                 </tr>
                 {% for staff in category.list %}
-                    <tr>
+                    <tr class="default">
                         <td style="vertical-align: middle;" class="sticky">
                             <div class="text-nowrap staff-status-contact">{{ staff.staff_member.get_contact_info_html|safe }}</div>
                             <div class="staff-status-add">{% if user.is_facility_manager %}<span class="glyphicon glyphicon-plus-sign success-highlight" onclick="ajax_get('{% url "create_staff_absence" %}?staff_id={{ staff.id }}&timestamp={{ page_timestamp }}&view={{ page_view }}', undefined, ajax_success_callback)" title="Add staff absence"></span>{% endif %}</div>
                         </td>
                         {% for day in days %}
                             {% with staff_available=staff.weekly_availability|get_item:day.weekday staff_absent=staff_absences|get_item:staff.id|get_item:day.day closure_time=closure_times|get_item:day.day %}
                                 {% with start_closure_time=closure_time.start_time|localtime end_closure_time=closure_time.end_time|localtime %}
                                 <td {% if prev and next and days_length == 1 %}colspan="3" {% elif forloop.first and prev or forloop.last and next %}colspan="2"{% endif %} class="staff-status-availability text-center {% if staff_absent or closure_time %}{% if staff_absent and not staff_absent.full_day %}alert-warning{% elif closure_time %}{% if start_closure_time.date == day.date and start_closure_time.hour > 0 or start_closure_time.date == day.date and start_closure_time.minute > 0 %}alert-warning{% elif end_closure_time.date == day.date and end_closure_time.hour < 23 or end_closure_time.date == day.date and end_closure_time.minute < 59 %}alert-warning{% else %}alert-danger{% endif %}{% else %}alert-danger{% endif %}{% elif staff_available %}alert-success{% elif not user.is_facility_manager %}alert-danger{% endif %}">
                                     {% if closure_time %}
                                         {% with custom_data_template="<div class='tooltip' role='tooltip'><div class='arrow'></div><div class='tooltip-inner' style='text-align:left; max-width: 300px'></div></div>" %}
                                             <div data-toggle="tooltip" data-template="{{ custom_data_template }}" title="{% if closure_time.closure.alert_template %}{{ closure_time.alert_contents|linebreaksbr }}{% else %}{{ closure_time.closure.name }} {{ closure_time }}{% endif %}"><div>Closed</div></div>
                                         {% endwith %}
                                     {% elif staff_absent %}
                                         {% if not user.is_facility_manager %}
-                                            <div data-toggle="tooltip" title="{{ staff_absent.description|linebreaksbr }}">&nbsp;</div>
+                                            {% if "dashboard"|customization:"dashboard_staff_status_absence_view_staff" and user.is_staff or "dashboard"|customization:"dashboard_staff_status_absence_view_user_office" and user.is_user_office or "dashboard"|customization:"dashboard_staff_status_absence_view_accounting_officer" and user.is_accounting_officer %}
+                                                <div data-toggle="tooltip" title="{{ staff_absent.details_for_manager }}"><span>{{ staff_absent.absence_type.name }}</span></div>
+                                            {% else %}
+                                                <div data-toggle="tooltip" title="{{ staff_absent.description|linebreaksbr }}">&nbsp;</div>
+                                            {% endif %}
                                         {% else %}
                                             <div data-toggle="tooltip" title="{{ staff_absent.details_for_manager }}"><span style="cursor: pointer" onclick="ajax_get('{% url "edit_staff_absence" staff_absent.id %}?timestamp={{ page_timestamp }}&view={{ page_view }}', undefined, ajax_success_callback)">{{ staff_absent.absence_type.name }}</span></div>
                                         {% endif %}
                                     {% elif staff_available %}
                                         <div data-toggle="tooltip" title="{{ staff.daily_hours }}">&nbsp;</div>
                                     {% endif %}
                                 </td>
@@ -96,14 +101,17 @@
                         {% endfor %}
                     </tr>
                 {% endfor %}
             {% endfor %}
         </tbody>
     </table>
 </div>
+{% endif %}
 <script>
     $(".contact-info-tooltip").on('click', function () {
+        {# Remove associated data to prevent toggling issues #}
+        $(this).removeData('bs.tooltip');
         $(".tooltip").remove();
       	$(this).tooltip({trigger: 'manual', html: 'true', container: '#contact-info-tooltip-container'}).tooltip('toggle');
     });
     $("[data-toggle='tooltip']").tooltip({html: 'true'});
 </script>
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
 {% load custom_tags_and_filters %} {% load tz %}
+ {% if staffs %}
 Staff availability is highlighted in green
 Staff partial availability is highlighted in orange
 Staff absence is highlighted in red
 
 Extra information (if available) can be found by hovering over a time block
 Clicking on a staff member will display their contact information
 {% if user_view != 'day' %}
@@ -12,23 +13,25 @@
 % if page_view == 'month' %}aria-pressed="true"{% endif %}>Month {% endif %}
 {% if user.is_facility_manager %} {% url 'status_dashboard_tab' 'staff' as
 staff_status_url %} {% button style="margin-left: 10px" value="Export"
 type="export" url=staff_status_url|concat:"?timestamp="|concat:
 page_timestamp|concat:"&view="|concat:page_view|concat:"&csv=true"
 role="button" target="_blank" %} {% endif %}
 {% endif %}
-                                              % if day|date:'Y-m-d' == today
-                                              %}data-toggle='tooltip' data-
-                                              title="Today's date"{% endif %}>
-                                              {{ day|date:staff_date_format }}
+                                               % if day|date:'Y-m-d' == today
+                                               %}data-toggle='tooltip' data-
+                                               title="Today's date"{% endif
+                                               %}>{{ day|date:
+                                               staff_date_format }}
 {{ category.grouper|default_if_none:'Other'
 }}
 {
 {
 staff.staff_member.get_contact_info_html|safe
 }}
 {% if user.is_facility_manager %}
  %}?staff_id={{ staff.id }}&timestamp={
 { page_timestamp }}&view={{ page_view }}',
 undefined, ajax_success_callback)" title="Add
 staff absence">{% endif %}
+{% endif %}
```

### Comparing `NEMO-4.5.5/NEMO/templates/status_dashboard/staff_absence.html` & `NEMO-4.6.0/NEMO/templates/status_dashboard/staff_absence.html`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,16 @@
         if(response)
         {
             $("#dialog .modal-content").html(response);
             $("#dialog").modal('show');
         }
         else
         {
-            window.location = '{% url 'status_dashboard_tab' 'staff' %}?timestamp={{ page_timestamp }}';
+            $("#dialog").modal('hide');
+            refresh_staff_status_dashboard();
         }
     }
 
     function submit_form(form)
     {
         let post_data = serialize("#" + form.id);
         ajax_post(form.action, post_data, absence_callback);
```

### Comparing `NEMO-4.5.5/NEMO/templates/status_dashboard/status_dashboard.html` & `NEMO-4.6.0/NEMO/templates/status_dashboard/status_dashboard.html`

 * *Files 8% similar despite different names*

```diff
@@ -54,310 +54,363 @@
 00000350: 2075 7361 6765 3c2f 613e 3c2f 6c69 3e7b   usage</a></li>{
 00000360: 2520 656e 6469 6620 257d 0a20 2020 207b  % endif %}.    {
 00000370: 2520 6966 2073 686f 775f 7374 6166 665f  % if show_staff_
 00000380: 7374 6174 7573 2025 7d3c 6c69 207b 2520  status %}<li {% 
 00000390: 6966 2074 6162 203d 3d20 2773 7461 6666  if tab == 'staff
 000003a0: 2720 257d 636c 6173 733d 2261 6374 6976  ' %}class="activ
 000003b0: 6522 7b25 2065 6e64 6966 2025 7d3e 3c61  e"{% endif %}><a
-000003c0: 2068 7265 663d 2223 7374 6166 6622 3e53   href="#staff">S
-000003d0: 7461 6666 2073 7461 7475 733c 2f61 3e3c  taff status</a><
-000003e0: 2f6c 693e 7b25 2065 6e64 6966 2025 7d0a  /li>{% endif %}.
-000003f0: 3c2f 756c 3e0a 0a3c 6469 7620 6964 3d22  </ul>..<div id="
-00000400: 636f 6e74 656e 7422 2063 6c61 7373 3d22  content" class="
-00000410: 7461 622d 636f 6e74 656e 7422 2073 7479  tab-content" sty
-00000420: 6c65 3d22 7061 6464 696e 672d 746f 703a  le="padding-top:
-00000430: 3130 7078 223e 0a09 3c64 6976 2063 6c61  10px">..<div cla
-00000440: 7373 3d22 7461 622d 7061 6e65 7b25 2069  ss="tab-pane{% i
-00000450: 6620 6172 6561 735f 6578 6973 7420 616e  f areas_exist an
-00000460: 6420 7461 6220 3d3d 2027 6f63 6375 7061  d tab == 'occupa
-00000470: 6e63 7927 2025 7d20 6163 7469 7665 7b25  ncy' %} active{%
-00000480: 2065 6e64 6966 2025 7d22 2069 643d 226f   endif %}" id="o
-00000490: 6363 7570 616e 6379 223e 0a09 097b 2520  ccupancy">...{% 
-000004a0: 696e 636c 7564 6520 2773 7461 7475 735f  include 'status_
-000004b0: 6461 7368 626f 6172 642f 6f63 6375 7061  dashboard/occupa
-000004c0: 6e63 792e 6874 6d6c 2720 257d 0a09 3c2f  ncy.html' %}..</
-000004d0: 6469 763e 0a09 3c64 6976 2063 6c61 7373  div>..<div class
-000004e0: 3d22 7461 622d 7061 6e65 7b25 2069 6620  ="tab-pane{% if 
-000004f0: 746f 6f6c 735f 6578 6973 7420 616e 6420  tools_exist and 
-00000500: 7461 6220 3d3d 2027 746f 6f6c 7327 2025  tab == 'tools' %
-00000510: 7d20 6163 7469 7665 7b25 2065 6e64 6966  } active{% endif
-00000520: 2025 7d20 696e 666f 2d74 6f6f 6c74 6970   %} info-tooltip
-00000530: 2d63 6f6e 7461 696e 6572 2220 6964 3d22  -container" id="
-00000540: 746f 6f6c 7322 3e0a 0909 3c64 6976 2063  tools">...<div c
-00000550: 6c61 7373 3d22 6274 6e2d 6772 6f75 7020  lass="btn-group 
-00000560: 7369 6465 6261 722d 6974 656d 223e 0a09  sidebar-item">..
-00000570: 0909 3c62 7574 746f 6e20 6964 3d22 6669  ..<button id="fi
-00000580: 6c74 6572 2220 7479 7065 3d22 6275 7474  lter" type="butt
-00000590: 6f6e 2220 636c 6173 733d 2262 746e 2062  on" class="btn b
-000005a0: 746e 2d64 6566 6175 6c74 2064 726f 7064  tn-default dropd
-000005b0: 6f77 6e2d 746f 6767 6c65 2220 6461 7461  own-toggle" data
-000005c0: 2d74 6f67 676c 653d 2264 726f 7064 6f77  -toggle="dropdow
-000005d0: 6e22 207b 2520 6966 206e 6f5f 6865 6164  n" {% if no_head
-000005e0: 6572 2025 7d73 7479 6c65 3d22 6469 7370  er %}style="disp
-000005f0: 6c61 793a 6e6f 6e65 3b22 7b25 2065 6e64  lay:none;"{% end
-00000600: 6966 2025 7d3e 0a09 0909 0953 686f 7769  if %}>.....Showi
-00000610: 6e67 2074 6f6f 6c73 2069 6e20 7573 650a  ng tools in use.
-00000620: 0909 0909 3c73 7061 6e20 636c 6173 733d  ....<span class=
-00000630: 2263 6172 6574 223e 3c2f 7370 616e 3e0a  "caret"></span>.
-00000640: 0909 093c 2f62 7574 746f 6e3e 0a09 0909  ...</button>....
-00000650: 3c75 6c20 636c 6173 733d 2264 726f 7064  <ul class="dropd
-00000660: 6f77 6e2d 6d65 6e75 223e 0a09 0909 093c  own-menu">.....<
-00000670: 6c69 2063 6c61 7373 3d22 6472 6f70 646f  li class="dropdo
-00000680: 776e 2d68 6561 6465 7222 3e46 696c 7465  wn-header">Filte
-00000690: 7220 6279 2e2e 2e3c 2f6c 693e 0a09 0909  r by...</li>....
-000006a0: 093c 6c69 3e3c 6120 6872 6566 3d22 6a61  .<li><a href="ja
-000006b0: 7661 7363 7269 7074 3a76 6f69 6428 3029  vascript:void(0)
-000006c0: 2220 6f6e 636c 6963 6b3d 2266 696c 7465  " onclick="filte
-000006d0: 7228 2761 6c6c 2074 6f6f 6c73 2729 223e  r('all tools')">
-000006e0: 416c 6c20 746f 6f6c 733c 2f61 3e3c 2f6c  All tools</a></l
-000006f0: 693e 0a09 0909 093c 6c69 3e3c 6120 6872  i>.....<li><a hr
-00000700: 6566 3d22 6a61 7661 7363 7269 7074 3a76  ef="javascript:v
-00000710: 6f69 6428 3029 2220 6f6e 636c 6963 6b3d  oid(0)" onclick=
-00000720: 2266 696c 7465 7228 2774 6f6f 6c73 2069  "filter('tools i
-00000730: 6e20 7573 6527 2922 3e54 6f6f 6c73 2069  n use')">Tools i
-00000740: 6e20 7573 653c 2f61 3e3c 2f6c 693e 0a09  n use</a></li>..
-00000750: 0909 093c 6c69 3e3c 6120 6872 6566 3d22  ...<li><a href="
-00000760: 6a61 7661 7363 7269 7074 3a76 6f69 6428  javascript:void(
-00000770: 3029 2220 6f6e 636c 6963 6b3d 2266 696c  0)" onclick="fil
-00000780: 7465 7228 2770 726f 626c 656d 6174 6963  ter('problematic
-00000790: 2074 6f6f 6c73 2729 223e 5072 6f62 6c65   tools')">Proble
-000007a0: 6d61 7469 6320 746f 6f6c 733c 2f61 3e3c  matic tools</a><
-000007b0: 2f6c 693e 0a09 0909 093c 6c69 3e3c 6120  /li>.....<li><a 
-000007c0: 6872 6566 3d22 6a61 7661 7363 7269 7074  href="javascript
-000007d0: 3a76 6f69 6428 3029 2220 6f6e 636c 6963  :void(0)" onclic
-000007e0: 6b3d 2266 696c 7465 7228 2769 646c 6520  k="filter('idle 
-000007f0: 746f 6f6c 7327 2922 3e49 646c 6520 746f  tools')">Idle to
-00000800: 6f6c 733c 2f61 3e3c 2f6c 693e 0a09 0909  ols</a></li>....
-00000810: 3c2f 756c 3e0a 0909 3c2f 6469 763e 0a09  </ul>...</div>..
-00000820: 093c 703e 0a09 093c 6469 7620 6964 3d22  .<p>...<div id="
-00000830: 746f 6f6c 5f73 7461 7475 735f 7461 626c  tool_status_tabl
-00000840: 6522 3e0a 0909 097b 2520 696e 636c 7564  e">....{% includ
-00000850: 6520 2773 7461 7475 735f 6461 7368 626f  e 'status_dashbo
-00000860: 6172 642f 746f 6f6c 732e 6874 6d6c 2720  ard/tools.html' 
-00000870: 257d 0a09 093c 2f64 6976 3e0a 093c 2f64  %}...</div>..</d
-00000880: 6976 3e0a 2020 2020 7b25 2069 6620 7368  iv>.    {% if sh
-00000890: 6f77 5f73 7461 6666 5f73 7461 7475 7320  ow_staff_status 
-000008a0: 257d 0a20 2020 2020 2020 203c 6469 7620  %}.        <div 
-000008b0: 636c 6173 733d 2274 6162 2d70 616e 657b  class="tab-pane{
-000008c0: 2520 6966 2074 6162 203d 3d20 2773 7461  % if tab == 'sta
-000008d0: 6666 2720 257d 2061 6374 6976 657b 2520  ff' %} active{% 
-000008e0: 656e 6469 6620 257d 2220 6964 3d22 7374  endif %}" id="st
-000008f0: 6166 6622 3e0a 2020 2020 2020 2020 2020  aff">.          
-00000900: 2020 7b25 2069 6e63 6c75 6465 2027 7374    {% include 'st
-00000910: 6174 7573 5f64 6173 6862 6f61 7264 2f73  atus_dashboard/s
-00000920: 7461 6666 2e68 746d 6c27 2025 7d0a 2020  taff.html' %}.  
-00000930: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-00000940: 207b 2520 656e 6469 6620 257d 0a3c 2f64   {% endif %}.</d
-00000950: 6976 3e0a 0a3c 7363 7269 7074 3e0a 0966  iv>..<script>..f
-00000960: 756e 6374 696f 6e20 6f6e 5f6c 6f61 6428  unction on_load(
-00000970: 290a 097b 0a09 0966 696c 7465 7228 2774  )..{...filter('t
-00000980: 6f6f 6c73 2069 6e20 7573 6527 293b 0a20  ools in use');. 
-00000990: 2020 2020 2020 206c 6574 2074 6162 5f6a         let tab_j
-000009a0: 7120 3d20 2428 2223 7461 6273 2061 2229  q = $("#tabs a")
-000009b0: 3b0a 0909 7461 625f 6a71 2e63 6c69 636b  ;...tab_jq.click
-000009c0: 2873 7769 7463 685f 7461 6229 3b0a 0909  (switch_tab);...
-000009d0: 7461 625f 6a71 2e63 6c69 636b 2872 6566  tab_jq.click(ref
-000009e0: 7265 7368 5f73 7461 7475 735f 6461 7368  resh_status_dash
-000009f0: 626f 6172 6429 3b0a 0909 7461 625f 6a71  board);...tab_jq
-00000a00: 2e63 6c69 636b 2875 7064 6174 655f 7572  .click(update_ur
-00000a10: 6c29 3b0a 0909 7365 745f 696e 7465 7276  l);...set_interv
-00000a20: 616c 5f77 6865 6e5f 7669 7369 626c 6528  al_when_visible(
-00000a30: 646f 6375 6d65 6e74 2c20 7265 6672 6573  document, refres
-00000a40: 685f 7374 6174 7573 5f64 6173 6862 6f61  h_status_dashboa
-00000a50: 7264 2c20 3130 3030 3029 3b0a 2020 2020  rd, 10000);.    
-00000a60: 2020 2020 7b23 2053 6574 2061 2067 6c6f      {# Set a glo
-00000a70: 6261 6c20 636c 6963 6b20 6861 6e64 6c65  bal click handle
-00000a80: 7220 746f 2064 6973 6d69 7373 206d 616e  r to dismiss man
-00000a90: 7561 6c20 746f 6f6c 7469 7073 2023 7d0a  ual tooltips #}.
-00000aa0: 2020 2020 2020 2020 2428 2768 746d 6c27          $('html'
-00000ab0: 292e 6f6e 2827 636c 6963 6b27 2c20 6675  ).on('click', fu
-00000ac0: 6e63 7469 6f6e 2865 290a 2020 2020 2020  nction(e).      
-00000ad0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00000ae0: 7b23 204f 6e6c 7920 6469 6d69 7373 2074  {# Only dimiss t
-00000af0: 6f6f 6c74 6970 7320 7768 656e 2063 6c69  ooltips when cli
-00000b00: 636b 696e 6720 6f75 7473 6964 6520 6f66  cking outside of
-00000b10: 2074 6865 6d20 237d 0a20 2020 2020 2020   them #}.       
-00000b20: 2020 2020 206c 6574 2074 6172 6765 745f       let target_
-00000b30: 6964 203d 2024 2865 2e74 6172 6765 7429  id = $(e.target)
-00000b40: 2e70 6172 656e 7473 2827 2e74 6f6f 6c74  .parents('.toolt
-00000b50: 6970 2729 2e61 7474 7228 2769 6427 293b  ip').attr('id');
-00000b60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00000b70: 2874 7970 656f 6620 2428 652e 7461 7267  (typeof $(e.targ
-00000b80: 6574 292e 6461 7461 2827 6f72 6967 696e  et).data('origin
-00000b90: 616c 2d74 6974 6c65 2729 203d 3d20 2775  al-title') == 'u
-00000ba0: 6e64 6566 696e 6564 2729 0a20 2020 2020  ndefined').     
-00000bb0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00000bc0: 2020 2020 2020 2020 2024 2822 2e74 6f6f           $(".too
-00000bd0: 6c74 6970 2229 2e6e 6f74 2827 2327 2b74  ltip").not('#'+t
-00000be0: 6172 6765 745f 6964 292e 7265 6d6f 7665  arget_id).remove
-00000bf0: 2829 3b0a 2020 2020 2020 2020 2020 2020  ();.            
-00000c00: 7d0a 2020 2020 2020 2020 7d29 3b0a 097d  }.        });..}
-00000c10: 0a09 2428 6f6e 5f6c 6f61 6429 3b0a 0a20  ..$(on_load);.. 
-00000c20: 2020 2066 756e 6374 696f 6e20 7570 6461     function upda
-00000c30: 7465 5f75 726c 2829 0a20 2020 207b 0a20  te_url().    {. 
-00000c40: 2020 2020 2020 207b 2320 5365 7420 7065         {# Set pe
-00000c50: 726d 616e 656e 7420 7572 6c20 736f 2077  rmanent url so w
-00000c60: 6520 6361 6e20 7265 6672 6573 6820 7370  e can refresh sp
-00000c70: 6563 6966 6963 2074 6162 2023 7d0a 2020  ecific tab #}.  
-00000c80: 2020 2020 2020 6c65 7420 7469 746c 6520        let title 
-00000c90: 3d20 2241 7265 6120 6f63 6375 7061 6e63  = "Area occupanc
-00000ca0: 7922 3b0a 2020 2020 2020 2020 6c65 7420  y";.        let 
-00000cb0: 6e65 775f 7572 6c20 3d20 227b 2520 7572  new_url = "{% ur
-00000cc0: 6c20 2773 7461 7475 735f 6461 7368 626f  l 'status_dashbo
-00000cd0: 6172 645f 7461 6227 2027 6f63 6375 7061  ard_tab' 'occupa
-00000ce0: 6e63 7927 2025 7d22 3b0a 2020 2020 2020  ncy' %}";.      
-00000cf0: 2020 6966 2028 2428 2223 746f 6f6c 7322    if ($("#tools"
-00000d00: 292e 6861 7343 6c61 7373 2822 6163 7469  ).hasClass("acti
-00000d10: 7665 2229 290a 2020 2020 2020 2020 7b0a  ve")).        {.
-00000d20: 2020 2020 2020 2020 2020 2020 7469 746c              titl
-00000d30: 6520 3d20 2254 6f6f 6c20 7374 6174 7573  e = "Tool status
-00000d40: 223b 0a20 2020 2020 2020 2020 2020 206e  ";.            n
-00000d50: 6577 5f75 726c 203d 2022 7b25 2075 726c  ew_url = "{% url
-00000d60: 2027 7374 6174 7573 5f64 6173 6862 6f61   'status_dashboa
-00000d70: 7264 5f74 6162 2720 2774 6f6f 6c73 2720  rd_tab' 'tools' 
-00000d80: 257d 223b 0a20 2020 2020 2020 207d 0a20  %}";.        }. 
-00000d90: 2020 2020 2020 2065 6c73 6520 6966 2028         else if (
-00000da0: 2428 2223 7374 6166 6622 292e 6861 7343  $("#staff").hasC
-00000db0: 6c61 7373 2822 6163 7469 7665 2229 290a  lass("active")).
-00000dc0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00000dd0: 2020 2020 2020 7469 746c 6520 3d20 2253        title = "S
-00000de0: 7461 6666 2073 7461 7475 7322 3b0a 2020  taff status";.  
-00000df0: 2020 2020 2020 2020 2020 6e65 775f 7572            new_ur
-00000e00: 6c20 3d20 227b 2520 7572 6c20 2773 7461  l = "{% url 'sta
-00000e10: 7475 735f 6461 7368 626f 6172 645f 7461  tus_dashboard_ta
-00000e20: 6227 2027 7374 6166 6627 2025 7d22 3b0a  b' 'staff' %}";.
-00000e30: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00000e40: 2020 6869 7374 6f72 792e 7075 7368 5374    history.pushSt
-00000e50: 6174 6528 2727 2c20 7469 746c 652c 206e  ate('', title, n
-00000e60: 6577 5f75 726c 293b 0a20 2020 207d 0a0a  ew_url);.    }..
-00000e70: 0966 756e 6374 696f 6e20 7265 6672 6573  .function refres
-00000e80: 685f 7374 6174 7573 5f64 6173 6862 6f61  h_status_dashboa
-00000e90: 7264 2829 0a09 7b0a 0909 6c65 7420 6f63  rd()..{...let oc
-00000ea0: 6375 7061 6e63 795f 7461 6220 3d20 2428  cupancy_tab = $(
-00000eb0: 2223 6f63 6375 7061 6e63 7922 293b 0a09  "#occupancy");..
-00000ec0: 0969 6628 6f63 6375 7061 6e63 795f 7461  .if(occupancy_ta
-00000ed0: 622e 6861 7343 6c61 7373 2822 6163 7469  b.hasClass("acti
-00000ee0: 7665 2229 290a 0909 096f 6363 7570 616e  ve"))....occupan
-00000ef0: 6379 5f74 6162 2e6c 6f61 6428 227b 2520  cy_tab.load("{% 
-00000f00: 7572 6c20 2773 7461 7475 735f 6461 7368  url 'status_dash
-00000f10: 626f 6172 6427 2025 7d3f 696e 7465 7265  board' %}?intere
-00000f20: 7374 3d6f 6363 7570 616e 6379 2229 3b0a  st=occupancy");.
-00000f30: 0a09 0969 6628 2428 2223 746f 6f6c 7322  ...if($("#tools"
-00000f40: 292e 6861 7343 6c61 7373 2822 6163 7469  ).hasClass("acti
-00000f50: 7665 2229 290a 0909 0924 2822 2374 6f6f  ve"))....$("#too
-00000f60: 6c5f 7374 6174 7573 5f74 6162 6c65 2229  l_status_table")
-00000f70: 2e6c 6f61 6428 227b 2520 7572 6c20 2773  .load("{% url 's
-00000f80: 7461 7475 735f 6461 7368 626f 6172 6427  tatus_dashboard'
-00000f90: 2025 7d3f 696e 7465 7265 7374 3d74 6f6f   %}?interest=too
-00000fa0: 6c73 2229 3b0a 097d 0a0a 0966 756e 6374  ls");..}...funct
-00000fb0: 696f 6e20 666f 7263 655f 7573 6572 5f6f  ion force_user_o
-00000fc0: 7574 5f6f 665f 7468 655f 6172 6561 2875  ut_of_the_area(u
-00000fd0: 726c 290a 097b 0a20 2020 2020 2020 2069  rl)..{.        i
-00000fe0: 6620 2863 6f6e 6669 726d 2822 4172 6520  f (confirm("Are 
-00000ff0: 796f 7520 7375 7265 2079 6f75 2077 616e  you sure you wan
-00001000: 7420 746f 206c 6f67 2074 6869 7320 7573  t to log this us
-00001010: 6572 206f 7574 206f 6620 7468 6520 6172  er out of the ar
-00001020: 6561 3f22 2929 0a20 2020 2020 2020 207b  ea?")).        {
-00001030: 0a09 0920 2020 206c 6574 2066 6169 6c75  ...    let failu
-00001040: 7265 5f64 6961 6c6f 6720 3d20 616a 6178  re_dialog = ajax
-00001050: 5f66 6169 6c75 7265 5f63 616c 6c62 6163  _failure_callbac
-00001060: 6b28 2255 6e61 626c 6520 746f 2066 6f72  k("Unable to for
-00001070: 6365 2074 6865 2075 7365 7220 746f 206c  ce the user to l
-00001080: 6f67 206f 7574 206f 6620 7468 6520 6172  og out of the ar
-00001090: 6561 2229 3b0a 0909 2020 2020 616a 6178  ea");...    ajax
-000010a0: 5f70 6f73 7428 7572 6c2c 2075 6e64 6566  _post(url, undef
-000010b0: 696e 6564 2c20 756e 6465 6669 6e65 642c  ined, undefined,
-000010c0: 2066 6169 6c75 7265 5f64 6961 6c6f 672c   failure_dialog,
-000010d0: 2072 6566 7265 7368 5f73 7461 7475 735f   refresh_status_
-000010e0: 6461 7368 626f 6172 6429 3b0a 2020 2020  dashboard);.    
-000010f0: 2020 2020 7d0a 097d 0a0a 0966 756e 6374      }..}...funct
-00001100: 696f 6e20 666f 7263 655f 7573 6572 5f6f  ion force_user_o
-00001110: 6666 5f6f 665f 746f 6f6c 2875 726c 290a  ff_of_tool(url).
-00001120: 097b 0a20 2020 2020 2020 2069 6620 2863  .{.        if (c
-00001130: 6f6e 6669 726d 2822 4172 6520 796f 7520  onfirm("Are you 
-00001140: 7375 7265 2079 6f75 2077 616e 7420 746f  sure you want to
-00001150: 206c 6f67 2074 6869 7320 7573 6572 206f   log this user o
-00001160: 6666 206f 6620 7468 6520 746f 6f6c 3f22  ff of the tool?"
-00001170: 2929 0a20 2020 2020 2020 207b 0a20 2020  )).        {.   
-00001180: 2020 2020 2020 2020 206c 6574 2066 6169           let fai
-00001190: 6c75 7265 5f64 6961 6c6f 6720 3d20 616a  lure_dialog = aj
-000011a0: 6178 5f66 6169 6c75 7265 5f63 616c 6c62  ax_failure_callb
-000011b0: 6163 6b28 2255 6e61 626c 6520 746f 2066  ack("Unable to f
-000011c0: 6f72 6365 2075 7365 7220 6f66 6620 7468  orce user off th
-000011d0: 6520 746f 6f6c 2229 3b0a 2020 2020 2020  e tool");.      
-000011e0: 2020 2020 2020 6c65 7420 636f 6e74 656e        let conten
-000011f0: 7473 203d 207b 2273 7461 7465 223a 2022  ts = {"state": "
-00001200: 6469 7361 626c 6522 7d3b 0a20 2020 2020  disable"};.     
-00001210: 2020 2020 2020 2061 6a61 785f 706f 7374         ajax_post
-00001220: 2875 726c 2c20 636f 6e74 656e 7473 2c20  (url, contents, 
-00001230: 756e 6465 6669 6e65 642c 2066 6169 6c75  undefined, failu
-00001240: 7265 5f64 6961 6c6f 672c 2072 6566 7265  re_dialog, refre
-00001250: 7368 5f73 7461 7475 735f 6461 7368 626f  sh_status_dashbo
-00001260: 6172 6429 3b0a 2020 2020 2020 2020 7d0a  ard);.        }.
-00001270: 097d 0a0a 097b 2320 5468 6973 2066 756e  .}...{# This fun
-00001280: 6374 696f 6e20 6d6f 6469 6669 6573 2074  ction modifies t
-00001290: 6865 2063 6f6e 7465 6e74 7320 6f66 2061  he contents of a
-000012a0: 2073 7479 6c65 2073 6865 6574 2061 6674   style sheet aft
-000012b0: 6572 2074 6865 2070 6167 6520 6861 7320  er the page has 
-000012c0: 6265 656e 206c 6f61 6465 642e 2023 7d0a  been loaded. #}.
-000012d0: 0966 756e 6374 696f 6e20 7365 745f 7374  .function set_st
-000012e0: 796c 6528 6373 735f 7465 7874 290a 097b  yle(css_text)..{
-000012f0: 0a09 096c 6574 2073 6865 6574 203d 2064  ...let sheet = d
-00001300: 6f63 756d 656e 742e 6372 6561 7465 456c  ocument.createEl
-00001310: 656d 656e 7428 2773 7479 6c65 2729 3b0a  ement('style');.
-00001320: 0909 7368 6565 742e 7479 7065 203d 2027  ..sheet.type = '
-00001330: 7465 7874 2f63 7373 273b 0a09 0928 646f  text/css';...(do
-00001340: 6375 6d65 6e74 2e68 6561 6420 7c7c 2064  cument.head || d
-00001350: 6f63 756d 656e 742e 6765 7445 6c65 6d65  ocument.getEleme
-00001360: 6e74 7342 7954 6167 4e61 6d65 2827 6865  ntsByTagName('he
-00001370: 6164 2729 5b30 5d29 2e61 7070 656e 6443  ad')[0]).appendC
-00001380: 6869 6c64 2873 6865 6574 293b 0a09 0972  hild(sheet);...r
-00001390: 6574 7572 6e20 2873 6574 5f73 7479 6c65  eturn (set_style
-000013a0: 203d 2066 756e 6374 696f 6e28 6373 735f   = function(css_
-000013b0: 7465 7874 2c20 6e6f 6465 290a 0909 7b0a  text, node)...{.
-000013c0: 0909 0969 6628 216e 6f64 6520 7c7c 206e  ...if(!node || n
-000013d0: 6f64 652e 7061 7265 6e74 4e6f 6465 2021  ode.parentNode !
-000013e0: 3d3d 2073 6865 6574 290a 0909 0909 7265  == sheet).....re
-000013f0: 7475 726e 2073 6865 6574 2e61 7070 656e  turn sheet.appen
-00001400: 6443 6869 6c64 2864 6f63 756d 656e 742e  dChild(document.
-00001410: 6372 6561 7465 5465 7874 4e6f 6465 2863  createTextNode(c
-00001420: 7373 5f74 6578 7429 293b 0a09 0909 6e6f  ss_text));....no
-00001430: 6465 2e6e 6f64 6556 616c 7565 203d 2063  de.nodeValue = c
-00001440: 7373 5f74 6578 743b 0a09 0909 7265 7475  ss_text;....retu
-00001450: 726e 206e 6f64 653b 0a09 097d 2928 6373  rn node;...})(cs
-00001460: 735f 7465 7874 293b 0a09 7d0a 0a09 6675  s_text);..}...fu
-00001470: 6e63 7469 6f6e 2066 696c 7465 7228 7368  nction filter(sh
-00001480: 6f77 290a 097b 0a09 0924 2822 2366 696c  ow)..{...$("#fil
-00001490: 7465 7222 292e 6874 6d6c 2822 5368 6f77  ter").html("Show
-000014a0: 696e 6720 2220 2b20 7368 6f77 202b 2022  ing " + show + "
-000014b0: 203c 7370 616e 2063 6c61 7373 3d27 6361   <span class='ca
-000014c0: 7265 7427 3e3c 2f73 7061 6e3e 2229 3b0a  ret'></span>");.
-000014d0: 0909 6966 2873 686f 7720 3d3d 3d20 2261  ..if(show === "a
-000014e0: 6c6c 2074 6f6f 6c73 2229 0a09 0909 7365  ll tools")....se
-000014f0: 745f 7374 796c 6528 272e 696e 5f75 7365  t_style('.in_use
-00001500: 207b 2064 6973 706c 6179 3a20 7461 626c   { display: tabl
-00001510: 652d 726f 773b 207d 202e 6964 6c65 207b  e-row; } .idle {
-00001520: 2064 6973 706c 6179 3a20 7461 626c 652d   display: table-
-00001530: 726f 773b 207d 2729 3b0a 0909 656c 7365  row; }');...else
-00001540: 2069 6628 7368 6f77 203d 3d3d 2022 746f   if(show === "to
-00001550: 6f6c 7320 696e 2075 7365 2229 0a09 0909  ols in use")....
-00001560: 7365 745f 7374 796c 6528 272e 696e 5f75  set_style('.in_u
-00001570: 7365 207b 2064 6973 706c 6179 3a20 7461  se { display: ta
-00001580: 626c 652d 726f 773b 207d 202e 6964 6c65  ble-row; } .idle
-00001590: 207b 2064 6973 706c 6179 3a20 6e6f 6e65   { display: none
-000015a0: 3b20 7d27 293b 0a09 0965 6c73 6520 6966  ; }');...else if
-000015b0: 2873 686f 7720 3d3d 3d20 2270 726f 626c  (show === "probl
-000015c0: 656d 6174 6963 2074 6f6f 6c73 2229 0a09  ematic tools")..
-000015d0: 0909 7365 745f 7374 796c 6528 272e 7072  ..set_style('.pr
-000015e0: 6f62 6c65 6d61 7469 6320 7b20 6469 7370  oblematic { disp
-000015f0: 6c61 793a 2074 6162 6c65 2d72 6f77 207d  lay: table-row }
-00001600: 202e 6865 616c 7468 7920 7b20 6469 7370   .healthy { disp
-00001610: 6c61 793a 206e 6f6e 653b 207d 2729 3b0a  lay: none; }');.
-00001620: 0909 656c 7365 2069 6628 7368 6f77 203d  ..else if(show =
-00001630: 3d3d 2022 6964 6c65 2074 6f6f 6c73 2229  == "idle tools")
-00001640: 0a09 0909 7365 745f 7374 796c 6528 272e  ....set_style('.
-00001650: 6964 6c65 207b 2064 6973 706c 6179 3a20  idle { display: 
-00001660: 7461 626c 652d 726f 773b 207d 202e 696e  table-row; } .in
-00001670: 5f75 7365 207b 2064 6973 706c 6179 3a20  _use { display: 
-00001680: 6e6f 6e65 3b20 7d27 293b 0a09 7d0a 3c2f  none; }');..}.</
-00001690: 7363 7269 7074 3e0a 0a7b 2520 656e 6462  script>..{% endb
-000016a0: 6c6f 636b 2025 7d                        lock %}
+000003c0: 2069 643d 2273 7461 6666 5f6c 696e 6b22   id="staff_link"
+000003d0: 2068 7265 663d 2223 7374 6166 6622 3e53   href="#staff">S
+000003e0: 7461 6666 2073 7461 7475 733c 2f61 3e3c  taff status</a><
+000003f0: 2f6c 693e 7b25 2065 6e64 6966 2025 7d0a  /li>{% endif %}.
+00000400: 3c2f 756c 3e0a 0a3c 6469 7620 6964 3d22  </ul>..<div id="
+00000410: 636f 6e74 656e 7422 2063 6c61 7373 3d22  content" class="
+00000420: 7461 622d 636f 6e74 656e 7422 2073 7479  tab-content" sty
+00000430: 6c65 3d22 7061 6464 696e 672d 746f 703a  le="padding-top:
+00000440: 3130 7078 223e 0a09 3c64 6976 2063 6c61  10px">..<div cla
+00000450: 7373 3d22 7461 622d 7061 6e65 7b25 2069  ss="tab-pane{% i
+00000460: 6620 6172 6561 735f 6578 6973 7420 616e  f areas_exist an
+00000470: 6420 7461 6220 3d3d 2027 6f63 6375 7061  d tab == 'occupa
+00000480: 6e63 7927 2025 7d20 6163 7469 7665 7b25  ncy' %} active{%
+00000490: 2065 6e64 6966 2025 7d22 2069 643d 226f   endif %}" id="o
+000004a0: 6363 7570 616e 6379 223e 0a09 097b 2520  ccupancy">...{% 
+000004b0: 696e 636c 7564 6520 2773 7461 7475 735f  include 'status_
+000004c0: 6461 7368 626f 6172 642f 6f63 6375 7061  dashboard/occupa
+000004d0: 6e63 792e 6874 6d6c 2720 257d 0a09 3c2f  ncy.html' %}..</
+000004e0: 6469 763e 0a09 3c64 6976 2063 6c61 7373  div>..<div class
+000004f0: 3d22 7461 622d 7061 6e65 7b25 2069 6620  ="tab-pane{% if 
+00000500: 746f 6f6c 735f 6578 6973 7420 616e 6420  tools_exist and 
+00000510: 7461 6220 3d3d 2027 746f 6f6c 7327 2025  tab == 'tools' %
+00000520: 7d20 6163 7469 7665 7b25 2065 6e64 6966  } active{% endif
+00000530: 2025 7d20 696e 666f 2d74 6f6f 6c74 6970   %} info-tooltip
+00000540: 2d63 6f6e 7461 696e 6572 2220 6964 3d22  -container" id="
+00000550: 746f 6f6c 7322 3e0a 0909 3c64 6976 2063  tools">...<div c
+00000560: 6c61 7373 3d22 6274 6e2d 6772 6f75 7020  lass="btn-group 
+00000570: 7369 6465 6261 722d 6974 656d 223e 0a09  sidebar-item">..
+00000580: 0909 3c62 7574 746f 6e20 6964 3d22 6669  ..<button id="fi
+00000590: 6c74 6572 2220 7479 7065 3d22 6275 7474  lter" type="butt
+000005a0: 6f6e 2220 636c 6173 733d 2262 746e 2062  on" class="btn b
+000005b0: 746e 2d64 6566 6175 6c74 2064 726f 7064  tn-default dropd
+000005c0: 6f77 6e2d 746f 6767 6c65 2220 6461 7461  own-toggle" data
+000005d0: 2d74 6f67 676c 653d 2264 726f 7064 6f77  -toggle="dropdow
+000005e0: 6e22 207b 2520 6966 206e 6f5f 6865 6164  n" {% if no_head
+000005f0: 6572 2025 7d73 7479 6c65 3d22 6469 7370  er %}style="disp
+00000600: 6c61 793a 6e6f 6e65 3b22 7b25 2065 6e64  lay:none;"{% end
+00000610: 6966 2025 7d3e 0a09 0909 0953 686f 7769  if %}>.....Showi
+00000620: 6e67 2074 6f6f 6c73 2069 6e20 7573 650a  ng tools in use.
+00000630: 0909 0909 3c73 7061 6e20 636c 6173 733d  ....<span class=
+00000640: 2263 6172 6574 223e 3c2f 7370 616e 3e0a  "caret"></span>.
+00000650: 0909 093c 2f62 7574 746f 6e3e 0a09 0909  ...</button>....
+00000660: 3c75 6c20 636c 6173 733d 2264 726f 7064  <ul class="dropd
+00000670: 6f77 6e2d 6d65 6e75 223e 0a09 0909 093c  own-menu">.....<
+00000680: 6c69 2063 6c61 7373 3d22 6472 6f70 646f  li class="dropdo
+00000690: 776e 2d68 6561 6465 7222 3e46 696c 7465  wn-header">Filte
+000006a0: 7220 6279 2e2e 2e3c 2f6c 693e 0a09 0909  r by...</li>....
+000006b0: 093c 6c69 3e3c 6120 6872 6566 3d22 6a61  .<li><a href="ja
+000006c0: 7661 7363 7269 7074 3a76 6f69 6428 3029  vascript:void(0)
+000006d0: 2220 6f6e 636c 6963 6b3d 2266 696c 7465  " onclick="filte
+000006e0: 7228 2761 6c6c 2074 6f6f 6c73 2729 223e  r('all tools')">
+000006f0: 416c 6c20 746f 6f6c 733c 2f61 3e3c 2f6c  All tools</a></l
+00000700: 693e 0a09 0909 093c 6c69 3e3c 6120 6872  i>.....<li><a hr
+00000710: 6566 3d22 6a61 7661 7363 7269 7074 3a76  ef="javascript:v
+00000720: 6f69 6428 3029 2220 6f6e 636c 6963 6b3d  oid(0)" onclick=
+00000730: 2266 696c 7465 7228 2774 6f6f 6c73 2069  "filter('tools i
+00000740: 6e20 7573 6527 2922 3e54 6f6f 6c73 2069  n use')">Tools i
+00000750: 6e20 7573 653c 2f61 3e3c 2f6c 693e 0a09  n use</a></li>..
+00000760: 0909 093c 6c69 3e3c 6120 6872 6566 3d22  ...<li><a href="
+00000770: 6a61 7661 7363 7269 7074 3a76 6f69 6428  javascript:void(
+00000780: 3029 2220 6f6e 636c 6963 6b3d 2266 696c  0)" onclick="fil
+00000790: 7465 7228 2770 726f 626c 656d 6174 6963  ter('problematic
+000007a0: 2074 6f6f 6c73 2729 223e 5072 6f62 6c65   tools')">Proble
+000007b0: 6d61 7469 6320 746f 6f6c 733c 2f61 3e3c  matic tools</a><
+000007c0: 2f6c 693e 0a09 0909 093c 6c69 3e3c 6120  /li>.....<li><a 
+000007d0: 6872 6566 3d22 6a61 7661 7363 7269 7074  href="javascript
+000007e0: 3a76 6f69 6428 3029 2220 6f6e 636c 6963  :void(0)" onclic
+000007f0: 6b3d 2266 696c 7465 7228 2769 646c 6520  k="filter('idle 
+00000800: 746f 6f6c 7327 2922 3e49 646c 6520 746f  tools')">Idle to
+00000810: 6f6c 733c 2f61 3e3c 2f6c 693e 0a09 0909  ols</a></li>....
+00000820: 3c2f 756c 3e0a 0909 3c2f 6469 763e 0a09  </ul>...</div>..
+00000830: 093c 703e 0a09 093c 6469 7620 6964 3d22  .<p>...<div id="
+00000840: 746f 6f6c 5f73 7461 7475 735f 7461 626c  tool_status_tabl
+00000850: 6522 3e0a 0909 097b 2520 696e 636c 7564  e">....{% includ
+00000860: 6520 2773 7461 7475 735f 6461 7368 626f  e 'status_dashbo
+00000870: 6172 642f 746f 6f6c 732e 6874 6d6c 2720  ard/tools.html' 
+00000880: 257d 0a09 093c 2f64 6976 3e0a 093c 2f64  %}...</div>..</d
+00000890: 6976 3e0a 2020 2020 7b25 2069 6620 7368  iv>.    {% if sh
+000008a0: 6f77 5f73 7461 6666 5f73 7461 7475 7320  ow_staff_status 
+000008b0: 257d 0a20 2020 2020 2020 203c 6469 7620  %}.        <div 
+000008c0: 636c 6173 733d 2274 6162 2d70 616e 657b  class="tab-pane{
+000008d0: 2520 6966 2074 6162 203d 3d20 2773 7461  % if tab == 'sta
+000008e0: 6666 2720 257d 2061 6374 6976 657b 2520  ff' %} active{% 
+000008f0: 656e 6469 6620 257d 2220 6964 3d22 7374  endif %}" id="st
+00000900: 6166 6622 3e0a 2020 2020 2020 2020 2020  aff">.          
+00000910: 2020 7b25 2069 6e63 6c75 6465 2027 7374    {% include 'st
+00000920: 6174 7573 5f64 6173 6862 6f61 7264 2f73  atus_dashboard/s
+00000930: 7461 6666 2e68 746d 6c27 2025 7d0a 2020  taff.html' %}.  
+00000940: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+00000950: 207b 2520 656e 6469 6620 257d 0a3c 2f64   {% endif %}.</d
+00000960: 6976 3e0a 0a3c 7363 7269 7074 3e0a 2020  iv>..<script>.  
+00000970: 2020 6c65 7420 7374 6166 665f 7374 6174    let staff_stat
+00000980: 7573 5f70 6172 616d 6574 6572 7320 3d20  us_parameters = 
+00000990: 2274 696d 6573 7461 6d70 3d7b 7b20 7061  "timestamp={{ pa
+000009a0: 6765 5f74 696d 6573 7461 6d70 207d 7d26  ge_timestamp }}&
+000009b0: 7669 6577 3d7b 7b20 7061 6765 5f76 6965  view={{ page_vie
+000009c0: 7720 7d7d 223b 0a09 6675 6e63 7469 6f6e  w }}";..function
+000009d0: 206f 6e5f 6c6f 6164 2829 0a09 7b0a 2020   on_load()..{.  
+000009e0: 2020 2020 2020 7b23 206c 6f61 6420 6576        {# load ev
+000009f0: 6572 7974 6869 6e67 2061 7379 6e63 6872  erything asynchr
+00000a00: 6f6e 6f75 736c 792e 2065 7370 6563 6961  onously. especia
+00000a10: 6c6c 7920 746f 6f6c 7320 7461 6220 7369  lly tools tab si
+00000a20: 6e63 6520 6974 2074 616b 6573 2061 2062  nce it takes a b
+00000a30: 6974 206c 6f6e 6765 7220 746f 206c 6f61  it longer to loa
+00000a40: 6420 237d 0a20 2020 2020 2020 2024 2822  d #}.        $("
+00000a50: 2374 6f6f 6c5f 7374 6174 7573 5f74 6162  #tool_status_tab
+00000a60: 6c65 2229 2e6c 6f61 6428 227b 2520 7572  le").load("{% ur
+00000a70: 6c20 2773 7461 7475 735f 6461 7368 626f  l 'status_dashbo
+00000a80: 6172 6427 2025 7d3f 696e 7465 7265 7374  ard' %}?interest
+00000a90: 3d74 6f6f 6c73 222c 2068 6964 655f 7370  =tools", hide_sp
+00000aa0: 696e 6e65 7229 3b0a 2020 2020 2020 2020  inner);.        
+00000ab0: 7265 6672 6573 685f 7374 6166 665f 7374  refresh_staff_st
+00000ac0: 6174 7573 5f64 6173 6862 6f61 7264 2829  atus_dashboard()
+00000ad0: 3b0a 2020 2020 2020 2020 7265 6672 6573  ;.        refres
+00000ae0: 685f 7374 6174 7573 5f64 6173 6862 6f61  h_status_dashboa
+00000af0: 7264 2829 3b0a 0909 6669 6c74 6572 2827  rd();...filter('
+00000b00: 746f 6f6c 7320 696e 2075 7365 2729 3b0a  tools in use');.
+00000b10: 2020 2020 2020 2020 6c65 7420 7461 625f          let tab_
+00000b20: 6a71 203d 2024 2822 2374 6162 7320 6122  jq = $("#tabs a"
+00000b30: 293b 0a20 2020 2020 2020 2074 6162 5f6a  );.        tab_j
+00000b40: 712e 636c 6963 6b28 6675 6e63 7469 6f6e  q.click(function
+00000b50: 2028 2920 7b73 686f 775f 7370 696e 6e65   () {show_spinne
+00000b60: 7228 297d 293b 0a09 0974 6162 5f6a 712e  r()});...tab_jq.
+00000b70: 636c 6963 6b28 7377 6974 6368 5f74 6162  click(switch_tab
+00000b80: 293b 0a09 0974 6162 5f6a 712e 636c 6963  );...tab_jq.clic
+00000b90: 6b28 7265 6672 6573 685f 7374 6174 7573  k(refresh_status
+00000ba0: 5f64 6173 6862 6f61 7264 293b 0a09 0974  _dashboard);...t
+00000bb0: 6162 5f6a 712e 636c 6963 6b28 7570 6461  ab_jq.click(upda
+00000bc0: 7465 5f75 726c 293b 0a20 2020 2020 2020  te_url);.       
+00000bd0: 2024 2822 2373 7461 6666 5f6c 696e 6b22   $("#staff_link"
+00000be0: 292e 636c 6963 6b28 7265 6672 6573 685f  ).click(refresh_
+00000bf0: 7374 6166 665f 7374 6174 7573 5f64 6173  staff_status_das
+00000c00: 6862 6f61 7264 293b 0a09 0973 6574 5f69  hboard);...set_i
+00000c10: 6e74 6572 7661 6c5f 7768 656e 5f76 6973  nterval_when_vis
+00000c20: 6962 6c65 2864 6f63 756d 656e 742c 2072  ible(document, r
+00000c30: 6566 7265 7368 5f73 7461 7475 735f 6461  efresh_status_da
+00000c40: 7368 626f 6172 642c 2031 3030 3030 293b  shboard, 10000);
+00000c50: 0a20 2020 2020 2020 207b 2320 5365 7420  .        {# Set 
+00000c60: 6120 676c 6f62 616c 2063 6c69 636b 2068  a global click h
+00000c70: 616e 646c 6572 2074 6f20 6469 736d 6973  andler to dismis
+00000c80: 7320 6d61 6e75 616c 2074 6f6f 6c74 6970  s manual tooltip
+00000c90: 7320 237d 0a20 2020 2020 2020 2024 2827  s #}.        $('
+00000ca0: 6874 6d6c 2729 2e6f 6e28 2763 6c69 636b  html').on('click
+00000cb0: 272c 2066 756e 6374 696f 6e28 6529 0a20  ', function(e). 
+00000cc0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00000cd0: 2020 2020 207b 2320 4f6e 6c79 2064 696d       {# Only dim
+00000ce0: 6973 7320 746f 6f6c 7469 7073 2077 6865  iss tooltips whe
+00000cf0: 6e20 636c 6963 6b69 6e67 206f 7574 7369  n clicking outsi
+00000d00: 6465 206f 6620 7468 656d 2023 7d0a 2020  de of them #}.  
+00000d10: 2020 2020 2020 2020 2020 6c65 7420 7461            let ta
+00000d20: 7267 6574 5f69 6420 3d20 2428 652e 7461  rget_id = $(e.ta
+00000d30: 7267 6574 292e 7061 7265 6e74 7328 272e  rget).parents('.
+00000d40: 746f 6f6c 7469 7027 292e 6174 7472 2827  tooltip').attr('
+00000d50: 6964 2729 3b0a 2020 2020 2020 2020 2020  id');.          
+00000d60: 2020 6966 2028 7479 7065 6f66 2024 2865    if (typeof $(e
+00000d70: 2e74 6172 6765 7429 2e64 6174 6128 276f  .target).data('o
+00000d80: 7269 6769 6e61 6c2d 7469 746c 6527 2920  riginal-title') 
+00000d90: 3d3d 2027 756e 6465 6669 6e65 6427 290a  == 'undefined').
+00000da0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+00000db0: 2020 2020 2020 2020 2020 2020 2020 2428                $(
+00000dc0: 222e 746f 6f6c 7469 7022 292e 6e6f 7428  ".tooltip").not(
+00000dd0: 2723 272b 7461 7267 6574 5f69 6429 2e72  '#'+target_id).r
+00000de0: 656d 6f76 6528 293b 0a20 2020 2020 2020  emove();.       
+00000df0: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
+00000e00: 293b 0a09 7d0a 0924 286f 6e5f 6c6f 6164  );..}..$(on_load
+00000e10: 293b 0a0a 2020 2020 6675 6e63 7469 6f6e  );..    function
+00000e20: 2075 7064 6174 655f 7572 6c28 290a 2020   update_url().  
+00000e30: 2020 7b0a 2020 2020 2020 2020 7b23 2053    {.        {# S
+00000e40: 6574 2070 6572 6d61 6e65 6e74 2075 726c  et permanent url
+00000e50: 2073 6f20 7765 2063 616e 2072 6566 7265   so we can refre
+00000e60: 7368 2073 7065 6369 6669 6320 7461 6220  sh specific tab 
+00000e70: 237d 0a20 2020 2020 2020 206c 6574 2074  #}.        let t
+00000e80: 6974 6c65 203d 2022 4172 6561 206f 6363  itle = "Area occ
+00000e90: 7570 616e 6379 223b 0a20 2020 2020 2020  upancy";.       
+00000ea0: 206c 6574 206e 6577 5f75 726c 203d 2022   let new_url = "
+00000eb0: 7b25 2075 726c 2027 7374 6174 7573 5f64  {% url 'status_d
+00000ec0: 6173 6862 6f61 7264 5f74 6162 2720 276f  ashboard_tab' 'o
+00000ed0: 6363 7570 616e 6379 2720 257d 223b 0a20  ccupancy' %}";. 
+00000ee0: 2020 2020 2020 2069 6620 2824 2822 2374         if ($("#t
+00000ef0: 6f6f 6c73 2229 2e68 6173 436c 6173 7328  ools").hasClass(
+00000f00: 2261 6374 6976 6522 2929 0a20 2020 2020  "active")).     
+00000f10: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00000f20: 2074 6974 6c65 203d 2022 546f 6f6c 2073   title = "Tool s
+00000f30: 7461 7475 7322 3b0a 2020 2020 2020 2020  tatus";.        
+00000f40: 2020 2020 6e65 775f 7572 6c20 3d20 227b      new_url = "{
+00000f50: 2520 7572 6c20 2773 7461 7475 735f 6461  % url 'status_da
+00000f60: 7368 626f 6172 645f 7461 6227 2027 746f  shboard_tab' 'to
+00000f70: 6f6c 7327 2025 7d22 3b0a 2020 2020 2020  ols' %}";.      
+00000f80: 2020 7d0a 2020 2020 2020 2020 656c 7365    }.        else
+00000f90: 2069 6620 2824 2822 2373 7461 6666 2229   if ($("#staff")
+00000fa0: 2e68 6173 436c 6173 7328 2261 6374 6976  .hasClass("activ
+00000fb0: 6522 2929 0a20 2020 2020 2020 207b 0a20  e")).        {. 
+00000fc0: 2020 2020 2020 2020 2020 2074 6974 6c65             title
+00000fd0: 203d 2022 5374 6166 6620 7374 6174 7573   = "Staff status
+00000fe0: 223b 0a20 2020 2020 2020 2020 2020 206e  ";.            n
+00000ff0: 6577 5f75 726c 203d 2022 7b25 2075 726c  ew_url = "{% url
+00001000: 2027 7374 6174 7573 5f64 6173 6862 6f61   'status_dashboa
+00001010: 7264 5f74 6162 2720 2773 7461 6666 2720  rd_tab' 'staff' 
+00001020: 257d 3f22 202b 2073 7461 6666 5f73 7461  %}?" + staff_sta
+00001030: 7475 735f 7061 7261 6d65 7465 7273 3b0a  tus_parameters;.
+00001040: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00001050: 2020 6869 7374 6f72 792e 7075 7368 5374    history.pushSt
+00001060: 6174 6528 2727 2c20 7469 746c 652c 206e  ate('', title, n
+00001070: 6577 5f75 726c 293b 0a20 2020 207d 0a0a  ew_url);.    }..
+00001080: 0966 756e 6374 696f 6e20 7265 6672 6573  .function refres
+00001090: 685f 7374 6174 7573 5f64 6173 6862 6f61  h_status_dashboa
+000010a0: 7264 2829 0a09 7b0a 0909 6c65 7420 6f63  rd()..{...let oc
+000010b0: 6375 7061 6e63 795f 7461 6220 3d20 2428  cupancy_tab = $(
+000010c0: 2223 6f63 6375 7061 6e63 7922 293b 0a09  "#occupancy");..
+000010d0: 0969 6628 6f63 6375 7061 6e63 795f 7461  .if(occupancy_ta
+000010e0: 622e 6861 7343 6c61 7373 2822 6163 7469  b.hasClass("acti
+000010f0: 7665 2229 2920 6f63 6375 7061 6e63 795f  ve")) occupancy_
+00001100: 7461 622e 6c6f 6164 2822 7b25 2075 726c  tab.load("{% url
+00001110: 2027 7374 6174 7573 5f64 6173 6862 6f61   'status_dashboa
+00001120: 7264 2720 257d 3f69 6e74 6572 6573 743d  rd' %}?interest=
+00001130: 6f63 6375 7061 6e63 7922 2c20 6869 6465  occupancy", hide
+00001140: 5f73 7069 6e6e 6572 293b 0a09 0969 6628  _spinner);...if(
+00001150: 2428 2223 746f 6f6c 7322 292e 6861 7343  $("#tools").hasC
+00001160: 6c61 7373 2822 6163 7469 7665 2229 2920  lass("active")) 
+00001170: 2428 2223 746f 6f6c 5f73 7461 7475 735f  $("#tool_status_
+00001180: 7461 626c 6522 292e 6c6f 6164 2822 7b25  table").load("{%
+00001190: 2075 726c 2027 7374 6174 7573 5f64 6173   url 'status_das
+000011a0: 6862 6f61 7264 2720 257d 3f69 6e74 6572  hboard' %}?inter
+000011b0: 6573 743d 746f 6f6c 7322 2c20 6869 6465  est=tools", hide
+000011c0: 5f73 7069 6e6e 6572 293b 0a09 7d0a 0a20  _spinner);..}.. 
+000011d0: 2020 2066 756e 6374 696f 6e20 7265 6672     function refr
+000011e0: 6573 685f 7374 6166 665f 7374 6174 7573  esh_staff_status
+000011f0: 5f64 6173 6862 6f61 7264 2870 6172 616d  _dashboard(param
+00001200: 6574 6572 7329 0a20 2020 207b 0a20 2020  eters).    {.   
+00001210: 2020 2020 2069 6620 2870 6172 616d 6574       if (paramet
+00001220: 6572 7320 2626 2074 7970 656f 6620 7061  ers && typeof pa
+00001230: 7261 6d65 7465 7273 203d 3d3d 2027 7374  rameters === 'st
+00001240: 7269 6e67 2720 2920 7374 6166 665f 7374  ring' ) staff_st
+00001250: 6174 7573 5f70 6172 616d 6574 6572 7320  atus_parameters 
+00001260: 3d20 7061 7261 6d65 7465 7273 3b0a 2020  = parameters;.  
+00001270: 2020 2020 2020 2428 2223 7374 6166 6622        $("#staff"
+00001280: 292e 6c6f 6164 2822 7b25 2075 726c 2027  ).load("{% url '
+00001290: 7374 6174 7573 5f64 6173 6862 6f61 7264  status_dashboard
+000012a0: 2720 257d 3f69 6e74 6572 6573 743d 7374  ' %}?interest=st
+000012b0: 6166 6626 2220 2b20 7374 6166 665f 7374  aff&" + staff_st
+000012c0: 6174 7573 5f70 6172 616d 6574 6572 732c  atus_parameters,
+000012d0: 2068 6964 655f 7370 696e 6e65 7229 3b0a   hide_spinner);.
+000012e0: 2020 2020 2020 2020 7570 6461 7465 5f75          update_u
+000012f0: 726c 2829 3b0a 2020 2020 7d0a 0a09 6675  rl();.    }...fu
+00001300: 6e63 7469 6f6e 2066 6f72 6365 5f75 7365  nction force_use
+00001310: 725f 6f75 745f 6f66 5f74 6865 5f61 7265  r_out_of_the_are
+00001320: 6128 7572 6c29 0a09 7b0a 2020 2020 2020  a(url)..{.      
+00001330: 2020 6966 2028 636f 6e66 6972 6d28 2241    if (confirm("A
+00001340: 7265 2079 6f75 2073 7572 6520 796f 7520  re you sure you 
+00001350: 7761 6e74 2074 6f20 6c6f 6720 7468 6973  want to log this
+00001360: 2075 7365 7220 6f75 7420 6f66 2074 6865   user out of the
+00001370: 2061 7265 613f 2229 290a 2020 2020 2020   area?")).      
+00001380: 2020 7b0a 0909 2020 2020 6c65 7420 6661    {...    let fa
+00001390: 696c 7572 655f 6469 616c 6f67 203d 2061  ilure_dialog = a
+000013a0: 6a61 785f 6661 696c 7572 655f 6361 6c6c  jax_failure_call
+000013b0: 6261 636b 2822 556e 6162 6c65 2074 6f20  back("Unable to 
+000013c0: 666f 7263 6520 7468 6520 7573 6572 2074  force the user t
+000013d0: 6f20 6c6f 6720 6f75 7420 6f66 2074 6865  o log out of the
+000013e0: 2061 7265 6122 293b 0a09 0920 2020 2061   area");...    a
+000013f0: 6a61 785f 706f 7374 2875 726c 2c20 756e  jax_post(url, un
+00001400: 6465 6669 6e65 642c 2075 6e64 6566 696e  defined, undefin
+00001410: 6564 2c20 6661 696c 7572 655f 6469 616c  ed, failure_dial
+00001420: 6f67 2c20 7265 6672 6573 685f 7374 6174  og, refresh_stat
+00001430: 7573 5f64 6173 6862 6f61 7264 293b 0a20  us_dashboard);. 
+00001440: 2020 2020 2020 207d 0a09 7d0a 0a09 6675         }..}...fu
+00001450: 6e63 7469 6f6e 2066 6f72 6365 5f75 7365  nction force_use
+00001460: 725f 6f66 665f 6f66 5f74 6f6f 6c28 7572  r_off_of_tool(ur
+00001470: 6c29 0a09 7b0a 2020 2020 2020 2020 6966  l)..{.        if
+00001480: 2028 636f 6e66 6972 6d28 2241 7265 2079   (confirm("Are y
+00001490: 6f75 2073 7572 6520 796f 7520 7761 6e74  ou sure you want
+000014a0: 2074 6f20 6c6f 6720 7468 6973 2075 7365   to log this use
+000014b0: 7220 6f66 6620 6f66 2074 6865 2074 6f6f  r off of the too
+000014c0: 6c3f 2229 290a 2020 2020 2020 2020 7b0a  l?")).        {.
+000014d0: 2020 2020 2020 2020 2020 2020 6c65 7420              let 
+000014e0: 6661 696c 7572 655f 6469 616c 6f67 203d  failure_dialog =
+000014f0: 2061 6a61 785f 6661 696c 7572 655f 6361   ajax_failure_ca
+00001500: 6c6c 6261 636b 2822 556e 6162 6c65 2074  llback("Unable t
+00001510: 6f20 666f 7263 6520 7573 6572 206f 6666  o force user off
+00001520: 2074 6865 2074 6f6f 6c22 293b 0a20 2020   the tool");.   
+00001530: 2020 2020 2020 2020 206c 6574 2063 6f6e           let con
+00001540: 7465 6e74 7320 3d20 7b22 7374 6174 6522  tents = {"state"
+00001550: 3a20 2264 6973 6162 6c65 227d 3b0a 2020  : "disable"};.  
+00001560: 2020 2020 2020 2020 2020 616a 6178 5f70            ajax_p
+00001570: 6f73 7428 7572 6c2c 2063 6f6e 7465 6e74  ost(url, content
+00001580: 732c 2075 6e64 6566 696e 6564 2c20 6661  s, undefined, fa
+00001590: 696c 7572 655f 6469 616c 6f67 2c20 7265  ilure_dialog, re
+000015a0: 6672 6573 685f 7374 6174 7573 5f64 6173  fresh_status_das
+000015b0: 6862 6f61 7264 293b 0a20 2020 2020 2020  hboard);.       
+000015c0: 207d 0a09 7d0a 0a09 7b23 2054 6869 7320   }..}...{# This 
+000015d0: 6675 6e63 7469 6f6e 206d 6f64 6966 6965  function modifie
+000015e0: 7320 7468 6520 636f 6e74 656e 7473 206f  s the contents o
+000015f0: 6620 6120 7374 796c 6520 7368 6565 7420  f a style sheet 
+00001600: 6166 7465 7220 7468 6520 7061 6765 2068  after the page h
+00001610: 6173 2062 6565 6e20 6c6f 6164 6564 2e20  as been loaded. 
+00001620: 237d 0a09 6675 6e63 7469 6f6e 2073 6574  #}..function set
+00001630: 5f73 7479 6c65 2863 7373 5f74 6578 7429  _style(css_text)
+00001640: 0a09 7b0a 0909 6c65 7420 7368 6565 7420  ..{...let sheet 
+00001650: 3d20 646f 6375 6d65 6e74 2e63 7265 6174  = document.creat
+00001660: 6545 6c65 6d65 6e74 2827 7374 796c 6527  eElement('style'
+00001670: 293b 0a09 0973 6865 6574 2e74 7970 6520  );...sheet.type 
+00001680: 3d20 2774 6578 742f 6373 7327 3b0a 0909  = 'text/css';...
+00001690: 2864 6f63 756d 656e 742e 6865 6164 207c  (document.head |
+000016a0: 7c20 646f 6375 6d65 6e74 2e67 6574 456c  | document.getEl
+000016b0: 656d 656e 7473 4279 5461 674e 616d 6528  ementsByTagName(
+000016c0: 2768 6561 6427 295b 305d 292e 6170 7065  'head')[0]).appe
+000016d0: 6e64 4368 696c 6428 7368 6565 7429 3b0a  ndChild(sheet);.
+000016e0: 0909 7265 7475 726e 2028 7365 745f 7374  ..return (set_st
+000016f0: 796c 6520 3d20 6675 6e63 7469 6f6e 2863  yle = function(c
+00001700: 7373 5f74 6578 742c 206e 6f64 6529 0a09  ss_text, node)..
+00001710: 097b 0a09 0909 6966 2821 6e6f 6465 207c  .{....if(!node |
+00001720: 7c20 6e6f 6465 2e70 6172 656e 744e 6f64  | node.parentNod
+00001730: 6520 213d 3d20 7368 6565 7429 0a09 0909  e !== sheet)....
+00001740: 0972 6574 7572 6e20 7368 6565 742e 6170  .return sheet.ap
+00001750: 7065 6e64 4368 696c 6428 646f 6375 6d65  pendChild(docume
+00001760: 6e74 2e63 7265 6174 6554 6578 744e 6f64  nt.createTextNod
+00001770: 6528 6373 735f 7465 7874 2929 3b0a 0909  e(css_text));...
+00001780: 096e 6f64 652e 6e6f 6465 5661 6c75 6520  .node.nodeValue 
+00001790: 3d20 6373 735f 7465 7874 3b0a 0909 0972  = css_text;....r
+000017a0: 6574 7572 6e20 6e6f 6465 3b0a 0909 7d29  eturn node;...})
+000017b0: 2863 7373 5f74 6578 7429 3b0a 097d 0a0a  (css_text);..}..
+000017c0: 0966 756e 6374 696f 6e20 6669 6c74 6572  .function filter
+000017d0: 2873 686f 7729 0a09 7b0a 0909 2428 2223  (show)..{...$("#
+000017e0: 6669 6c74 6572 2229 2e68 746d 6c28 2253  filter").html("S
+000017f0: 686f 7769 6e67 2022 202b 2073 686f 7720  howing " + show 
+00001800: 2b20 2220 3c73 7061 6e20 636c 6173 733d  + " <span class=
+00001810: 2763 6172 6574 273e 3c2f 7370 616e 3e22  'caret'></span>"
+00001820: 293b 0a09 0969 6628 7368 6f77 203d 3d3d  );...if(show ===
+00001830: 2022 616c 6c20 746f 6f6c 7322 290a 0909   "all tools")...
+00001840: 0973 6574 5f73 7479 6c65 2827 2e69 6e5f  .set_style('.in_
+00001850: 7573 6520 7b20 6469 7370 6c61 793a 2074  use { display: t
+00001860: 6162 6c65 2d72 6f77 3b20 7d20 2e69 646c  able-row; } .idl
+00001870: 6520 7b20 6469 7370 6c61 793a 2074 6162  e { display: tab
+00001880: 6c65 2d72 6f77 3b20 7d27 293b 0a09 0965  le-row; }');...e
+00001890: 6c73 6520 6966 2873 686f 7720 3d3d 3d20  lse if(show === 
+000018a0: 2274 6f6f 6c73 2069 6e20 7573 6522 290a  "tools in use").
+000018b0: 0909 0973 6574 5f73 7479 6c65 2827 2e69  ...set_style('.i
+000018c0: 6e5f 7573 6520 7b20 6469 7370 6c61 793a  n_use { display:
+000018d0: 2074 6162 6c65 2d72 6f77 3b20 7d20 2e69   table-row; } .i
+000018e0: 646c 6520 7b20 6469 7370 6c61 793a 206e  dle { display: n
+000018f0: 6f6e 653b 207d 2729 3b0a 0909 656c 7365  one; }');...else
+00001900: 2069 6628 7368 6f77 203d 3d3d 2022 7072   if(show === "pr
+00001910: 6f62 6c65 6d61 7469 6320 746f 6f6c 7322  oblematic tools"
+00001920: 290a 0909 0973 6574 5f73 7479 6c65 2827  )....set_style('
+00001930: 2e70 726f 626c 656d 6174 6963 207b 2064  .problematic { d
+00001940: 6973 706c 6179 3a20 7461 626c 652d 726f  isplay: table-ro
+00001950: 7720 7d20 2e68 6561 6c74 6879 207b 2064  w } .healthy { d
+00001960: 6973 706c 6179 3a20 6e6f 6e65 3b20 7d27  isplay: none; }'
+00001970: 293b 0a09 0965 6c73 6520 6966 2873 686f  );...else if(sho
+00001980: 7720 3d3d 3d20 2269 646c 6520 746f 6f6c  w === "idle tool
+00001990: 7322 290a 0909 0973 6574 5f73 7479 6c65  s")....set_style
+000019a0: 2827 2e69 646c 6520 7b20 6469 7370 6c61  ('.idle { displa
+000019b0: 793a 2074 6162 6c65 2d72 6f77 3b20 7d20  y: table-row; } 
+000019c0: 2e69 6e5f 7573 6520 7b20 6469 7370 6c61  .in_use { displa
+000019d0: 793a 206e 6f6e 653b 207d 2729 3b0a 097d  y: none; }');..}
+000019e0: 0a3c 2f73 6372 6970 743e 0a0a 7b25 2065  .</script>..{% e
+000019f0: 6e64 626c 6f63 6b20 257d                 ndblock %}
```

### Comparing `NEMO-4.5.5/NEMO/templates/status_dashboard/tools.html` & `NEMO-4.6.0/NEMO/templates/status_dashboard/tools.html`

 * *Files 5% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 					{% if user.is_staff or user.is_user_office %}
 						<span class="glyphicon glyphicon-remove-circle grey pointer" onclick="force_user_off_of_tool('{% url 'disable_tool' tool.id %}')" title="Force {{ tool.operator }} to stop using the {{ tool.name }}"></span>
 					{% endif %}
 					{{ tool.user }}
 				</td>
 				<td>{{ tool.in_use_since|date:"l @ "}} {{ tool.in_use_since|time }}</td>
 			{% else %}
-				<td></td>
-				<td></td>
+				<td aria-label="No user"></td>
+				<td aria-label="Not in use"></td>
 			{% endif %}
 		</tr>
 	{% endfor %}
 	</tbody>
 </table>
 <script>
     $(".tool-info-tooltip").on('click', function () {
```

### Comparing `NEMO-4.5.5/NEMO/templates/tasks/resolve.html` & `NEMO-4.6.0/NEMO/templates/tasks/resolve.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/tasks/update.html` & `NEMO-4.6.0/NEMO/templates/tasks/update.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/tool_control/get_projects.html` & `NEMO-4.6.0/NEMO/templates/tool_control/get_projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/tool_control/interlock_error.html` & `NEMO-4.6.0/NEMO/templates/tool_control/interlock_error.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <div>
     <h1 class="text-center">
         <span style="font-size: xx-large;margin-right:10px;" class="glyphicon glyphicon-exclamation-sign danger-highlight"></span>
         Interlock error
     </h1>
-    <h3 class="interlock_message text-center"></h3>
+    <h3 class="interlock_message text-center" aria-label="Interlock message"></h3>
 
     <div class="modal-footer" style="text-align: center">
-        <button type="button" class="inter_bypass btn btn-success" style="display: none;">
+        <button type="button" class="inter_bypass btn btn-success" style="display: none;" aria-label="Bypass button">
             <span class="bypass_text"></span>
         </button>
         <button type="button" class="inter_try_again btn btn-primary">Try again</button>
         <button type="button" class="btn btn-warning" onclick="$('#dialog').modal('hide')">Cancel</button>
     </div>
 </div>
```

### Comparing `NEMO-4.5.5/NEMO/templates/tool_control/past_tasks_and_comments.html` & `NEMO-4.6.0/NEMO/templates/tool_control/past_tasks_and_comments.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/tool_control/qualified_users.html` & `NEMO-4.6.0/NEMO/templates/tool_control/qualified_users.html`

 * *Files 5% similar despite different names*

```diff
@@ -16,22 +16,20 @@
 			<input type="hidden" name="chosen_tool[]" value="{{ tool.id }}">
 			<input type="hidden" name="action" value="qualify">
 		</form>
 		{% with tool.user_set.all as qualified_users %}
 			{% if qualified_users %}
 				<p>You can email <a href="{% url 'compose_email' %}?audience=tool&selection={{ tool.id }}"><span class="glyphicon glyphicon-send"></span> all qualified users</a>.</p>
 				<p>
-					Current qualified users are listed below. Inactive qualified users are marked in <span class="light-grey">light grey</span>.<br>
+					Current qualified users are listed below. Inactive qualified users are <span class="strikethrough light-grey">crossed out</span>.<br>
 					{% for u in qualified_users %}
 						{% if u.is_active %}
 							<a href="javascript:remove_qualified_user('{{ u.id }}', '{{ tool.id }}')" class="grey hover-black" title="Disqualify {{ u.first_name }}"><span class="glyphicon glyphicon-remove-circle"></span></a> {{ u }}
 						{% else %}
-							<span class="light-grey">
-									<a href="javascript:remove_qualified_user('{{ u.id }}', '{{ tool.id }}')" class="light-grey hover-black" title="Disqualify {{ u.first_name }}"><span class="glyphicon glyphicon-remove-circle"></span></a> {{ u }}
-								</span>
+							<a href="javascript:remove_qualified_user('{{ u.id }}', '{{ tool.id }}')" class="grey hover-black" title="Disqualify {{ u.first_name }}"><span class="glyphicon glyphicon-remove-circle"></span></a> <span class="strikethrough light-grey">{{ u }}</span>
 						{% endif %}
 						<br>
 					{% endfor %}
 				</p>
 			{% endif %}
 		{% endwith %}
 	</div>
```

#### html2text {}

```diff
@@ -5,13 +5,13 @@
 Qualifying a user for this tool automatically grants them the physical access
 level "{{ tool.grant_physical_access_level_upon_qualification }}".
 {% endif %}
 Add a qualified user [                    ]
 
 {% with tool.user_set.all as qualified_users %} {% if qualified_users %}
 You can email all_qualified_users.
-Current qualified users are listed below. Inactive qualified users are marked
-in light grey.
-{% for u in qualified_users %} {% if u.is_active %}  {{ u }} {% else %}   {{ u
-}}  {% endif %}
+Current qualified users are listed below. Inactive qualified users are crossed
+out.
+{% for u in qualified_users %} {% if u.is_active %}  {{ u }} {% else %}  {{ u
+}} {% endif %}
 {% endfor %}
 {% endif %} {% endwith %}
```

### Comparing `NEMO-4.5.5/NEMO/templates/tool_control/tool_control.html` & `NEMO-4.6.0/NEMO/templates/tool_control/tool_control.html`

 * *Files 8% similar despite different names*

```diff
@@ -3,37 +3,35 @@
 {% block title %}Tool control{% endblock %}
 {% block extrahead %}
 	{% load static %}
 	<script type="text/javascript" src="{% static "datetimepicker/bootstrap-datetimepicker.js" %}"></script>
 	<link rel="stylesheet" type="text/css" href="{% static "datetimepicker/bootstrap-datetimepicker.css" %}"/>
 {% endblock %}
 {% block body %}
-
+<div id="main-content">
 	<style>
 		h3
 		{
 			margin-top: 0;
 		}
 	</style>
 
 	{% if device == 'mobile' %}
 		<div id="content" class="container"></div>
 	{% else %}
 		<div id="sidebar" class="application-sidebar">
 			<div id="expand-collapse" class="btn-group sidebar-item">
                 {% if calendar_qualified_tools and not user.is_staff %}
-                    <button type="button" class="btn btn-default" style="width:33%" onclick="expand_all_categories()" title="Expand all categories"><span class="glyphicon glyphicon glyphicon-resize-full"></span></button>
-                    <button type="button" class="btn btn-default" style="width:33%" onclick="collapse_all_categories()" title="Collapse all categories"><span class="glyphicon glyphicon glyphicon-resize-small"></span></button>
-                    <button type="button" class="btn btn-default" id="qualified_tools_btn" style="width:34%" onclick="toggle_qualified_tools(retrieve_user_qualifications())" title="Only show qualified tools"><span class="glyphicon glyphicon-check"></span></button>
+                    <button type="button" class="btn btn-default" style="width:50%" onclick="toggle_categories()" title="Expand/collapse all categories"><span id="expand_collapse_icon" class="glyphicon glyphicon"></span></button>
+                    <button type="button" class="btn btn-default" id="qualified_tools_btn" style="width:50%" onclick="toggle_qualified_tools(retrieve_user_qualifications())" title="Only show qualified tools"><span class="glyphicon glyphicon-check"></span></button>
                 {% else %}
-                    <button type="button" class="btn btn-default" style="width:50%" onclick="expand_all_categories()" title="Expand all categories"><span class="glyphicon glyphicon glyphicon-resize-full"></span></button>
-                    <button type="button" class="btn btn-default" style="width:50%" onclick="collapse_all_categories()" title="Collapse all categories"><span class="glyphicon glyphicon glyphicon-resize-small"></span></button>
+                    <button type="button" class="btn btn-default" style="width:100%" onclick="toggle_categories()" title="Expand/collapse all categories"><span id="expand_collapse_icon" class="glyphicon glyphicon"></span></button>
                 {% endif %}
 			</div>
-			<input type="text" id="item_search" placeholder="Search for a tool" class="form-control sidebar-item">
+			<input aria-label="Search for a tool" type="search" id="item_search" placeholder="Search for a tool" class="form-control sidebar-item">
 			{{ rendered_item_tree_html }}
 			<div style="height:50px"></div>
 		</div>
 		<div id="content" class="application-content" style="padding-right: 20px; overflow-y:scroll"></div>
 		<div id="loading-div" class="application-content spinner-container" style="display: none">
 			<div class="glyphicon glyphicon-repeat normal-right-spinner"></div>
 		</div>
@@ -182,19 +180,20 @@
 			else
 				success_callbacks = [refresh_tool_status, ajax_success_callback];
 			let enable_start_button = function() { $("#start button").prop("disabled", false); };
             let data = "remote_work=" + $("#remote_work").val();
 			try_post_catch_interlock_error(url, data, success_callbacks, enable_start_button);
 		}
 
-		function disable_tool(url)
+		function disable_tool(url, shorten)
 		{
-			$("#stop").prop("disabled", true);
+			$("#stop_wrapper button").prop("disabled", true);
 			let data = $("#tool_control").serialize();
-			let enable_stop_button = function() { $("#stop").prop("disabled", false); };
+            if (shorten !== undefined && shorten) data += '&shorten=True';
+			let enable_stop_button = function() { $("#stop_wrapper button").prop("disabled", false); };
 			try_post_catch_interlock_error(url, data, [refresh_tool_status, ajax_success_callback], enable_stop_button);
 		}
 
 		{% if user.is_staff %}
 
 			{# Only staff can perform the functions in this if-block. #}
 
@@ -352,9 +351,9 @@
 			{% endif %}
 			refresh_tool_status();
 		}
 
 		$(on_load);
 
 	</script>
-
+</div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% extends 'base.html' %} {% load custom_tags_and_filters %} {% block title
 %}Tool control{% endblock %} {% block extrahead %} {% load static %}
 ootstrap-datetimepicker.js" %}">
 ootstrap-datetimepicker.css" %}"/> {% endblock %} {% block body %}
  {% if device == 'mobile' %}
 {% else %}
-{% if calendar_qualified_tools and not user.is_staff %}    {% else %}   {%
-endif %}
-[                    ] {{ rendered_item_tree_html }}
+{% if calendar_qualified_tools and not user.is_staff %}   {% else %}  {% endif
+%}
+[Unknown INPUT type] {{ rendered_item_tree_html }}
 {% endif %}
 {% include 'tool_control/interlock_error.html' %}
- {% endblock %}
+{% endblock %}
```

### Comparing `NEMO-4.5.5/NEMO/templates/tool_control/tool_status.html` & `NEMO-4.6.0/NEMO/templates/tool_control/tool_status.html`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 							{% if current_usage_event.operator.id != current_usage_event.user.id %}
 								on behalf of {{ current_usage_event.user }}
 							{% endif %}
 							for the project named {{ current_usage_event.project.name }} since {{ current_usage_event.start|date:"l @ " }}{{ current_usage_event.start|time }}.
 						</h2>
 					{% endwith %}
 				</div>
-				{% if time_left %}
+				{% if time_left and not user.is_staff %}
 					<div>
 						Your reservation for this tool will end at {{ time_left|time }}. The remainder of your reservation will be relinquished when you stop using this tool.
 					</div>
 				{% endif %}
 			{% elif tool.delayed_logoff_in_progress %}
 				{% with tool.get_delayed_logoff_usage_event as delayed_logoff_event %}
 					<div class="primary-highlight">
@@ -292,47 +292,55 @@
 					{{ post_usage_questions }}
 					{% if tool.allow_delayed_logoff and not tool.delayed_logoff_in_progress %}
 						<div class="form-group">
 							Prevent others from using the tool for <input type="number" id="downtime" name="downtime" aria-label="Downtime" class="form-control" style="display:inline; width:auto" min="5" max="120" inputmode="numeric" pattern="[0-9]*" placeholder="0"> minutes after disabling the tool.
 							<a id="delayed_logoff_help" class="pointer" tabindex="0" data-toggle="popover" data-placement="bottom" data-trigger="focus" data-content="Some tools may require downtime after you finish using them. (For example, to perform automated cleaning or pump-down). Once you click &quot;Stop using the {{ tool.name_or_child_in_use_name }}&quot; the tool interlock will immediately disable the tool and it will remain unusable for the specified duration. Leave the duration blank to indicate that no post-usage downtime is required.">What's this?</a>
 						</div>
 					{% endif %}
-					<div id="stop_wrapper" style="display:inline-block" data-toggle="tooltip" data-placement="bottom" title="Please answer the required questions (above) to proceed">
-                        {% url 'disable_tool' tool.get_current_usage_event.tool.id as disable_tool_url %}
-                        {% button type="delete" id="stop" icon="glyphicon-stop" onclick="disable_tool('"|concat:disable_tool_url|concat:"'); return false;" value="Stop using the "|concat:tool.name_or_child_in_use_name %}
+					<div id="stop_wrapper">
+                        <div style="display:inline-block" data-toggle="tooltip" data-placement="bottom" title="Please answer the required questions (above) to proceed">
+                            {% url 'disable_tool' tool.get_current_usage_event.tool.id as disable_tool_url %}
+                            {% button type="delete" id="stop" icon="glyphicon-stop" onclick="disable_tool('"|concat:disable_tool_url|concat:"'); return false;" value="Stop using the "|concat:tool.name_or_child_in_use_name %}
+                        </div>
+                        {% if time_left and user.is_staff %}
+                            <div style="display:inline-block" data-toggle="tooltip" data-placement="bottom" title="Please answer the required questions (above) to proceed">
+                                {% url 'disable_tool' tool.get_current_usage_event.tool.id as disable_tool_url %}
+                                {% with left_until=time_left|timeuntil %}
+                                    {% button type="delete" id="stop" icon="glyphicon-stop" onclick="disable_tool('"|concat:disable_tool_url|concat:"', true); return false;" value="Stop using the "|concat:tool.name_or_child_in_use_name|concat:" and relinquish the remaining "|concat:left_until|concat:" of your reservation" %}
+                                {% endwith %}
+                            </div>
+                        {% endif %}
                     </div>
 				{% endif %}
 			{% else %}
 				{% if user.is_staff or user.is_service_personnel and tool in user.qualifications.all %}
-					<h4>What would you like to do?</h4>
+					<h4 id="what_to_do_label">What would you like to do?</h4>
                     <input type="hidden" id="remote_work" name="remote_work" value="">
-					<div class="radio"><label><input type="radio" onchange="use_tool_for_self()" name="staff_charge" value="false">Use this tool for my own project</label></div>
-					{% if user.is_staff %}
-						<div class="radio"><label><input type="radio" onchange="use_tool_for_other()" name="staff_charge" value="false">Use this tool on behalf of another user{% if "remote_work"|customization:"remote_work_ask_explicitly" %} (no remote){% endif %}</label></div>
-                        {% if "remote_work"|customization:"remote_work_ask_explicitly" %}
-						    <div class="radio">
-                                <label><input type="radio" onchange="use_tool_for_other(true)" name="staff_charge" value="false">Use this tool for a remote project</label>
-                            </div>
+					<div class="radio" role="group" aria-labelledby="what_to_do_label">
+                        <label><input type="radio" onchange="use_tool_for_self()" name="staff_charge" value="false">Use this tool for my own project</label>
+                        {% if user.is_staff %}
+                            <br><label><input type="radio" onchange="use_tool_for_other()" name="staff_charge" value="false">Use this tool on behalf of another user{% if "remote_work"|customization:"remote_work_ask_explicitly" %} (no remote){% endif %}</label>
+                            {% if "remote_work"|customization:"remote_work_ask_explicitly" %}
+                                <br><label><input type="radio" onchange="use_tool_for_other(true)" name="staff_charge" value="false">Use this tool for a remote project</label>
+                            {% endif %}
+                            {% if user.charging_staff_time %}
+                                {% with user.get_staff_charge as staff_charge %}
+                                    <br><label id="staff_charge_tooltip_container" class="strikethrough light-grey" data-toggle="tooltip" data-placement="right" title="This option is not available because you are already charging staff time to {{ staff_charge.customer }} for the project named {{ staff_charge.project }} since {{ staff_charge.start }}.">
+                                        <input type="radio" onchange="use_tool_for_other()" disabled>
+                                        <span id="staff_charge_tooltip_location">Use this tool for a remote project{% if "remote_work"|customization:"remote_work_ask_explicitly" %} (charge staff time{% if tool.requires_area_access and "remote_work"|customization:"remote_work_start_area_access_automatically" == "enabled" %} & {{ tool.requires_area_access }} time{% endif %}){% endif %}</span>
+                                    </label>
+                                    <script>
+                                        $("#staff_charge_tooltip_container").tooltip();
+                                    </script>
+                                {% endwith %}
+                            {% else %}
+                                <br><label><input type="radio" onchange="use_tool_for_other()" name="staff_charge" value="true">Use this tool for a remote project{% if "remote_work"|customization:"remote_work_ask_explicitly" %} (charge staff time{% if tool.requires_area_access and "remote_work"|customization:"remote_work_start_area_access_automatically" == "enabled" %} & {{ tool.requires_area_access }} time{% endif %}){% endif %}</label>
+                            {% endif %}
                         {% endif %}
-						{% if user.charging_staff_time %}
-							{% with user.get_staff_charge as staff_charge %}
-								<div class="radio disabled">
-									<label id="staff_charge_tooltip_container" class="light-grey" data-toggle="tooltip" data-placement="right" title="This option is not available because you are already charging staff time to {{ staff_charge.customer }} for the project named {{ staff_charge.project }} since {{ staff_charge.start }}.">
-										<input type="radio" onchange="use_tool_for_other()" disabled>
-										<span id="staff_charge_tooltip_location">Use this tool for a remote project{% if "remote_work"|customization:"remote_work_ask_explicitly" %} (charge staff time{% if tool.requires_area_access and "remote_work"|customization:"remote_work_start_area_access_automatically" == "enabled" %} & {{ tool.requires_area_access }} time{% endif %}){% endif %}</span>
-									</label>
-								</div>
-								<script>
-									$("#staff_charge_tooltip_container").tooltip();
-								</script>
-							{% endwith %}
-						{% else %}
-							<div class="radio"><label><input type="radio" onchange="use_tool_for_other()" name="staff_charge" value="true">Use this tool for a remote project{% if "remote_work"|customization:"remote_work_ask_explicitly" %} (charge staff time{% if tool.requires_area_access and "remote_work"|customization:"remote_work_start_area_access_automatically" == "enabled" %} & {{ tool.requires_area_access }} time{% endif %}){% endif %}</label></div>
-						{% endif %}
-					{% endif %}
+                    </div>
 					<div id="project_choice"></div>
 				{% elif tool.operational and not tool.required_resource_is_unavailable and not tool.delayed_logoff_in_progress and not tool.scheduled_outage_in_progress %}
 					{% include 'tool_control/get_projects.html' with active_projects=user.active_projects user_id=user.id %}
 				{% endif %}
 				{% if user.is_staff or user.is_service_personnel and tool in user.qualifications.all or tool.ready_to_use %}
 					<div id="start" style="display:none">
 						{% if tool.is_parent_tool %}
@@ -351,15 +359,15 @@
 		</form>
 
         <div style="height:15px">{# Spacer #}</div>
 
         {% if messages %}
             {% for message in messages %}
                 <div class="alert alert-{{ message.level_tag }} alert-dismissible show-on-load" {% if message.extra_tags %}{{ message.extra_tags }}{% endif %} style="display: none">
-                    <button type="button" class="close" data-dismiss="alert">&times;</button>
+                    <button type="button" class="close" data-dismiss="alert" aria-label="Modal close button">&times;</button>
                     {{message}}
                 </div>
             {% endfor %}
         {% endif %}
 		
 		{% if tool.description or tool.image or tool.tool_documents %}
 			<div style="background-color: #f5f5f5;">
@@ -602,15 +610,15 @@
 				</div>
 			{% endif %}
 			<div class="form-group">
 				<div class="checkbox"><label><input name="safety_hazard" type="checkbox"/>This problem represents a safety hazard to the {{ facility_name }} and should be regarded as urgent. Notify the {{ facility_name }} safety officer of this issue.</label></div>
 				<div class="checkbox"><label><input name="force_shutdown" type="checkbox"/>Shut down the tool so that it may not be used until this problem is resolved.</label></div>
 			</div>
 			<div class="form-group">
-				<input id="fileupload" type="file" name="image" multiple>
+				<input aria-label="File upload" id="fileupload" type="file" name="image" multiple>
 			</div>
 			<div class="form-group">
                 {% button type="delete" submit=True icon="glyphicon-send" value="Report problem" %}
 			</div>
 		</form>
 		<div style="height:150px">{# Spacer #}</div>
 	</div>
@@ -635,16 +643,16 @@
 						<option value="60">60 days</option>
 						<option value="90">90 days</option>
 						<option value="0">Indefinitely</option>
 					</select>
 				</label>
 			</div>
 			<div class="form-group">
-				<label for="content">What would you like to say?</label>
-				<textarea name="content" id="content" class="form-control" rows="6" required></textarea>
+				<label for="content-area">What would you like to say?</label>
+				<textarea name="content" id="content-area" class="form-control" rows="6" required></textarea>
 			</div>
 			{% if user.is_staff %}
 				<div class="form-group">
 					<input type="checkbox" id="staff_only" name="staff_only"/>
 					<label for="staff_only" style="padding-left: 5px">Make this comment only visible to staff users</label>
 				</div>
 			{% endif %}
@@ -667,20 +675,20 @@
 	$('#delayed_logoff_help').popover();
 
 	function update_stop_button()
 	{
 		if(document.querySelector('#tool_control').checkValidity())
 		{
 			$('#stop_wrapper').tooltip('disable');
-			$("#stop").prop("disabled", false);
+			$("#stop_wrapper button").prop("disabled", false);
 		}
 		else
 		{
 			$('#stop_wrapper').tooltip('enable');
-			$("#stop").prop("disabled", true);
+			$("#stop_wrapper button").prop("disabled", true);
 		}
 	}
 
     show_alerts();
 	update_stop_button();
 	$('body').on('question-group-changed', update_stop_button);
 	$('body').on('change keyup', '#tool_control input, #tool_control select, #tool_control textarea, #downtime', update_stop_button);
```

#### html2text {}

```diff
@@ -33,15 +33,15 @@
 ***** {% if current_usage_event.operator.id == user.id %} You are using this
 tool {% else %} {{_current_usage_event.operator_}} is using this tool {% endif
 %} {% if current_usage_event.operator.id != current_usage_event.user.id %} on
 behalf of {{ current_usage_event.user }} {% endif %} for the project named {
 { current_usage_event.project.name }} since {{ current_usage_event.start|date:
 "l @ " }}{{ current_usage_event.start|time }}. *****
 {% endwith %}
-{% if time_left %}
+{% if time_left and not user.is_staff %}
 Your reservation for this tool will end at {{ time_left|time }}. The remainder
 of your reservation will be relinquished when you stop using this tool.
 {% endif %} {% elif tool.delayed_logoff_in_progress %} {% with
 tool.get_delayed_logoff_usage_event as delayed_logoff_event %}
 ***** {{ delayed_logoff_event.operator }} has finished using the {
 { tool.name_or_child_in_use_name }} but delayed logoff is in effect. The tool
 will be available at {{ delayed_logoff_event.end|time }}. *****
@@ -141,37 +141,43 @@
 Prevent others from using the tool for [Unknown INPUT type] minutes after
 disabling the tool. What's this?
 {% endif %}
 {% url 'disable_tool' tool.get_current_usage_event.tool.id as disable_tool_url
 %} {% button type="delete" id="stop" icon="glyphicon-stop"
 onclick="disable_tool('"|concat:disable_tool_url|concat:"'); return false;"
 value="Stop using the "|concat:tool.name_or_child_in_use_name %}
+{% if time_left and user.is_staff %}
+{% url 'disable_tool' tool.get_current_usage_event.tool.id as disable_tool_url
+%} {% with left_until=time_left|timeuntil %} {% button type="delete" id="stop"
+icon="glyphicon-stop" onclick="disable_tool('"|concat:disable_tool_url|concat:
+"', true); return false;" value="Stop using the "|concat:
+tool.name_or_child_in_use_name|concat:" and relinquish the remaining "|concat:
+left_until|concat:" of your reservation" %} {% endwith %}
+{% endif %}
 {% endif %} {% else %} {% if user.is_staff or user.is_service_personnel and
 tool in user.qualifications.all %}
 *** What would you like to do? ***
-oUse this tool for my own project
-{% if user.is_staff %}
+oUse this tool for my own project {% if user.is_staff %}
 oUse this tool on behalf of another user{% if "remote_work"|customization:
-"remote_work_ask_explicitly" %} (no remote){% endif %}
-{% if "remote_work"|customization:"remote_work_ask_explicitly" %}
-oUse this tool for a remote project
-{% endif %} {% if user.charging_staff_time %} {% with user.get_staff_charge as
-staff_charge %}
- o Use this tool for a remote project{% if "remote_work"|customization:
+"remote_work_ask_explicitly" %} (no remote){% endif %} {% if
+"remote_work"|customization:"remote_work_ask_explicitly" %}
+oUse this tool for a remote project {% endif %} {% if user.charging_staff_time
+%} {% with user.get_staff_charge as staff_charge %}
+o Use this tool for a remote project{% if "remote_work"|customization:
 "remote_work_ask_explicitly" %} (charge staff time{% if
 tool.requires_area_access and "remote_work"|customization:
 "remote_work_start_area_access_automatically" == "enabled" %} & {
 { tool.requires_area_access }} time{% endif %}){% endif %}
  {% endwith %} {% else %}
 oUse this tool for a remote project{% if "remote_work"|customization:
 "remote_work_ask_explicitly" %} (charge staff time{% if
 tool.requires_area_access and "remote_work"|customization:
 "remote_work_start_area_access_automatically" == "enabled" %} & {
-{ tool.requires_area_access }} time{% endif %}){% endif %}
-{% endif %} {% endif %}
+{ tool.requires_area_access }} time{% endif %}){% endif %} {% endif %} {% endif
+%}
 {% elif tool.operational and not tool.required_resource_is_unavailable and not
 tool.delayed_logoff_in_progress and not tool.scheduled_outage_in_progress %} {%
 include 'tool_control/get_projects.html' with
 active_projects=user.active_projects user_id=user.id %} {% endif %} {% if
 user.is_staff or user.is_service_personnel and tool in user.qualifications.all
 or tool.ready_to_use %}
 {% if tool.is_parent_tool %} You have {{ tool.tool_children_set.all|length|add:
```

### Comparing `NEMO-4.5.5/NEMO/templates/tool_control/usage_data.html` & `NEMO-4.6.0/NEMO/templates/tool_control/usage_data.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/training/get_projects.html` & `NEMO-4.6.0/NEMO/templates/training/get_projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/training/training.html` & `NEMO-4.6.0/NEMO/templates/training/training.html`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 	Remove a participant or blank row by clicking the circled X on that row.</p>
 	<p>When a user has successfully completed a training session you have the option to check the "Qualify" box, which qualifies the user for that tool.</p>
 	<br>
 	<form onsubmit="return on_submit()" id="training_session_form">
 		{% csrf_token %}
 		<table id="training_entries" class="table">
 			<tr>
-				<th>&nbsp;</th>
+				<th aria-label="Action">&nbsp;</th>
 				<th style="min-width:200px">Trainee</th>
 				<th style="min-width:200px">Tool</th>
 				<th style="min-width:200px">Project</th>
-				<th>Duration (in minutes)</th>
+				<th>Duration</th>
 				<th>Training type</th>
 				<th>Qualify</th>
 			</tr>
 			{# Rows are inserted here upon load & when "Add another participant" is clicked. #}
 			{% include 'training/training_entry.html' with entry_number=0 %}
 			<tr>
 				<td colspan="7" style="text-align:center"><a href="javascript:void(0)" onclick="add_participant()">Add another participant</a></td>
```

#### html2text {}

```diff
@@ -5,14 +5,14 @@
 You can add participants to a training session by clicking the 'Add another
 participant' link. Remove a participant or blank row by clicking the circled X
 on that row.
 When a user has successfully completed a training session you have the option
 to check the "Qualify" box, which qualifies the user for that tool.
 
 {% csrf_token %}
- Trainee Tool Project Duration (in minutes) Training type Qualify
+ Trainee Tool Project Duration Training type Qualify
 Add_another_participant
 
 {# Note: onclick need to stay blank so it will trigger the onsumbit of this
 form #} {% button id="record_training_sessions" type="save" value="Record
 training sessions" onclick="" %}
  {% endblock %}
```

### Comparing `NEMO-4.5.5/NEMO/templates/training/training_entry.html` & `NEMO-4.6.0/NEMO/templates/training/training_entry.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 <tr id="row_{{ entry_number }}">
 	<td style="vertical-align: middle"><span class="glyphicon glyphicon-remove-circle grey pointer" onclick="remove_row({{ entry_number }})"></span></td>
 	<td>
-		<input type="text" class="form-control" id="user_textbox__{{ entry_number }}" name="chosen_user__{{ entry_number }}" data-row="{{ entry_number }}">
-		<input type="button" class="btn btn-default" style="display:none" id="user_button__{{ entry_number }}" onclick="purge_trainee({{ entry_number }})">
+		<input aria-label="training user #{{ entry_number }}"  type="text" class="form-control" id="user_textbox__{{ entry_number }}" name="chosen_user__{{ entry_number }}" data-row="{{ entry_number }}">
+		<input type="button" class="btn btn-default" style="display:none" id="user_button__{{ entry_number }}" onclick="purge_trainee({{ entry_number }})" value="user">
 	</td>
 	<td>
-		<input type="text" class="form-control" id="tool_textbox__{{ entry_number }}" name="chosen_tool__{{ entry_number }}" data-row="{{ entry_number }}">
+		<input aria-label="training tool #{{ entry_number }}" type="text" class="form-control" id="tool_textbox__{{ entry_number }}" name="chosen_tool__{{ entry_number }}" data-row="{{ entry_number }}">
 		<input type="hidden" id="tool_textbox_type__{{ entry_number }}" name="chosen_type__{{ entry_number }}" data-row="{{ entry_number }}">
-		<input type="button" class="btn btn-default" style="display:none" id="tool_button__{{ entry_number }}" onclick="purge_tool({{ entry_number }})">
+		<input type="button" class="btn btn-default" style="display:none" id="tool_button__{{ entry_number }}" onclick="purge_tool({{ entry_number }})" value="tool">
 	</td>
 	<td id="project__{{ entry_number }}" style="vertical-align: middle">
 
 	</td>
-	<td><input type="number" class="form-control" name="duration__{{ entry_number }}" id="duration__{{ entry_number }}" min="1" inputmode="numeric" pattern="[0-9]*" required></td>
 	<td>
-		<select class="form-control" name="charge_type__{{ entry_number }}" required>
+		<div class="input-group">
+			<input aria-label="training duration #{{ entry_number }}" type="number" class="form-control" name="duration__{{ entry_number }}" id="duration__{{ entry_number }}" min="1" inputmode="numeric" pattern="[0-9]*" required>
+			<div class="input-group-addon">min</div>
+		</div>
+    </td>
+	<td>
+		<select aria-label="training type #{{ entry_number }}" class="form-control" name="charge_type__{{ entry_number }}" required>
 			<option disabled selected value="">&nbsp;</option>
 			{% for charge_type in charge_types %}
 				<option value="{{ charge_type.0 }}">{{ charge_type.1 }}</option>
 			{% endfor %}
 		</select>
 	</td>
-	<td style="vertical-align: middle"><input type="checkbox" name="qualify__{{ entry_number }}" checked></td>
+	<td style="vertical-align: middle"><input aria-label="training qualification #{{ entry_number }}"  type="checkbox" name="qualify__{{ entry_number }}" checked></td>
 </tr>
```

### Comparing `NEMO-4.5.5/NEMO/templates/usage/adjustment_request_button.html` & `NEMO-4.6.0/NEMO/templates/usage/adjustment_request_button.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% load custom_tags_and_filters %}
 {% if "requests"|customization:"adjustment_requests_enabled" %}
     {% with content_type=charge|content_type %}
         {% url 'create_adjustment_request' content_type.id charge.id as create_adjustment_request %}
         {% if not existing_adjustments or content_type.id not in existing_adjustments or charge.id not in existing_adjustments|get_item:content_type.id %}
-            <span style="position: absolute; top: 15px; right: 15px">
+            <span class="usage-charge-adjustment-button">
                 {% button size="small" type="warn" url=create_adjustment_request value="Request an adjustment" icon="glyphicon-flag" %}
             </span>
         {% else %}
-            <span style="position: absolute; top: 15px; right: 15px" title="An adjustment request already exists for this charge">
+            <span class="usage-charge-adjustment-button" title="An adjustment request already exists for this charge">
                 {% button size="small" type="warn" url=create_adjustment_request value="Request an adjustment" icon="glyphicon-flag" disabled="true" %}
             </span>
         {% endif %}
     {% endwith %}
 {% endif %}
```

### Comparing `NEMO-4.5.5/NEMO/templates/usage/billing.html` & `NEMO-4.6.0/NEMO/templates/usage/billing.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/usage/usage.html` & `NEMO-4.6.0/NEMO/templates/usage/usage.html`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 			{% if no_charges %}
 				<h3>There was no usage between {{ start_date|date }} and {{ end_date|date }}.</h3>
             {% endif %}
             {% with adj_reservation="requests"|customization:"adjustment_requests_missed_reservation_enabled" adj_tool_usage="requests"|customization:"adjustment_requests_tool_usage_enabled" adj_area_access="requests"|customization:"adjustment_requests_area_access_enabled" adj_staff_charge="requests"|customization:"adjustment_requests_staff_staff_charges_enabled" %}
                 {% if missed_reservations %}
                     <h3>Missed reservations</h3>
                     {% for m in missed_reservations %}
-                        <div class="alert alert-danger" style="position: relative">
+                        <div class="usage-charge alert alert-danger">
                             <span style="font-weight:bold">{{ m.reservation_item }}</span><br>
                             {% if project_autocomplete or selected_project %}Missed by {{ m.user }}<br>{% endif %}
                             {{ m.start }}<br>
                             Charged to project {{ m.project }}
                             {% if adj_reservation == "enabled" %}
                                 {% if not adjustment_time_limit or adjustment_time_limit <= m.end %}
                                     {% if m.user == user or m.project in pi_projects %}
@@ -38,27 +38,27 @@
                             {% endif %}
                         </div>
                     {% endfor %}
                 {% endif %}
                 {% if consumables %}
                     <h3>Supplies and consumables</h3>
                     {% for c in consumables %}
-                        <div class="alert alert-info" style="position: relative">
+                        <div class="usage-charge alert alert-info">
                             <span style="font-weight:bold">{{ c.consumable }}</span><br>
                             {% if project_autocomplete or selected_project %}<span style="font-weight:bold">For {{ c.customer }}</span><br>{% endif %}
                             Quantity {{ c.quantity }}<br>
                             Purchased from {{ c.merchant }} on {{ c.date }}<br>
                             Charged to project {{ c.project }}
                         </div>
                     {% endfor %}
                 {% endif %}
                 {% if staff_charges %}
                     <h3>Staff charges</h3>
                     {% for s in staff_charges %}
-                        <div class="alert alert-info" style="position: relative">
+                        <div class="usage-charge alert alert-info">
                             <span style="font-weight:bold">Work performed by {{ s.staff_member }} {% if project_autocomplete or selected_project %}on behalf of {{ s.customer }}{% else %}on your behalf{% endif %}</span><br>
                             {% if s.note %}Charge note: {{ s.note|linebreaksbr }}<br>{% endif %}
                             {{ s.start }}<br>
                             {{ s.end }}<br>
                             Charged to project {{ s.project }}
                             {% if adj_staff_charge == "enabled" and s.staff_member == user and user.is_staff %}
                                 {% if not adjustment_time_limit or adjustment_time_limit <= s.end %}
@@ -67,26 +67,26 @@
                             {% endif %}
                         </div>
                     {% endfor %}
                 {% endif %}
                 {% if training_sessions %}
                     <h3>Training sessions</h3>
                     {% for t in training_sessions %}
-                        <div class="alert alert-info" style="position: relative">
+                        <div class="usage-charge alert alert-info">
                             <span style="font-weight:bold">{{ t.tool }}</span> {{ t.get_type_display }} training {% if project_autocomplete or selected_project %}for {{ t.trainee }} {% endif %}<br>
                             Trained by <span style="font-weight:bold">{{ t.trainer }}</span><br>
                             {{ t.date }} ({{ t.duration }} minutes)<br>
                             Charged to project {{ t.project }}
                         </div>
                     {% endfor %}
                 {% endif %}
                 {% if area_access %}
                     <h3>Area access</h3>
                     {% for a in area_access %}
-                        <div class="alert {% if not a.staff_charge %}alert-info{% else %}alert-warning{% endif %}" style="position: relative">
+                        <div class="usage-charge alert {% if not a.staff_charge %}alert-info{% else %}alert-warning{% endif %}">
                             <span style="font-weight:bold">{{ a.area }}</span><br>
                             {% if a.staff_charge %}<span style="font-weight:bold">Area accessed by {{ a.staff_charge.staff_member }} {% if project_autocomplete or selected_project %}on behalf of {{ a.customer }}{% else %}on your behalf{% endif %}</span><br>
                             {% else %}{% if project_autocomplete or selected_project %}<span style="font-weight:bold">Area accessed by {{ a.customer }}</span><br>{% endif %}
                             {% endif %}
                             {{ a.start }}<br>
                             {{ a.end|default_if_none:"In progress" }}<br>
                             Charged to project {{ a.project }}
@@ -105,15 +105,15 @@
                             {% endif %}
                         </div>
                     {% endfor %}
                 {% endif %}
                 {% if usage_events %}
                     <h3>Tool usage</h3>
                     {% for u in usage_events %}
-                        <div class="alert {% if u.user == u.operator %}alert-info{% else %}alert-warning{% endif %}" style="position: relative">
+                        <div class="usage-charge alert {% if u.user == u.operator %}alert-info{% else %}alert-warning{% endif %}">
                             <span style="font-weight:bold">{{ u.tool }}</span><br>
                             {% if u.user != u.operator %}<span style="font-weight:bold">Operated by {{ u.operator }} {% if project_autocomplete or selected_project %}on behalf of {{ u.user }}{% else %}on your behalf{% endif %}</span><br>
                             {% else %}{% if project_autocomplete or selected_project %}<span style="font-weight:bold">Operated by {{ u.user }}</span><br>{% endif %}
                             {% endif %}
                             {{ u.start }}<br>
                             {{ u.end }}<br>
                             Charged to project {{ u.project }}
```

### Comparing `NEMO-4.5.5/NEMO/templates/usage/usage_base.html` & `NEMO-4.6.0/NEMO/templates/usage/usage_base.html`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 {% block title %}Usage{% if billing_service %} and billing information{% endif %}{% endblock %}
 {% block extrahead %}
 	<script type="text/javascript" src="{% static "datetimepicker/bootstrap-datetimepicker.js" %}"></script>
 	<link rel="stylesheet" type="text/css" href="{% static "datetimepicker/bootstrap-datetimepicker.css" %}"/>
 {% endblock %}
 {% block content %}
 	<h1>Usage{% if billing_service %} and billing information{% endif %}
-		<small> between {{ start_date|date }} and {{ end_date|date }}</small>
+		<small class="light-grey"> between {{ start_date|date }} and {{ end_date|date }}</small>
 	</h1>
 	<p>
 		This page presents a monthly report of your {{ facility_name }} usage{% if billing_service %} and billing information{% endif %}. Approved adjustments are{% if not billing_service %} not{% endif %} reflected{% if billing_service %} in the billing information data but not{% endif %} in the usage data.
 	</p>
 	<div style="height: 20px"></div>
 	<form class="form-horizontal" role="form">
 		<div class="form-group">
@@ -50,22 +50,35 @@
                             <option selected value="">All</option>
                             {% for project in pi_projects %}
                                 <option value="{{ project.id }}" {% if selected_project and selected_project.id == project.id %}selected{% endif %}>{{ project.name }}</option>
                             {% endfor %}
                         </select>
                     </div>
             {% endif %}
+			{% if user.active_projects %}
+                </div>
+                <div class="form-group">
+                    <div class="control-label col-sm-2">
+                        <label for="project">Project</label>
+                    </div>
+                    <div class="col-sm-3 col-md-3 col-lg-2">
+                        <select name="project" id="project" class="form-control" style="text-align-last:center" title="Select a project to see usage for only that project">
+                            <option selected value="">All</option>
+                            {% for project in user.active_projects %}
+                                <option value="{{ project.id }}" {% if selected_user_project and selected_user_project.id == project.id %}selected{% endif %}>{{ project.name }}</option>
+                            {% endfor %}
+                        </select>
+                    </div>
+            {% endif %}
 			{% if not project_autocomplete %}
-				<div class="hidden-lg hidden-md hidden-sm">&nbsp;</div>
-				<div class="col-md-3">
+				<div class="hidden-lg hidden-md {% if user.active_projects or pi_projects %}hidden-sm{% else %}col-sm-12{% endif %}">&nbsp;</div>
+				<div class="col-sm-4 col-lg-3 {% if user.active_projects or pi_projects %}text-right{% else %}col-md-3{% endif %}">
                     {% button type="save" submit=False onclick="$('#csv_export').val('');this.form.submit();" value="Update" icon="glyphicon-refresh" %}
-                    {% if can_export %}
-                        <input id="csv_export" type="hidden" name="csv" value="">
-                        {% button style="margin-left: 15px" type="export" onclick="$('#csv_export').val('true');this.form.submit();" value="Export" %}
-                    {% endif %}
+                    <input id="csv_export" type="hidden" name="csv" value="">
+                    {% button style="margin-left: 15px" type="export" onclick="$('#csv_export').val('true');this.form.submit();" value="Export" %}
 				</div>
 			{% endif %}
 		</div>
 		<input id="type" name="type" type="hidden" value="{{ kind|default:'' }}"/>
 		<input id="id" name="id" type="hidden" value="{{ identifier|default:'' }}"/>
 
 		<script>
```

#### html2text {}

```diff
@@ -19,20 +19,26 @@
 [{{ end_date.date|input_date_format }}]
 {% if pi_projects %}
 Managed project
 {% for project in pi_projects %}
 % if selected_project and selected_project.id == project.id %}selected{% endif
 %}>{{ project.name }}
 {% endfor %}
+{% endif %} {% if user.active_projects %}
+Project
+{% for project in user.active_projects %}
+% if selected_user_project and selected_user_project.id == project.id
+%}selected{% endif %}>{{ project.name }}
+{% endfor %}
 {% endif %} {% if not project_autocomplete %}
  
 {% button type="save" submit=False onclick="$('#csv_export').val
-('');this.form.submit();" value="Update" icon="glyphicon-refresh" %} {% if
-can_export %}  {% button style="margin-left: 15px" type="export" onclick="$
-('#csv_export').val('true');this.form.submit();" value="Export" %} {% endif %}
+('');this.form.submit();" value="Update" icon="glyphicon-refresh" %}  {% button
+style="margin-left: 15px" type="export" onclick="$('#csv_export').val
+('true');this.form.submit();" value="Export" %}
 {% endif %}
 
  {% if project_autocomplete %}
 For
 % if selection %}placeholder="{{ selection }}" {% else %}placeholder="Search
 for an account, project, application or user"{% endif %}>
```

### Comparing `NEMO-4.5.5/NEMO/templates/users/create_or_modify_user.html` & `NEMO-4.6.0/NEMO/templates/users/create_or_modify_user.html`

 * *Files 0% similar despite different names*

```diff
@@ -334,15 +334,15 @@
 					{% for d in form.instance.user_documents.all %}
 						<div id="document_{{ d.id }}">{% if not readonly %}<a href="javascript:mark_document_for_removal('{{ d.id }}')" class="grey hover-black" title="Remove {{ d.filename }}"><span class="glyphicon glyphicon-remove-circle"></span></a>{% endif %} <a href="{{ d.document.url }}" target="_blank" style="margin-right: 5px">{{ d.filename }}</a></div>
 					{% empty %}
                         <div class="form-control-static">This user doesn't have any documents.</div>
 					{% endfor %}
                     {% if not readonly and allow_document_upload %}
                         <div style="padding-top: 10px">
-                            <input id="fileupload" type="file" name="user_documents" multiple>
+                            <input aria-label="File upload" id="fileupload" type="file" name="user_documents" multiple>
                         </div>
                     {% endif %}
 				</div>
 			</div>
 		{% endif %}
         {% if not readonly %}
             <div class="form-group">
```

### Comparing `NEMO-4.5.5/NEMO/templates/users/safe_deactivation.html` & `NEMO-4.6.0/NEMO/templates/users/safe_deactivation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/templates/users/users.html` & `NEMO-4.6.0/NEMO/templates/users/users.html`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 					<th>{% include 'pagination/pagination_column.html' with order_by='username' name='Username' %}</th>
 					{% if user_types %}<th>{% include 'pagination/pagination_column.html' with order_by='type' name='Type' %}</th>{% endif %}
 					<th>{% include 'pagination/pagination_column.html' with order_by='is_active' name='Active' %}</th>
 					<th>{% include 'pagination/pagination_column.html' with order_by='is_staff' name='Staff' %}</th>
 					<th>{% include 'pagination/pagination_column.html' with order_by='is_user_office' name='User Office' %}</th>
 					<th>{% include 'pagination/pagination_column.html' with order_by='is_accounting_officer' name='Accounting' %}</th>
 					<th>{% include 'pagination/pagination_column.html' with order_by='is_superuser' name='Admin' %}</th>
-					<th></th>
+					<th aria-label="Actions"></th>
 				</tr>
 			</thead>
 			<tbody>
 				{% for user in page %}
 					<tr>
 						<td>{{ user.first_name }}</td>
 						<td>{{ user.last_name }}</td>
```

### Comparing `NEMO-4.5.5/NEMO/templatetags/custom_tags_and_filters.py` & `NEMO-4.6.0/NEMO/templatetags/custom_tags_and_filters.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
 from datetime import timedelta
 from importlib.metadata import PackageNotFoundError, version
+from urllib.parse import quote
 
 from django import template
 from django.contrib.contenttypes.models import ContentType
 from django.shortcuts import resolve_url
 from django.template import Context, Template
 from django.template.defaultfilters import date, time
 from django.urls import NoReverseMatch, reverse
@@ -12,14 +13,15 @@
 from django.utils.formats import localize_input
 from django.utils.html import escape, escapejs, format_html
 from django.utils.safestring import mark_safe
 
 from NEMO.mixins import BillableItemMixin
 from NEMO.models import User
 from NEMO.utilities import get_full_url
+from NEMO.views.constants import NEXT_PARAMETER_NAME
 from NEMO.views.customization import CustomizationBase, ProjectsAccountsCustomization
 
 register = template.Library()
 
 
 @register.filter
 def class_name(value):
@@ -173,21 +175,37 @@
 @register.filter
 def content_type(obj):
 	if obj:
 		return ContentType.objects.get_for_model(obj)
 
 
 @register.simple_tag(takes_context=True)
-def admin_edit_url(context, obj):
+def admin_edit_url(context, obj, redirect_url=None):
 	user = context["request"].user
 	try:
 		obj_type = content_type(obj)
 		permission = user.has_perm(f"{obj_type.app_label}.change_{obj_type.model}")
 		if permission:
 			url = reverse(f"admin:{obj_type.app_label}_{obj_type.model}_change", args=[obj.id])
+			if redirect_url:
+				url += f"?{NEXT_PARAMETER_NAME}={quote(redirect_url)}"
+			return url
+	except:
+		pass
+
+
+@register.simple_tag(takes_context=True)
+def admin_add_url(context, app_label, model_name, next_url=None):
+	user = context["request"].user
+	try:
+		permission = user.has_perm(f"{app_label}.add_{model_name}")
+		if permission:
+			url = reverse(f"admin:{app_label}_{model_name}_add")
+			if next_url:
+				url += f"?{NEXT_PARAMETER_NAME}={quote(next_url)}"
 			return url
 	except:
 		pass
 
 
 @register.filter
 def billable_display(item: BillableItemMixin, user: User):
@@ -237,15 +255,15 @@
 		"btn_title": value if title is None else title,
 		"btn_class": btn_class,
 		"btn_icon": btn_icon + second_icon if icon is None else btn_icon + icon,
 		"btn_onclick": onclick if onclick is not None else "submit_and_disable(this);" if submit else "",
 		"btn_type": None if url else "submit" if submit else "button",
 		"btn_url": resolve_url(url) if url else None,
 		"btn_dismiss": dismiss,
-		"kwargs": kwargs,  # pass the rest of the kwargs directly to the button to be used as attributes
+		"kwargs": {key.replace("_", "-"): value for key, value in kwargs.items()},  # pass the rest of the kwargs directly to the button to be used as attributes
 	}
 
 
 @register.simple_tag(takes_context=True)
 def absolute_url(context, view_name, *args, **kwargs):
 	url = reverse(view_name, args=args, kwargs=kwargs)
 	return get_full_url(url, request=context['request'])
```

### Comparing `NEMO-4.5.5/NEMO/urls.py` & `NEMO-4.6.0/NEMO/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import logging
+import os
 from importlib import import_module
 
 from django.apps import apps
 from django.conf import settings
 from django.conf.urls import include
 from django.contrib import admin
 from django.contrib.auth.decorators import login_required
 from django.contrib.auth.views import LogoutView
 from django.urls import path, re_path
 from django.views.decorators.clickjacking import xframe_options_sameorigin
 from django.views.generic import RedirectView
 from django.views.static import serve
 from rest_framework import routers
 
+from NEMO.decorators import any_staff_required
 from NEMO.models import ReservationItemType
 from NEMO.views import (
 	abuse,
 	access_requests,
 	accounts_and_projects,
 	adjustment_requests,
 	alerts,
@@ -52,14 +54,15 @@
 	tool_control,
 	training,
 	tutorials,
 	usage,
 	user_requests,
 	users,
 )
+from NEMO.views.constants import MEDIA_PROTECTED
 
 logger = logging.getLogger(__name__)
 
 # REST API URLs
 router = routers.DefaultRouter()
 router.register(r"auth_groups", api.GroupViewSet)
 router.register(r"auth_permissions", api.PermissionViewSet)
@@ -187,14 +190,15 @@
 	path("resize_reservation/", calendar.resize_reservation, name="resize_reservation"),
 	path("resize_outage/", calendar.resize_outage, name="resize_outage"),
 	path("move_reservation/", calendar.move_reservation, name="move_reservation"),
 	path("move_outage/", calendar.move_outage, name="move_outage"),
 	path("cancel_reservation/<int:reservation_id>/", calendar.cancel_reservation, name="cancel_reservation"),
 	path("cancel_outage/<int:outage_id>/", calendar.cancel_outage, name="cancel_outage"),
 	path("set_reservation_title/<int:reservation_id>/", calendar.set_reservation_title, name="set_reservation_title"),
+	path("change_reservation_date/", calendar.change_reservation_date, name="change_reservation_date"),
 	path("change_reservation_project/<int:reservation_id>/", calendar.change_reservation_project, name="change_reservation_project"),
 	path("proxy_reservation/", calendar.proxy_reservation, name="proxy_reservation"),
 	path("reservation_group_question/<int:reservation_question_id>/<str:group_name>/", calendar.reservation_group_question, name="reservation_group_question"),
 
 	# Event Details:
 	path("event_details/reservation/<int:reservation_id>/", event_details.reservation_details, name="reservation_details"),
 	path("event_details/outage/<int:outage_id>/", event_details.outage_details, name="outage_details"),
@@ -339,16 +343,19 @@
 	path("news/archive_story/<int:story_id>/", news.archive_story, name="archive_story"),
 	path("news/new/", news.new_news_form, name="new_news_form"),
 	path("news/update/<int:story_id>/", news.news_update_form, name="news_update_form"),
 	path("news/publish/", news.publish, name="publish_new_news"),
 	path("news/publish/<int:story_id>/", news.publish, name="publish_news_update"),
 
 	# Media
+	re_path(r"^media/" + MEDIA_PROTECTED + "/(?P<path>.*)$", any_staff_required(xframe_options_sameorigin(serve)), {"document_root": os.path.join(settings.MEDIA_ROOT, MEDIA_PROTECTED)}, name="media_protected"),
 	re_path(r"^media/(?P<path>.*)$", login_required(xframe_options_sameorigin(serve)), {"document_root": settings.MEDIA_ROOT}, name="media"),
-	re_path(r"^media_view/(?P<popup>(true|false))/(?P<document_type>\w+)/(?P<document_id>\d+)/$", documents.media_view, name="media_view"),
+	re_path(r"^media_view/(?P<popup>(true|false))/(?P<content_type_id>\d+)/(?P<document_id>\d+)/$", documents.media_view, name="media_view"),
+	re_path(r"^media_list_view/(?P<popup>(true|false))/(?P<allow_zip>(true|false))/$", documents.media_list_view, name="media_list_view"),
+	path("media_zip/", documents.media_zip, name="media_zip"),
 
 	# User Preferences
 	path("user_preferences/", users.user_preferences, name="user_preferences"),
 ]
 
 if settings.ALLOW_CONDITIONAL_URLS:
 	if apps.is_installed("django.contrib.admin"):
@@ -405,15 +412,15 @@
 
 		# Site customization:
 		path("customization/", customization.customization, name="customization"),
 		path("customization/<str:key>/", customization.customization, name="customization"),
 		path("customize/<str:key>/", customization.customize, name="customize"),
 		path("customize/<str:key>/<str:element>/", customization.customize, name="customize"),
 
-		# Project Usage:
+		# Project usage:
 		path("project_usage/", usage.project_usage, name="project_usage"),
 		path("project_billing/", usage.project_billing, name="project_billing"),
 
 		# Staff absence
 		path("create_staff_absence/", status_dashboard.create_staff_absence, name="create_staff_absence"),
 		path("edit_staff_absence/<int:absence_id>/", status_dashboard.create_staff_absence, name="edit_staff_absence"),
 		path("delete_staff_absence/<int:absence_id>/", status_dashboard.delete_staff_absence, name="delete_staff_absence"),
```

### Comparing `NEMO-4.5.5/NEMO/utilities.py` & `NEMO-4.6.0/NEMO/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import importlib
 import os
 from calendar import monthrange
 from datetime import date, datetime, time
 from email import encoders
 from email.mime.base import MIMEBase
 from enum import Enum
-from io import BytesIO
+from io import BytesIO, StringIO
 from logging import getLogger
 from typing import Dict, List, Optional, Sequence, Set, Tuple, Union
 from urllib.parse import urljoin
 
+import pytz
 from PIL import Image
 from dateutil import rrule
 from dateutil.parser import parse
 from django.apps import apps
 from django.conf import global_settings, settings
 from django.contrib.admin import ModelAdmin
 from django.contrib.contenttypes.models import ContentType
@@ -74,14 +75,19 @@
 date_input_format = get_format("DATE_INPUT_FORMATS")[0]
 datetime_input_format = get_format("DATETIME_INPUT_FORMATS")[0]
 time_input_js_format = convert_py_format_to_js(time_input_format)
 date_input_js_format = convert_py_format_to_js(date_input_format)
 datetime_input_js_format = convert_py_format_to_js(datetime_input_format)
 
 
+supported_embedded_video_extensions = [".mp4", ".ogv", ".webm", ".3gp"]
+supported_embedded_pdf_extensions = [".pdf"]
+supported_embedded_extensions = supported_embedded_pdf_extensions + supported_embedded_video_extensions
+
+
 class EmptyHttpRequest(HttpRequest):
 	def __init__(self):
 		super().__init__()
 		self.session = QueryDict(mutable=True)
 		self.device = "desktop"
 
 
@@ -403,14 +409,17 @@
 	except TypeError:
 		raise TypeError("to, cc and bcc arguments must be a list, set or tuple")
 	user_reply_to = getattr(settings, "EMAIL_USE_DEFAULT_AND_REPLY_TO", False)
 	reply_to = None
 	if user_reply_to:
 		reply_to = [from_email]
 		from_email = None
+	email_prefix = getattr(settings, "NEMO_EMAIL_SUBJECT_PREFIX", None)
+	if email_prefix and not subject.startswith(email_prefix):
+		subject = email_prefix + subject
 	mail = EmailMessage(
 		subject=subject,
 		body=content,
 		from_email=from_email,
 		to=clean_to,
 		bcc=clean_bcc,
 		cc=clean_cc,
@@ -490,21 +499,14 @@
 	from django.template.defaultfilters import slugify
 
 	tool_name = slugify(tool)
 	ext = os.path.splitext(filename)[1]
 	return f"tool_images/{tool_name}{ext}"
 
 
-def get_tool_document_filename(tool_documents, filename):
-	from django.template.defaultfilters import slugify
-
-	tool_name = slugify(tool_documents.tool.name)
-	return f"tool_documents/{tool_name}/{filename}"
-
-
 def get_hazard_logo_filename(category, filename):
 	from django.template.defaultfilters import slugify
 
 	category_name = slugify(category)
 	ext = os.path.splitext(filename)[1]
 	return f"chemical_hazard_logos/{category_name}{ext}"
 
@@ -512,33 +514,16 @@
 def get_chemical_document_filename(chemical, filename):
 	from django.template.defaultfilters import slugify
 
 	chemical_name = slugify(chemical.name)
 	return f"chemical_documents/{chemical_name}/{filename}"
 
 
-def get_project_document_filename(project_documents, filename):
-	from django.template.defaultfilters import slugify
-
-	project_name = slugify(project_documents.project.name)
-	return f"project_documents/{project_name}/{filename}"
-
-
-def get_user_document_filename(user_documents, filename):
-	from django.template.defaultfilters import slugify
-
-	username = slugify(user_documents.user.username)
-	return f"user_documents/{username}/{filename}"
-
-
-def get_safety_document_filename(safety_documents, filename):
-	from django.template.defaultfilters import slugify
-
-	item_name = slugify(safety_documents.safety_item.name)
-	return f"safety_item/{item_name}/{filename}"
+def document_filename_upload(instance, filename):
+	return instance.get_filename_upload(filename)
 
 
 def resize_image(image: InMemoryUploadedFile, max: int, quality=85) -> InMemoryUploadedFile:
 	"""Returns a resized image based on the given maximum size"""
 	with Image.open(image) as img:
 		width, height = img.size
 		# no need to resize if width or height is already less than the max
@@ -679,7 +664,49 @@
 
 def get_class_from_settings(setting_name: str, default_value: str):
 	setting_class = getattr(settings, setting_name, default_value)
 	assert isinstance(setting_class, str)
 	pkg, attr = setting_class.rsplit(".", 1)
 	ret = getattr(importlib.import_module(pkg), attr)
 	return ret()
+
+
+def create_ics(identifier, event_name, start: datetime, end: datetime, user, organizer=None, cancelled: bool = False):
+	from NEMO.views.customization import ApplicationCustomization
+
+	site_title = ApplicationCustomization.get("site_title")
+	if organizer:
+		organizer_email = organizer.email
+		organizer = organizer.get_name()
+	else:
+		organizer_email = getattr(settings, "RESERVATION_ORGANIZER_EMAIL", "no_reply")
+		organizer = getattr(settings, "RESERVATION_ORGANIZER", site_title)
+	method_name = "CANCEL" if cancelled else "REQUEST"
+	sequence = "SEQUENCE:2\n" if cancelled else "SEQUENCE:0\n"
+	priority = "PRIORITY:5\n" if cancelled else "PRIORITY:0\n"
+	now = datetime.utcnow().strftime("%Y%m%dT%H%M%SZ")
+	start = start.astimezone(pytz.utc).strftime("%Y%m%dT%H%M%SZ")
+	end = end.astimezone(pytz.utc).strftime("%Y%m%dT%H%M%SZ")
+	lines = [
+		"BEGIN:VCALENDAR\n",
+		"VERSION:2.0\n",
+		f"METHOD:{method_name}\n",
+		"BEGIN:VEVENT\n",
+		f"UID:{str(identifier)}\n",
+		sequence,
+		priority,
+		f"DTSTAMP:{now}\n",
+		f"DTSTART:{start}\n",
+		f"DTEND:{end}\n",
+		f'ATTENDEE;CN="{user.get_name()}";RSVP=TRUE:mailto:{user.email}\n',
+		f'ORGANIZER;CN="{organizer}":mailto:{organizer_email}\n',
+		f"SUMMARY:[{site_title}] {event_name}\n",
+		f"STATUS:{'CANCELLED' if cancelled else 'CONFIRMED'}\n",
+		"END:VEVENT\n",
+		"END:VCALENDAR\n"
+	]
+	ics = StringIO("")
+	ics.writelines(lines)
+	ics.seek(0)
+
+	attachment = create_email_attachment(ics, maintype="text", subtype="calendar", method=method_name)
+	return attachment
```

### Comparing `NEMO-4.5.5/NEMO/views/abuse.py` & `NEMO-4.6.0/NEMO/views/abuse.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/views/access_requests.py` & `NEMO-4.6.0/NEMO/views/access_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 	Notification,
 	PhysicalAccessLevel,
 	RequestStatus,
 	TemporaryPhysicalAccess,
 	TemporaryPhysicalAccessRequest,
 	User,
 )
+from NEMO.typing import QuerySetType
 from NEMO.utilities import (
 	BasicDisplayTable,
 	EmailCategory,
 	beginning_of_the_day,
 	bootstrap_primary_color,
 	export_format_datetime,
 	format_datetime,
@@ -312,28 +313,27 @@
 
 @user_office_or_manager_required
 @require_GET
 def csv_export(request):
 	return access_csv_export(TemporaryPhysicalAccessRequest.objects.filter(deleted=False))
 
 
-def access_csv_export(request_list: List[TemporaryPhysicalAccessRequest]) -> HttpResponse:
+def access_csv_export(request_qs: QuerySetType[TemporaryPhysicalAccessRequest]) -> HttpResponse:
 	table_result = BasicDisplayTable()
 	table_result.add_header(("status", "Status"))
 	table_result.add_header(("created_date", "Created date"))
 	table_result.add_header(("last_updated", "Last updated"))
 	table_result.add_header(("creator", "Creator"))
 	table_result.add_header(("other_users", "Buddies"))
 	table_result.add_header(("area", "Area"))
 	table_result.add_header(("access_level", "Access level"))
 	table_result.add_header(("start", "Start"))
 	table_result.add_header(("end", "End"))
 	table_result.add_header(("reviewer", "Reviewer"))
-	for req in request_list:
-		req: TemporaryPhysicalAccessRequest = req
+	for req in request_qs:
 		table_result.add_row(
 			{
 				"status": req.get_status_display(),
 				"created_date": req.creation_time,
 				"last_updated": req.last_updated,
 				"creator": req.creator,
 				"other_users": ", ".join([str(user) for user in req.other_users.all()]),
```

### Comparing `NEMO-4.5.5/NEMO/views/accounts_and_projects.py` & `NEMO-4.6.0/NEMO/views/accounts_and_projects.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/views/adjustment_requests.py` & `NEMO-4.6.0/NEMO/views/adjustment_requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from datetime import timedelta
 from typing import List
 
 from django.contrib.auth.decorators import login_required
 from django.contrib.contenttypes.models import ContentType
+from django.db.models import Q
 from django.http import HttpResponse, HttpResponseBadRequest
 from django.shortcuts import get_object_or_404, redirect, render
 from django.template.defaultfilters import linebreaksbr
 from django.urls import reverse
 from django.utils import timezone
 from django.views.decorators.http import require_GET, require_POST, require_http_methods
 
@@ -25,15 +26,14 @@
     User,
 )
 from NEMO.utilities import (
     BasicDisplayTable,
     EmailCategory,
     bootstrap_primary_color,
     export_format_datetime,
-    get_email_from_settings,
     get_full_url,
     quiet_int,
     render_email_template,
     send_mail,
 )
 from NEMO.views.customization import (
     EmailsCustomization,
@@ -55,14 +55,24 @@
         return HttpResponseBadRequest("Adjustment requests are not enabled")
 
     user: User = request.user
     max_requests = quiet_int(UserRequestsCustomization.get("adjustment_requests_display_max"), None)
     adj_requests = AdjustmentRequest.objects.filter(deleted=False)
     if not user.is_facility_manager and not user.is_user_office and not user.is_accounting_officer:
         adj_requests = adj_requests.filter(creator=user)
+    if user.is_facility_manager and user.get_preferences().tool_adjustment_notifications.all():
+        exclude = []
+        tools = user.get_preferences().tool_adjustment_notifications.all()
+        if tools:
+            for adj in adj_requests:
+                tool = getattr(adj.item, "tool", None) if adj.item else None
+                if tool and tool not in tools:
+                    exclude.append(adj.pk)
+            adj_requests = adj_requests.exclude(pk__in=exclude)
+
     dictionary = {
         "pending_adjustment_requests": adj_requests.filter(status=RequestStatus.PENDING),
         "approved_adjustment_requests": adj_requests.filter(status=RequestStatus.APPROVED)[:max_requests],
         "denied_adjustment_requests": adj_requests.filter(status=RequestStatus.DENIED)[:max_requests],
         "adjustment_requests_description": UserRequestsCustomization.get("adjustment_requests_description"),
         "request_notifications": get_notifications(
             request.user, Notification.Types.ADJUSTMENT_REQUEST, delete=not user.is_facility_manager
@@ -210,16 +220,20 @@
 
 
 def send_request_received_email(request, adjustment_request: AdjustmentRequest, edit):
     user_office_email = EmailsCustomization.get("user_office_email_address")
     adjustment_request_notification_email = get_media_file_contents("adjustment_request_notification_email.html")
     if user_office_email and adjustment_request_notification_email:
         # cc facility managers
-        facility_managers: List[User] = list(User.objects.filter(is_active=True, is_facility_manager=True))
-        ccs = [
+        tool = getattr(adjustment_request.item, "tool", None) if adjustment_request.item else None
+        facility_managers_qs = User.objects.filter(is_active=True, is_facility_manager=True)
+        if tool:
+            facility_managers_qs = facility_managers_qs.filter(Q(preferences__tool_adjustment_notifications__isnull=True)|Q(preferences__tool_adjustment_notifications__in=[tool]))
+        facility_managers: List[User] = list(facility_managers_qs)
+        manager_emails = [
             email
             for user in facility_managers
             for email in user.get_emails(user.get_preferences().email_send_adjustment_request_updates)
         ]
         status = (
             "approved"
             if adjustment_request.status == RequestStatus.APPROVED
@@ -236,34 +250,45 @@
             "adjustment_request": adjustment_request,
             "status": status,
             "adjustment_requests_url": absolute_url,
             "manager_note": adjustment_request.manager_note if status == "denied" else None,
             "user_office": False,
         }
         message = render_email_template(adjustment_request_notification_email, dictionary)
-        email_notification = adjustment_request.creator.get_preferences().email_send_adjustment_request_updates
-        send_mail(
-            subject=f"Your adjustment request has been {status}",
-            content=message,
-            from_email=user_office_email,
-            to=adjustment_request.creator.get_emails(email_notification),
-            cc=ccs,
-            email_category=EmailCategory.ADJUSTMENT_REQUESTS,
-        )
+        creator_notification = adjustment_request.creator.get_preferences().email_send_adjustment_request_updates
+        if status in ["received", "updated"]:
+            send_mail(
+                subject=f"Adjustment request {status}",
+                content=message,
+                from_email=adjustment_request.creator.email,
+                to=manager_emails,
+                cc=adjustment_request.creator.get_emails(creator_notification),
+                email_category=EmailCategory.ADJUSTMENT_REQUESTS,
+            )
+        else:
+            send_mail(
+                subject=f"Your adjustment request has been {status}",
+                content=message,
+                from_email=adjustment_request.reviewer.email,
+                to=adjustment_request.creator.get_emails(creator_notification),
+                cc=manager_emails,
+                email_category=EmailCategory.ADJUSTMENT_REQUESTS,
+            )
+
         # Send separate email to the user office (with the extra note) when a request is approved
         if adjustment_request.status == RequestStatus.APPROVED:
             dictionary["manager_note"] = adjustment_request.manager_note
             dictionary["user_office"] = True
             message = render_email_template(adjustment_request_notification_email, dictionary)
             send_mail(
                 subject=f"{adjustment_request.creator.get_name()}'s adjustment request has been {status}",
                 content=message,
-                from_email=get_email_from_settings(),
+                from_email=adjustment_request.reviewer.email,
                 to=[user_office_email],
-                cc=ccs,
+                cc=manager_emails,
                 email_category=EmailCategory.ADJUSTMENT_REQUESTS,
             )
 
 
 def email_interested_parties(reply: RequestMessage, reply_url):
     creator: User = reply.content_object.creator
     for user in reply.content_object.creator_and_reply_users():
@@ -276,15 +301,15 @@
 {linebreaksbr(reply.content)}
 <br><br>
 Please visit {reply_url} to reply"""
             email_notification = user.get_preferences().email_send_adjustment_request_updates
             user.email_user(
                 subject=subject,
                 message=message,
-                from_email=get_email_from_settings(),
+                from_email=reply.author.email,
                 email_notification=email_notification,
                 email_category=EmailCategory.ADJUSTMENT_REQUESTS,
             )
 
 
 def can_change_times(item):
     can_change_reservation_times = UserRequestsCustomization.get_bool("adjustment_requests_missed_reservation_times")
```

### Comparing `NEMO-4.5.5/NEMO/views/alerts.py` & `NEMO-4.6.0/NEMO/views/alerts.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/views/api.py` & `NEMO-4.6.0/NEMO/views/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,25 +118,26 @@
 		"id": ["exact", "in"],
 		"type": ["exact", "in"],
 		"domain": ["exact", "in", "isempty"],
 		"username": ["iexact", "in"],
 		"first_name": ["iexact", "icontains"],
 		"last_name": ["iexact", "icontains"],
 		"email": ["iexact", "icontains"],
-		"badge_number": ["exact"],
+		"badge_number": ["iexact", "isempty"],
 		"is_active": ["exact"],
 		"is_staff": ["exact"],
 		"is_facility_manager": ["exact"],
 		"is_superuser": ["exact"],
 		"is_service_personnel": ["exact"],
 		"is_technician": ["exact"],
 		"training_required": ["exact"],
 		"date_joined": ["month", "year", "day", "gte", "gt", "lte", "lt"],
 		"last_login": ["month", "year", "day", "gte", "gt", "lte", "lt", "isnull"],
 		"access_expiration": ["month", "year", "day", "gte", "gt", "lte", "lt", "isnull"],
+		"physical_access_levels": ["exact"],
 	}
 
 
 class ProjectDisciplineViewSet(ModelViewSet):
 	filename = "project_disciplines"
 	queryset = ProjectDiscipline.objects.all()
 	serializer_class = ProjectDisciplineSerializer
@@ -156,22 +157,22 @@
 	}
 
 
 class AccountTypeViewSet(ModelViewSet):
 	filename = "account_types"
 	queryset = AccountType.objects.all()
 	serializer_class = AccountTypeSerializer
-	filterset_fields = {"id": ["exact", "in"], "name": ["iexact"], "display_order": ["exact"]}
+	filterset_fields = {"id": ["exact", "in"], "name": ["exact", "iexact"], "display_order": ["exact"]}
 
 
 class AccountViewSet(ModelViewSet):
 	filename = "accounts"
 	queryset = Account.objects.all()
 	serializer_class = AccountSerializer
-	filterset_fields = {"id": ["exact", "in"], "name": ["iexact"], "active": ["exact"]}
+	filterset_fields = {"id": ["exact", "in"], "name": ["exact", "iexact"], "active": ["exact"]}
 
 
 class ToolViewSet(ModelViewSet):
 	filename = "tools"
 	queryset = Tool.objects.all()
 	serializer_class = ToolSerializer
 	filterset_fields = {
```

### Comparing `NEMO-4.5.5/NEMO/views/api_billing.py` & `NEMO-4.6.0/NEMO/views/api_billing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from datetime import datetime, timedelta
 from decimal import Decimal
 from typing import List, Optional
 
 from django import forms
-from django.db.models import QuerySet
 
 from NEMO.models import (
 	AreaAccessRecord,
 	ConsumableWithdraw,
 	Project,
 	Reservation,
 	StaffCharge,
 	TrainingSession,
 	UsageEvent,
 	User,
 )
+from NEMO.typing import QuerySetType
 from NEMO.utilities import localize
 
 
 class BillingFilterForm(forms.Form):
 	start = forms.DateField(required=True)
 	end = forms.DateField(required=True)
 	username = forms.CharField(required=False)
@@ -183,96 +183,96 @@
 	if billing_form.get_application_name():
 		queryset = queryset.filter(project__application_identifier=billing_form.get_application_name())
 	if billing_form.get_username():
 		queryset = queryset.filter(trainee__username=billing_form.get_username())
 	return billable_items_training_sessions(queryset)
 
 
-def billable_items_usage_events(usage_events: QuerySet) -> List[BillableItem]:
+def billable_items_usage_events(usage_events: QuerySetType[UsageEvent]) -> List[BillableItem]:
 	billable_items: List[BillableItem] = []
-	usage_event: UsageEvent
 	for usage_event in usage_events:
 		item = BillableItem("tool_usage", usage_event.project, usage_event.user)
 		item.name = usage_event.tool.name
+		item.item_id = usage_event.id
 		item.details = (
 			f"Work performed by {usage_event.operator} on user's behalf"
 			if usage_event.operator != usage_event.user
 			else ""
 		)
 		item.start = usage_event.start
 		item.end = usage_event.end
 		item.quantity = get_minutes_between_dates(usage_event.start, usage_event.end)
 		billable_items.append(item)
 	return billable_items
 
 
-def billable_items_area_access_records(area_access_records: QuerySet) -> List[BillableItem]:
+def billable_items_area_access_records(area_access_records: QuerySetType[AreaAccessRecord]) -> List[BillableItem]:
 	billable_items: List[BillableItem] = []
-	area_access_record: AreaAccessRecord
 	for area_access_record in area_access_records:
 		item = BillableItem("area_access", area_access_record.project, area_access_record.customer)
 		item.name = area_access_record.area.name
+		item.item_id = area_access_record.id
 		item.details = (
 			f"Area accessed by {area_access_record.staff_charge.staff_member} on user's behalf"
 			if area_access_record.staff_charge
 			else ""
 		)
 		item.start = area_access_record.start
 		item.end = area_access_record.end
 		item.quantity = get_minutes_between_dates(area_access_record.start, area_access_record.end)
 		billable_items.append(item)
 	return billable_items
 
 
-def billable_items_consumable_withdrawals(withdrawals: QuerySet) -> List[BillableItem]:
+def billable_items_consumable_withdrawals(withdrawals: QuerySetType[ConsumableWithdraw]) -> List[BillableItem]:
 	billable_items: List[BillableItem] = []
-	consumable_withdrawal: ConsumableWithdraw
 	for consumable_withdrawal in withdrawals:
 		item = BillableItem("consumable", consumable_withdrawal.project, consumable_withdrawal.customer)
 		item.name = consumable_withdrawal.consumable.name
+		item.item_id = consumable_withdrawal.id
 		item.start = consumable_withdrawal.date
 		item.end = consumable_withdrawal.date
 		item.quantity = consumable_withdrawal.quantity
 		billable_items.append(item)
 	return billable_items
 
 
-def billable_items_missed_reservations(missed_reservations: QuerySet) -> List[BillableItem]:
+def billable_items_missed_reservations(missed_reservations: QuerySetType[Reservation]) -> List[BillableItem]:
 	billable_items: List[BillableItem] = []
-	missed_reservation: Reservation
 	for missed_reservation in missed_reservations:
 		item = BillableItem("missed_reservation", missed_reservation.project, missed_reservation.user)
 		item.name = missed_reservation.reservation_item.name
+		item.item_id = missed_reservation.id
 		item.start = missed_reservation.start
 		item.end = missed_reservation.end
 		item.quantity = 1
 		billable_items.append(item)
 	return billable_items
 
 
-def billable_items_staff_charges(staff_charges: QuerySet) -> List[BillableItem]:
+def billable_items_staff_charges(staff_charges: QuerySetType[StaffCharge]) -> List[BillableItem]:
 	billable_items: List[BillableItem] = []
-	staff_charge: StaffCharge
 	for staff_charge in staff_charges:
 		item = BillableItem("staff_charge", staff_charge.project, staff_charge.customer)
+		item.item_id = staff_charge.id
 		item.details = staff_charge.note
 		item.name = f"Work performed by {staff_charge.staff_member}"
 		item.start = staff_charge.start
 		item.end = staff_charge.end
 		item.quantity = get_minutes_between_dates(staff_charge.start, staff_charge.end)
 		billable_items.append(item)
 	return billable_items
 
 
-def billable_items_training_sessions(training_sessions: QuerySet) -> List[BillableItem]:
+def billable_items_training_sessions(training_sessions: QuerySetType[TrainingSession]) -> List[BillableItem]:
 	billable_items: List[BillableItem] = []
-	training_session: TrainingSession
 	for training_session in training_sessions:
 		item = BillableItem("training_session", training_session.project, training_session.trainee)
 		item.name = training_session.tool.name
+		item.item_id = training_session.id
 		item.details = f"{training_session.get_type_display()} training provided by {training_session.trainer}"
 		item.start = training_session.date
 		item.end = training_session.date
 		item.quantity = training_session.duration
 		billable_items.append(item)
 	return billable_items
```

### Comparing `NEMO-4.5.5/NEMO/views/api_file_import.py` & `NEMO-4.6.0/NEMO/views/api_file_import.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 from logging import getLogger
 
 import requests
-from django.contrib.auth.decorators import login_required
+from django.conf import settings
 from django.http import HttpResponse
 from django.shortcuts import redirect
 from django.views.decorators.csrf import csrf_exempt
 from django.views.decorators.http import require_http_methods
 from rest_framework.exceptions import NotFound
 
 from NEMO.utilities import get_full_url, render_combine_responses
 
 api_logger = getLogger(__name__)
 
 
 @require_http_methods(["GET", "POST"])
-@login_required
 @csrf_exempt
 def file_import(request):
 	if request.method == "GET":
 		return redirect("api-root")
 	url = None
+	headers = get_new_headers(request)
 	try:
 		url = get_full_url(request.POST["request_url"], request)
-		if "import_file" not in request.FILES:
+		import_file = request.FILES.get("import_file")
+		if not import_file:
 			raise NotFound("Please upload a file")
-		data = request.FILES.get("import_file").read()
-		response = requests.post(url, data, headers=get_new_headers(request))
+		data = import_file.read()
+		headers["Content-Type"] = import_file.content_type
+		response = requests.post(url, data, headers=headers, cookies=request.COOKIES, allow_redirects=False)
+		# Deal with potential redirect here by resubmitting
+		if response.status_code == 301:
+			response = requests.post(response.headers["Location"], data, headers=headers, cookies=request.COOKIES)
 		return HttpResponse(
 			response.content, status=response.status_code, content_type=response.headers["Content-Type"]
 		)
 	except Exception as e:
 		api_logger.exception("Error processing API file import")
 		if url:
 			# This is a bit of a hack to display an error message, using the OPTIONS request method and changing the content
 			status_code = getattr(e, "status_code", 400)
-			response = requests.options(url, headers=get_new_headers(request))
+			response = requests.options(url, headers=headers)
 			template_response = HttpResponse(
 				response.content, status=status_code, content_type=response.headers["Content-Type"]
 			)
 			context = {
 				"error": str(e),
 				"status_code": template_response.status_code,
 				"status_text": template_response.reason_phrase,
@@ -46,11 +51,15 @@
 			return render_combine_responses(request, template_response, "rest_framework/custom_error.html", context)
 		else:
 			raise
 
 
 def get_new_headers(request):
 	headers = {key: value for key, value in request.headers.items()}
-	headers["X-csrftoken"] = request.POST["csrfmiddlewaretoken"]
-	if "import_file" in request.FILES:
-		headers["Content-Type"] = request.FILES.get("import_file").content_type
+	# Put new csrf in the correct header
+	new_csrf = request.POST["csrfmiddlewaretoken"]
+	csrf_header_name = settings.CSRF_HEADER_NAME
+	if csrf_header_name.startswith("HTTP_"):
+		csrf_header_name = csrf_header_name[5:]
+	csrf_header_name = csrf_header_name.replace("_", "-")
+	headers[csrf_header_name] = new_csrf
 	return headers
```

### Comparing `NEMO-4.5.5/NEMO/views/area_access.py` & `NEMO-4.6.0/NEMO/views/area_access.py`

 * *Files 10% similar despite different names*

```diff
@@ -120,61 +120,58 @@
 
 			dictionary['user_accessible_areas'], dictionary['areas'] = load_areas_for_use_in_template(customer)
 			return render(request, 'area_access/new_area_access_record_details.html', dictionary)
 		except:
 			pass
 		return render(request, 'area_access/new_area_access_record.html', dictionary)
 	if request.method == 'POST':
+		record = AreaAccessRecord()
 		try:
-			user = User.objects.get(id=request.POST['customer'])
-			project = Project.objects.get(id=request.POST['project'])
-			area = Area.objects.get(id=request.POST['area'])
+			record.customer = User.objects.get(id=request.POST['customer'])
+			record.project = Project.objects.get(id=request.POST['project'])
+			record.area = Area.objects.get(id=request.POST['area'])
 		except:
 			dictionary['error_message'] = 'Your request contained an invalid identifier.'
 			return render(request, 'area_access/new_area_access_record.html', dictionary)
 		try:
-			error_message = check_policy_for_user(customer=user)
+			error_message = check_policy_for_user(customer=record.customer)
 			if error_message:
 				dictionary['error_message'] = error_message
 				return render(request, 'area_access/new_area_access_record.html', dictionary)
-			policy.check_billing_to_project(project, user, area)
-			policy.check_to_enter_area(area=area, user=user)
+			policy.check_billing_to_project(record.project, record.customer, record.area, record)
+			policy.check_to_enter_area(area=record.area, user=record.customer)
 		except ProjectChargeException as e:
 			dictionary['error_message'] = e.msg
 			return render(request, 'area_access/new_area_access_record.html', dictionary)
 		except NoAccessiblePhysicalAccessUserError as error:
 			if error.closure_time:
-				dictionary['error_message'] = '{} does not have access to the {} at this time due to the following closure: {}.'.format(user, area.name, error.closure_time.closure.name)
+				dictionary['error_message'] = '{} does not have access to the {} at this time due to the following closure: {}.'.format(record.customer, record.area.name, error.closure_time.closure.name)
 			else:
-				dictionary['error_message'] = '{} does not have a physical access level that allows access to the {} at this time.'.format(user, area.name)
+				dictionary['error_message'] = '{} does not have a physical access level that allows access to the {} at this time.'.format(record.customer, record.area.name)
 			return render(request, 'area_access/new_area_access_record.html', dictionary)
 		except UnavailableResourcesUserError as error:
 			dictionary['error_message'] = 'The {} is inaccessible because a required resource ({}) is unavailable. You must make all required resources for this area available before creating a new area access record.'.format(error.area.name, error.resources[0])
 			return render(request, 'area_access/new_area_access_record.html', dictionary)
 		except MaximumCapacityReachedError as error:
-			dictionary['error_message'] = 'The {} is inaccessible because the {} has reached its maximum capacity. Wait for somebody to exit and try again.'.format(area.name, error.area.name)
+			dictionary['error_message'] = 'The {} is inaccessible because the {} has reached its maximum capacity. Wait for somebody to exit and try again.'.format(record.area.name, error.area.name)
 			return render(request, 'area_access/new_area_access_record.html', dictionary)
 		except ScheduledOutageInProgressError as error:
 			dictionary['error_message'] = 'The {} is inaccessible because a scheduled outage is in effect. You must wait for the outage to end before creating a new area access record.'.format(error.area.name)
 			return render(request, 'area_access/new_area_access_record.html', dictionary)
 		except ReservationRequiredUserError:
-			dictionary['error_message'] = 'You do not have a current reservation for the {}. Please make a reservation before trying to access this area.'.format(area.name)
+			dictionary['error_message'] = 'You do not have a current reservation for the {}. Please make a reservation before trying to access this area.'.format(record.area.name)
 			return render(request, 'area_access/new_area_access_record.html', dictionary)
-		if user.billing_to_project():
-			dictionary['error_message'] = '{} is already billing area access to another area. The user must log out of that area before entering another.'.format(user)
+		if record.customer.billing_to_project():
+			dictionary['error_message'] = '{} is already billing area access to another area. The user must log out of that area before entering another.'.format(record.customer)
 			return render(request, 'area_access/new_area_access_record.html', dictionary)
-		if project not in user.active_projects():
-			dictionary['error_message'] = '{} is not authorized to bill that project.'.format(user)
+		if record.project not in record.customer.active_projects():
+			dictionary['error_message'] = '{} is not authorized to bill that project.'.format(record.customer)
 			return render(request, 'area_access/new_area_access_record.html', dictionary)
-		record = AreaAccessRecord()
-		record.area = area
-		record.customer = user
-		record.project = project
 		record.save()
-		dictionary['success'] = '{} is now logged in to the {}.'.format(user, area.name)
+		dictionary['success'] = '{} is now logged in to the {}.'.format(record.customer, record.area.name)
 		return render(request, 'area_access/new_area_access_record.html', dictionary)
 
 
 def check_policy_for_user(customer: User):
 	error_message = None
 	try:
 		policy.check_to_enter_any_area(user=customer)
@@ -214,15 +211,15 @@
 		}
 		return render(request, 'area_access/change_project.html', dictionary)
 	# If we're already billing the requested project then there's nothing to do.
 	if old_project.id == new_project:
 		return redirect(reverse('landing'))
 	new_project = get_object_or_404(Project, id=new_project)
 	try:
-		policy.check_billing_to_project(new_project, user, user.area_access_record().area)
+		policy.check_billing_to_project(new_project, user, user.area_access_record().area, user.area_access_record())
 	except ProjectChargeException as e:
 		dictionary = {
 			'error': e.msg
 		}
 		return render(request, 'area_access/change_project.html', dictionary)
 	# Stop billing the user's initial project
 	record = user.area_access_record()
@@ -304,15 +301,15 @@
 	if request.method == 'GET':
 		return render(request, 'area_access/self_login.html', dictionary)
 	if request.method == 'POST':
 		try:
 			a = Area.objects.get(id=request.POST['area'])
 			p = Project.objects.get(id=request.POST['project'])
 			policy.check_to_enter_area(a, request.user)
-			policy.check_billing_to_project(p, user, a)
+			policy.check_billing_to_project(p, user, a, AreaAccessRecord(customer=user, project=p, area=a))
 			log_in_user_to_area(a, request.user, p)
 		except ProjectChargeException as e:
 			dictionary['area_error_message'] = e.msg
 			return render(request, 'area_access/self_login.html', dictionary)
 		except NoAccessiblePhysicalAccessUserError as error:
 			if error.closure_time:
 				dictionary['area_error_message'] = f"You do not have access to the {error.area.name} at this time due to the following closure: {error.closure_time.closure.name}. The closure ends on {localize(error.closure_time.end_time.astimezone(timezone.get_current_timezone()))}"
```

### Comparing `NEMO-4.5.5/NEMO/views/authentication.py` & `NEMO-4.6.0/NEMO/views/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from _ssl import CERT_REQUIRED, PROTOCOL_TLSv1_2
 from base64 import b64decode
 from logging import getLogger
+from urllib.parse import urljoin, urlparse
 
 from django.conf import settings
 from django.contrib.auth import REDIRECT_FIELD_NAME, authenticate, get_backends, login
 from django.contrib.auth.backends import ModelBackend
 from django.contrib.auth.middleware import RemoteUserMiddleware
 from django.http import HttpResponse, HttpResponseForbidden, HttpResponseRedirect
 from django.shortcuts import redirect, render
@@ -261,15 +262,15 @@
 		except (User.DoesNotExist, InactiveUserError):
 			return redirect('authorization_failed')
 
 		if user:
 			login(request, user)
 			try:
 				next_page = request.GET[REDIRECT_FIELD_NAME]
-				resolve(next_page)  # Make sure the next page is a legitimate URL for NEMO
+				resolve(urljoin(next_page, urlparse(next_page).path))  # Make sure the next page is a legitimate URL for NEMO
 			except:
 				next_page = reverse("landing")
 			return HttpResponseRedirect(next_page)
 		dictionary["user_name_or_password_incorrect"] = True
 		return render(request, "login.html", dictionary)
```

### Comparing `NEMO-4.5.5/NEMO/views/buddy_requests.py` & `NEMO-4.6.0/NEMO/views/buddy_requests.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/views/calendar.py` & `NEMO-4.6.0/NEMO/views/calendar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-import io
 from datetime import date, datetime, timedelta
 from http import HTTPStatus
 from json import dumps, loads
 from logging import getLogger
 from re import match
 from typing import Dict, Iterable, List, Optional, Union
 
-import pytz
-from django.conf import settings
 from django.contrib.auth.decorators import login_required, permission_required
 from django.core.exceptions import ValidationError
 from django.db.models import Q
 from django.http import HttpResponse, HttpResponseBadRequest, HttpResponseForbidden, HttpResponseNotFound
 from django.shortcuts import get_object_or_404, redirect, render
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.safestring import mark_safe
+from django.utils.timezone import make_aware
 from django.views.decorators.http import require_GET, require_POST
 
-from NEMO.decorators import disable_session_expiry_refresh, staff_member_required, synchronized
+from NEMO.decorators import disable_session_expiry_refresh, postpone, staff_member_required, synchronized
 from NEMO.exceptions import ProjectChargeException, RequiredUnansweredQuestionsException
 from NEMO.forms import nice_errors
 from NEMO.models import (
 	Alert,
 	Area,
 	AreaAccessRecord,
 	Closure,
@@ -36,25 +34,27 @@
 	ReservationItemType,
 	ReservationQuestions,
 	ScheduledOutage,
 	ScheduledOutageCategory,
 	StaffCharge,
 	Tool,
 	UsageEvent,
-	User,
+	User, UserPreferences,
 )
 from NEMO.policy import policy_class as policy
 from NEMO.utilities import (
 	EmailCategory,
 	RecurrenceFrequency,
 	as_timezone,
 	beginning_of_the_day,
 	bootstrap_primary_color,
-	create_email_attachment,
+	create_ics,
 	date_input_format,
+	datetime_input_format,
+	distinct_qs_value_list,
 	extract_times,
 	format_datetime,
 	get_email_from_settings,
 	get_full_url,
 	get_recurring_rule,
 	localize,
 	parse_parameter_string,
@@ -411,15 +411,15 @@
 				return render(request, 'calendar/project_choice.html', {
 					'active_projects': active_projects,
 					'missed_reservation_threshold': new_reservation.reservation_item.missed_reservation_threshold
 				})
 
 		# Check if we are allowed to bill to project
 		try:
-			policy.check_billing_to_project(new_reservation.project, user, new_reservation.reservation_item)
+			policy.check_billing_to_project(new_reservation.project, user, new_reservation.reservation_item, new_reservation)
 		except ProjectChargeException as e:
 			policy_problems.append(e.msg)
 			return render(request, 'calendar/policy_dialog.html', {'policy_problems': policy_problems, 'overridable': False, 'reservation_action': 'create'})
 
 	# Reservation questions if applicable
 	reservation_questions = render_reservation_questions(item_type, item_id, new_reservation.project)
 	if reservation_questions:
@@ -676,14 +676,15 @@
 		reservation_action = "resize" if start_delta is None else "move"
 		return render(request, 'calendar/policy_dialog.html', {'policy_problems': policy_problems, 'overridable': overridable and request.user.is_staff, 'reservation_action': reservation_action})
 	else:
 		# All policy checks passed, so save the reservation.
 		new_reservation.save_and_notify()
 		reservation_to_cancel.descendant = new_reservation
 		reservation_to_cancel.save_and_notify()
+		send_tool_free_time_notification(request, reservation_to_cancel, new_reservation)
 	return reservation_success(request, new_reservation)
 
 
 def modify_outage(request, start_delta, end_delta):
 	try:
 		outage = ScheduledOutage.objects.get(pk=request.POST.get('id'))
 	except ScheduledOutage.DoesNotExist:
@@ -704,15 +705,15 @@
 @require_POST
 def cancel_reservation(request, reservation_id):
 	""" Cancel a reservation for a user. """
 	reservation = get_object_or_404(Reservation, id=reservation_id)
 
 	reason = parse_parameter_string(request.POST, 'reason')
 	response = cancel_the_reservation(reservation=reservation, user_cancelling_reservation=request.user, reason=reason, request=request)
-
+	send_tool_free_time_notification(request, reservation)
 	if request.device == 'desktop':
 		return response
 	if request.device == 'mobile':
 		if response.status_code == HTTPStatus.OK:
 			return render(request, 'mobile/cancellation_result.html', {'event_type': 'Reservation', 'tool': reservation.tool})
 		else:
 			return render(request, 'mobile/error.html', {'message': response.content})
@@ -738,20 +739,50 @@
 	reservation.title = request.POST.get('title', '')[:reservation._meta.get_field('title').max_length]
 	reservation.save()
 	return HttpResponse()
 
 
 @login_required
 @require_POST
+def change_reservation_date(request):
+	""" Change a reservation's start or end date for a user. """
+	reservation = get_object_or_404(Reservation, id=request.POST['id'])
+	start_delta, end_delta = None, None
+	new_start = request.POST.get('new_start', None)
+	if new_start:
+		try:
+			new_start = make_aware(datetime.strptime(new_start, datetime_input_format))
+			if new_start.time().minute not in [0, 15, 30, 45]:
+				return HttpResponseBadRequest("Reservation time only works with 15 min increments")
+		except ValueError:
+			return HttpResponseBadRequest("Invalid date format for start date")
+		start_delta = (new_start - reservation.start)
+	new_end = request.POST.get('new_end', None)
+	if new_end:
+		try:
+			new_end = make_aware(datetime.strptime(new_end, datetime_input_format))
+			if new_end.time().minute not in [0, 15, 30, 45]:
+				return HttpResponseBadRequest("Reservation time only works with 15 min increments")
+		except ValueError:
+			return HttpResponseBadRequest("Invalid date format for end date")
+		end_delta = (new_end - reservation.end) if new_end else None
+	if start_delta or end_delta:
+		return modify_reservation(request, request.user, start_delta, end_delta)
+	else:
+		return HttpResponseBadRequest('Invalid delta')
+
+
+@login_required
+@require_POST
 def change_reservation_project(request, reservation_id):
 	""" Change reservation project for a user. """
 	reservation = get_object_or_404(Reservation, id=reservation_id)
 	project = get_object_or_404(Project, id=request.POST['project_id'])
 	try:
-		policy.check_billing_to_project(project, reservation.user, reservation.reservation_item)
+		policy.check_billing_to_project(project, reservation.user, reservation.reservation_item, reservation)
 	except ProjectChargeException as e:
 		return HttpResponseBadRequest(e.msg)
 
 	if (request.user.is_staff or request.user == reservation.user) and \
 		reservation.has_not_ended() and reservation.has_not_started() and \
 		project in reservation.user.active_projects():
 		reservation.project = project
@@ -1060,23 +1091,23 @@
 	reservation_questions = get_and_combine_reservation_questions(item_type, item_id, project)
 	reservation_questions_json = []
 	for reservation_question in reservation_questions:
 		reservation_questions_json.extend(loads(reservation_question.questions))
 	return DynamicForm(dumps(reservation_questions_json)).extract(request) if len(reservation_questions_json) else ""
 
 
-def shorten_reservation(user: User, item: Union[Area, Tool], new_end: datetime = None):
+def shorten_reservation(user: User, item: Union[Area, Tool], new_end: datetime = None, force=False):
 	try:
 		if new_end is None:
 			new_end = timezone.now()
 		current_reservation_qs = Reservation.objects.filter(start__lt=timezone.now(), end__gt=timezone.now(),
 															cancelled=False, missed=False, shortened=False, user=user)
 		current_reservation = current_reservation_qs.get(**{ReservationItemType.from_item(item).value: item})
 		# Staff are exempt from mandatory reservation shortening.
-		if user.is_staff is False:
+		if user.is_staff is False or force:
 			new_reservation = current_reservation.copy(new_end=new_end)
 			new_reservation.save()
 			current_reservation.shortened = True
 			current_reservation.descendant = new_reservation
 			current_reservation.save()
 	except Reservation.DoesNotExist:
 		pass
@@ -1114,15 +1145,18 @@
 					'template_color': bootstrap_primary_color('info')
 				}
 				cancellation_email = render_email_template(email_contents, dictionary, request)
 				recipients = reservation.user.get_emails(reservation.user.get_preferences().email_send_reservation_emails)
 				if reservation.area:
 					recipients.extend(reservation.area.reservation_email_list())
 				if reservation.user.get_preferences().attach_cancelled_reservation:
-					attachment = create_ics_for_reservation(reservation, cancelled=True)
+					event_name = f"{reservation.reservation_item.name} Reservation"
+					attachment = create_ics(reservation.id, event_name, reservation.start, reservation.end,
+											reservation.user,
+											cancelled=True)
 					send_mail(subject='Your reservation was cancelled', content=cancellation_email, from_email=user_cancelling_reservation.email, to=recipients, attachments=[attachment])
 				else:
 					send_mail(subject='Your reservation was cancelled', content=cancellation_email, from_email=user_cancelling_reservation.email, to=recipients)
 
 		else:
 			''' here the user cancelled his own reservation so notify him '''
 			reservation.save_and_notify()
@@ -1155,74 +1189,52 @@
 		recipients.extend(reservation.area.abuse_email_list())
 		send_mail(subject=subject, content=message, from_email=user_office_email, to=recipients, email_category=EmailCategory.TIMED_SERVICES)
 	else:
 		calendar_logger.error("Out of time reservation email couldn't be send because out_of_time_reservation_email.html or user_office_email are not defined")
 
 
 def send_user_created_reservation_notification(reservation: Reservation):
-	site_title = ApplicationCustomization.get('site_title')
 	user = reservation.user
 	recipients = user.get_emails(user.get_preferences().email_send_reservation_emails) if user.get_preferences().attach_created_reservation else []
 	if reservation.area:
 		recipients.extend(reservation.area.reservation_email_list())
 	if recipients:
-		subject = f"[{site_title}] Reservation for the " + str(reservation.reservation_item)
+		subject = f"Reservation for the " + str(reservation.reservation_item)
 		message = get_media_file_contents('reservation_created_user_email.html')
 		message = render_email_template(message, {'reservation': reservation})
 		user_office_email = EmailsCustomization.get('user_office_email_address')
 		# We don't need to check for existence of reservation_created_user_email because we are attaching the ics reservation and sending the email regardless (message will be blank)
 		if user_office_email:
-			attachment = create_ics_for_reservation(reservation)
+			event_name = f"{reservation.reservation_item.name} Reservation"
+			attachment = create_ics(reservation.id, event_name, reservation.start, reservation.end, reservation.user)
 			send_mail(subject=subject, content=message, from_email=user_office_email, to=recipients, attachments=[attachment])
 		else:
 			calendar_logger.error("User created reservation notification could not be send because user_office_email_address is not defined")
 
 
 def send_user_cancelled_reservation_notification(reservation: Reservation):
-	site_title = ApplicationCustomization.get('site_title')
 	user = reservation.user
 	recipients = user.get_emails(user.get_preferences().email_send_reservation_emails) if user.get_preferences().attach_cancelled_reservation else []
 	if reservation.area:
 		recipients.extend(reservation.area.reservation_email_list())
 	if recipients:
-		subject = f"[{site_title}] Cancelled Reservation for the " + str(reservation.reservation_item)
+		subject = f"Cancelled Reservation for the " + str(reservation.reservation_item)
 		message = get_media_file_contents('reservation_cancelled_user_email.html')
 		message = render_email_template(message, {'reservation': reservation})
 		user_office_email = EmailsCustomization.get('user_office_email_address')
 		# We don't need to check for existence of reservation_cancelled_user_email because we are attaching the ics reservation and sending the email regardless (message will be blank)
 		if user_office_email:
-			attachment = create_ics_for_reservation(reservation, cancelled=True)
+			event_name = f"{reservation.reservation_item.name} Reservation"
+			attachment = create_ics(reservation.id, event_name, reservation.start, reservation.end, reservation.user,
+							  cancelled=True)
 			send_mail(subject=subject, content=message, from_email=user_office_email, to=recipients, attachments=[attachment])
 		else:
 			calendar_logger.error("User cancelled reservation notification could not be send because user_office_email_address is not defined")
 
 
-def create_ics_for_reservation(reservation: Reservation, cancelled=False):
-	site_title = ApplicationCustomization.get('site_title')
-	reservation_organizer_email = getattr(settings, "RESERVATION_ORGANIZER_EMAIL", "no_reply")
-	reservation_organizer = getattr(settings, "RESERVATION_ORGANIZER", site_title)
-	method_name = 'CANCEL' if cancelled else 'REQUEST'
-	method = f'METHOD:{method_name}\n'
-	status = 'STATUS:CANCELLED\n' if cancelled else 'STATUS:CONFIRMED\n'
-	uid = 'UID:'+str(reservation.id)+'\n'
-	sequence = 'SEQUENCE:2\n' if cancelled else 'SEQUENCE:0\n'
-	priority = 'PRIORITY:5\n' if cancelled else 'PRIORITY:0\n'
-	now = datetime.utcnow().strftime('%Y%m%dT%H%M%SZ')
-	start = reservation.start.astimezone(pytz.utc).strftime('%Y%m%dT%H%M%SZ')
-	end = reservation.end.astimezone(pytz.utc).strftime('%Y%m%dT%H%M%SZ')
-	reservation_name = reservation.reservation_item.name
-	lines = ['BEGIN:VCALENDAR\n', 'VERSION:2.0\n', method, 'BEGIN:VEVENT\n', uid, sequence, priority, f'DTSTAMP:{now}\n', f'DTSTART:{start}\n', f'DTEND:{end}\n', f'ATTENDEE;CN="{reservation.user.get_name()}";RSVP=TRUE:mailto:{reservation.user.email}\n', f'ORGANIZER;CN="{reservation_organizer}":mailto:{reservation_organizer_email}\n', f'SUMMARY:[{site_title}] {reservation_name} Reservation\n', status, 'END:VEVENT\n', 'END:VCALENDAR\n']
-	ics = io.StringIO('')
-	ics.writelines(lines)
-	ics.seek(0)
-
-	attachment = create_email_attachment(ics, maintype='text', subtype='calendar', method=method_name)
-	return attachment
-
-
 @login_required
 @require_GET
 @permission_required("NEMO.trigger_timed_services", raise_exception=True)
 def create_closure_alerts(request):
 	return do_create_closure_alerts()
 
 
@@ -1317,20 +1329,21 @@
 	qualification_expiration_days = ToolCustomization.get("tool_qualification_expiration_days")
 	qualification_expiration_never_used = ToolCustomization.get("tool_qualification_expiration_never_used_days")
 	template = get_media_file_contents("tool_qualification_expiration_email.html")
 	if user_office_email and template:
 		if qualification_expiration_days or qualification_expiration_never_used:
 			qualification_expiration_days = quiet_int(qualification_expiration_days, None)
 			qualification_expiration_never_used = quiet_int(qualification_expiration_never_used, None)
-			for qualification in Qualification.objects.filter(user__is_active=True, user__is_staff=False):
+			for qualification in Qualification.objects.filter(user__is_active=True, user__is_staff=False, tool___qualifications_never_expire=False).prefetch_related("tool", "user"):
 				user = qualification.user
 				tool = qualification.tool
 				last_tool_use = None
 				try:
-					last_tool_use = as_timezone(UsageEvent.objects.filter(user=user, tool=tool).latest("start").start).date()
+					# Last tool use cannot be before the last time they qualified
+					last_tool_use = max(as_timezone(UsageEvent.objects.filter(user=user, tool=tool).latest("start").start).date(), qualification.qualified_on)
 					expiration_date: date = last_tool_use + timedelta(days=qualification_expiration_days) if qualification_expiration_days else None
 				except UsageEvent.DoesNotExist:
 					# User never used the tool, use the qualification date
 					expiration_date: date = qualification.qualified_on + timedelta(days=qualification_expiration_never_used) if qualification_expiration_never_used else None
 				if expiration_date:
 					if expiration_date <= date.today():
 						qualification.delete()
@@ -1425,7 +1438,48 @@
 	if message and user_office_email:
 		for user_reminders in reminders:
 			subject = f"{recurring_charges_name} will be charged in {user_reminders['reminder_days']} day(s)"
 			user_instance: User = user_reminders["user"]
 			rendered_message = render_email_template(message, user_reminders, request)
 			email_notification = user_instance.get_preferences().email_send_recurring_charges_reminder_emails
 			user_instance.email_user(subject=subject, message=rendered_message, from_email=user_office_email, email_category=EmailCategory.TIMED_SERVICES, email_notification=email_notification)
+
+
+@postpone
+def send_tool_free_time_notification(request, cancelled_reservation: Reservation, new_reservation: Optional[Reservation] = None):
+	tool = cancelled_reservation.tool
+	if tool and cancelled_reservation.start > timezone.now():
+		max_duration = cancelled_reservation.duration().total_seconds() / 60
+		freed_time = None
+		start_time = None
+		days_in_the_future = (cancelled_reservation.start - timezone.now()).total_seconds() / 3600 / 24
+		if not new_reservation:
+			# this is a cancel action, we only have to take into account the cancelled time
+			freed_time = max_duration
+			start_time = cancelled_reservation.start
+		else:
+			# this is a modification (move or resize)
+			end_diff = (cancelled_reservation.end - new_reservation.end).total_seconds() / 60
+			if cancelled_reservation.start == new_reservation.start and end_diff > 0:
+				# reservation was shrunk
+				freed_time = end_diff
+				start_time = cancelled_reservation.end - timedelta(minutes=end_diff)
+			elif cancelled_reservation.start != new_reservation.start:
+				# reservation was moved
+				freed_time = min(max_duration, abs(end_diff))
+				start_time = (cancelled_reservation.end - timedelta(minutes=freed_time)) if end_diff > 0 else cancelled_reservation.start
+		if freed_time and start_time:
+			tool_notifications = UserPreferences.objects.filter(tool_freed_time_notifications__in=[tool], tool_freed_time_notifications_min_time__lte=freed_time, tool_freed_time_notifications_max_future_days__gte=days_in_the_future)
+			formatted_start = format_datetime(start_time)
+			formatted_time = f"{freed_time:0.0f}"
+			link = get_full_url(reverse("calendar"), request)
+			user_ids = distinct_qs_value_list(tool_notifications, "user")
+			for user in User.objects.in_bulk(user_ids).values():
+				if user != cancelled_reservation.user:
+					subject = f"[{tool.name}] {formatted_time} minutes freed starting {formatted_start}"
+					message = f"Dear {user.first_name},<br>\n"
+					message += f"The following time slot has been freed for the {tool.name}:<br><br>\n\n"
+					message += f"Start: {formatted_start}<br>\n"
+					message += f"End: {format_datetime(start_time + timedelta(minutes=freed_time))}<br>\n"
+					message += f"Duration: {formatted_time} minutes<br><br>\n\n"
+					message += f'Go to the <a href={link} target="_blank">calendar</a> to make a reservation.<br>\n'
+					user.email_user(subject=subject, message=message, from_email=get_email_from_settings(), email_notification=user.get_preferences().email_send_reservation_emails)
```

### Comparing `NEMO-4.5.5/NEMO/views/charge_validation.py` & `NEMO-4.6.0/NEMO/views/charge_validation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from django.http import HttpResponse
 from django.shortcuts import get_object_or_404
 from django.views.decorators.http import require_POST
 
 from NEMO.decorators import staff_member_required
-from NEMO.models import StaffCharge, UsageEvent, AreaAccessRecord, Reservation, TrainingSession, ConsumableWithdraw
+from NEMO.models import AreaAccessRecord, ConsumableWithdraw, Reservation, StaffCharge, TrainingSession, UsageEvent
 
 
 @staff_member_required
 @require_POST
 def validate_staff_charge(request, staff_charge_id):
     staff_charge = get_object_or_404(StaffCharge, id=staff_charge_id)
     staff_charge.validated = True
     staff_charge.validated_by = request.user
     staff_charge.save()
+    # Validate associated area access records
+    for area_access_record in staff_charge.areaaccessrecord_set.all():
+        validate_area_access_record(request, area_access_record.id)
     return HttpResponse()
 
 
 @staff_member_required
 @require_POST
 def validate_usage_event(request, usage_event_id):
     usage_event = get_object_or_404(UsageEvent, id=usage_event_id)
```

### Comparing `NEMO-4.5.5/NEMO/views/configuration_agenda.py` & `NEMO-4.6.0/NEMO/views/configuration_agenda.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/views/consumables.py` & `NEMO-4.6.0/NEMO/views/consumables.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,80 @@
 from datetime import date
 from logging import getLogger
 from typing import List
 
 from django.contrib import messages
+from django.contrib.auth.decorators import login_required, user_passes_test
 from django.http import HttpResponseBadRequest
 from django.shortcuts import get_object_or_404, redirect, render
 from django.utils.text import slugify
 from django.views.decorators.http import require_GET, require_POST, require_http_methods
 
-from NEMO.decorators import staff_member_or_user_office_required, user_office_or_manager_required
+from NEMO.decorators import user_office_or_manager_required
 from NEMO.exceptions import ProjectChargeException
 from NEMO.forms import ConsumableWithdrawForm, RecurringConsumableChargeForm
 from NEMO.models import Consumable, ConsumableWithdraw, RecurringConsumableCharge, User
 from NEMO.policy import policy_class as policy
 from NEMO.utilities import (
 	BasicDisplayTable,
 	EmailCategory,
 	as_timezone,
 	export_format_datetime,
 	format_datetime,
 	queryset_search_filter, render_email_template,
 	send_mail,
 )
-from NEMO.views.customization import EmailsCustomization, RecurringChargesCustomization, get_media_file_contents
+from NEMO.views.customization import (
+	ApplicationCustomization,
+	EmailsCustomization,
+	RecurringChargesCustomization,
+	get_media_file_contents,
+)
 from NEMO.views.pagination import SortedPaginator
 
 consumables_logger = getLogger(__name__)
 
 
-@staff_member_or_user_office_required
+def consumable_permissions(user):
+	user_allowed = ApplicationCustomization.get_bool("consumable_user_self_checkout")
+	return user.is_active and (user_allowed or user.is_staff or user.is_user_office or user.is_superuser)
+
+
+def self_checkout(user) -> bool:
+	return user.is_active and not (user.is_staff or user.is_user_office or user.is_superuser)
+
+
+@login_required
+@user_passes_test(consumable_permissions)
 @require_http_methods(["GET", "POST"])
 def consumables(request):
+	user: User = request.user
 	if request.method == "GET":
 		from NEMO.rates import rate_class
 
 		rate_dict = rate_class.get_consumable_rates(Consumable.objects.all())
 
 		dictionary = {
 			"users": User.objects.filter(is_active=True),
 			"consumables": Consumable.objects.filter(visible=True).order_by("category", "name"),
 			"rates": rate_dict,
+			"self_checkout": self_checkout(user),
 		}
+		if self_checkout(user):
+			dictionary["projects"] = user.active_projects()
 		return render(request, "consumables/consumables.html", dictionary)
 	elif request.method == "POST":
-		form = ConsumableWithdrawForm(request.POST)
+		updated_post_data = request.POST.copy()
+		if self_checkout(user):
+			updated_post_data.update({'customer': user.id})
+		form = ConsumableWithdrawForm(updated_post_data)
 		if form.is_valid():
 			withdraw = form.save(commit=False)
 			try:
-				policy.check_billing_to_project(withdraw.project, withdraw.customer, withdraw.consumable)
+				policy.check_billing_to_project(withdraw.project, withdraw.customer, withdraw.consumable, withdraw)
 			except ProjectChargeException as e:
 				return HttpResponseBadRequest(e.msg)
 			add_withdraw_to_session(request, withdraw)
 		else:
 			return HttpResponseBadRequest(form.errors.as_ul())
 		return render(request, "consumables/consumables_order.html")
 
@@ -69,45 +92,50 @@
 			"project_id": withdrawal.project_id,
 			"quantity": withdrawal.quantity,
 		}
 		withdrawals.append(withdrawal_dict)
 	request.session["withdrawals"] = withdrawals
 
 
-@staff_member_or_user_office_required
+@login_required
+@user_passes_test(consumable_permissions)
 @require_GET
 def remove_withdraw_at_index(request, index: str):
 	try:
 		index = int(index)
 		withdrawals: List = request.session.get("withdrawals")
 		if withdrawals:
 			del withdrawals[index]
 			request.session["withdrawals"] = withdrawals
 	except Exception as e:
 		consumables_logger.exception(e)
 	return render(request, "consumables/consumables_order.html")
 
 
-@staff_member_or_user_office_required
+@login_required
+@user_passes_test(consumable_permissions)
 @require_GET
 def clear_withdrawals(request):
 	if "withdrawals" in request.session:
 		del request.session["withdrawals"]
 	return render(request, "consumables/consumables_order.html")
 
 
-@staff_member_or_user_office_required
+@login_required
+@user_passes_test(consumable_permissions)
 @require_POST
 def make_withdrawals(request):
+	user: User = request.user
 	withdrawals: List = request.session.setdefault("withdrawals", [])
+	force_customer = user.id if self_checkout(user) else None
 	for withdraw in withdrawals:
 		make_withdrawal(
 			consumable_id=withdraw["consumable_id"],
 			merchant=request.user,
-			customer_id=withdraw["customer_id"],
+			customer_id=force_customer or withdraw["customer_id"],
 			quantity=withdraw["quantity"],
 			project_id=withdraw["project_id"],
 			request=request,
 		)
 	del request.session["withdrawals"]
 	return redirect("consumables")
 
@@ -226,21 +254,22 @@
 
 def extended_permissions(request) -> bool:
 	user: User = request.user
 	lock_charges = RecurringChargesCustomization.get_bool("recurring_charges_lock")
 	return not lock_charges or user.is_facility_manager or user.is_superuser
 
 
-def make_withdrawal(consumable_id: int, quantity: int, project_id: int, merchant: User, customer_id: int, request=None):
+def make_withdrawal(consumable_id: int, quantity: int, project_id: int, merchant: User, customer_id: int, tool_usage=False, request=None):
 	withdraw = ConsumableWithdraw.objects.create(
 		consumable_id=consumable_id,
 		quantity=quantity,
 		merchant=merchant,
 		customer_id=customer_id,
 		project_id=project_id,
+		tool_usage=tool_usage
 	)
 	if not withdraw.consumable.reusable:
 		# Only withdraw if it's an actual consumable (not reusable)
 		withdraw.consumable.quantity -= withdraw.quantity
 	withdraw.consumable.save()
 	# Only add notification message if request is present
 	if request:
```

### Comparing `NEMO-4.5.5/NEMO/views/customization.py` & `NEMO-4.6.0/NEMO/views/customization.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC
 from datetime import date, datetime
-from typing import Dict, Iterable
+from typing import Dict, Iterable, List
 
 from dateutil.relativedelta import relativedelta
 from django.contrib import messages
 from django.core.exceptions import ValidationError
 from django.core.files.storage import get_storage_class
 from django.core.validators import (
 	validate_comma_separated_integer_list,
@@ -16,15 +16,15 @@
 from django.template import Context, Template
 from django.utils import timezone
 from django.views.decorators.http import require_GET, require_POST
 
 from NEMO import init_admin_site
 from NEMO.decorators import administrator_required, customization
 from NEMO.exceptions import InvalidCustomizationException
-from NEMO.models import ConsumableCategory, Customization, Project, RecurringConsumableCharge
+from NEMO.models import BadgeReader, ConsumableCategory, Customization, Project, RecurringConsumableCharge
 from NEMO.utilities import RecurrenceFrequency, date_input_format, datetime_input_format, quiet_int
 
 
 class CustomizationBase(ABC):
 	_instances = {}
 	# Here we can place variables that we need in NEMO but don't need to be set in UI
 	variables = {"weekend_access_notification_last_sent": ""}
@@ -120,20 +120,34 @@
 	@classmethod
 	def get_date(cls, name: str, raise_exception=True) -> date:
 		str_date = cls.get(name, raise_exception)
 		if str_date:
 			return datetime.strptime(str_date, date_input_format).date()
 
 	@classmethod
-	def get_datetime(cls, name:str, raise_exception=True) -> datetime:
+	def get_datetime(cls, name: str, raise_exception=True) -> datetime:
 		str_datetime = cls.get(name, raise_exception)
 		if str_datetime:
 			return datetime.strptime(str_datetime, datetime_input_format)
 
 	@classmethod
+	def get_list(cls, name: str, raise_exception=True) -> List[str]:
+		return [item.strip() for item in cls.get(name, raise_exception).split(",") if item]
+
+	@classmethod
+	def get_list_int(cls, name: str, raise_exception=True) -> List[int]:
+		result = []
+		for item in cls.get_list(name, raise_exception):
+			if item:
+				integer = quiet_int(item.strip(), None)
+				if integer:
+					result.append(integer)
+		return result
+
+	@classmethod
 	def set(cls, name: str, value):
 		if name not in cls.variables:
 			raise InvalidCustomizationException(name, value)
 		if value:
 			Customization.objects.update_or_create(name=name, defaults={"value": value})
 		else:
 			try:
@@ -146,16 +160,24 @@
 class ApplicationCustomization(CustomizationBase):
 	variables = {
 		"facility_name": "Facility",
 		"site_title": "NEMO",
 		"self_log_in": "",
 		"self_log_out": "",
 		"calendar_login_logout": "",
+		"area_logout_already_logged_in": "",
+		"default_badge_reader_id": "",
+		"consumable_user_self_checkout": "",
 	}
 
+	def context(self) -> Dict:
+		context_dict = super().context()
+		context_dict["badge_readers"] = BadgeReader.objects.all()
+		return context_dict
+
 	def save(self, request, element=None):
 		errors = super().save(request, element)
 		init_admin_site()
 		return errors
 
 
 @customization(key="projects_and_accounts", title="Projects & accounts")
@@ -223,15 +245,15 @@
 		"calendar_start_of_the_day": "07:00:00",
 		"calendar_now_indicator": "",
 		"calendar_display_not_qualified_areas": "",
 		"calendar_all_tools": "",
 		"calendar_all_areas": "",
 		"calendar_all_areastools": "",
 		"calendar_outage_recurrence_limit": "90",
-		"calendar_qualified_tools": ""
+		"calendar_qualified_tools": "",
 	}
 
 
 @customization(key="dashboard", title="Status dashboard")
 class StatusDashboardCustomization(CustomizationBase):
 	variables = {
 		"dashboard_display_not_qualified_areas": "",
@@ -239,14 +261,17 @@
 		"dashboard_staff_status_staff_only": "",
 		"dashboard_staff_status_weekdays_only": "",
 		"dashboard_staff_status_date_format": "D m/d",
 		"dashboard_staff_status_check_past_status": "",
 		"dashboard_staff_status_check_future_status": "",
 		"dashboard_staff_status_user_view": "",
 		"dashboard_staff_status_staff_view": "",
+		"dashboard_staff_status_absence_view_staff": "",
+		"dashboard_staff_status_absence_view_user_office": "",
+		"dashboard_staff_status_absence_view_accounting_officer": "",
 	}
 
 
 @customization(key="interlock", title="Interlock")
 class InterlockCustomization(CustomizationBase):
 	variables = {
 		"allow_bypass_interlock_on_failure": "",
@@ -309,27 +334,29 @@
 		if name == "weekend_access_notification_emails":
 			recipients = tuple([e for e in value.split(",") if e])
 			for email in recipients:
 				validate_email(email)
 		if value and name == "adjustment_requests_time_limit_frequency":
 			try:
 				if RecurrenceFrequency(int(value)) not in self.frequencies:
-					raise ValidationError(f"frequency must be one of {[freq.display_value for freq in self.frequencies]}")
+					raise ValidationError(
+						f"frequency must be one of {[freq.display_value for freq in self.frequencies]}"
+					)
 			except Exception as e:
 				raise ValidationError(str(e))
 
 
 @customization(key="recurring_charges", title="Recurring charges")
 class RecurringChargesCustomization(CustomizationBase):
 	variables = {
 		"recurring_charges_name": "Recurring charges",
 		"recurring_charges_lock": "",
 		"recurring_charges_category": "",
 		"recurring_charges_force_quantity": "",
-		"recurring_charges_skip_customer_validation": ""
+		"recurring_charges_skip_customer_validation": "",
 	}
 
 	def __init__(self, key, title):
 		super().__init__(key, title)
 		self.update_title()
 
 	def context(self) -> Dict:
@@ -352,14 +379,15 @@
 
 
 @customization(key="tool", title="Tools")
 class ToolCustomization(CustomizationBase):
 	variables = {
 		"tool_phone_number_required": "enabled",
 		"tool_location_required": "enabled",
+		"tool_task_updates_facility_managers": "enabled",
 		"tool_control_hide_data_history_users": "",
 		"tool_control_configuration_setting_template": "{{ current_setting }}",
 		"tool_qualification_reminder_days": "",
 		"tool_qualification_expiration_days": "",
 		"tool_qualification_expiration_never_used_days": "",
 		"tool_qualification_cc": "",
 	}
@@ -449,15 +477,15 @@
 			from NEMO.rates import rate_class
 
 			rate_class.load_rates(force_reload=True)
 		return errors
 
 
 def get_media_file_contents(file_name):
-	""" Get the contents of a media file if it exists. Return a blank string if it does not exist. """
+	"""Get the contents of a media file if it exists. Return a blank string if it does not exist."""
 	storage = get_storage_class()()
 	if not storage.exists(file_name):
 		return ""
 	with storage.open(file_name) as opened_file:
 		read_file = opened_file.read()
 		try:
 			return read_file.decode().strip()
```

### Comparing `NEMO-4.5.5/NEMO/views/email.py` & `NEMO-4.6.0/NEMO/views/email.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 from logging import getLogger
 from smtplib import SMTPException
 from typing import List
 
 from django.contrib import messages
 from django.contrib.auth.decorators import login_required
 from django.core.validators import validate_email
-from django.db.models import Q, QuerySet
+from django.db.models import Q
 from django.http import HttpResponse, HttpResponseBadRequest
 from django.shortcuts import get_object_or_404, redirect, render
 from django.urls import reverse
 from django.utils.safestring import mark_safe
 from django.views.decorators.http import require_GET, require_POST
 
 from NEMO.decorators import any_staff_required
 from NEMO.forms import EmailBroadcastForm
 from NEMO.models import Account, Area, Project, Tool, User, UserType
+from NEMO.typing import QuerySetType
 from NEMO.utilities import EmailCategory, export_format_datetime, render_email_template, send_mail
 from NEMO.views.customization import ApplicationCustomization, get_media_file_contents
 
 logger = getLogger(__name__)
 
 
 @login_required
@@ -234,15 +235,15 @@
 			"template_color": form.data["color"],
 		}
 		email_content = render_email_template(generic_email_template, email_context, request)
 		return HttpResponse(mark_safe(email_content))
 	return HttpResponse()
 
 
-def get_users_for_email(audience: str, selection: List, no_type: bool) -> QuerySet:
+def get_users_for_email(audience: str, selection: List, no_type: bool) -> QuerySetType[User]:
 	users = User.objects.none()
 	if audience == "tool":
 		users = User.objects.filter(qualifications__id__in=selection).distinct()
 	elif audience == "area":
 		access_levels = [access_level for area in Area.objects.filter(pk__in=selection) for access_level in area.get_physical_access_levels()]
 		user_filter = Q(physical_access_levels__in=access_levels)
 		# if one of the access levels allows staff, add all staff & user office
```

### Comparing `NEMO-4.5.5/NEMO/views/event_details.py` & `NEMO-4.6.0/NEMO/views/event_details.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/views/feedback.py` & `NEMO-4.6.0/NEMO/views/feedback.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/views/get_projects.py` & `NEMO-4.6.0/NEMO/views/get_projects.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/views/history.py` & `NEMO-4.6.0/NEMO/views/history.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/views/jumbotron.py` & `NEMO-4.6.0/NEMO/views/jumbotron.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/views/landing.py` & `NEMO-4.6.0/NEMO/views/landing.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/views/maintenance.py` & `NEMO-4.6.0/NEMO/views/maintenance.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from itertools import chain
 
 from django.db.models import Q
 from django.shortcuts import get_object_or_404, render
 from django.views.decorators.http import require_GET
 
 from NEMO.decorators import staff_member_required
-from NEMO.models import Task, TaskCategory, TaskStatus
+from NEMO.models import Task, TaskCategory, TaskStatus, User
 from NEMO.utilities import as_timezone
 
 
 @staff_member_required
 @require_GET
 def maintenance(request, sort_by=''):
+	user: User = request.user
 	pending_tasks = Task.objects.filter(cancelled=False, resolved=False)
+	if user.get_preferences().tool_task_notifications.exists():
+		# Limit tools to preferences + tools user is the owner of + tools user is a backup owner of.
+		limit_tools = set(user.get_preferences().tool_task_notifications.all())
+		limit_tools.update(user.primary_tool_owner.all())
+		limit_tools.update(user.superuser_for_tools.all())
+		pending_tasks = pending_tasks.filter(tool__in=limit_tools)
 	if sort_by in ['urgency', 'force_shutdown', 'tool', 'problem_category', 'last_updated', 'creation_time']:
 		if sort_by == 'last_updated':
 			pending_tasks = pending_tasks.exclude(last_updated=None).order_by('-last_updated')
 			not_yet_updated_tasks = Task.objects.filter(cancelled=False, resolved=False, last_updated=None).order_by('-creation_time')
 			pending_tasks = list(chain(pending_tasks, not_yet_updated_tasks))
 		else:
 			pending_tasks = pending_tasks.order_by(sort_by)
```

### Comparing `NEMO-4.5.5/NEMO/views/mobile.py` & `NEMO-4.6.0/NEMO/views/mobile.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 	if policy_problems:
 		return render(request, 'mobile/error.html', {'message': policy_problems[0]})
 
 	# All policy checks have passed.
 	try:
 		reservation.project = Project.objects.get(id=request.POST['project_id'])
 		# Check if we are allowed to bill to project
-		policy.check_billing_to_project(reservation.project, request.user, reservation.reservation_item)
+		policy.check_billing_to_project(reservation.project, request.user, reservation.reservation_item, reservation)
 	except ProjectChargeException as e:
 		return render(request, 'mobile/error.html', {'message': e.msg})
 	except:
 		if not request.user.is_staff:
 			return render(request, 'mobile/error.html', {'message': 'You must specify a project for your reservation'})
 
 	reservation.additional_information, reservation.self_configuration = extract_configuration(request)
```

### Comparing `NEMO-4.5.5/NEMO/views/news.py` & `NEMO-4.6.0/NEMO/views/news.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/views/notifications.py` & `NEMO-4.6.0/NEMO/views/notifications.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import datetime, timedelta
 from typing import List, Set
 
 from django.contrib.contenttypes.models import ContentType
+from django.db.models import Q
 from django.utils import timezone
 
 from NEMO.models import (
 	AdjustmentRequest,
 	BuddyRequest,
 	Notification,
 	RequestMessage,
@@ -115,15 +116,18 @@
 			object_id=access_request.id,
 			defaults={"expiration": expiration},
 		)
 
 
 def create_adjustment_request_notification(adjustment_request: AdjustmentRequest):
 	users_to_notify = {adjustment_request.creator}
-	reviewers: List[User] = User.objects.filter(is_active=True, is_facility_manager=True)
+	tool = getattr(adjustment_request.item, "tool", None) if adjustment_request.item else None
+	reviewers = User.objects.filter(is_active=True, is_facility_manager=True)
+	if tool:
+		reviewers = reviewers.filter(Q(preferences__tool_adjustment_notifications__isnull=True) | Q(preferences__tool_adjustment_notifications__in=[tool]))
 	users_to_notify.update(reviewers)
 	expiration = timezone.now() + timedelta(days=30)  # 30 days for adjustment requests to expire
 	for user in users_to_notify:
 		# Only update users other than the one who last updated it
 		if not adjustment_request.last_updated_by or adjustment_request.last_updated_by != user:
 			Notification.objects.get_or_create(
 				user=user,
```

### Comparing `NEMO-4.5.5/NEMO/views/pagination.py` & `NEMO-4.6.0/NEMO/views/pagination.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/views/qualifications.py` & `NEMO-4.6.0/NEMO/views/qualifications.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/views/remote_work.py` & `NEMO-4.6.0/NEMO/views/remote_work.py`

 * *Files 3% similar despite different names*

```diff
@@ -202,20 +202,20 @@
 def begin_staff_charge(request):
 	user: User = request.user
 	if user.charging_staff_time():
 		return HttpResponseBadRequest("You cannot create a new staff charge when one is already in progress.")
 	charge = StaffCharge()
 	charge.customer = User.objects.get(id=request.POST["customer"])
 	charge.project = Project.objects.get(id=request.POST["project"])
+	charge.staff_member = request.user
 	# Check if we are allowed to bill to project
 	try:
-		policy.check_billing_to_project(charge.project, charge.customer, charge)
+		policy.check_billing_to_project(charge.project, charge.customer, charge, charge)
 	except ProjectChargeException as e:
 		return HttpResponseBadRequest(e.msg)
-	charge.staff_member = request.user
 	charge.save()
 	return redirect(reverse("staff_charges"))
 
 
 @staff_member_required
 @require_POST
 def end_staff_charge(request):
@@ -235,33 +235,33 @@
 
 
 @staff_member_required
 @require_POST
 def begin_staff_area_charge(request):
 	user: User = request.user
 	charge = user.get_staff_charge()
+	record = AreaAccessRecord()
+	record.staff_charge = charge
+	record.customer = charge.customer
+	record.project = charge.project
 	if not charge:
 		return HttpResponseBadRequest(
 			"You do not have a staff charge in progress, so you cannot begin an area access charge."
 		)
 	if AreaAccessRecord.objects.filter(staff_charge=charge, end=None).count() > 0:
 		return HttpResponseBadRequest("You cannot create an area access charge when one is already in progress.")
 	try:
-		area = Area.objects.get(id=request.POST["area"])
-		policy.check_billing_to_project(charge.project, charge.customer, area)
+		record.area = Area.objects.get(id=request.POST["area"])
+		policy.check_billing_to_project(charge.project, charge.customer, record.area, record)
 	except ProjectChargeException as e:
 		return HttpResponseBadRequest(e.msg)
 	except:
 		return HttpResponseBadRequest("Invalid area")
-	area_access = AreaAccessRecord()
-	area_access.area = area
-	area_access.staff_charge = charge
-	area_access.customer = charge.customer
-	area_access.project = charge.project
-	area_access.save()
+	# No errors, save it
+	record.save()
 	return redirect(reverse("staff_charges"))
 
 
 @staff_member_required
 @require_POST
 def end_staff_area_charge(request):
 	user: User = request.user
```

### Comparing `NEMO-4.5.5/NEMO/views/resources.py` & `NEMO-4.6.0/NEMO/views/resources.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/views/safety.py` & `NEMO-4.6.0/NEMO/views/safety.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/views/sidebar.py` & `NEMO-4.6.0/NEMO/views/sidebar.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/views/status_dashboard.py` & `NEMO-4.6.0/NEMO/views/status_dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 from datetime import datetime, timedelta
 from typing import Dict, List, Optional, Union
 
 from dateutil.relativedelta import relativedelta
 from dateutil.rrule import DAILY, rrule
 from django.conf import settings
 from django.contrib.auth.decorators import login_required
-from django.db.models import F, Prefetch, Q, QuerySet
+from django.db.models import F, Prefetch, Q
 from django.http import HttpResponse
 from django.shortcuts import get_object_or_404, redirect, render
 from django.urls import reverse
 from django.utils import timezone
 from django.views.decorators.http import require_GET, require_http_methods
 
 from NEMO.decorators import disable_session_expiry_refresh, facility_manager_required
 from NEMO.forms import StaffAbsenceForm
-from NEMO.model_tree import ModelTreeHelper, TreeItem, get_area_model_tree
+from NEMO.model_tree import get_area_model_tree, ModelTreeHelper, TreeItem
 from NEMO.models import (
 	Area,
 	AreaAccessRecord,
 	ClosureTime,
 	Resource,
 	ScheduledOutage,
 	StaffAbsence,
 	StaffAvailability,
 	Task,
 	Tool,
 	UsageEvent,
 	User,
 )
+from NEMO.typing import QuerySetType
 from NEMO.utilities import (
-	BasicDisplayTable,
 	as_timezone,
+	BasicDisplayTable,
 	beginning_of_the_day,
 	export_format_datetime,
 	format_datetime,
 	localize,
 	quiet_int,
 )
 from NEMO.views.customization import StatusDashboardCustomization
@@ -45,25 +46,26 @@
 @disable_session_expiry_refresh
 def status_dashboard(request, tab=None):
 	"""
 	Present a web page to allow users to view the status and usage of all tools.
 	"""
 	interest = request.GET.get("interest")
 	if interest is None:
-		csv_export = bool(request.GET.get("csv", False))
-		if tab == "staff" and csv_export:
-			return get_staff_status(request, csv_export)
 		dictionary = {
 			"tab": tab if tab else "occupancy",
 			"show_staff_status": show_staff_status(request),
-			**get_tools_dictionary(),
-			**get_occupancy_dictionary(request),
-			**get_staff_status(request),
 		}
+		csv_export = bool(request.GET.get("csv", False))
+		if tab == "staff":
+			if csv_export:
+				return get_staff_status(request, csv_export)
+			dictionary.update(get_staff_status(request))
 		return render(request, "status_dashboard/status_dashboard.html", dictionary)
+	elif interest == "staff":
+		return render(request, "status_dashboard/staff.html", get_staff_status(request))
 	elif interest == "tools":
 		return render(request, "status_dashboard/tools.html", get_tools_dictionary())
 	elif interest == "occupancy":
 		return render(request, "status_dashboard/occupancy.html", get_occupancy_dictionary(request))
 
 
 def get_tools_dictionary():
@@ -140,15 +142,15 @@
 		end_delta = timedelta(weeks=1)
 	end = start + end_delta - timedelta(days=1)
 	# If we are only showing weekdays, we have to subtract 2 days from the end of the week. Only applies to week view
 	if view == "week" and weekdays_only:
 		end = end - timedelta(days=2)
 	# Reset timestamp to be right in the middle of the period
 	timestamp = int((start + timedelta(days=(end - start).days / 2)).timestamp())
-	staffs = StaffAvailability.objects.filter(visible=True)
+	staffs = StaffAvailability.objects.filter(visible=True).prefetch_related("staff_member", "category")
 	staffs.query.add_ordering(F("category__display_order").asc(nulls_last=True))
 	staffs.query.add_ordering(F("staff_member__first_name").asc())
 	days = rrule(DAILY, dtstart=start, until=end)
 	staff_date_format = StatusDashboardCustomization.get("dashboard_staff_status_date_format")
 	if csv_export:
 		return export_staff_status(request, staffs, days, start, end, staff_date_format)
 	return {
@@ -205,15 +207,15 @@
 	view = request.GET.get("view", "")
 	url = reverse("status_dashboard_tab", args=["staff"])
 	return redirect(f"{url}?timestamp={timestamp}&view={view}")
 
 
 def staff_absences_dict(staffs, days, start, end):
 	dictionary = {staff.id: {} for staff in staffs}
-	absences = StaffAbsence.objects.filter(start_date__lte=end, end_date__gte=start).order_by("creation_time")
+	absences = StaffAbsence.objects.filter(start_date__lte=end, end_date__gte=start).order_by("creation_time").prefetch_related("staff_member")
 	for staff_absence in absences:
 		for day in days:
 			# comparing dates here so no timezone issues (dates don't have timezones)
 			# non-working days should not count as absence
 			staff_works_this_day = staff_absence.staff_member.weekly_availability()[day.weekday()]
 			if staff_works_this_day and staff_absence.start_date <= day.date() <= staff_absence.end_date:
 				dictionary[staff_absence.staff_member.id][day.day] = staff_absence
@@ -293,15 +295,15 @@
 		area_summary_dict = {area["id"]: area for area in area_summary}
 		for area_item in areas_and_parents:
 			area_item.item = area_summary_dict[area_item.id]
 		area_items = area_tree_helper(areas_and_parents, records)
 	return area_items, no_occupants
 
 
-def area_tree_helper(filtered_area: List[TreeItem], records: QuerySet, areas: Optional[List[TreeItem]] = None):
+def area_tree_helper(filtered_area: List[TreeItem], records: QuerySetType[AreaAccessRecord], areas: Optional[List[TreeItem]] = None):
 	""" Recursively build a list of areas. The resulting list is meant to be iterated over in a view """
 	if areas is None:
 		# Get the root areas
 		areas = [area for area in filtered_area if area.is_root]
 	else:
 		yield "in"
 
@@ -316,15 +318,18 @@
 			area.occupants = records.filter(area__id=area.id)
 			area.leaf = True
 	yield "out"
 
 
 def create_tool_summary(tooltip_info=False):
 	tools = Tool.objects.filter(visible=True).prefetch_related(
-		Prefetch("_requires_area_access", queryset=Area.objects.all().only("name"))
+		"_primary_owner",
+		"_backup_owners",
+		"_superusers",
+		Prefetch("_requires_area_access", queryset=Area.objects.all().only("name")),
 	)
 	tasks = Task.objects.filter(cancelled=False, resolved=False, tool__visible=True).prefetch_related("tool")
 	unavailable_resources = Resource.objects.filter(available=False).prefetch_related(
 		"fully_dependent_tools", "partially_dependent_tools"
 	)
 	# also check for visibility on the parent if there is one (alternate tool are hidden)
 	usage_events = UsageEvent.objects.filter(
```

### Comparing `NEMO-4.5.5/NEMO/views/tasks.py` & `NEMO-4.6.0/NEMO/views/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from logging import getLogger
-from typing import List
+from typing import List, Set
 
 from django.conf import settings
 from django.contrib.auth.decorators import login_required
 from django.core.files.base import ContentFile
+from django.db.models import Q
 from django.shortcuts import get_object_or_404, redirect, render
 from django.template.defaultfilters import linebreaksbr
 from django.utils import timezone
 from django.views.decorators.http import require_GET, require_POST
 
 from NEMO.decorators import staff_member_required
 from NEMO.forms import TaskForm, TaskImagesForm, nice_errors
@@ -25,21 +26,25 @@
 )
 from NEMO.utilities import (
 	EmailCategory,
 	as_timezone,
 	bootstrap_primary_color,
 	create_email_attachment,
 	format_datetime,
-	get_email_from_settings,
 	get_full_url,
 	render_email_template,
 	resize_image,
 	send_mail,
 )
-from NEMO.views.customization import ApplicationCustomization, EmailsCustomization, get_media_file_contents
+from NEMO.views.customization import (
+	ApplicationCustomization,
+	EmailsCustomization,
+	ToolCustomization,
+	get_media_file_contents,
+)
 from NEMO.views.safety import send_safety_email_notification
 from NEMO.views.tool_control import determine_tool_status
 
 tasks_logger = getLogger("NEMO.Tasks")
 
 
 @login_required
@@ -108,16 +113,14 @@
 			'task': task,
 			'tool': task.tool,
 			'tool_control_absolute_url': get_full_url(task.tool.get_absolute_url(), request)
 		}
 		subject = ('SAFETY HAZARD: ' if task.safety_hazard else '') + task.tool.name + (' shutdown' if task.force_shutdown else ' problem')
 		message = render_email_template(message, dictionary, request)
 		recipients = get_task_email_recipients(task)
-		if task.tool.notification_email_address:
-			recipients.append(task.tool.notification_email_address)
 		send_mail(subject=subject, content=message, from_email=request.user.email, to=recipients, attachments=attachments, email_category=EmailCategory.TASKS)
 
 	# Email any user (excluding staff) with a future reservation on the tool:
 	user_office_email = EmailsCustomization.get('user_office_email_address')
 	message = get_media_file_contents('reservation_warning_email.html')
 	if user_office_email and message:
 		upcoming_reservations = Reservation.objects.filter(start__gt=timezone.now(), cancelled=False, tool=task.tool, user__is_staff=False)
@@ -173,29 +176,30 @@
 			task_user = task.resolver
 			task_status = 'resolved'
 		else:
 			task_user = task.last_updated_by
 			task_status = 'updated'
 		message = f"""
 A task for the {task.tool} was just modified by {task_user}.
+{('<br><br>Estimated resolution:' + format_datetime(task.estimated_resolution_time)) if task.estimated_resolution_time else ''}
 <br/><br/>
 The latest update is at the bottom of the description. The entirety of the task status follows: 
 <br/><br/>
 Task problem description:<br/>
 {linebreaksbr(task.problem_description)}
 <br/><br/>
 Task progress description:<br/>
 {linebreaksbr(task.progress_description)}
 <br/><br/>
 Task resolution description:<br/>
 {linebreaksbr(task.resolution_description)}
 <br/><br/>
 Visit {url} to view the tool control page for the task.<br/>
 """
-		send_mail(subject=f'{task.tool} task {task_status}', content=message, from_email=get_email_from_settings(), to=recipients, attachments=attachments, email_category=EmailCategory.TASKS)
+		send_mail(subject=f'{task.tool} task {task_status}', content=message, from_email=task_user.email, to=recipients, attachments=attachments, email_category=EmailCategory.TASKS)
 	except Exception as error:
 		site_title = ApplicationCustomization.get('site_title')
 		error_message = f"{site_title} was unable to send the task updated email. The error message that was received is: " + str(error)
 		tasks_logger.exception(error_message)
 
 
 @staff_member_required
@@ -307,14 +311,19 @@
 	except Exception as e:
 		tasks_logger.exception(e)
 	return task_images
 
 
 def get_task_email_recipients(task: Task) -> List[str]:
 	# Add all recipients, starting with primary owner
-	recipient_users: List[User] = [task.tool.primary_owner]
+	recipient_users: Set[User] = {task.tool.primary_owner}
 	# Add backup owners
-	recipient_users.extend(task.tool.backup_owners.all())
-	# Add facility managers
-	recipient_users.extend(User.objects.filter(is_active=True, is_facility_manager=True))
+	recipient_users.update(task.tool.backup_owners.all())
+	# Add facility managers and take into account their preferences
+	if ToolCustomization.get_bool("tool_task_updates_facility_managers"):
+		recipient_users.update(User.objects.filter(is_active=True, is_facility_manager=True).filter(Q(preferences__tool_task_notifications__isnull=True)|Q(preferences__tool_task_notifications__in=[task.tool])))
+	# Add staff/service personnel with preferences set to receive notifications for this tool
+	recipient_users.update(User.objects.filter(is_active=True).filter(Q(is_staff=True)|Q(is_service_personnel=True)).filter(Q(preferences__tool_task_notifications__in=[task.tool])))
 	recipients = [email for user in recipient_users for email in user.get_emails(user.get_preferences().email_send_task_updates)]
+	if task.tool.notification_email_address:
+		recipients.append(task.tool.notification_email_address)
 	return recipients
```

### Comparing `NEMO-4.5.5/NEMO/views/tool_control.py` & `NEMO-4.6.0/NEMO/views/tool_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from itertools import chain
 from json import JSONDecodeError, loads
 from logging import getLogger
 from typing import Dict, List
 
 from django.conf import settings
 from django.contrib.auth.decorators import login_required
+from django.db.models import Q
 from django.http import HttpResponse, HttpResponseBadRequest, HttpResponseNotFound, JsonResponse
 from django.shortcuts import get_object_or_404, redirect, render
 from django.template.defaultfilters import linebreaksbr
 from django.utils import formats, timezone
 from django.utils.safestring import mark_safe
 from django.views.decorators.http import require_GET, require_POST
 
@@ -327,32 +328,32 @@
 
 	tool = get_object_or_404(Tool, id=tool_id)
 	operator = request.user
 	user = get_object_or_404(User, id=user_id)
 	project = get_object_or_404(Project, id=project_id)
 	staff_charge = staff_charge == "true"
 	bypass_interlock = request.POST.get("bypass", 'False') == 'True'
-	response = policy.check_to_enable_tool(tool, operator, user, project, staff_charge)
+	# Figure out if the tool usage is part of remote work
+	# 1: Staff charge means it's always remote work
+	# 2: Always remote if operator is different from the user
+	# 3: Unless customization is set to ask explicitly
+	remote_work = (user != operator and operator.is_staff)
+	if RemoteWorkCustomization.get_bool("remote_work_ask_explicitly"):
+		remote_work = remote_work and bool(request.POST.get("remote_work", False))
+	response = policy.check_to_enable_tool(tool, operator, user, project, staff_charge, remote_work)
 	if response.status_code != HTTPStatus.OK:
 		return response
 
 	# All policy checks passed so enable the tool for the user.
 	if tool.interlock and not tool.interlock.unlock():
 		if bypass_interlock and interlock_bypass_allowed(user):
 			pass
 		else:
 			return interlock_error("Enable", user)
 
-	# Figure out if the tool usage is part of remote work
-	# 1: Staff charge means it's always remote work
-	# 2: Always remote if operator is different from the user
-	# 3: Unless customization is set to ask explicitly
-	remote_work = (user != operator and operator.is_staff)
-	if RemoteWorkCustomization.get_bool("remote_work_ask_explicitly"):
-		remote_work = remote_work and bool(request.POST.get("remote_work", False))
 	# Start staff charge before tool usage
 	if staff_charge:
 		# Staff charge means always a remote
 		remote_work = True
 		new_staff_charge = StaffCharge()
 		new_staff_charge.staff_member = request.user
 		new_staff_charge.customer = user
@@ -400,15 +401,16 @@
 	if tool.interlock and not tool.interlock.lock():
 		if bypass_interlock and interlock_bypass_allowed(user):
 			pass
 		else:
 			return interlock_error("Disable", user)
 
 	# Shorten the user's tool reservation since we are now done using the tool
-	shorten_reservation(user=user, item=tool, new_end=timezone.now() + downtime)
+	staff_shortening = request.POST.get("shorten", False)
+	shorten_reservation(user=user, item=tool, new_end=timezone.now() + downtime, force=staff_shortening)
 
 	# End the current usage event for the tool
 	current_usage_event = tool.get_current_usage_event()
 	current_usage_event.end = timezone.now() + downtime
 
 	# Collect post-usage questions
 	dynamic_form = DynamicForm(tool.post_usage_questions)
@@ -571,36 +573,39 @@
 		"message": linebreaksbr(error_message),
 		"bypass_allowed": interlock_bypass_allowed(user),
 		"action": action
 	}
 	return JsonResponse(dictionary, status=501)
 
 
-def email_managers_required_questions_disable_tool(tool_user:User, staff_member:User, tool:Tool, questions:List[PostUsageQuestion]):
+def email_managers_required_questions_disable_tool(tool_user: User, staff_member: User, tool: Tool, questions: List[PostUsageQuestion]):
+	user_office_email = EmailsCustomization.get('user_office_email_address')
 	abuse_email_address = EmailsCustomization.get('abuse_email_address')
 	cc_users: List[User] = [staff_member, tool.primary_owner]
-	cc_users.extend(tool.backup_owners.all())
-	cc_users.extend(User.objects.filter(is_active=True, is_facility_manager=True))
+	# Add facility managers as CC based on their tool notification preferences if any
+	cc_users.extend(User.objects.filter(is_active=True, is_facility_manager=True).filter(
+		Q(preferences__tool_task_notifications__isnull=True) | Q(preferences__tool_task_notifications__in=[tool])))
 	facility_name = ApplicationCustomization.get('facility_name')
 	ccs = [email for user in cc_users for email in user.get_emails(EmailNotificationType.BOTH_EMAILS)]
+	ccs.append(abuse_email_address)
 	display_questions = "".join([linebreaksbr(mark_safe(question.render_as_text())) + "<br/><br/>" for question in questions])
 	message = f"""
 Dear {tool_user.get_name()},<br/>
 You have been logged off by staff from the {tool} that requires answers to the following post-usage questions:<br/>
 <br/>
 {display_questions}
 <br/>
 Regards,<br/>
 <br/>
 {facility_name} Management<br/>
 """
 	tos = tool_user.get_emails(EmailNotificationType.BOTH_EMAILS)
-	send_mail(subject=f"Unanswered post‑usage questions after logoff from the {tool.name}", content=message, from_email=abuse_email_address, to=tos, cc=ccs, email_category=EmailCategory.ABUSE)
+	send_mail(subject=f"Unanswered post‑usage questions after logoff from the {tool.name}", content=message, from_email=user_office_email, to=tos, cc=ccs, email_category=EmailCategory.ABUSE)
 
 
 def send_tool_usage_counter_email(counter: ToolUsageCounter):
 	user_office_email = EmailsCustomization.get('user_office_email_address')
 	message = get_media_file_contents('counter_threshold_reached_email.html')
 	if user_office_email and message:
 		subject = f"Warning threshold reached for {counter.tool.name} {counter.name} counter"
 		rendered_message = render_email_template(message, {"counter": counter})
-		send_mail(subject=subject, content=rendered_message, from_email=user_office_email, to=counter.warning_email, email_category=EmailCategory.SYSTEM)
+		send_mail(subject=subject, content=rendered_message, from_email=user_office_email, to=counter.warning_email, email_category=EmailCategory.SYSTEM)
```

### Comparing `NEMO-4.5.5/NEMO/views/training.py` & `NEMO-4.6.0/NEMO/views/training.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,31 +18,46 @@
 
 training_logger = getLogger(__name__)
 
 
 @staff_member_or_tool_superuser_required
 @require_GET
 def training(request):
-	""" Present a web page to allow staff or tool superusers to charge training and qualify users on particular tools. """
+	"""Present a web page to allow staff or tool superusers to charge training and qualify users on particular tools."""
 	user: User = request.user
 	users = User.objects.filter(is_active=True).exclude(id=user.id)
 	tools = Tool.objects.filter(visible=True)
 	tool_groups = ToolQualificationGroup.objects.all()
 	if not user.is_staff and user.is_tool_superuser:
 		tools = tools.filter(_superusers__in=[user])
 		# Superusers can only use groups if they are superusers for all those
-		tool_groups = tool_groups.annotate(num_tools=Count("tools")).filter(tools__in=tools).filter(num_tools=len(tools))
-	return render(request, 'training/training.html', {'users': users, 'tools': list(tools), 'tool_groups': list(tool_groups), 'charge_types': TrainingSession.Type.Choices})
+		tool_groups = (
+			tool_groups.annotate(num_tools=Count("tools")).filter(tools__in=tools).filter(num_tools=len(tools))
+		)
+	return render(
+		request,
+		"training/training.html",
+		{
+			"users": users,
+			"tools": list(tools),
+			"tool_groups": list(tool_groups),
+			"charge_types": TrainingSession.Type.Choices,
+		},
+	)
 
 
 @staff_member_or_tool_superuser_required
 @require_GET
 def training_entry(request):
-	entry_number = int(request.GET['entry_number'])
-	return render(request, 'training/training_entry.html', {'entry_number': entry_number, 'charge_types': TrainingSession.Type.Choices})
+	entry_number = int(request.GET["entry_number"])
+	return render(
+		request,
+		"training/training_entry.html",
+		{"entry_number": entry_number, "charge_types": TrainingSession.Type.Choices},
+	)
 
 
 def is_valid_field(field):
 	return search("^(chosen_user|chosen_tool|chosen_project|duration|charge_type|qualify)__[0-9]+$", field) is not None
 
 
 @staff_member_or_tool_superuser_required
@@ -59,54 +74,62 @@
 					charges[index] = TrainingSession()
 					charges[index].trainer = trainer
 				if attribute == "chosen_user":
 					charges[index].trainee = User.objects.get(id=to_int_or_negative(value))
 				if attribute == "chosen_tool":
 					chosen_type = request.POST.get(f"chosen_type{separator}{index}", "tool")
 					identifier = to_int_or_negative(value)
-					setattr(charges[index], "qualify_tools", [Tool.objects.get(id=identifier)] if chosen_type == "tool" else ToolQualificationGroup.objects.get(id=identifier).tools.all())
+					setattr(
+						charges[index],
+						"qualify_tools",
+						[Tool.objects.get(id=identifier)]
+						if chosen_type == "tool"
+						else ToolQualificationGroup.objects.get(id=identifier).tools.all(),
+					)
 					# Even with a group of tools, we only charge training on the first one
 					charges[index].tool = next(iter(charges[index].qualify_tools))
 					if not trainer.is_staff and trainer.is_tool_superuser:
 						if not set(charges[index].qualify_tools).issubset(trainer.superuser_for_tools.all()):
 							return HttpResponseBadRequest("The trainer is not authorized to train on this tool")
 				if attribute == "chosen_project":
 					charges[index].project = Project.objects.get(id=to_int_or_negative(value))
 				if attribute == "duration":
 					charges[index].duration = int(value)
 				if attribute == "charge_type":
 					charges[index].type = int(value)
 				if attribute == "qualify":
-					charges[index].qualified = (value == "on")
+					charges[index].qualified = value == "on"
 		for c in charges.values():
 			c.full_clean()
-			policy.check_billing_to_project(c.project, c.trainee, c.tool)
+			policy.check_billing_to_project(c.project, c.trainee, c.tool, c)
 	except ProjectChargeException as e:
 		return HttpResponseBadRequest(e.msg)
 	except User.DoesNotExist:
 		return HttpResponseBadRequest("Please select a trainee from the list")
 	except Tool.DoesNotExist:
 		return HttpResponseBadRequest("Please select a tool from the list")
 	except Project.DoesNotExist:
 		return HttpResponseBadRequest("Please select a project from the list")
 	except Exception as e:
 		training_logger.exception(e)
-		return HttpResponseBadRequest('An error occurred while processing the training charges. None of the charges were committed to the database. Please review the form for errors and omissions then submit the form again.')
+		return HttpResponseBadRequest(
+			"An error occurred while processing the training charges. None of the charges were committed to the database. Please review the form for errors and omissions then submit the form again."
+		)
 	else:
 		for c in charges.values():
 			if c.qualified:
 				for tool in c.qualify_tools:
 					qualify(c.trainer, c.trainee, tool)
 			c.save()
 		dictionary = {
-			'title': 'Success!',
-			'content': 'Training charges were successfully saved.',
-			'redirect': reverse('landing'),
+			"title": "Success!",
+			"content": "Training charges were successfully saved.",
+			"redirect": reverse("landing"),
 		}
-		return render(request, 'display_success_and_redirect.html', dictionary)
+		return render(request, "display_success_and_redirect.html", dictionary)
 
 
 def qualify(authorizer, user, tool):
 	if tool in user.qualifications.all():
 		return
 	user.qualifications.add(tool)
 	entry = MembershipHistory()
@@ -122,23 +145,23 @@
 			entry = MembershipHistory()
 			entry.authorizer = authorizer
 			entry.parent_content_object = tool.grant_physical_access_level_upon_qualification
 			entry.child_content_object = user
 			entry.action = entry.Action.ADDED
 			entry.save()
 
-	if get_identity_service().get('available', False):
+	if get_identity_service().get("available", False):
 		if tool.grant_badge_reader_access_upon_qualification:
 			parameters = {
-				'username': user.username,
-				'domain': user.domain,
-				'requested_area': tool.grant_badge_reader_access_upon_qualification,
+				"username": user.username,
+				"domain": user.domain,
+				"requested_area": tool.grant_badge_reader_access_upon_qualification,
 			}
-			timeout = settings.IDENTITY_SERVICE.get('timeout', 3)
-			requests.put(urljoin(settings.IDENTITY_SERVICE['url'], '/add/'), data=parameters, timeout=timeout)
+			timeout = settings.IDENTITY_SERVICE.get("timeout", 3)
+			requests.put(urljoin(settings.IDENTITY_SERVICE["url"], "/add/"), data=parameters, timeout=timeout)
 
 
 def to_int_or_negative(value: str):
 	try:
 		return int(value)
 	except ValueError:
 		return -1
```

### Comparing `NEMO-4.5.5/NEMO/views/tutorials.py` & `NEMO-4.6.0/NEMO/views/tutorials.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/views/usage.py` & `NEMO-4.6.0/NEMO/views/usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,67 +84,69 @@
 def date_parameters_dictionary(request):
 	if request.GET.get('start') and request.GET.get('end'):
 		start_date, end_date = extract_optional_beginning_and_end_dates(request.GET, date_only=True)
 	else:
 		start_date, end_date = get_month_timeframe()
 	kind = request.GET.get("type")
 	identifier = request.GET.get("id")
+	existing_adjustments = defaultdict(list)
+	for values in AdjustmentRequest.objects.filter(deleted=False, creator=request.user).values("item_type", "item_id").distinct():
+		existing_adjustments[values["item_type"]].append(values["item_id"])
 	dictionary = {
 		'month_list': month_list(),
 		'start_date': start_date,
 		'end_date': end_date,
 		'kind': kind,
 		'identifier': identifier,
-		'tab_url': get_url_for_other_tab(request) if  get_billing_service().get('available', False) else '',
+		'tab_url': get_url_for_other_tab(request) if get_billing_service().get('available', False) else '',
 		'billing_service': get_billing_service().get('available', False),
+		'adjustment_time_limit': UserRequestsCustomization.get_date_limit(),
+		'existing_adjustments': existing_adjustments,
 	}
 	return dictionary, start_date, end_date, kind, identifier
 
 
 @login_required
 @require_GET
 def usage(request):
 	user: User = request.user
 	user_managed_projects = get_managed_projects(user)
 	base_dictionary, start_date, end_date, kind, identifier = date_parameters_dictionary(request)
 	customer_filter = Q(customer=user) | Q(project__in=user_managed_projects)
 	user_filter = Q(user=user) | Q(project__in=user_managed_projects)
 	trainee_filter = Q(trainee=user) | Q(project__in=user_managed_projects)
-	project_id = request.GET.get("pi_project")
+	project_id = request.GET.get("project") or request.GET.get("pi_project")
 	csv_export = bool(request.GET.get("csv", False))
 	if user_managed_projects:
 		base_dictionary['selected_project'] = "all"
 	if project_id:
 		project = get_object_or_404(Project, id=project_id)
-		base_dictionary['selected_project'] = project
+		if request.GET.get("project"):
+			base_dictionary['selected_user_project'] = project
+		else:
+			base_dictionary['selected_project'] = project
 		customer_filter = customer_filter & Q(project=project)
 		user_filter = user_filter & Q(project=project)
 		trainee_filter = trainee_filter & Q(project=project)
 	area_access = AreaAccessRecord.objects.filter(customer_filter).filter(end__gt=start_date, end__lte=end_date).order_by('-start')
 	consumables = ConsumableWithdraw.objects.filter(customer_filter).filter(date__gt=start_date, date__lte=end_date)
 	missed_reservations = Reservation.objects.filter(user_filter).filter(missed=True, end__gt=start_date, end__lte=end_date)
 	staff_charges = StaffCharge.objects.filter(customer_filter).filter(end__gt=start_date, end__lte=end_date)
 	training_sessions = TrainingSession.objects.filter(trainee_filter).filter(date__gt=start_date, date__lte=end_date)
 	usage_events = UsageEvent.objects.filter(user_filter).filter(end__gt=start_date, end__lte=end_date)
 	if csv_export:
 		return csv_export_response(usage_events, area_access, training_sessions, staff_charges, consumables, missed_reservations)
 	else:
-		existing_adjustments = defaultdict(list)
-		for values in AdjustmentRequest.objects.filter(deleted=False, creator=user).values("item_type", "item_id").distinct():
-			existing_adjustments[values["item_type"]].append(values["item_id"])
 		dictionary = {
 			'area_access': area_access,
 			'consumables': consumables,
 			'missed_reservations': missed_reservations,
 			'staff_charges': staff_charges,
 			'training_sessions': training_sessions,
 			'usage_events': usage_events,
-			'adjustment_time_limit': UserRequestsCustomization.get_date_limit(),
-			'existing_adjustments': existing_adjustments,
-			'can_export': True,
 		}
 		if user_managed_projects:
 			dictionary['pi_projects'] = user_managed_projects
 		dictionary['no_charges'] = not (dictionary['area_access'] or dictionary['consumables'] or dictionary['missed_reservations'] or dictionary['staff_charges'] or dictionary['training_sessions'] or dictionary['usage_events'])
 		return render(request, 'usage/usage.html', {**base_dictionary, **dictionary})
 
 
@@ -205,30 +207,24 @@
 				staff_charges = staff_charges.filter(customer=user)
 				training_sessions = training_sessions.filter(trainee=user)
 				usage_events = usage_events.filter(user=user)
 			if bool(request.GET.get("csv", False)):
 				return csv_export_response(usage_events, area_access, training_sessions, staff_charges, consumables, missed_reservations)
 	except:
 		pass
-	existing_adjustments = defaultdict(list)
-	for values in AdjustmentRequest.objects.filter(deleted=False, creator=request.user).values("item_type", "item_id").distinct():
-		existing_adjustments[values["item_type"]].append(values["item_id"])
 	dictionary = {
 		'search_items': set(Account.objects.all()) | set(Project.objects.all()) | set(get_project_applications()) | set(User.objects.filter(is_active=True)),
 		'area_access': area_access,
 		'consumables': consumables,
 		'missed_reservations': missed_reservations,
 		'staff_charges': staff_charges,
 		'training_sessions': training_sessions,
 		'usage_events': usage_events,
-		'adjustment_time_limit': UserRequestsCustomization.get_date_limit(),
-		'existing_adjustments': existing_adjustments,
 		'project_autocomplete': True,
 		'selection': selection,
-		'can_export': True,
 	}
 	dictionary['no_charges'] = not (dictionary['area_access'] or dictionary['consumables'] or dictionary['missed_reservations'] or dictionary['staff_charges'] or dictionary['training_sessions'] or dictionary['usage_events'])
 	return render(request, 'usage/usage.html', {**base_dictionary, **dictionary})
 
 
 @accounting_or_user_office_or_manager_required
 @require_GET
```

### Comparing `NEMO-4.5.5/NEMO/views/user_requests.py` & `NEMO-4.6.0/NEMO/views/user_requests.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/views/users.py` & `NEMO-4.6.0/NEMO/views/users.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/widgets/configuration_editor.py` & `NEMO-4.6.0/NEMO/widgets/configuration_editor.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO/widgets/dynamic_form.py` & `NEMO-4.6.0/NEMO/widgets/dynamic_form.py`

 * *Files 1% similar despite different names*

```diff
@@ -562,14 +562,15 @@
 				if quantity > 0:
 					make_withdrawal(
 						consumable_id=consumable.id,
 						customer_id=customer.id,
 						merchant=merchant,
 						quantity=quantity,
 						project_id=project.id,
+						tool_usage=True,
 						request=request,
 					)
 			except Exception as e:
 				dynamic_form_logger.warning(
 					f"Could not withdraw consumable: '{question.consumable}' with quantity: '{input_data}' for customer: '{customer}' by merchant: '{merchant}' for project: '{project}'",
 					e,
 				)
```

### Comparing `NEMO-4.5.5/NEMO/widgets/item_tree.py` & `NEMO-4.6.0/NEMO/widgets/item_tree.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/NEMO.egg-info/PKG-INFO` & `NEMO-4.6.0/NEMO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NEMO
-Version: 4.5.5
+Version: 4.6.0
 Summary: NEMO is a laboratory logistics web application. Use it to schedule reservations, control tool access, track maintenance issues, and more.
 Home-page: https://github.com/usnistgov/NEMO
 Author: Center for Nanoscale Science and Technology
 Author-email: CNSTapplications@nist.gov
 License: Public domain
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `NEMO-4.5.5/NEMO.egg-info/SOURCES.txt` & `NEMO-4.6.0/NEMO.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 NEMO/parsers.py
 NEMO/permissions.py
 NEMO/policy.py
 NEMO/provisioning.py
 NEMO/rates.py
 NEMO/rest_filter_backend.py
 NEMO/serializers.py
+NEMO/typing.py
 NEMO/urls.py
 NEMO/utilities.py
 NEMO/wsgi.py
 NEMO.egg-info/PKG-INFO
 NEMO.egg-info/SOURCES.txt
 NEMO.egg-info/dependency_links.txt
 NEMO.egg-info/entry_points.txt
@@ -49,14 +50,32 @@
 NEMO/apps/area_access/templates/area_access/logout_success.html
 NEMO/apps/area_access/templates/area_access/logout_warning.html
 NEMO/apps/area_access/templates/area_access/no_active_projects.html
 NEMO/apps/area_access/templates/area_access/not_logged_in.html
 NEMO/apps/area_access/templates/area_access/physical_access_denied.html
 NEMO/apps/area_access/templates/area_access/resource_unavailable.html
 NEMO/apps/area_access/templates/area_access/welcome_screen.html
+NEMO/apps/contracts/__init__.py
+NEMO/apps/contracts/admin.py
+NEMO/apps/contracts/apps.py
+NEMO/apps/contracts/customization.py
+NEMO/apps/contracts/models.py
+NEMO/apps/contracts/urls.py
+NEMO/apps/contracts/management/__init__.py
+NEMO/apps/contracts/management/commands/__init__.py
+NEMO/apps/contracts/management/commands/send_email_contract_reminders.py
+NEMO/apps/contracts/migrations/0001_initial.py
+NEMO/apps/contracts/migrations/__init__.py
+NEMO/apps/contracts/templates/contracts/contractors.html
+NEMO/apps/contracts/templates/contracts/contracts_and_procurements.html
+NEMO/apps/contracts/templates/contracts/procurements.html
+NEMO/apps/contracts/templates/contracts/service_contracts.html
+NEMO/apps/contracts/templates/customizations/customizations_contracts.html
+NEMO/apps/contracts/views/__init__.py
+NEMO/apps/contracts/views/contracts.py
 NEMO/apps/kiosk/__init__.py
 NEMO/apps/kiosk/urls.py
 NEMO/apps/kiosk/views.py
 NEMO/apps/kiosk/static/kiosk/kiosk.css
 NEMO/apps/kiosk/templates/kiosk/acknowledgement.html
 NEMO/apps/kiosk/templates/kiosk/category_choices.html
 NEMO/apps/kiosk/templates/kiosk/choices.html
@@ -127,14 +146,15 @@
 NEMO/migrations/0040_version_4_2_0.py
 NEMO/migrations/0041_version_4_2_1.py
 NEMO/migrations/0042_version_4_3_0.py
 NEMO/migrations/0043_version_4_3_2.py
 NEMO/migrations/0044_version_4_4_0.py
 NEMO/migrations/0045_version_4_5_0.py
 NEMO/migrations/0045_version_4_5_5.py
+NEMO/migrations/0046_version_4_6_0.py
 NEMO/migrations/__init__.py
 NEMO/static/badge_reader.js
 NEMO/static/favicon.ico
 NEMO/static/jquery.js
 NEMO/static/jquery.min.js
 NEMO/static/jumbotron_watermark.bmp
 NEMO/static/mobile.js
@@ -310,14 +330,15 @@
 NEMO/templates/safety/safety_issues.html
 NEMO/templates/safety/safety_issues_create.html
 NEMO/templates/safety/safety_issues_resolved.html
 NEMO/templates/safety/safety_issues_update.html
 NEMO/templates/safety/safety_items.html
 NEMO/templates/snippets/button.html
 NEMO/templates/snippets/contact_person.html
+NEMO/templates/snippets/document_list.html
 NEMO/templates/snippets/embedded_document.html
 NEMO/templates/snippets/tool_info.html
 NEMO/templates/staff_charges/change_status.html
 NEMO/templates/staff_charges/choose_project.html
 NEMO/templates/staff_charges/end_area_charge.html
 NEMO/templates/staff_charges/new_staff_charge.html
 NEMO/templates/staff_charges/reminder.html
@@ -395,8 +416,9 @@
 NEMO/views/usage.py
 NEMO/views/user_requests.py
 NEMO/views/users.py
 NEMO/widgets/__init__.py
 NEMO/widgets/configuration_editor.py
 NEMO/widgets/dynamic_form.py
 NEMO/widgets/item_tree.py
+resources/settings.py
 resources/splash_pad_settings.py
```

### Comparing `NEMO-4.5.5/PKG-INFO` & `NEMO-4.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NEMO
-Version: 4.5.5
+Version: 4.6.0
 Summary: NEMO is a laboratory logistics web application. Use it to schedule reservations, control tool access, track maintenance issues, and more.
 Home-page: https://github.com/usnistgov/NEMO
 Author: Center for Nanoscale Science and Technology
 Author-email: CNSTapplications@nist.gov
 License: Public domain
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `NEMO-4.5.5/README.md` & `NEMO-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.5/resources/splash_pad_settings.py` & `NEMO-4.6.0/resources/splash_pad_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 	'django.contrib.staticfiles',
 	'django.contrib.admin',
 	'django.contrib.humanize',
 	'NEMO',
 	'NEMO.apps.kiosk',
 	'NEMO.apps.area_access',
 	'NEMO.apps.sensors',
+	'NEMO.apps.contracts',
 	'rest_framework',
 	'django_filters',
 	'mptt',
 	'auditlog',
 ]
 
 MIDDLEWARE = [
```

### Comparing `NEMO-4.5.5/setup.py` & `NEMO-4.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 setup(
 	name='NEMO',
-	version='4.5.5',
+	version='4.6.0',
 	python_requires='>=3.8, <4',
 	packages=find_namespace_packages(exclude=['NEMO.tests', 'NEMO.tests.*']),
 	include_package_data=True,
 	url='https://github.com/usnistgov/NEMO',
 	license='Public domain',
 	author='Center for Nanoscale Science and Technology',
 	author_email='CNSTapplications@nist.gov',
@@ -20,26 +20,26 @@
 		'Intended Audience :: System Administrators',
 		'License :: Public Domain',
 		'Natural Language :: English',
 		'Operating System :: OS Independent',
 		'Programming Language :: Python :: 3.8',
 	],
 	install_requires=[
-		'cryptography==40.0.1',
-		'Django==3.2.19',
-		'django-auditlog==2.2.2',
-		'django-filter==23.1',
+		'cryptography==41.0.2',
+		'Django==3.2.20',
+		'django-auditlog==2.3.0',
+		'django-filter==23.2',
 		'django-mptt==0.14.0',
 		'djangorestframework==3.14.0',
-		'drf-excel==2.3.0',
+		'drf-excel==2.4.0',
 		'drf-flex-fields==1.0.2',
 		'ldap3==2.9.1',
-		'Pillow==9.5.0',
-		'pymodbus==3.2.2',
+		'Pillow==10.0.0',
+		'pymodbus==3.3.2',
 		'python-dateutil==2.8.2',
 		'pytz==2023.3',
-		'requests==2.28.2',
+		'requests==2.31.0',
 	],
 	entry_points={
 		'console_scripts': ['nemo=NEMO.provisioning:entry_point'],
 	},
 )
```

