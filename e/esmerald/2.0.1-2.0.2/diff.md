# Comparing `tmp/esmerald-2.0.1.tar.gz` & `tmp/esmerald-2.0.2.tar.gz`

## Comparing `esmerald-2.0.1.tar` & `esmerald-2.0.2.tar`

### file list

```diff
@@ -1,186 +1,188 @@
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/__init__.py
--rw-r--r--   0        0        0    39505 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/applications.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/backgound.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/concurrency.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/enums.py
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/exception_handlers.py
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/exceptions.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/injector.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/logging.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/param_functions.py
--rw-r--r--   0        0        0    21321 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/params.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/parsers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/py.typed
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/requests.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/staticfiles.py
--rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/testclient.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/types.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/typing.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/websockets.py
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/__init__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/enums.py
--rw-r--r--   0        0        0    14737 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/global_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/app_template/__init__.py-tpl
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/app_template/tests.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/app_template/directives/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/app_template/directives/operations/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/app_template/v1/__init__.py-tpl
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/app_template/v1/schemas.py-tpl
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/app_template/v1/urls.py-tpl
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/app_template/v1/views.py-tpl
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/.gitignore.e-tpl
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/main.py-tpl
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/serve.py-tpl
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/apps/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/configs/__init__.py-tpl
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/configs/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/configs/development/__init__.py-tpl
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/configs/development/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/configs/testing/__init__.py-tpl
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/configs/testing/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/conf/project_template/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/config/__init__.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/config/asyncexit.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/config/cors.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/config/csrf.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/config/jwt.py
--rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/config/openapi.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/config/session.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/config/static_files.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/config/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/contrib/__init__.py
--rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/contrib/encoding.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/contrib/auth/__init__.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/contrib/auth/constants.py
--rw-r--r--   0        0        0     8616 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/contrib/auth/hashers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/contrib/auth/common/__init__.py
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/contrib/auth/common/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/contrib/auth/saffier/__init__.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/contrib/auth/saffier/base_user.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/contrib/auth/saffier/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/__init__.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/base.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/cli.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/constants.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/env.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/exceptions.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/parsers.py
--rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/templates.py
--rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/utils.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/operations/__init__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/operations/_constants.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/operations/createapp.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/operations/createproject.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/operations/list.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/operations/run.py
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/operations/runserver.py
--rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/directives/operations/show_urls.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/terminal/__init__.py
--rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/terminal/base.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/terminal/print.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/terminal/terminal.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/urls/__init__.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/core/urls/base.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/datastructures/__init__.py
--rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/datastructures/base.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/datastructures/encoders.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/datastructures/file.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/datastructures/json.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/datastructures/redirect.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/datastructures/stream.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/datastructures/template.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/datastructures/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/interceptors/__init__.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/interceptors/interceptor.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/interceptors/types.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/__init__.py
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/_exception_handlers.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/asyncexitstack.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/authentication.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/basic.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/cors.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/csrf.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/errors.py
--rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/exceptions.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/gzip.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/https.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/sessions.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/settings_middleware.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/trustedhost.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/__init__.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/_internal.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/constants.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/datastructures.py
--rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/docs.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/enums.py
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/models.py
--rw-r--r--   0        0        0    17266 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/openapi.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/params.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/responses.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/openapi/utils.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/permissions/__init__.py
--rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/permissions/base.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/permissions/types.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/permissions/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/pluggables/__init__.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/pluggables/base.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/protocols/__init__.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/protocols/asyncdao.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/protocols/dao.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/protocols/extension.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/protocols/interceptor.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/protocols/middleware.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/protocols/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/protocols/utils/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/protocols/utils/protocols.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/responses/__init__.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/responses/base.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/responses/encoders.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/responses/json.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/responses/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/routing/__init__.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/routing/_internal.py
--rw-r--r--   0        0        0    22141 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/routing/base.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/routing/events.py
--rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/routing/gateways.py
--rw-r--r--   0        0        0    22735 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/routing/handlers.py
--rw-r--r--   0        0        0    42063 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/routing/router.py
--rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/routing/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/security/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/security/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/security/jwt/__init__.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/security/jwt/token.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/template/__init__.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/template/jinja.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/template/mako.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/transformers/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/transformers/constants.py
--rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/transformers/datastructures.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/transformers/helpers.py
--rw-r--r--   0        0        0    14628 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/transformers/model.py
--rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/transformers/signature.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/transformers/types.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/transformers/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/__init__.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/constants.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/crypto.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/dependency.py
--rw-r--r--   0        0        0     7143 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/functional.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/helpers.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/model.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/module_loading.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/sync.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/url.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/pydantic/__init__.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 esmerald-2.0.1/esmerald/utils/pydantic/schema.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 esmerald-2.0.1/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-2.0.1/LICENSE
--rw-r--r--   0        0        0    15936 2020-02-02 00:00:00.000000 esmerald-2.0.1/README.md
--rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 esmerald-2.0.1/pyproject.toml
--rw-r--r--   0        0        0    21144 2020-02-02 00:00:00.000000 esmerald-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/__init__.py
+-rw-r--r--   0        0        0    39505 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/applications.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/backgound.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/concurrency.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/enums.py
+-rw-r--r--   0        0        0     3699 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/exception_handlers.py
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/exceptions.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/injector.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/logging.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/param_functions.py
+-rw-r--r--   0        0        0    22750 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/params.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/py.typed
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/requests.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/staticfiles.py
+-rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/testclient.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/types.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/typing.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/websockets.py
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/__init__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/enums.py
+-rw-r--r--   0        0        0    14769 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/global_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/app_template/tests.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/app_template/directives/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/app_template/directives/operations/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/app_template/v1/__init__.py-tpl
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/app_template/v1/schemas.py-tpl
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/app_template/v1/urls.py-tpl
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/app_template/v1/views.py-tpl
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/.gitignore.e-tpl
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/main.py-tpl
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/serve.py-tpl
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/apps/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/configs/__init__.py-tpl
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/configs/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/configs/development/__init__.py-tpl
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/configs/development/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/configs/testing/__init__.py-tpl
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/configs/testing/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/config/__init__.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/config/asyncexit.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/config/cors.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/config/csrf.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/config/jwt.py
+-rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/config/openapi.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/config/session.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/config/static_files.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/config/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/contrib/__init__.py
+-rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/contrib/encoding.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/contrib/auth/__init__.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/contrib/auth/constants.py
+-rw-r--r--   0        0        0     8616 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/contrib/auth/hashers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/contrib/auth/common/__init__.py
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/contrib/auth/common/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/contrib/auth/saffier/__init__.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/contrib/auth/saffier/base_user.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/contrib/auth/saffier/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/__init__.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/base.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/cli.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/constants.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/env.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/exceptions.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/parsers.py
+-rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/templates.py
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/utils.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/operations/__init__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/operations/_constants.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/operations/createapp.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/operations/createproject.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/operations/list.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/operations/run.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/operations/runserver.py
+-rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/operations/show_urls.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/terminal/base.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/terminal/print.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/terminal/terminal.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/urls/__init__.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/urls/base.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/datastructures/__init__.py
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/datastructures/base.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/datastructures/encoders.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/datastructures/file.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/datastructures/json.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/datastructures/multidict.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/datastructures/redirect.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/datastructures/stream.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/datastructures/template.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/datastructures/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/interceptors/__init__.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/interceptors/interceptor.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/interceptors/types.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/__init__.py
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/_exception_handlers.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/asyncexitstack.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/authentication.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/basic.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/cors.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/csrf.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/errors.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/exceptions.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/gzip.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/https.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/sessions.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/settings_middleware.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/trustedhost.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/__init__.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/_internal.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/constants.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/datastructures.py
+-rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/docs.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/enums.py
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/models.py
+-rw-r--r--   0        0        0    17141 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/openapi.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/params.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/responses.py
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/utils.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/validation.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/permissions/__init__.py
+-rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/permissions/base.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/permissions/types.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/permissions/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/pluggables/__init__.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/pluggables/base.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/protocols/__init__.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/protocols/asyncdao.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/protocols/dao.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/protocols/extension.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/protocols/interceptor.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/protocols/middleware.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/protocols/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/protocols/utils/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/protocols/utils/protocols.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/responses/__init__.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/responses/base.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/responses/encoders.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/responses/json.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/responses/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/routing/__init__.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/routing/_internal.py
+-rw-r--r--   0        0        0    22141 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/routing/base.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/routing/events.py
+-rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/routing/gateways.py
+-rw-r--r--   0        0        0    22735 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/routing/handlers.py
+-rw-r--r--   0        0        0    42063 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/routing/router.py
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/routing/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/security/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/security/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/security/jwt/__init__.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/security/jwt/token.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/template/__init__.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/template/jinja.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/template/mako.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/transformers/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/transformers/constants.py
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/transformers/datastructures.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/transformers/helpers.py
+-rw-r--r--   0        0        0    14627 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/transformers/model.py
+-rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/transformers/signature.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/transformers/types.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/transformers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/__init__.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/constants.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/crypto.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/dependency.py
+-rw-r--r--   0        0        0     7143 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/functional.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/helpers.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/models.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/module_loading.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/sync.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/url.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/pydantic/__init__.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/pydantic/schema.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 esmerald-2.0.2/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-2.0.2/LICENSE
+-rw-r--r--   0        0        0    15936 2020-02-02 00:00:00.000000 esmerald-2.0.2/README.md
+-rw-r--r--   0        0        0     5803 2020-02-02 00:00:00.000000 esmerald-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0    21120 2020-02-02 00:00:00.000000 esmerald-2.0.2/PKG-INFO
```

