# Comparing `tmp/reflex-0.2.0a2.tar.gz` & `tmp/reflex-0.2.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.2.0a2.tar", max compression
+gzip compressed data, was "reflex-0.2.1a1.tar", max compression
```

## Comparing `reflex-0.2.0a2.tar` & `reflex-0.2.1a1.tar`

### file list

```diff
@@ -1,175 +1,177 @@
--rw-r--r--   0        0        0    11358 2023-06-27 19:44:11.125503 reflex-0.2.0a2/LICENSE
--rw-r--r--   0        0        0     8461 2023-06-27 19:44:11.125656 reflex-0.2.0a2/README.md
--rw-r--r--   0        0        0     1896 2023-06-30 17:42:25.432387 reflex-0.2.0a2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 19:44:11.128524 reflex-0.2.0a2/reflex/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1337 2023-06-27 19:44:11.128663 reflex-0.2.0a2/reflex/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-06-27 19:44:11.128732 reflex-0.2.0a2/reflex/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1226 2023-06-27 19:44:11.128954 reflex-0.2.0a2/reflex/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2023-06-27 19:44:11.129101 reflex-0.2.0a2/reflex/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      181 2023-06-27 19:44:11.129299 reflex-0.2.0a2/reflex/.templates/jinja/app/rxconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-06-27 19:44:11.129433 reflex-0.2.0a2/reflex/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-06-27 19:44:11.129488 reflex-0.2.0a2/reflex/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-06-27 19:44:11.129541 reflex-0.2.0a2/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     3312 2023-06-27 19:44:11.129632 reflex-0.2.0a2/reflex/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     3170 2023-06-27 19:44:11.129721 reflex-0.2.0a2/reflex/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      356 2023-06-27 19:44:11.129809 reflex-0.2.0a2/reflex/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0       38 2023-06-27 19:44:11.129890 reflex-0.2.0a2/reflex/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-06-27 19:44:11.129970 reflex-0.2.0a2/reflex/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   284503 2023-06-27 19:44:11.130872 reflex-0.2.0a2/reflex/.templates/web/bun.lockb
--rw-r--r--   0        0        0       50 2023-06-27 19:44:11.130961 reflex-0.2.0a2/reflex/.templates/web/jsconfig.json
--rw-r--r--   0        0        0       47 2023-06-27 19:44:11.131031 reflex-0.2.0a2/reflex/.templates/web/next.config.js
--rw-r--r--   0        0        0     1141 2023-06-27 19:44:11.131301 reflex-0.2.0a2/reflex/.templates/web/package.json
--rw-r--r--   0        0        0      502 2023-06-27 19:44:11.131463 reflex-0.2.0a2/reflex/.templates/web/pages/404.js
--rw-r--r--   0        0        0      597 2023-06-27 19:44:11.131568 reflex-0.2.0a2/reflex/.templates/web/pages/_app.js
--rw-r--r--   0        0        0       82 2023-06-27 19:44:11.131644 reflex-0.2.0a2/reflex/.templates/web/postcss.config.js
--rw-r--r--   0        0        0    29404 2023-06-27 19:44:11.131867 reflex-0.2.0a2/reflex/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0       59 2023-06-27 19:44:11.131951 reflex-0.2.0a2/reflex/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0     9656 2023-06-28 21:01:51.884154 reflex-0.2.0a2/reflex/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1917 2023-06-28 21:01:51.884307 reflex-0.2.0a2/reflex/__init__.py
--rw-r--r--   0        0        0      373 2023-06-28 01:25:19.553569 reflex-0.2.0a2/reflex/admin.py
--rw-r--r--   0        0        0    22302 2023-06-30 17:42:07.289348 reflex-0.2.0a2/reflex/app.py
--rw-r--r--   0        0        0     2438 2023-06-27 19:44:11.133013 reflex-0.2.0a2/reflex/base.py
--rw-r--r--   0        0        0       27 2023-06-27 19:44:11.133168 reflex-0.2.0a2/reflex/compiler/__init__.py
--rw-r--r--   0        0        0     7404 2023-06-30 17:42:07.289532 reflex-0.2.0a2/reflex/compiler/compiler.py
--rw-r--r--   0        0        0     2725 2023-06-27 19:44:11.133429 reflex-0.2.0a2/reflex/compiler/templates.py
--rw-r--r--   0        0        0     8502 2023-06-30 17:42:07.289680 reflex-0.2.0a2/reflex/compiler/utils.py
--rw-r--r--   0        0        0     7471 2023-06-27 19:44:11.134065 reflex-0.2.0a2/reflex/components/__init__.py
--rw-r--r--   0        0        0      229 2023-06-27 19:44:11.134184 reflex-0.2.0a2/reflex/components/base/__init__.py
--rw-r--r--   0        0        0      719 2023-06-27 19:44:11.134368 reflex-0.2.0a2/reflex/components/base/bare.py
--rw-r--r--   0        0        0      151 2023-06-27 19:44:11.134560 reflex-0.2.0a2/reflex/components/base/body.py
--rw-r--r--   0        0        0      721 2023-06-27 19:44:11.134715 reflex-0.2.0a2/reflex/components/base/document.py
--rw-r--r--   0        0        0      263 2023-06-27 19:44:11.134873 reflex-0.2.0a2/reflex/components/base/head.py
--rw-r--r--   0        0        0      929 2023-06-27 19:44:11.134990 reflex-0.2.0a2/reflex/components/base/link.py
--rw-r--r--   0        0        0     1408 2023-06-27 19:44:11.135110 reflex-0.2.0a2/reflex/components/base/meta.py
--rw-r--r--   0        0        0    24223 2023-06-27 19:44:11.135393 reflex-0.2.0a2/reflex/components/component.py
--rw-r--r--   0        0        0      496 2023-06-27 19:44:11.135502 reflex-0.2.0a2/reflex/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      330 2023-06-27 19:44:11.135630 reflex-0.2.0a2/reflex/components/datadisplay/badge.py
--rw-r--r--   0        0        0     3518 2023-06-30 17:42:07.289969 reflex-0.2.0a2/reflex/components/datadisplay/code.py
--rw-r--r--   0        0        0     4025 2023-06-27 19:44:11.136022 reflex-0.2.0a2/reflex/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      533 2023-06-27 19:44:11.136138 reflex-0.2.0a2/reflex/components/datadisplay/divider.py
--rw-r--r--   0        0        0      185 2023-06-27 19:44:11.136281 reflex-0.2.0a2/reflex/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1422 2023-06-27 19:44:11.136404 reflex-0.2.0a2/reflex/components/datadisplay/list.py
--rw-r--r--   0        0        0     2151 2023-06-27 19:44:11.136541 reflex-0.2.0a2/reflex/components/datadisplay/stat.py
--rw-r--r--   0        0        0     5785 2023-06-27 19:44:11.136687 reflex-0.2.0a2/reflex/components/datadisplay/table.py
--rw-r--r--   0        0        0     2182 2023-06-27 19:44:11.136854 reflex-0.2.0a2/reflex/components/datadisplay/tag.py
--rw-r--r--   0        0        0      384 2023-06-27 19:44:11.137000 reflex-0.2.0a2/reflex/components/disclosure/__init__.py
--rw-r--r--   0        0        0     3511 2023-06-27 19:44:11.137163 reflex-0.2.0a2/reflex/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2771 2023-06-27 19:44:11.137730 reflex-0.2.0a2/reflex/components/disclosure/tabs.py
--rw-r--r--   0        0        0     1737 2023-06-27 19:44:11.137878 reflex-0.2.0a2/reflex/components/disclosure/transition.py
--rw-r--r--   0        0        0      283 2023-06-27 19:44:11.138089 reflex-0.2.0a2/reflex/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2023-06-27 19:44:11.138179 reflex-0.2.0a2/reflex/components/feedback/__init__.py
--rw-r--r--   0        0        0     1565 2023-06-27 19:44:11.138437 reflex-0.2.0a2/reflex/components/feedback/alert.py
--rw-r--r--   0        0        0     1899 2023-06-27 19:44:11.138584 reflex-0.2.0a2/reflex/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      875 2023-06-27 19:44:11.138721 reflex-0.2.0a2/reflex/components/feedback/progress.py
--rw-r--r--   0        0        0     1781 2023-06-27 19:44:11.138852 reflex-0.2.0a2/reflex/components/feedback/skeleton.py
--rw-r--r--   0        0        0      674 2023-06-27 19:44:11.138989 reflex-0.2.0a2/reflex/components/feedback/spinner.py
--rw-r--r--   0        0        0     1471 2023-06-27 19:44:11.139091 reflex-0.2.0a2/reflex/components/forms/__init__.py
--rw-r--r--   0        0        0     1761 2023-06-27 19:44:11.139232 reflex-0.2.0a2/reflex/components/forms/button.py
--rw-r--r--   0        0        0     2448 2023-06-27 19:44:11.139361 reflex-0.2.0a2/reflex/components/forms/checkbox.py
--rw-r--r--   0        0        0     3137 2023-06-27 19:44:11.139608 reflex-0.2.0a2/reflex/components/forms/colormodeswitch.py
--rw-r--r--   0        0        0      574 2023-06-27 19:44:11.139743 reflex-0.2.0a2/reflex/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0      239 2023-06-27 19:44:11.139887 reflex-0.2.0a2/reflex/components/forms/date_picker.py
--rw-r--r--   0        0        0      273 2023-06-27 19:44:11.140156 reflex-0.2.0a2/reflex/components/forms/date_time_picker.py
--rw-r--r--   0        0        0     1943 2023-06-27 19:44:11.140298 reflex-0.2.0a2/reflex/components/forms/editable.py
--rw-r--r--   0        0        0      239 2023-06-27 19:44:11.140427 reflex-0.2.0a2/reflex/components/forms/email.py
--rw-r--r--   0        0        0     2990 2023-06-27 19:44:11.140597 reflex-0.2.0a2/reflex/components/forms/form.py
--rw-r--r--   0        0        0      798 2023-06-27 19:44:11.140858 reflex-0.2.0a2/reflex/components/forms/iconbutton.py
--rw-r--r--   0        0        0     2872 2023-06-27 19:44:11.140996 reflex-0.2.0a2/reflex/components/forms/input.py
--rw-r--r--   0        0        0    12659 2023-06-27 19:44:11.141249 reflex-0.2.0a2/reflex/components/forms/multiselect.py
--rw-r--r--   0        0        0     3889 2023-06-27 19:44:11.141372 reflex-0.2.0a2/reflex/components/forms/numberinput.py
--rw-r--r--   0        0        0      249 2023-06-27 19:44:11.141494 reflex-0.2.0a2/reflex/components/forms/password.py
--rw-r--r--   0        0        0     2662 2023-06-27 19:44:11.141620 reflex-0.2.0a2/reflex/components/forms/pininput.py
--rw-r--r--   0        0        0     3029 2023-06-27 19:44:11.141743 reflex-0.2.0a2/reflex/components/forms/radio.py
--rw-r--r--   0        0        0     2845 2023-06-27 19:44:11.141920 reflex-0.2.0a2/reflex/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3510 2023-06-27 19:44:11.142041 reflex-0.2.0a2/reflex/components/forms/select.py
--rw-r--r--   0        0        0     3116 2023-06-27 19:44:11.142160 reflex-0.2.0a2/reflex/components/forms/slider.py
--rw-r--r--   0        0        0     1567 2023-06-27 19:44:11.142316 reflex-0.2.0a2/reflex/components/forms/switch.py
--rw-r--r--   0        0        0     1526 2023-06-27 19:44:11.142445 reflex-0.2.0a2/reflex/components/forms/textarea.py
--rw-r--r--   0        0        0     2905 2023-06-27 19:44:11.142612 reflex-0.2.0a2/reflex/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-06-27 19:44:11.142690 reflex-0.2.0a2/reflex/components/graphing/__init__.py
--rw-r--r--   0        0        0     1351 2023-06-27 19:44:11.142821 reflex-0.2.0a2/reflex/components/graphing/plotly.py
--rw-r--r--   0        0        0    17354 2023-06-27 19:44:11.143107 reflex-0.2.0a2/reflex/components/graphing/victory.py
--rw-r--r--   0        0        0      872 2023-06-27 19:44:11.143220 reflex-0.2.0a2/reflex/components/layout/__init__.py
--rw-r--r--   0        0        0      320 2023-06-27 19:44:11.143353 reflex-0.2.0a2/reflex/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      760 2023-06-27 19:44:11.143479 reflex-0.2.0a2/reflex/components/layout/box.py
--rw-r--r--   0        0        0     2853 2023-06-27 19:44:11.143617 reflex-0.2.0a2/reflex/components/layout/card.py
--rw-r--r--   0        0        0      394 2023-06-27 19:44:11.143865 reflex-0.2.0a2/reflex/components/layout/center.py
--rw-r--r--   0        0        0     3832 2023-06-27 19:44:11.144010 reflex-0.2.0a2/reflex/components/layout/cond.py
--rw-r--r--   0        0        0      359 2023-06-27 19:44:11.144122 reflex-0.2.0a2/reflex/components/layout/container.py
--rw-r--r--   0        0        0      652 2023-06-27 19:44:11.144331 reflex-0.2.0a2/reflex/components/layout/flex.py
--rw-r--r--   0        0        0     3159 2023-06-27 19:44:11.144459 reflex-0.2.0a2/reflex/components/layout/foreach.py
--rw-r--r--   0        0        0      312 2023-06-27 19:44:11.144576 reflex-0.2.0a2/reflex/components/layout/fragment.py
--rw-r--r--   0        0        0     4323 2023-06-27 19:44:11.144810 reflex-0.2.0a2/reflex/components/layout/grid.py
--rw-r--r--   0        0        0      977 2023-06-27 19:44:11.144963 reflex-0.2.0a2/reflex/components/layout/html.py
--rw-r--r--   0        0        0     1898 2023-06-27 19:44:11.145102 reflex-0.2.0a2/reflex/components/layout/responsive.py
--rw-r--r--   0        0        0      184 2023-06-27 19:44:11.145217 reflex-0.2.0a2/reflex/components/layout/spacer.py
--rw-r--r--   0        0        0      991 2023-06-27 19:44:11.145353 reflex-0.2.0a2/reflex/components/layout/stack.py
--rw-r--r--   0        0        0     1465 2023-06-27 19:44:11.145602 reflex-0.2.0a2/reflex/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2023-06-27 19:44:11.145672 reflex-0.2.0a2/reflex/components/libs/__init__.py
--rw-r--r--   0        0        0      220 2023-06-27 19:44:11.145809 reflex-0.2.0a2/reflex/components/libs/chakra.py
--rw-r--r--   0        0        0     1385 2023-06-27 19:44:11.145926 reflex-0.2.0a2/reflex/components/libs/react_player.py
--rw-r--r--   0        0        0      240 2023-06-27 19:44:11.146020 reflex-0.2.0a2/reflex/components/media/__init__.py
--rw-r--r--   0        0        0      195 2023-06-27 19:44:11.146153 reflex-0.2.0a2/reflex/components/media/audio.py
--rw-r--r--   0        0        0     1520 2023-06-27 19:44:11.146292 reflex-0.2.0a2/reflex/components/media/avatar.py
--rw-r--r--   0        0        0     2387 2023-06-27 19:44:11.146473 reflex-0.2.0a2/reflex/components/media/icon.py
--rw-r--r--   0        0        0     2053 2023-06-27 19:44:11.146591 reflex-0.2.0a2/reflex/components/media/image.py
--rw-r--r--   0        0        0      195 2023-06-27 19:44:11.146711 reflex-0.2.0a2/reflex/components/media/video.py
--rw-r--r--   0        0        0      450 2023-06-27 19:44:11.146794 reflex-0.2.0a2/reflex/components/navigation/__init__.py
--rw-r--r--   0        0        0     2017 2023-06-27 19:44:11.146909 reflex-0.2.0a2/reflex/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1602 2023-06-30 17:42:07.290376 reflex-0.2.0a2/reflex/components/navigation/link.py
--rw-r--r--   0        0        0      526 2023-06-27 19:44:11.147151 reflex-0.2.0a2/reflex/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      503 2023-06-27 19:44:11.147264 reflex-0.2.0a2/reflex/components/navigation/nextlink.py
--rw-r--r--   0        0        0     2836 2023-06-27 19:44:11.147387 reflex-0.2.0a2/reflex/components/navigation/stepper.py
--rw-r--r--   0        0        0      887 2023-06-27 19:44:11.147466 reflex-0.2.0a2/reflex/components/overlay/__init__.py
--rw-r--r--   0        0        0     5019 2023-06-27 19:44:11.147600 reflex-0.2.0a2/reflex/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     1008 2023-06-27 19:44:11.147723 reflex-0.2.0a2/reflex/components/overlay/banner.py
--rw-r--r--   0        0        0     4673 2023-06-27 19:44:11.147856 reflex-0.2.0a2/reflex/components/overlay/drawer.py
--rw-r--r--   0        0        0     5524 2023-06-27 19:44:11.147979 reflex-0.2.0a2/reflex/components/overlay/menu.py
--rw-r--r--   0        0        0     4909 2023-06-27 19:44:11.148109 reflex-0.2.0a2/reflex/components/overlay/modal.py
--rw-r--r--   0        0        0     5682 2023-06-27 19:44:11.148207 reflex-0.2.0a2/reflex/components/overlay/popover.py
--rw-r--r--   0        0        0     1945 2023-06-27 19:44:11.148335 reflex-0.2.0a2/reflex/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2023-06-27 19:44:11.148399 reflex-0.2.0a2/reflex/components/tags/__init__.py
--rw-r--r--   0        0        0      447 2023-06-27 19:44:11.148512 reflex-0.2.0a2/reflex/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2294 2023-06-27 19:44:11.148635 reflex-0.2.0a2/reflex/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5008 2023-06-27 19:44:11.148727 reflex-0.2.0a2/reflex/components/tags/tag.py
--rw-r--r--   0        0        0      587 2023-06-27 19:44:11.148966 reflex-0.2.0a2/reflex/components/tags/tagless.py
--rw-r--r--   0        0        0      302 2023-06-27 19:44:11.149095 reflex-0.2.0a2/reflex/components/typography/__init__.py
--rw-r--r--   0        0        0      278 2023-06-27 19:44:11.149223 reflex-0.2.0a2/reflex/components/typography/heading.py
--rw-r--r--   0        0        0      676 2023-06-27 19:44:11.149340 reflex-0.2.0a2/reflex/components/typography/highlight.py
--rw-r--r--   0        0        0     3454 2023-06-27 19:44:11.149473 reflex-0.2.0a2/reflex/components/typography/markdown.py
--rw-r--r--   0        0        0      333 2023-06-27 19:44:11.149590 reflex-0.2.0a2/reflex/components/typography/span.py
--rw-r--r--   0        0        0      302 2023-06-27 19:44:11.149709 reflex-0.2.0a2/reflex/components/typography/text.py
--rw-r--r--   0        0        0     7120 2023-06-27 19:44:11.149845 reflex-0.2.0a2/reflex/config.py
--rw-r--r--   0        0        0    10486 2023-06-27 19:44:11.149975 reflex-0.2.0a2/reflex/constants.py
--rw-r--r--   0        0        0       73 2023-06-27 19:44:11.150039 reflex-0.2.0a2/reflex/el/__init__.py
--rw-r--r--   0        0        0      113 2023-06-27 19:44:11.150151 reflex-0.2.0a2/reflex/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-06-27 19:44:11.150219 reflex-0.2.0a2/reflex/el/constants/html.py
--rw-r--r--   0        0        0    15554 2023-06-27 19:44:11.150474 reflex-0.2.0a2/reflex/el/constants/react.py
--rw-r--r--   0        0        0     1717 2023-06-27 19:44:11.150571 reflex-0.2.0a2/reflex/el/constants/reflex.py
--rw-r--r--   0        0        0     1318 2023-06-27 19:44:11.150906 reflex-0.2.0a2/reflex/el/element.py
--rw-r--r--   0        0        0   106323 2023-06-27 19:44:11.151244 reflex-0.2.0a2/reflex/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2655 2023-06-27 19:44:11.151376 reflex-0.2.0a2/reflex/el/precompile.py
--rw-r--r--   0        0        0    13398 2023-06-28 21:01:51.884492 reflex-0.2.0a2/reflex/event.py
--rw-r--r--   0        0        0      111 2023-06-27 19:44:11.151669 reflex-0.2.0a2/reflex/middleware/__init__.py
--rw-r--r--   0        0        0     1726 2023-06-27 19:44:11.151870 reflex-0.2.0a2/reflex/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1157 2023-06-27 19:44:11.151991 reflex-0.2.0a2/reflex/middleware/middleware.py
--rw-r--r--   0        0        0     2382 2023-06-27 19:44:11.152120 reflex-0.2.0a2/reflex/model.py
--rw-r--r--   0        0        0        0 2023-06-27 19:44:11.152148 reflex-0.2.0a2/reflex/py.typed
--rw-r--r--   0        0        0     8891 2023-06-28 01:25:19.554153 reflex-0.2.0a2/reflex/reflex.py
--rw-r--r--   0        0        0     4104 2023-06-27 19:44:11.152409 reflex-0.2.0a2/reflex/route.py
--rw-r--r--   0        0        0    31805 2023-06-30 17:42:07.290862 reflex-0.2.0a2/reflex/state.py
--rw-r--r--   0        0        0     1113 2023-06-27 19:44:11.152777 reflex-0.2.0a2/reflex/style.py
--rw-r--r--   0        0        0       24 2023-06-27 19:44:11.152904 reflex-0.2.0a2/reflex/utils/__init__.py
--rw-r--r--   0        0        0     7585 2023-06-28 01:25:15.379838 reflex-0.2.0a2/reflex/utils/build.py
--rw-r--r--   0        0        0     1759 2023-06-27 19:44:11.153226 reflex-0.2.0a2/reflex/utils/console.py
--rw-r--r--   0        0        0     4680 2023-06-30 17:42:07.291282 reflex-0.2.0a2/reflex/utils/exec.py
--rw-r--r--   0        0        0    11845 2023-06-30 17:42:02.061676 reflex-0.2.0a2/reflex/utils/format.py
--rw-r--r--   0        0        0      585 2023-06-27 19:44:11.153583 reflex-0.2.0a2/reflex/utils/imports.py
--rw-r--r--   0        0        0     2429 2023-06-30 17:42:07.291621 reflex-0.2.0a2/reflex/utils/path_ops.py
--rw-r--r--   0        0        0    12296 2023-06-30 17:42:07.291811 reflex-0.2.0a2/reflex/utils/prerequisites.py
--rw-r--r--   0        0        0     3734 2023-06-28 23:03:00.473042 reflex-0.2.0a2/reflex/utils/processes.py
--rw-r--r--   0        0        0     2362 2023-06-27 19:44:11.154002 reflex-0.2.0a2/reflex/utils/telemetry.py
--rw-r--r--   0        0        0     4804 2023-06-27 19:44:11.154115 reflex-0.2.0a2/reflex/utils/types.py
--rw-r--r--   0        0        0     2632 2023-06-27 19:44:11.154230 reflex-0.2.0a2/reflex/utils/watch.py
--rw-r--r--   0        0        0    31837 2023-06-27 19:44:11.154394 reflex-0.2.0a2/reflex/vars.py
--rw-r--r--   0        0        0    10138 1970-01-01 00:00:00.000000 reflex-0.2.0a2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-14 23:13:37.760267 reflex-0.2.1a1/LICENSE
+-rw-r--r--   0        0        0     7766 2023-07-17 23:29:33.625723 reflex-0.2.1a1/README.md
+-rw-r--r--   0        0        0     2002 2023-07-17 23:59:03.104219 reflex-0.2.1a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769763 reflex-0.2.1a1/reflex/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1337 2023-07-17 03:56:35.638995 reflex-0.2.1a1/reflex/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769883 reflex-0.2.1a1/reflex/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1225 2023-07-14 23:13:37.769942 reflex-0.2.1a1/reflex/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2023-07-14 23:13:37.770037 reflex-0.2.1a1/reflex/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      181 2023-07-14 23:13:37.770146 reflex-0.2.1a1/reflex/.templates/jinja/app/rxconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-07-14 23:13:37.770264 reflex-0.2.1a1/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-07-14 23:13:37.770322 reflex-0.2.1a1/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-07-14 23:13:37.770383 reflex-0.2.1a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     3312 2023-07-14 23:13:37.770458 reflex-0.2.1a1/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     3170 2023-07-14 23:13:37.770519 reflex-0.2.1a1/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      356 2023-07-14 23:13:37.770572 reflex-0.2.1a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0       38 2023-07-14 23:13:37.770645 reflex-0.2.1a1/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-07-14 23:13:37.770733 reflex-0.2.1a1/reflex/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   284503 2023-07-14 23:13:37.771555 reflex-0.2.1a1/reflex/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       50 2023-07-14 23:13:37.771627 reflex-0.2.1a1/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0       65 2023-07-14 23:13:37.771678 reflex-0.2.1a1/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0     1179 2023-07-14 23:13:37.771733 reflex-0.2.1a1/reflex/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2023-07-14 23:13:37.771821 reflex-0.2.1a1/reflex/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      597 2023-07-14 23:13:37.771876 reflex-0.2.1a1/reflex/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0       82 2023-07-14 23:13:37.771931 reflex-0.2.1a1/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0    29404 2023-07-14 23:13:37.772115 reflex-0.2.1a1/reflex/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0       59 2023-07-14 23:13:37.772177 reflex-0.2.1a1/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0     9692 2023-07-14 23:13:37.772301 reflex-0.2.1a1/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1917 2023-07-17 23:54:14.126636 reflex-0.2.1a1/reflex/__init__.py
+-rw-r--r--   0        0        0      373 2023-07-14 23:13:37.772422 reflex-0.2.1a1/reflex/admin.py
+-rw-r--r--   0        0        0    23303 2023-07-17 23:29:33.626521 reflex-0.2.1a1/reflex/app.py
+-rw-r--r--   0        0        0     2438 2023-07-14 23:13:37.772635 reflex-0.2.1a1/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-07-14 23:13:37.772707 reflex-0.2.1a1/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0     6604 2023-07-17 23:29:33.627133 reflex-0.2.1a1/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     2725 2023-07-14 23:13:37.772848 reflex-0.2.1a1/reflex/compiler/templates.py
+-rw-r--r--   0        0        0     8527 2023-07-17 23:54:14.127035 reflex-0.2.1a1/reflex/compiler/utils.py
+-rw-r--r--   0        0        0     7601 2023-07-17 23:54:14.127174 reflex-0.2.1a1/reflex/components/__init__.py
+-rw-r--r--   0        0        0      229 2023-07-17 23:54:14.127269 reflex-0.2.1a1/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      719 2023-07-14 23:13:37.773188 reflex-0.2.1a1/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-07-14 23:13:37.773235 reflex-0.2.1a1/reflex/components/base/body.py
+-rw-r--r--   0        0        0      721 2023-07-17 23:54:14.127363 reflex-0.2.1a1/reflex/components/base/document.py
+-rw-r--r--   0        0        0      263 2023-07-14 23:13:37.773334 reflex-0.2.1a1/reflex/components/base/head.py
+-rw-r--r--   0        0        0      929 2023-07-14 23:13:37.773386 reflex-0.2.1a1/reflex/components/base/link.py
+-rw-r--r--   0        0        0     1408 2023-07-14 23:13:37.773437 reflex-0.2.1a1/reflex/components/base/meta.py
+-rw-r--r--   0        0        0    24321 2023-07-14 23:13:37.773563 reflex-0.2.1a1/reflex/components/component.py
+-rw-r--r--   0        0        0      496 2023-07-14 23:13:37.773654 reflex-0.2.1a1/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      330 2023-07-14 23:13:37.773723 reflex-0.2.1a1/reflex/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     3495 2023-07-14 23:13:37.773785 reflex-0.2.1a1/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4025 2023-07-14 23:13:37.773859 reflex-0.2.1a1/reflex/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      533 2023-07-14 23:13:37.773921 reflex-0.2.1a1/reflex/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      185 2023-07-14 23:13:37.773974 reflex-0.2.1a1/reflex/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1422 2023-07-14 23:13:37.774028 reflex-0.2.1a1/reflex/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2151 2023-07-14 23:13:37.774087 reflex-0.2.1a1/reflex/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     5785 2023-07-14 23:13:37.774148 reflex-0.2.1a1/reflex/components/datadisplay/table.py
+-rw-r--r--   0        0        0     2182 2023-07-14 23:13:37.774210 reflex-0.2.1a1/reflex/components/datadisplay/tag.py
+-rw-r--r--   0        0        0      384 2023-07-14 23:13:37.774286 reflex-0.2.1a1/reflex/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     3511 2023-07-14 23:13:37.774347 reflex-0.2.1a1/reflex/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2771 2023-07-14 23:13:37.774404 reflex-0.2.1a1/reflex/components/disclosure/tabs.py
+-rw-r--r--   0        0        0     1737 2023-07-14 23:13:37.774459 reflex-0.2.1a1/reflex/components/disclosure/transition.py
+-rw-r--r--   0        0        0      283 2023-07-14 23:13:37.774510 reflex-0.2.1a1/reflex/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2023-07-14 23:13:37.774594 reflex-0.2.1a1/reflex/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1565 2023-07-14 23:13:37.774654 reflex-0.2.1a1/reflex/components/feedback/alert.py
+-rw-r--r--   0        0        0     1899 2023-07-14 23:13:37.774714 reflex-0.2.1a1/reflex/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      875 2023-07-14 23:13:37.774769 reflex-0.2.1a1/reflex/components/feedback/progress.py
+-rw-r--r--   0        0        0     1781 2023-07-14 23:13:37.774821 reflex-0.2.1a1/reflex/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      674 2023-07-14 23:13:37.774872 reflex-0.2.1a1/reflex/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1573 2023-07-14 23:13:37.774956 reflex-0.2.1a1/reflex/components/forms/__init__.py
+-rw-r--r--   0        0        0     1761 2023-07-14 23:13:37.775013 reflex-0.2.1a1/reflex/components/forms/button.py
+-rw-r--r--   0        0        0     2448 2023-07-14 23:13:37.775073 reflex-0.2.1a1/reflex/components/forms/checkbox.py
+-rw-r--r--   0        0        0     3137 2023-07-14 23:13:37.775129 reflex-0.2.1a1/reflex/components/forms/colormodeswitch.py
+-rw-r--r--   0        0        0      574 2023-07-14 23:13:37.775183 reflex-0.2.1a1/reflex/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775234 reflex-0.2.1a1/reflex/components/forms/date_picker.py
+-rw-r--r--   0        0        0      273 2023-07-14 23:13:37.775287 reflex-0.2.1a1/reflex/components/forms/date_time_picker.py
+-rw-r--r--   0        0        0     2627 2023-07-14 23:13:37.775352 reflex-0.2.1a1/reflex/components/forms/debounce.py
+-rw-r--r--   0        0        0     1943 2023-07-14 23:13:37.775412 reflex-0.2.1a1/reflex/components/forms/editable.py
+-rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775465 reflex-0.2.1a1/reflex/components/forms/email.py
+-rw-r--r--   0        0        0     2990 2023-07-14 23:13:37.775521 reflex-0.2.1a1/reflex/components/forms/form.py
+-rw-r--r--   0        0        0      798 2023-07-14 23:13:37.775579 reflex-0.2.1a1/reflex/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     3246 2023-07-14 23:13:37.775648 reflex-0.2.1a1/reflex/components/forms/input.py
+-rw-r--r--   0        0        0    12659 2023-07-14 23:13:37.775734 reflex-0.2.1a1/reflex/components/forms/multiselect.py
+-rw-r--r--   0        0        0     3889 2023-07-14 23:13:37.775802 reflex-0.2.1a1/reflex/components/forms/numberinput.py
+-rw-r--r--   0        0        0      249 2023-07-14 23:13:37.775849 reflex-0.2.1a1/reflex/components/forms/password.py
+-rw-r--r--   0        0        0     2662 2023-07-14 23:13:37.775908 reflex-0.2.1a1/reflex/components/forms/pininput.py
+-rw-r--r--   0        0        0     3029 2023-07-14 23:13:37.775964 reflex-0.2.1a1/reflex/components/forms/radio.py
+-rw-r--r--   0        0        0     2845 2023-07-14 23:13:37.776021 reflex-0.2.1a1/reflex/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3510 2023-07-14 23:13:37.776068 reflex-0.2.1a1/reflex/components/forms/select.py
+-rw-r--r--   0        0        0     3116 2023-07-14 23:13:37.776140 reflex-0.2.1a1/reflex/components/forms/slider.py
+-rw-r--r--   0        0        0     1567 2023-07-14 23:13:37.776193 reflex-0.2.1a1/reflex/components/forms/switch.py
+-rw-r--r--   0        0        0     1526 2023-07-14 23:13:37.776244 reflex-0.2.1a1/reflex/components/forms/textarea.py
+-rw-r--r--   0        0        0     2905 2023-07-14 23:13:37.776307 reflex-0.2.1a1/reflex/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-07-14 23:13:37.776385 reflex-0.2.1a1/reflex/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1351 2023-07-14 23:13:37.776443 reflex-0.2.1a1/reflex/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17354 2023-07-14 23:13:37.776536 reflex-0.2.1a1/reflex/components/graphing/victory.py
+-rw-r--r--   0        0        0      872 2023-07-14 23:13:37.776623 reflex-0.2.1a1/reflex/components/layout/__init__.py
+-rw-r--r--   0        0        0      320 2023-07-14 23:13:37.776678 reflex-0.2.1a1/reflex/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      760 2023-07-14 23:13:37.776730 reflex-0.2.1a1/reflex/components/layout/box.py
+-rw-r--r--   0        0        0     2853 2023-07-14 23:13:37.776787 reflex-0.2.1a1/reflex/components/layout/card.py
+-rw-r--r--   0        0        0      394 2023-07-14 23:13:37.776833 reflex-0.2.1a1/reflex/components/layout/center.py
+-rw-r--r--   0        0        0     3832 2023-07-14 23:13:37.776892 reflex-0.2.1a1/reflex/components/layout/cond.py
+-rw-r--r--   0        0        0      359 2023-07-14 23:13:37.776948 reflex-0.2.1a1/reflex/components/layout/container.py
+-rw-r--r--   0        0        0      652 2023-07-14 23:13:37.776999 reflex-0.2.1a1/reflex/components/layout/flex.py
+-rw-r--r--   0        0        0     3159 2023-07-14 23:13:37.777060 reflex-0.2.1a1/reflex/components/layout/foreach.py
+-rw-r--r--   0        0        0      312 2023-07-14 23:13:37.777113 reflex-0.2.1a1/reflex/components/layout/fragment.py
+-rw-r--r--   0        0        0     4323 2023-07-14 23:13:37.777175 reflex-0.2.1a1/reflex/components/layout/grid.py
+-rw-r--r--   0        0        0      977 2023-07-14 23:13:37.777231 reflex-0.2.1a1/reflex/components/layout/html.py
+-rw-r--r--   0        0        0     1898 2023-07-14 23:13:37.777279 reflex-0.2.1a1/reflex/components/layout/responsive.py
+-rw-r--r--   0        0        0      184 2023-07-14 23:13:37.777323 reflex-0.2.1a1/reflex/components/layout/spacer.py
+-rw-r--r--   0        0        0      991 2023-07-14 23:13:37.777374 reflex-0.2.1a1/reflex/components/layout/stack.py
+-rw-r--r--   0        0        0     1465 2023-07-14 23:13:37.777429 reflex-0.2.1a1/reflex/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2023-07-14 23:13:37.777503 reflex-0.2.1a1/reflex/components/libs/__init__.py
+-rw-r--r--   0        0        0      220 2023-07-14 23:13:37.777552 reflex-0.2.1a1/reflex/components/libs/chakra.py
+-rw-r--r--   0        0        0     1385 2023-07-14 23:13:37.777604 reflex-0.2.1a1/reflex/components/libs/react_player.py
+-rw-r--r--   0        0        0      240 2023-07-14 23:13:37.777685 reflex-0.2.1a1/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777734 reflex-0.2.1a1/reflex/components/media/audio.py
+-rw-r--r--   0        0        0     1520 2023-07-14 23:13:37.777790 reflex-0.2.1a1/reflex/components/media/avatar.py
+-rw-r--r--   0        0        0     2387 2023-07-14 23:13:37.777859 reflex-0.2.1a1/reflex/components/media/icon.py
+-rw-r--r--   0        0        0     2053 2023-07-14 23:13:37.777927 reflex-0.2.1a1/reflex/components/media/image.py
+-rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777986 reflex-0.2.1a1/reflex/components/media/video.py
+-rw-r--r--   0        0        0      450 2023-07-14 23:13:37.778063 reflex-0.2.1a1/reflex/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2017 2023-07-14 23:13:37.778119 reflex-0.2.1a1/reflex/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1602 2023-07-14 23:13:37.778175 reflex-0.2.1a1/reflex/components/navigation/link.py
+-rw-r--r--   0        0        0      526 2023-07-14 23:13:37.778225 reflex-0.2.1a1/reflex/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      503 2023-07-14 23:13:37.778277 reflex-0.2.1a1/reflex/components/navigation/nextlink.py
+-rw-r--r--   0        0        0     2836 2023-07-14 23:13:37.778336 reflex-0.2.1a1/reflex/components/navigation/stepper.py
+-rw-r--r--   0        0        0      887 2023-07-14 23:13:37.778422 reflex-0.2.1a1/reflex/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5019 2023-07-14 23:13:37.778510 reflex-0.2.1a1/reflex/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     1008 2023-07-14 23:13:37.778561 reflex-0.2.1a1/reflex/components/overlay/banner.py
+-rw-r--r--   0        0        0     4673 2023-07-14 23:13:37.778619 reflex-0.2.1a1/reflex/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5524 2023-07-14 23:13:37.778690 reflex-0.2.1a1/reflex/components/overlay/menu.py
+-rw-r--r--   0        0        0     4909 2023-07-14 23:13:37.778744 reflex-0.2.1a1/reflex/components/overlay/modal.py
+-rw-r--r--   0        0        0     5682 2023-07-14 23:13:37.778818 reflex-0.2.1a1/reflex/components/overlay/popover.py
+-rw-r--r--   0        0        0     1945 2023-07-14 23:13:37.778874 reflex-0.2.1a1/reflex/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2023-07-14 23:13:37.778947 reflex-0.2.1a1/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-07-14 23:13:37.779004 reflex-0.2.1a1/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2294 2023-07-14 23:13:37.779060 reflex-0.2.1a1/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5008 2023-07-14 23:13:37.779125 reflex-0.2.1a1/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-07-14 23:13:37.779176 reflex-0.2.1a1/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779262 reflex-0.2.1a1/reflex/components/typography/__init__.py
+-rw-r--r--   0        0        0      278 2023-07-14 23:13:37.779315 reflex-0.2.1a1/reflex/components/typography/heading.py
+-rw-r--r--   0        0        0      676 2023-07-14 23:13:37.779367 reflex-0.2.1a1/reflex/components/typography/highlight.py
+-rw-r--r--   0        0        0     3593 2023-07-14 23:13:37.779432 reflex-0.2.1a1/reflex/components/typography/markdown.py
+-rw-r--r--   0        0        0      333 2023-07-14 23:13:37.779494 reflex-0.2.1a1/reflex/components/typography/span.py
+-rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779551 reflex-0.2.1a1/reflex/components/typography/text.py
+-rw-r--r--   0        0        0     7215 2023-07-14 23:13:37.779630 reflex-0.2.1a1/reflex/config.py
+-rw-r--r--   0        0        0    10821 2023-07-17 23:29:33.627808 reflex-0.2.1a1/reflex/constants.py
+-rw-r--r--   0        0        0       73 2023-07-14 23:13:37.779820 reflex-0.2.1a1/reflex/el/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-14 23:13:37.779899 reflex-0.2.1a1/reflex/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-07-14 23:13:37.779984 reflex-0.2.1a1/reflex/el/constants/html.py
+-rw-r--r--   0        0        0    15554 2023-07-14 23:13:37.780082 reflex-0.2.1a1/reflex/el/constants/react.py
+-rw-r--r--   0        0        0     1717 2023-07-14 23:13:37.780152 reflex-0.2.1a1/reflex/el/constants/reflex.py
+-rw-r--r--   0        0        0     1318 2023-07-14 23:13:37.780228 reflex-0.2.1a1/reflex/el/element.py
+-rw-r--r--   0        0        0   106323 2023-07-14 23:13:37.780493 reflex-0.2.1a1/reflex/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2655 2023-07-14 23:13:37.780585 reflex-0.2.1a1/reflex/el/precompile.py
+-rw-r--r--   0        0        0    13398 2023-07-14 23:13:37.780692 reflex-0.2.1a1/reflex/event.py
+-rw-r--r--   0        0        0      111 2023-07-14 23:13:37.780772 reflex-0.2.1a1/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1726 2023-07-14 23:13:37.780837 reflex-0.2.1a1/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1157 2023-07-14 23:13:37.780910 reflex-0.2.1a1/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0     8611 2023-07-17 23:29:30.479899 reflex-0.2.1a1/reflex/model.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.781036 reflex-0.2.1a1/reflex/py.typed
+-rw-r--r--   0        0        0     9136 2023-07-17 23:29:33.627991 reflex-0.2.1a1/reflex/reflex.py
+-rw-r--r--   0        0        0     4104 2023-07-14 23:13:37.781214 reflex-0.2.1a1/reflex/route.py
+-rw-r--r--   0        0        0    31805 2023-07-14 23:13:37.781402 reflex-0.2.1a1/reflex/state.py
+-rw-r--r--   0        0        0     1113 2023-07-14 23:13:37.781487 reflex-0.2.1a1/reflex/style.py
+-rw-r--r--   0        0        0    15063 2023-07-14 23:13:37.781613 reflex-0.2.1a1/reflex/testing.py
+-rw-r--r--   0        0        0       24 2023-07-14 23:13:37.781705 reflex-0.2.1a1/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     7585 2023-07-17 23:29:30.480212 reflex-0.2.1a1/reflex/utils/build.py
+-rw-r--r--   0        0        0     1759 2023-07-14 23:13:37.781884 reflex-0.2.1a1/reflex/utils/console.py
+-rw-r--r--   0        0        0     4225 2023-07-17 23:29:33.628283 reflex-0.2.1a1/reflex/utils/exec.py
+-rw-r--r--   0        0        0    11845 2023-07-14 23:13:37.782067 reflex-0.2.1a1/reflex/utils/format.py
+-rw-r--r--   0        0        0      585 2023-07-14 23:13:37.782125 reflex-0.2.1a1/reflex/utils/imports.py
+-rw-r--r--   0        0        0     2429 2023-07-14 23:13:37.782189 reflex-0.2.1a1/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    12672 2023-07-17 23:29:30.480515 reflex-0.2.1a1/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0     4105 2023-07-17 23:29:33.628618 reflex-0.2.1a1/reflex/utils/processes.py
+-rw-r--r--   0        0        0     2362 2023-07-14 23:13:37.782441 reflex-0.2.1a1/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0     4804 2023-07-14 23:13:37.782520 reflex-0.2.1a1/reflex/utils/types.py
+-rw-r--r--   0        0        0     2632 2023-07-14 23:13:37.782576 reflex-0.2.1a1/reflex/utils/watch.py
+-rw-r--r--   0        0        0    32892 2023-07-14 23:13:37.782718 reflex-0.2.1a1/reflex/vars.py
+-rw-r--r--   0        0        0     9545 1970-01-01 00:00:00.000000 reflex-0.2.1a1/PKG-INFO
```

### Comparing `reflex-0.2.0a2/LICENSE` & `reflex-0.2.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/README.md` & `reflex-0.2.1a1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,529 +1,486 @@
-00000000: 6060 6064 6966 660a 2b20 4154 5445 4e54  ```diff.+ ATTENT
-00000010: 494f 4e3a 204f 7665 7220 7468 6520 6e65  ION: Over the ne
-00000020: 7874 2077 6565 6b20 7765 2077 696c 6c20  xt week we will 
-00000030: 6265 2063 6861 6e67 696e 6720 6f75 7220  be changing our 
-00000040: 7072 6f6a 6563 7420 6e61 6d65 2066 726f  project name fro
-00000050: 6d20 5079 6e65 636f 6e65 2074 6f20 5265  m Pynecone to Re
-00000060: 666c 6578 2e0a 0a54 6865 206e 6577 206e  flex...The new n
-00000070: 616d 6520 616c 6967 6e73 2077 6974 6820  ame aligns with 
-00000080: 6f75 7220 676f 616c 206f 6620 616c 6c6f  our goal of allo
-00000090: 7769 6e67 2079 6f75 2074 6f20 6275 696c  wing you to buil
-000000a0: 6420 6170 7073 2065 6173 696c 792c 2077  d apps easily, w
-000000b0: 6869 6c65 2061 6c73 6f20 6265 696e 6720  hile also being 
-000000c0: 666c 6578 6962 6c65 2061 6e64 2070 6f77  flexible and pow
-000000d0: 6572 6675 6c20 656e 6f75 6768 2074 6f20  erful enough to 
-000000e0: 6861 6e64 6c65 2061 6c6c 2079 6f75 7220  handle all your 
-000000f0: 7573 6520 6361 7365 732e 0a0a 4d61 6a6f  use cases...Majo
-00000100: 7220 4368 616e 6765 733a 0a2b 204f 7572  r Changes:.+ Our
-00000110: 2064 6f6d 6169 6e20 7769 6c6c 2073 7769   domain will swi
-00000120: 7463 6820 6672 6f6d 2068 7474 7073 3a2f  tch from https:/
-00000130: 2f70 796e 6563 6f6e 652e 696f 2f20 2d3e  /pynecone.io/ ->
-00000140: 2068 7474 7073 3a2f 2f72 6566 6c65 782e   https://reflex.
-00000150: 6465 762f 0a2b 204f 7572 2070 6970 2069  dev/.+ Our pip i
-00000160: 6e73 7461 6c6c 2077 696c 6c20 7377 6974  nstall will swit
-00000170: 6368 2066 726f 6d20 7069 7020 696e 7374  ch from pip inst
-00000180: 616c 6c20 7079 6e65 636f 6e65 202d 3e20  all pynecone -> 
-00000190: 7069 7020 696e 7374 616c 6c20 7265 666c  pip install refl
-000001a0: 6578 0a2b 204f 7572 2047 6974 6875 6220  ex.+ Our Github 
-000001b0: 7265 706f 2077 696c 6c20 7377 6974 6368  repo will switch
-000001c0: 2066 726f 6d20 6874 7470 733a 2f2f 6769   from https://gi
-000001d0: 7468 7562 2e63 6f6d 2f70 796e 6563 6f6e  thub.com/pynecon
-000001e0: 652d 696f 2f70 796e 6563 6f6e 6520 2d3e  e-io/pynecone ->
-000001f0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000200: 636f 6d2f 7265 666c 6578 2d64 6576 2f72  com/reflex-dev/r
-00000210: 6566 6c65 780a 2b20 4f75 7220 6c69 6272  eflex.+ Our libr
-00000220: 6172 7920 7769 6c6c 2063 6861 6e67 6520  ary will change 
-00000230: 6672 6f6d 2069 6d70 6f72 7420 7079 6e65  from import pyne
-00000240: 636f 6e65 2061 7320 7063 2074 6f20 696d  cone as pc to im
-00000250: 706f 7274 2072 6566 6c65 7820 6173 2072  port reflex as r
-00000260: 780a 0a57 6520 7769 6c6c 2068 6176 6520  x..We will have 
-00000270: 6120 6665 6174 7572 6520 6672 6565 7a65  a feature freeze
-00000280: 2075 6e74 696c 2077 6520 6d69 6772 6174   until we migrat
-00000290: 6520 6f75 7220 636f 6465 2061 6e64 2077  e our code and w
-000002a0: 6562 7369 7465 2074 6f20 7468 6520 6e65  ebsite to the ne
-000002b0: 7720 6e61 6d65 2e0a 0a4f 7572 2067 6f61  w name...Our goa
-000002c0: 6c20 6973 2074 6f20 636f 6d70 6c65 7465  l is to complete
-000002d0: 2074 6865 2074 7261 6e73 6974 696f 6e20   the transition 
-000002e0: 6279 204a 756e 6520 3330 2e20 5468 616e  by June 30. Than
-000002f0: 6b73 2066 6f72 2079 6f75 7220 7375 7070  ks for your supp
-00000300: 6f72 7420 2d20 706c 6561 7365 206d 6573  ort - please mes
-00000310: 7361 6765 206f 6e20 4469 7363 6f72 6420  sage on Discord 
-00000320: 6966 2079 6f75 2068 6176 6520 616e 7920  if you have any 
-00000330: 7175 6573 7469 6f6e 7320 6f72 2063 6f6e  questions or con
-00000340: 6365 726e 7321 0a60 6060 0a0a 3c64 6976  cerns!.```..<div
-00000350: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-00000360: 0a0a 3c69 6d67 2073 7263 3d22 646f 6373  ..<img src="docs
-00000370: 2f69 6d61 6765 732f 636f 6e65 732e 706e  /images/cones.pn
-00000380: 6722 3e0a 3c68 723e 0a0a 2a2a e29c a820  g">.<hr>..**... 
-00000390: 5065 7266 6f72 6d61 6e74 2c20 6375 7374  Performant, cust
-000003a0: 6f6d 697a 6162 6c65 2077 6562 2061 7070  omizable web app
-000003b0: 7320 696e 2070 7572 6520 5079 7468 6f6e  s in pure Python
-000003c0: 2e20 4465 706c 6f79 2069 6e20 7365 636f  . Deploy in seco
-000003d0: 6e64 732e 2a2a 0a0a f09f 9391 205b 446f  nds.**...... [Do
-000003e0: 6373 5d28 6874 7470 733a 2f2f 7079 6e65  cs](https://pyne
-000003f0: 636f 6e65 2e69 6f2f 646f 6373 2f67 6574  cone.io/docs/get
-00000400: 7469 6e67 2d73 7461 7274 6564 2f69 6e74  ting-started/int
-00000410: 726f 6475 6374 696f 6e29 2026 6e62 7370  roduction) &nbsp
-00000420: 3b20 f09f 93b1 205b 436f 6d70 6f6e 656e  ; .... [Componen
-00000430: 7420 4c69 6272 6172 795d 2868 7474 7073  t Library](https
-00000440: 3a2f 2f70 796e 6563 6f6e 652e 696f 2f64  ://pynecone.io/d
-00000450: 6f63 732f 6c69 6272 6172 7929 2026 6e62  ocs/library) &nb
-00000460: 7370 3b20 f09f 96bc efb8 8f20 5b47 616c  sp; ....... [Gal
-00000470: 6c65 7279 5d28 6874 7470 733a 2f2f 7079  lery](https://py
-00000480: 6e65 636f 6e65 2e69 6f2f 646f 6373 2f67  necone.io/docs/g
-00000490: 616c 6c65 7279 2920 266e 6273 703b 20f0  allery) &nbsp; .
-000004a0: 9f9b b820 5b44 6570 6c6f 796d 656e 745d  ... [Deployment]
-000004b0: 2868 7474 7073 3a2f 2f70 796e 6563 6f6e  (https://pynecon
-000004c0: 652e 696f 2f64 6f63 732f 686f 7374 696e  e.io/docs/hostin
-000004d0: 672f 6465 706c 6f79 290a 0a5b 215b 5079  g/deploy)..[![Py
-000004e0: 5049 2076 6572 7369 6f6e 5d28 6874 7470  PI version](http
-000004f0: 733a 2f2f 6261 6467 652e 6675 7279 2e69  s://badge.fury.i
-00000500: 6f2f 7079 2f70 796e 6563 6f6e 652e 7376  o/py/pynecone.sv
-00000510: 6729 5d28 6874 7470 733a 2f2f 6261 6467  g)](https://badg
-00000520: 652e 6675 7279 2e69 6f2f 7079 2f70 796e  e.fury.io/py/pyn
-00000530: 6563 6f6e 6529 0a21 5b74 6573 7473 5d28  econe).![tests](
-00000540: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000550: 6f6d 2f70 796e 6563 6f6e 652d 696f 2f70  om/pynecone-io/p
-00000560: 796e 6563 6f6e 652f 6163 7469 6f6e 732f  ynecone/actions/
-00000570: 776f 726b 666c 6f77 732f 6275 696c 642e  workflows/build.
-00000580: 796d 6c2f 6261 6467 652e 7376 6729 0a21  yml/badge.svg).!
-00000590: 5b76 6572 7369 6f6e 735d 2868 7474 7073  [versions](https
-000005a0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-000005b0: 6f2f 7079 7069 2f70 7976 6572 7369 6f6e  o/pypi/pyversion
-000005c0: 732f 7079 6e65 636f 6e65 2d69 6f2e 7376  s/pynecone-io.sv
-000005d0: 6729 0a5b 215b 4469 7363 6f72 645d 2868  g).[![Discord](h
-000005e0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000005f0: 6473 2e69 6f2f 6469 7363 6f72 642f 3130  ds.io/discord/10
-00000600: 3239 3835 3330 3935 3532 3737 3237 3136  2985309552772716
-00000610: 353f 636f 6c6f 723d 2532 3337 3238 3964  5?color=%237289d
-00000620: 6126 6c61 6265 6c3d 4469 7363 6f72 6429  a&label=Discord)
-00000630: 5d28 6874 7470 733a 2f2f 6469 7363 6f72  ](https://discor
-00000640: 642e 6767 2f54 3557 5362 4332 5974 5129  d.gg/T5WSbC2YtQ)
-00000650: 0a0a 3c2f 6469 763e 0a0a 2323 2320 5245  ..</div>..### RE
-00000660: 4144 4d45 2069 6e20 6469 6666 6572 656e  ADME in differen
-00000670: 7420 6c61 6e67 7561 6765 0a0a 2d2d 2d0a  t language..---.
-00000680: 0a5b 456e 676c 6973 685d 2852 4541 444d  .[English](READM
-00000690: 452e 6d64 2920 7c20 5be7 b981 e9ab 94e4  E.md) | [.......
-000006a0: b8ad e696 875d 282f 646f 6373 2f7a 682f  .....](/docs/zh/
-000006b0: 7a68 5f74 772f 5245 4144 4d45 2e6d 6429  zh_tw/README.md)
-000006c0: 0a0a 2d2d 2d0a 0a23 2320 f09f 93a6 2031  ..---..## .... 1
-000006d0: 2e20 496e 7374 616c 6c0a 0a50 796e 6563  . Install..Pynec
-000006e0: 6f6e 6520 7265 7175 6972 6573 2074 6865  one requires the
-000006f0: 2066 6f6c 6c6f 7769 6e67 2074 6f20 6765   following to ge
-00000700: 7420 7374 6172 7465 643a 0a0a 2d20 2020  t started:..-   
-00000710: 5079 7468 6f6e 2033 2e37 2b0a 2d20 2020  Python 3.7+.-   
-00000720: 5b4e 6f64 652e 6a73 2031 362e 382e 302b  [Node.js 16.8.0+
-00000730: 5d28 6874 7470 733a 2f2f 6e6f 6465 6a73  ](https://nodejs
-00000740: 2e6f 7267 2f65 6e2f 2920 2844 6f6e 2774  .org/en/) (Don't
-00000750: 2077 6f72 7279 2c20 796f 7520 776f 6ee2   worry, you won.
-00000760: 8099 7420 6861 7665 2074 6f20 7772 6974  ..t have to writ
-00000770: 6520 616e 7920 4a61 7661 5363 7269 7074  e any JavaScript
-00000780: 2129 0a0a 6060 600a 7069 7020 696e 7374  !)..```.pip inst
-00000790: 616c 6c20 7079 6e65 636f 6e65 0a60 6060  all pynecone.```
-000007a0: 0a0a 2323 20f0 9fa5 b320 322e 2043 7265  ..## .... 2. Cre
-000007b0: 6174 6520 796f 7572 2066 6972 7374 2061  ate your first a
-000007c0: 7070 0a0a 496e 7374 616c 6c69 6e67 2050  pp..Installing P
-000007d0: 796e 6563 6f6e 6520 616c 736f 2069 6e73  ynecone also ins
-000007e0: 7461 6c6c 7320 7468 6520 6070 6360 2063  talls the `pc` c
-000007f0: 6f6d 6d61 6e64 206c 696e 6520 746f 6f6c  ommand line tool
-00000800: 2e20 5465 7374 2074 6861 7420 7468 6520  . Test that the 
-00000810: 696e 7374 616c 6c20 7761 7320 7375 6363  install was succ
-00000820: 6573 7366 756c 2062 7920 6372 6561 7469  essful by creati
-00000830: 6e67 2061 206e 6577 2070 726f 6a65 6374  ng a new project
-00000840: 2e0a 0a52 6570 6c61 6365 206d 795f 6170  ...Replace my_ap
-00000850: 705f 6e61 6d65 2077 6974 6820 796f 7572  p_name with your
-00000860: 2070 726f 6a65 6374 206e 616d 653a 0a0a   project name:..
-00000870: 6060 600a 6d6b 6469 7220 6d79 5f61 7070  ```.mkdir my_app
-00000880: 5f6e 616d 650a 6364 206d 795f 6170 705f  _name.cd my_app_
-00000890: 6e61 6d65 0a70 6320 696e 6974 0a60 6060  name.pc init.```
-000008a0: 0a0a 5768 656e 2079 6f75 2072 756e 2074  ..When you run t
-000008b0: 6869 7320 636f 6d6d 616e 6420 666f 7220  his command for 
-000008c0: 7468 6520 6669 7273 7420 7469 6d65 2c20  the first time, 
-000008d0: 7765 2077 696c 6c20 646f 776e 6c6f 6164  we will download
-000008e0: 2061 6e64 2069 6e73 7461 6c6c 205b 6275   and install [bu
-000008f0: 6e5d 2868 7474 7073 3a2f 2f62 756e 2e73  n](https://bun.s
-00000900: 682f 2920 6175 746f 6d61 7469 6361 6c6c  h/) automaticall
-00000910: 792e 0a0a 5468 6973 2063 6f6d 6d61 6e64  y...This command
-00000920: 2069 6e69 7469 616c 697a 6573 2061 2074   initializes a t
-00000930: 656d 706c 6174 6520 6170 7020 696e 2079  emplate app in y
-00000940: 6f75 7220 6e65 7720 6469 7265 6374 6f72  our new director
-00000950: 792e 0a0a 2323 20f0 9f8f 8320 332e 2052  y...## .... 3. R
-00000960: 756e 0a0a 596f 7520 6361 6e20 7275 6e20  un..You can run 
-00000970: 7468 6973 2061 7070 2069 6e20 6465 7665  this app in deve
-00000980: 6c6f 706d 656e 7420 6d6f 6465 3a0a 0a60  lopment mode:..`
-00000990: 6060 0a70 6320 7275 6e0a 6060 600a 0a59  ``.pc run.```..Y
-000009a0: 6f75 2073 686f 756c 6420 7365 6520 796f  ou should see yo
-000009b0: 7572 2061 7070 2072 756e 6e69 6e67 2061  ur app running a
-000009c0: 7420 6874 7470 3a2f 2f6c 6f63 616c 686f  t http://localho
-000009d0: 7374 3a33 3030 302e 0a0a 4e6f 7720 796f  st:3000...Now yo
-000009e0: 7520 6361 6e20 6d6f 6469 6679 2074 6865  u can modify the
-000009f0: 2073 6f75 7263 6520 636f 6465 2069 6e20   source code in 
-00000a00: 606d 795f 6170 705f 6e61 6d65 2f6d 795f  `my_app_name/my_
-00000a10: 6170 705f 6e61 6d65 2e70 7960 2e20 5079  app_name.py`. Py
-00000a20: 6e65 636f 6e65 2068 6173 2066 6173 7420  necone has fast 
-00000a30: 7265 6672 6573 6865 7320 736f 2079 6f75  refreshes so you
-00000a40: 2063 616e 2073 6565 2079 6f75 7220 6368   can see your ch
-00000a50: 616e 6765 7320 696e 7374 616e 746c 7920  anges instantly 
-00000a60: 7768 656e 2079 6f75 2073 6176 6520 796f  when you save yo
-00000a70: 7572 2063 6f64 652e 0a0a 2323 20f0 9fab  ur code...## ...
-00000a80: a720 4578 616d 706c 650a 0a4c 6574 2773  . Example..Let's
-00000a90: 2067 6f20 6f76 6572 2061 6e20 6578 616d   go over an exam
-00000aa0: 706c 653a 2063 7265 6174 696e 6720 616e  ple: creating an
-00000ab0: 2069 6d61 6765 2067 656e 6572 6174 696f   image generatio
-00000ac0: 6e20 5549 2061 726f 756e 6420 4441 4c4c  n UI around DALL
-00000ad0: c2b7 452e 2046 6f72 2073 696d 706c 6963  ..E. For simplic
-00000ae0: 6974 792c 2077 6520 6a75 7374 2063 616c  ity, we just cal
-00000af0: 6c20 7468 6520 4f70 656e 4149 2041 5049  l the OpenAI API
-00000b00: 2c20 6275 7420 796f 7520 636f 756c 6420  , but you could 
-00000b10: 7265 706c 6163 6520 7468 6973 2077 6974  replace this wit
-00000b20: 6820 616e 204d 4c20 6d6f 6465 6c20 7275  h an ML model ru
-00000b30: 6e20 6c6f 6361 6c6c 792e 0a0a 266e 6273  n locally...&nbs
-00000b40: 703b 0a0a 3c64 6976 2061 6c69 676e 3d22  p;..<div align="
-00000b50: 6365 6e74 6572 223e 0a3c 696d 6720 7372  center">.<img sr
-00000b60: 633d 2264 6f63 732f 696d 6167 6573 2f64  c="docs/images/d
-00000b70: 616c 6c65 2e67 6966 2220 616c 743d 2241  alle.gif" alt="A
-00000b80: 2066 726f 6e74 656e 6420 7772 6170 7065   frontend wrappe
-00000b90: 7220 666f 7220 4441 4c4c c2b7 452c 2073  r for DALL..E, s
-00000ba0: 686f 776e 2069 6e20 7468 6520 7072 6f63  hown in the proc
-00000bb0: 6573 7320 6f66 2067 656e 6572 6174 696e  ess of generatin
-00000bc0: 6720 616e 2069 6d61 6765 2e22 2077 6964  g an image." wid
-00000bd0: 7468 3d22 3535 3022 202f 3e0a 3c2f 6469  th="550" />.</di
-00000be0: 763e 0a0a 266e 6273 703b 0a0a 4865 7265  v>..&nbsp;..Here
-00000bf0: 2069 7320 7468 6520 636f 6d70 6c65 7465   is the complete
-00000c00: 2063 6f64 6520 746f 2063 7265 6174 6520   code to create 
-00000c10: 7468 6973 2e20 5468 6973 2069 7320 616c  this. This is al
-00000c20: 6c20 646f 6e65 2069 6e20 6f6e 6520 5079  l done in one Py
-00000c30: 7468 6f6e 2066 696c 6521 0a0a 6060 6070  thon file!..```p
-00000c40: 7974 686f 6e0a 696d 706f 7274 2070 796e  ython.import pyn
-00000c50: 6563 6f6e 6520 6173 2070 630a 696d 706f  econe as pc.impo
-00000c60: 7274 206f 7065 6e61 690a 0a6f 7065 6e61  rt openai..opena
-00000c70: 692e 6170 695f 6b65 7920 3d20 2259 4f55  i.api_key = "YOU
-00000c80: 525f 4150 495f 4b45 5922 0a0a 636c 6173  R_API_KEY"..clas
-00000c90: 7320 5374 6174 6528 7063 2e53 7461 7465  s State(pc.State
-00000ca0: 293a 0a20 2020 2022 2222 5468 6520 6170  ):.    """The ap
-00000cb0: 7020 7374 6174 652e 2222 220a 2020 2020  p state.""".    
-00000cc0: 7072 6f6d 7074 203d 2022 220a 2020 2020  prompt = "".    
-00000cd0: 696d 6167 655f 7572 6c20 3d20 2222 0a20  image_url = "". 
-00000ce0: 2020 2070 726f 6365 7373 696e 6720 3d20     processing = 
-00000cf0: 4661 6c73 650a 2020 2020 636f 6d70 6c65  False.    comple
-00000d00: 7465 203d 2046 616c 7365 0a0a 2020 2020  te = False..    
-00000d10: 6465 6620 6765 745f 696d 6167 6528 7365  def get_image(se
-00000d20: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00000d30: 4765 7420 7468 6520 696d 6167 6520 6672  Get the image fr
-00000d40: 6f6d 2074 6865 2070 726f 6d70 742e 2222  om the prompt.""
-00000d50: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
-00000d60: 662e 7072 6f6d 7074 203d 3d20 2222 3a0a  f.prompt == "":.
-00000d70: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00000d80: 726e 2070 632e 7769 6e64 6f77 5f61 6c65  rn pc.window_ale
-00000d90: 7274 2822 5072 6f6d 7074 2045 6d70 7479  rt("Prompt Empty
-00000da0: 2229 0a0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00000db0: 2e70 726f 6365 7373 696e 672c 2073 656c  .processing, sel
-00000dc0: 662e 636f 6d70 6c65 7465 203d 2054 7275  f.complete = Tru
-00000dd0: 652c 2046 616c 7365 0a20 2020 2020 2020  e, False.       
-00000de0: 2079 6965 6c64 0a20 2020 2020 2020 2072   yield.        r
-00000df0: 6573 706f 6e73 6520 3d20 6f70 656e 6169  esponse = openai
-00000e00: 2e49 6d61 6765 2e63 7265 6174 6528 7072  .Image.create(pr
-00000e10: 6f6d 7074 3d73 656c 662e 7072 6f6d 7074  ompt=self.prompt
-00000e20: 2c20 6e3d 312c 2073 697a 653d 2231 3032  , n=1, size="102
-00000e30: 3478 3130 3234 2229 0a20 2020 2020 2020  4x1024").       
-00000e40: 2073 656c 662e 696d 6167 655f 7572 6c20   self.image_url 
-00000e50: 3d20 7265 7370 6f6e 7365 5b22 6461 7461  = response["data
-00000e60: 225d 5b30 5d5b 2275 726c 225d 0a20 2020  "][0]["url"].   
-00000e70: 2020 2020 2073 656c 662e 7072 6f63 6573       self.proces
-00000e80: 7369 6e67 2c20 7365 6c66 2e63 6f6d 706c  sing, self.compl
-00000e90: 6574 6520 3d20 4661 6c73 652c 2054 7275  ete = False, Tru
-00000ea0: 650a 2020 2020 2020 2020 0a0a 6465 6620  e.        ..def 
-00000eb0: 696e 6465 7828 293a 0a20 2020 2072 6574  index():.    ret
-00000ec0: 7572 6e20 7063 2e63 656e 7465 7228 0a20  urn pc.center(. 
-00000ed0: 2020 2020 2020 2070 632e 7673 7461 636b         pc.vstack
-00000ee0: 280a 2020 2020 2020 2020 2020 2020 7063  (.            pc
-00000ef0: 2e68 6561 6469 6e67 2822 4441 4c4c c2b7  .heading("DALL..
-00000f00: 4522 292c 0a20 2020 2020 2020 2020 2020  E"),.           
-00000f10: 2070 632e 696e 7075 7428 706c 6163 6568   pc.input(placeh
-00000f20: 6f6c 6465 723d 2245 6e74 6572 2061 2070  older="Enter a p
-00000f30: 726f 6d70 7422 2c20 6f6e 5f62 6c75 723d  rompt", on_blur=
-00000f40: 5374 6174 652e 7365 745f 7072 6f6d 7074  State.set_prompt
-00000f50: 292c 0a20 2020 2020 2020 2020 2020 2070  ),.            p
-00000f60: 632e 6275 7474 6f6e 280a 2020 2020 2020  c.button(.      
-00000f70: 2020 2020 2020 2020 2020 2247 656e 6572            "Gener
-00000f80: 6174 6520 496d 6167 6522 2c0a 2020 2020  ate Image",.    
-00000f90: 2020 2020 2020 2020 2020 2020 6f6e 5f63              on_c
-00000fa0: 6c69 636b 3d53 7461 7465 2e67 6574 5f69  lick=State.get_i
-00000fb0: 6d61 6765 2c0a 2020 2020 2020 2020 2020  mage,.          
-00000fc0: 2020 2020 2020 6973 5f6c 6f61 6469 6e67        is_loading
-00000fd0: 3d53 7461 7465 2e70 726f 6365 7373 696e  =State.processin
-00000fe0: 672c 0a20 2020 2020 2020 2020 2020 2020  g,.             
-00000ff0: 2020 2077 6964 7468 3d22 3130 3025 222c     width="100%",
-00001000: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
-00001010: 2020 2020 2020 2020 2020 2020 7063 2e63              pc.c
-00001020: 6f6e 6428 0a20 2020 2020 2020 2020 2020  ond(.           
-00001030: 2020 2020 2053 7461 7465 2e63 6f6d 706c       State.compl
-00001040: 6574 652c 0a20 2020 2020 2020 2020 2020  ete,.           
-00001050: 2020 2020 2020 2020 2020 7063 2e69 6d61            pc.ima
-00001060: 6765 280a 2020 2020 2020 2020 2020 2020  ge(.            
-00001070: 2020 2020 2020 2020 2020 2020 2073 7263               src
-00001080: 3d53 7461 7465 2e69 6d61 6765 5f75 726c  =State.image_url
-00001090: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000010a0: 2020 2020 2020 2020 2020 2068 6569 6768             heigh
-000010b0: 743d 2232 3565 6d22 2c0a 2020 2020 2020  t="25em",.      
-000010c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010d0: 2020 2077 6964 7468 3d22 3235 656d 222c     width="25em",
-000010e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000010f0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00001100: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-00001110: 2020 7061 6464 696e 673d 2232 656d 222c    padding="2em",
-00001120: 0a20 2020 2020 2020 2020 2020 2073 6861  .            sha
-00001130: 646f 773d 226c 6722 2c0a 2020 2020 2020  dow="lg",.      
-00001140: 2020 2020 2020 626f 7264 6572 5f72 6164        border_rad
-00001150: 6975 733d 226c 6722 2c0a 2020 2020 2020  ius="lg",.      
-00001160: 2020 292c 0a20 2020 2020 2020 2077 6964    ),.        wid
-00001170: 7468 3d22 3130 3025 222c 0a20 2020 2020  th="100%",.     
-00001180: 2020 2068 6569 6768 743d 2231 3030 7668     height="100vh
-00001190: 222c 0a20 2020 2029 0a0a 2320 4164 6420  ",.    )..# Add 
-000011a0: 7374 6174 6520 616e 6420 7061 6765 2074  state and page t
-000011b0: 6f20 7468 6520 6170 702e 0a61 7070 203d  o the app..app =
-000011c0: 2070 632e 4170 7028 7374 6174 653d 5374   pc.App(state=St
-000011d0: 6174 6529 0a61 7070 2e61 6464 5f70 6167  ate).app.add_pag
-000011e0: 6528 696e 6465 782c 2074 6974 6c65 3d22  e(index, title="
-000011f0: 5079 6e65 636f 6e65 3a44 414c 4cc2 b745  Pynecone:DALL..E
-00001200: 2229 0a61 7070 2e63 6f6d 7069 6c65 2829  ").app.compile()
-00001210: 0a60 6060 0a0a 4c65 7427 7320 6272 6561  .```..Let's brea
-00001220: 6b20 7468 6973 2064 6f77 6e2e 0a0a 2323  k this down...##
-00001230: 2320 2a2a 5549 2049 6e20 5079 6e65 636f  # **UI In Pyneco
-00001240: 6e65 2a2a 0a0a 4c65 7427 7320 7374 6172  ne**..Let's star
-00001250: 7420 7769 7468 2074 6865 2055 492e 0a0a  t with the UI...
-00001260: 6060 6070 7974 686f 6e0a 6465 6620 696e  ```python.def in
-00001270: 6465 7828 293a 0a20 2020 2072 6574 7572  dex():.    retur
-00001280: 6e20 7063 2e63 656e 7465 7228 0a20 2020  n pc.center(.   
-00001290: 2020 2020 202e 2e2e 0a20 2020 2029 0a60       ....    ).`
-000012a0: 6060 0a0a 5468 6973 2060 696e 6465 7860  ``..This `index`
-000012b0: 2066 756e 6374 696f 6e20 6465 6669 6e65   function define
-000012c0: 7320 7468 6520 6672 6f6e 7465 6e64 206f  s the frontend o
-000012d0: 6620 7468 6520 6170 702e 0a0a 5765 2075  f the app...We u
-000012e0: 7365 2064 6966 6665 7265 6e74 2063 6f6d  se different com
-000012f0: 706f 6e65 6e74 7320 7375 6368 2061 7320  ponents such as 
-00001300: 6063 656e 7465 7260 2c20 6076 7374 6163  `center`, `vstac
-00001310: 6b60 2c20 6069 6e70 7574 602c 2061 6e64  k`, `input`, and
-00001320: 2060 6275 7474 6f6e 6020 746f 2062 7569   `button` to bui
-00001330: 6c64 2074 6865 2066 726f 6e74 656e 642e  ld the frontend.
-00001340: 2043 6f6d 706f 6e65 6e74 7320 6361 6e20   Components can 
-00001350: 6265 206e 6573 7465 6420 7769 7468 696e  be nested within
-00001360: 2065 6163 6820 6f74 6865 720a 746f 2063   each other.to c
-00001370: 7265 6174 6520 636f 6d70 6c65 7820 6c61  reate complex la
-00001380: 796f 7574 732e 2041 6e64 2079 6f75 2063  youts. And you c
-00001390: 616e 2075 7365 206b 6579 776f 7264 2061  an use keyword a
-000013a0: 7267 7320 746f 2073 7479 6c65 2074 6865  rgs to style the
-000013b0: 6d20 7769 7468 2074 6865 2066 756c 6c20  m with the full 
-000013c0: 706f 7765 7220 6f66 2043 5353 2e0a 0a50  power of CSS...P
-000013d0: 796e 6563 6f6e 6520 636f 6d65 7320 7769  ynecone comes wi
-000013e0: 7468 205b 3630 2b20 6275 696c 742d 696e  th [60+ built-in
-000013f0: 2063 6f6d 706f 6e65 6e74 735d 2868 7474   components](htt
-00001400: 7073 3a2f 2f70 796e 6563 6f6e 652e 696f  ps://pynecone.io
-00001410: 2f64 6f63 732f 6c69 6272 6172 7929 2074  /docs/library) t
-00001420: 6f20 6865 6c70 2079 6f75 2067 6574 2073  o help you get s
-00001430: 7461 7274 6564 2e20 5765 2061 7265 2061  tarted. We are a
-00001440: 6374 6976 656c 7920 6164 6469 6e67 206d  ctively adding m
-00001450: 6f72 6520 636f 6d70 6f6e 656e 7473 2c20  ore components, 
-00001460: 616e 6420 6974 2773 2065 6173 7920 746f  and it's easy to
-00001470: 205b 6372 6561 7465 2079 6f75 7220 6f77   [create your ow
-00001480: 6e20 636f 6d70 6f6e 656e 7473 5d28 6874  n components](ht
-00001490: 7470 733a 2f2f 7079 6e65 636f 6e65 2e69  tps://pynecone.i
-000014a0: 6f2f 646f 6373 2f61 6476 616e 6365 642d  o/docs/advanced-
-000014b0: 6775 6964 652f 7772 6170 7069 6e67 2d72  guide/wrapping-r
-000014c0: 6561 6374 292e 0a0a 2323 2320 2a2a 5374  eact)...### **St
-000014d0: 6174 652a 2a0a 0a50 796e 6563 6f6e 6520  ate**..Pynecone 
-000014e0: 7265 7072 6573 656e 7473 2079 6f75 7220  represents your 
-000014f0: 5549 2061 7320 6120 6675 6e63 7469 6f6e  UI as a function
-00001500: 206f 6620 796f 7572 2073 7461 7465 2e0a   of your state..
-00001510: 0a60 6060 7079 7468 6f6e 0a63 6c61 7373  .```python.class
-00001520: 2053 7461 7465 2870 632e 5374 6174 6529   State(pc.State)
-00001530: 3a0a 2020 2020 2222 2254 6865 2061 7070  :.    """The app
-00001540: 2073 7461 7465 2e22 2222 0a20 2020 2070   state.""".    p
-00001550: 726f 6d70 7420 3d20 2222 0a20 2020 2069  rompt = "".    i
-00001560: 6d61 6765 5f75 726c 203d 2022 220a 2020  mage_url = "".  
-00001570: 2020 7072 6f63 6573 7369 6e67 203d 2046    processing = F
-00001580: 616c 7365 0a20 2020 2063 6f6d 706c 6574  alse.    complet
-00001590: 6520 3d20 4661 6c73 650a 6060 600a 0a54  e = False.```..T
-000015a0: 6865 2073 7461 7465 2064 6566 696e 6573  he state defines
-000015b0: 2061 6c6c 2074 6865 2076 6172 6961 626c   all the variabl
-000015c0: 6573 2028 6361 6c6c 6564 2076 6172 7329  es (called vars)
-000015d0: 2069 6e20 616e 2061 7070 2074 6861 7420   in an app that 
-000015e0: 6361 6e20 6368 616e 6765 2061 6e64 2074  can change and t
-000015f0: 6865 2066 756e 6374 696f 6e73 2074 6861  he functions tha
-00001600: 7420 6368 616e 6765 2074 6865 6d2e 0a0a  t change them...
-00001610: 4865 7265 2074 6865 2073 7461 7465 2069  Here the state i
-00001620: 7320 636f 6d70 7269 7365 6420 6f66 2061  s comprised of a
-00001630: 2060 7072 6f6d 7074 6020 616e 6420 6069   `prompt` and `i
-00001640: 6d61 6765 5f75 726c 602e 2054 6865 7265  mage_url`. There
-00001650: 2061 7265 2061 6c73 6f20 7468 6520 626f   are also the bo
-00001660: 6f6c 6561 6e73 2060 7072 6f63 6573 7369  oleans `processi
-00001670: 6e67 6020 616e 6420 6063 6f6d 706c 6574  ng` and `complet
-00001680: 6560 2074 6f20 696e 6469 6361 7465 2077  e` to indicate w
-00001690: 6865 6e20 746f 2073 686f 7720 7468 6520  hen to show the 
-000016a0: 6369 7263 756c 6172 2070 726f 6772 6573  circular progres
-000016b0: 7320 616e 6420 696d 6167 652e 0a0a 2323  s and image...##
-000016c0: 2320 2a2a 4576 656e 7420 4861 6e64 6c65  # **Event Handle
-000016d0: 7273 2a2a 0a0a 6060 6070 7974 686f 6e0a  rs**..```python.
-000016e0: 6465 6620 6765 745f 696d 6167 6528 7365  def get_image(se
-000016f0: 6c66 293a 0a20 2020 2022 2222 4765 7420  lf):.    """Get 
-00001700: 7468 6520 696d 6167 6520 6672 6f6d 2074  the image from t
-00001710: 6865 2070 726f 6d70 742e 2222 220a 2020  he prompt.""".  
-00001720: 2020 6966 2073 656c 662e 7072 6f6d 7074    if self.prompt
-00001730: 203d 3d20 2222 3a0a 2020 2020 2020 2020   == "":.        
-00001740: 7265 7475 726e 2070 632e 7769 6e64 6f77  return pc.window
-00001750: 5f61 6c65 7274 2822 5072 6f6d 7074 2045  _alert("Prompt E
-00001760: 6d70 7479 2229 0a0a 2020 2020 7365 6c66  mpty")..    self
-00001770: 2e70 726f 6365 7373 696e 672c 2073 656c  .processing, sel
-00001780: 662e 636f 6d70 6c65 7465 203d 2054 7275  f.complete = Tru
-00001790: 652c 2046 616c 7365 0a20 2020 2079 6965  e, False.    yie
-000017a0: 6c64 0a20 2020 2072 6573 706f 6e73 6520  ld.    response 
-000017b0: 3d20 6f70 656e 6169 2e49 6d61 6765 2e63  = openai.Image.c
-000017c0: 7265 6174 6528 7072 6f6d 7074 3d73 656c  reate(prompt=sel
-000017d0: 662e 7072 6f6d 7074 2c20 6e3d 312c 2073  f.prompt, n=1, s
-000017e0: 697a 653d 2231 3032 3478 3130 3234 2229  ize="1024x1024")
-000017f0: 0a20 2020 2073 656c 662e 696d 6167 655f  .    self.image_
-00001800: 7572 6c20 3d20 7265 7370 6f6e 7365 5b22  url = response["
-00001810: 6461 7461 225d 5b30 5d5b 2275 726c 225d  data"][0]["url"]
-00001820: 0a20 2020 2073 656c 662e 7072 6f63 6573  .    self.proces
-00001830: 7369 6e67 2c20 7365 6c66 2e63 6f6d 706c  sing, self.compl
-00001840: 6574 6520 3d20 4661 6c73 652c 2054 7275  ete = False, Tru
-00001850: 650a 6060 600a 0a57 6974 6869 6e20 7468  e.```..Within th
-00001860: 6520 7374 6174 652c 2077 6520 6465 6669  e state, we defi
-00001870: 6e65 2066 756e 6374 696f 6e73 2063 616c  ne functions cal
-00001880: 6c65 6420 6576 656e 7420 6861 6e64 6c65  led event handle
-00001890: 7273 2074 6861 7420 6368 616e 6765 2074  rs that change t
-000018a0: 6865 2073 7461 7465 2076 6172 732e 2045  he state vars. E
-000018b0: 7665 6e74 2068 616e 646c 6572 7320 6172  vent handlers ar
-000018c0: 6520 7468 6520 7761 7920 7468 6174 2077  e the way that w
-000018d0: 6520 6361 6e20 6d6f 6469 6679 2074 6865  e can modify the
-000018e0: 2073 7461 7465 2069 6e20 5079 6e65 636f   state in Pyneco
-000018f0: 6e65 2e20 5468 6579 2063 616e 2062 6520  ne. They can be 
-00001900: 6361 6c6c 6564 2069 6e20 7265 7370 6f6e  called in respon
-00001910: 7365 2074 6f20 7573 6572 2061 6374 696f  se to user actio
-00001920: 6e73 2c20 7375 6368 2061 7320 636c 6963  ns, such as clic
-00001930: 6b69 6e67 2061 2062 7574 746f 6e20 6f72  king a button or
-00001940: 2074 7970 696e 6720 696e 2061 2074 6578   typing in a tex
-00001950: 7420 626f 782e 2054 6865 7365 2061 6374  t box. These act
-00001960: 696f 6e73 2061 7265 2063 616c 6c65 6420  ions are called 
-00001970: 6576 656e 7473 2e0a 0a4f 7572 2044 414c  events...Our DAL
-00001980: 4cc2 b745 2e20 6170 7020 6861 7320 616e  L..E. app has an
-00001990: 2065 7665 6e74 2068 616e 646c 6572 2c20   event handler, 
-000019a0: 6067 6574 5f69 6d61 6765 6020 746f 2077  `get_image` to w
-000019b0: 6869 6368 2067 6574 2074 6869 7320 696d  hich get this im
-000019c0: 6167 6520 6672 6f6d 2074 6865 204f 7065  age from the Ope
-000019d0: 6e41 4920 4150 492e 2055 7369 6e67 2060  nAI API. Using `
-000019e0: 7969 656c 6460 2069 6e20 7468 6520 6d69  yield` in the mi
-000019f0: 6464 6c65 206f 6620 616e 2065 7665 6e74  ddle of an event
-00001a00: 2068 616e 646c 6572 2077 696c 6c20 6361   handler will ca
-00001a10: 7573 6520 7468 6520 5549 2074 6f20 7570  use the UI to up
-00001a20: 6461 7465 2e20 4f74 6865 7277 6973 6520  date. Otherwise 
-00001a30: 7468 6520 5549 2077 696c 6c20 7570 6461  the UI will upda
-00001a40: 7465 2061 7420 7468 6520 656e 6420 6f66  te at the end of
-00001a50: 2074 6865 2065 7665 6e74 2068 616e 646c   the event handl
-00001a60: 6572 2e0a 0a23 2323 202a 2a52 6f75 7469  er...### **Routi
-00001a70: 6e67 2a2a 0a0a 4669 6e61 6c6c 792c 2077  ng**..Finally, w
-00001a80: 6520 6465 6669 6e65 206f 7572 2061 7070  e define our app
-00001a90: 2061 6e64 2070 6173 7320 6974 206f 7572   and pass it our
-00001aa0: 2073 7461 7465 2e0a 0a60 6060 7079 7468   state...```pyth
-00001ab0: 6f6e 0a61 7070 203d 2070 632e 4170 7028  on.app = pc.App(
-00001ac0: 7374 6174 653d 5374 6174 6529 0a60 6060  state=State).```
-00001ad0: 0a0a 5765 2061 6464 2061 2072 6f75 7465  ..We add a route
-00001ae0: 2066 726f 6d20 7468 6520 726f 6f74 206f   from the root o
-00001af0: 6620 7468 6520 6170 7020 746f 2074 6865  f the app to the
-00001b00: 2069 6e64 6578 2063 6f6d 706f 6e65 6e74   index component
-00001b10: 2e20 5765 2061 6c73 6f20 6164 6420 6120  . We also add a 
-00001b20: 7469 746c 6520 7468 6174 2077 696c 6c20  title that will 
-00001b30: 7368 6f77 2075 7020 696e 2074 6865 2070  show up in the p
-00001b40: 6167 6520 7072 6576 6965 772f 6272 6f77  age preview/brow
-00001b50: 7365 7220 7461 622e 0a0a 6060 6070 7974  ser tab...```pyt
-00001b60: 686f 6e0a 6170 702e 6164 645f 7061 6765  hon.app.add_page
-00001b70: 2869 6e64 6578 2c20 7469 746c 653d 2250  (index, title="P
-00001b80: 796e 6563 6f6e 653a 4441 4c4c 2d45 2229  ynecone:DALL-E")
-00001b90: 0a61 7070 2e63 6f6d 7069 6c65 2829 0a60  .app.compile().`
-00001ba0: 6060 0a0a 596f 7520 6361 6e20 6372 6561  ``..You can crea
-00001bb0: 7465 2061 206d 756c 7469 2d70 6167 6520  te a multi-page 
-00001bc0: 6170 7020 6279 2061 6464 696e 6720 6d6f  app by adding mo
-00001bd0: 7265 2072 6f75 7465 732e 0a0a 2323 2053  re routes...## S
-00001be0: 7461 7475 730a 0a50 796e 6563 6f6e 6520  tatus..Pynecone 
-00001bf0: 6c61 756e 6368 6564 2069 6e20 4465 6365  launched in Dece
-00001c00: 6d62 6572 2032 3032 322e 0a0a 4173 206f  mber 2022...As o
-00001c10: 6620 4a75 6e65 2032 3032 332c 2077 6520  f June 2023, we 
-00001c20: 6172 6520 696e 2074 6865 202a 2a50 7562  are in the **Pub
-00001c30: 6c69 6320 4265 7461 2a2a 2073 7461 6765  lic Beta** stage
-00001c40: 2e0a 0a2d 2020 203a 7768 6974 655f 6368  ...-   :white_ch
-00001c50: 6563 6b5f 6d61 726b 3a20 2a2a 5075 626c  eck_mark: **Publ
-00001c60: 6963 2041 6c70 6861 2a2a 3a20 416e 796f  ic Alpha**: Anyo
-00001c70: 6e65 2063 616e 2069 6e73 7461 6c6c 2061  ne can install a
-00001c80: 6e64 2075 7365 2050 796e 6563 6f6e 652e  nd use Pynecone.
-00001c90: 2054 6865 7265 206d 6179 2062 6520 6973   There may be is
-00001ca0: 7375 6573 2c20 6275 7420 7765 2061 7265  sues, but we are
-00001cb0: 2077 6f72 6b69 6e67 2074 6f20 7265 736f   working to reso
-00001cc0: 6c76 6520 7468 656d 2061 6374 6976 656c  lve them activel
-00001cd0: 792e 0a2d 2020 203a 6c61 7267 655f 6f72  y..-   :large_or
-00001ce0: 616e 6765 5f64 6961 6d6f 6e64 3a20 2a2a  ange_diamond: **
-00001cf0: 5075 626c 6963 2042 6574 612a 2a3a 2053  Public Beta**: S
-00001d00: 7461 626c 6520 656e 6f75 6768 2066 6f72  table enough for
-00001d10: 206e 6f6e 2d65 6e74 6572 7072 6973 6520   non-enterprise 
-00001d20: 7573 652d 6361 7365 732e 0a2d 2020 202a  use-cases..-   *
-00001d30: 2a50 7562 6c69 6320 486f 7374 696e 6720  *Public Hosting 
-00001d40: 4265 7461 2a2a 3a20 5f4f 7074 696f 6e61  Beta**: _Optiona
-00001d50: 6c6c 795f 2c20 6465 706c 6f79 2061 6e64  lly_, deploy and
-00001d60: 2068 6f73 7420 796f 7572 2061 7070 7320   host your apps 
-00001d70: 6f6e 2050 796e 6563 6f6e 6521 0a2d 2020  on Pynecone!.-  
-00001d80: 202a 2a50 7562 6c69 632a 2a3a 2050 796e   **Public**: Pyn
-00001d90: 6563 6f6e 6520 6973 2070 726f 6475 6374  econe is product
-00001da0: 696f 6e20 7265 6164 792e 0a0a 5079 6e65  ion ready...Pyne
-00001db0: 636f 6e65 2068 6173 206e 6577 2072 656c  cone has new rel
-00001dc0: 6561 7365 7320 616e 6420 6665 6174 7572  eases and featur
-00001dd0: 6573 2063 6f6d 696e 6720 6576 6572 7920  es coming every 
-00001de0: 7765 656b 2120 4d61 6b65 2073 7572 6520  week! Make sure 
-00001df0: 746f 203a 7374 6172 3a20 7374 6172 2061  to :star: star a
-00001e00: 6e64 203a 6579 6573 3a20 7761 7463 6820  nd :eyes: watch 
-00001e10: 7468 6973 2072 6570 6f73 6974 6f72 7920  this repository 
-00001e20: 746f 2073 7461 7920 7570 2074 6f20 6461  to stay up to da
-00001e30: 7465 2e0a 0a23 2320 436f 6e74 7269 6275  te...## Contribu
-00001e40: 7469 6e67 0a0a 5765 2077 656c 636f 6d65  ting..We welcome
-00001e50: 2063 6f6e 7472 6962 7574 696f 6e73 206f   contributions o
-00001e60: 6620 616e 7920 7369 7a65 2120 4265 6c6f  f any size! Belo
-00001e70: 7720 6172 6520 736f 6d65 2067 6f6f 6420  w are some good 
-00001e80: 7761 7973 2074 6f20 6765 7420 7374 6172  ways to get star
-00001e90: 7465 6420 696e 2074 6865 2050 796e 6563  ted in the Pynec
-00001ea0: 6f6e 6520 636f 6d6d 756e 6974 792e 0a0a  one community...
-00001eb0: 2d20 2020 2a2a 4a6f 696e 204f 7572 2044  -   **Join Our D
-00001ec0: 6973 636f 7264 2a2a 3a20 4f75 7220 5b44  iscord**: Our [D
-00001ed0: 6973 636f 7264 5d28 6874 7470 733a 2f2f  iscord](https://
-00001ee0: 6469 7363 6f72 642e 6767 2f54 3557 5362  discord.gg/T5WSb
-00001ef0: 4332 5974 5129 2069 7320 7468 6520 6265  C2YtQ) is the be
-00001f00: 7374 2070 6c61 6365 2074 6f20 6765 7420  st place to get 
-00001f10: 6865 6c70 206f 6e20 796f 7572 2050 796e  help on your Pyn
-00001f20: 6563 6f6e 6520 7072 6f6a 6563 7420 616e  econe project an
-00001f30: 6420 746f 2064 6973 6375 7373 2068 6f77  d to discuss how
-00001f40: 2079 6f75 2063 616e 2063 6f6e 7472 6962   you can contrib
-00001f50: 7574 652e 0a2d 2020 202a 2a47 6974 4875  ute..-   **GitHu
-00001f60: 6220 4469 7363 7573 7369 6f6e 732a 2a3a  b Discussions**:
-00001f70: 2041 2067 7265 6174 2077 6179 2074 6f20   A great way to 
-00001f80: 7461 6c6b 2061 626f 7574 2066 6561 7475  talk about featu
-00001f90: 7265 7320 796f 7520 7761 6e74 2061 6464  res you want add
-00001fa0: 6564 206f 7220 7468 696e 6773 2074 6861  ed or things tha
-00001fb0: 7420 6172 6520 636f 6e66 7573 696e 672f  t are confusing/
-00001fc0: 6e65 6564 2063 6c61 7269 6669 6361 7469  need clarificati
-00001fd0: 6f6e 2e0a 2d20 2020 2a2a 4769 7448 7562  on..-   **GitHub
-00001fe0: 2049 7373 7565 732a 2a3a 2054 6865 7365   Issues**: These
-00001ff0: 2061 7265 2061 6e20 6578 6365 6c6c 656e   are an excellen
-00002000: 7420 7761 7920 746f 2072 6570 6f72 7420  t way to report 
-00002010: 6275 6773 2e20 4164 6469 7469 6f6e 616c  bugs. Additional
-00002020: 6c79 2c20 796f 7520 6361 6e20 7472 7920  ly, you can try 
-00002030: 616e 6420 736f 6c76 6520 616e 2065 7869  and solve an exi
-00002040: 7374 696e 6720 6973 7375 6520 616e 6420  sting issue and 
-00002050: 7375 626d 6974 2061 2050 522e 0a0a 5765  submit a PR...We
-00002060: 2061 7265 2061 6374 6976 656c 7920 6c6f   are actively lo
-00002070: 6f6b 696e 6720 666f 7220 636f 6e74 7269  oking for contri
-00002080: 6275 746f 7273 2c20 6e6f 206d 6174 7465  butors, no matte
-00002090: 7220 796f 7572 2073 6b69 6c6c 206c 6576  r your skill lev
-000020a0: 656c 206f 7220 6578 7065 7269 656e 6365  el or experience
-000020b0: 2e0a 0a23 2320 4c69 6365 6e73 650a 0a50  ...## License..P
-000020c0: 796e 6563 6f6e 6520 6973 206f 7065 6e2d  ynecone is open-
-000020d0: 736f 7572 6365 2061 6e64 206c 6963 656e  source and licen
-000020e0: 7365 6420 756e 6465 7220 7468 6520 5b41  sed under the [A
-000020f0: 7061 6368 6520 4c69 6365 6e73 6520 322e  pache License 2.
-00002100: 305d 284c 4943 454e 5345 292e 0a         0](LICENSE)..
+00000000: 6060 6064 6966 660a 2b20 5365 6172 6368  ```diff.+ Search
+00000010: 696e 6720 666f 7220 5079 6e65 636f 6e65  ing for Pynecone
+00000020: 3f20 596f 7520 6172 6520 696e 2074 6865  ? You are in the
+00000030: 2072 6967 6874 2072 6570 6f2e 2050 796e   right repo. Pyn
+00000040: 6563 6f6e 6520 6861 7320 6265 656e 2072  econe has been r
+00000050: 656e 616d 6564 2074 6f20 5265 666c 6578  enamed to Reflex
+00000060: 2e20 2b0a 6060 600a 0a3c 6469 7620 616c  . +.```..<div al
+00000070: 6967 6e3d 2263 656e 7465 7222 3e0a 0a3c  ign="center">..<
+00000080: 696d 6720 7372 633d 2264 6f63 732f 696d  img src="docs/im
+00000090: 6167 6573 2f72 6566 6c65 782e 706e 6722  ages/reflex.png"
+000000a0: 3e0a 3c68 723e 0a0a 2320 2a2a 5265 666c  >.<hr>..# **Refl
+000000b0: 6578 2a2a 200a 2a2a e29c a820 5065 7266  ex** .**... Perf
+000000c0: 6f72 6d61 6e74 2c20 6375 7374 6f6d 697a  ormant, customiz
+000000d0: 6162 6c65 2077 6562 2061 7070 7320 696e  able web apps in
+000000e0: 2070 7572 6520 5079 7468 6f6e 2e20 4465   pure Python. De
+000000f0: 706c 6f79 2069 6e20 7365 636f 6e64 732e  ploy in seconds.
+00000100: 2a2a 0a0a f09f 9391 205b 446f 6373 5d28  **...... [Docs](
+00000110: 6874 7470 733a 2f2f 7265 666c 6578 2e64  https://reflex.d
+00000120: 6576 2f64 6f63 732f 6765 7474 696e 672d  ev/docs/getting-
+00000130: 7374 6172 7465 642f 696e 7472 6f64 7563  started/introduc
+00000140: 7469 6f6e 2920 266e 6273 703b 20f0 9f93  tion) &nbsp; ...
+00000150: b120 5b43 6f6d 706f 6e65 6e74 204c 6962  . [Component Lib
+00000160: 7261 7279 5d28 6874 7470 733a 2f2f 7265  rary](https://re
+00000170: 666c 6578 2e64 6576 2f64 6f63 732f 6c69  flex.dev/docs/li
+00000180: 6272 6172 7929 2026 6e62 7370 3b20 f09f  brary) &nbsp; ..
+00000190: 96bc efb8 8f20 5b47 616c 6c65 7279 5d28  ..... [Gallery](
+000001a0: 6874 7470 733a 2f2f 7265 666c 6578 2e64  https://reflex.d
+000001b0: 6576 2f64 6f63 732f 6761 6c6c 6572 7929  ev/docs/gallery)
+000001c0: 2026 6e62 7370 3b20 f09f 9bb8 205b 4465   &nbsp; .... [De
+000001d0: 706c 6f79 6d65 6e74 5d28 6874 7470 733a  ployment](https:
+000001e0: 2f2f 7265 666c 6578 2e64 6576 2f64 6f63  //reflex.dev/doc
+000001f0: 732f 686f 7374 696e 672f 6465 706c 6f79  s/hosting/deploy
+00000200: 290a 0a5b 215b 5079 5049 2076 6572 7369  )..[![PyPI versi
+00000210: 6f6e 5d28 6874 7470 733a 2f2f 6261 6467  on](https://badg
+00000220: 652e 6675 7279 2e69 6f2f 7079 2f72 6566  e.fury.io/py/ref
+00000230: 6c65 782e 7376 6729 5d28 6874 7470 733a  lex.svg)](https:
+00000240: 2f2f 6261 6467 652e 6675 7279 2e69 6f2f  //badge.fury.io/
+00000250: 7079 2f72 6566 6c65 7829 0a21 5b74 6573  py/reflex).![tes
+00000260: 7473 5d28 6874 7470 733a 2f2f 6769 7468  ts](https://gith
+00000270: 7562 2e63 6f6d 2f70 796e 6563 6f6e 652d  ub.com/pynecone-
+00000280: 696f 2f70 796e 6563 6f6e 652f 6163 7469  io/pynecone/acti
+00000290: 6f6e 732f 776f 726b 666c 6f77 732f 6275  ons/workflows/bu
+000002a0: 696c 642e 796d 6c2f 6261 6467 652e 7376  ild.yml/badge.sv
+000002b0: 6729 0a21 5b76 6572 7369 6f6e 735d 2868  g).![versions](h
+000002c0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000002d0: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
+000002e0: 7369 6f6e 732f 7265 666c 6578 2e73 7667  sions/reflex.svg
+000002f0: 290a 5b21 5b44 6973 636f 7264 5d28 6874  ).[![Discord](ht
+00000300: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000310: 732e 696f 2f64 6973 636f 7264 2f31 3032  s.io/discord/102
+00000320: 3938 3533 3039 3535 3237 3732 3731 3635  9853095527727165
+00000330: 3f63 6f6c 6f72 3d25 3233 3732 3839 6461  ?color=%237289da
+00000340: 266c 6162 656c 3d44 6973 636f 7264 295d  &label=Discord)]
+00000350: 2868 7474 7073 3a2f 2f64 6973 636f 7264  (https://discord
+00000360: 2e67 672f 5435 5753 6243 3259 7451 290a  .gg/T5WSbC2YtQ).
+00000370: 0a3c 2f64 6976 3e0a 0a23 2323 2052 4541  .</div>..### REA
+00000380: 444d 4520 696e 2064 6966 6665 7265 6e74  DME in different
+00000390: 206c 616e 6775 6167 650a 0a2d 2d2d 0a0a   language..---..
+000003a0: 5b45 6e67 6c69 7368 5d28 5245 4144 4d45  [English](README
+000003b0: 2e6d 6429 207c 205b e7ae 80e4 bd93 e4b8  .md) | [........
+000003c0: ade6 9687 5d28 2f64 6f63 732f 7a68 2f7a  ....](/docs/zh/z
+000003d0: 685f 636e 2f52 4541 444d 452e 6d64 2920  h_cn/README.md) 
+000003e0: 7c20 5be7 b981 e9ab 94e4 b8ad e696 875d  | [............]
+000003f0: 282f 646f 6373 2f7a 682f 7a68 5f74 772f  (/docs/zh/zh_tw/
+00000400: 5245 4144 4d45 2e6d 6429 0a0a 2d2d 2d0a  README.md)..---.
+00000410: 0a23 2320 f09f 93a6 2031 2e20 496e 7374  .## .... 1. Inst
+00000420: 616c 6c0a 0a52 6566 6c65 7820 7265 7175  all..Reflex requ
+00000430: 6972 6573 2074 6865 2066 6f6c 6c6f 7769  ires the followi
+00000440: 6e67 2074 6f20 6765 7420 7374 6172 7465  ng to get starte
+00000450: 643a 0a0a 2d20 2020 5079 7468 6f6e 2033  d:..-   Python 3
+00000460: 2e37 2b0a 2d20 2020 5b4e 6f64 652e 6a73  .7+.-   [Node.js
+00000470: 2031 362e 382e 302b 5d28 6874 7470 733a   16.8.0+](https:
+00000480: 2f2f 6e6f 6465 6a73 2e6f 7267 2f65 6e2f  //nodejs.org/en/
+00000490: 2920 2844 6f6e 2774 2077 6f72 7279 2c20  ) (Don't worry, 
+000004a0: 796f 7520 776f 6ee2 8099 7420 6861 7665  you won...t have
+000004b0: 2074 6f20 7772 6974 6520 616e 7920 4a61   to write any Ja
+000004c0: 7661 5363 7269 7074 2129 0a0a 6060 600a  vaScript!)..```.
+000004d0: 7069 7020 696e 7374 616c 6c20 7265 666c  pip install refl
+000004e0: 6578 0a60 6060 0a0a 2323 20f0 9fa5 b320  ex.```..## .... 
+000004f0: 322e 2043 7265 6174 6520 796f 7572 2066  2. Create your f
+00000500: 6972 7374 2061 7070 0a0a 496e 7374 616c  irst app..Instal
+00000510: 6c69 6e67 2060 7265 666c 6578 6020 616c  ling `reflex` al
+00000520: 736f 2069 6e73 7461 6c6c 7320 7468 6520  so installs the 
+00000530: 6072 6566 6c65 7860 2063 6f6d 6d61 6e64  `reflex` command
+00000540: 206c 696e 6520 746f 6f6c 2e20 5465 7374   line tool. Test
+00000550: 2074 6861 7420 7468 6520 696e 7374 616c   that the instal
+00000560: 6c20 7761 7320 7375 6363 6573 7366 756c  l was successful
+00000570: 2062 7920 6372 6561 7469 6e67 2061 206e   by creating a n
+00000580: 6577 2070 726f 6a65 6374 2e0a 0a52 6570  ew project...Rep
+00000590: 6c61 6365 206d 795f 6170 705f 6e61 6d65  lace my_app_name
+000005a0: 2077 6974 6820 796f 7572 2070 726f 6a65   with your proje
+000005b0: 6374 206e 616d 653a 0a0a 6060 600a 6d6b  ct name:..```.mk
+000005c0: 6469 7220 6d79 5f61 7070 5f6e 616d 650a  dir my_app_name.
+000005d0: 6364 206d 795f 6170 705f 6e61 6d65 0a72  cd my_app_name.r
+000005e0: 6566 6c65 7820 696e 6974 0a60 6060 0a0a  eflex init.```..
+000005f0: 5768 656e 2079 6f75 2072 756e 2074 6869  When you run thi
+00000600: 7320 636f 6d6d 616e 6420 666f 7220 7468  s command for th
+00000610: 6520 6669 7273 7420 7469 6d65 2c20 7765  e first time, we
+00000620: 2077 696c 6c20 646f 776e 6c6f 6164 2061   will download a
+00000630: 6e64 2069 6e73 7461 6c6c 205b 6275 6e5d  nd install [bun]
+00000640: 2868 7474 7073 3a2f 2f62 756e 2e73 682f  (https://bun.sh/
+00000650: 2920 6175 746f 6d61 7469 6361 6c6c 792e  ) automatically.
+00000660: 0a0a 5468 6973 2063 6f6d 6d61 6e64 2069  ..This command i
+00000670: 6e69 7469 616c 697a 6573 2061 2074 656d  nitializes a tem
+00000680: 706c 6174 6520 6170 7020 696e 2079 6f75  plate app in you
+00000690: 7220 6e65 7720 6469 7265 6374 6f72 792e  r new directory.
+000006a0: 0a0a 2323 20f0 9f8f 8320 332e 2052 756e  ..## .... 3. Run
+000006b0: 2079 6f75 7220 6170 700a 0a59 6f75 2063   your app..You c
+000006c0: 616e 2072 756e 2074 6869 7320 6170 7020  an run this app 
+000006d0: 696e 2064 6576 656c 6f70 6d65 6e74 206d  in development m
+000006e0: 6f64 653a 0a0a 6060 600a 7265 666c 6578  ode:..```.reflex
+000006f0: 2072 756e 0a60 6060 0a0a 596f 7520 7368   run.```..You sh
+00000700: 6f75 6c64 2073 6565 2079 6f75 7220 6170  ould see your ap
+00000710: 7020 7275 6e6e 696e 6720 6174 2068 7474  p running at htt
+00000720: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3330  p://localhost:30
+00000730: 3030 2e0a 0a4e 6f77 2079 6f75 2063 616e  00...Now you can
+00000740: 206d 6f64 6966 7920 7468 6520 736f 7572   modify the sour
+00000750: 6365 2063 6f64 6520 696e 2060 6d79 5f61  ce code in `my_a
+00000760: 7070 5f6e 616d 652f 6d79 5f61 7070 5f6e  pp_name/my_app_n
+00000770: 616d 652e 7079 602e 2052 6566 6c65 7820  ame.py`. Reflex 
+00000780: 6861 7320 6661 7374 2072 6566 7265 7368  has fast refresh
+00000790: 6573 2073 6f20 796f 7520 6361 6e20 7365  es so you can se
+000007a0: 6520 796f 7572 2063 6861 6e67 6573 2069  e your changes i
+000007b0: 6e73 7461 6e74 6c79 2077 6865 6e20 796f  nstantly when yo
+000007c0: 7520 7361 7665 2079 6f75 7220 636f 6465  u save your code
+000007d0: 2e0a 0a23 2320 f09f aba7 2045 7861 6d70  ...## .... Examp
+000007e0: 6c65 0a0a 4c65 7427 7320 676f 206f 7665  le..Let's go ove
+000007f0: 7220 616e 2065 7861 6d70 6c65 3a20 6372  r an example: cr
+00000800: 6561 7469 6e67 2061 6e20 696d 6167 6520  eating an image 
+00000810: 6765 6e65 7261 7469 6f6e 2055 4920 6172  generation UI ar
+00000820: 6f75 6e64 2044 414c 4cc2 b745 2e20 466f  ound DALL..E. Fo
+00000830: 7220 7369 6d70 6c69 6369 7479 2c20 7765  r simplicity, we
+00000840: 206a 7573 7420 6361 6c6c 2074 6865 204f   just call the O
+00000850: 7065 6e41 4920 4150 492c 2062 7574 2079  penAI API, but y
+00000860: 6f75 2063 6f75 6c64 2072 6570 6c61 6365  ou could replace
+00000870: 2074 6869 7320 7769 7468 2061 6e20 4d4c   this with an ML
+00000880: 206d 6f64 656c 2072 756e 206c 6f63 616c   model run local
+00000890: 6c79 2e0a 0a26 6e62 7370 3b0a 0a3c 6469  ly...&nbsp;..<di
+000008a0: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
+000008b0: 3e0a 3c69 6d67 2073 7263 3d22 646f 6373  >.<img src="docs
+000008c0: 2f69 6d61 6765 732f 6461 6c6c 652e 6769  /images/dalle.gi
+000008d0: 6622 2061 6c74 3d22 4120 6672 6f6e 7465  f" alt="A fronte
+000008e0: 6e64 2077 7261 7070 6572 2066 6f72 2044  nd wrapper for D
+000008f0: 414c 4cc2 b745 2c20 7368 6f77 6e20 696e  ALL..E, shown in
+00000900: 2074 6865 2070 726f 6365 7373 206f 6620   the process of 
+00000910: 6765 6e65 7261 7469 6e67 2061 6e20 696d  generating an im
+00000920: 6167 652e 2220 7769 6474 683d 2235 3530  age." width="550
+00000930: 2220 2f3e 0a3c 2f64 6976 3e0a 0a26 6e62  " />.</div>..&nb
+00000940: 7370 3b0a 0a48 6572 6520 6973 2074 6865  sp;..Here is the
+00000950: 2063 6f6d 706c 6574 6520 636f 6465 2074   complete code t
+00000960: 6f20 6372 6561 7465 2074 6869 732e 2054  o create this. T
+00000970: 6869 7320 6973 2061 6c6c 2064 6f6e 6520  his is all done 
+00000980: 696e 206f 6e65 2050 7974 686f 6e20 6669  in one Python fi
+00000990: 6c65 210a 0a60 6060 7079 7468 6f6e 0a69  le!..```python.i
+000009a0: 6d70 6f72 7420 7265 666c 6578 2061 7320  mport reflex as 
+000009b0: 7278 0a69 6d70 6f72 7420 6f70 656e 6169  rx.import openai
+000009c0: 0a0a 6f70 656e 6169 2e61 7069 5f6b 6579  ..openai.api_key
+000009d0: 203d 2022 594f 5552 5f41 5049 5f4b 4559   = "YOUR_API_KEY
+000009e0: 220a 0a63 6c61 7373 2053 7461 7465 2872  "..class State(r
+000009f0: 782e 5374 6174 6529 3a0a 2020 2020 2222  x.State):.    ""
+00000a00: 2254 6865 2061 7070 2073 7461 7465 2e22  "The app state."
+00000a10: 2222 0a20 2020 2070 726f 6d70 7420 3d20  "".    prompt = 
+00000a20: 2222 0a20 2020 2069 6d61 6765 5f75 726c  "".    image_url
+00000a30: 203d 2022 220a 2020 2020 7072 6f63 6573   = "".    proces
+00000a40: 7369 6e67 203d 2046 616c 7365 0a20 2020  sing = False.   
+00000a50: 2063 6f6d 706c 6574 6520 3d20 4661 6c73   complete = Fals
+00000a60: 650a 0a20 2020 2064 6566 2067 6574 5f69  e..    def get_i
+00000a70: 6d61 6765 2873 656c 6629 3a0a 2020 2020  mage(self):.    
+00000a80: 2020 2020 2222 2247 6574 2074 6865 2069      """Get the i
+00000a90: 6d61 6765 2066 726f 6d20 7468 6520 7072  mage from the pr
+00000aa0: 6f6d 7074 2e22 2222 0a20 2020 2020 2020  ompt.""".       
+00000ab0: 2069 6620 7365 6c66 2e70 726f 6d70 7420   if self.prompt 
+00000ac0: 3d3d 2022 223a 0a20 2020 2020 2020 2020  == "":.         
+00000ad0: 2020 2072 6574 7572 6e20 7278 2e77 696e     return rx.win
+00000ae0: 646f 775f 616c 6572 7428 2250 726f 6d70  dow_alert("Promp
+00000af0: 7420 456d 7074 7922 290a 0a20 2020 2020  t Empty")..     
+00000b00: 2020 2073 656c 662e 7072 6f63 6573 7369     self.processi
+00000b10: 6e67 2c20 7365 6c66 2e63 6f6d 706c 6574  ng, self.complet
+00000b20: 6520 3d20 5472 7565 2c20 4661 6c73 650a  e = True, False.
+00000b30: 2020 2020 2020 2020 7969 656c 640a 2020          yield.  
+00000b40: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+00000b50: 206f 7065 6e61 692e 496d 6167 652e 6372   openai.Image.cr
+00000b60: 6561 7465 2870 726f 6d70 743d 7365 6c66  eate(prompt=self
+00000b70: 2e70 726f 6d70 742c 206e 3d31 2c20 7369  .prompt, n=1, si
+00000b80: 7a65 3d22 3130 3234 7831 3032 3422 290a  ze="1024x1024").
+00000b90: 2020 2020 2020 2020 7365 6c66 2e69 6d61          self.ima
+00000ba0: 6765 5f75 726c 203d 2072 6573 706f 6e73  ge_url = respons
+00000bb0: 655b 2264 6174 6122 5d5b 305d 5b22 7572  e["data"][0]["ur
+00000bc0: 6c22 5d0a 2020 2020 2020 2020 7365 6c66  l"].        self
+00000bd0: 2e70 726f 6365 7373 696e 672c 2073 656c  .processing, sel
+00000be0: 662e 636f 6d70 6c65 7465 203d 2046 616c  f.complete = Fal
+00000bf0: 7365 2c20 5472 7565 0a20 2020 2020 2020  se, True.       
+00000c00: 200a 0a64 6566 2069 6e64 6578 2829 3a0a   ..def index():.
+00000c10: 2020 2020 7265 7475 726e 2072 782e 6365      return rx.ce
+00000c20: 6e74 6572 280a 2020 2020 2020 2020 7278  nter(.        rx
+00000c30: 2e76 7374 6163 6b28 0a20 2020 2020 2020  .vstack(.       
+00000c40: 2020 2020 2072 782e 6865 6164 696e 6728       rx.heading(
+00000c50: 2244 414c 4cc2 b745 2229 2c0a 2020 2020  "DALL..E"),.    
+00000c60: 2020 2020 2020 2020 7278 2e69 6e70 7574          rx.input
+00000c70: 2870 6c61 6365 686f 6c64 6572 3d22 456e  (placeholder="En
+00000c80: 7465 7220 6120 7072 6f6d 7074 222c 206f  ter a prompt", o
+00000c90: 6e5f 626c 7572 3d53 7461 7465 2e73 6574  n_blur=State.set
+00000ca0: 5f70 726f 6d70 7429 2c0a 2020 2020 2020  _prompt),.      
+00000cb0: 2020 2020 2020 7278 2e62 7574 746f 6e28        rx.button(
+00000cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000cd0: 2022 4765 6e65 7261 7465 2049 6d61 6765   "Generate Image
+00000ce0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00000cf0: 2020 206f 6e5f 636c 6963 6b3d 5374 6174     on_click=Stat
+00000d00: 652e 6765 745f 696d 6167 652c 0a20 2020  e.get_image,.   
+00000d10: 2020 2020 2020 2020 2020 2020 2069 735f               is_
+00000d20: 6c6f 6164 696e 673d 5374 6174 652e 7072  loading=State.pr
+00000d30: 6f63 6573 7369 6e67 2c0a 2020 2020 2020  ocessing,.      
+00000d40: 2020 2020 2020 2020 2020 7769 6474 683d            width=
+00000d50: 2231 3030 2522 2c0a 2020 2020 2020 2020  "100%",.        
+00000d60: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00000d70: 2020 2072 782e 636f 6e64 280a 2020 2020     rx.cond(.    
+00000d80: 2020 2020 2020 2020 2020 2020 5374 6174              Stat
+00000d90: 652e 636f 6d70 6c65 7465 2c0a 2020 2020  e.complete,.    
+00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000db0: 2072 782e 696d 6167 6528 0a20 2020 2020   rx.image(.     
+00000dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000dd0: 2020 2020 7372 633d 5374 6174 652e 696d      src=State.im
+00000de0: 6167 655f 7572 6c2c 0a20 2020 2020 2020  age_url,.       
+00000df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e00: 2020 6865 6967 6874 3d22 3235 656d 222c    height="25em",
+00000e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000e20: 2020 2020 2020 2020 2020 7769 6474 683d            width=
+00000e30: 2232 3565 6d22 2c0a 2020 2020 2020 2020  "25em",.        
+00000e40: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00000e50: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+00000e60: 2020 2020 2020 2020 2070 6164 6469 6e67           padding
+00000e70: 3d22 3265 6d22 2c0a 2020 2020 2020 2020  ="2em",.        
+00000e80: 2020 2020 7368 6164 6f77 3d22 6c67 222c      shadow="lg",
+00000e90: 0a20 2020 2020 2020 2020 2020 2062 6f72  .            bor
+00000ea0: 6465 725f 7261 6469 7573 3d22 6c67 222c  der_radius="lg",
+00000eb0: 0a20 2020 2020 2020 2029 2c0a 2020 2020  .        ),.    
+00000ec0: 2020 2020 7769 6474 683d 2231 3030 2522      width="100%"
+00000ed0: 2c0a 2020 2020 2020 2020 6865 6967 6874  ,.        height
+00000ee0: 3d22 3130 3076 6822 2c0a 2020 2020 290a  ="100vh",.    ).
+00000ef0: 0a23 2041 6464 2073 7461 7465 2061 6e64  .# Add state and
+00000f00: 2070 6167 6520 746f 2074 6865 2061 7070   page to the app
+00000f10: 2e0a 6170 7020 3d20 7278 2e41 7070 2873  ..app = rx.App(s
+00000f20: 7461 7465 3d53 7461 7465 290a 6170 702e  tate=State).app.
+00000f30: 6164 645f 7061 6765 2869 6e64 6578 2c20  add_page(index, 
+00000f40: 7469 746c 653d 2272 6566 6c65 783a 4441  title="reflex:DA
+00000f50: 4c4c c2b7 4522 290a 6170 702e 636f 6d70  LL..E").app.comp
+00000f60: 696c 6528 290a 6060 600a 0a4c 6574 2773  ile().```..Let's
+00000f70: 2062 7265 616b 2074 6869 7320 646f 776e   break this down
+00000f80: 2e0a 0a23 2323 202a 2a55 4920 496e 2052  ...### **UI In R
+00000f90: 6566 6c65 782a 2a0a 0a4c 6574 2773 2073  eflex**..Let's s
+00000fa0: 7461 7274 2077 6974 6820 7468 6520 5549  tart with the UI
+00000fb0: 2e0a 0a60 6060 7079 7468 6f6e 0a64 6566  ...```python.def
+00000fc0: 2069 6e64 6578 2829 3a0a 2020 2020 7265   index():.    re
+00000fd0: 7475 726e 2072 782e 6365 6e74 6572 280a  turn rx.center(.
+00000fe0: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
+00000ff0: 290a 6060 600a 0a54 6869 7320 6069 6e64  ).```..This `ind
+00001000: 6578 6020 6675 6e63 7469 6f6e 2064 6566  ex` function def
+00001010: 696e 6573 2074 6865 2066 726f 6e74 656e  ines the fronten
+00001020: 6420 6f66 2074 6865 2061 7070 2e0a 0a57  d of the app...W
+00001030: 6520 7573 6520 6469 6666 6572 656e 7420  e use different 
+00001040: 636f 6d70 6f6e 656e 7473 2073 7563 6820  components such 
+00001050: 6173 2060 6365 6e74 6572 602c 2060 7673  as `center`, `vs
+00001060: 7461 636b 602c 2060 696e 7075 7460 2c20  tack`, `input`, 
+00001070: 616e 6420 6062 7574 746f 6e60 2074 6f20  and `button` to 
+00001080: 6275 696c 6420 7468 6520 6672 6f6e 7465  build the fronte
+00001090: 6e64 2e20 436f 6d70 6f6e 656e 7473 2063  nd. Components c
+000010a0: 616e 2062 6520 6e65 7374 6564 2077 6974  an be nested wit
+000010b0: 6869 6e20 6561 6368 206f 7468 6572 0a74  hin each other.t
+000010c0: 6f20 6372 6561 7465 2063 6f6d 706c 6578  o create complex
+000010d0: 206c 6179 6f75 7473 2e20 416e 6420 796f   layouts. And yo
+000010e0: 7520 6361 6e20 7573 6520 6b65 7977 6f72  u can use keywor
+000010f0: 6420 6172 6773 2074 6f20 7374 796c 6520  d args to style 
+00001100: 7468 656d 2077 6974 6820 7468 6520 6675  them with the fu
+00001110: 6c6c 2070 6f77 6572 206f 6620 4353 532e  ll power of CSS.
+00001120: 0a0a 5265 666c 6578 2063 6f6d 6573 2077  ..Reflex comes w
+00001130: 6974 6820 5b36 302b 2062 7569 6c74 2d69  ith [60+ built-i
+00001140: 6e20 636f 6d70 6f6e 656e 7473 5d28 6874  n components](ht
+00001150: 7470 733a 2f2f 7265 666c 6578 2e64 6576  tps://reflex.dev
+00001160: 2f64 6f63 732f 6c69 6272 6172 7929 2074  /docs/library) t
+00001170: 6f20 6865 6c70 2079 6f75 2067 6574 2073  o help you get s
+00001180: 7461 7274 6564 2e20 5765 2061 7265 2061  tarted. We are a
+00001190: 6374 6976 656c 7920 6164 6469 6e67 206d  ctively adding m
+000011a0: 6f72 6520 636f 6d70 6f6e 656e 7473 2c20  ore components, 
+000011b0: 616e 6420 6974 2773 2065 6173 7920 746f  and it's easy to
+000011c0: 205b 6372 6561 7465 2079 6f75 7220 6f77   [create your ow
+000011d0: 6e20 636f 6d70 6f6e 656e 7473 5d28 6874  n components](ht
+000011e0: 7470 733a 2f2f 7265 666c 6578 2e64 6576  tps://reflex.dev
+000011f0: 2f64 6f63 732f 6164 7661 6e63 6564 2d67  /docs/advanced-g
+00001200: 7569 6465 2f77 7261 7070 696e 672d 7265  uide/wrapping-re
+00001210: 6163 7429 2e0a 0a23 2323 202a 2a53 7461  act)...### **Sta
+00001220: 7465 2a2a 0a0a 5265 666c 6578 2072 6570  te**..Reflex rep
+00001230: 7265 7365 6e74 7320 796f 7572 2055 4920  resents your UI 
+00001240: 6173 2061 2066 756e 6374 696f 6e20 6f66  as a function of
+00001250: 2079 6f75 7220 7374 6174 652e 0a0a 6060   your state...``
+00001260: 6070 7974 686f 6e0a 636c 6173 7320 5374  `python.class St
+00001270: 6174 6528 7278 2e53 7461 7465 293a 0a20  ate(rx.State):. 
+00001280: 2020 2022 2222 5468 6520 6170 7020 7374     """The app st
+00001290: 6174 652e 2222 220a 2020 2020 7072 6f6d  ate.""".    prom
+000012a0: 7074 203d 2022 220a 2020 2020 696d 6167  pt = "".    imag
+000012b0: 655f 7572 6c20 3d20 2222 0a20 2020 2070  e_url = "".    p
+000012c0: 726f 6365 7373 696e 6720 3d20 4661 6c73  rocessing = Fals
+000012d0: 650a 2020 2020 636f 6d70 6c65 7465 203d  e.    complete =
+000012e0: 2046 616c 7365 0a60 6060 0a0a 5468 6520   False.```..The 
+000012f0: 7374 6174 6520 6465 6669 6e65 7320 616c  state defines al
+00001300: 6c20 7468 6520 7661 7269 6162 6c65 7320  l the variables 
+00001310: 2863 616c 6c65 6420 7661 7273 2920 696e  (called vars) in
+00001320: 2061 6e20 6170 7020 7468 6174 2063 616e   an app that can
+00001330: 2063 6861 6e67 6520 616e 6420 7468 6520   change and the 
+00001340: 6675 6e63 7469 6f6e 7320 7468 6174 2063  functions that c
+00001350: 6861 6e67 6520 7468 656d 2e0a 0a48 6572  hange them...Her
+00001360: 6520 7468 6520 7374 6174 6520 6973 2063  e the state is c
+00001370: 6f6d 7072 6973 6564 206f 6620 6120 6070  omprised of a `p
+00001380: 726f 6d70 7460 2061 6e64 2060 696d 6167  rompt` and `imag
+00001390: 655f 7572 6c60 2e20 5468 6572 6520 6172  e_url`. There ar
+000013a0: 6520 616c 736f 2074 6865 2062 6f6f 6c65  e also the boole
+000013b0: 616e 7320 6070 726f 6365 7373 696e 6760  ans `processing`
+000013c0: 2061 6e64 2060 636f 6d70 6c65 7465 6020   and `complete` 
+000013d0: 746f 2069 6e64 6963 6174 6520 7768 656e  to indicate when
+000013e0: 2074 6f20 7368 6f77 2074 6865 2063 6972   to show the cir
+000013f0: 6375 6c61 7220 7072 6f67 7265 7373 2061  cular progress a
+00001400: 6e64 2069 6d61 6765 2e0a 0a23 2323 202a  nd image...### *
+00001410: 2a45 7665 6e74 2048 616e 646c 6572 732a  *Event Handlers*
+00001420: 2a0a 0a60 6060 7079 7468 6f6e 0a64 6566  *..```python.def
+00001430: 2067 6574 5f69 6d61 6765 2873 656c 6629   get_image(self)
+00001440: 3a0a 2020 2020 2222 2247 6574 2074 6865  :.    """Get the
+00001450: 2069 6d61 6765 2066 726f 6d20 7468 6520   image from the 
+00001460: 7072 6f6d 7074 2e22 2222 0a20 2020 2069  prompt.""".    i
+00001470: 6620 7365 6c66 2e70 726f 6d70 7420 3d3d  f self.prompt ==
+00001480: 2022 223a 0a20 2020 2020 2020 2072 6574   "":.        ret
+00001490: 7572 6e20 7278 2e77 696e 646f 775f 616c  urn rx.window_al
+000014a0: 6572 7428 2250 726f 6d70 7420 456d 7074  ert("Prompt Empt
+000014b0: 7922 290a 0a20 2020 2073 656c 662e 7072  y")..    self.pr
+000014c0: 6f63 6573 7369 6e67 2c20 7365 6c66 2e63  ocessing, self.c
+000014d0: 6f6d 706c 6574 6520 3d20 5472 7565 2c20  omplete = True, 
+000014e0: 4661 6c73 650a 2020 2020 7969 656c 640a  False.    yield.
+000014f0: 2020 2020 7265 7370 6f6e 7365 203d 206f      response = o
+00001500: 7065 6e61 692e 496d 6167 652e 6372 6561  penai.Image.crea
+00001510: 7465 2870 726f 6d70 743d 7365 6c66 2e70  te(prompt=self.p
+00001520: 726f 6d70 742c 206e 3d31 2c20 7369 7a65  rompt, n=1, size
+00001530: 3d22 3130 3234 7831 3032 3422 290a 2020  ="1024x1024").  
+00001540: 2020 7365 6c66 2e69 6d61 6765 5f75 726c    self.image_url
+00001550: 203d 2072 6573 706f 6e73 655b 2264 6174   = response["dat
+00001560: 6122 5d5b 305d 5b22 7572 6c22 5d0a 2020  a"][0]["url"].  
+00001570: 2020 7365 6c66 2e70 726f 6365 7373 696e    self.processin
+00001580: 672c 2073 656c 662e 636f 6d70 6c65 7465  g, self.complete
+00001590: 203d 2046 616c 7365 2c20 5472 7565 0a60   = False, True.`
+000015a0: 6060 0a0a 5769 7468 696e 2074 6865 2073  ``..Within the s
+000015b0: 7461 7465 2c20 7765 2064 6566 696e 6520  tate, we define 
+000015c0: 6675 6e63 7469 6f6e 7320 6361 6c6c 6564  functions called
+000015d0: 2065 7665 6e74 2068 616e 646c 6572 7320   event handlers 
+000015e0: 7468 6174 2063 6861 6e67 6520 7468 6520  that change the 
+000015f0: 7374 6174 6520 7661 7273 2e20 4576 656e  state vars. Even
+00001600: 7420 6861 6e64 6c65 7273 2061 7265 2074  t handlers are t
+00001610: 6865 2077 6179 2074 6861 7420 7765 2063  he way that we c
+00001620: 616e 206d 6f64 6966 7920 7468 6520 7374  an modify the st
+00001630: 6174 6520 696e 2052 6566 6c65 782e 2054  ate in Reflex. T
+00001640: 6865 7920 6361 6e20 6265 2063 616c 6c65  hey can be calle
+00001650: 6420 696e 2072 6573 706f 6e73 6520 746f  d in response to
+00001660: 2075 7365 7220 6163 7469 6f6e 732c 2073   user actions, s
+00001670: 7563 6820 6173 2063 6c69 636b 696e 6720  uch as clicking 
+00001680: 6120 6275 7474 6f6e 206f 7220 7479 7069  a button or typi
+00001690: 6e67 2069 6e20 6120 7465 7874 2062 6f78  ng in a text box
+000016a0: 2e20 5468 6573 6520 6163 7469 6f6e 7320  . These actions 
+000016b0: 6172 6520 6361 6c6c 6564 2065 7665 6e74  are called event
+000016c0: 732e 0a0a 4f75 7220 4441 4c4c c2b7 452e  s...Our DALL..E.
+000016d0: 2061 7070 2068 6173 2061 6e20 6576 656e   app has an even
+000016e0: 7420 6861 6e64 6c65 722c 2060 6765 745f  t handler, `get_
+000016f0: 696d 6167 6560 2074 6f20 7768 6963 6820  image` to which 
+00001700: 6765 7420 7468 6973 2069 6d61 6765 2066  get this image f
+00001710: 726f 6d20 7468 6520 4f70 656e 4149 2041  rom the OpenAI A
+00001720: 5049 2e20 5573 696e 6720 6079 6965 6c64  PI. Using `yield
+00001730: 6020 696e 2074 6865 206d 6964 646c 6520  ` in the middle 
+00001740: 6f66 2061 6e20 6576 656e 7420 6861 6e64  of an event hand
+00001750: 6c65 7220 7769 6c6c 2063 6175 7365 2074  ler will cause t
+00001760: 6865 2055 4920 746f 2075 7064 6174 652e  he UI to update.
+00001770: 204f 7468 6572 7769 7365 2074 6865 2055   Otherwise the U
+00001780: 4920 7769 6c6c 2075 7064 6174 6520 6174  I will update at
+00001790: 2074 6865 2065 6e64 206f 6620 7468 6520   the end of the 
+000017a0: 6576 656e 7420 6861 6e64 6c65 722e 0a0a  event handler...
+000017b0: 2323 2320 2a2a 526f 7574 696e 672a 2a0a  ### **Routing**.
+000017c0: 0a46 696e 616c 6c79 2c20 7765 2064 6566  .Finally, we def
+000017d0: 696e 6520 6f75 7220 6170 7020 616e 6420  ine our app and 
+000017e0: 7061 7373 2069 7420 6f75 7220 7374 6174  pass it our stat
+000017f0: 652e 0a0a 6060 6070 7974 686f 6e0a 6170  e...```python.ap
+00001800: 7020 3d20 7278 2e41 7070 2873 7461 7465  p = rx.App(state
+00001810: 3d53 7461 7465 290a 6060 600a 0a57 6520  =State).```..We 
+00001820: 6164 6420 6120 726f 7574 6520 6672 6f6d  add a route from
+00001830: 2074 6865 2072 6f6f 7420 6f66 2074 6865   the root of the
+00001840: 2061 7070 2074 6f20 7468 6520 696e 6465   app to the inde
+00001850: 7820 636f 6d70 6f6e 656e 742e 2057 6520  x component. We 
+00001860: 616c 736f 2061 6464 2061 2074 6974 6c65  also add a title
+00001870: 2074 6861 7420 7769 6c6c 2073 686f 7720   that will show 
+00001880: 7570 2069 6e20 7468 6520 7061 6765 2070  up in the page p
+00001890: 7265 7669 6577 2f62 726f 7773 6572 2074  review/browser t
+000018a0: 6162 2e0a 0a60 6060 7079 7468 6f6e 0a61  ab...```python.a
+000018b0: 7070 2e61 6464 5f70 6167 6528 696e 6465  pp.add_page(inde
+000018c0: 782c 2074 6974 6c65 3d22 4441 4c4c 2d45  x, title="DALL-E
+000018d0: 2229 0a61 7070 2e63 6f6d 7069 6c65 2829  ").app.compile()
+000018e0: 0a60 6060 0a0a 596f 7520 6361 6e20 6372  .```..You can cr
+000018f0: 6561 7465 2061 206d 756c 7469 2d70 6167  eate a multi-pag
+00001900: 6520 6170 7020 6279 2061 6464 696e 6720  e app by adding 
+00001910: 6d6f 7265 2072 6f75 7465 732e 0a0a 2323  more routes...##
+00001920: 2053 7461 7475 730a 0a52 6566 6c65 7820   Status..Reflex 
+00001930: 6c61 756e 6368 6564 2069 6e20 4465 6365  launched in Dece
+00001940: 6d62 6572 2032 3032 3220 7769 7468 2074  mber 2022 with t
+00001950: 6865 206e 616d 6520 5079 6e65 636f 6e65  he name Pynecone
+00001960: 2e0a 0a41 7320 6f66 204a 756e 6520 3230  ...As of June 20
+00001970: 3233 2c20 7765 2061 7265 2069 6e20 7468  23, we are in th
+00001980: 6520 2a2a 5075 626c 6963 2042 6574 612a  e **Public Beta*
+00001990: 2a20 7374 6167 652e 0a0a 2d20 2020 3a77  * stage...-   :w
+000019a0: 6869 7465 5f63 6865 636b 5f6d 6172 6b3a  hite_check_mark:
+000019b0: 202a 2a50 7562 6c69 6320 416c 7068 612a   **Public Alpha*
+000019c0: 2a3a 2041 6e79 6f6e 6520 6361 6e20 696e  *: Anyone can in
+000019d0: 7374 616c 6c20 616e 6420 7573 6520 5265  stall and use Re
+000019e0: 666c 6578 2e20 5468 6572 6520 6d61 7920  flex. There may 
+000019f0: 6265 2069 7373 7565 732c 2062 7574 2077  be issues, but w
+00001a00: 6520 6172 6520 776f 726b 696e 6720 746f  e are working to
+00001a10: 2072 6573 6f6c 7665 2074 6865 6d20 6163   resolve them ac
+00001a20: 7469 7665 6c79 2e0a 2d20 2020 3a6c 6172  tively..-   :lar
+00001a30: 6765 5f6f 7261 6e67 655f 6469 616d 6f6e  ge_orange_diamon
+00001a40: 643a 202a 2a50 7562 6c69 6320 4265 7461  d: **Public Beta
+00001a50: 2a2a 3a20 5374 6162 6c65 2065 6e6f 7567  **: Stable enoug
+00001a60: 6820 666f 7220 6e6f 6e2d 656e 7465 7270  h for non-enterp
+00001a70: 7269 7365 2075 7365 2d63 6173 6573 2e0a  rise use-cases..
+00001a80: 2d20 2020 2a2a 5075 626c 6963 2048 6f73  -   **Public Hos
+00001a90: 7469 6e67 2042 6574 612a 2a3a 205f 4f70  ting Beta**: _Op
+00001aa0: 7469 6f6e 616c 6c79 5f2c 2064 6570 6c6f  tionally_, deplo
+00001ab0: 7920 616e 6420 686f 7374 2079 6f75 7220  y and host your 
+00001ac0: 6170 7073 206f 6e20 5265 666c 6578 210a  apps on Reflex!.
+00001ad0: 2d20 2020 2a2a 5075 626c 6963 2a2a 3a20  -   **Public**: 
+00001ae0: 5265 666c 6578 2069 7320 7072 6f64 7563  Reflex is produc
+00001af0: 7469 6f6e 2072 6561 6479 2e0a 0a52 6566  tion ready...Ref
+00001b00: 6c65 7820 6861 7320 6e65 7720 7265 6c65  lex has new rele
+00001b10: 6173 6573 2061 6e64 2066 6561 7475 7265  ases and feature
+00001b20: 7320 636f 6d69 6e67 2065 7665 7279 2077  s coming every w
+00001b30: 6565 6b21 204d 616b 6520 7375 7265 2074  eek! Make sure t
+00001b40: 6f20 3a73 7461 723a 2073 7461 7220 616e  o :star: star an
+00001b50: 6420 3a65 7965 733a 2077 6174 6368 2074  d :eyes: watch t
+00001b60: 6869 7320 7265 706f 7369 746f 7279 2074  his repository t
+00001b70: 6f20 7374 6179 2075 7020 746f 2064 6174  o stay up to dat
+00001b80: 652e 0a0a 2323 2043 6f6e 7472 6962 7574  e...## Contribut
+00001b90: 696e 670a 0a57 6520 7765 6c63 6f6d 6520  ing..We welcome 
+00001ba0: 636f 6e74 7269 6275 7469 6f6e 7320 6f66  contributions of
+00001bb0: 2061 6e79 2073 697a 6521 2042 656c 6f77   any size! Below
+00001bc0: 2061 7265 2073 6f6d 6520 676f 6f64 2077   are some good w
+00001bd0: 6179 7320 746f 2067 6574 2073 7461 7274  ays to get start
+00001be0: 6564 2069 6e20 7468 6520 5265 666c 6578  ed in the Reflex
+00001bf0: 2063 6f6d 6d75 6e69 7479 2e0a 0a2d 2020   community...-  
+00001c00: 202a 2a4a 6f69 6e20 4f75 7220 4469 7363   **Join Our Disc
+00001c10: 6f72 642a 2a3a 204f 7572 205b 4469 7363  ord**: Our [Disc
+00001c20: 6f72 645d 2868 7474 7073 3a2f 2f64 6973  ord](https://dis
+00001c30: 636f 7264 2e67 672f 5435 5753 6243 3259  cord.gg/T5WSbC2Y
+00001c40: 7451 2920 6973 2074 6865 2062 6573 7420  tQ) is the best 
+00001c50: 706c 6163 6520 746f 2067 6574 2068 656c  place to get hel
+00001c60: 7020 6f6e 2079 6f75 7220 5265 666c 6578  p on your Reflex
+00001c70: 2070 726f 6a65 6374 2061 6e64 2074 6f20   project and to 
+00001c80: 6469 7363 7573 7320 686f 7720 796f 7520  discuss how you 
+00001c90: 6361 6e20 636f 6e74 7269 6275 7465 2e0a  can contribute..
+00001ca0: 2d20 2020 2a2a 4769 7448 7562 2044 6973  -   **GitHub Dis
+00001cb0: 6375 7373 696f 6e73 2a2a 3a20 4120 6772  cussions**: A gr
+00001cc0: 6561 7420 7761 7920 746f 2074 616c 6b20  eat way to talk 
+00001cd0: 6162 6f75 7420 6665 6174 7572 6573 2079  about features y
+00001ce0: 6f75 2077 616e 7420 6164 6465 6420 6f72  ou want added or
+00001cf0: 2074 6869 6e67 7320 7468 6174 2061 7265   things that are
+00001d00: 2063 6f6e 6675 7369 6e67 2f6e 6565 6420   confusing/need 
+00001d10: 636c 6172 6966 6963 6174 696f 6e2e 0a2d  clarification..-
+00001d20: 2020 202a 2a47 6974 4875 6220 4973 7375     **GitHub Issu
+00001d30: 6573 2a2a 3a20 5468 6573 6520 6172 6520  es**: These are 
+00001d40: 616e 2065 7863 656c 6c65 6e74 2077 6179  an excellent way
+00001d50: 2074 6f20 7265 706f 7274 2062 7567 732e   to report bugs.
+00001d60: 2041 6464 6974 696f 6e61 6c6c 792c 2079   Additionally, y
+00001d70: 6f75 2063 616e 2074 7279 2061 6e64 2073  ou can try and s
+00001d80: 6f6c 7665 2061 6e20 6578 6973 7469 6e67  olve an existing
+00001d90: 2069 7373 7565 2061 6e64 2073 7562 6d69   issue and submi
+00001da0: 7420 6120 5052 2e0a 0a57 6520 6172 6520  t a PR...We are 
+00001db0: 6163 7469 7665 6c79 206c 6f6f 6b69 6e67  actively looking
+00001dc0: 2066 6f72 2063 6f6e 7472 6962 7574 6f72   for contributor
+00001dd0: 732c 206e 6f20 6d61 7474 6572 2079 6f75  s, no matter you
+00001de0: 7220 736b 696c 6c20 6c65 7665 6c20 6f72  r skill level or
+00001df0: 2065 7870 6572 6965 6e63 652e 0a0a 2323   experience...##
+00001e00: 204c 6963 656e 7365 0a0a 5265 666c 6578   License..Reflex
+00001e10: 2069 7320 6f70 656e 2d73 6f75 7263 6520   is open-source 
+00001e20: 616e 6420 6c69 6365 6e73 6564 2075 6e64  and licensed und
+00001e30: 6572 2074 6865 205b 4170 6163 6865 204c  er the [Apache L
+00001e40: 6963 656e 7365 2032 2e30 5d28 4c49 4345  icense 2.0](LICE
+00001e50: 4e53 4529 2e0a                           NSE)..
```

### Comparing `reflex-0.2.0a2/pyproject.toml` & `reflex-0.2.1a1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "reflex"
-version = "0.2.0a2"
+version = "0.2.1a1"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
-homepage = "https://pynecone.io"
+homepage = "https://reflex.dev"
 repository = "https://github.com/pynecone-io/pynecone"
