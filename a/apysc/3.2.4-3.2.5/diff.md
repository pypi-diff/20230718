# Comparing `tmp/apysc-3.2.4.tar.gz` & `tmp/apysc-3.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apysc-3.2.4.tar", last modified: Tue Jul 18 13:04:23 2023, max compression
+gzip compressed data, was "apysc-3.2.5.tar", last modified: Tue Jul 18 13:16:36 2023, max compression
```

## Comparing `apysc-3.2.4.tar` & `apysc-3.2.5.tar`

### file list

```diff
@@ -1,701 +1,701 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.641837 apysc-3.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-18 13:04:02.000000 apysc-3.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-18 13:04:02.000000 apysc-3.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-18 13:04:23.641837 apysc-3.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-18 13:04:02.000000 apysc-3.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.577838 apysc-3.2.4/apysc/
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.585837 apysc-3.2.4/apysc/_animation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_cx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_cx_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_cy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_cy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_finish_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_height.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_height_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_height_for_ellipse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_line_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_line_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_line_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_line_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_move.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_move_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_parallel_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_pause_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_play_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_radius.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_radius_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_reset_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_reverse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_rotation_around_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_rotation_around_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_scale_x_from_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_scale_x_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_scale_x_from_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_scale_x_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_scale_y_from_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_scale_y_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_scale_y_from_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_scale_y_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_time_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_width.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_width_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_width_for_ellipse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/animation_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_animation/easing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.585837 apysc-3.2.4/apysc/_auto_reloading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_auto_reloading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_auto_reloading/auto_reloading_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.585837 apysc-3.2.4/apysc/_branch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_branch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_branch/_elif.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_branch/_else.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_branch/_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_branch/if_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.585837 apysc-3.2.4/apysc/_callable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_callable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_callable/callable_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.589837 apysc-3.2.4/apysc/_chart/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/add_background_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/add_border_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/axis_label_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/axis_label_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/axis_label_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/axis_label_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/axis_label_font_size_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/axis_label_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/axis_line_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/axis_line_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/axis_line_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/background_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/border_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/chart_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/chart_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    19347 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/create_single_column_y_axis_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/initialize_each_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/is_display_axis_label_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/overall_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/set_initial_background_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/set_initial_background_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/set_initial_border_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/set_initial_border_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/set_initial_border_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/set_initial_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/set_initial_horizontal_padding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/set_initial_matrix_data_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/set_initial_overall_container_coordinates_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/set_initial_vertical_padding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/set_initial_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/set_initial_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/set_initial_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/tick_max_num_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/tick_text_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/tick_text_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/tick_text_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/tick_text_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/tick_text_font_size_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/tick_text_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/tick_text_max_num_of_decimal_places_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/vertical_bar_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/x_axis_column_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/x_axis_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/x_axis_label_position.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/x_axis_label_position_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/x_axis_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/y_axis_column_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/y_axis_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/y_axis_label_position.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/y_axis_label_position_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    13401 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/y_axis_single_column_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/y_max_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_chart/y_min_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.589837 apysc-3.2.4/apysc/_color/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_color/color_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.589837 apysc-3.2.4/apysc/_console/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_console/_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    31322 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_console/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_console/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.589837 apysc-3.2.4/apysc/_converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_converter/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_converter/to_apysc_val_from_builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_converter/to_builtin_val_from_apysc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.601837 apysc-3.2.4/apysc/_display/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/any_display_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/append_fill_alpha_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/append_fill_color_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/append_line_alpha_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/append_line_cap_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/append_line_color_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/append_line_joints_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/append_line_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/append_line_thickness_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/append_x_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/append_y_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/begin_fill_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15384 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/child_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    17139 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/css_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/cx_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/cy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/display_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    17102 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/ellipse_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/ellipse_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/flip_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/flip_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/flip_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/get_bounds_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    48598 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/graphics_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/graphics_clear_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/graphics_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/line_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/line_cap_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/line_caps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/line_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/line_dash_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/line_dash_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/line_dash_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/line_dash_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/line_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/line_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/line_joints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/line_joints_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/line_round_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/line_round_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    27082 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/line_style_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/line_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/parent_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/points_2d_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/points_var_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/polygon_append_constructor_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/polygon_apply_current_points_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/polygon_x1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/polygon_x2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/polygon_x3_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/polygon_y1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/polygon_y2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/polygon_y3_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    17186 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/polyline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/radius_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    19212 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/rotation_around_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/rotation_around_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/rotation_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/scale_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/scale_x_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/scale_x_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/scale_y_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/scale_y_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/set_lower_scale_limit_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/set_overflow_visible_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/set_x_and_y_with_minimum_point_interface_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/skew_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/skew_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/sprite.py
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)    22712 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_align_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_delta_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_delta_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_font_size_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_leading_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_set_align_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_set_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_set_delta_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_set_delta_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_set_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_set_font_size_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_set_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_set_leading_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_set_text_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_singleton_for_text_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/svg_text_text_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    17517 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/visible_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/width_and_height_mixin_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/x_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/y_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_display/y_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.601837 apysc-3.2.4/apysc/_event/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/animation_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/click_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/custom_event_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/custom_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/document_mouse_wheel_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/double_click_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/enter_frame_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    15210 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/enter_frame_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/handler_circular_calling_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/mouse_down_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/mouse_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/mouse_event_binding_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/mouse_event_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/mouse_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/mouse_event_unbinding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/mouse_move_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/mouse_out_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/mouse_over_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/mouse_up_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/prevent_default_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/set_handler_data_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/stop_propagation_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/timer_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_event/wheel_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.605837 apysc-3.2.4/apysc/_expression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_expression/event_handler_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_expression/expression_data_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_expression/expression_variables_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_expression/get_last_scope_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_expression/indent_num.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_expression/js_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_expression/last_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_expression/var_names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.605837 apysc-3.2.4/apysc/_file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_file/file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_file/module_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.605837 apysc-3.2.4/apysc/_geom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_bezier_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_bezier_2d_continual.py
--rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_bezier_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_bezier_3d_continual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_close.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_control_x1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_control_x2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_control_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_control_y1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_control_y2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_control_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_data_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_data_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_dest_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_dest_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_horizontal.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_line_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_move_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_vertical.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/path_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/point2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/rectangle_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/rectangle_geom_bottom_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/rectangle_geom_center_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/rectangle_geom_center_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/rectangle_geom_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/rectangle_geom_left_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/rectangle_geom_right_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/rectangle_geom_top_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/rectangle_geom_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_geom/relative_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.609837 apysc-3.2.4/apysc/_html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14536 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_html/debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_html/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_html/html_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_html/html_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.609837 apysc-3.2.4/apysc/_jslib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_jslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    89947 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_jslib/jquery-3.6.3.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_jslib/jquery.mousewheel-3.1.13.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_jslib/jslib_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    78572 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_jslib/svg-3.1.2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    19431 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_jslib/underscore-1.12.0.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.609837 apysc-3.2.4/apysc/_jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_jupyter/jupyter_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.609837 apysc-3.2.4/apysc/_lint_and_doc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_lint_and_doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17625 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_lint_and_doc/conf_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_lint_and_doc/docs_keyword_link_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_lint_and_doc/docs_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_lint_and_doc/docs_toctree_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_lint_and_doc/docs_translation_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_lint_and_doc/docstring_to_markdown_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    51969 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_lint_and_doc/docstring_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_lint_and_doc/document_text_split_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_lint_and_doc/document_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.609837 apysc-3.2.4/apysc/_lint_and_doc/fixed_translation_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_lint_and_doc/fixed_translation_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   220738 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_lint_and_doc/fixed_translation_mapping/jp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_lint_and_doc/lint_and_doc_hash_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11174 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_lint_and_doc/translation_mapping_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.609837 apysc-3.2.4/apysc/_loop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_loop/_continue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_loop/_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_loop/for_array_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_loop/for_array_indices_and_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_loop/for_array_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_loop/for_dict_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_loop/for_dict_keys_and_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_loop/for_dict_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_loop/for_loop_exit_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_loop/initialize_for_loop_key_or_value_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_loop/loop_count.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.613838 apysc-3.2.4/apysc/_math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_math/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_math/max_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_math/min_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_math/trunc_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.613838 apysc-3.2.4/apysc/_string/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_string/indent_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_string/string_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.613838 apysc-3.2.4/apysc/_testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_testing/e2e_testing_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_testing/testing_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.613838 apysc-3.2.4/apysc/_time/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_time/datetime_.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_time/day_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_time/days_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_time/fps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_time/hour_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_time/left_and_right_datetimes_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_time/millisecond_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_time/minute_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_time/month_end_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_time/month_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_time/now_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_time/second_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_time/timedelta_.py
--rw-r--r--   0 runner    (1001) docker     (123)    22477 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_time/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_time/total_seconds_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_time/weekday_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_time/year_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.613838 apysc-3.2.4/apysc/_translation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.633838 apysc-3.2.4/apysc/_translation/jp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/about_handler_options_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/add_child_and_remove_child.py
--rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/add_debug_info_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_base_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_base_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_complete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14221 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_finish.py
--rw-r--r--   0 runner    (1001) docker     (123)   145266 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_interfaces_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_line_color.py
--rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_method_chaining.py
--rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_move.py
--rw-r--r--   0 runner    (1001) docker     (123)    13755 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_pause_and_play.py
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_radius.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_return_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    22568 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_scale_x_and_y_from_center.py
--rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_scale_x_and_y_from_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    24195 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_width_and_height.py
--rw-r--r--   0 runner    (1001) docker     (123)    12950 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_x.py
--rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/animation_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/append_js_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/array_append_and_push.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/array_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/array_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/array_extend_and_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/array_index_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/array_insert_and_insert_at.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/array_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/array_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/array_pop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/array_remove_and_remove_at.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/array_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/array_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/array_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    16116 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/assert_defined_and_undefined.py
--rw-r--r--   0 runner    (1001) docker     (123)    16632 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/assert_equal_and_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/assert_greater_and_greater_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/assert_less_and_less_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/assert_true_and_false.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/assertion_basic_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)    25457 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/bind_and_trigger_custom_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    47773 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)    18686 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     7848 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/contains.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/continue.py
--rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/datetime_day.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/datetime_hour.py
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/datetime_millisecond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/datetime_minute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/datetime_month.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/datetime_now.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/datetime_second.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/datetime_set_month_end.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/datetime_year.py
--rw-r--r--   0 runner    (1001) docker     (123)    16407 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/dblclick.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/dictionary_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/dictionary_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/dictionary_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/display_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    23206 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/display_object_get_and_set_css.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/display_object_mouse_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/display_object_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/display_object_visible.py
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/display_object_x_and_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/display_on_colaboratory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/display_on_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/draw_interfaces_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    85305 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/easing_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/elif.py
--rw-r--r--   0 runner    (1001) docker     (123)    48615 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/else.py
--rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/enter_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/for_array_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/for_array_indices_and_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/for_array_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/for_dict_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/for_dict_keys_and_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/for_dict_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/fps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/fundamental_data_classes_value_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/get_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/get_child_at.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_base_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_base_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_base_flip_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_base_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_base_line_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_base_line_dash_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_base_line_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_base_line_round_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_base_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_base_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (123)    11652 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_base_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    15977 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_base_scale_from_center.py
--rw-r--r--   0 runner    (1001) docker     (123)    24403 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_base_scale_from_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_base_skew.py
--rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_begin_fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_draw_circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_draw_dash_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_draw_dashed_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_draw_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_draw_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_draw_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_draw_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_draw_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_draw_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_draw_round_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_draw_round_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_draw_triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)    62909 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_line_style.py
--rw-r--r--   0 runner    (1001) docker     (123)    18060 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/graphics_move_to_and_line_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/if.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/import_conventions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19496 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    18368 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/int_and_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/int_and_number_arithmetic_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/int_and_number_comparison_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/int_and_number_to_fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)    47237 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/math_max.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/math_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/math_trunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/mouse_event_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    37919 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/mouse_event_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    27631 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/mousedown_and_mouseup.py
--rw-r--r--   0 runner    (1001) docker     (123)    17444 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/mousemove.py
--rw-r--r--   0 runner    (1001) docker     (123)    28202 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/mouseover_and_mouseout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/num_children.py
--rw-r--r--   0 runner    (1001) docker     (123)    61118 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/path_bezier_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    11005 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/path_bezier_2d_continual.py
--rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/path_bezier_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    16113 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/path_bezier_3d_continual.py
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/path_close.py
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/path_horizontal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/path_line_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/path_move_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/path_vertical.py
--rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/point2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    49935 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)    52180 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/polyline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/quick_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/range.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/recommended_type_checker_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    52560 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)    25403 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/rectangle_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/remove_children.py
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/return.py
--rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/save_overall_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/sequential_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/set_debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/sprite.py
--rw-r--r--   0 runner    (1001) docker     (123)    31117 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9529 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/string_addition_and_multiplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/string_apply_max_num_of_decimal_places.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/string_comparison_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/string_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/string_lstrip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/string_rstrip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/string_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/string_strip.py
--rw-r--r--   0 runner    (1001) docker     (123)    48403 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/svg_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    44956 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/svg_text_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/timedelta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/timedelta_days.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/timedelta_total_seconds.py
--rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/timer_complete.py
--rw-r--r--   0 runner    (1001) docker     (123)    17278 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/timer_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/timer_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/timer_repeat_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/timer_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/timer_start_and_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/to_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    64954 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/true_and_false.py
--rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/unset_debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/variable_name_suffix.py
--rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/what_apysc_can_do.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.637838 apysc-3.2.4/apysc/_type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/_return.py
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/any_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    46614 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/attr_linking_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/blank_object_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/bool_const_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    18006 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/copy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/deleted_object_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    23937 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/dictionary_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/expression_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/false.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/hashable_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/initial_substitution_exp_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/initialize_locals_and_globals_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/initialize_top_level_constants_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/number.py
--rw-r--r--   0 runner    (1001) docker     (123)    34277 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/number_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/py_builtin_iter_disabling_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/repr_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/revert_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/revert_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    27995 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/string_apply_max_num_of_decimal_places_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/string_length_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/string_lstrip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/string_rstrip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/string_split_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/string_strip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/to_fixed_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/to_number_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/to_string_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/true.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/type_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/type_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/value_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/variable_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/variable_name_suffix_attr_or_var_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/variable_name_suffix_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_type/variable_name_suffix_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.641837 apysc-3.2.4/apysc/_validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   109237 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_validation/arg_validation_decos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_validation/bool_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_validation/color_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_validation/display_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_validation/event_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_validation/geom_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_validation/handler_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_validation/matrix_data_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_validation/number_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_validation/parent_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_validation/path_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_validation/string_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_validation/validate_stage_is_created_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_validation/validation_common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-18 13:04:02.000000 apysc-3.2.4/apysc/_validation/variable_name_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:04:23.581838 apysc-3.2.4/apysc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-18 13:04:23.000000 apysc-3.2.4/apysc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26359 2023-07-18 13:04:23.000000 apysc-3.2.4/apysc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:04:23.000000 apysc-3.2.4/apysc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 13:04:23.000000 apysc-3.2.4/apysc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 13:04:23.000000 apysc-3.2.4/apysc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:04:23.641837 apysc-3.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.245253 apysc-3.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-18 13:16:17.000000 apysc-3.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-18 13:16:17.000000 apysc-3.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-18 13:16:36.245253 apysc-3.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-18 13:16:17.000000 apysc-3.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.181254 apysc-3.2.5/apysc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.189253 apysc-3.2.5/apysc/_animation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_cx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_cx_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_cy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_cy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_finish_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_height.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_height_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_height_for_ellipse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_move_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_parallel_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_pause_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_play_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_radius_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_reset_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_reverse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_rotation_around_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_rotation_around_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_scale_x_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_scale_x_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_scale_x_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_scale_x_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_scale_y_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_scale_y_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_scale_y_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_scale_y_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_time_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_width.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_width_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_width_for_ellipse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/animation_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_animation/easing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.189253 apysc-3.2.5/apysc/_auto_reloading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_auto_reloading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_auto_reloading/auto_reloading_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.189253 apysc-3.2.5/apysc/_branch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_branch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_branch/_elif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_branch/_else.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_branch/_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_branch/if_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.189253 apysc-3.2.5/apysc/_callable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_callable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_callable/callable_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.193253 apysc-3.2.5/apysc/_chart/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/add_background_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/add_border_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/axis_label_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/axis_label_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/axis_label_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/axis_label_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/axis_label_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/axis_label_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/axis_line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/axis_line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/axis_line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/background_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/border_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/chart_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/chart_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19347 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/create_single_column_y_axis_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/initialize_each_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/is_display_axis_label_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/overall_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/set_initial_background_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/set_initial_background_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/set_initial_border_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/set_initial_border_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/set_initial_border_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/set_initial_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/set_initial_horizontal_padding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/set_initial_matrix_data_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/set_initial_overall_container_coordinates_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/set_initial_vertical_padding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/set_initial_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/set_initial_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/set_initial_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/tick_max_num_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/tick_text_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/tick_text_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/tick_text_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/tick_text_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/tick_text_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/tick_text_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/tick_text_max_num_of_decimal_places_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/vertical_bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/x_axis_column_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/x_axis_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/x_axis_label_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/x_axis_label_position_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/x_axis_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/y_axis_column_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/y_axis_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/y_axis_label_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/y_axis_label_position_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13401 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/y_axis_single_column_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/y_max_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_chart/y_min_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.193253 apysc-3.2.5/apysc/_color/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_color/color_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.193253 apysc-3.2.5/apysc/_console/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_console/_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31322 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_console/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_console/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.193253 apysc-3.2.5/apysc/_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_converter/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_converter/to_apysc_val_from_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_converter/to_builtin_val_from_apysc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.205253 apysc-3.2.5/apysc/_display/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/any_display_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/append_fill_alpha_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/append_fill_color_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/append_line_alpha_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/append_line_cap_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/append_line_color_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/append_line_joints_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/append_line_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/append_line_thickness_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/append_x_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/append_y_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/begin_fill_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15384 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/child_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17139 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/css_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/cx_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/cy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/display_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17102 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/ellipse_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/ellipse_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/flip_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/flip_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/flip_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/get_bounds_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48598 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/graphics_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/graphics_clear_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/graphics_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/line_cap_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/line_caps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/line_dash_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/line_dash_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/line_dash_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/line_dash_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/line_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/line_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/line_joints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/line_joints_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/line_round_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/line_round_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27082 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/line_style_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/parent_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/points_2d_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/points_var_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/polygon_append_constructor_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/polygon_apply_current_points_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/polygon_x1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/polygon_x2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/polygon_x3_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/polygon_y1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/polygon_y2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/polygon_y3_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17186 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/radius_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19212 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/rotation_around_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/rotation_around_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/rotation_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/scale_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/scale_x_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/scale_x_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/scale_y_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/scale_y_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/set_lower_scale_limit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/set_overflow_visible_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/set_x_and_y_with_minimum_point_interface_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/skew_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/skew_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/sprite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22712 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_align_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_delta_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_delta_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_leading_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_set_align_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_set_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_set_delta_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_set_delta_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_set_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_set_font_size_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_set_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_set_leading_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_set_text_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_singleton_for_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/svg_text_text_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17517 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/visible_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/width_and_height_mixin_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/x_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/y_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_display/y_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.205253 apysc-3.2.5/apysc/_event/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/animation_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/click_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/custom_event_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/custom_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/document_mouse_wheel_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/double_click_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/enter_frame_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15210 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/enter_frame_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/handler_circular_calling_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/mouse_down_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/mouse_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/mouse_event_binding_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/mouse_event_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/mouse_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/mouse_event_unbinding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/mouse_move_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/mouse_out_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/mouse_over_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/mouse_up_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/prevent_default_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/set_handler_data_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/stop_propagation_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/timer_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_event/wheel_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.209253 apysc-3.2.5/apysc/_expression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_expression/event_handler_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_expression/expression_data_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_expression/expression_variables_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_expression/get_last_scope_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_expression/indent_num.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_expression/js_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_expression/last_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_expression/var_names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.209253 apysc-3.2.5/apysc/_file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_file/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_file/module_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.209253 apysc-3.2.5/apysc/_geom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_bezier_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_bezier_2d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_bezier_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_bezier_3d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_close.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_control_x1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_control_x2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_control_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_control_y1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_control_y2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_control_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_data_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_data_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_dest_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_dest_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_move_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_vertical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/path_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/point2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/rectangle_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/rectangle_geom_bottom_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/rectangle_geom_center_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/rectangle_geom_center_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/rectangle_geom_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/rectangle_geom_left_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/rectangle_geom_right_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/rectangle_geom_top_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/rectangle_geom_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_geom/relative_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.213253 apysc-3.2.5/apysc/_html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14536 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_html/debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_html/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_html/html_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_html/html_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.213253 apysc-3.2.5/apysc/_jslib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_jslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89947 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_jslib/jquery-3.6.3.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_jslib/jquery.mousewheel-3.1.13.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_jslib/jslib_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78572 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_jslib/svg-3.1.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19431 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_jslib/underscore-1.12.0.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.213253 apysc-3.2.5/apysc/_jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_jupyter/jupyter_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.213253 apysc-3.2.5/apysc/_lint_and_doc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_lint_and_doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17625 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_lint_and_doc/conf_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_lint_and_doc/docs_keyword_link_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_lint_and_doc/docs_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_lint_and_doc/docs_toctree_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_lint_and_doc/docs_translation_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_lint_and_doc/docstring_to_markdown_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51969 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_lint_and_doc/docstring_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_lint_and_doc/document_text_split_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_lint_and_doc/document_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.213253 apysc-3.2.5/apysc/_lint_and_doc/fixed_translation_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_lint_and_doc/fixed_translation_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   220738 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_lint_and_doc/fixed_translation_mapping/jp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_lint_and_doc/lint_and_doc_hash_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11174 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_lint_and_doc/translation_mapping_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.213253 apysc-3.2.5/apysc/_loop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_loop/_continue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_loop/_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_loop/for_array_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_loop/for_array_indices_and_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_loop/for_array_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_loop/for_dict_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_loop/for_dict_keys_and_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_loop/for_dict_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_loop/for_loop_exit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_loop/initialize_for_loop_key_or_value_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_loop/loop_count.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.217253 apysc-3.2.5/apysc/_math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_math/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_math/max_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_math/min_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_math/trunc_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.217253 apysc-3.2.5/apysc/_string/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_string/indent_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_string/string_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.217253 apysc-3.2.5/apysc/_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_testing/e2e_testing_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_testing/testing_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.217253 apysc-3.2.5/apysc/_time/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_time/datetime_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_time/day_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_time/days_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_time/fps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_time/hour_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_time/left_and_right_datetimes_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_time/millisecond_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_time/minute_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_time/month_end_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_time/month_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_time/now_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_time/second_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_time/timedelta_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22477 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_time/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_time/total_seconds_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_time/weekday_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_time/year_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.217253 apysc-3.2.5/apysc/_translation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.237253 apysc-3.2.5/apysc/_translation/jp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/about_handler_options_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/add_child_and_remove_child.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/add_debug_info_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_base_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_base_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14221 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)   145266 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_interfaces_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_method_chaining.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_move.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13755 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_pause_and_play.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_return_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22568 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_scale_x_and_y_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_scale_x_and_y_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24195 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_width_and_height.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12950 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/animation_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/append_js_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/array_append_and_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/array_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/array_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/array_extend_and_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/array_index_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/array_insert_and_insert_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/array_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/array_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/array_pop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/array_remove_and_remove_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/array_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/array_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/array_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16116 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/assert_defined_and_undefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16632 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/assert_equal_and_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/assert_greater_and_greater_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/assert_less_and_less_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/assert_true_and_false.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/assertion_basic_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25457 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/bind_and_trigger_custom_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47773 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18686 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7848 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/contains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/continue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/datetime_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/datetime_hour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/datetime_millisecond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/datetime_minute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/datetime_month.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/datetime_now.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/datetime_second.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/datetime_set_month_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/datetime_year.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16407 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/dblclick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/dictionary_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/dictionary_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/dictionary_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/display_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23206 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/display_object_get_and_set_css.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/display_object_mouse_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/display_object_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/display_object_visible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/display_object_x_and_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/display_on_colaboratory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/display_on_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/draw_interfaces_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85305 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/easing_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/elif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48615 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/else.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/enter_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/for_array_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/for_array_indices_and_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/for_array_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/for_dict_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/for_dict_keys_and_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/for_dict_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/fps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/fundamental_data_classes_value_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/get_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/get_child_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_base_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_base_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_base_flip_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_base_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_base_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_base_line_dash_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_base_line_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_base_line_round_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_base_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_base_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11652 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_base_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15977 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_base_scale_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24403 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_base_scale_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_base_skew.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_begin_fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_draw_circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_draw_dash_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_draw_dashed_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_draw_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_draw_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_draw_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_draw_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_draw_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_draw_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_draw_round_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_draw_round_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_draw_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62909 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_line_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18060 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/graphics_move_to_and_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/import_conventions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19496 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18368 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/int_and_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/int_and_number_arithmetic_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/int_and_number_comparison_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/int_and_number_to_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47237 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/math_max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/math_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/math_trunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/mouse_event_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37919 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/mouse_event_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27631 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/mousedown_and_mouseup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17444 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/mousemove.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28202 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/mouseover_and_mouseout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/num_children.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61118 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/path_bezier_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11005 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/path_bezier_2d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/path_bezier_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16113 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/path_bezier_3d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/path_close.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/path_horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/path_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/path_move_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/path_vertical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/point2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49935 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52180 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/quick_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/recommended_type_checker_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52560 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25403 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/rectangle_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/remove_children.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/return.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/save_overall_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/sequential_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/set_debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/sprite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31117 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9529 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/string_addition_and_multiplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/string_apply_max_num_of_decimal_places.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/string_comparison_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/string_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/string_lstrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/string_rstrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/string_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/string_strip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48403 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/svg_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44956 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/svg_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/timedelta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/timedelta_days.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/timedelta_total_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/timer_complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17278 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/timer_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/timer_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/timer_repeat_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/timer_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/timer_start_and_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/to_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64954 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/true_and_false.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/unset_debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/variable_name_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/what_apysc_can_do.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.241253 apysc-3.2.5/apysc/_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/any_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46614 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/attr_linking_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/blank_object_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/bool_const_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18006 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/copy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/deleted_object_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23937 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/dictionary_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/expression_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/false.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/hashable_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/initial_substitution_exp_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/initialize_locals_and_globals_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/initialize_top_level_constants_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34277 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/number_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/py_builtin_iter_disabling_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/repr_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/revert_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/revert_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27995 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/string_apply_max_num_of_decimal_places_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/string_length_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/string_lstrip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/string_rstrip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/string_split_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/string_strip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/to_fixed_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/to_number_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/to_string_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/true.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/type_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/value_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/variable_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/variable_name_suffix_attr_or_var_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/variable_name_suffix_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_type/variable_name_suffix_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.245253 apysc-3.2.5/apysc/_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109237 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_validation/arg_validation_decos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_validation/bool_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_validation/color_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_validation/display_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_validation/event_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_validation/geom_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_validation/handler_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_validation/matrix_data_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_validation/number_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_validation/parent_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_validation/path_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_validation/string_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_validation/validate_stage_is_created_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_validation/validation_common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-18 13:16:17.000000 apysc-3.2.5/apysc/_validation/variable_name_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:16:36.181254 apysc-3.2.5/apysc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-18 13:16:36.000000 apysc-3.2.5/apysc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26359 2023-07-18 13:16:36.000000 apysc-3.2.5/apysc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:16:36.000000 apysc-3.2.5/apysc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 13:16:36.000000 apysc-3.2.5/apysc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 13:16:36.000000 apysc-3.2.5/apysc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:16:36.245253 apysc-3.2.5/setup.cfg
```

### Comparing `apysc-3.2.4/LICENSE` & `apysc-3.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/PKG-INFO` & `apysc-3.2.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apysc
-Version: 3.2.4
+Version: 3.2.5
 Summary: apysc is the Python's frontend library to create html and js file, that has the ActionScript 3 (as3)-like interface.
 Home-page: https://github.com/simon-ritchie/apysc
 Maintainer: simon-ritchie
 Maintainer-email: 
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apysc-3.2.4/README.md` & `apysc-3.2.5/README.md`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/__init__.py` & `apysc-3.2.5/apysc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,8 +132,8 @@
 from apysc._chart.y_axis_label_position import YAxisLabelPosition
 from apysc._type.true import _True as __True
 from apysc._type.false import _False as __False
 
 True_: __True
 False_: __False
 
-__version__: str = "3.2.4"
+__version__: str = "3.2.5"
```

