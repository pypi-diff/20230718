# Comparing `tmp/sym_flow_cli-8.0.2.tar.gz` & `tmp/sym_flow_cli-8.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sym_flow_cli-8.0.2.tar", max compression
+gzip compressed data, was "sym_flow_cli-8.0.3.tar", max compression
```

## Comparing `sym_flow_cli-8.0.2.tar` & `sym_flow_cli-8.0.3.tar`

### file list

```diff
@@ -1,139 +1,139 @@
--rw-r--r--   0        0        0      160 2023-06-08 14:52:57.737688 sym_flow_cli-8.0.2/DESCRIPTION.md
--rw-r--r--   0        0        0     1790 2023-06-08 14:52:59.545685 sym_flow_cli-8.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 14:52:57.737688 sym_flow_cli-8.0.2/sym/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 14:52:57.737688 sym_flow_cli-8.0.2/sym/flow/__init__.py
--rw-r--r--   0        0        0       60 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/__init__.py
--rw-r--r--   0        0        0     4711 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/core/README.md
--rw-r--r--   0        0        0        0 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/core/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/core/connectors/__init__.py
--rw-r--r--   0        0        0      350 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/core/connectors/connectors.tf
--rw-r--r--   0        0        0      689 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/core/connectors/iam_connector.tf
--rw-r--r--   0        0        0      315 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/core/connectors/runtime_connector.tf
--rw-r--r--   0        0        0      467 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/core/connectors/runtime_connector_with_account_id_safelist.tf
--rw-r--r--   0        0        0     1676 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/core/connectors/sso_connector.tf
--rw-r--r--   0        0        0     1268 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/core/environment.tf
--rw-r--r--   0        0        0      232 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/core/environment_with_runtime.tf
--rw-r--r--   0        0        0     1142 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/core/secrets.tf
--rw-r--r--   0        0        0      115 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/core/versions.tf
--rw-r--r--   0        0        0        0 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/__init__.py
--rw-r--r--   0        0        0     1494 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/approval_impl.txt
--rw-r--r--   0        0        0      910 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/approval_only.tf
--rw-r--r--   0        0        0     2985 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/aws_iam.tf
--rw-r--r--   0        0        0     4187 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/aws_lambda.tf
--rw-r--r--   0        0        0     2082 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/aws_sso.tf
--rw-r--r--   0        0        0     1189 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/aws_sso_group_target.tf
--rw-r--r--   0        0        0     1052 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/aws_sso_permission_set_target.tf
--rw-r--r--   0        0        0      450 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/impl.txt
--rw-r--r--   0        0        0     1777 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/lambda_handler.txt
--rw-r--r--   0        0        0     1250 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/lambda_impl.txt
--rw-r--r--   0        0        0     4025 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/okta.tf
--rw-r--r--   0        0        0        0 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/migration/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/migration/v8/__init__.py
--rw-r--r--   0        0        0      679 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/migration/v8/migration_v8.tf
--rw-r--r--   0        0        0        0 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/__init__.py
--rw-r--r--   0        0        0       84 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/bots/__init__.py
--rw-r--r--   0        0        0      775 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/bots/bots.py
--rw-r--r--   0        0        0     1762 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/bots/create.py
--rw-r--r--   0        0        0     1444 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/bots/delete.py
--rw-r--r--   0        0        0     1607 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/bots/delete_identity.py
--rw-r--r--   0        0        0     1922 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/bots/list.py
--rw-r--r--   0        0        0     1665 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/bots/update_identity.py
--rw-r--r--   0        0        0       46 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/config/__init__.py
--rw-r--r--   0        0        0      458 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/config/config.py
--rw-r--r--   0        0        0     1027 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/config/config_get.py
--rw-r--r--   0        0        0      560 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/docs.py
--rw-r--r--   0        0        0       93 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/domains/__init__.py
--rw-r--r--   0        0        0      565 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/domains/add.py
--rw-r--r--   0        0        0      936 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/domains/domains.py
--rw-r--r--   0        0        0     1180 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/domains/list.py
--rw-r--r--   0        0        0      658 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/domains/remove.py
--rw-r--r--   0        0        0     9432 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/generate.py
--rw-r--r--   0        0        0     5120 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/init.py
--rw-r--r--   0        0        0     2110 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/login.py
--rw-r--r--   0        0        0     4578 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/migrate.py
--rw-r--r--   0        0        0       72 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/organization/__init__.py
--rw-r--r--   0        0        0      434 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/organization/organization.py
--rw-r--r--   0        0        0     1635 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/organization/organization_configure_mfa.py
--rw-r--r--   0        0        0       99 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/resources/__init__.py
--rw-r--r--   0        0        0     2316 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/resources/list.py
--rw-r--r--   0        0        0      640 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/resources/resources.py
--rw-r--r--   0        0        0       60 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/services/__init__.py
--rw-r--r--   0        0        0      551 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/services/click/external_id_option.py
--rw-r--r--   0        0        0      805 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/services/click/inquirer_choice.py
--rw-r--r--   0        0        0     1058 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/services/click/service_type_choice.py
--rw-r--r--   0        0        0      728 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/services/click/service_type_option.py
--rw-r--r--   0        0        0      570 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/services/hooks/slack_delete.py
--rw-r--r--   0        0        0      626 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/services/services.py
--rw-r--r--   0        0        0     2221 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/services/services_delete.py
--rw-r--r--   0        0        0      947 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/services/services_list.py
--rw-r--r--   0        0        0     1081 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/services/services_update.py
--rw-r--r--   0        0        0     3845 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/status.py
--rw-r--r--   0        0        0     2802 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/symflow.py
--rw-r--r--   0        0        0       90 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/tokens/__init__.py
--rw-r--r--   0        0        0     2563 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/tokens/issue.py
--rw-r--r--   0        0        0     1711 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/tokens/list.py
--rw-r--r--   0        0        0      589 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/tokens/revoke.py
--rw-r--r--   0        0        0      564 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/tokens/tokens.py
--rw-r--r--   0        0        0       87 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/users/__init__.py
--rw-r--r--   0        0        0     4428 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/users/create.py
--rw-r--r--   0        0        0     1471 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/users/delete.py
--rw-r--r--   0        0        0     1614 2023-06-08 14:52:57.741688 sym_flow_cli-8.0.2/sym/flow/cli/commands/users/delete_identity.py
--rw-r--r--   0        0        0     1207 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/commands/users/list.py
--rw-r--r--   0        0        0     1503 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/commands/users/list_identities.py
--rw-r--r--   0        0        0     1289 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/commands/users/set_role.py
--rw-r--r--   0        0        0     3561 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/commands/users/update.py
--rw-r--r--   0        0        0     1652 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/commands/users/update_identity.py
--rw-r--r--   0        0        0     1501 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/commands/users/update_name.py
--rw-r--r--   0        0        0     1177 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/commands/users/users.py
--rw-r--r--   0        0        0     1448 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/commands/users/utils.py
--rw-r--r--   0        0        0      297 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/commands/version.py
--rw-r--r--   0        0        0     7211 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/errors.py
--rw-r--r--   0        0        0        0 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/__init__.py
--rw-r--r--   0        0        0    10200 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/api.py
--rw-r--r--   0        0        0     5196 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/api_operations.py
--rw-r--r--   0        0        0        0 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/code_generation/__init__.py
--rw-r--r--   0        0        0     1300 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/code_generation/approval_only.py
--rw-r--r--   0        0        0     3812 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/code_generation/aws.py
--rw-r--r--   0        0        0     2978 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/code_generation/aws_iam.py
--rw-r--r--   0        0        0     2704 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/code_generation/aws_lambda.py
--rw-r--r--   0        0        0     9082 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/code_generation/aws_sso.py
--rw-r--r--   0        0        0    10792 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/code_generation/core.py
--rw-r--r--   0        0        0        0 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/code_generation/migration/__init__.py
--rw-r--r--   0        0        0    20689 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/code_generation/migration/migrate.py
--rw-r--r--   0        0        0      460 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/code_generation/migration/moved_block.py
--rw-r--r--   0        0        0     3392 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/code_generation/okta.py
--rw-r--r--   0        0        0       39 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/config/__init__.py
--rw-r--r--   0        0        0     5992 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/config/config.py
--rw-r--r--   0        0        0     1929 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/config/lock.py
--rw-r--r--   0        0        0     1923 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/config/thread_safe_file.py
--rw-r--r--   0        0        0      507 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/constants.py
--rw-r--r--   0        0        0     2178 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/global_options.py
--rw-r--r--   0        0        0     2378 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/identity_operations.py
--rw-r--r--   0        0        0     1469 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/jwt.py
--rw-r--r--   0        0        0        0 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/login/__init__.py
--rw-r--r--   0        0        0     8826 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/login/handler.py
--rw-r--r--   0        0        0     3986 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/login/login_flow.py
--rw-r--r--   0        0        0     1446 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/output.py
--rw-r--r--   0        0        0     1336 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/profile_operations.py
--rw-r--r--   0        0        0     4933 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/rest.py
--rw-r--r--   0        0        0     3025 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/sentry.py
--rw-r--r--   0        0        0     4102 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/terraform.py
--rw-r--r--   0        0        0     2267 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/tracked_command.py
--rw-r--r--   0        0        0     6681 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/users.py
--rw-r--r--   0        0        0     1212 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/utils.py
--rw-r--r--   0        0        0     1972 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/version.py
--rw-r--r--   0        0        0      412 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/helpers/yaml.py
--rw-r--r--   0        0        0      192 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/models/__init__.py
--rw-r--r--   0        0        0      123 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/models/auth.py
--rw-r--r--   0        0        0      206 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/models/organization.py
--rw-r--r--   0        0        0     1105 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/models/resource.py
--rw-r--r--   0        0        0      372 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/models/service.py
--rw-r--r--   0        0        0     3090 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/models/service_type.py
--rw-r--r--   0        0        0      705 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/models/token.py
--rw-r--r--   0        0        0     4814 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/models/user.py
--rw-r--r--   0        0        0      286 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/models/user_type.py
--rw-r--r--   0        0        0      171 2023-06-08 14:52:57.745688 sym_flow_cli-8.0.2/sym/flow/cli/symflow.py
--rw-r--r--   0        0        0       22 2023-06-08 14:52:59.601685 sym_flow_cli-8.0.2/sym/flow/cli/version.py
--rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 sym_flow_cli-8.0.2/setup.py
--rw-r--r--   0        0        0     1440 1970-01-01 00:00:00.000000 sym_flow_cli-8.0.2/PKG-INFO
+-rw-r--r--   0        0        0      160 2023-07-18 21:13:12.760681 sym_flow_cli-8.0.3/DESCRIPTION.md
+-rw-r--r--   0        0        0     1790 2023-07-18 21:13:14.732693 sym_flow_cli-8.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/__init__.py
+-rw-r--r--   0        0        0       60 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/__init__.py
+-rw-r--r--   0        0        0     4711 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/core/README.md
+-rw-r--r--   0        0        0        0 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/core/connectors/__init__.py
+-rw-r--r--   0        0        0      350 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/core/connectors/connectors.tf
+-rw-r--r--   0        0        0      689 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/core/connectors/iam_connector.tf
+-rw-r--r--   0        0        0      315 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/core/connectors/runtime_connector.tf
+-rw-r--r--   0        0        0      467 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/core/connectors/runtime_connector_with_account_id_safelist.tf
+-rw-r--r--   0        0        0     1676 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/core/connectors/sso_connector.tf
+-rw-r--r--   0        0        0     1268 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/core/environment.tf
+-rw-r--r--   0        0        0      232 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/core/environment_with_runtime.tf
+-rw-r--r--   0        0        0     1142 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/core/secrets.tf
+-rw-r--r--   0        0        0      115 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/core/versions.tf
+-rw-r--r--   0        0        0        0 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/__init__.py
+-rw-r--r--   0        0        0     1494 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/approval_impl.txt
+-rw-r--r--   0        0        0      910 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/approval_only.tf
+-rw-r--r--   0        0        0     2985 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/aws_iam.tf
+-rw-r--r--   0        0        0     4187 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/aws_lambda.tf
+-rw-r--r--   0        0        0     2082 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/aws_sso.tf
+-rw-r--r--   0        0        0     1189 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/aws_sso_group_target.tf
+-rw-r--r--   0        0        0     1052 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/aws_sso_permission_set_target.tf
+-rw-r--r--   0        0        0      450 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/impl.txt
+-rw-r--r--   0        0        0     1777 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/lambda_handler.txt
+-rw-r--r--   0        0        0     1250 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/lambda_impl.txt
+-rw-r--r--   0        0        0     4025 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/okta.tf
+-rw-r--r--   0        0        0        0 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/migration/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/migration/v8/__init__.py
+-rw-r--r--   0        0        0      679 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/migration/v8/migration_v8.tf
+-rw-r--r--   0        0        0        0 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/commands/__init__.py
+-rw-r--r--   0        0        0       84 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/commands/bots/__init__.py
+-rw-r--r--   0        0        0      775 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/commands/bots/bots.py
+-rw-r--r--   0        0        0     1762 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/commands/bots/create.py
+-rw-r--r--   0        0        0     1444 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/commands/bots/delete.py
+-rw-r--r--   0        0        0     1607 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/commands/bots/delete_identity.py
+-rw-r--r--   0        0        0     1922 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/commands/bots/list.py
+-rw-r--r--   0        0        0     1665 2023-07-18 21:13:12.764681 sym_flow_cli-8.0.3/sym/flow/cli/commands/bots/update_identity.py
+-rw-r--r--   0        0        0       46 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/config/__init__.py
+-rw-r--r--   0        0        0      458 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/config/config.py
+-rw-r--r--   0        0        0     1027 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/config/config_get.py
+-rw-r--r--   0        0        0      560 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/docs.py
+-rw-r--r--   0        0        0       93 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/domains/__init__.py
+-rw-r--r--   0        0        0      565 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/domains/add.py
+-rw-r--r--   0        0        0      936 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/domains/domains.py
+-rw-r--r--   0        0        0     1180 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/domains/list.py
+-rw-r--r--   0        0        0      658 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/domains/remove.py
+-rw-r--r--   0        0        0     9432 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/generate.py
+-rw-r--r--   0        0        0     5120 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/init.py
+-rw-r--r--   0        0        0     2110 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/login.py
+-rw-r--r--   0        0        0     4578 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/migrate.py
+-rw-r--r--   0        0        0       72 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/organization/__init__.py
+-rw-r--r--   0        0        0      434 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/organization/organization.py
+-rw-r--r--   0        0        0     1635 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/organization/organization_configure_mfa.py
+-rw-r--r--   0        0        0       99 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/resources/__init__.py
+-rw-r--r--   0        0        0     2316 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/resources/list.py
+-rw-r--r--   0        0        0      640 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/resources/resources.py
+-rw-r--r--   0        0        0       60 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/services/__init__.py
+-rw-r--r--   0        0        0      551 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/services/click/external_id_option.py
+-rw-r--r--   0        0        0      805 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/services/click/inquirer_choice.py
+-rw-r--r--   0        0        0     1058 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/services/click/service_type_choice.py
+-rw-r--r--   0        0        0      728 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/services/click/service_type_option.py
+-rw-r--r--   0        0        0      570 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/services/hooks/slack_delete.py
+-rw-r--r--   0        0        0      626 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/services/services.py
+-rw-r--r--   0        0        0     2221 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/services/services_delete.py
+-rw-r--r--   0        0        0      947 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/services/services_list.py
+-rw-r--r--   0        0        0     1081 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/services/services_update.py
+-rw-r--r--   0        0        0     3817 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/status.py
+-rw-r--r--   0        0        0     2802 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/symflow.py
+-rw-r--r--   0        0        0       90 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/tokens/__init__.py
+-rw-r--r--   0        0        0     2563 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/tokens/issue.py
+-rw-r--r--   0        0        0     1711 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/tokens/list.py
+-rw-r--r--   0        0        0      589 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/tokens/revoke.py
+-rw-r--r--   0        0        0      564 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/tokens/tokens.py
+-rw-r--r--   0        0        0       87 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/users/__init__.py
+-rw-r--r--   0        0        0     4428 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/users/create.py
+-rw-r--r--   0        0        0     1471 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/users/delete.py
+-rw-r--r--   0        0        0     1614 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/users/delete_identity.py
+-rw-r--r--   0        0        0     1207 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/users/list.py
+-rw-r--r--   0        0        0     1503 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/users/list_identities.py
+-rw-r--r--   0        0        0     1289 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/users/set_role.py
+-rw-r--r--   0        0        0     3561 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/users/update.py
+-rw-r--r--   0        0        0     1652 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/users/update_identity.py
+-rw-r--r--   0        0        0     1501 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/users/update_name.py
+-rw-r--r--   0        0        0     1177 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/users/users.py
+-rw-r--r--   0        0        0     1448 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/users/utils.py
+-rw-r--r--   0        0        0      297 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/commands/version.py
+-rw-r--r--   0        0        0     7211 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/errors.py
+-rw-r--r--   0        0        0        0 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/helpers/__init__.py
+-rw-r--r--   0        0        0    10871 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/helpers/api.py
+-rw-r--r--   0        0        0     5196 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/helpers/api_operations.py
+-rw-r--r--   0        0        0        0 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/helpers/code_generation/__init__.py
+-rw-r--r--   0        0        0     1300 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/helpers/code_generation/approval_only.py
+-rw-r--r--   0        0        0     3812 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/helpers/code_generation/aws.py
+-rw-r--r--   0        0        0     2978 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/helpers/code_generation/aws_iam.py
+-rw-r--r--   0        0        0     2704 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/helpers/code_generation/aws_lambda.py
+-rw-r--r--   0        0        0     9082 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/helpers/code_generation/aws_sso.py
+-rw-r--r--   0        0        0    10792 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/helpers/code_generation/core.py
+-rw-r--r--   0        0        0        0 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/helpers/code_generation/migration/__init__.py
+-rw-r--r--   0        0        0    20689 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/helpers/code_generation/migration/migrate.py
+-rw-r--r--   0        0        0      460 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/helpers/code_generation/migration/moved_block.py
+-rw-r--r--   0        0        0     3392 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/helpers/code_generation/okta.py
+-rw-r--r--   0        0        0       39 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/helpers/config/__init__.py
+-rw-r--r--   0        0        0     5992 2023-07-18 21:13:12.768681 sym_flow_cli-8.0.3/sym/flow/cli/helpers/config/config.py
+-rw-r--r--   0        0        0     1929 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/helpers/config/lock.py
+-rw-r--r--   0        0        0     1923 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/helpers/config/thread_safe_file.py
+-rw-r--r--   0        0        0      578 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/helpers/constants.py
+-rw-r--r--   0        0        0     2178 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/helpers/global_options.py
+-rw-r--r--   0        0        0     2378 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/helpers/identity_operations.py
+-rw-r--r--   0        0        0     1469 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/helpers/jwt.py
+-rw-r--r--   0        0        0        0 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/helpers/login/__init__.py
+-rw-r--r--   0        0        0     8840 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/helpers/login/handler.py
+-rw-r--r--   0        0        0     3986 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/helpers/login/login_flow.py
+-rw-r--r--   0        0        0     1446 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/helpers/output.py
+-rw-r--r--   0        0        0     1336 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/helpers/profile_operations.py
+-rw-r--r--   0        0        0     4933 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/helpers/rest.py
+-rw-r--r--   0        0        0     3025 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/helpers/sentry.py
+-rw-r--r--   0        0        0     4102 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/helpers/terraform.py
+-rw-r--r--   0        0        0     2267 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/helpers/tracked_command.py
+-rw-r--r--   0        0        0     6681 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/helpers/users.py
+-rw-r--r--   0        0        0     1212 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/helpers/utils.py
+-rw-r--r--   0        0        0     1972 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/helpers/version.py
+-rw-r--r--   0        0        0      412 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/helpers/yaml.py
+-rw-r--r--   0        0        0      192 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/models/__init__.py
+-rw-r--r--   0        0        0      123 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/models/auth.py
+-rw-r--r--   0        0        0      206 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/models/organization.py
+-rw-r--r--   0        0        0     1105 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/models/resource.py
+-rw-r--r--   0        0        0      372 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/models/service.py
+-rw-r--r--   0        0        0     3090 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/models/service_type.py
+-rw-r--r--   0        0        0      705 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/models/token.py
+-rw-r--r--   0        0        0     4814 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/models/user.py
+-rw-r--r--   0        0        0      286 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/models/user_type.py
+-rw-r--r--   0        0        0      171 2023-07-18 21:13:12.772682 sym_flow_cli-8.0.3/sym/flow/cli/symflow.py
+-rw-r--r--   0        0        0       22 2023-07-18 21:13:14.796693 sym_flow_cli-8.0.3/sym/flow/cli/version.py
+-rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 sym_flow_cli-8.0.3/setup.py
+-rw-r--r--   0        0        0     1440 1970-01-01 00:00:00.000000 sym_flow_cli-8.0.3/PKG-INFO
```

### Comparing `sym_flow_cli-8.0.2/pyproject.toml` & `sym_flow_cli-8.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sym-flow-cli"
-version = "8.0.2"
+version = "8.0.3"
 description = "Sym's Official CLI for Implementers"
 authors = ["SymOps, Inc. <pypi@symops.io>"]
 packages = [{ include = "sym" }]
 readme = "DESCRIPTION.md"
 homepage = "https://symops.com/"
 documentation = "https://docs.symops.com/docs/install-sym-flow-cli"
 classifiers = [
```

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/core/README.md` & `sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/core/README.md`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/core/connectors/iam_connector.tf` & `sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/core/connectors/iam_connector.tf`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/core/connectors/sso_connector.tf` & `sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/core/connectors/sso_connector.tf`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/core/environment.tf` & `sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/core/environment.tf`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/core/secrets.tf` & `sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/core/secrets.tf`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/approval_impl.txt` & `sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/approval_impl.txt`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/approval_only.tf` & `sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/approval_only.tf`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/aws_iam.tf` & `sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/aws_iam.tf`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/aws_lambda.tf` & `sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/aws_lambda.tf`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/aws_sso.tf` & `sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/aws_sso.tf`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/aws_sso_group_target.tf` & `sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/aws_sso_group_target.tf`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/aws_sso_permission_set_target.tf` & `sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/aws_sso_permission_set_target.tf`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/lambda_handler.txt` & `sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/lambda_handler.txt`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/lambda_impl.txt` & `sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/lambda_impl.txt`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/flows/okta.tf` & `sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/flows/okta.tf`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/code_generation_templates/migration/v8/migration_v8.tf` & `sym_flow_cli-8.0.3/sym/flow/cli/code_generation_templates/migration/v8/migration_v8.tf`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/bots/bots.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/bots/bots.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/bots/create.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/bots/create.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/bots/delete.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/bots/delete.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/bots/delete_identity.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/bots/delete_identity.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/bots/list.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/bots/list.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/bots/update_identity.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/bots/update_identity.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/config/config_get.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/config/config_get.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/docs.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/docs.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/domains/add.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/domains/add.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/domains/domains.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/domains/domains.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/domains/list.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/domains/list.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/domains/remove.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/domains/remove.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/generate.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/init.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/login.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/migrate.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/organization/organization_configure_mfa.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/organization/organization_configure_mfa.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/resources/list.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/resources/list.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/resources/resources.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/resources/resources.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/services/click/external_id_option.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/services/click/external_id_option.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/services/click/inquirer_choice.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/services/click/inquirer_choice.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/services/click/service_type_choice.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/services/click/service_type_choice.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/services/click/service_type_option.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/services/click/service_type_option.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/services/hooks/slack_delete.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/services/hooks/slack_delete.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/services/services.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/services/services.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/services/services_delete.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/services/services_delete.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/services/services_list.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/services/services_list.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/services/services_update.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/services/services_update.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/status.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/status.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import click
 
 import sym.flow.cli.helpers.output as cli_output
 from sym.flow.cli.errors import SymAPIRequestError
 from sym.flow.cli.helpers.api import SymAPI
 from sym.flow.cli.helpers.config import Config
+from sym.flow.cli.helpers.constants import SERVER_ERROR
 from sym.flow.cli.helpers.global_options import GlobalOptions
 from sym.flow.cli.helpers.tracked_command import TrackedCommand
 
 
 @click.command(cls=TrackedCommand, short_help="Check your stored auth token")
 @click.make_pass_decorator(GlobalOptions, ensure=True)
 def status(options: GlobalOptions) -> None:
@@ -19,15 +20,15 @@
 
 
 def check_status_by_sym_jwt(api: SymAPI):
     """Validate that the environment variable SYM_JWT contains a valid JWT."""
     try:
         user_data = api.verify_login()
     except SymAPIRequestError:
-        cli_output.fail("A server error has occurred, Please try again later.")
+        cli_output.fail(SERVER_ERROR)
 
     if user_data.get("error") and user_data.get("message"):
         if user_data.get("code") == "Authentication:INVALID_JWT":
             # This specific error message is very generic, and the Bot Token has probably just expired.
             cli_output.fail(
                 "Status check failed!",
                 f"  {user_data['message']} Use `symflow tokens list` to make sure your token is still valid.",
@@ -59,15 +60,15 @@
     email = Config.get_email()
 
     try:
         # Check the User's session with the Sym API. This will validate that the JWT is still valid,
         # and matches the email address that the User is logged in with.
         user_data = api.verify_login(email)
     except SymAPIRequestError:
-        cli_output.fail("A server error has occurred, Please try again later.")
+        cli_output.fail(SERVER_ERROR)
 
     if user_data.get("error") and user_data.get("message"):
         if user_data.get("code") == "Authentication:INVALID_JWT":
             # This specific error message is very generic, and the User probably just needs to log in again.
             cli_output.fail("Status check failed!", f"  {user_data['message']} Try running `symflow login`.")
         else:
             cli_output.fail("Status check failed!", f"  {user_data['message']}")
```

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/symflow.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/symflow.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/tokens/issue.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/tokens/issue.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/tokens/list.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/tokens/list.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/tokens/revoke.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/tokens/revoke.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/tokens/tokens.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/tokens/tokens.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/users/create.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/users/create.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/users/delete.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/users/delete.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/users/delete_identity.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/users/delete_identity.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/users/list.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/users/list.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/users/list_identities.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/users/list_identities.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/users/set_role.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/users/set_role.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/users/update.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/users/update.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/users/update_identity.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/users/update_identity.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/users/update_name.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/users/update_name.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/users/users.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/users/users.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/commands/users/utils.py` & `sym_flow_cli-8.0.3/sym/flow/cli/commands/users/utils.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/errors.py` & `sym_flow_cli-8.0.3/sym/flow/cli/errors.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/api.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from json import JSONDecodeError
 from typing import Dict, List, Optional
 from uuid import UUID
 
 from pydantic import parse_obj_as
 
 from sym.flow.cli.errors import (
     SymAPIUnknownError,
@@ -54,20 +55,33 @@
 
     def verify_login(self, email: Optional[str] = None, segment_track: Optional[bool] = False) -> dict:
         """Calls the Sym API to validate that the User's current credentials are valid.
 
         Returns:
             A dictionary containing User data if the credentials were validated, or error information
             if they were not.
+
+        Raises:
+            SymAPIUnknownError: If unable to communicate with the server or did not get a well-formed JSON response body
         """
         response = self.rest.get(
             "auth/login", filter_dict({"email": email, "segment_track": segment_track}), validate=False
         )
 
-        return response.json()
+        if 500 <= response.status_code < 600:  # If a server error has occurred
+            raise SymAPIUnknownError(
+                message=response.text, request_id=self.rest.last_request_id, response_code=response.status_code
+            )
+
+        try:
+            return response.json()
+        except JSONDecodeError:  # If did not get a well-formed JSON body
+            raise SymAPIUnknownError(
+                message=response.text, request_id=self.rest.last_request_id, response_code=response.status_code
+            )
 
     def get_integrations(self) -> List[dict]:
         """Retrieve all Sym Integrations accessible to the currently
         authenticated user.
         """
         return self.rest.get("entities/integrations").json()
```

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/api_operations.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/api_operations.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/code_generation/approval_only.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/code_generation/approval_only.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/code_generation/aws.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/code_generation/aws.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/code_generation/aws_iam.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/code_generation/aws_iam.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/code_generation/aws_lambda.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/code_generation/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/code_generation/aws_sso.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/code_generation/aws_sso.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/code_generation/core.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/code_generation/core.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/code_generation/migration/migrate.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/code_generation/migration/migrate.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/code_generation/okta.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/code_generation/okta.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/config/config.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/config/config.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/config/lock.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/config/lock.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/config/thread_safe_file.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/config/thread_safe_file.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/global_options.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/global_options.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/identity_operations.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/identity_operations.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/jwt.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/jwt.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/login/handler.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/login/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from http.server import BaseHTTPRequestHandler
 
 import requests
 
 import sym.flow.cli.helpers.output as cli_output
 from sym.flow.cli.errors import SymAPIRequestError
 from sym.flow.cli.helpers.config import Config
+from sym.flow.cli.helpers.constants import SERVER_ERROR
 from sym.flow.cli.helpers.global_options import GlobalOptions
 from sym.flow.cli.helpers.jwt import JWT
 from sym.flow.cli.models import AuthToken, Organization
 
 
 def make_auth0_callback_handler(
     options: GlobalOptions, redirect_uri: str, state: str, code_verifier: str, organization: Organization
@@ -158,15 +159,15 @@
 
             # Verify user exists in the organization
             try:
                 # Check the User's session with the Sym API. This will validate that the JWT is still valid,
                 # and matches the email address that the User is logged in with.
                 user_data = options.sym_api.verify_login(segment_track=True)
             except SymAPIRequestError:
-                self._exit_with_error("A server error has occurred, please try again later.")
+                self._exit_with_error(SERVER_ERROR)
 
             if user_data.get("error") and user_data.get("message"):
                 self._exit_with_error(user_data["message"])
             elif user_data.get("error"):
                 # All Sym API errors should have a message field, but just in case...
                 self._exit_with_error(f"{jwt.email} is not a valid user in the Organization {organization.slug}")
```

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/login/login_flow.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/login/login_flow.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/output.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/output.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/profile_operations.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/profile_operations.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/rest.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/rest.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/sentry.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/sentry.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/terraform.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/terraform.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/tracked_command.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/tracked_command.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/users.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/users.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/utils.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/helpers/version.py` & `sym_flow_cli-8.0.3/sym/flow/cli/helpers/version.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/models/resource.py` & `sym_flow_cli-8.0.3/sym/flow/cli/models/resource.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/models/service_type.py` & `sym_flow_cli-8.0.3/sym/flow/cli/models/service_type.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/models/token.py` & `sym_flow_cli-8.0.3/sym/flow/cli/models/token.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/sym/flow/cli/models/user.py` & `sym_flow_cli-8.0.3/sym/flow/cli/models/user.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-8.0.2/setup.py` & `sym_flow_cli-8.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
  'tabulate>=0.8.7,<0.9.0']
 
 entry_points = \
 {'console_scripts': ['symflow = sym.flow.cli.symflow:symflow']}
 
 setup_kwargs = {
     'name': 'sym-flow-cli',
-    'version': '8.0.2',
+    'version': '8.0.3',
     'description': "Sym's Official CLI for Implementers",
     'long_description': '# sym-flow-cli\n\nThis is the official CLI for [Sym](https://symops.com/) Implementers. Check out the docs [here](https://docs.symops.com/docs/install-sym-flow).\n',
     'author': 'SymOps, Inc.',
     'author_email': 'pypi@symops.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://symops.com/',
```

### Comparing `sym_flow_cli-8.0.2/PKG-INFO` & `sym_flow_cli-8.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sym-flow-cli
-Version: 8.0.2
+Version: 8.0.3
 Summary: Sym's Official CLI for Implementers
 Home-page: https://symops.com/
 Author: SymOps, Inc.
 Author-email: pypi@symops.io
 Requires-Python: >=3.8,<4.0
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