-documentation = "https://pynecone.io/docs/getting-started/introduction"
+documentation = "https://reflex.dev/docs/getting-started/introduction"
 keywords = [
     "web",
     "framework",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
 ]
@@ -23,15 +23,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 cloudpickle = "^2.2.1"
 fastapi = "^0.96.0"
 gunicorn = "^20.1.0"
-httpx = "^0.23.0"
+httpx = "^0.24.0"
 jinja2 = "^3.1.2"
 plotly = "^5.13.0"
 psutil = "^5.9.4"
 pydantic = "^1.10.2"
 python-multipart = "^0.0.5"
 python-socketio = "^5.7.0"
 redis = "^4.3.5"
@@ -40,14 +40,15 @@
 typer = "0.4.2"
 uvicorn = "^0.20.0"
 watchdog = "^2.3.1"
 watchfiles = "^0.19.0"
 websockets = "^10.4"
 starlette-admin = "^0.9.0"
 python-dotenv = "^0.13.0"
+importlib-metadata = {version = "^6.7.0", python = ">=3.7, <3.8"}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 pytest-mock = "^3.10.0"
 pyright = "^1.1.229"
 darglint = "^1.8.1"
 toml = "^0.10.2"
@@ -57,14 +58,16 @@
 ruff = "^0.0.244"
 pandas = [
     {version = "^1.5.3", python = ">=3.8,<4.0"},
     {version = "^1.1", python = ">=3.7, <3.8"}
 ]
 asynctest = "^0.13.0"
 pre-commit = {version = "^3.2.1", python = ">=3.8,<4.0"}