### Comparing `apysc-3.2.4/apysc/_animation/animation_base.py` & `apysc-3.2.5/apysc/_animation/animation_base.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_cx.py` & `apysc-3.2.5/apysc/_animation/animation_cx.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_cx_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_cx_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_cy.py` & `apysc-3.2.5/apysc/_animation/animation_cy.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_cy_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_cy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_fill_alpha.py` & `apysc-3.2.5/apysc/_animation/animation_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_fill_alpha_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_fill_color.py` & `apysc-3.2.5/apysc/_animation/animation_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_fill_color_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_finish_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_finish_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_height.py` & `apysc-3.2.5/apysc/_animation/animation_height.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_height_for_ellipse.py` & `apysc-3.2.5/apysc/_animation/animation_height_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_height_for_ellipse_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_height_for_ellipse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_height_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_line_alpha.py` & `apysc-3.2.5/apysc/_animation/animation_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_line_alpha_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_line_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_line_color.py` & `apysc-3.2.5/apysc/_animation/animation_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_line_color_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_line_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_line_thickness.py` & `apysc-3.2.5/apysc/_animation/animation_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_line_thickness_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_line_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_mixins.py` & `apysc-3.2.5/apysc/_animation/animation_mixins.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_move.py` & `apysc-3.2.5/apysc/_animation/animation_move.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_move_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_move_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_parallel.py` & `apysc-3.2.5/apysc/_animation/animation_parallel.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_parallel_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_parallel_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_pause_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_pause_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_play_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_play_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_radius.py` & `apysc-3.2.5/apysc/_animation/animation_radius.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_radius_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_radius_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_reset_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_reset_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_reverse_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_reverse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_rotation_around_center.py` & `apysc-3.2.5/apysc/_animation/animation_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_rotation_around_center_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_rotation_around_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_rotation_around_point.py` & `apysc-3.2.5/apysc/_animation/animation_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_rotation_around_point_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_rotation_around_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_scale_x_from_center.py` & `apysc-3.2.5/apysc/_animation/animation_scale_x_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_scale_x_from_center_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_scale_x_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_scale_x_from_point.py` & `apysc-3.2.5/apysc/_animation/animation_scale_x_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_scale_x_from_point_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_scale_x_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_scale_y_from_center.py` & `apysc-3.2.5/apysc/_animation/animation_scale_y_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_scale_y_from_center_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_scale_y_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_scale_y_from_point.py` & `apysc-3.2.5/apysc/_animation/animation_scale_y_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_scale_y_from_point_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_scale_y_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_time_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_time_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_width.py` & `apysc-3.2.5/apysc/_animation/animation_width.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_width_for_ellipse.py` & `apysc-3.2.5/apysc/_animation/animation_width_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_width_for_ellipse_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_width_for_ellipse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_width_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_x.py` & `apysc-3.2.5/apysc/_animation/animation_x.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_x_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_y.py` & `apysc-3.2.5/apysc/_animation/animation_y.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/animation_y_mixin.py` & `apysc-3.2.5/apysc/_animation/animation_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_animation/easing.py` & `apysc-3.2.5/apysc/_animation/easing.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_auto_reloading/auto_reloading_decorator.py` & `apysc-3.2.5/apysc/_auto_reloading/auto_reloading_decorator.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_branch/_elif.py` & `apysc-3.2.5/apysc/_branch/_elif.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_branch/_else.py` & `apysc-3.2.5/apysc/_branch/_else.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_branch/_if.py` & `apysc-3.2.5/apysc/_branch/_if.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_branch/if_base.py` & `apysc-3.2.5/apysc/_branch/if_base.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_callable/callable_util.py` & `apysc-3.2.5/apysc/_callable/callable_util.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/add_background_mixin.py` & `apysc-3.2.5/apysc/_chart/add_background_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/add_border_mixin.py` & `apysc-3.2.5/apysc/_chart/add_border_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/axis_label_bold_mixin.py` & `apysc-3.2.5/apysc/_chart/axis_label_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/axis_label_fill_alpha_mixin.py` & `apysc-3.2.5/apysc/_chart/axis_label_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/axis_label_fill_color_mixin.py` & `apysc-3.2.5/apysc/_chart/axis_label_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/axis_label_font_family_mixin.py` & `apysc-3.2.5/apysc/_chart/axis_label_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/axis_label_font_size_mixin.py` & `apysc-3.2.5/apysc/_chart/axis_label_font_size_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/axis_label_italic_mixin.py` & `apysc-3.2.5/apysc/_chart/axis_label_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/axis_line_alpha_mixin.py` & `apysc-3.2.5/apysc/_chart/axis_line_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/axis_line_color_mixin.py` & `apysc-3.2.5/apysc/_chart/axis_line_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/axis_line_thickness_mixin.py` & `apysc-3.2.5/apysc/_chart/axis_line_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/background_container_mixin.py` & `apysc-3.2.5/apysc/_chart/background_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/border_container_mixin.py` & `apysc-3.2.5/apysc/_chart/border_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/chart_container_mixin.py` & `apysc-3.2.5/apysc/_chart/chart_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/create_single_column_y_axis_mixin.py` & `apysc-3.2.5/apysc/_chart/create_single_column_y_axis_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/initialize_each_container_mixin.py` & `apysc-3.2.5/apysc/_chart/initialize_each_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/is_display_axis_label_mixin.py` & `apysc-3.2.5/apysc/_chart/is_display_axis_label_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/overall_container_mixin.py` & `apysc-3.2.5/apysc/_chart/overall_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/set_initial_background_fill_alpha_mixin.py` & `apysc-3.2.5/apysc/_chart/set_initial_background_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/set_initial_background_fill_color_mixin.py` & `apysc-3.2.5/apysc/_chart/set_initial_background_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/set_initial_border_alpha_mixin.py` & `apysc-3.2.5/apysc/_chart/set_initial_border_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/set_initial_border_color_mixin.py` & `apysc-3.2.5/apysc/_chart/set_initial_border_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/set_initial_border_thickness_mixin.py` & `apysc-3.2.5/apysc/_chart/set_initial_border_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/set_initial_height_mixin.py` & `apysc-3.2.5/apysc/_chart/set_initial_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/set_initial_horizontal_padding_mixin.py` & `apysc-3.2.5/apysc/_chart/set_initial_horizontal_padding_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/set_initial_matrix_data_mixin.py` & `apysc-3.2.5/apysc/_chart/set_initial_matrix_data_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/set_initial_overall_container_coordinates_mixin.py` & `apysc-3.2.5/apysc/_chart/set_initial_overall_container_coordinates_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/set_initial_vertical_padding_mixin.py` & `apysc-3.2.5/apysc/_chart/set_initial_vertical_padding_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/set_initial_width_mixin.py` & `apysc-3.2.5/apysc/_chart/set_initial_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/set_initial_x_mixin.py` & `apysc-3.2.5/apysc/_chart/set_initial_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/set_initial_y_mixin.py` & `apysc-3.2.5/apysc/_chart/set_initial_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/tick_max_num_mixin.py` & `apysc-3.2.5/apysc/_chart/tick_max_num_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/tick_text_bold_mixin.py` & `apysc-3.2.5/apysc/_chart/tick_text_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/tick_text_fill_alpha_mixin.py` & `apysc-3.2.5/apysc/_chart/tick_text_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/tick_text_fill_color_mixin.py` & `apysc-3.2.5/apysc/_chart/tick_text_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/tick_text_font_family_mixin.py` & `apysc-3.2.5/apysc/_chart/tick_text_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/tick_text_font_size_mixin.py` & `apysc-3.2.5/apysc/_chart/tick_text_font_size_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/tick_text_italic_mixin.py` & `apysc-3.2.5/apysc/_chart/tick_text_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/tick_text_max_num_of_decimal_places_mixin.py` & `apysc-3.2.5/apysc/_chart/tick_text_max_num_of_decimal_places_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/vertical_bar_chart.py` & `apysc-3.2.5/apysc/_chart/vertical_bar_chart.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/x_axis_column_name_mixin.py` & `apysc-3.2.5/apysc/_chart/x_axis_column_name_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/x_axis_container_mixin.py` & `apysc-3.2.5/apysc/_chart/x_axis_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/x_axis_label_position_mixin.py` & `apysc-3.2.5/apysc/_chart/x_axis_label_position_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/x_axis_settings.py` & `apysc-3.2.5/apysc/_chart/x_axis_settings.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/y_axis_column_name_mixin.py` & `apysc-3.2.5/apysc/_chart/y_axis_column_name_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/y_axis_container_mixin.py` & `apysc-3.2.5/apysc/_chart/y_axis_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/y_axis_label_position_mixin.py` & `apysc-3.2.5/apysc/_chart/y_axis_label_position_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/y_axis_single_column_settings.py` & `apysc-3.2.5/apysc/_chart/y_axis_single_column_settings.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/y_max_mixin.py` & `apysc-3.2.5/apysc/_chart/y_max_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_chart/y_min_mixin.py` & `apysc-3.2.5/apysc/_chart/y_min_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_color/color_util.py` & `apysc-3.2.5/apysc/_color/color_util.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_console/_trace.py` & `apysc-3.2.5/apysc/_console/_trace.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_console/assertion.py` & `apysc-3.2.5/apysc/_console/assertion.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_console/loggers.py` & `apysc-3.2.5/apysc/_console/loggers.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_converter/cast.py` & `apysc-3.2.5/apysc/_converter/cast.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_converter/to_apysc_val_from_builtin.py` & `apysc-3.2.5/apysc/_converter/to_apysc_val_from_builtin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_converter/to_builtin_val_from_apysc.py` & `apysc-3.2.5/apysc/_converter/to_builtin_val_from_apysc.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/_document.py` & `apysc-3.2.5/apysc/_display/_document.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/any_display_object.py` & `apysc-3.2.5/apysc/_display/any_display_object.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/append_fill_alpha_attr_expression_mixin.py` & `apysc-3.2.5/apysc/_display/append_fill_alpha_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/append_fill_color_expression_mixin.py` & `apysc-3.2.5/apysc/_display/append_fill_color_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/append_line_alpha_attr_expression_mixin.py` & `apysc-3.2.5/apysc/_display/append_line_alpha_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/append_line_cap_attr_expression_mixin.py` & `apysc-3.2.5/apysc/_display/append_line_cap_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/append_line_color_attr_expression_mixin.py` & `apysc-3.2.5/apysc/_display/append_line_color_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/append_line_joints_attr_expression_mixin.py` & `apysc-3.2.5/apysc/_display/append_line_joints_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/append_line_point_mixin.py` & `apysc-3.2.5/apysc/_display/append_line_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/append_line_thickness_attr_expression_mixin.py` & `apysc-3.2.5/apysc/_display/append_line_thickness_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/append_x_attr_expression_mixin.py` & `apysc-3.2.5/apysc/_display/append_x_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/append_y_attr_expression_mixin.py` & `apysc-3.2.5/apysc/_display/append_y_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/begin_fill_mixin.py` & `apysc-3.2.5/apysc/_display/begin_fill_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/child_mixin.py` & `apysc-3.2.5/apysc/_display/child_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/circle.py` & `apysc-3.2.5/apysc/_display/circle.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/css_interface.py` & `apysc-3.2.5/apysc/_display/css_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/css_mixin.py` & `apysc-3.2.5/apysc/_display/css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/cx_mixin.py` & `apysc-3.2.5/apysc/_display/cx_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/cy_mixin.py` & `apysc-3.2.5/apysc/_display/cy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/display_object.py` & `apysc-3.2.5/apysc/_display/display_object.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/ellipse.py` & `apysc-3.2.5/apysc/_display/ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/ellipse_height_mixin.py` & `apysc-3.2.5/apysc/_display/ellipse_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/ellipse_width_mixin.py` & `apysc-3.2.5/apysc/_display/ellipse_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/fill_alpha_mixin.py` & `apysc-3.2.5/apysc/_display/fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/fill_color_mixin.py` & `apysc-3.2.5/apysc/_display/fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/flip_interface_helper.py` & `apysc-3.2.5/apysc/_display/flip_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/flip_x_mixin.py` & `apysc-3.2.5/apysc/_display/flip_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/flip_y_mixin.py` & `apysc-3.2.5/apysc/_display/flip_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/get_bounds_mixin.py` & `apysc-3.2.5/apysc/_display/get_bounds_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/graphics.py` & `apysc-3.2.5/apysc/_display/graphics.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/graphics_base.py` & `apysc-3.2.5/apysc/_display/graphics_base.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/graphics_clear_mixin.py` & `apysc-3.2.5/apysc/_display/graphics_clear_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/graphics_expression.py` & `apysc-3.2.5/apysc/_display/graphics_expression.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/height_mixin.py` & `apysc-3.2.5/apysc/_display/height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/line.py` & `apysc-3.2.5/apysc/_display/line.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/line_alpha_mixin.py` & `apysc-3.2.5/apysc/_display/line_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/line_cap_mixin.py` & `apysc-3.2.5/apysc/_display/line_cap_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/line_caps.py` & `apysc-3.2.5/apysc/_display/line_caps.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/line_color_mixin.py` & `apysc-3.2.5/apysc/_display/line_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/line_dash_dot_setting.py` & `apysc-3.2.5/apysc/_display/line_dash_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/line_dash_dot_setting_mixin.py` & `apysc-3.2.5/apysc/_display/line_dash_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/line_dash_setting.py` & `apysc-3.2.5/apysc/_display/line_dash_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/line_dash_setting_mixin.py` & `apysc-3.2.5/apysc/_display/line_dash_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/line_dot_setting.py` & `apysc-3.2.5/apysc/_display/line_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/line_dot_setting_mixin.py` & `apysc-3.2.5/apysc/_display/line_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/line_joints.py` & `apysc-3.2.5/apysc/_display/line_joints.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/line_joints_mixin.py` & `apysc-3.2.5/apysc/_display/line_joints_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/line_round_dot_setting.py` & `apysc-3.2.5/apysc/_display/line_round_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/line_round_dot_setting_mixin.py` & `apysc-3.2.5/apysc/_display/line_round_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/line_style_mixin.py` & `apysc-3.2.5/apysc/_display/line_style_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/line_thickness_mixin.py` & `apysc-3.2.5/apysc/_display/line_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/parent_mixin.py` & `apysc-3.2.5/apysc/_display/parent_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/path.py` & `apysc-3.2.5/apysc/_display/path.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/points_2d_mixin.py` & `apysc-3.2.5/apysc/_display/points_2d_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/polygon.py` & `apysc-3.2.5/apysc/_display/polygon.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/polygon_append_constructor_expression_mixin.py` & `apysc-3.2.5/apysc/_display/polygon_append_constructor_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/polygon_apply_current_points_mixin.py` & `apysc-3.2.5/apysc/_display/polygon_apply_current_points_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/polygon_x1_mixin.py` & `apysc-3.2.5/apysc/_display/polygon_x1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/polygon_x2_mixin.py` & `apysc-3.2.5/apysc/_display/polygon_x2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/polygon_x3_mixin.py` & `apysc-3.2.5/apysc/_display/polygon_x3_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/polygon_y1_mixin.py` & `apysc-3.2.5/apysc/_display/polygon_y1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/polygon_y2_mixin.py` & `apysc-3.2.5/apysc/_display/polygon_y2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/polygon_y3_mixin.py` & `apysc-3.2.5/apysc/_display/polygon_y3_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/polyline.py` & `apysc-3.2.5/apysc/_display/polyline.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/radius_mixin.py` & `apysc-3.2.5/apysc/_display/radius_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/rectangle.py` & `apysc-3.2.5/apysc/_display/rectangle.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/rotation_around_center_mixin.py` & `apysc-3.2.5/apysc/_display/rotation_around_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/rotation_around_point_mixin.py` & `apysc-3.2.5/apysc/_display/rotation_around_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/rotation_interface_helper.py` & `apysc-3.2.5/apysc/_display/rotation_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/scale_interface_helper.py` & `apysc-3.2.5/apysc/_display/scale_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/scale_x_from_center_mixin.py` & `apysc-3.2.5/apysc/_display/scale_x_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/scale_x_from_point_mixin.py` & `apysc-3.2.5/apysc/_display/scale_x_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/scale_y_from_center_mixin.py` & `apysc-3.2.5/apysc/_display/scale_y_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/scale_y_from_point_mixin.py` & `apysc-3.2.5/apysc/_display/scale_y_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/set_lower_scale_limit_mixin.py` & `apysc-3.2.5/apysc/_display/set_lower_scale_limit_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/set_overflow_visible_setting_mixin.py` & `apysc-3.2.5/apysc/_display/set_overflow_visible_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/skew_x_mixin.py` & `apysc-3.2.5/apysc/_display/skew_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/skew_y_mixin.py` & `apysc-3.2.5/apysc/_display/skew_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/sprite.py` & `apysc-3.2.5/apysc/_display/sprite.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/stage.py` & `apysc-3.2.5/apysc/_display/stage.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text.py` & `apysc-3.2.5/apysc/_display/svg_text.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_align_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_align_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_bold_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_delta_x_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_delta_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_delta_y_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_delta_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_font_family_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_font_size_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_font_size_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_italic_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_leading_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_leading_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_set_align_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_set_align_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_set_bold_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_set_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_set_delta_x_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_set_delta_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_set_delta_y_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_set_delta_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_set_font_family_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_set_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_set_font_size_value_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_set_font_size_value_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_set_italic_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_set_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_set_leading_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_set_leading_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_set_text_value_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_set_text_value_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_singleton_for_text_span.py` & `apysc-3.2.5/apysc/_display/svg_text_singleton_for_text_span.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_span.py` & `apysc-3.2.5/apysc/_display/svg_text_span.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/svg_text_text_mixin.py` & `apysc-3.2.5/apysc/_display/svg_text_text_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/triangle.py` & `apysc-3.2.5/apysc/_display/triangle.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/visible_mixin.py` & `apysc-3.2.5/apysc/_display/visible_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/width_and_height_mixin_for_ellipse.py` & `apysc-3.2.5/apysc/_display/width_and_height_mixin_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/width_mixin.py` & `apysc-3.2.5/apysc/_display/width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/x_interface.py` & `apysc-3.2.5/apysc/_display/x_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/x_mixin.py` & `apysc-3.2.5/apysc/_display/x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/y_interface.py` & `apysc-3.2.5/apysc/_display/y_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_display/y_mixin.py` & `apysc-3.2.5/apysc/_display/y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/animation_event.py` & `apysc-3.2.5/apysc/_event/animation_event.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/click_mixin.py` & `apysc-3.2.5/apysc/_event/click_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/custom_event_mixin.py` & `apysc-3.2.5/apysc/_event/custom_event_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/document_mouse_wheel_func.py` & `apysc-3.2.5/apysc/_event/document_mouse_wheel_func.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/double_click_mixin.py` & `apysc-3.2.5/apysc/_event/double_click_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/enter_frame_event.py` & `apysc-3.2.5/apysc/_event/enter_frame_event.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/enter_frame_mixin.py` & `apysc-3.2.5/apysc/_event/enter_frame_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/event.py` & `apysc-3.2.5/apysc/_event/event.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/handler.py` & `apysc-3.2.5/apysc/_event/handler.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/handler_circular_calling_util.py` & `apysc-3.2.5/apysc/_event/handler_circular_calling_util.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/mouse_down_mixin.py` & `apysc-3.2.5/apysc/_event/mouse_down_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/mouse_event.py` & `apysc-3.2.5/apysc/_event/mouse_event.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/mouse_event_binding_expression_mixin.py` & `apysc-3.2.5/apysc/_event/mouse_event_binding_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/mouse_event_mixins.py` & `apysc-3.2.5/apysc/_event/mouse_event_mixins.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/mouse_event_unbinding_mixin.py` & `apysc-3.2.5/apysc/_event/mouse_event_unbinding_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/mouse_move_mixin.py` & `apysc-3.2.5/apysc/_event/mouse_move_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/mouse_out_mixin.py` & `apysc-3.2.5/apysc/_event/mouse_out_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/mouse_over_mixin.py` & `apysc-3.2.5/apysc/_event/mouse_over_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/mouse_up_mixin.py` & `apysc-3.2.5/apysc/_event/mouse_up_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/prevent_default_mixin.py` & `apysc-3.2.5/apysc/_event/prevent_default_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/set_handler_data_mixin.py` & `apysc-3.2.5/apysc/_event/set_handler_data_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/stop_propagation_mixin.py` & `apysc-3.2.5/apysc/_event/stop_propagation_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/timer_event.py` & `apysc-3.2.5/apysc/_event/timer_event.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_event/wheel_event.py` & `apysc-3.2.5/apysc/_event/wheel_event.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_expression/event_handler_scope.py` & `apysc-3.2.5/apysc/_expression/event_handler_scope.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_expression/expression_data_util.py` & `apysc-3.2.5/apysc/_expression/expression_data_util.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_expression/expression_variables_util.py` & `apysc-3.2.5/apysc/_expression/expression_variables_util.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_expression/indent_num.py` & `apysc-3.2.5/apysc/_expression/indent_num.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_expression/js_functions.py` & `apysc-3.2.5/apysc/_expression/js_functions.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_expression/last_scope.py` & `apysc-3.2.5/apysc/_expression/last_scope.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_expression/var_names.py` & `apysc-3.2.5/apysc/_expression/var_names.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_file/file_util.py` & `apysc-3.2.5/apysc/_file/file_util.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_file/module_util.py` & `apysc-3.2.5/apysc/_file/module_util.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_bezier_2d.py` & `apysc-3.2.5/apysc/_geom/path_bezier_2d.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_bezier_2d_continual.py` & `apysc-3.2.5/apysc/_geom/path_bezier_2d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_bezier_3d.py` & `apysc-3.2.5/apysc/_geom/path_bezier_3d.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_bezier_3d_continual.py` & `apysc-3.2.5/apysc/_geom/path_bezier_3d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_close.py` & `apysc-3.2.5/apysc/_geom/path_close.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_control_x1_mixin.py` & `apysc-3.2.5/apysc/_geom/path_control_x1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_control_x2_mixin.py` & `apysc-3.2.5/apysc/_geom/path_control_x2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_control_x_mixin.py` & `apysc-3.2.5/apysc/_geom/path_control_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_control_y1_mixin.py` & `apysc-3.2.5/apysc/_geom/path_control_y1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_control_y2_mixin.py` & `apysc-3.2.5/apysc/_geom/path_control_y2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_control_y_mixin.py` & `apysc-3.2.5/apysc/_geom/path_control_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_data.py` & `apysc-3.2.5/apysc/_geom/path_data.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_data_base.py` & `apysc-3.2.5/apysc/_geom/path_data_base.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_data_util.py` & `apysc-3.2.5/apysc/_geom/path_data_util.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_dest_x_mixin.py` & `apysc-3.2.5/apysc/_geom/path_dest_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_dest_y_mixin.py` & `apysc-3.2.5/apysc/_geom/path_dest_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_horizontal.py` & `apysc-3.2.5/apysc/_geom/path_horizontal.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_line_to.py` & `apysc-3.2.5/apysc/_geom/path_line_to.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_move_to.py` & `apysc-3.2.5/apysc/_geom/path_move_to.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_vertical.py` & `apysc-3.2.5/apysc/_geom/path_vertical.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_x_mixin.py` & `apysc-3.2.5/apysc/_geom/path_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/path_y_mixin.py` & `apysc-3.2.5/apysc/_geom/path_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/point2d.py` & `apysc-3.2.5/apysc/_geom/point2d.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/rectangle_geom.py` & `apysc-3.2.5/apysc/_geom/rectangle_geom.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/rectangle_geom_bottom_y_mixin.py` & `apysc-3.2.5/apysc/_geom/rectangle_geom_bottom_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/rectangle_geom_center_x_mixin.py` & `apysc-3.2.5/apysc/_geom/rectangle_geom_center_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/rectangle_geom_center_y_mixin.py` & `apysc-3.2.5/apysc/_geom/rectangle_geom_center_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/rectangle_geom_height_mixin.py` & `apysc-3.2.5/apysc/_geom/rectangle_geom_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/rectangle_geom_left_x_mixin.py` & `apysc-3.2.5/apysc/_geom/rectangle_geom_left_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/rectangle_geom_right_x_mixin.py` & `apysc-3.2.5/apysc/_geom/rectangle_geom_right_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/rectangle_geom_top_y_mixin.py` & `apysc-3.2.5/apysc/_geom/rectangle_geom_top_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/rectangle_geom_width_mixin.py` & `apysc-3.2.5/apysc/_geom/rectangle_geom_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_geom/relative_mixin.py` & `apysc-3.2.5/apysc/_geom/relative_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_html/debug_mode.py` & `apysc-3.2.5/apysc/_html/debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_html/exporter.py` & `apysc-3.2.5/apysc/_html/exporter.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_html/html_util.py` & `apysc-3.2.5/apysc/_html/html_util.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_jslib/jquery-3.6.3.min.js` & `apysc-3.2.5/apysc/_jslib/jquery-3.6.3.min.js`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_jslib/jquery.mousewheel-3.1.13.min.js` & `apysc-3.2.5/apysc/_jslib/jquery.mousewheel-3.1.13.min.js`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_jslib/jslib_util.py` & `apysc-3.2.5/apysc/_jslib/jslib_util.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_jslib/svg-3.1.2.min.js` & `apysc-3.2.5/apysc/_jslib/svg-3.1.2.min.js`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_jslib/underscore-1.12.0.min.js` & `apysc-3.2.5/apysc/_jslib/underscore-1.12.0.min.js`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_jupyter/jupyter_util.py` & `apysc-3.2.5/apysc/_jupyter/jupyter_util.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py` & `apysc-3.2.5/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_lint_and_doc/conf_common.py` & `apysc-3.2.5/apysc/_lint_and_doc/conf_common.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_lint_and_doc/docs_keyword_link_mapping.py` & `apysc-3.2.5/apysc/_lint_and_doc/docs_keyword_link_mapping.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_lint_and_doc/docs_lang.py` & `apysc-3.2.5/apysc/_lint_and_doc/docs_lang.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_lint_and_doc/docs_toctree_util.py` & `apysc-3.2.5/apysc/_lint_and_doc/docs_toctree_util.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_lint_and_doc/docs_translation_converter.py` & `apysc-3.2.5/apysc/_lint_and_doc/docs_translation_converter.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_lint_and_doc/docstring_to_markdown_converter.py` & `apysc-3.2.5/apysc/_lint_and_doc/docstring_to_markdown_converter.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_lint_and_doc/docstring_util.py` & `apysc-3.2.5/apysc/_lint_and_doc/docstring_util.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_lint_and_doc/document_text_split_util.py` & `apysc-3.2.5/apysc/_lint_and_doc/document_text_split_util.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_lint_and_doc/document_util.py` & `apysc-3.2.5/apysc/_lint_and_doc/document_util.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py` & `apysc-3.2.5/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_lint_and_doc/fixed_translation_mapping/jp.py` & `apysc-3.2.5/apysc/_lint_and_doc/fixed_translation_mapping/jp.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_lint_and_doc/lint_and_doc_hash_util.py` & `apysc-3.2.5/apysc/_lint_and_doc/lint_and_doc_hash_util.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_lint_and_doc/translation_mapping_utils.py` & `apysc-3.2.5/apysc/_lint_and_doc/translation_mapping_utils.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_loop/_continue.py` & `apysc-3.2.5/apysc/_loop/_continue.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_loop/_range.py` & `apysc-3.2.5/apysc/_loop/_range.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_loop/for_array_indices.py` & `apysc-3.2.5/apysc/_loop/for_array_indices.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_loop/for_array_indices_and_values.py` & `apysc-3.2.5/apysc/_loop/for_array_indices_and_values.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_loop/for_array_values.py` & `apysc-3.2.5/apysc/_loop/for_array_values.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_loop/for_dict_keys.py` & `apysc-3.2.5/apysc/_loop/for_dict_keys.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_loop/for_dict_keys_and_values.py` & `apysc-3.2.5/apysc/_loop/for_dict_keys_and_values.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_loop/for_dict_values.py` & `apysc-3.2.5/apysc/_loop/for_dict_values.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_loop/for_loop_exit_mixin.py` & `apysc-3.2.5/apysc/_loop/for_loop_exit_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_loop/initialize_for_loop_key_or_value_interface.py` & `apysc-3.2.5/apysc/_loop/initialize_for_loop_key_or_value_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_loop/loop_count.py` & `apysc-3.2.5/apysc/_loop/loop_count.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_math/max_mixin.py` & `apysc-3.2.5/apysc/_math/max_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_math/min_mixin.py` & `apysc-3.2.5/apysc/_math/min_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_math/trunc_mixin.py` & `apysc-3.2.5/apysc/_math/trunc_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_string/indent_util.py` & `apysc-3.2.5/apysc/_string/indent_util.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_string/string_util.py` & `apysc-3.2.5/apysc/_string/string_util.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_testing/e2e_testing_helper.py` & `apysc-3.2.5/apysc/_testing/e2e_testing_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_testing/testing_helper.py` & `apysc-3.2.5/apysc/_testing/testing_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_time/datetime_.py` & `apysc-3.2.5/apysc/_time/datetime_.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_time/day_mixin.py` & `apysc-3.2.5/apysc/_time/day_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_time/days_mixin.py` & `apysc-3.2.5/apysc/_time/days_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_time/fps.py` & `apysc-3.2.5/apysc/_time/fps.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_time/hour_mixin.py` & `apysc-3.2.5/apysc/_time/hour_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_time/left_and_right_datetimes_mixin.py` & `apysc-3.2.5/apysc/_time/left_and_right_datetimes_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_time/millisecond_mixin.py` & `apysc-3.2.5/apysc/_time/millisecond_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_time/minute_mixin.py` & `apysc-3.2.5/apysc/_time/minute_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_time/month_end_mixin.py` & `apysc-3.2.5/apysc/_time/month_end_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_time/month_mixin.py` & `apysc-3.2.5/apysc/_time/month_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_time/now_mixin.py` & `apysc-3.2.5/apysc/_time/now_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_time/second_mixin.py` & `apysc-3.2.5/apysc/_time/second_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_time/timedelta_.py` & `apysc-3.2.5/apysc/_time/timedelta_.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_time/timer.py` & `apysc-3.2.5/apysc/_time/timer.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_time/total_seconds_mixin.py` & `apysc-3.2.5/apysc/_time/total_seconds_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_time/weekday_mixin.py` & `apysc-3.2.5/apysc/_time/weekday_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_time/year_mixin.py` & `apysc-3.2.5/apysc/_time/year_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/about_handler_options_type.py` & `apysc-3.2.5/apysc/_translation/jp/about_handler_options_type.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/add_child_and_remove_child.py` & `apysc-3.2.5/apysc/_translation/jp/add_child_and_remove_child.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/add_debug_info_setting.py` & `apysc-3.2.5/apysc/_translation/jp/add_debug_info_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_base_start.py` & `apysc-3.2.5/apysc/_translation/jp/animation_base_start.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_base_target.py` & `apysc-3.2.5/apysc/_translation/jp/animation_base_target.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_complete.py` & `apysc-3.2.5/apysc/_translation/jp/animation_complete.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_delay.py` & `apysc-3.2.5/apysc/_translation/jp/animation_delay.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_duration.py` & `apysc-3.2.5/apysc/_translation/jp/animation_duration.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_event.py` & `apysc-3.2.5/apysc/_translation/jp/animation_event.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_fill_alpha.py` & `apysc-3.2.5/apysc/_translation/jp/animation_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_fill_color.py` & `apysc-3.2.5/apysc/_translation/jp/animation_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_finish.py` & `apysc-3.2.5/apysc/_translation/jp/animation_finish.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_interfaces_abstract.py` & `apysc-3.2.5/apysc/_translation/jp/animation_interfaces_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_line_alpha.py` & `apysc-3.2.5/apysc/_translation/jp/animation_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_line_color.py` & `apysc-3.2.5/apysc/_translation/jp/animation_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_line_thickness.py` & `apysc-3.2.5/apysc/_translation/jp/animation_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_method_chaining.py` & `apysc-3.2.5/apysc/_translation/jp/animation_method_chaining.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_move.py` & `apysc-3.2.5/apysc/_translation/jp/animation_move.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_parallel.py` & `apysc-3.2.5/apysc/_translation/jp/animation_parallel.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_pause_and_play.py` & `apysc-3.2.5/apysc/_translation/jp/animation_pause_and_play.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_radius.py` & `apysc-3.2.5/apysc/_translation/jp/animation_radius.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_reset.py` & `apysc-3.2.5/apysc/_translation/jp/animation_reset.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_return_value.py` & `apysc-3.2.5/apysc/_translation/jp/animation_return_value.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_reverse.py` & `apysc-3.2.5/apysc/_translation/jp/animation_reverse.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_rotation_around_center.py` & `apysc-3.2.5/apysc/_translation/jp/animation_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_rotation_around_point.py` & `apysc-3.2.5/apysc/_translation/jp/animation_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_scale_x_and_y_from_center.py` & `apysc-3.2.5/apysc/_translation/jp/animation_scale_x_and_y_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_scale_x_and_y_from_point.py` & `apysc-3.2.5/apysc/_translation/jp/animation_scale_x_and_y_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_time.py` & `apysc-3.2.5/apysc/_translation/jp/animation_time.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_width_and_height.py` & `apysc-3.2.5/apysc/_translation/jp/animation_width_and_height.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_x.py` & `apysc-3.2.5/apysc/_translation/jp/animation_x.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/animation_y.py` & `apysc-3.2.5/apysc/_translation/jp/animation_y.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/append_js_expression.py` & `apysc-3.2.5/apysc/_translation/jp/append_js_expression.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/array.py` & `apysc-3.2.5/apysc/_translation/jp/array.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/array_append_and_push.py` & `apysc-3.2.5/apysc/_translation/jp/array_append_and_push.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/array_clear.py` & `apysc-3.2.5/apysc/_translation/jp/array_clear.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/array_comparison.py` & `apysc-3.2.5/apysc/_translation/jp/array_comparison.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/array_extend_and_concat.py` & `apysc-3.2.5/apysc/_translation/jp/array_extend_and_concat.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/array_index_of.py` & `apysc-3.2.5/apysc/_translation/jp/array_index_of.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/array_insert_and_insert_at.py` & `apysc-3.2.5/apysc/_translation/jp/array_insert_and_insert_at.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/array_join.py` & `apysc-3.2.5/apysc/_translation/jp/array_join.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/array_length.py` & `apysc-3.2.5/apysc/_translation/jp/array_length.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/array_pop.py` & `apysc-3.2.5/apysc/_translation/jp/array_pop.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/array_remove_and_remove_at.py` & `apysc-3.2.5/apysc/_translation/jp/array_remove_and_remove_at.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/array_reverse.py` & `apysc-3.2.5/apysc/_translation/jp/array_reverse.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/array_slice.py` & `apysc-3.2.5/apysc/_translation/jp/array_slice.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/array_sort.py` & `apysc-3.2.5/apysc/_translation/jp/array_sort.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py` & `apysc-3.2.5/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/assert_defined_and_undefined.py` & `apysc-3.2.5/apysc/_translation/jp/assert_defined_and_undefined.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py` & `apysc-3.2.5/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/assert_equal_and_not_equal.py` & `apysc-3.2.5/apysc/_translation/jp/assert_equal_and_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/assert_greater_and_greater_equal.py` & `apysc-3.2.5/apysc/_translation/jp/assert_greater_and_greater_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/assert_less_and_less_equal.py` & `apysc-3.2.5/apysc/_translation/jp/assert_less_and_less_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/assert_true_and_false.py` & `apysc-3.2.5/apysc/_translation/jp/assert_true_and_false.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/assertion_basic_behavior.py` & `apysc-3.2.5/apysc/_translation/jp/assertion_basic_behavior.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/bind_and_trigger_custom_event.py` & `apysc-3.2.5/apysc/_translation/jp/bind_and_trigger_custom_event.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/boolean.py` & `apysc-3.2.5/apysc/_translation/jp/boolean.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py` & `apysc-3.2.5/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/circle.py` & `apysc-3.2.5/apysc/_translation/jp/circle.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/click.py` & `apysc-3.2.5/apysc/_translation/jp/click.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/contains.py` & `apysc-3.2.5/apysc/_translation/jp/contains.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/continue.py` & `apysc-3.2.5/apysc/_translation/jp/continue.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/datetime.py` & `apysc-3.2.5/apysc/_translation/jp/datetime.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/datetime_day.py` & `apysc-3.2.5/apysc/_translation/jp/datetime_day.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/datetime_hour.py` & `apysc-3.2.5/apysc/_translation/jp/datetime_hour.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/datetime_millisecond.py` & `apysc-3.2.5/apysc/_translation/jp/datetime_millisecond.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/datetime_minute.py` & `apysc-3.2.5/apysc/_translation/jp/datetime_minute.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/datetime_month.py` & `apysc-3.2.5/apysc/_translation/jp/datetime_month.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/datetime_now.py` & `apysc-3.2.5/apysc/_translation/jp/datetime_now.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/datetime_second.py` & `apysc-3.2.5/apysc/_translation/jp/datetime_second.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/datetime_set_month_end.py` & `apysc-3.2.5/apysc/_translation/jp/datetime_set_month_end.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py` & `apysc-3.2.5/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/datetime_year.py` & `apysc-3.2.5/apysc/_translation/jp/datetime_year.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/dblclick.py` & `apysc-3.2.5/apysc/_translation/jp/dblclick.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/delete.py` & `apysc-3.2.5/apysc/_translation/jp/delete.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/dictionary.py` & `apysc-3.2.5/apysc/_translation/jp/dictionary.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/dictionary_generic.py` & `apysc-3.2.5/apysc/_translation/jp/dictionary_generic.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/dictionary_get.py` & `apysc-3.2.5/apysc/_translation/jp/dictionary_get.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/dictionary_length.py` & `apysc-3.2.5/apysc/_translation/jp/dictionary_length.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/display_object.py` & `apysc-3.2.5/apysc/_translation/jp/display_object.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py` & `apysc-3.2.5/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/display_object_get_and_set_css.py` & `apysc-3.2.5/apysc/_translation/jp/display_object_get_and_set_css.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/display_object_mouse_event.py` & `apysc-3.2.5/apysc/_translation/jp/display_object_mouse_event.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/display_object_parent.py` & `apysc-3.2.5/apysc/_translation/jp/display_object_parent.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/display_object_visible.py` & `apysc-3.2.5/apysc/_translation/jp/display_object_visible.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/display_object_x_and_y.py` & `apysc-3.2.5/apysc/_translation/jp/display_object_x_and_y.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/display_on_colaboratory.py` & `apysc-3.2.5/apysc/_translation/jp/display_on_colaboratory.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/display_on_jupyter.py` & `apysc-3.2.5/apysc/_translation/jp/display_on_jupyter.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/draw_interfaces_abstract.py` & `apysc-3.2.5/apysc/_translation/jp/draw_interfaces_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/easing_enum.py` & `apysc-3.2.5/apysc/_translation/jp/easing_enum.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/elif.py` & `apysc-3.2.5/apysc/_translation/jp/elif.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/ellipse.py` & `apysc-3.2.5/apysc/_translation/jp/ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/else.py` & `apysc-3.2.5/apysc/_translation/jp/else.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/enter_frame.py` & `apysc-3.2.5/apysc/_translation/jp/enter_frame.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py` & `apysc-3.2.5/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/for_array_indices.py` & `apysc-3.2.5/apysc/_translation/jp/for_array_indices.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/for_array_indices_and_values.py` & `apysc-3.2.5/apysc/_translation/jp/for_array_indices_and_values.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/for_array_values.py` & `apysc-3.2.5/apysc/_translation/jp/for_array_values.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/for_dict_keys.py` & `apysc-3.2.5/apysc/_translation/jp/for_dict_keys.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/for_dict_keys_and_values.py` & `apysc-3.2.5/apysc/_translation/jp/for_dict_keys_and_values.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/for_dict_values.py` & `apysc-3.2.5/apysc/_translation/jp/for_dict_values.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/fps.py` & `apysc-3.2.5/apysc/_translation/jp/fps.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/fundamental_data_classes_value_interface.py` & `apysc-3.2.5/apysc/_translation/jp/fundamental_data_classes_value_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/get_bounds.py` & `apysc-3.2.5/apysc/_translation/jp/get_bounds.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/get_child_at.py` & `apysc-3.2.5/apysc/_translation/jp/get_child_at.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics.py` & `apysc-3.2.5/apysc/_translation/jp/graphics.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_base_fill_alpha.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_base_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_base_fill_color.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_base_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_base_flip_interfaces.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_base_flip_interfaces.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_base_line_alpha.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_base_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_base_line_color.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_base_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_base_line_dash_setting.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_base_line_dash_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_base_line_dot_setting.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_base_line_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_base_line_round_dot_setting.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_base_line_round_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_base_line_thickness.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_base_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_base_rotation_around_center.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_base_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_base_rotation_around_point.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_base_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_base_scale_from_center.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_base_scale_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_base_scale_from_point.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_base_scale_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_base_skew.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_base_skew.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_begin_fill.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_begin_fill.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_clear.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_clear.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_draw_circle.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_draw_circle.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_draw_dash_dotted_line.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_draw_dash_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_draw_dashed_line.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_draw_dashed_line.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_draw_dotted_line.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_draw_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_draw_ellipse.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_draw_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_draw_line.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_draw_line.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_draw_path.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_draw_path.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_draw_polygon.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_draw_polygon.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_draw_rect.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_draw_rect.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_draw_round_dotted_line.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_draw_round_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_draw_round_rect.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_draw_round_rect.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_draw_triangle.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_draw_triangle.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_line_style.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_line_style.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/graphics_move_to_and_line_to.py` & `apysc-3.2.5/apysc/_translation/jp/graphics_move_to_and_line_to.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/if.py` & `apysc-3.2.5/apysc/_translation/jp/if.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/import_conventions.py` & `apysc-3.2.5/apysc/_translation/jp/import_conventions.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/index.py` & `apysc-3.2.5/apysc/_translation/jp/index.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/int_and_number.py` & `apysc-3.2.5/apysc/_translation/jp/int_and_number.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/int_and_number_arithmetic_operations.py` & `apysc-3.2.5/apysc/_translation/jp/int_and_number_arithmetic_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/int_and_number_comparison_operations.py` & `apysc-3.2.5/apysc/_translation/jp/int_and_number_comparison_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/int_and_number_to_fixed.py` & `apysc-3.2.5/apysc/_translation/jp/int_and_number_to_fixed.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/line.py` & `apysc-3.2.5/apysc/_translation/jp/line.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/math_max.py` & `apysc-3.2.5/apysc/_translation/jp/math_max.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/math_min.py` & `apysc-3.2.5/apysc/_translation/jp/math_min.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/math_trunc.py` & `apysc-3.2.5/apysc/_translation/jp/math_trunc.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/mouse_event_abstract.py` & `apysc-3.2.5/apysc/_translation/jp/mouse_event_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/mouse_event_basic.py` & `apysc-3.2.5/apysc/_translation/jp/mouse_event_basic.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/mousedown_and_mouseup.py` & `apysc-3.2.5/apysc/_translation/jp/mousedown_and_mouseup.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/mousemove.py` & `apysc-3.2.5/apysc/_translation/jp/mousemove.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/mouseover_and_mouseout.py` & `apysc-3.2.5/apysc/_translation/jp/mouseover_and_mouseout.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/num_children.py` & `apysc-3.2.5/apysc/_translation/jp/num_children.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/path.py` & `apysc-3.2.5/apysc/_translation/jp/path.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/path_bezier_2d.py` & `apysc-3.2.5/apysc/_translation/jp/path_bezier_2d.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/path_bezier_2d_continual.py` & `apysc-3.2.5/apysc/_translation/jp/path_bezier_2d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/path_bezier_3d.py` & `apysc-3.2.5/apysc/_translation/jp/path_bezier_3d.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/path_bezier_3d_continual.py` & `apysc-3.2.5/apysc/_translation/jp/path_bezier_3d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/path_close.py` & `apysc-3.2.5/apysc/_translation/jp/path_close.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/path_horizontal.py` & `apysc-3.2.5/apysc/_translation/jp/path_horizontal.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/path_line_to.py` & `apysc-3.2.5/apysc/_translation/jp/path_line_to.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/path_move_to.py` & `apysc-3.2.5/apysc/_translation/jp/path_move_to.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/path_vertical.py` & `apysc-3.2.5/apysc/_translation/jp/path_vertical.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/point2d.py` & `apysc-3.2.5/apysc/_translation/jp/point2d.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/polygon.py` & `apysc-3.2.5/apysc/_translation/jp/polygon.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/polyline.py` & `apysc-3.2.5/apysc/_translation/jp/polyline.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/quick_start.py` & `apysc-3.2.5/apysc/_translation/jp/quick_start.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/range.py` & `apysc-3.2.5/apysc/_translation/jp/range.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/recommended_type_checker_settings.py` & `apysc-3.2.5/apysc/_translation/jp/recommended_type_checker_settings.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/rectangle.py` & `apysc-3.2.5/apysc/_translation/jp/rectangle.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/rectangle_geom.py` & `apysc-3.2.5/apysc/_translation/jp/rectangle_geom.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/remove_children.py` & `apysc-3.2.5/apysc/_translation/jp/remove_children.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/return.py` & `apysc-3.2.5/apysc/_translation/jp/return.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/save_overall_html.py` & `apysc-3.2.5/apysc/_translation/jp/save_overall_html.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/sequential_animation.py` & `apysc-3.2.5/apysc/_translation/jp/sequential_animation.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/set_debug_mode.py` & `apysc-3.2.5/apysc/_translation/jp/set_debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/sprite.py` & `apysc-3.2.5/apysc/_translation/jp/sprite.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/stage.py` & `apysc-3.2.5/apysc/_translation/jp/stage.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/string.py` & `apysc-3.2.5/apysc/_translation/jp/string.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/string_addition_and_multiplication.py` & `apysc-3.2.5/apysc/_translation/jp/string_addition_and_multiplication.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/string_apply_max_num_of_decimal_places.py` & `apysc-3.2.5/apysc/_translation/jp/string_apply_max_num_of_decimal_places.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/string_comparison_operations.py` & `apysc-3.2.5/apysc/_translation/jp/string_comparison_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/string_length.py` & `apysc-3.2.5/apysc/_translation/jp/string_length.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/string_lstrip.py` & `apysc-3.2.5/apysc/_translation/jp/string_lstrip.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/string_rstrip.py` & `apysc-3.2.5/apysc/_translation/jp/string_rstrip.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/string_split.py` & `apysc-3.2.5/apysc/_translation/jp/string_split.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/string_strip.py` & `apysc-3.2.5/apysc/_translation/jp/string_strip.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/svg_text.py` & `apysc-3.2.5/apysc/_translation/jp/svg_text.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/svg_text_span.py` & `apysc-3.2.5/apysc/_translation/jp/svg_text_span.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/timedelta.py` & `apysc-3.2.5/apysc/_translation/jp/timedelta.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/timedelta_days.py` & `apysc-3.2.5/apysc/_translation/jp/timedelta_days.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/timedelta_total_seconds.py` & `apysc-3.2.5/apysc/_translation/jp/timedelta_total_seconds.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/timer.py` & `apysc-3.2.5/apysc/_translation/jp/timer.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/timer_complete.py` & `apysc-3.2.5/apysc/_translation/jp/timer_complete.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/timer_delay.py` & `apysc-3.2.5/apysc/_translation/jp/timer_delay.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/timer_event.py` & `apysc-3.2.5/apysc/_translation/jp/timer_event.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/timer_repeat_count.py` & `apysc-3.2.5/apysc/_translation/jp/timer_repeat_count.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/timer_reset.py` & `apysc-3.2.5/apysc/_translation/jp/timer_reset.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/timer_start_and_stop.py` & `apysc-3.2.5/apysc/_translation/jp/timer_start_and_stop.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/to_string.py` & `apysc-3.2.5/apysc/_translation/jp/to_string.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/trace.py` & `apysc-3.2.5/apysc/_translation/jp/trace.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/triangle.py` & `apysc-3.2.5/apysc/_translation/jp/triangle.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/true_and_false.py` & `apysc-3.2.5/apysc/_translation/jp/true_and_false.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py` & `apysc-3.2.5/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/unset_debug_mode.py` & `apysc-3.2.5/apysc/_translation/jp/unset_debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/variable_name_suffix.py` & `apysc-3.2.5/apysc/_translation/jp/variable_name_suffix.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/what_apysc_can_do.py` & `apysc-3.2.5/apysc/_translation/jp/what_apysc_can_do.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py` & `apysc-3.2.5/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/_delete.py` & `apysc-3.2.5/apysc/_type/_delete.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/_return.py` & `apysc-3.2.5/apysc/_type/_return.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/any_value.py` & `apysc-3.2.5/apysc/_type/any_value.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/array.py` & `apysc-3.2.5/apysc/_type/array.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/attr_linking_mixin.py` & `apysc-3.2.5/apysc/_type/attr_linking_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py` & `apysc-3.2.5/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/blank_object_mixin.py` & `apysc-3.2.5/apysc/_type/blank_object_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/bool_const_mixin.py` & `apysc-3.2.5/apysc/_type/bool_const_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/boolean.py` & `apysc-3.2.5/apysc/_type/boolean.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/copy_mixin.py` & `apysc-3.2.5/apysc/_type/copy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/deleted_object_mixin.py` & `apysc-3.2.5/apysc/_type/deleted_object_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/dictionary.py` & `apysc-3.2.5/apysc/_type/dictionary.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/expression_string.py` & `apysc-3.2.5/apysc/_type/expression_string.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/false.py` & `apysc-3.2.5/apysc/_type/false.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/initial_substitution_exp_mixin.py` & `apysc-3.2.5/apysc/_type/initial_substitution_exp_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/initialize_locals_and_globals_mixin.py` & `apysc-3.2.5/apysc/_type/initialize_locals_and_globals_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/initialize_top_level_constants_mixin.py` & `apysc-3.2.5/apysc/_type/initialize_top_level_constants_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/int.py` & `apysc-3.2.5/apysc/_type/int.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/number.py` & `apysc-3.2.5/apysc/_type/number.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/number_value_mixin.py` & `apysc-3.2.5/apysc/_type/number_value_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/py_builtin_iter_disabling_mixin.py` & `apysc-3.2.5/apysc/_type/py_builtin_iter_disabling_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/revert_interface.py` & `apysc-3.2.5/apysc/_type/revert_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/revert_mixin.py` & `apysc-3.2.5/apysc/_type/revert_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/string.py` & `apysc-3.2.5/apysc/_type/string.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/string_apply_max_num_of_decimal_places_mixin.py` & `apysc-3.2.5/apysc/_type/string_apply_max_num_of_decimal_places_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/string_length_mixin.py` & `apysc-3.2.5/apysc/_type/string_length_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/string_lstrip_mixin.py` & `apysc-3.2.5/apysc/_type/string_lstrip_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/string_rstrip_mixin.py` & `apysc-3.2.5/apysc/_type/string_rstrip_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/string_split_mixin.py` & `apysc-3.2.5/apysc/_type/string_split_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/string_strip_mixin.py` & `apysc-3.2.5/apysc/_type/string_strip_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/to_fixed_mixin.py` & `apysc-3.2.5/apysc/_type/to_fixed_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/to_number_mixin.py` & `apysc-3.2.5/apysc/_type/to_number_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/to_string_mixin.py` & `apysc-3.2.5/apysc/_type/to_string_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/true.py` & `apysc-3.2.5/apysc/_type/true.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/type_util.py` & `apysc-3.2.5/apysc/_type/type_util.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/value_util.py` & `apysc-3.2.5/apysc/_type/value_util.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/variable_name_mixin.py` & `apysc-3.2.5/apysc/_type/variable_name_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/variable_name_suffix_attr_or_var_mixin.py` & `apysc-3.2.5/apysc/_type/variable_name_suffix_attr_or_var_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/variable_name_suffix_mixin.py` & `apysc-3.2.5/apysc/_type/variable_name_suffix_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_type/variable_name_suffix_utils.py` & `apysc-3.2.5/apysc/_type/variable_name_suffix_utils.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_validation/arg_validation_decos.py` & `apysc-3.2.5/apysc/_validation/arg_validation_decos.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_validation/bool_validation.py` & `apysc-3.2.5/apysc/_validation/bool_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_validation/color_validation.py` & `apysc-3.2.5/apysc/_validation/color_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_validation/display_validation.py` & `apysc-3.2.5/apysc/_validation/display_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_validation/event_validation.py` & `apysc-3.2.5/apysc/_validation/event_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_validation/geom_validation.py` & `apysc-3.2.5/apysc/_validation/geom_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_validation/handler_validation.py` & `apysc-3.2.5/apysc/_validation/handler_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_validation/matrix_data_validation.py` & `apysc-3.2.5/apysc/_validation/matrix_data_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_validation/number_validation.py` & `apysc-3.2.5/apysc/_validation/number_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_validation/parent_validation.py` & `apysc-3.2.5/apysc/_validation/parent_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_validation/path_validation.py` & `apysc-3.2.5/apysc/_validation/path_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_validation/string_validation.py` & `apysc-3.2.5/apysc/_validation/string_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_validation/validate_stage_is_created_mixin.py` & `apysc-3.2.5/apysc/_validation/validate_stage_is_created_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_validation/validation_common_utils.py` & `apysc-3.2.5/apysc/_validation/validation_common_utils.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc/_validation/variable_name_validation.py` & `apysc-3.2.5/apysc/_validation/variable_name_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-3.2.4/apysc.egg-info/PKG-INFO` & `apysc-3.2.5/apysc.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apysc
-Version: 3.2.4
+Version: 3.2.5
 Summary: apysc is the Python's frontend library to create html and js file, that has the ActionScript 3 (as3)-like interface.
 Home-page: https://github.com/simon-ritchie/apysc
 Maintainer: simon-ritchie
 Maintainer-email: 
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apysc-3.2.4/apysc.egg-info/SOURCES.txt` & `apysc-3.2.5/apysc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