### Comparing `esmerald-2.0.1/esmerald/__init__.py` & `esmerald-2.0.2/esmerald/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.0.1"
+__version__ = "2.0.2"
 
 
 from starlette import status
 
 from esmerald.conf import settings
 from esmerald.conf.global_settings import EsmeraldAPISettings
 from esmerald.injector import Inject
```

### Comparing `esmerald-2.0.1/esmerald/applications.py` & `esmerald-2.0.2/esmerald/applications.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/backgound.py` & `esmerald-2.0.2/esmerald/backgound.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/enums.py` & `esmerald-2.0.2/esmerald/enums.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/exception_handlers.py` & `esmerald-2.0.2/esmerald/exception_handlers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import Union
+from typing import Any, List, Union
 
+from orjson import JSONDecodeError, loads
 from pydantic import ValidationError
 from starlette import status
 from starlette.exceptions import HTTPException as StarletteHTTPException
 from starlette.requests import Request
 from starlette.responses import Response as StarletteResponse
 
 from esmerald.enums import MediaType
@@ -33,23 +34,50 @@
         )
     elif not headers and extra:
         return JSONResponse({"detail": exc.detail, "extra": extra}, status_code=exc.status_code)
     else:
         return JSONResponse({"detail": exc.detail}, status_code=exc.status_code)
 
 
+def parse_non_serializable_objects_from_validation_error(values: List[Any]) -> List[Any]:
+    """
+    Parses non serializable objects from the validation error extras.
+    """
+    details = []
+    for detail in values:
+        detail_inputs = detail.get("input", None)
+        if not isinstance(detail_inputs, list):
+            details.append(detail)
+            continue
+
+        inputs = []
+        for input in detail_inputs:
+            if isinstance(input, object):
+                inputs.append(str(input.__class__.__name__))
+        detail["input"] = inputs
+        details.append(detail)
+
+    return details
+
+
 async def validation_error_exception_handler(
     request: Request, exc: ValidationError
 ) -> JSONResponse:
     extra = getattr(exc, "extra", None)
     status_code = status.HTTP_400_BAD_REQUEST
 
     if extra:
+        errors_extra = exc.extra.get("extra", {})
+        try:
+            details = loads(errors_extra)
+        except (TypeError, JSONDecodeError):
+            details = parse_non_serializable_objects_from_validation_error(errors_extra)
+
         return JSONResponse(
-            {"detail": exc.detail, "errors": exc.extra.get("extra", {})},
+            {"detail": exc.detail, "errors": details},
             status_code=status_code,
         )
     else:
         return JSONResponse(
             {"detail": exc.detail},
             status_code=status_code,
         )
```

### Comparing `esmerald-2.0.1/esmerald/exceptions.py` & `esmerald-2.0.2/esmerald/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/injector.py` & `esmerald-2.0.2/esmerald/injector.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/logging.py` & `esmerald-2.0.2/esmerald/logging.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/params.py` & `esmerald-2.0.2/esmerald/params.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,73 +3,74 @@
 from pydantic.dataclasses import dataclass
 from pydantic.fields import AliasChoices, AliasPath, FieldInfo
 
 from esmerald.enums import EncodingType, ParamType
 from esmerald.typing import Undefined
 from esmerald.utils.constants import IS_DEPENDENCY, SKIP_VALIDATION
 
+_PyUndefined: Any = Undefined
+
 
 class Param(FieldInfo):
     in_: ParamType
 
     def __init__(
         self,
-        default: Any = Undefined,
+        default: Any = _PyUndefined,
         *,
         allow_none: Optional[bool] = True,
-        default_factory: Optional[Callable[..., Any]] = None,
+        default_factory: Optional[Callable[..., Any]] = _PyUndefined,
         annotation: Optional[Any] = None,
         alias: Optional[str] = None,
-        alias_priority: Optional[int] = None,
-        value_type: Any = Undefined,
+        alias_priority: Optional[int] = _PyUndefined,
+        value_type: Any = _PyUndefined,
         header: Optional[str] = None,
         cookie: Optional[str] = None,
         query: Optional[str] = None,
         path: Optional[str] = None,
         content_encoding: Optional[str] = None,
         required: bool = True,
         title: Optional[str] = None,
         description: Optional[str] = None,
         const: Optional[bool] = None,
         gt: Optional[float] = None,
         ge: Optional[float] = None,
         lt: Optional[float] = None,
         le: Optional[float] = None,
-        multiple_of: Optional[float] = None,
-        allow_inf_nan: Optional[bool] = None,
+        multiple_of: Optional[float] = _PyUndefined,
+        allow_inf_nan: Optional[bool] = _PyUndefined,
         min_length: Optional[int] = None,
         max_length: Optional[int] = None,
+        max_digits: Optional[int] = _PyUndefined,
+        strict: Optional[bool] = _PyUndefined,
         pattern: Optional[str] = None,
-        example: Any = Undefined,
         examples: Optional[List[Any]] = None,
         deprecated: Optional[bool] = None,
         include_in_schema: bool = True,
         validation_alias: Optional[Union[str, AliasPath, AliasChoices]] = None,
         discriminator: Optional[str] = None,
         frozen: Optional[bool] = None,
         validate_default: bool = True,
         init_var: bool = True,
         kw_only: bool = True,
     ) -> None:
         self.deprecated = deprecated
-        self.example = example
         self.examples = examples
         self.include_in_schema = include_in_schema
         self.const = const
         self.allow_none = allow_none
 
         extra: Dict[str, Any] = {}
         extra.update(header=header)
         extra.update(cookie=cookie)
         extra.update(query=query)
         extra.update(path=path)
         extra.update(required=required)
         extra.update(content_encoding=content_encoding)
         extra.update(value_type=value_type)