+alembic = "^1.11.1"
+selenium = "^4.10.0"
 
 [tool.poetry.scripts]
 reflex = "reflex.reflex:main"
 
 [build-system]
 requires = ["poetry-core>=1.5.1"]
 build-backend = "poetry.core.masonry.api"
@@ -79,8 +82,8 @@
 
 target-version = "py37"
 
 [tool.ruff.per-file-ignores]
 
 "__init__.py" = ["F401"]
 "tests/*.py" = ["D100", "D103", "D104"]
-"reflex/.templates/*.py" = ["D100", "D103", "D104"]
+"reflex/.templates/*.py" = ["D100", "D103", "D104"]
```

### Comparing `reflex-0.2.0a2/reflex/.templates/apps/counter/counter.py` & `reflex-0.2.1a1/reflex/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/.templates/apps/default/default.py` & `reflex-0.2.1a1/reflex/.templates/apps/default/default.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Welcome to Reflex! This file outlines the steps to create a basic app."""
 from rxconfig import config
 
 import reflex as rx
 
-docs_url = "https://pynecone.io/docs/getting-started/introduction"
+docs_url = "https://reflex.dev/docs/getting-started/introduction"
 filename = f"{config.app_name}/{config.app_name}.py"
 
 
 class State(rx.State):
     """The app state."""
 
     pass
```

### Comparing `reflex-0.2.0a2/reflex/.templates/assets/favicon.ico` & `reflex-0.2.1a1/reflex/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/.templates/jinja/web/pages/index.js.jinja2` & `reflex-0.2.1a1/reflex/.templates/jinja/web/pages/index.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/.templates/jinja/web/pages/utils.js.jinja2` & `reflex-0.2.1a1/reflex/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/.templates/web/bun.lockb` & `reflex-0.2.1a1/reflex/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/.templates/web/package.json` & `reflex-0.2.1a1/reflex/.templates/web/package.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9956896551724138%*

 * *Differences: {"'dependencies'": "{'react-debounce-input': '^3.3.0'}"}*

```diff
@@ -11,14 +11,15 @@
         "framer-motion": "^10.12.4",
         "gridjs": "^6.0.6",
         "gridjs-react": "^6.0.1",
         "json5": "^2.2.3",
         "next": "^13.3.1",
         "plotly.js": "^2.22.0",
         "react": "^18.2.0",
+        "react-debounce-input": "^3.3.0",
         "react-dom": "^18.2.0",
         "react-dropzone": "^14.2.3",
         "react-markdown": "^8.0.7",
         "react-player": "^2.12.0",
         "react-plotly.js": "^2.6.0",
         "react-syntax-highlighter": "^15.5.0",
         "rehype-katex": "^6.0.3",
```

### Comparing `reflex-0.2.0a2/reflex/.templates/web/pages/_app.js` & `reflex-0.2.1a1/reflex/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/.templates/web/styles/code/prism.js` & `reflex-0.2.1a1/reflex/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/.templates/web/utils/state.js` & `reflex-0.2.1a1/reflex/.templates/web/utils/state.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -243,15 +243,15 @@
     } else {
         eventSent = await applyEvent(event, router, socket);
     }
 
     // If no event was sent, set processing to false.
     if (!eventSent) {
         setResult({
-            ...state,
+            ...result,
             final: true,
             processing: false
         });
     }
 };
 
 /**
@@ -293,20 +293,20 @@
         setNotConnected(true)
     });
 
     // On each received message, apply the delta and set the result.
     socket.current.on("event", update => {
         update = JSON5.parse(update);
         applyDelta(state, update.delta);
-        setResult({
+        setResult(result => ({
             state: state,
-            events: update.events,
+            events: [...result.events, ...update.events],
             final: update.final,
             processing: true,
-        });
+        }));
     });
 };
 
 /**
  * Upload files to the server.
  *
  * @param state The state to apply the delta to.
```

### Comparing `reflex-0.2.0a2/reflex/__init__.py` & `reflex-0.2.1a1/reflex/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/app.py` & `reflex-0.2.1a1/reflex/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Tuple,
     Type,
     Union,
 )
 
 from fastapi import FastAPI, UploadFile
 from fastapi.middleware import cors
+from rich.progress import MofNCompleteColumn, Progress, TimeElapsedColumn
 from socketio import ASGIApp, AsyncNamespace, AsyncServer
 from starlette_admin.contrib.sqla.admin import Admin
 from starlette_admin.contrib.sqla.view import ModelView
 
 from reflex import constants
 from reflex.admin import AdminDash
 from reflex.base import Base
@@ -433,69 +434,90 @@
                 view = config.admin_dash.view_overrides.get(model, ModelView)
                 admin.add_view(view(model))
 
             admin.mount_to(self.api)
 
     def compile(self):
         """Compile the app and output it to the pages folder."""
+        # Create a progress bar.
+        progress = Progress(
+            *Progress.get_default_columns()[:-1],
+            MofNCompleteColumn(),
+            TimeElapsedColumn(),
+        )
+        task = progress.add_task("Compiling: ", total=len(self.pages))
+
         for render, kwargs in DECORATED_ROUTES:
             self.add_page(render, **kwargs)
 
         # Get the env mode.
         config = get_config()
 
         # Update models during hot reload.
-        if config.db_url is not None:
+        if config.db_url is not None and not Model.automigrate():
             Model.create_all()
 
         # Empty the .web pages directory
         compiler.purge_web_pages_dir()
 
+        # Store the compile results.
+        compile_results = []
+
+        # Compile the pages in parallel.
+        custom_components = set()
+        thread_pool = ThreadPool()
+        with progress:
+            for route, component in self.pages.items():
+                progress.advance(task)
+                component.add_style(self.style)
+                compile_results.append(
+                    thread_pool.apply_async(
+                        compiler.compile_page,
+                        args=(
+                            route,
+                            component,
+                            self.state,
+                            self.connect_error_component,
+                        ),
+                    )
+                )
+                # Add the custom components from the page to the set.
+                custom_components |= component.get_custom_components()
+        thread_pool.close()
+        thread_pool.join()
+
+        # Get the results.
+        compile_results = [result.get() for result in compile_results]
+
+        # Compile the custom components.
+        compile_results.append(compiler.compile_components(custom_components))
+
         # Compile the root document with base styles and fonts.
-        compiler.compile_document_root(self.stylesheets)
+        compile_results.append(compiler.compile_document_root(self.stylesheets))
 
         # Compile the theme.
-        compiler.compile_theme(self.style)
+        compile_results.append(compiler.compile_theme(self.style))
 
         # Compile the Tailwind config.
-        compiler.compile_tailwind(
-            dict(**config.tailwind, content=constants.TAILWIND_CONTENT)
-            if config.tailwind is not None
-            else {}
+        compile_results.append(
+            compiler.compile_tailwind(
+                dict(**config.tailwind, content=constants.TAILWIND_CONTENT)
+                if config.tailwind is not None
+                else {}
+            )
         )
 
-        # Compile the pages.
-        custom_components = set()
+        # Write the pages at the end to trigger the NextJS hot reload only once.
         thread_pool = ThreadPool()
-        compile_results = []
-        for route, component in self.pages.items():
-            component.add_style(self.style)
-            compile_results.append(
-                thread_pool.apply_async(
-                    compiler.compile_page,
-                    args=(
-                        route,
-                        component,
-                        self.state,
-                        self.connect_error_component,
-                    ),
-                )
-            )
-            # Add the custom components from the page to the set.
-            custom_components |= component.get_custom_components()
+        for output_path, code in compile_results:
+            compiler_utils.write_page(output_path, code)
+            thread_pool.apply_async(compiler_utils.write_page, args=(output_path, code))
         thread_pool.close()
         thread_pool.join()
 
-        # check the results of all the threads in case an exception was raised.
-        for r in compile_results:
-            r.get()
-
-        # Compile the custom components.
-        compiler.compile_components(custom_components)
-
 
 async def process(
     app: App, event: Event, sid: str, headers: Dict, client_ip: str
 ) -> AsyncIterator[StateUpdate]:
     """Process an event.
 
     Args:
