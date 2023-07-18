# Comparing `tmp/port_ocean-0.1.0rc1.tar.gz` & `tmp/port_ocean-0.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_ocean-0.1.0rc1.tar", max compression
+gzip compressed data, was "port_ocean-0.1.0rc2.tar", max compression
```

## Comparing `port_ocean-0.1.0rc1.tar` & `port_ocean-0.1.0rc2.tar`

### file list

```diff
@@ -1,89 +1,96 @@
--rw-r--r--   0        0        0    11357 2023-07-17 09:45:56.503705 port_ocean-0.1.0rc1/LICENSE
--rw-r--r--   0        0        0     4585 2023-07-17 09:45:56.507705 port_ocean-0.1.0rc1/README.md
--rw-r--r--   0        0        0      614 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/__init__.py
--rw-r--r--   0        0        0       57 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cli.py
--rw-r--r--   0        0        0     5081 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/commands.py
--rw-r--r--   0        0        0      429 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/cookiecutter.json
--rw-r--r--   0        0        0       42 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
--rw-r--r--   0        0        0     2698 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
--rw-r--r--   0        0        0      388 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
--rw-r--r--   0        0        0      598 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
--rw-r--r--   0        0        0     1699 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
--rw-r--r--   0        0        0      653 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
--rw-r--r--   0        0        0       12 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog_fragments/.gitignore
--rw-r--r--   0        0        0      778 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
--rw-r--r--   0        0        0       71 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
--rw-r--r--   0        0        0     1669 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
--rw-r--r--   0        0        0       46 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
--rw-r--r--   0        0        0     1267 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
--rw-r--r--   0        0        0     1755 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/download_git_folder.py
--rw-r--r--   0        0        0      722 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/list_integrations.py
--rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/clients/port/__init__.py
--rw-r--r--   0        0        0     2519 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/clients/port/authentication.py
--rw-r--r--   0        0        0     2664 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/clients/port/client.py
--rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/clients/port/mixins/__init__.py
--rw-r--r--   0        0        0     5666 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/clients/port/mixins/entities.py
--rw-r--r--   0        0        0     3085 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/clients/port/mixins/integrations.py
--rw-r--r--   0        0        0      593 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/clients/port/types.py
--rw-r--r--   0        0        0      142 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/clients/port/utils.py
--rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/config/__init__.py
--rw-r--r--   0        0        0     2277 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/config/base.py
--rw-r--r--   0        0        0     1053 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/config/dynamic.py
--rw-r--r--   0        0        0      966 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/config/integration.py
--rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/consumers/__init__.py
--rw-r--r--   0        0        0      125 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/consumers/base_consumer.py
--rw-r--r--   0        0        0     4058 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/consumers/kafka_consumer.py
--rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/context/__init__.py
--rw-r--r--   0        0        0     3201 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/context/event.py
--rw-r--r--   0        0        0     4044 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/context/ocean.py
--rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/__init__.py
--rw-r--r--   0        0        0      219 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/base.py
--rw-r--r--   0        0        0      593 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/event_listener/__init__.py
--rw-r--r--   0        0        0      560 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/event_listener/base.py
--rw-r--r--   0        0        0     3083 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/event_listener/factory.py
--rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/event_listener/http/__init__.py
--rw-r--r--   0        0        0     1197 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/event_listener/http/event_listener.py
--rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/event_listener/kafka/__init__.py
--rw-r--r--   0        0        0     3123 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/event_listener/kafka/event_listener.py
--rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/event_listener/sample/__init__.py
--rw-r--r--   0        0        0     1852 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/event_listener/sample/event_listener.py
--rw-r--r--   0        0        0     2799 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/event_listener/sample/utils.py
--rw-r--r--   0        0        0      716 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/__init__.py
--rw-r--r--   0        0        0      863 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/base.py
--rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/port/__init__.py
--rw-r--r--   0        0        0     7855 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/port/applier.py
--rw-r--r--   0        0        0     1339 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
--rw-r--r--   0        0        0      988 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
--rw-r--r--   0        0        0     1392 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
--rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/entity_processor/__init__.py
--rw-r--r--   0        0        0      949 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/entity_processor/base.py
--rw-r--r--   0        0        0     2679 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
--rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/port_app_config/__init__.py
--rw-r--r--   0        0        0      396 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/port_app_config/api.py
--rw-r--r--   0        0        0      651 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/port_app_config/base.py
--rw-r--r--   0        0        0     1432 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/port_app_config/models.py
--rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/integrations/__init__.py
--rw-r--r--   0        0        0     1966 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/integrations/base.py
--rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/integrations/mixins/__init__.py
--rw-r--r--   0        0        0      692 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/integrations/mixins/events.py
--rw-r--r--   0        0        0     2706 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/integrations/mixins/handler.py
--rw-r--r--   0        0        0    11343 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/integrations/mixins/sync.py
--rw-r--r--   0        0        0      588 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/models.py
--rw-r--r--   0        0        0      563 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/types.py
--rw-r--r--   0        0        0     1916 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/utils.py
--rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/exceptions/__init__.py
--rw-r--r--   0        0        0      426 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/exceptions/api.py
--rw-r--r--   0        0        0       46 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/exceptions/base.py
--rw-r--r--   0        0        0      180 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/exceptions/clients.py
--rw-r--r--   0        0        0      235 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/exceptions/context.py
--rw-r--r--   0        0        0      532 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/exceptions/core.py
--rw-r--r--   0        0        0      670 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/logger_setup.py
--rw-r--r--   0        0        0     2475 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/middlewares.py
--rw-r--r--   0        0        0     4220 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/ocean.py
--rw-r--r--   0        0        0     1007 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/utils.py
--rw-r--r--   0        0        0     2741 2023-07-17 09:45:56.539705 port_ocean-0.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     6202 1970-01-01 00:00:00.000000 port_ocean-0.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-18 13:16:05.239473 port_ocean-0.1.0rc2/LICENSE
+-rw-r--r--   0        0        0     4585 2023-07-18 13:16:05.239473 port_ocean-0.1.0rc2/README.md
+-rw-r--r--   0        0        0      255 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/__init__.py
+-rw-r--r--   0        0        0      321 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/__init__.py
+-rw-r--r--   0        0        0       57 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/cli.py
+-rw-r--r--   0        0        0     5561 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/commands.py
+-rw-r--r--   0        0        0      429 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/cookiecutter.json
+-rw-r--r--   0        0        0       42 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
+-rw-r--r--   0        0        0     2698 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
+-rw-r--r--   0        0        0       12 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/defaults/.gitignore
+-rw-r--r--   0        0        0       12 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
+-rw-r--r--   0        0        0      388 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
+-rw-r--r--   0        0        0      598 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
+-rw-r--r--   0        0        0     1680 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
+-rw-r--r--   0        0        0      653 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
+-rw-r--r--   0        0        0       12 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog_fragments/.gitignore
+-rw-r--r--   0        0        0      778 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
+-rw-r--r--   0        0        0       65 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
+-rw-r--r--   0        0        0     1669 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
+-rw-r--r--   0        0        0       46 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
+-rw-r--r--   0        0        0     1302 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0     1755 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/download_git_folder.py
+-rw-r--r--   0        0        0      722 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/cli/list_integrations.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/clients/port/__init__.py
+-rw-r--r--   0        0        0     2519 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/clients/port/authentication.py
+-rw-r--r--   0        0        0     2398 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/clients/port/client.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/clients/port/mixins/__init__.py
+-rw-r--r--   0        0        0     3049 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/clients/port/mixins/blueprints.py
+-rw-r--r--   0        0        0     5681 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/clients/port/mixins/entities.py
+-rw-r--r--   0        0        0     3866 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/clients/port/mixins/integrations.py
+-rw-r--r--   0        0        0      593 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/clients/port/types.py
+-rw-r--r--   0        0        0      142 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/clients/port/utils.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:16:05.263473 port_ocean-0.1.0rc2/port_ocean/config/__init__.py
+-rw-r--r--   0        0        0     2277 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/config/base.py
+-rw-r--r--   0        0        0     1053 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/config/dynamic.py
+-rw-r--r--   0        0        0     1116 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/config/integration.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/consumers/__init__.py
+-rw-r--r--   0        0        0      125 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/consumers/base_consumer.py
+-rw-r--r--   0        0        0     4058 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/consumers/kafka_consumer.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/context/__init__.py
+-rw-r--r--   0        0        0     3201 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/context/event.py
+-rw-r--r--   0        0        0     4050 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/context/ocean.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/__init__.py
+-rw-r--r--   0        0        0      219 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/base.py
+-rw-r--r--   0        0        0      593 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/event_listener/__init__.py
+-rw-r--r--   0        0        0      560 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/event_listener/base.py
+-rw-r--r--   0        0        0     3083 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/event_listener/factory.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/event_listener/http/__init__.py
+-rw-r--r--   0        0        0     1197 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/event_listener/http/event_listener.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/event_listener/kafka/__init__.py
+-rw-r--r--   0        0        0     3123 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/event_listener/kafka/event_listener.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/event_listener/sample/__init__.py
+-rw-r--r--   0        0        0     1852 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/event_listener/sample/event_listener.py
+-rw-r--r--   0        0        0     2799 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/event_listener/sample/utils.py
+-rw-r--r--   0        0        0      716 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/handlers/entities_state_applier/__init__.py
+-rw-r--r--   0        0        0      863 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/handlers/entities_state_applier/base.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/handlers/entities_state_applier/port/__init__.py
+-rw-r--r--   0        0        0     7855 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/handlers/entities_state_applier/port/applier.py
+-rw-r--r--   0        0        0     1339 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
+-rw-r--r--   0        0        0      988 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
+-rw-r--r--   0        0        0     1392 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/handlers/entity_processor/__init__.py
+-rw-r--r--   0        0        0      949 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/handlers/entity_processor/base.py
+-rw-r--r--   0        0        0     2679 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/handlers/port_app_config/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/handlers/port_app_config/api.py
+-rw-r--r--   0        0        0      651 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/handlers/port_app_config/base.py
+-rw-r--r--   0        0        0     1810 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/handlers/port_app_config/models.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/integrations/__init__.py
+-rw-r--r--   0        0        0     1912 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/integrations/mixins/__init__.py
+-rw-r--r--   0        0        0      692 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/integrations/mixins/events.py
+-rw-r--r--   0        0        0     2569 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/integrations/mixins/handler.py
+-rw-r--r--   0        0        0    11343 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/integrations/mixins/sync.py
+-rw-r--r--   0        0        0      588 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/models.py
+-rw-r--r--   0        0        0      563 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/types.py
+-rw-r--r--   0        0        0     1916 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/core/utils.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/exceptions/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/exceptions/api.py
+-rw-r--r--   0        0        0       46 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/exceptions/base.py
+-rw-r--r--   0        0        0      180 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/exceptions/clients.py
+-rw-r--r--   0        0        0      235 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/exceptions/context.py
+-rw-r--r--   0        0        0      532 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/exceptions/core.py
+-rw-r--r--   0        0        0      407 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/exceptions/port_defaults.py
+-rw-r--r--   0        0        0      554 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/logger_setup.py
+-rw-r--r--   0        0        0     2475 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/middlewares.py
+-rw-r--r--   0        0        0     2266 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/ocean.py
+-rw-r--r--   0        0        0     7212 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/port_defaults.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/py.typed
+-rw-r--r--   0        0        0     2837 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/run.py
+-rw-r--r--   0        0        0     1007 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/port_ocean/utils.py
+-rw-r--r--   0        0        0     2735 2023-07-18 13:16:05.267473 port_ocean-0.1.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     6204 1970-01-01 00:00:00.000000 port_ocean-0.1.0rc2/PKG-INFO
```

### Comparing `port_ocean-0.1.0rc1/LICENSE` & `port_ocean-0.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/README.md` & `port_ocean-0.1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/cli/commands.py` & `port_ocean-0.1.0rc2/port_ocean/cli/commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from rich.console import Console
 
 from port_ocean import __version__
 from port_ocean.cli.download_git_folder import download_github_folder
 from port_ocean.cli.list_integrations import list_git_folders
 from port_ocean.config.integration import LogLevelType
 
-CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 console = Console()
 
 
 def print_logo() -> None:
     ascii_art = """
 =====================================================================================
           ::::::::       ::::::::       ::::::::::           :::        ::::    ::: 
@@ -29,15 +28,15 @@
 By: Port.io
 """
 
     # Display ASCII art
     Console().print(ascii_art.strip())
 
 
-@click.group(context_settings=CONTEXT_SETTINGS)
+@click.group
 def cli_start() -> None:
     # Ocean root command
     pass
 
 
 @cli_start.command()
 @click.option(
@@ -64,30 +63,52 @@
 @click.option(
     "-l",
     "--log-level",
     "log_level",
     type=click.Choice(["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]),
     default="DEBUG",
     help="""Set the logging level for the integration.
-Supported levels are DEBUG, INFO, WARNING, ERROR,
-and CRITICAL. If not specified, the default level
-is DEBUG.""",
+            Supported levels are DEBUG, INFO, WARNING, ERROR,
+            and CRITICAL. If not specified, the default level
+            is DEBUG.""",
 )
-def sail(path: str, log_level: LogLevelType) -> None:
+@click.option(
+    "-p",
+    "--port",
+    "port",
+    type=int,
+    default=8000,
+    help="""Set the port for the integration to run on.
+            If not specified, the default port is 8000.""",
+)
+@click.option(
+    "-i",
+    "--initialize-port-resources",
+    "initialize_port_resources",
+    type=bool,
+    help="""Set to true to create default resources on installation.
+            If not specified, the default value is false.""",
+)
+def sail(
+    path: str,
+    log_level: LogLevelType,
+    port: int,
+    initialize_port_resources: bool | None,
+) -> None:
     """
     Runs the integration in the given PATH. if no PATH is provided, the current directory will be used.
 
     PATH: Path to the integration.
     """
-    from port_ocean.ocean import run
+    from port_ocean import run
 
     print_logo()
 
     console.print("Setting sail... ⛵️⚓️⛵️⚓️ All hands on deck! ⚓️")
-    run(path, log_level)
+    run(path, log_level, port, initialize_port_resources)
 
 
 @cli_start.command()
 @click.argument("path", default=".", type=click.Path(exists=True))
 def new(path: str) -> None:
     """
     Scaffold a new integration in the given PATH.
```

### Comparing `port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore` & `port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile` & `port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md` & `port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml` & `port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py` & `port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml` & `port_ocean-0.1.0rc2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "{{cookiecutter.integration_name}}"
 version = "0.1.0"
 description = "{{cookiecutter.integration_short_description}}"
 authors = ["{{cookiecutter.full_name}} <{{cookiecutter.email}}>"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-port_ocean = { version = "^0.1.0.dev3", extras = ["cli"] }
+port_ocean = { version = "^0.1.0", extras = ["cli"] }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2"
 black = "^23.3.0"
 mypy = "^1.3.0"
 pylint = "^2.17.4"
 towncrier = "^23.6.0"
@@ -20,14 +20,18 @@
 filename = "CHANGELOG.md"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.mypy]
+exclude = [
+    'venv',
+    '.venv',
+]
 plugins = [
     "pydantic.mypy"
 ]
 
 follow_imports = "silent"
 warn_redundant_casts = true
 warn_unused_ignores = true
@@ -59,8 +63,8 @@
   \.toml
   |\.sh
   |\.git
   |\.ini
   |\.venv
   |Dockerfile
 )/
-'''
+'''
```

### Comparing `port_ocean-0.1.0rc1/port_ocean/cli/download_git_folder.py` & `port_ocean-0.1.0rc2/port_ocean/cli/download_git_folder.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/cli/list_integrations.py` & `port_ocean-0.1.0rc2/port_ocean/cli/list_integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/clients/port/authentication.py` & `port_ocean-0.1.0rc2/port_ocean/clients/port/authentication.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/clients/port/client.py` & `port_ocean-0.1.0rc2/port_ocean/clients/port/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import httpx as httpx
 from loguru import logger
 
 from port_ocean.clients.port.authentication import PortAuthentication
+from port_ocean.clients.port.mixins.blueprints import BlueprintClientMixin
 from port_ocean.clients.port.mixins.entities import EntityClientMixin
 from port_ocean.clients.port.mixins.integrations import IntegrationClientMixin
 from port_ocean.clients.port.types import (
     KafkaCreds,
 )
 from port_ocean.clients.port.utils import handle_status_code
-from port_ocean.core.models import Blueprint
 from port_ocean.exceptions.clients import KafkaCredentialsNotFound
 
 
-class PortClient(EntityClientMixin, IntegrationClientMixin):
+class PortClient(EntityClientMixin, IntegrationClientMixin, BlueprintClientMixin):
     def __init__(
         self,
         base_url: str,
         client_id: str,
         client_secret: str,
         integration_identifier: str,
         integration_type: str,
@@ -31,14 +31,15 @@
             integration_identifier,
             integration_type,
         )
         EntityClientMixin.__init__(self, self.auth, self.client)
         IntegrationClientMixin.__init__(
             self, integration_identifier, self.auth, self.client
         )
+        BlueprintClientMixin.__init__(self, self.auth, self.client)
 
     async def get_kafka_creds(self, silent: bool = False) -> KafkaCreds:
         logger.info("Fetching organization kafka credentials")
         response = await self.client.get(
             f"{self.api_url}/kafka-credentials", headers=await self.auth.headers()
         )
         if response.is_error:
@@ -59,16 +60,7 @@
             f"{self.api_url}/organization", headers=await self.auth.headers()
         )
         if response.is_error:
             logger.error(f"Error getting organization id, error: {response.text}")
             response.raise_for_status()
 
         return response.json()["organization"]["id"]
-
-    async def get_blueprint(self, identifier: str) -> Blueprint:
-        logger.info(f"Fetching blueprint with id: {identifier}")
-        response = await self.client.get(
-            f"{self.api_url}/blueprints/{identifier}",
-            headers=await self.auth.headers(),
-        )
-        response.raise_for_status()
-        return Blueprint.parse_obj(response.json()["blueprint"])
```

### Comparing `port_ocean-0.1.0rc1/port_ocean/clients/port/mixins/entities.py` & `port_ocean-0.1.0rc2/port_ocean/clients/port/mixins/entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         logger.info(
             f"{'Validating' if validation_only else 'Upserting'} entity: {entity.identifier} of blueprint: {entity.blueprint}"
         )
         headers = await self.auth.headers(user_agent_type)
 
         response = await self.client.post(
             f"{self.auth.api_url}/blueprints/{entity.blueprint}/entities",
-            json=entity.dict(exclude_unset=True),
+            json=entity.dict(exclude_unset=True, by_alias=True),
             headers=headers,
             params={
                 "upsert": "true",
                 "merge": str(request_options.get("merge", False)).lower(),
                 "create_missing_related_entities": str(
                     request_options.get("create_missing_related_entities", False)
                 ).lower(),
```

### Comparing `port_ocean-0.1.0rc1/port_ocean/clients/port/types.py` & `port_ocean-0.1.0rc2/port_ocean/clients/port/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/config/base.py` & `port_ocean-0.1.0rc2/port_ocean/config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/config/dynamic.py` & `port_ocean-0.1.0rc2/port_ocean/config/dynamic.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/config/integration.py` & `port_ocean-0.1.0rc2/port_ocean/config/integration.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Literal
 
-from pydantic import BaseModel, Field, BaseSettings
+from pydantic import Field, BaseSettings
 
 from port_ocean.config.base import BaseOceanSettings
 from port_ocean.core.event_listener import EventListenerSettingsType
 
 
 class PortSettings(BaseSettings):
     client_id: str = Field(alias="clientId")
@@ -18,16 +18,22 @@
     config: dict[str, Any]
 
 
 class IntegrationConfiguration(BaseOceanSettings):
     port: PortSettings
     event_listener: EventListenerSettingsType = Field(alias="eventListener")
     batch_work_size: int | None = Field(alias="batchWorkSize", default=None)
+    initialize_port_resources: bool = Field(
+        alias="initializePortResources", default=False
+    )
     integration: IntegrationSettings
 
 
 LogLevelType = Literal["ERROR", "WARNING", "INFO", "DEBUG", "CRITICAL"]
 
 
-class LoggerConfiguration(BaseModel):
-    level: LogLevelType = "DEBUG"
-    serialize: bool = False
+class ApplicationSettings(BaseSettings):
+    log_level: LogLevelType = "DEBUG"
+    port: int = 8000
+
+    class Config:
+        env_prefix = "APPLICATION_"
```

### Comparing `port_ocean-0.1.0rc1/port_ocean/consumers/kafka_consumer.py` & `port_ocean-0.1.0rc2/port_ocean/consumers/kafka_consumer.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/context/event.py` & `port_ocean-0.1.0rc2/port_ocean/context/event.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/context/ocean.py` & `port_ocean-0.1.0rc2/port_ocean/context/ocean.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from dataclasses import dataclass
 from typing import Callable, TYPE_CHECKING, Any
 
 from fastapi import APIRouter
 from werkzeug.local import LocalProxy, LocalStack
 
-from port_ocean.clients.port.client import PortClient
 from port_ocean.clients.port.types import UserAgentType
 from port_ocean.core.models import Entity
 from port_ocean.core.types import (
     RESYNC_EVENT_LISTENER,
     START_EVENT_LISTENER,
     RawEntityDiff,
 )
 from port_ocean.exceptions.context import PortOceanContextNotFoundError
 
 if TYPE_CHECKING:
     from port_ocean.config.integration import IntegrationConfiguration
     from port_ocean.core.integrations.base import BaseIntegration
     from port_ocean.ocean import Ocean
+    from port_ocean.clients.port.client import PortClient
 
 
 @dataclass
 class PortOceanContext:
     app: "Ocean"
 
     @property
@@ -37,15 +37,15 @@
         return self.app.integration
 
     @property
     def integration_config(self) -> dict[str, Any]:
         return self.app.config.integration.config
 
     @property
-    def port_client(self) -> PortClient:
+    def port_client(self) -> "PortClient":
         return self.app.port_client
 
     def on_resync(
         self,
         kind: str | None = None,
     ) -> Callable[[RESYNC_EVENT_LISTENER], RESYNC_EVENT_LISTENER]:
         def wrapper(function: RESYNC_EVENT_LISTENER) -> RESYNC_EVENT_LISTENER:
```

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/event_listener/__init__.py` & `port_ocean-0.1.0rc2/port_ocean/core/event_listener/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/event_listener/base.py` & `port_ocean-0.1.0rc2/port_ocean/core/event_listener/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/event_listener/factory.py` & `port_ocean-0.1.0rc2/port_ocean/core/event_listener/factory.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/event_listener/http/event_listener.py` & `port_ocean-0.1.0rc2/port_ocean/core/event_listener/http/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/event_listener/kafka/event_listener.py` & `port_ocean-0.1.0rc2/port_ocean/core/event_listener/kafka/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/event_listener/sample/event_listener.py` & `port_ocean-0.1.0rc2/port_ocean/core/event_listener/sample/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/event_listener/sample/utils.py` & `port_ocean-0.1.0rc2/port_ocean/core/event_listener/sample/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/handlers/__init__.py` & `port_ocean-0.1.0rc2/port_ocean/core/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/base.py` & `port_ocean-0.1.0rc2/port_ocean/core/handlers/entities_state_applier/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/port/applier.py` & `port_ocean-0.1.0rc2/port_ocean/core/handlers/entities_state_applier/port/applier.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py` & `port_ocean-0.1.0rc2/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py` & `port_ocean-0.1.0rc2/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py` & `port_ocean-0.1.0rc2/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/handlers/entity_processor/base.py` & `port_ocean-0.1.0rc2/port_ocean/core/handlers/entity_processor/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/handlers/entity_processor/jq_entity_processor.py` & `port_ocean-0.1.0rc2/port_ocean/core/handlers/entity_processor/jq_entity_processor.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/handlers/port_app_config/base.py` & `port_ocean-0.1.0rc2/port_ocean/core/handlers/port_app_config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/handlers/port_app_config/models.py` & `port_ocean-0.1.0rc2/port_ocean/core/handlers/port_app_config/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from typing import Optional
+from typing import Optional, Any
 
-from port_ocean.clients.port.types import RequestOptions
 from pydantic import BaseModel, Field
 
+from port_ocean.clients.port.types import RequestOptions
+
 
 class EntityMapping(BaseModel):
     identifier: str
     title: str | None
     blueprint: str
     properties: dict[str, str] = Field(default_factory=dict)
     relations: dict[str, str] = Field(default_factory=dict)
@@ -41,10 +42,18 @@
     def get_port_request_options(self) -> RequestOptions:
         return {
             "delete_dependent_entities": self.delete_dependent_entities,
             "create_missing_related_entities": self.create_missing_related_entities,
             "merge": self.enable_merge_entity,
         }
 
+    def to_request(self) -> dict[str, Any]:
+        return {
+            "deleteDependentEntities": self.delete_dependent_entities,
+            "createMissingRelatedEntities": self.create_missing_related_entities,
+            "enableMergeEntity": self.enable_merge_entity,
+            "resources": [resource.dict(by_alias=True) for resource in self.resources],
+        }
+
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
```

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/integrations/base.py` & `port_ocean-0.1.0rc2/port_ocean/core/integrations/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,16 +36,15 @@
             and self.__class__._on_resync == BaseIntegration._on_resync
         ):
             raise NotImplementedError("on_resync is not implemented")
 
         await self.initialize_handlers()
 
         logger.info("Initializing integration at port")
-        await self.context.port_client.initiate_integration(
-            self.context.config.integration.identifier,
+        await self.context.port_client.initialize_integration(
             self.context.config.integration.type,
             self.context.config.event_listener.to_request(),
         )
 
         self.started = True
 
         async with event_context(EventType.START, trigger_type="machine"):
```

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/integrations/mixins/events.py` & `port_ocean-0.1.0rc2/port_ocean/core/integrations/mixins/events.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/integrations/mixins/handler.py` & `port_ocean-0.1.0rc2/port_ocean/core/integrations/mixins/handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,29 @@
-from typing import Callable
+from typing import Type
 
 from loguru import logger
 
-from port_ocean.context.ocean import PortOceanContext, ocean
+from port_ocean.context.ocean import ocean
 from port_ocean.core.handlers import (
     BaseEntityProcessor,
     BasePortAppConfig,
     BaseEntitiesStateApplier,
     HttpEntitiesStateApplier,
     JQEntityProcessor,
     APIPortAppConfig,
 )
-
 from port_ocean.exceptions.core import IntegrationNotStartedException
 
 
 class HandlerMixin:
-    EntityProcessorClass: Callable[
-        [PortOceanContext], BaseEntityProcessor
-    ] = JQEntityProcessor
-
-    AppConfigHandlerClass: Callable[
-        [PortOceanContext], BasePortAppConfig
-    ] = APIPortAppConfig
-
-    EntitiesStateApplierClass: Callable[
-        [PortOceanContext], BaseEntitiesStateApplier
-    ] = HttpEntitiesStateApplier
+    EntityProcessorClass: Type[BaseEntityProcessor] = JQEntityProcessor
+
+    AppConfigHandlerClass: Type[BasePortAppConfig] = APIPortAppConfig
+
+    EntitiesStateApplierClass: Type[BaseEntitiesStateApplier] = HttpEntitiesStateApplier
 
     def __init__(self) -> None:
         self._entity_processor: BaseEntityProcessor | None = None
         self._port_app_config_handler: BasePortAppConfig | None = None
         self._entities_state_applier: BaseEntitiesStateApplier | None = None
 
     @property
```

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/integrations/mixins/sync.py` & `port_ocean-0.1.0rc2/port_ocean/core/integrations/mixins/sync.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/models.py` & `port_ocean-0.1.0rc2/port_ocean/core/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/types.py` & `port_ocean-0.1.0rc2/port_ocean/core/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/core/utils.py` & `port_ocean-0.1.0rc2/port_ocean/core/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/exceptions/core.py` & `port_ocean-0.1.0rc2/port_ocean/exceptions/core.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/middlewares.py` & `port_ocean-0.1.0rc2/port_ocean/middlewares.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/port_ocean/ocean.py` & `port_ocean-0.1.0rc2/port_ocean/clients/port/mixins/integrations.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,119 +1,108 @@
-import sys
-from importlib.util import spec_from_file_location, module_from_spec
-from inspect import getmembers, isclass
-from types import ModuleType
-from typing import Type, Callable
+from typing import Any, TYPE_CHECKING, Optional
 
-import uvicorn
-from fastapi import FastAPI, APIRouter
+import httpx
 from loguru import logger
-from pydantic import BaseModel
-from starlette.types import Scope, Receive, Send
+from starlette import status
 
-from port_ocean.clients.port.client import PortClient
-from port_ocean.config.dynamic import default_config_factory
-from port_ocean.config.integration import IntegrationConfiguration, LogLevelType
-from port_ocean.context.ocean import (
-    PortOceanContext,
-    ocean,
-    initialize_port_ocean_context,
-)
-from port_ocean.core.integrations.base import BaseIntegration
-from port_ocean.logger_setup import setup_logger
-from port_ocean.middlewares import request_handler
-from port_ocean.utils import get_spec_file
-
-
-def _get_base_integration_class_from_module(
-    module: ModuleType,
-) -> Type[BaseIntegration]:
-    for name, obj in getmembers(module):
-        if (
-            isclass(obj)
-            and type(obj) == type
-            and issubclass(obj, BaseIntegration)
-            and obj != BaseIntegration
-        ):
-            return obj
-
-    raise Exception(f"Failed to load integration from module: {module.__name__}")
-
-
-def _load_module(file_path: str) -> ModuleType:
-    spec = spec_from_file_location("module_name", file_path)
-    if spec is None or spec.loader is None:
-        raise Exception(f"Failed to load integration from path: {file_path}")
+from port_ocean.clients.port.authentication import PortAuthentication
 
-    module = module_from_spec(spec)
-    spec.loader.exec_module(module)
+if TYPE_CHECKING:
+    from port_ocean.core.handlers.port_app_config.models import PortAppConfig
 
-    return module
 
-
-class Ocean:
+class IntegrationClientMixin:
     def __init__(
         self,
-        app: FastAPI | None = None,
-        integration_class: Callable[[PortOceanContext], BaseIntegration] | None = None,
-        integration_router: APIRouter | None = None,
-        config_factory: Callable[..., BaseModel] | None = None,
+        integration_identifier: str,
+        auth: PortAuthentication,
+        client: httpx.AsyncClient,
     ):
-        initialize_port_ocean_context(self)
-        self.fast_api_app = app or FastAPI()
-        self.fast_api_app.middleware("http")(request_handler)
-
-        self.config = IntegrationConfiguration(base_path="./")
-        if config_factory:
-            self.config.integration.config = config_factory(
-                **self.config.integration.config
-            ).dict()
-        self.integration_router = integration_router or APIRouter()
-
-        self.port_client = PortClient(
-            base_url=self.config.port.base_url,
-            client_id=self.config.port.client_id,
-            client_secret=self.config.port.client_secret,
-            integration_identifier=self.config.integration.identifier,
-            integration_type=self.config.integration.type,
+        self.integration_identifier = integration_identifier
+        self.auth = auth
+        self.client = client
+
+    async def get_current_integration(self) -> dict[str, Any]:
+        logger.info(f"Fetching integration with id: {self.integration_identifier}")
+        response = await self.client.get(
+            f"{self.auth.api_url}/integration/{self.integration_identifier}",
+            headers=await self.auth.headers(),
         )
-        self.integration = (
-            integration_class(ocean) if integration_class else BaseIntegration(ocean)
+        response.raise_for_status()
+        return response.json()["integration"]
+
+    async def create_integration(
+        self,
+        _type: str,
+        changelog_destination: dict[str, Any],
+        port_app_config: Optional["PortAppConfig"] = None,
+    ) -> None:
+        logger.info(f"Creating integration with id: {self.integration_identifier}")
+        headers = await self.auth.headers()
+        json = {
+            "installationId": self.integration_identifier,
+            "installationAppType": _type,
+            "changelogDestination": changelog_destination,
+        }
+        if port_app_config:
+            json["config"] = port_app_config.to_request()
+        response = await self.client.post(
+            f"{self.auth.api_url}/integration", headers=headers, json=json
         )
+        response.raise_for_status()
 
-    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
-        self.fast_api_app.include_router(self.integration_router, prefix="/integration")
+    async def patch_integration(
+        self,
+        _type: str | None = None,
+        changelog_destination: dict[str, Any] | None = None,
+        port_app_config: Optional["PortAppConfig"] = None,
+    ) -> None:
+        logger.info(f"Updating integration with id: {self.integration_identifier}")
+        headers = await self.auth.headers()
+        json = {}
+        if _type:
+            json["installationAppType"] = _type
+        if changelog_destination:
+            json["changelogDestination"] = changelog_destination
+        if port_app_config:
+            json["config"] = port_app_config.to_request()
+
+        response = await self.client.patch(
+            f"{self.auth.api_url}/integration/{self.integration_identifier}",
+            headers=headers,
+            json=json,
+        )
+        response.raise_for_status()
 
-        @self.fast_api_app.on_event("startup")
-        async def startup() -> None:
-            try:
-                await self.integration.start()
-            except Exception as e:
-                logger.error(f"Failed to start integration with error: {e}")
-                sys.exit("Server stopped")
-
-        await self.fast_api_app(scope, receive, send)
-
-
-def run(path: str = ".", log_level: LogLevelType = "DEBUG") -> None:
-    setup_logger(log_level)
-    sys.path.append(".")
-    try:
-        integration_path = f"{path}/integration.py" if path else "integration.py"
-        module = _load_module(integration_path)
-        integration_class = _get_base_integration_class_from_module(module)
-    except Exception:
-        integration_class = None
-
-    spec = get_spec_file()
-    config_factory = None
-    if spec is not None:
-        config_factory = default_config_factory(spec.get("configurations", []))
-    default_app = Ocean(
-        integration_class=integration_class, config_factory=config_factory
-    )
-
-    main_path = f"{path}/main.py" if path else "main.py"
-    app_module = _load_module(main_path)
-    app = {name: item for name, item in getmembers(app_module)}.get("app", default_app)
+    async def initialize_integration(
+        self,
+        _type: str,
+        changelog_destination: dict[str, Any],
+        port_app_config: Optional["PortAppConfig"] = None,
+    ) -> None:
+        logger.info(f"Initiating integration with id: {self.integration_identifier}")
+        try:
+            integration = await self.get_current_integration()
+
+            logger.info("Checking for diff in integration configuration")
+            if (
+                integration["changelogDestination"] != changelog_destination
+                or integration["installationAppType"] != _type
+            ):
+                await self.patch_integration(
+                    _type, changelog_destination, port_app_config
+                )
+        except httpx.HTTPStatusError as e:
+            if e.response.status_code == status.HTTP_404_NOT_FOUND:
+                await self.create_integration(
+                    _type, changelog_destination, port_app_config
+                )
+                return
+
+            logger.error(
+                f"Error initiating integration with id: {self.integration_identifier}, error: {e.response.text}"
+            )
+            raise
 
-    uvicorn.run(app, host="0.0.0.0", port=8000)
+        logger.info(
+            f"Integration with id: {self.integration_identifier} successfully registered"
+        )
```

### Comparing `port_ocean-0.1.0rc1/port_ocean/utils.py` & `port_ocean-0.1.0rc2/port_ocean/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc1/pyproject.toml` & `port_ocean-0.1.0rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "port-ocean"
-version = "0.1.0.rc1"
+version = "0.1.0.rc2"
 description = "Port Ocean is a CLI tool for managing your Port projects."
 readme = "README.md"
 homepage = "https://app.getport.io"
 repository = "https://github.com/port-labs/Port-Ocean"
 
 authors = ["Daniel Sinai <daniel@getport.io>", "Yair Siman-Tov <yair@getport.io>"]
 packages = [
@@ -36,38 +36,38 @@
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^1.10.8"
 loguru = "^0.7.0"
 pyyaml = "^6.0"
 werkzeug = "^2.3.4"
-fastapi = "^0.96.0"
+fastapi = "^0.100.0"
 uvicorn = "^0.22.0"
 confluent-kafka = "^2.1.1"
 httpx = "^0.24.1"
 pyjq = "^2.6.0"
 urllib3 = "^1.26.16"
 six = "^1.16.0"
 
 # CLI
 click = { version = "^8.1.3", optional = true }
 rich = { version = "^13.4.1", optional = true }
 cookiecutter = { version = "^2.1.1", optional = true }
 
 [tool.poetry.extras]
-cli = ["click", "rich", "cookiecutter", "toml"]
+cli = ["click", "rich", "cookiecutter"]
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2"
 black = "^23.3.0"
 mypy = "^1.3.0"
 pylint = "^2.17.4"
 types-pyyaml = "^6.0.12.10"
-ruff = "^0.0.272"
+ruff = "^0.0.278"
 types-toml = "^0.10.8.6"
 towncrier = "^23.6.0"
 
 [tool.towncrier]
 directory = "changelog_fragments"
 filename = "CHANGELOG.md"
 package = "port_ocean"
@@ -116,8 +116,8 @@
   |\.sh
   |\.git
   |\.ini
   |Dockerfile
   |\.venv
   |integrations
 )/
-'''
+'''
```

### Comparing `port_ocean-0.1.0rc1/PKG-INFO` & `port_ocean-0.1.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-ocean
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: Port Ocean is a CLI tool for managing your Port projects.
 Home-page: https://app.getport.io
 Keywords: ocean,port-ocean,port
 Author: Daniel Sinai
 Author-email: daniel@getport.io
 Requires-Python: >=3.11,<4.0
 Classifier: Framework :: FastAPI
@@ -19,15 +19,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Provides-Extra: cli
 Requires-Dist: click (>=8.1.3,<9.0.0) ; extra == "cli"
 Requires-Dist: confluent-kafka (>=2.1.1,<3.0.0)
 Requires-Dist: cookiecutter (>=2.1.1,<3.0.0) ; extra == "cli"
-Requires-Dist: fastapi (>=0.96.0,<0.97.0)
+Requires-Dist: fastapi (>=0.100.0,<0.101.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: pyjq (>=2.6.0,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0) ; extra == "cli"
 Requires-Dist: six (>=1.16.0,<2.0.0)
```