-        extra.update(example=self.example)
         extra.update(examples=self.examples)
         extra.update(deprecated=self.deprecated)
         extra.update(include_in_schema=self.include_in_schema)
         extra.update(const=self.const)
         extra.update(allow_none=self.allow_none)
 
         super().__init__(
@@ -92,49 +93,55 @@
             examples=examples,
             allow_inf_nan=allow_inf_nan,
             json_schema_extra=extra,
             include=include_in_schema,
             validate_default=validate_default,
             validation_alias=validation_alias,
             discriminator=discriminator,
+            max_digits=max_digits,
+            strict=strict,
             frozen=frozen,
             init_var=init_var,
             kw_only=kw_only,
         )
 
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(annotation={self.annotation}, default={self.default})"
+
 
 class Header(Param):
     in_ = ParamType.HEADER
 
     def __init__(
         self,
         *,
-        default: Any = Undefined,
+        default: Any = _PyUndefined,
         allow_none: Optional[bool] = True,
-        default_factory: Optional[Callable[..., Any]] = None,
+        default_factory: Optional[Callable[..., Any]] = _PyUndefined,
         annotation: Optional[Any] = None,
         alias: Optional[str] = None,
-        alias_priority: Optional[int] = None,
+        alias_priority: Optional[int] = _PyUndefined,
         value: Optional[str] = None,
-        value_type: Any = Undefined,
+        value_type: Any = _PyUndefined,
         content_encoding: Optional[str] = None,
         required: bool = True,
         title: Optional[str] = None,
         description: Optional[str] = None,
         const: Optional[bool] = None,
         gt: Optional[float] = None,
         ge: Optional[float] = None,
         lt: Optional[float] = None,
         le: Optional[float] = None,
-        multiple_of: Optional[float] = None,
-        allow_inf_nan: Optional[bool] = None,
+        multiple_of: Optional[float] = _PyUndefined,
+        allow_inf_nan: Optional[bool] = _PyUndefined,
         min_length: Optional[int] = None,
         max_length: Optional[int] = None,
+        max_digits: Optional[int] = _PyUndefined,
+        strict: Optional[bool] = _PyUndefined,
         pattern: Optional[str] = None,
-        example: Any = Undefined,
         examples: Optional[List[Any]] = None,
         deprecated: Optional[bool] = None,
         include_in_schema: bool = True,
         validation_alias: Optional[Union[str, AliasPath, AliasChoices]] = None,
         discriminator: Optional[str] = None,
         frozen: Optional[bool] = None,
         validate_default: bool = True,
@@ -156,19 +163,20 @@
             ge=ge,
             lt=lt,
             le=le,
             multiple_of=multiple_of,
             allow_inf_nan=allow_inf_nan,
             min_length=min_length,
             max_length=max_length,
+            max_digits=max_digits,
+            strict=strict,
             pattern=pattern,
             required=required,
             content_encoding=content_encoding,
             value_type=value_type,
-            example=example,
             examples=examples,
             deprecated=deprecated,
             include_in_schema=include_in_schema,
             validate_default=validate_default,
             validation_alias=validation_alias,
             discriminator=discriminator,
             frozen=frozen,
@@ -178,38 +186,39 @@
 
 
 class Cookie(Param):
     in_ = ParamType.COOKIE
 
     def __init__(
         self,
-        default: Any = Undefined,
+        default: Any = _PyUndefined,
         *,
         allow_none: Optional[bool] = True,
-        default_factory: Optional[Callable[..., Any]] = None,
+        default_factory: Optional[Callable[..., Any]] = _PyUndefined,
         annotation: Optional[Any] = None,
         alias: Optional[str] = None,
-        alias_priority: Optional[int] = None,
-        value_type: Any = Undefined,
+        alias_priority: Optional[int] = _PyUndefined,
+        value_type: Any = _PyUndefined,
         value: Optional[str] = None,
         content_encoding: Optional[str] = None,
         required: bool = True,
         title: Optional[str] = None,
         description: Optional[str] = None,
         const: Optional[bool] = None,
         gt: Optional[float] = None,
         ge: Optional[float] = None,
         lt: Optional[float] = None,
         le: Optional[float] = None,
-        multiple_of: Optional[float] = None,
-        allow_inf_nan: Optional[bool] = None,
+        multiple_of: Optional[float] = _PyUndefined,
+        allow_inf_nan: Optional[bool] = _PyUndefined,
         min_length: Optional[int] = None,
         max_length: Optional[int] = None,
+        max_digits: Optional[int] = _PyUndefined,
+        strict: Optional[bool] = _PyUndefined,
         pattern: Optional[str] = None,
-        example: Any = Undefined,
         examples: Optional[List[Any]] = None,
         deprecated: Optional[bool] = None,
         include_in_schema: bool = True,
         validation_alias: Optional[Union[str, AliasPath, AliasChoices]] = None,
         discriminator: Optional[str] = None,
         frozen: Optional[bool] = None,
         validate_default: bool = True,
@@ -231,19 +240,20 @@
             ge=ge,
             lt=lt,
             le=le,
             multiple_of=multiple_of,
             allow_inf_nan=allow_inf_nan,
             min_length=min_length,
             max_length=max_length,
+            max_digits=max_digits,
+            strict=strict,
             pattern=pattern,
             required=required,
             content_encoding=content_encoding,
             value_type=value_type,
-            example=example,
             examples=examples,
             deprecated=deprecated,
             include_in_schema=include_in_schema,
             validate_default=validate_default,
             validation_alias=validation_alias,
             discriminator=discriminator,
             frozen=frozen,
@@ -253,38 +263,39 @@
 
 
 class Query(Param):
     in_ = ParamType.QUERY
 
     def __init__(
         self,
-        default: Any = Undefined,
+        default: Any = _PyUndefined,
         *,
         allow_none: Optional[bool] = True,
-        default_factory: Optional[Callable[..., Any]] = None,
+        default_factory: Optional[Callable[..., Any]] = _PyUndefined,
         annotation: Optional[Any] = None,
         alias: Optional[str] = None,
-        alias_priority: Optional[int] = None,
-        value_type: Any = Undefined,
+        alias_priority: Optional[int] = _PyUndefined,
+        value_type: Any = _PyUndefined,
         value: Optional[str] = None,
         content_encoding: Optional[str] = None,
         required: bool = True,
         title: Optional[str] = None,
         description: Optional[str] = None,
         const: Optional[bool] = None,
         gt: Optional[float] = None,
         ge: Optional[float] = None,
         lt: Optional[float] = None,
         le: Optional[float] = None,
-        multiple_of: Optional[float] = None,
-        allow_inf_nan: Optional[bool] = None,
+        multiple_of: Optional[float] = _PyUndefined,
+        allow_inf_nan: Optional[bool] = _PyUndefined,
         min_length: Optional[int] = None,
         max_length: Optional[int] = None,
+        max_digits: Optional[int] = _PyUndefined,
+        strict: Optional[bool] = _PyUndefined,
         pattern: Optional[str] = None,
-        example: Any = Undefined,
         examples: Optional[List[Any]] = None,
         deprecated: Optional[bool] = None,
         include_in_schema: bool = True,
         validation_alias: Optional[Union[str, AliasPath, AliasChoices]] = None,
         discriminator: Optional[str] = None,
         frozen: Optional[bool] = None,
         validate_default: bool = True,
@@ -306,19 +317,20 @@
             ge=ge,
             lt=lt,
             le=le,
             multiple_of=multiple_of,
             allow_inf_nan=allow_inf_nan,
             min_length=min_length,
             max_length=max_length,
+            max_digits=max_digits,
+            strict=strict,
             pattern=pattern,
             required=required,
             content_encoding=content_encoding,
             value_type=value_type,
-            example=example,
             examples=examples,
             deprecated=deprecated,
             include_in_schema=include_in_schema,
             validate_default=validate_default,
             validation_alias=validation_alias,
             discriminator=discriminator,
             frozen=frozen,
@@ -328,33 +340,34 @@
 
 
 class Path(Param):
     in_ = ParamType.PATH
 
     def __init__(
         self,
-        default: Any = Undefined,
+        default: Any = _PyUndefined,
         *,
         allow_none: Optional[bool] = True,
-        default_factory: Optional[Callable[..., Any]] = None,
+        default_factory: Optional[Callable[..., Any]] = _PyUndefined,
         annotation: Optional[Any] = None,
-        value_type: Any = Undefined,
+        value_type: Any = _PyUndefined,
         content_encoding: Optional[str] = None,
         required: bool = True,
         title: Optional[str] = None,
         description: Optional[str] = None,
         const: Optional[bool] = None,
         gt: Optional[float] = None,
         ge: Optional[float] = None,
         lt: Optional[float] = None,
         le: Optional[float] = None,
         min_length: Optional[int] = None,
         max_length: Optional[int] = None,
+        max_digits: Optional[int] = _PyUndefined,
+        strict: Optional[bool] = _PyUndefined,
         pattern: Optional[str] = None,
-        example: Any = Undefined,
         examples: Optional[List[Any]] = None,
         deprecated: Optional[bool] = None,
         include_in_schema: bool = True,
         validation_alias: Optional[Union[str, AliasPath, AliasChoices]] = None,
         discriminator: Optional[str] = None,
         frozen: Optional[bool] = None,
         validate_default: bool = True,
@@ -371,19 +384,20 @@
             const=const,
             gt=gt,
             ge=ge,
             lt=lt,
             le=le,
             min_length=min_length,
             max_length=max_length,
+            max_digits=max_digits,
+            strict=strict,
             pattern=pattern,
             required=required,
             content_encoding=content_encoding,
             value_type=value_type,
-            example=example,
             examples=examples,
             deprecated=deprecated,
             include_in_schema=include_in_schema,
             validate_default=validate_default,
             validation_alias=validation_alias,
             discriminator=discriminator,
             frozen=frozen,
@@ -391,50 +405,50 @@
             kw_only=kw_only,
         )
 
 
 class Body(FieldInfo):
     def __init__(
         self,
+        default: Any = _PyUndefined,
         *,
-        default: Any = Undefined,
         allow_none: Optional[bool] = True,
-        default_factory: Optional[Callable[..., Any]] = None,
+        default_factory: Optional[Callable[..., Any]] = _PyUndefined,
         annotation: Optional[Any] = None,
         media_type: Union[str, EncodingType] = EncodingType.JSON,
         content_encoding: Optional[str] = None,
         title: Optional[str] = None,
         alias: Optional[str] = None,
-        alias_priority: Optional[int] = None,
+        alias_priority: Optional[int] = _PyUndefined,
         description: Optional[str] = None,
         const: Optional[bool] = None,
         embed: Optional[bool] = None,
         gt: Optional[float] = None,
         ge: Optional[float] = None,
         lt: Optional[float] = None,
         le: Optional[float] = None,
-        multiple_of: Optional[float] = None,
-        allow_inf_nan: Optional[bool] = None,
+        multiple_of: Optional[float] = _PyUndefined,
+        allow_inf_nan: Optional[bool] = _PyUndefined,
+        max_digits: Optional[int] = _PyUndefined,
+        strict: Optional[bool] = _PyUndefined,
         min_length: Optional[int] = None,
         max_length: Optional[int] = None,
         pattern: Optional[str] = None,
-        example: Any = Undefined,
         examples: Optional[List[Any]] = None,
         validation_alias: Optional[Union[str, AliasPath, AliasChoices]] = None,
         discriminator: Optional[str] = None,
         frozen: Optional[bool] = None,
         validate_default: bool = True,
         init_var: bool = True,
         kw_only: bool = True,
         include_in_schema: bool = True,
     ) -> None:
         extra: Dict[str, Any] = {}
         self.media_type = media_type
         self.content_encoding = content_encoding
-        self.example = example
         self.examples = examples
         self.allow_none = allow_none
         self.include_in_schema = include_in_schema
 
         extra.update(media_type=self.media_type)
         extra.update(content_encoding=self.content_encoding)
         extra.update(embed=embed)
@@ -450,60 +464,68 @@
             description=description,
             const=const,
             gt=gt,
             ge=ge,
             lt=lt,
             le=le,
             multiple_of=multiple_of,
+            max_digits=max_digits,
             allow_inf_nan=allow_inf_nan,
             min_length=min_length,
             max_length=max_length,
             pattern=pattern,
             json_schema_extra=extra,
             validate_default=validate_default,
             validation_alias=validation_alias,
             discriminator=discriminator,
             frozen=frozen,
             init_var=init_var,
+            strict=strict,
             kw_only=kw_only,
         )
 
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(annotation={self.annotation}, default={self.default})"
+
 
 class Form(Body):
     def __init__(
         self,
-        default: Any,
+        default: Any = _PyUndefined,
         *,
-        default_factory: Optional[Callable[..., Any]] = None,
+        annotation: Optional[Any] = None,
+        default_factory: Optional[Callable[..., Any]] = _PyUndefined,
         allow_none: Optional[bool] = True,
         media_type: Union[str, EncodingType] = EncodingType.URL_ENCODED,
         content_encoding: Optional[str] = None,
         alias: Optional[str] = None,
-        alias_priority: Optional[int] = None,
+        alias_priority: Optional[int] = _PyUndefined,
         title: Optional[str] = None,
         description: Optional[str] = None,
         gt: Optional[float] = None,
         ge: Optional[float] = None,
         lt: Optional[float] = None,
         le: Optional[float] = None,
         min_length: Optional[int] = None,
         max_length: Optional[int] = None,
         pattern: Optional[str] = None,
-        example: Any = Undefined,
         examples: Optional[List[Any]] = None,
         validation_alias: Optional[Union[str, AliasPath, AliasChoices]] = None,
         discriminator: Optional[str] = None,
+        max_digits: Optional[int] = _PyUndefined,
+        strict: Optional[bool] = _PyUndefined,
         frozen: Optional[bool] = None,
         validate_default: bool = True,
         init_var: bool = True,
         kw_only: bool = True,
         include_in_schema: bool = True,
     ) -> None:
         super().__init__(
             default=default,
+            annotation=annotation,
             allow_none=allow_none,
             default_factory=default_factory,
             embed=True,
             media_type=media_type,
             content_encoding=content_encoding,
             alias=alias,
             alias_priority=alias_priority,
@@ -512,58 +534,62 @@
             gt=gt,
             ge=ge,
             lt=lt,
             le=le,
             min_length=min_length,
             max_length=max_length,
             pattern=pattern,
-            example=example,
             examples=examples,
             validate_default=validate_default,
             validation_alias=validation_alias,
             discriminator=discriminator,
             frozen=frozen,
             init_var=init_var,
             kw_only=kw_only,
             include_in_schema=include_in_schema,
+            max_digits=max_digits,
+            strict=strict,
         )
 
 
 class File(Form):
     def __init__(
         self,
-        default: Any,
+        default: Any = _PyUndefined,
         *,
+        annotation: Optional[Any] = None,
         allow_none: Optional[bool] = True,
-        default_factory: Optional[Callable[..., Any]] = None,
+        default_factory: Optional[Callable[..., Any]] = _PyUndefined,
         media_type: Union[str, EncodingType] = EncodingType.MULTI_PART,
         content_encoding: Optional[str] = None,
         alias: Optional[str] = None,
-        alias_priority: Optional[int] = None,
+        alias_priority: Optional[int] = _PyUndefined,
         title: Optional[str] = None,
         description: Optional[str] = None,
         gt: Optional[float] = None,
         ge: Optional[float] = None,
         lt: Optional[float] = None,
         le: Optional[float] = None,
         min_length: Optional[int] = None,
         max_length: Optional[int] = None,
         pattern: Optional[str] = None,
-        example: Any = Undefined,
         examples: Optional[List[Any]] = None,
         validation_alias: Optional[Union[str, AliasPath, AliasChoices]] = None,
         discriminator: Optional[str] = None,
+        max_digits: Optional[int] = _PyUndefined,
+        strict: Optional[bool] = _PyUndefined,
         frozen: Optional[bool] = None,
         validate_default: bool = True,
         init_var: bool = True,
         kw_only: bool = True,
         include_in_schema: bool = True,
     ) -> None:
         super().__init__(
             default=default,
+            annotation=annotation,
             allow_none=allow_none,
             default_factory=default_factory,
             media_type=media_type,
             content_encoding=content_encoding,
             alias=alias,
             alias_priority=alias_priority,
             title=title,
@@ -571,19 +597,20 @@
             gt=gt,
             ge=ge,
             lt=lt,
             le=le,
             min_length=min_length,
             max_length=max_length,
             pattern=pattern,
-            example=example,
             examples=examples,
             validate_default=validate_default,
             validation_alias=validation_alias,
             discriminator=discriminator,
+            max_digits=max_digits,
+            strict=strict,
             frozen=frozen,
             init_var=init_var,
             kw_only=kw_only,
             include_in_schema=include_in_schema,
         )
```

### Comparing `esmerald-2.0.1/esmerald/parsers.py` & `esmerald-2.0.2/esmerald/parsers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from contextlib import suppress
 from json import JSONDecodeError, loads
-from typing import TYPE_CHECKING, Any, Dict
+from typing import TYPE_CHECKING, Any, Dict, List, get_args, get_origin
 
 from pydantic import BaseModel, ConfigDict
-from pydantic.v1.fields import SHAPE_LIST, SHAPE_SINGLETON
+from starlette.datastructures import UploadFile as StarletteUploadFile
 
 from esmerald.datastructures import UploadFile
 from esmerald.enums import EncodingType
 
 if TYPE_CHECKING:
     from pydantic.fields import FieldInfo
     from starlette.datastructures import FormData
@@ -57,39 +57,53 @@
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
 
 class ArbitraryExtraBaseModel(BaseModel):
     model_config = ConfigDict(extra="allow", arbitrary_types_allowed=True)
 
 
-def validate_media_type(field: "FieldInfo", values: Any) -> Any:
+def flatten(values: List[Any]) -> List[Any]:
     """
-    Validates the media type against the available types.
+    Flattens a list
     """
-    if field.shape == SHAPE_LIST:
-        return list(values.values())
-    if field.shape == SHAPE_SINGLETON and field.type_in[UploadFile] and values:
-        return list(values.values())[0]
+    flattened = []
+
+    for value in values:
+        if isinstance(value, list):
+            flattened.extend(flatten(value))
+        else:
+            flattened.append(value)
+    return flattened
 
 
 def parse_form_data(media_type: "EncodingType", form_data: "FormData", field: "FieldInfo") -> Any:
-    values: Any = {}
+    """
+    Converts, parses and transforms a multidict into a dict and tries to load them all into
+    json.
+    """
+    values_dict: Dict[str, Any] = {}
     for key, value in form_data.multi_items():
-        if not isinstance(value, UploadFile):
+        if not isinstance(value, StarletteUploadFile):
             with suppress(JSONDecodeError):
                 value = loads(value)
-        if isinstance(value, UploadFile):
-            value = UploadFile(
-                file=value.file,
-                filename=value.filename,
-                headers=value.headers,
-            )
-        if values.get(key):
-            if isinstance(values[key], list):
-                values[key].append(value)
-            else:
-                values[key] = [values[key], value]
+        value_in_dict = values_dict.get(key)
+        if isinstance(value_in_dict, list):
+            values_dict[key].append(value)
+        elif value_in_dict:
+            values_dict[key] = [value_in_dict, value]
         else:
-            values[key] = value
+            values_dict[key] = value
+
     if media_type == EncodingType.MULTI_PART:
-        return validate_media_type(field=field, values=values)
-    return values
+        if get_origin(field.annotation) is list:
+            values = list(values_dict.values())
+            return flatten(values=values)
+        if field.annotation in (StarletteUploadFile, UploadFile) and values_dict:
+            return list(values_dict.values())[0]
+
+        # Check the arguments if there is any MULTI_PART in a possible Union with UploadFile
+        # and a None (Optional).
+        for arg in get_args(field.annotation):
+            if issubclass(arg, (StarletteUploadFile, UploadFile)) and values_dict:
+                return list(values_dict.values())[0]
+
+    return values_dict if values_dict else None
```

### Comparing `esmerald-2.0.1/esmerald/requests.py` & `esmerald-2.0.2/esmerald/requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from json import loads
+# from json import loads
 from typing import TYPE_CHECKING, Any, cast
 
+from orjson import loads
 from starlette.datastructures import URL  # noqa
 from starlette.requests import ClientDisconnect as ClientDisconnect  # noqa
 from starlette.requests import HTTPConnection as HTTPConnection  # noqa: F401
 from starlette.requests import Request as StarletteRequest  # noqa: F401
 from starlette.requests import empty_receive, empty_send  # noqa
+from starlette.types import Receive, Scope, Send
 
 from esmerald.typing import Void
 
 if TYPE_CHECKING:
     from esmerald.applications import Esmerald
     from esmerald.conf.global_settings import EsmeraldAPISettings
-    from esmerald.types import HTTPMethod, Receive, Scope, Send
+    from esmerald.types import HTTPMethod
 
 
 class Request(StarletteRequest):
     def __init__(
         self,
         scope: "Scope",
         receive: "Receive" = empty_receive,
```

### Comparing `esmerald-2.0.1/esmerald/testclient.py` & `esmerald-2.0.2/esmerald/testclient.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/types.py` & `esmerald-2.0.2/esmerald/types.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/websockets.py` & `esmerald-2.0.2/esmerald/websockets.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/conf/__init__.py` & `esmerald-2.0.2/esmerald/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/conf/global_settings.py` & `esmerald-2.0.2/esmerald/conf/global_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,18 @@
     docs_url: Optional[str] = "/docs/swagger"
     redoc_url: Optional[str] = "/docs/redoc"
     swagger_ui_oauth2_redirect_url: Optional[str] = "/docs/oauth2-redirect"
     redoc_js_url: str = "https://cdn.jsdelivr.net/npm/redoc@next/bundles/redoc.standalone.js"
     redoc_favicon_url: str = "https://esmerald.dev/statics/images/favicon.ico"
     swagger_ui_init_oauth: Optional[Dict[str, Any]] = None
     swagger_ui_parameters: Optional[Dict[str, Any]] = None
-    swagger_js_url: str = "https://cdn.jsdelivr.net/npm/swagger-ui-dist@5/swagger-ui-bundle.js"
-    swagger_css_url: str = "https://cdn.jsdelivr.net/npm/swagger-ui-dist@5/swagger-ui.css"
+    swagger_js_url: str = (
+        "https://cdn.jsdelivr.net/npm/swagger-ui-dist@5.1.3/swagger-ui-bundle.min.js"
+    )
+    swagger_css_url: str = "https://cdn.jsdelivr.net/npm/swagger-ui-dist@5.1.3/swagger-ui.min.css"
     swagger_favicon_url: str = "https://esmerald.dev/statics/images/favicon.ico"
 
     # Model configuration
     model_config = SettingsConfigDict(extra="allow", ignored_types=(cached_property,))
 
     @property
     def reload(self) -> bool:
```

### Comparing `esmerald-2.0.1/esmerald/conf/project_template/.gitignore.e-tpl` & `esmerald-2.0.2/esmerald/conf/project_template/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/conf/project_template/Makefile.e-tpl` & `esmerald-2.0.2/esmerald/conf/project_template/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/conf/project_template/project_name/main.py-tpl` & `esmerald-2.0.2/esmerald/conf/project_template/project_name/main.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/conf/project_template/project_name/serve.py-tpl` & `esmerald-2.0.2/esmerald/conf/project_template/project_name/serve.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/conf/project_template/project_name/urls.py-tpl` & `esmerald-2.0.2/esmerald/conf/project_template/project_name/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/conf/project_template/project_name/configs/settings.py-tpl` & `esmerald-2.0.2/esmerald/conf/project_template/project_name/configs/settings.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/config/jwt.py` & `esmerald-2.0.2/esmerald/config/jwt.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/config/openapi.py` & `esmerald-2.0.2/esmerald/config/openapi.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/config/session.py` & `esmerald-2.0.2/esmerald/config/session.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/config/static_files.py` & `esmerald-2.0.2/esmerald/config/static_files.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/contrib/encoding.py` & `esmerald-2.0.2/esmerald/contrib/encoding.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/contrib/auth/hashers.py` & `esmerald-2.0.2/esmerald/contrib/auth/hashers.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/contrib/auth/common/middleware.py` & `esmerald-2.0.2/esmerald/contrib/auth/common/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/contrib/auth/saffier/base_user.py` & `esmerald-2.0.2/esmerald/contrib/auth/saffier/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/contrib/auth/saffier/middleware.py` & `esmerald-2.0.2/esmerald/contrib/auth/saffier/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/core/directives/base.py` & `esmerald-2.0.2/esmerald/core/directives/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/core/directives/cli.py` & `esmerald-2.0.2/esmerald/core/directives/cli.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/core/directives/env.py` & `esmerald-2.0.2/esmerald/core/directives/env.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/core/directives/templates.py` & `esmerald-2.0.2/esmerald/core/directives/templates.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/core/directives/utils.py` & `esmerald-2.0.2/esmerald/core/directives/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/core/directives/operations/createapp.py` & `esmerald-2.0.2/esmerald/core/directives/operations/createapp.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/core/directives/operations/createproject.py` & `esmerald-2.0.2/esmerald/core/directives/operations/createproject.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/core/directives/operations/list.py` & `esmerald-2.0.2/esmerald/core/directives/operations/list.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/core/directives/operations/run.py` & `esmerald-2.0.2/esmerald/core/directives/operations/run.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/core/directives/operations/runserver.py` & `esmerald-2.0.2/esmerald/core/directives/operations/runserver.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/core/directives/operations/show_urls.py` & `esmerald-2.0.2/esmerald/core/directives/operations/show_urls.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/core/terminal/base.py` & `esmerald-2.0.2/esmerald/core/terminal/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/core/terminal/print.py` & `esmerald-2.0.2/esmerald/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/core/terminal/terminal.py` & `esmerald-2.0.2/esmerald/core/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/core/urls/base.py` & `esmerald-2.0.2/esmerald/core/urls/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/datastructures/__init__.py` & `esmerald-2.0.2/esmerald/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/datastructures/encoders.py` & `esmerald-2.0.2/esmerald/datastructures/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/datastructures/file.py` & `esmerald-2.0.2/esmerald/datastructures/file.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/datastructures/json.py` & `esmerald-2.0.2/esmerald/datastructures/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/datastructures/redirect.py` & `esmerald-2.0.2/esmerald/datastructures/redirect.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/datastructures/stream.py` & `esmerald-2.0.2/esmerald/datastructures/stream.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/datastructures/template.py` & `esmerald-2.0.2/esmerald/datastructures/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/interceptors/interceptor.py` & `esmerald-2.0.2/esmerald/interceptors/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/middleware/__init__.py` & `esmerald-2.0.2/esmerald/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/middleware/_exception_handlers.py` & `esmerald-2.0.2/esmerald/middleware/_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/middleware/asyncexitstack.py` & `esmerald-2.0.2/esmerald/middleware/asyncexitstack.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/middleware/authentication.py` & `esmerald-2.0.2/esmerald/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/middleware/basic.py` & `esmerald-2.0.2/esmerald/middleware/basic.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/middleware/csrf.py` & `esmerald-2.0.2/esmerald/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/middleware/errors.py` & `esmerald-2.0.2/esmerald/middleware/errors.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/middleware/exceptions.py` & `esmerald-2.0.2/esmerald/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/middleware/settings_middleware.py` & `esmerald-2.0.2/esmerald/middleware/settings_middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/openapi/datastructures.py` & `esmerald-2.0.2/esmerald/openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/openapi/docs.py` & `esmerald-2.0.2/esmerald/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/openapi/models.py` & `esmerald-2.0.2/esmerald/openapi/models.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/openapi/openapi.py` & `esmerald-2.0.2/esmerald/openapi/openapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 import http.client
 import json
 import warnings
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Set, Tuple, Union, cast
+from typing import Any, Dict, List, Optional, Sequence, Set, Tuple, Union, cast
 
 from pydantic import AnyUrl
 from pydantic.fields import FieldInfo
 from pydantic.json_schema import GenerateJsonSchema, JsonSchemaValue
 from starlette.routing import BaseRoute
 from starlette.status import HTTP_422_UNPROCESSABLE_ENTITY
 from typing_extensions import Literal
 
+from esmerald.enums import MediaType
 from esmerald.openapi.constants import METHODS_WITH_BODY, REF_PREFIX, REF_TEMPLATE
 from esmerald.openapi.models import Contact, Info, License, OpenAPI, Operation, Parameter, Tag
 from esmerald.openapi.responses import create_internal_response
 from esmerald.openapi.utils import (
+    STATUS_CODE_RANGES,
+    VALIDATION_ERROR_DEFINITION,
+    VALIDATION_ERROR_RESPONSE_DEFINITION,
     dict_update,
     get_definitions,
     get_schema_from_model_field,
     is_status_code_allowed,
-    status_code_ranges,
-    validation_error_definition,
-    validation_error_response_definition,
 )
-from esmerald.params import Body, Param
+from esmerald.params import Param
 from esmerald.routing import gateways, router
-from esmerald.typing import Undefined
 from esmerald.utils.constants import DATA
 from esmerald.utils.helpers import is_class_and_subclass
 from esmerald.utils.url import clean_path
 
-if TYPE_CHECKING:
-    pass
-
 
 def get_flat_params(route: Union[router.HTTPHandler, Any]) -> List[Any]:
     """Gets all the neded params of the request and route"""
     path_params = [param.field_info for param in route.transformer.get_path_params()]
     cookie_params = [param.field_info for param in route.transformer.get_cookie_params()]
     query_params = [param.field_info for param in route.transformer.get_query_params()]
     header_params = [param.field_info for param in route.transformer.get_header_params()]
@@ -134,16 +131,16 @@
             param_in=field_info.in_.value,
             required=param.is_required(),
             schema=param_schema,  # type: ignore
         )
 
         if field_info.description:
             parameter.description = field_info.description
-        if field_info.example != Undefined:
-            parameter.example = json.dumps(field_info.example)
+        if field_info.examples is not None:
+            parameter.example = json.dumps(field_info.examples)
         if field_info.deprecated:
             parameter.deprecated = field_info.deprecated
 
         parameters.append(parameter.model_dump(by_alias=True))
     return parameters
 
 
@@ -152,30 +149,26 @@
     data_field: Optional[FieldInfo],
     field_mapping: Dict[Tuple[FieldInfo, Literal["validation", "serialization"]], JsonSchemaValue],
 ) -> Optional[Dict[str, Any]]:
     if not data_field:
         return None
 
     assert isinstance(data_field, FieldInfo), "The 'data' needs to be a FieldInfo"
-    schema = get_schema_from_model_field(
-        field=data_field,
-        field_mapping=field_mapping,
-    )
-
-    field_info = cast(Body, data_field)
-    request_media_type = field_info.media_type.value  # type: ignore
+    schema = get_schema_from_model_field(field=data_field, field_mapping=field_mapping)
+    field_info = data_field
+    request_media_type = data_field.json_schema_extra.get("media_type").value
     required = field_info.is_required()
 
     request_data_oai: Dict[str, Any] = {}
     if required:
         request_data_oai["required"] = required
 
     request_media_content: Dict[str, Any] = {"schema": schema}
-    if field_info.example != Undefined:
-        request_media_content["example"] = json.dumps(field_info.example)
+    if field_info.examples is not None:
+        request_media_content["example"] = json.dumps(field_info.examples)
     request_data_oai["content"] = {request_media_type: request_media_content}
     return request_data_oai
 
 
 def get_openapi_path(
     *,
     route: gateways.Gateway,
@@ -247,24 +240,23 @@
         operation.setdefault("responses", {}).setdefault(status_code, {})[
             "description"
         ] = handler.response_description
 
         # Media type
         if route_response_media_type and is_status_code_allowed(handler.status_code):
             response_schema = {"type": "string"}
-            response_schema = {}
 
             operation.setdefault("responses", {}).setdefault(status_code, {}).setdefault(
                 "content", {}
             ).setdefault(route_response_media_type, {})["schema"] = response_schema
 
         # Additional responses
         if handler.response_models:
             operation_responses = operation.setdefault("responses", {})
-            for additional_status_code, _additional_response in handler.response_models.items():
+            for additional_status_code, _ in handler.response_models.items():
                 process_response = handler.responses[additional_status_code].model_copy()
                 status_code_key = str(additional_status_code).upper()
 
                 if status_code_key == "DEFAULT":
                     status_code_key = "default"
 
                 openapi_response = operation_responses.setdefault(status_code_key, {})
@@ -273,26 +265,26 @@
                 additional_field_schema: Optional[Dict[str, Any]] = None
                 model_schema = process_response.model_json_schema()
 
                 if field:
                     additional_field_schema = get_schema_from_model_field(
                         field=field, field_mapping=field_mapping
                     )
-                    media_type = route_response_media_type or "application/json"
+                    media_type = route_response_media_type or MediaType.JSON.value
                     additional_schema = (
                         model_schema.setdefault("content", {})
                         .setdefault(media_type, {})
                         .setdefault("schema", {})
                     )
                     dict_update(additional_schema, additional_field_schema)
 
                 # status
                 status_text = (
                     process_response.status_text
-                    or status_code_ranges.get(str(additional_status_code).upper())
+                    or STATUS_CODE_RANGES.get(str(additional_status_code).upper())
                     or http.client.responses.get(int(additional_status_code))
                 )
                 description = (
                     process_response.description
                     or openapi_response.get("description")
                     or status_text
                     or "Additional Response"
@@ -310,16 +302,16 @@
                 "content": {
                     "application/json": {"schema": {"$ref": REF_PREFIX + "HTTPValidationError"}}
                 },
             }
             if "ValidationError" not in definitions:
                 definitions.update(
                     {
-                        "ValidationError": validation_error_definition,
-                        "HTTPValidationError": validation_error_response_definition,
+                        "ValidationError": VALIDATION_ERROR_DEFINITION,
+                        "HTTPValidationError": VALIDATION_ERROR_RESPONSE_DEFINITION,
                     }
                 )
         path[method.lower()] = operation
     return path, security_schemes, definitions
 
 
 def should_include_in_schema(route: router.Include) -> bool:
```

### Comparing `esmerald-2.0.1/esmerald/openapi/responses.py` & `esmerald-2.0.2/esmerald/openapi/responses.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/openapi/utils.py` & `esmerald-2.0.2/esmerald/openapi/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,25 @@
 from typing import Any, Dict, List, Tuple, Union
 
 from pydantic import TypeAdapter
 from pydantic.fields import FieldInfo
 from pydantic.json_schema import GenerateJsonSchema, JsonSchemaValue
 from typing_extensions import Literal
 
-from esmerald.openapi.constants import REF_PREFIX
+from esmerald.openapi.validation import (
+    validation_error_definition,
+    validation_error_response_definition,
+)
 
-validation_error_definition = {
-    "title": "ValidationError",
-    "type": "object",
-    "properties": {
-        "loc": {
-            "title": "Location",
-            "type": "array",
-            "items": {"anyOf": [{"type": "string"}, {"type": "integer"}]},
-        },
-        "msg": {"title": "Message", "type": "string"},
-        "type": {"title": "Error Type", "type": "string"},
-    },
-    "required": ["loc", "msg", "type"],
-}
-
-validation_error_response_definition = {
-    "title": "HTTPValidationError",
-    "type": "object",
-    "properties": {
-        "detail": {
-            "title": "Detail",
-            "type": "array",
-            "items": {"$ref": REF_PREFIX + "ValidationError"},
-        }
-    },
-}
+VALIDATION_ERROR_DEFINITION = validation_error_definition.model_dump(exclude_none=True)
+VALIDATION_ERROR_RESPONSE_DEFINITION = validation_error_response_definition.model_dump(
+    exclude_none=True
+)
 
-status_code_ranges: Dict[str, str] = {
+STATUS_CODE_RANGES: Dict[str, str] = {
     "1XX": "Information",
     "2XX": "Success",
     "3XX": "Redirection",
     "4XX": "Client Error",
     "5XX": "Server Error",
     "DEFAULT": "Default Response",
 }
```

### Comparing `esmerald-2.0.1/esmerald/permissions/base.py` & `esmerald-2.0.2/esmerald/permissions/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/permissions/utils.py` & `esmerald-2.0.2/esmerald/permissions/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/pluggables/base.py` & `esmerald-2.0.2/esmerald/pluggables/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/protocols/asyncdao.py` & `esmerald-2.0.2/esmerald/protocols/asyncdao.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/protocols/dao.py` & `esmerald-2.0.2/esmerald/protocols/dao.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/protocols/interceptor.py` & `esmerald-2.0.2/esmerald/protocols/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/protocols/template.py` & `esmerald-2.0.2/esmerald/protocols/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/responses/base.py` & `esmerald-2.0.2/esmerald/responses/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/responses/encoders.py` & `esmerald-2.0.2/esmerald/responses/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/responses/json.py` & `esmerald-2.0.2/esmerald/responses/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/responses/template.py` & `esmerald-2.0.2/esmerald/responses/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/routing/base.py` & `esmerald-2.0.2/esmerald/routing/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/routing/events.py` & `esmerald-2.0.2/esmerald/routing/events.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/routing/gateways.py` & `esmerald-2.0.2/esmerald/routing/gateways.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/routing/handlers.py` & `esmerald-2.0.2/esmerald/routing/handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/routing/router.py` & `esmerald-2.0.2/esmerald/routing/router.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/routing/views.py` & `esmerald-2.0.2/esmerald/routing/views.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/security/jwt/token.py` & `esmerald-2.0.2/esmerald/security/jwt/token.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/template/jinja.py` & `esmerald-2.0.2/esmerald/template/jinja.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/template/mako.py` & `esmerald-2.0.2/esmerald/template/mako.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/transformers/datastructures.py` & `esmerald-2.0.2/esmerald/transformers/datastructures.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/transformers/helpers.py` & `esmerald-2.0.2/esmerald/transformers/helpers.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/transformers/model.py` & `esmerald-2.0.2/esmerald/transformers/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,14 @@
         for param in param_settings:
             if param.param_type == ParamType.QUERY:
                 query_params.add(param)
 
         query_params_names: Set[ParamSetting] = set()
 
         form_data = None
-
         # For the reserved keyword data
         data_field = signature_model.model_fields.get("data")
         if data_field:
             extra = getattr(data_field, "json_schema_extra", None) or {}
             media_type = extra.get("media_type")
             if media_type in MEDIA_TYPES:
                 form_data = (media_type, data_field)
```

### Comparing `esmerald-2.0.1/esmerald/transformers/signature.py` & `esmerald-2.0.2/esmerald/transformers/signature.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/transformers/types.py` & `esmerald-2.0.2/esmerald/transformers/types.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/transformers/utils.py` & `esmerald-2.0.2/esmerald/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/utils/constants.py` & `esmerald-2.0.2/esmerald/utils/constants.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/utils/crypto.py` & `esmerald-2.0.2/esmerald/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/utils/dependency.py` & `esmerald-2.0.2/esmerald/utils/dependency.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/utils/functional.py` & `esmerald-2.0.2/esmerald/utils/functional.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/utils/helpers.py` & `esmerald-2.0.2/esmerald/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/utils/module_loading.py` & `esmerald-2.0.2/esmerald/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/utils/sync.py` & `esmerald-2.0.2/esmerald/utils/sync.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/esmerald/utils/pydantic/schema.py` & `esmerald-2.0.2/esmerald/utils/pydantic/schema.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/LICENSE` & `esmerald-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/README.md` & `esmerald-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.1/pyproject.toml` & `esmerald-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -46,17 +46,18 @@
     "httpx>=0.24.0,<0.30.0",
     "itsdangerous>=2.1.2,<3.0.0",
     "jinja2>=3.1.2,<4.0.0",
     "jsonschema_rs>=0.16.2,<0.20.0",
     "loguru>=0.7.0,<0.8.0",
     "pydantic>=2.0.1,<3.0.0",
     "pydantic-extra-types>=2.0.0,<3.0.0",
-    "pydantic-settings>=2.0.0,<3.0.0",
-    "python-multipart>=0.0.5,<0.0.7",
+    "pydantic-settings>=2.0.2,<3.0.0",
+    "python-multipart>=0.0.5",
     "openapi-schemas-pydantic>=2.0.0",
+    "orjson>=3.8.5,<4.0.0",
     "rich>=13.3.1,<14.0.0",
     "starlette>=0.30.0,<1.0",
 ]
 keywords = [
     "api",
     "rest",
     "http",
@@ -108,15 +109,14 @@
     "jinja2>=3.1.2,<4.0.0",
     "flask>=1.1.2,<3.0.0",
     "freezegun>=1.2.2,<2.0.0",
     "mock==5.0.1",
     "passlib==1.7.4",
     "polyfactory>=2.5.0,<3.0.0",
     "python-jose>=3.3.0,<4",
-    "orjson>=3.8.5,<4.0.0",
     "saffier[postgres]>=0.15.0",
     "requests>=2.28.2,<3.0.0",
     "ruff>=0.0.256,<1.0.0",
     "ujson>=5.7.0,<6",
 
     # types
     "types-ujson==5.8.0.0",
```

### Comparing `esmerald-2.0.1/PKG-INFO` & `esmerald-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esmerald
-Version: 2.0.1
+Version: 2.0.2
 Summary: Highly scalable, performant, easy to learn, easy to code and for every application.
 Project-URL: Homepage, https://github.com/dymmond/esmerald
 Project-URL: Documentation, https://esmerald.dymmond.com/
 Project-URL: Changelog, https://esmerald.dymmond.com/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/esmerald
 Author-email: Tiago Silva <tiago.silva@dymmond.com>
@@ -43,18 +43,19 @@
 Requires-Dist: click<9.0.0,>=8.1.4
 Requires-Dist: httpx<0.30.0,>=0.24.0
 Requires-Dist: itsdangerous<3.0.0,>=2.1.2
 Requires-Dist: jinja2<4.0.0,>=3.1.2
 Requires-Dist: jsonschema-rs<0.20.0,>=0.16.2
 Requires-Dist: loguru<0.8.0,>=0.7.0
 Requires-Dist: openapi-schemas-pydantic>=2.0.0
+Requires-Dist: orjson<4.0.0,>=3.8.5
 Requires-Dist: pydantic-extra-types<3.0.0,>=2.0.0
-Requires-Dist: pydantic-settings<3.0.0,>=2.0.0
+Requires-Dist: pydantic-settings<3.0.0,>=2.0.2
 Requires-Dist: pydantic<3.0.0,>=2.0.1
-Requires-Dist: python-multipart<0.0.7,>=0.0.5
+Requires-Dist: python-multipart>=0.0.5
 Requires-Dist: rich<14.0.0,>=13.3.1
 Requires-Dist: starlette<1.0,>=0.30.0
 Provides-Extra: dev
 Requires-Dist: autoflake>=1.4.0; extra == 'dev'
 Requires-Dist: flake8<6.0.0,>=3.8.3; extra == 'dev'
 Requires-Dist: pre-commit<4.0.0,>=3.0.4; extra == 'dev'
 Requires-Dist: uvicorn[standard]>=0.19.0; extra == 'dev'
@@ -88,15 +89,14 @@
 Requires-Dist: flake8>=5.0.4; extra == 'test'
 Requires-Dist: flask<3.0.0,>=1.1.2; extra == 'test'
 Requires-Dist: freezegun<2.0.0,>=1.2.2; extra == 'test'
 Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'test'
 Requires-Dist: jinja2<4.0.0,>=3.1.2; extra == 'test'
 Requires-Dist: mock==5.0.1; extra == 'test'
 Requires-Dist: mypy>=1.4.1; extra == 'test'
-Requires-Dist: orjson<4.0.0,>=3.8.5; extra == 'test'
 Requires-Dist: passlib==1.7.4; extra == 'test'
 Requires-Dist: polyfactory<3.0.0,>=2.5.0; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.19.0; extra == 'test'
 Requires-Dist: pytest-cov<5.0.0,>=2.12.0; extra == 'test'
 Requires-Dist: pytest<8.0.0,>=7.3.1; extra == 'test'
 Requires-Dist: python-jose<4,>=3.3.0; extra == 'test'
 Requires-Dist: requests<3.0.0,>=2.28.2; extra == 'test'
```