```

### Comparing `reflex-0.2.0a2/reflex/base.py` & `reflex-0.2.1a1/reflex/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/compiler/compiler.py` & `reflex-0.2.1a1/reflex/compiler/compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Compiler for the reflex apps."""
 from __future__ import annotations
 
-from functools import wraps
-from typing import Callable, List, Set, Tuple, Type
+from typing import List, Set, Tuple, Type
 
 from reflex import constants
 from reflex.compiler import templates, utils
-from reflex.components.component import Component, CustomComponent
+from reflex.components.component import Component, ComponentStyle, CustomComponent
 from reflex.state import State
-from reflex.style import Style
 from reflex.utils import imports
 from reflex.vars import ImportVar
 
 # Imports to be included in every Reflex app.
 DEFAULT_IMPORTS: imports.ImportDict = {
     "react": {
         ImportVar(tag="Fragment"),
@@ -140,44 +138,14 @@
         The compiled Tailwind config.
     """
     return templates.TAILWIND_CONFIG.render(
         **config,
     )
 
 
-def write_output(fn: Callable[..., Tuple[str, str]]):
-    """Write the output of the function to a file.
-
-    Args:
-        fn: The function to decorate.
-
-    Returns:
-        The decorated function.
-    """
-
-    @wraps(fn)
-    def wrapper(*args, write: bool = True) -> Tuple[str, str]:
-        """Write the output of the function to a file.
-
-        Args:
-            *args: The arguments to pass to the function.
-            write: Whether to write the output to a file.
-
-        Returns:
-            The path and code of the output.
-        """
-        path, code = fn(*args)
-        if write:
-            utils.write_page(path, code)
-        return path, code
-
-    return wrapper
-
-
-@write_output
 def compile_document_root(stylesheets: List[str]) -> Tuple[str, str]:
     """Compile the document root.
 
     Args:
         stylesheets: The stylesheets to include in the document root.
 
     Returns:
@@ -190,16 +158,15 @@
     document_root = utils.create_document_root(stylesheets)
 
     # Compile the document root.
     code = _compile_document_root(document_root)
     return output_path, code
 
 
-@write_output
-def compile_theme(style: Style) -> Tuple[str, str]:
+def compile_theme(style: ComponentStyle) -> Tuple[str, str]:
     """Compile the theme.
 
     Args:
         style: The style to compile.
 
     Returns:
         The path and code of the compiled theme.
@@ -210,15 +177,14 @@
     theme = utils.create_theme(style)
 
     # Compile the theme.
     code = _compile_theme(theme)
     return output_path, code
 
 
-@write_output
 def compile_page(
     path: str,
     component: Component,
     state: Type[State],
     connect_error_component: Component,
 ) -> Tuple[str, str]:
     """Compile a single page.
@@ -236,15 +202,14 @@
     output_path = utils.get_page_path(path)
 
     # Add the style to the component.
     code = _compile_page(component, state, connect_error_component)
     return output_path, code
 
 
-@write_output
 def compile_components(components: Set[CustomComponent]):
     """Compile the custom components.
 
     Args:
         components: The custom components to compile.
 
     Returns:
@@ -254,15 +219,14 @@
     output_path = utils.get_components_path()
 
     # Compile the components.
     code = _compile_components(components)
     return output_path, code
 
 
-@write_output
 def compile_tailwind(
     config: dict,
 ):
     """Compile the Tailwind config.
 
     Args:
         config: The Tailwind config.
```

### Comparing `reflex-0.2.0a2/reflex/compiler/templates.py` & `reflex-0.2.1a1/reflex/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/compiler/utils.py` & `reflex-0.2.1a1/reflex/compiler/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Image,
     Main,
     Meta,
     RawLink,
     Script,
     Title,
 )
-from reflex.components.component import Component, CustomComponent
+from reflex.components.component import Component, ComponentStyle, CustomComponent
 from reflex.event import get_hydrate_event
 from reflex.state import State
 from reflex.style import Style
 from reflex.utils import format, imports, path_ops
 from reflex.vars import ImportVar
 
 # To re-export this function.
@@ -184,15 +184,15 @@
             ColorModeScript.create(),
             Main.create(),
             Script.create(),
         ),
     )
 
 
-def create_theme(style: Style) -> Dict:
+def create_theme(style: ComponentStyle) -> Dict:
     """Create the base style for the app.
 
     Args:
         style: The style dict for the app.
 
     Returns:
         The base style for the app.
```

### Comparing `reflex-0.2.0a2/reflex/components/__init__.py` & `reflex-0.2.1a1/reflex/components/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,28 +90,31 @@
 button = Button.create
 button_group = ButtonGroup.create
 checkbox = Checkbox.create
 checkbox_group = CheckboxGroup.create
 copy_to_clipboard = CopyToClipboard.create
 date_picker = DatePicker.create
 date_time_picker = DateTimePicker.create
+debounce_input = DebounceInput.create
 editable = Editable.create
 editable_input = EditableInput.create
 editable_preview = EditablePreview.create
 editable_textarea = EditableTextarea.create
 form = Form.create
 form_control = FormControl.create
 form_error_message = FormErrorMessage.create
 form_helper_text = FormHelperText.create
 form_label = FormLabel.create
 icon_button = IconButton.create
 input = Input.create
 input_group = InputGroup.create
 input_left_addon = InputLeftAddon.create
 input_right_addon = InputRightAddon.create
+input_left_element = InputLeftElement.create
+input_right_element = InputRightElement.create
 multi_select = MultiSelect
 multi_select_option = MultiSelectOption
 number_decrement_stepper = NumberDecrementStepper.create
 number_increment_stepper = NumberIncrementStepper.create
 number_input = NumberInput.create
 number_input_field = NumberInputField.create
 number_input_stepper = NumberInputStepper.create
```

### Comparing `reflex-0.2.0a2/reflex/components/base/bare.py` & `reflex-0.2.1a1/reflex/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/base/document.py` & `reflex-0.2.1a1/reflex/components/base/document.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/base/link.py` & `reflex-0.2.1a1/reflex/components/base/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/base/meta.py` & `reflex-0.2.1a1/reflex/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/component.py` & `reflex-0.2.1a1/reflex/components/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -549,15 +549,16 @@
 
     def get_ref(self) -> Optional[str]:
         """Get the name of the ref for the component.
 
         Returns:
             The ref name.
         """
-        if self.id is None:
+        # do not create a ref if the id is dynamic or unspecified
+        if self.id is None or isinstance(self.id, BaseVar):
             return None
         return format.format_ref(self.id)
 
     def get_refs(self) -> Set[str]:
         """Get the refs for the children of the component.
 
         Returns:
```

### Comparing `reflex-0.2.0a2/reflex/components/datadisplay/code.py` & `reflex-0.2.1a1/reflex/components/datadisplay/code.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,16 +40,14 @@
 
     # A custom style for the code block.
     custom_style: Var[Dict[str, str]]
 
     # Props passed down to the code tag.
     code_tag_props: Var[Dict[str, str]]
 
-    is_default = True
-
     def _get_imports(self) -> imports.ImportDict:
         merged_imports = super()._get_imports()
         if self.theme is not None:
             merged_imports = imports.merge_imports(
                 merged_imports, {PRISM_STYLES_PATH: {ImportVar(tag=self.theme.name)}}
             )
         return merged_imports
```

### Comparing `reflex-0.2.0a2/reflex/components/datadisplay/datatable.py` & `reflex-0.2.1a1/reflex/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/datadisplay/divider.py` & `reflex-0.2.1a1/reflex/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/datadisplay/list.py` & `reflex-0.2.1a1/reflex/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/datadisplay/stat.py` & `reflex-0.2.1a1/reflex/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/datadisplay/table.py` & `reflex-0.2.1a1/reflex/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/datadisplay/tag.py` & `reflex-0.2.1a1/reflex/components/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/disclosure/accordion.py` & `reflex-0.2.1a1/reflex/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/disclosure/tabs.py` & `reflex-0.2.1a1/reflex/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/disclosure/transition.py` & `reflex-0.2.1a1/reflex/components/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/feedback/alert.py` & `reflex-0.2.1a1/reflex/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/feedback/circularprogress.py` & `reflex-0.2.1a1/reflex/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/feedback/progress.py` & `reflex-0.2.1a1/reflex/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/feedback/skeleton.py` & `reflex-0.2.1a1/reflex/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/feedback/spinner.py` & `reflex-0.2.1a1/reflex/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/forms/__init__.py` & `reflex-0.2.1a1/reflex/components/forms/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,19 +7,27 @@
     ColorModeIcon,
     ColorModeSwitch,
     color_mode_cond,
 )
 from .copytoclipboard import CopyToClipboard
 from .date_picker import DatePicker
 from .date_time_picker import DateTimePicker
+from .debounce import DebounceInput
 from .editable import Editable, EditableInput, EditablePreview, EditableTextarea
 from .email import Email
 from .form import Form, FormControl, FormErrorMessage, FormHelperText, FormLabel
 from .iconbutton import IconButton
-from .input import Input, InputGroup, InputLeftAddon, InputRightAddon
+from .input import (
+    Input,
+    InputGroup,
+    InputLeftAddon,
+    InputLeftElement,
+    InputRightAddon,
+    InputRightElement,
+)
 from .multiselect import Option as MultiSelectOption
 from .multiselect import Select as MultiSelect
 from .numberinput import (
     NumberDecrementStepper,
     NumberIncrementStepper,
     NumberInput,
     NumberInputField,
```

### Comparing `reflex-0.2.0a2/reflex/components/forms/button.py` & `reflex-0.2.1a1/reflex/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/forms/checkbox.py` & `reflex-0.2.1a1/reflex/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/forms/colormodeswitch.py` & `reflex-0.2.1a1/reflex/components/forms/colormodeswitch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/forms/copytoclipboard.py` & `reflex-0.2.1a1/reflex/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/forms/editable.py` & `reflex-0.2.1a1/reflex/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/forms/form.py` & `reflex-0.2.1a1/reflex/components/forms/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/forms/iconbutton.py` & `reflex-0.2.1a1/reflex/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/forms/input.py` & `reflex-0.2.1a1/reflex/components/forms/input.py`

 * *Files 12% similar despite different names*

```diff
@@ -82,7 +82,19 @@
     tag = "InputLeftAddon"
 
 
 class InputRightAddon(ChakraComponent):
     """The InputRightAddon component is a component that is used to add an addon to the right of an input."""
 
     tag = "InputRightAddon"
+
+
+class InputLeftElement(ChakraComponent):
+    """The InputLeftElement component is a component that is used to add an element to the left of an input."""
+
+    tag = "InputLeftElement"
+
+
+class InputRightElement(ChakraComponent):
+    """The InputRightElement component is a component that is used to add an element to the right of an input."""
+
+    tag = "InputRightElement"
```

### Comparing `reflex-0.2.0a2/reflex/components/forms/multiselect.py` & `reflex-0.2.1a1/reflex/components/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/forms/numberinput.py` & `reflex-0.2.1a1/reflex/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/forms/pininput.py` & `reflex-0.2.1a1/reflex/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/forms/radio.py` & `reflex-0.2.1a1/reflex/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/forms/rangeslider.py` & `reflex-0.2.1a1/reflex/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/forms/select.py` & `reflex-0.2.1a1/reflex/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/forms/slider.py` & `reflex-0.2.1a1/reflex/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/forms/switch.py` & `reflex-0.2.1a1/reflex/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/forms/textarea.py` & `reflex-0.2.1a1/reflex/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/forms/upload.py` & `reflex-0.2.1a1/reflex/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/graphing/plotly.py` & `reflex-0.2.1a1/reflex/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/graphing/victory.py` & `reflex-0.2.1a1/reflex/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/layout/__init__.py` & `reflex-0.2.1a1/reflex/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/layout/box.py` & `reflex-0.2.1a1/reflex/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/layout/card.py` & `reflex-0.2.1a1/reflex/components/layout/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/layout/cond.py` & `reflex-0.2.1a1/reflex/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/layout/flex.py` & `reflex-0.2.1a1/reflex/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/layout/foreach.py` & `reflex-0.2.1a1/reflex/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/layout/grid.py` & `reflex-0.2.1a1/reflex/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/layout/html.py` & `reflex-0.2.1a1/reflex/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/layout/responsive.py` & `reflex-0.2.1a1/reflex/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/layout/stack.py` & `reflex-0.2.1a1/reflex/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/layout/wrap.py` & `reflex-0.2.1a1/reflex/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/libs/react_player.py` & `reflex-0.2.1a1/reflex/components/libs/react_player.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/media/avatar.py` & `reflex-0.2.1a1/reflex/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/media/icon.py` & `reflex-0.2.1a1/reflex/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/media/image.py` & `reflex-0.2.1a1/reflex/components/media/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/navigation/breadcrumb.py` & `reflex-0.2.1a1/reflex/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/navigation/link.py` & `reflex-0.2.1a1/reflex/components/navigation/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/navigation/linkoverlay.py` & `reflex-0.2.1a1/reflex/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/navigation/stepper.py` & `reflex-0.2.1a1/reflex/components/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/overlay/__init__.py` & `reflex-0.2.1a1/reflex/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/overlay/alertdialog.py` & `reflex-0.2.1a1/reflex/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/overlay/banner.py` & `reflex-0.2.1a1/reflex/components/overlay/banner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/overlay/drawer.py` & `reflex-0.2.1a1/reflex/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/overlay/menu.py` & `reflex-0.2.1a1/reflex/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/overlay/modal.py` & `reflex-0.2.1a1/reflex/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/overlay/popover.py` & `reflex-0.2.1a1/reflex/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/overlay/tooltip.py` & `reflex-0.2.1a1/reflex/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/tags/iter_tag.py` & `reflex-0.2.1a1/reflex/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/tags/tag.py` & `reflex-0.2.1a1/reflex/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/tags/tagless.py` & `reflex-0.2.1a1/reflex/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/typography/highlight.py` & `reflex-0.2.1a1/reflex/components/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/components/typography/markdown.py` & `reflex-0.2.1a1/reflex/components/typography/markdown.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,23 +59,23 @@
 
     def _render(self):
         return (
             super()
             ._render()
             .add_props(
                 components={
-                    "h1": "{({node, ...props}) => <Heading size='2xl' {...props} />}",
-                    "h2": "{({node, ...props}) => <Heading size='xl' {...props} />}",
-                    "h3": "{({node, ...props}) => <Heading size='lg' {...props} />}",
-                    "h4": "{({node, ...props}) => <Heading size='sm' {...props} />}",
-                    "h5": "{({node, ...props}) => <Heading size='xs' {...props} />}",
+                    "h1": "{({node, ...props}) => <Heading size='2xl' paddingY='0.5em' {...props} />}",
+                    "h2": "{({node, ...props}) => <Heading size='xl' paddingY='0.5em' {...props} />}",
+                    "h3": "{({node, ...props}) => <Heading size='lg' paddingY='0.5em' {...props} />}",
+                    "h4": "{({node, ...props}) => <Heading size='sm' paddingY='0.5em' {...props} />}",
+                    "h5": "{({node, ...props}) => <Heading size='xs' paddingY='0.5em' {...props} />}",
                     "ul": "{UnorderedList}",
                     "ol": "{OrderedList}",
                     "li": "{ListItem}",
-                    "p": "{Text}",
+                    "p": "{({node, ...props}) => <Text paddingY='0.5em' {...props} />}",
                     "a": "{Link}",
                     "code": """{({node, inline, className, children, ...props}) =>
                     {
         const match = (className || '').match(/language-(?<lang>.*)/);
         return !inline ? (
           <Prism
             children={String(children).replace(/\n$/, '')}
```

### Comparing `reflex-0.2.0a2/reflex/config.py` & `reflex-0.2.1a1/reflex/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,17 @@
 
     # Tailwind config.
     tailwind: Optional[Dict[str, Any]] = None
 
     # Timeout when launching the gunicorn server.
     timeout: int = constants.TIMEOUT
 
+    # Whether to enable or disable nextJS gzip compression.
+    next_compression: bool = True
+
     def __init__(self, *args, **kwargs):
         """Initialize the config values.
 
         If db_url is not provided gets it from db_config.
 
         Args:
             *args: The args to pass to the Pydantic init method.
```

### Comparing `reflex-0.2.0a2/reflex/constants.py` & `reflex-0.2.1a1/reflex/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 
 import os
 import re
 from enum import Enum
 from types import SimpleNamespace
 from typing import Any, Type
 
-import pkg_resources
+# importlib is only available for Python 3.8+ so we need the backport for Python 3.7
+try:
+    from importlib import metadata
+except ImportError:
+    import importlib_metadata as metadata  # pyright: ignore[reportMissingImports]
 
 
 def get_value(key: str, default: Any = None, type_: Type = str) -> Type:
     """Get the value for the constant.
     Obtain os env value and cast non-string types into
     their original types.
 
@@ -34,15 +38,15 @@
         return value if value != "None" else None  # noqa B012
 
 
 # App names and versions.
 # The name of the Reflex package.
 MODULE_NAME = "reflex"
 # The current version of Reflex.
-VERSION = pkg_resources.get_distribution(MODULE_NAME).version
+VERSION = metadata.version(MODULE_NAME)
 # Minimum version of Node.js required to run Reflex.
 MIN_NODE_VERSION = "16.8.0"
 
 # Valid bun versions.
 MIN_BUN_VERSION = "0.5.9"
 MAX_BUN_VERSION = "0.6.9"
 
@@ -77,14 +81,16 @@
 WEB_UTILS_DIR = os.path.join(WEB_DIR, UTILS_DIR)
 # The directory where the assets are located.
 WEB_ASSETS_DIR = os.path.join(WEB_DIR, "public")
 # The Tailwind config.
 TAILWIND_CONFIG = os.path.join(WEB_DIR, "tailwind.config.js")
 # Default Tailwind content paths
 TAILWIND_CONTENT = ["./pages/**/*.{js,ts,jsx,tsx}"]
+# The NextJS config file
+NEXT_CONFIG_FILE = "next.config.js"
 # The sitemap config file.
 SITEMAP_CONFIG_FILE = os.path.join(WEB_DIR, "next-sitemap.config.js")
 # The node modules directory.
 NODE_MODULES = "node_modules"
 # The package lock file.
 PACKAGE_LOCK = "package-lock.json"
 # The reflex json file.
@@ -180,15 +186,15 @@
 # The name of the reflex config module.
 CONFIG_MODULE = "rxconfig"
 # The python config file.
 CONFIG_FILE = f"{CONFIG_MODULE}{PY_EXT}"
 # The previous config file.
 OLD_CONFIG_FILE = f"pcconfig{PY_EXT}"
 # The deployment URL.
-PRODUCTION_BACKEND_URL = "https://{username}-{app_name}.api.reflex.app"
+PRODUCTION_BACKEND_URL = "https://{username}-{app_name}.api.pynecone.app"
 # Token expiration time in seconds.
 TOKEN_EXPIRATION = 60 * 60
 
 
 # Env modes
 class Env(str, Enum):
     """The environment modes."""
@@ -345,7 +351,10 @@
 USE_COLOR_MODE = "useColorMode"
 COLOR_MODE = "colorMode"
 TOGGLE_COLOR_MODE = "toggleColorMode"
 
 # Server socket configuration variables
 CORS_ALLOWED_ORIGINS = get_value("CORS_ALLOWED_ORIGINS", ["*"], list)
 POLLING_MAX_HTTP_BUFFER_SIZE = 1000 * 1000
+
+# Alembic migrations
+ALEMBIC_CONFIG = os.environ.get("ALEMBIC_CONFIG", "alembic.ini")
```

### Comparing `reflex-0.2.0a2/reflex/el/constants/html.py` & `reflex-0.2.1a1/reflex/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/el/constants/react.py` & `reflex-0.2.1a1/reflex/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/el/constants/reflex.py` & `reflex-0.2.1a1/reflex/el/constants/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/el/element.py` & `reflex-0.2.1a1/reflex/el/element.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/el/elements/__init__.py` & `reflex-0.2.1a1/reflex/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/el/precompile.py` & `reflex-0.2.1a1/reflex/el/precompile.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/event.py` & `reflex-0.2.1a1/reflex/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/middleware/hydrate_middleware.py` & `reflex-0.2.1a1/reflex/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/middleware/middleware.py` & `reflex-0.2.1a1/reflex/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/reflex.py` & `reflex-0.2.1a1/reflex/reflex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Reflex CLI to create, run, and deploy apps."""
 
 import os
 import platform
+import signal
 import threading
 from pathlib import Path
 
 import httpx
 import typer
 
 from reflex import constants
@@ -62,15 +63,15 @@
     # Finish initializing the app.
     console.log(f"[bold green]Finished Initializing: {app_name}")
 
 
 @cli.command()
 def run(
     env: constants.Env = typer.Option(
-        constants.Env.DEV, help="The environment to run the app in."
+        get_config().env, help="The environment to run the app in."
     ),
     frontend: bool = typer.Option(
         False, "--frontend-only", help="Execute only frontend."
     ),
     backend: bool = typer.Option(False, "--backend-only", help="Execute only backend."),
     loglevel: constants.LogLevel = typer.Option(
         constants.LogLevel.ERROR, help="The log level to use."
@@ -159,14 +160,17 @@
     if backend:
         build.setup_backend()
         threading.Thread(
             target=backend_cmd,
             args=(app.__name__, backend_host, backend_port, loglevel),
         ).start()
 
+    # Display custom message when there is a keyboard interrupt.
+    signal.signal(signal.SIGINT, processes.catch_keyboard_interrupt)
+
 
 @cli.command()
 def deploy(dry_run: bool = typer.Option(False, help="Whether to run a dry run.")):
     """Deploy the app to the Reflex hosting service."""
     # Get the app config.
     config = get_config()
     config.api_url = prerequisites.get_production_backend_url()
@@ -174,16 +178,15 @@
     # Check if the deploy url is set.
     if config.rxdeploy_url is None:
         typer.echo("This feature is coming soon!")
         return
 
     # Compile the app in production mode.
     typer.echo("Compiling production app")
-    app = prerequisites.get_app().app
-    build.export_app(app, zip=True, deploy_url=config.deploy_url)
+    export(for_reflex_deploy=True)
 
     # Exit early if this is a dry run.
     if dry_run:
         return
 
     # Deploy the app.
     data = {"userId": config.username, "projectId": config.app_name}
@@ -224,14 +227,17 @@
         # Get the app config and modify the api_url base on username and app_name.
         config.api_url = prerequisites.get_production_backend_url()
 
     # Compile the app in production mode and export it.
     console.rule("[bold]Compiling production app and preparing for export.")
 
     if frontend:
+        # ensure module can be imported and app.compile() is called
+        prerequisites.get_app()
+        # set up .web directory and install frontend dependencies
         build.setup_frontend(Path.cwd())
 
     build.export_app(
         backend=backend,
         frontend=frontend,
         zip=zipping,
         deploy_url=config.deploy_url,
```

### Comparing `reflex-0.2.0a2/reflex/route.py` & `reflex-0.2.1a1/reflex/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/state.py` & `reflex-0.2.1a1/reflex/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/style.py` & `reflex-0.2.1a1/reflex/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/utils/build.py` & `reflex-0.2.1a1/reflex/utils/build.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/utils/console.py` & `reflex-0.2.1a1/reflex/utils/console.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/utils/exec.py` & `reflex-0.2.1a1/reflex/utils/exec.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Everything regarding execution of the built app."""
 
 from __future__ import annotations
 
 import os
 import platform
 import subprocess
-from datetime import datetime
 from pathlib import Path
 
 from rich import print
 
 from reflex import constants
 from reflex.config import get_config
 from reflex.utils import console, prerequisites, processes
@@ -38,30 +37,20 @@
         loglevel: The log level to use.
     """
     process = new_process(
         run_command,
         cwd=constants.WEB_DIR,
     )
 
-    current_time = datetime.now()
     if process.stdout:
         for line in process.stdout:
             if "ready started server on" in line:
                 url = line.split("url: ")[-1].strip()
                 print(f"App running at: [bold green]{url}")
-            if (
-                "Fast Refresh" in line
-                or "compiling..." in line
-                and (datetime.now() - current_time).total_seconds() > 1
-            ):
-                current_time = datetime.now()
-                print(
-                    f"[yellow][Updating App][/yellow] Applying changes and refreshing. Time: {current_time}"
-                )
-            elif loglevel == constants.LogLevel.DEBUG:
+            if loglevel == constants.LogLevel.DEBUG:
                 print(line, end="")
 
 
 def run_frontend(
     root: Path,
     port: str,
     loglevel: constants.LogLevel = constants.LogLevel.ERROR,
@@ -126,16 +115,16 @@
         "--host",
         host,
         "--port",
         str(port),
         "--log-level",
         loglevel,
         "--reload",
-        "--reload-exclude",
-        f"'{constants.WEB_DIR}/*'",
+        "--reload-dir",
+        app_name.split(".")[0],
     ]
     process = subprocess.Popen(cmd)
 
     try:
         process.wait()
     except KeyboardInterrupt:
         process.terminate()
```

### Comparing `reflex-0.2.0a2/reflex/utils/format.py` & `reflex-0.2.1a1/reflex/utils/format.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/utils/imports.py` & `reflex-0.2.1a1/reflex/utils/imports.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/utils/path_ops.py` & `reflex-0.2.1a1/reflex/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/utils/prerequisites.py` & `reflex-0.2.1a1/reflex/utils/prerequisites.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,19 +203,32 @@
     )
     path_ops.cp(constants.ASSETS_TEMPLATE_DIR, constants.APP_ASSETS_DIR)
 
 
 def initialize_web_directory():
     """Initialize the web directory on reflex init."""
     console.log("Initializing the web directory.")
-    path_ops.rm(os.path.join(constants.WEB_TEMPLATE_DIR, constants.NODE_MODULES))
-    path_ops.rm(os.path.join(constants.WEB_TEMPLATE_DIR, constants.PACKAGE_LOCK))
     path_ops.cp(constants.WEB_TEMPLATE_DIR, constants.WEB_DIR)
     path_ops.mkdir(constants.WEB_ASSETS_DIR)
 
+    # update nextJS config based on rxConfig
+    next_config_file = os.path.join(constants.WEB_DIR, constants.NEXT_CONFIG_FILE)
+
+    with open(next_config_file, "r") as file:
+        lines = file.readlines()
+        for i, line in enumerate(lines):
+            if "compress:" in line:
+                new_line = line.replace(
+                    "true", "true" if get_config().next_compression else "false"
+                )
+                lines[i] = new_line
+
+    with open(next_config_file, "w") as file:
+        file.writelines(lines)
+
     # Write the current version of distributed reflex package to a REFLEX_JSON."""
     with open(constants.REFLEX_JSON, "w") as f:
         reflex_json = {"version": constants.VERSION}
         json.dump(reflex_json, f, ensure_ascii=False)
 
 
 def validate_and_install_bun(initialize=True):
```

### Comparing `reflex-0.2.0a2/reflex/utils/processes.py` & `reflex-0.2.1a1/reflex/utils/processes.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 
 import contextlib
 import os
 import signal
 import subprocess
 import sys
+from datetime import datetime
 from typing import Optional
 from urllib.parse import urlparse
 
 import psutil
 
 from reflex import constants
 from reflex.config import get_config
@@ -141,7 +142,18 @@
         "encoding": "UTF-8",
         **kwargs,
     }
     return subprocess.Popen(
         args,
         **kwargs,
     )
+
+
+def catch_keyboard_interrupt(signal, frame):
+    """Display a custom message with the current time when exiting an app.
+
+    Args:
+        signal: The keyboard interrupt signal.
+        frame: The current stack frame.
+    """
+    current_time = datetime.now().isoformat()
+    console.print(f"\nReflex app stopped at time: {current_time}")
```

### Comparing `reflex-0.2.0a2/reflex/utils/telemetry.py` & `reflex-0.2.1a1/reflex/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/utils/types.py` & `reflex-0.2.1a1/reflex/utils/types.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/utils/watch.py` & `reflex-0.2.1a1/reflex/utils/watch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a2/reflex/vars.py` & `reflex-0.2.1a1/reflex/vars.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     List,
     Optional,
     Set,
+    Tuple,
     Type,
     Union,
     _GenericAlias,  # type: ignore
     cast,
     get_type_hints,
 )
 
@@ -194,39 +195,44 @@
 
         Returns:
             The indexed var.
 
         Raises:
             TypeError: If the var is not indexable.
         """
-        # Indexing is only supported for lists, dicts, and dataframes.
+        # Indexing is only supported for strings, lists, tuples, dicts, and dataframes.
         if not (
-            types._issubclass(self.type_, Union[List, Dict])
+            types._issubclass(self.type_, Union[List, Dict, Tuple, str])
             or types.is_dataframe(self.type_)
         ):
             if self.type_ == Any:
                 raise TypeError(
-                    f"Could not index into var of type Any. (If you are trying to index into a state var, add the correct type annotation to the var.)"
+                    f"Could not index into var of type Any. (If you are trying to index into a state var, "
+                    f"add the correct type annotation to the var.)"
                 )
             raise TypeError(
                 f"Var {self.name} of type {self.type_} does not support indexing."
             )
 
         # The type of the indexed var.
         type_ = Any
 
         # Convert any vars to local vars.
         if isinstance(i, Var):
             i = BaseVar(name=i.name, type_=i.type_, state=i.state, is_local=True)
 
-        # Handle list indexing.
-        if types._issubclass(self.type_, List):
-            # List indices must be ints, slices, or vars.
-            if not isinstance(i, types.get_args(Union[int, slice, Var])):
-                raise TypeError("Index must be an integer.")
+        # Handle list/tuple/str indexing.
+        if types._issubclass(self.type_, Union[List, Tuple, str]):
+            # List/Tuple/String indices must be ints, slices, or vars.
+            if (
+                not isinstance(i, types.get_args(Union[int, slice, Var]))
+                or isinstance(i, Var)
+                and not i.type_ == int
+            ):
+                raise TypeError("Index must be an integer or an integer var.")
 
             # Handle slices first.
             if isinstance(i, slice):
                 # Get the start and stop indices.
                 start = i.start or 0
                 stop = i.stop or "undefined"
 
@@ -248,14 +254,25 @@
             return BaseVar(
                 name=f"{self.name}.at({i})",
                 type_=type_,
                 state=self.state,
             )
 
         # Dictionary / dataframe indexing.
+        # Tuples are currently not supported as indexes.
+        if (
+            (types._issubclass(self.type_, Dict) or types.is_dataframe(self.type_))
+            and not isinstance(i, types.get_args(Union[int, str, float, Var]))
+        ) or (
+            isinstance(i, Var)
+            and not types._issubclass(i.type_, types.get_args(Union[int, str, float]))
+        ):
+            raise TypeError(
+                "Index must be one of the following types: int, str, int or str Var"
+            )
         # Get the type of the indexed var.
         if isinstance(i, str):
             i = format.wrap(i, '"')
         type_ = (
             types.get_args(self.type_)[1] if types.is_generic_alias(self.type_) else Any
         )
 
@@ -865,18 +882,26 @@
         """
         d = set()
         if obj is None:
             if self.fget is not None:
                 obj = cast(FunctionType, self.fget)
             else:
                 return set()
-        if not obj.__code__.co_varnames:
+        with contextlib.suppress(AttributeError):
+            # unbox functools.partial
+            obj = cast(FunctionType, obj.func)  # type: ignore
+        with contextlib.suppress(AttributeError):
+            # unbox EventHandler
+            obj = cast(FunctionType, obj.fn)  # type: ignore
+
+        try:
+            self_name = obj.__code__.co_varnames[0]
+        except (AttributeError, IndexError):
             # cannot reference self if method takes no args
             return set()
-        self_name = obj.__code__.co_varnames[0]
         self_is_top_of_stack = False
         for instruction in dis.get_instructions(obj):
             if instruction.opname == "LOAD_FAST" and instruction.argval == self_name:
                 self_is_top_of_stack = True
                 continue
             if self_is_top_of_stack and instruction.opname == "LOAD_ATTR":
                 d.add(instruction.argval)
```

### Comparing `reflex-0.2.0a2/PKG-INFO` & `reflex-0.2.1a1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: reflex
-Version: 0.2.0a2
+Version: 0.2.1a1
 Summary: Web apps in pure Python.
-Home-page: https://pynecone.io
+Home-page: https://reflex.dev
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,15 +15,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
 Requires-Dist: fastapi (>=0.96.0,<0.97.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: importlib-metadata (>=6.7.0,<7.0.0) ; python_version >= "3.7" and python_version < "3.8"
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: plotly (>=5.13.0,<6.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: python-dotenv (>=0.13.0,<0.14.0)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
 Requires-Dist: python-socketio (>=5.7.0,<6.0.0)
@@ -32,96 +33,85 @@
 Requires-Dist: sqlmodel (>=0.0.8,<0.0.9)
 Requires-Dist: starlette-admin (>=0.9.0,<0.10.0)
 Requires-Dist: typer (==0.4.2)
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0)
 Requires-Dist: watchdog (>=2.3.1,<3.0.0)
 Requires-Dist: watchfiles (>=0.19.0,<0.20.0)
 Requires-Dist: websockets (>=10.4,<11.0)
-Project-URL: Documentation, https://pynecone.io/docs/getting-started/introduction
+Project-URL: Documentation, https://reflex.dev/docs/getting-started/introduction
 Project-URL: Repository, https://github.com/pynecone-io/pynecone
 Description-Content-Type: text/markdown
 
 ```diff
-+ ATTENTION: Over the next week we will be changing our project name from Pynecone to Reflex.
-
-The new name aligns with our goal of allowing you to build apps easily, while also being flexible and powerful enough to handle all your use cases.
-
-Major Changes:
-+ Our domain will switch from https://pynecone.io/ -> https://reflex.dev/
-+ Our pip install will switch from pip install pynecone -> pip install reflex
-+ Our Github repo will switch from https://github.com/pynecone-io/pynecone -> https://github.com/reflex-dev/reflex
-+ Our library will change from import pynecone as pc to import reflex as rx
-
-We will have a feature freeze until we migrate our code and website to the new name.
-
-Our goal is to complete the transition by June 30. Thanks for your support - please message on Discord if you have any questions or concerns!
++ Searching for Pynecone? You are in the right repo. Pynecone has been renamed to Reflex. +
 ```
 
 <div align="center">
 
-<img src="docs/images/cones.png">
+<img src="docs/images/reflex.png">
 <hr>
 
+# **Reflex** 
 **✨ Performant, customizable web apps in pure Python. Deploy in seconds.**
 
-📑 [Docs](https://pynecone.io/docs/getting-started/introduction) &nbsp; 📱 [Component Library](https://pynecone.io/docs/library) &nbsp; 🖼️ [Gallery](https://pynecone.io/docs/gallery) &nbsp; 🛸 [Deployment](https://pynecone.io/docs/hosting/deploy)
+📑 [Docs](https://reflex.dev/docs/getting-started/introduction) &nbsp; 📱 [Component Library](https://reflex.dev/docs/library) &nbsp; 🖼️ [Gallery](https://reflex.dev/docs/gallery) &nbsp; 🛸 [Deployment](https://reflex.dev/docs/hosting/deploy)
 
-[![PyPI version](https://badge.fury.io/py/pynecone.svg)](https://badge.fury.io/py/pynecone)
+[![PyPI version](https://badge.fury.io/py/reflex.svg)](https://badge.fury.io/py/reflex)
 ![tests](https://github.com/pynecone-io/pynecone/actions/workflows/build.yml/badge.svg)
-![versions](https://img.shields.io/pypi/pyversions/pynecone-io.svg)
+![versions](https://img.shields.io/pypi/pyversions/reflex.svg)
 [![Discord](https://img.shields.io/discord/1029853095527727165?color=%237289da&label=Discord)](https://discord.gg/T5WSbC2YtQ)
 
 </div>
 
 ### README in different language
 
 ---
 
-[English](README.md) | [繁體中文](/docs/zh/zh_tw/README.md)
+[English](README.md) | [简体中文](/docs/zh/zh_cn/README.md) | [繁體中文](/docs/zh/zh_tw/README.md)
 
 ---
 
 ## 📦 1. Install
 
-Pynecone requires the following to get started:
+Reflex requires the following to get started:
 
 -   Python 3.7+
 -   [Node.js 16.8.0+](https://nodejs.org/en/) (Don't worry, you won’t have to write any JavaScript!)
 
 ```
-pip install pynecone
+pip install reflex
 ```
 
 ## 🥳 2. Create your first app
 
-Installing Pynecone also installs the `pc` command line tool. Test that the install was successful by creating a new project.
+Installing `reflex` also installs the `reflex` command line tool. Test that the install was successful by creating a new project.
 
 Replace my_app_name with your project name:
 
 ```
 mkdir my_app_name
 cd my_app_name
-pc init
+reflex init
 ```
 
 When you run this command for the first time, we will download and install [bun](https://bun.sh/) automatically.
 
 This command initializes a template app in your new directory.
 
-## 🏃 3. Run
+## 🏃 3. Run your app
 
 You can run this app in development mode:
 
 ```
-pc run
+reflex run
 ```
 
 You should see your app running at http://localhost:3000.
 
-Now you can modify the source code in `my_app_name/my_app_name.py`. Pynecone has fast refreshes so you can see your changes instantly when you save your code.
+Now you can modify the source code in `my_app_name/my_app_name.py`. Reflex has fast refreshes so you can see your changes instantly when you save your code.
 
 ## 🫧 Example
 
 Let's go over an example: creating an image generation UI around DALL·E. For simplicity, we just call the OpenAI API, but you could replace this with an ML model run locally.
 
 &nbsp;
 
@@ -130,97 +120,97 @@
 </div>
 
 &nbsp;
 
 Here is the complete code to create this. This is all done in one Python file!
 
 ```python
-import pynecone as pc
+import reflex as rx
 import openai
 
 openai.api_key = "YOUR_API_KEY"
 
-class State(pc.State):
+class State(rx.State):
     """The app state."""
     prompt = ""
     image_url = ""
     processing = False
     complete = False
 
     def get_image(self):
         """Get the image from the prompt."""
         if self.prompt == "":
-            return pc.window_alert("Prompt Empty")
+            return rx.window_alert("Prompt Empty")
 
         self.processing, self.complete = True, False
         yield
         response = openai.Image.create(prompt=self.prompt, n=1, size="1024x1024")
         self.image_url = response["data"][0]["url"]
         self.processing, self.complete = False, True
         
 
 def index():
-    return pc.center(
-        pc.vstack(
-            pc.heading("DALL·E"),
-            pc.input(placeholder="Enter a prompt", on_blur=State.set_prompt),
-            pc.button(
+    return rx.center(
+        rx.vstack(
+            rx.heading("DALL·E"),
+            rx.input(placeholder="Enter a prompt", on_blur=State.set_prompt),
+            rx.button(
                 "Generate Image",
                 on_click=State.get_image,
                 is_loading=State.processing,
                 width="100%",
             ),
-            pc.cond(
+            rx.cond(
                 State.complete,
-                     pc.image(
+                     rx.image(
                          src=State.image_url,
                          height="25em",
                          width="25em",
                     )
             ),
             padding="2em",
             shadow="lg",
             border_radius="lg",
         ),
         width="100%",
         height="100vh",
     )
 
 # Add state and page to the app.
-app = pc.App(state=State)
-app.add_page(index, title="Pynecone:DALL·E")
+app = rx.App(state=State)
+app.add_page(index, title="reflex:DALL·E")
 app.compile()
 ```
 
 Let's break this down.
 
-### **UI In Pynecone**
+### **UI In Reflex**
 
 Let's start with the UI.
 
 ```python
 def index():
-    return pc.center(
+    return rx.center(
         ...
     )
 ```
 
 This `index` function defines the frontend of the app.
 
 We use different components such as `center`, `vstack`, `input`, and `button` to build the frontend. Components can be nested within each other
 to create complex layouts. And you can use keyword args to style them with the full power of CSS.
 
-Pynecone comes with [60+ built-in components](https://pynecone.io/docs/library) to help you get started. We are actively adding more components, and it's easy to [create your own components](https://pynecone.io/docs/advanced-guide/wrapping-react).
+Reflex comes with [60+ built-in components](https://reflex.dev/docs/library) to help you get started. We are actively adding more components, and it's easy to [create your own components](https://reflex.dev/docs/advanced-guide/wrapping-react).
 
 ### **State**
 
-Pynecone represents your UI as a function of your state.
+Reflex represents your UI as a function of your state.
 
 ```python
-class State(pc.State):
+class State(rx.State):
     """The app state."""
     prompt = ""
     image_url = ""
     processing = False
     complete = False
 ```
 
@@ -230,64 +220,64 @@
 
 ### **Event Handlers**
 
 ```python
 def get_image(self):
     """Get the image from the prompt."""
     if self.prompt == "":
-        return pc.window_alert("Prompt Empty")
+        return rx.window_alert("Prompt Empty")
 
     self.processing, self.complete = True, False
     yield
     response = openai.Image.create(prompt=self.prompt, n=1, size="1024x1024")
     self.image_url = response["data"][0]["url"]
     self.processing, self.complete = False, True
 ```
 
-Within the state, we define functions called event handlers that change the state vars. Event handlers are the way that we can modify the state in Pynecone. They can be called in response to user actions, such as clicking a button or typing in a text box. These actions are called events.
+Within the state, we define functions called event handlers that change the state vars. Event handlers are the way that we can modify the state in Reflex. They can be called in response to user actions, such as clicking a button or typing in a text box. These actions are called events.
 
 Our DALL·E. app has an event handler, `get_image` to which get this image from the OpenAI API. Using `yield` in the middle of an event handler will cause the UI to update. Otherwise the UI will update at the end of the event handler.
 
 ### **Routing**
 
 Finally, we define our app and pass it our state.
 
 ```python
-app = pc.App(state=State)
+app = rx.App(state=State)
 ```
 
 We add a route from the root of the app to the index component. We also add a title that will show up in the page preview/browser tab.
 
 ```python
-app.add_page(index, title="Pynecone:DALL-E")
+app.add_page(index, title="DALL-E")
 app.compile()
 ```
 
 You can create a multi-page app by adding more routes.
 
 ## Status
 
-Pynecone launched in December 2022.
+Reflex launched in December 2022 with the name Pynecone.
 
 As of June 2023, we are in the **Public Beta** stage.
 
--   :white_check_mark: **Public Alpha**: Anyone can install and use Pynecone. There may be issues, but we are working to resolve them actively.
+-   :white_check_mark: **Public Alpha**: Anyone can install and use Reflex. There may be issues, but we are working to resolve them actively.
 -   :large_orange_diamond: **Public Beta**: Stable enough for non-enterprise use-cases.
--   **Public Hosting Beta**: _Optionally_, deploy and host your apps on Pynecone!
--   **Public**: Pynecone is production ready.
+-   **Public Hosting Beta**: _Optionally_, deploy and host your apps on Reflex!
+-   **Public**: Reflex is production ready.
 
-Pynecone has new releases and features coming every week! Make sure to :star: star and :eyes: watch this repository to stay up to date.
+Reflex has new releases and features coming every week! Make sure to :star: star and :eyes: watch this repository to stay up to date.
 
 ## Contributing
 
-We welcome contributions of any size! Below are some good ways to get started in the Pynecone community.
+We welcome contributions of any size! Below are some good ways to get started in the Reflex community.
 
--   **Join Our Discord**: Our [Discord](https://discord.gg/T5WSbC2YtQ) is the best place to get help on your Pynecone project and to discuss how you can contribute.
+-   **Join Our Discord**: Our [Discord](https://discord.gg/T5WSbC2YtQ) is the best place to get help on your Reflex project and to discuss how you can contribute.
 -   **GitHub Discussions**: A great way to talk about features you want added or things that are confusing/need clarification.
 -   **GitHub Issues**: These are an excellent way to report bugs. Additionally, you can try and solve an existing issue and submit a PR.
 
 We are actively looking for contributors, no matter your skill level or experience.
 
 ## License
 
-Pynecone is open-source and licensed under the [Apache License 2.0](LICENSE).
+Reflex is open-source and licensed under the [Apache License 2.0](LICENSE).
```

