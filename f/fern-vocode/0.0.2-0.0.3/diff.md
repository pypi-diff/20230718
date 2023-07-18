# Comparing `tmp/fern_vocode-0.0.2.tar.gz` & `tmp/fern_vocode-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_vocode-0.0.2.tar", max compression
+gzip compressed data, was "fern_vocode-0.0.3.tar", max compression
```

## Comparing `fern_vocode-0.0.2.tar` & `fern_vocode-0.0.3.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0        0 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/README.md
--rw-r--r--   0        0        0      372 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4436 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/__init__.py
--rw-r--r--   0        0        0     2074 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/client.py
--rw-r--r--   0        0        0      348 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      170 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/errors/__init__.py
--rw-r--r--   0        0        0      313 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/py.typed
--rw-r--r--   0        0        0      220 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/resources/actions/__init__.py
--rw-r--r--   0        0        0     9264 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/resources/actions/client.py
--rw-r--r--   0        0        0       65 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/resources/agents/__init__.py
--rw-r--r--   0        0        0     8720 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/resources/agents/client.py
--rw-r--r--   0        0        0       65 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/resources/calls/__init__.py
--rw-r--r--   0        0        0     8785 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/resources/calls/client.py
--rw-r--r--   0        0        0       65 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/resources/numbers/__init__.py
--rw-r--r--   0        0        0    10652 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/resources/numbers/client.py
--rw-r--r--   0        0        0       65 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/resources/usage/__init__.py
--rw-r--r--   0        0        0     2159 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/resources/usage/client.py
--rw-r--r--   0        0        0       65 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/resources/voices/__init__.py
--rw-r--r--   0        0        0     9214 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/resources/voices/client.py
--rw-r--r--   0        0        0       65 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/resources/webhooks/__init__.py
--rw-r--r--   0        0        0     8808 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/resources/webhooks/client.py
--rw-r--r--   0        0        0     6543 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/__init__.py
--rw-r--r--   0        0        0      731 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/action_config.py
--rw-r--r--   0        0        0      615 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/action_type.py
--rw-r--r--   0        0        0     1045 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/agent.py
--rw-r--r--   0        0        0      248 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/agent_actions_item.py
--rw-r--r--   0        0        0     1096 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/agent_params.py
--rw-r--r--   0        0        0      292 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/agent_params_actions_item.py
--rw-r--r--   0        0        0      332 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/agent_params_voice.py
--rw-r--r--   0        0        0      177 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/agent_params_webhook.py
--rw-r--r--   0        0        0     1360 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/agent_update_params.py
--rw-r--r--   0        0        0      368 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/agent_update_params_actions.py
--rw-r--r--   0        0        0      366 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/agent_update_params_actions_agent_update_params_actions_item.py
--rw-r--r--   0        0        0      177 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/agent_update_params_initial_message.py
--rw-r--r--   0        0        0      169 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/agent_update_params_prompt.py
--rw-r--r--   0        0        0      445 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/agent_update_params_voice.py
--rw-r--r--   0        0        0      246 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/agent_update_params_webhook.py
--rw-r--r--   0        0        0      269 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/agent_voice.py
--rw-r--r--   0        0        0      152 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/agent_webhook.py
--rw-r--r--   0        0        0      913 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/azure_voice.py
--rw-r--r--   0        0        0      873 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/azure_voice_params.py
--rw-r--r--   0        0        0     1197 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/azure_voice_update_params.py
--rw-r--r--   0        0        0      173 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/azure_voice_update_params_pitch.py
--rw-r--r--   0        0        0      172 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/azure_voice_update_params_rate.py
--rw-r--r--   0        0        0      177 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/azure_voice_update_params_voice_name.py
--rw-r--r--   0        0        0     1015 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/call.py
--rw-r--r--   0        0        0      143 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/call_agent.py
--rw-r--r--   0        0        0      832 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/call_status.py
--rw-r--r--   0        0        0      284 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/create_action_request.py
--rw-r--r--   0        0        0      247 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/create_action_response.py
--rw-r--r--   0        0        0      175 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/create_call_request_agent.py
--rw-r--r--   0        0        0      329 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/create_voice_request.py
--rw-r--r--   0        0        0      273 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/create_voice_response.py
--rw-r--r--   0        0        0      915 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/dtmf_action.py
--rw-r--r--   0        0        0      875 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/dtmf_action_params.py
--rw-r--r--   0        0        0      932 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/dtmf_action_update_params.py
--rw-r--r--   0        0        0      223 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/dtmf_action_update_params_config.py
--rw-r--r--   0        0        0      953 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/eleven_labs_voice.py
--rw-r--r--   0        0        0      913 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/eleven_labs_voice_params.py
--rw-r--r--   0        0        0     1455 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/eleven_labs_voice_update_params.py
--rw-r--r--   0        0        0      179 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/eleven_labs_voice_update_params_api_key.py
--rw-r--r--   0        0        0      190 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/eleven_labs_voice_update_params_similarity_boost.py
--rw-r--r--   0        0        0      184 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/eleven_labs_voice_update_params_stability.py
--rw-r--r--   0        0        0      180 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/eleven_labs_voice_update_params_voice_id.py
--rw-r--r--   0        0        0      926 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/end_conversation_action.py
--rw-r--r--   0        0        0      886 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/end_conversation_action_params.py
--rw-r--r--   0        0        0      977 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/end_conversation_action_update_params.py
--rw-r--r--   0        0        0      234 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/end_conversation_action_update_params_config.py
--rw-r--r--   0        0        0     1395 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/event_type.py
--rw-r--r--   0        0        0      244 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/get_action_response.py
--rw-r--r--   0        0        0      270 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/get_voice_response.py
--rw-r--r--   0        0        0      466 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/http_method.py
--rw-r--r--   0        0        0      843 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/http_validation_error.py
--rw-r--r--   0        0        0      250 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/list_actions_response_item.py
--rw-r--r--   0        0        0      276 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/list_voices_response_item.py
--rw-r--r--   0        0        0      900 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/phone_number.py
--rw-r--r--   0        0        0      157 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/phone_number_inbound_agent.py
--rw-r--r--   0        0        0      674 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/plan_type.py
--rw-r--r--   0        0        0      846 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/rime_voice.py
--rw-r--r--   0        0        0      806 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/rime_voice_params.py
--rw-r--r--   0        0        0      929 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/rime_voice_update_params.py
--rw-r--r--   0        0        0      174 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/rime_voice_update_params_speaker.py
--rw-r--r--   0        0        0      728 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/undefined.py
--rw-r--r--   0        0        0      326 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/update_action_request_body.py
--rw-r--r--   0        0        0      247 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/update_action_response.py
--rw-r--r--   0        0        0      203 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/update_number_request_inbound_agent.py
--rw-r--r--   0        0        0      390 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/update_voice_request_body.py
--rw-r--r--   0        0        0      273 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/update_voice_response.py
--rw-r--r--   0        0        0      866 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/usage.py
--rw-r--r--   0        0        0      869 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      907 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/voice_type.py
--rw-r--r--   0        0        0      921 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/webhook.py
--rw-r--r--   0        0        0      898 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/webhook_params.py
--rw-r--r--   0        0        0     1124 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/webhook_update_params.py
--rw-r--r--   0        0        0      214 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/webhook_update_params_method.py
--rw-r--r--   0        0        0      231 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/webhook_update_params_subscriptions.py
--rw-r--r--   0        0        0      168 2023-07-17 23:27:06.355486 fern_vocode-0.0.2/src/vocode/types/webhook_update_params_url.py
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 fern_vocode-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-18 00:31:52.788260 fern_vocode-0.0.3/README.md
+-rw-r--r--   0        0        0      372 2023-07-18 00:31:52.788260 fern_vocode-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4436 2023-07-18 00:31:52.788260 fern_vocode-0.0.3/src/vocode/__init__.py
+-rw-r--r--   0        0        0     2074 2023-07-18 00:31:52.788260 fern_vocode-0.0.3/src/vocode/client.py
+-rw-r--r--   0        0        0      348 2023-07-18 00:31:52.788260 fern_vocode-0.0.3/src/vocode/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-18 00:31:52.788260 fern_vocode-0.0.3/src/vocode/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-07-18 00:31:52.788260 fern_vocode-0.0.3/src/vocode/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-18 00:31:52.788260 fern_vocode-0.0.3/src/vocode/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-18 00:31:52.788260 fern_vocode-0.0.3/src/vocode/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      170 2023-07-18 00:31:52.788260 fern_vocode-0.0.3/src/vocode/errors/__init__.py
+-rw-r--r--   0        0        0      313 2023-07-18 00:31:52.788260 fern_vocode-0.0.3/src/vocode/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-07-18 00:31:52.788260 fern_vocode-0.0.3/src/vocode/py.typed
+-rw-r--r--   0        0        0      220 2023-07-18 00:31:52.788260 fern_vocode-0.0.3/src/vocode/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-18 00:31:52.788260 fern_vocode-0.0.3/src/vocode/resources/actions/__init__.py
+-rw-r--r--   0        0        0     9264 2023-07-18 00:31:52.788260 fern_vocode-0.0.3/src/vocode/resources/actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/resources/agents/__init__.py
+-rw-r--r--   0        0        0     8720 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/resources/agents/client.py
+-rw-r--r--   0        0        0       65 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/resources/calls/__init__.py
+-rw-r--r--   0        0        0     8785 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/resources/calls/client.py
+-rw-r--r--   0        0        0       65 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/resources/numbers/__init__.py
+-rw-r--r--   0        0        0    10652 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/resources/numbers/client.py
+-rw-r--r--   0        0        0       65 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/resources/usage/__init__.py
+-rw-r--r--   0        0        0     2159 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/resources/usage/client.py
+-rw-r--r--   0        0        0       65 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/resources/voices/__init__.py
+-rw-r--r--   0        0        0     9214 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/resources/voices/client.py
+-rw-r--r--   0        0        0       65 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/resources/webhooks/__init__.py
+-rw-r--r--   0        0        0     8808 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/resources/webhooks/client.py
+-rw-r--r--   0        0        0     6543 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/__init__.py
+-rw-r--r--   0        0        0      731 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/action_config.py
+-rw-r--r--   0        0        0      615 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/action_type.py
+-rw-r--r--   0        0        0     1045 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/agent.py
+-rw-r--r--   0        0        0      248 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/agent_actions_item.py
+-rw-r--r--   0        0        0     1096 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/agent_params.py
+-rw-r--r--   0        0        0      292 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/agent_params_actions_item.py
+-rw-r--r--   0        0        0      332 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/agent_params_voice.py
+-rw-r--r--   0        0        0      177 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/agent_params_webhook.py
+-rw-r--r--   0        0        0     1360 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/agent_update_params.py
+-rw-r--r--   0        0        0      368 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/agent_update_params_actions.py
+-rw-r--r--   0        0        0      366 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/agent_update_params_actions_agent_update_params_actions_item.py
+-rw-r--r--   0        0        0      177 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/agent_update_params_initial_message.py
+-rw-r--r--   0        0        0      169 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/agent_update_params_prompt.py
+-rw-r--r--   0        0        0      445 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/agent_update_params_voice.py
+-rw-r--r--   0        0        0      246 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/agent_update_params_webhook.py
+-rw-r--r--   0        0        0      269 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/agent_voice.py
+-rw-r--r--   0        0        0      152 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/agent_webhook.py
+-rw-r--r--   0        0        0      913 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/azure_voice.py
+-rw-r--r--   0        0        0      873 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/azure_voice_params.py
+-rw-r--r--   0        0        0     1197 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/azure_voice_update_params.py
+-rw-r--r--   0        0        0      173 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/azure_voice_update_params_pitch.py
+-rw-r--r--   0        0        0      172 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/azure_voice_update_params_rate.py
+-rw-r--r--   0        0        0      177 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/azure_voice_update_params_voice_name.py
+-rw-r--r--   0        0        0     1015 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/call.py
+-rw-r--r--   0        0        0      143 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/call_agent.py
+-rw-r--r--   0        0        0      832 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/call_status.py
+-rw-r--r--   0        0        0      284 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/create_action_request.py
+-rw-r--r--   0        0        0      247 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/create_action_response.py
+-rw-r--r--   0        0        0      175 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/create_call_request_agent.py
+-rw-r--r--   0        0        0      329 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/create_voice_request.py
+-rw-r--r--   0        0        0      273 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/create_voice_response.py
+-rw-r--r--   0        0        0      915 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/dtmf_action.py
+-rw-r--r--   0        0        0      875 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/dtmf_action_params.py
+-rw-r--r--   0        0        0      932 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/dtmf_action_update_params.py
+-rw-r--r--   0        0        0      223 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/dtmf_action_update_params_config.py
+-rw-r--r--   0        0        0      953 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/eleven_labs_voice.py
+-rw-r--r--   0        0        0      913 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/eleven_labs_voice_params.py
+-rw-r--r--   0        0        0     1455 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/eleven_labs_voice_update_params.py
+-rw-r--r--   0        0        0      179 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/eleven_labs_voice_update_params_api_key.py
+-rw-r--r--   0        0        0      190 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/eleven_labs_voice_update_params_similarity_boost.py
+-rw-r--r--   0        0        0      184 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/eleven_labs_voice_update_params_stability.py
+-rw-r--r--   0        0        0      180 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/eleven_labs_voice_update_params_voice_id.py
+-rw-r--r--   0        0        0      926 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/end_conversation_action.py
+-rw-r--r--   0        0        0      886 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/end_conversation_action_params.py
+-rw-r--r--   0        0        0      977 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/end_conversation_action_update_params.py
+-rw-r--r--   0        0        0      234 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/end_conversation_action_update_params_config.py
+-rw-r--r--   0        0        0     1395 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/event_type.py
+-rw-r--r--   0        0        0      244 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/get_action_response.py
+-rw-r--r--   0        0        0      270 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/get_voice_response.py
+-rw-r--r--   0        0        0      466 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/http_method.py
+-rw-r--r--   0        0        0      843 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/http_validation_error.py
+-rw-r--r--   0        0        0      250 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/list_actions_response_item.py
+-rw-r--r--   0        0        0      276 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/list_voices_response_item.py
+-rw-r--r--   0        0        0      900 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/phone_number.py
+-rw-r--r--   0        0        0      157 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/phone_number_inbound_agent.py
+-rw-r--r--   0        0        0      674 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/plan_type.py
+-rw-r--r--   0        0        0      846 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/rime_voice.py
+-rw-r--r--   0        0        0      806 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/rime_voice_params.py
+-rw-r--r--   0        0        0      929 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/rime_voice_update_params.py
+-rw-r--r--   0        0        0      174 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/rime_voice_update_params_speaker.py
+-rw-r--r--   0        0        0      728 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/undefined.py
+-rw-r--r--   0        0        0      326 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/update_action_request_body.py
+-rw-r--r--   0        0        0      247 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/update_action_response.py
+-rw-r--r--   0        0        0      203 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/update_number_request_inbound_agent.py
+-rw-r--r--   0        0        0      390 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/update_voice_request_body.py
+-rw-r--r--   0        0        0      273 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/update_voice_response.py
+-rw-r--r--   0        0        0      866 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/usage.py
+-rw-r--r--   0        0        0      869 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      907 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/voice_type.py
+-rw-r--r--   0        0        0      921 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/webhook.py
+-rw-r--r--   0        0        0      898 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/webhook_params.py
+-rw-r--r--   0        0        0     1124 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/webhook_update_params.py
+-rw-r--r--   0        0        0      214 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/webhook_update_params_method.py
+-rw-r--r--   0        0        0      231 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/webhook_update_params_subscriptions.py
+-rw-r--r--   0        0        0      168 2023-07-18 00:31:52.792261 fern_vocode-0.0.3/src/vocode/types/webhook_update_params_url.py
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 fern_vocode-0.0.3/PKG-INFO
```

### Comparing `fern_vocode-0.0.2/src/vocode/__init__.py` & `fern_vocode-0.0.3/src/vocode/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/client.py` & `fern_vocode-0.0.3/src/vocode/client.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/core/datetime_utils.py` & `fern_vocode-0.0.3/src/vocode/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/core/jsonable_encoder.py` & `fern_vocode-0.0.3/src/vocode/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/resources/actions/client.py` & `fern_vocode-0.0.3/src/vocode/resources/actions/client.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/resources/agents/client.py` & `fern_vocode-0.0.3/src/vocode/resources/agents/client.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/resources/calls/client.py` & `fern_vocode-0.0.3/src/vocode/resources/calls/client.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/resources/numbers/client.py` & `fern_vocode-0.0.3/src/vocode/resources/numbers/client.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/resources/usage/client.py` & `fern_vocode-0.0.3/src/vocode/resources/usage/client.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/resources/voices/client.py` & `fern_vocode-0.0.3/src/vocode/resources/voices/client.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/resources/webhooks/client.py` & `fern_vocode-0.0.3/src/vocode/resources/webhooks/client.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/__init__.py` & `fern_vocode-0.0.3/src/vocode/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/action_config.py` & `fern_vocode-0.0.3/src/vocode/types/action_config.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/action_type.py` & `fern_vocode-0.0.3/src/vocode/types/action_type.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/agent.py` & `fern_vocode-0.0.3/src/vocode/types/agent.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/agent_params.py` & `fern_vocode-0.0.3/src/vocode/types/agent_params.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/agent_update_params.py` & `fern_vocode-0.0.3/src/vocode/types/agent_update_params.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/azure_voice.py` & `fern_vocode-0.0.3/src/vocode/types/azure_voice.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/azure_voice_params.py` & `fern_vocode-0.0.3/src/vocode/types/azure_voice_params.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/azure_voice_update_params.py` & `fern_vocode-0.0.3/src/vocode/types/azure_voice_update_params.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/call.py` & `fern_vocode-0.0.3/src/vocode/types/call.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/call_status.py` & `fern_vocode-0.0.3/src/vocode/types/call_status.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/dtmf_action.py` & `fern_vocode-0.0.3/src/vocode/types/dtmf_action.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/dtmf_action_params.py` & `fern_vocode-0.0.3/src/vocode/types/dtmf_action_params.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/dtmf_action_update_params.py` & `fern_vocode-0.0.3/src/vocode/types/dtmf_action_update_params.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/eleven_labs_voice.py` & `fern_vocode-0.0.3/src/vocode/types/eleven_labs_voice.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/eleven_labs_voice_params.py` & `fern_vocode-0.0.3/src/vocode/types/eleven_labs_voice_params.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/eleven_labs_voice_update_params.py` & `fern_vocode-0.0.3/src/vocode/types/eleven_labs_voice_update_params.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/end_conversation_action.py` & `fern_vocode-0.0.3/src/vocode/types/end_conversation_action.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/end_conversation_action_params.py` & `fern_vocode-0.0.3/src/vocode/types/end_conversation_action_params.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/end_conversation_action_update_params.py` & `fern_vocode-0.0.3/src/vocode/types/end_conversation_action_update_params.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/event_type.py` & `fern_vocode-0.0.3/src/vocode/types/event_type.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/http_validation_error.py` & `fern_vocode-0.0.3/src/vocode/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/phone_number.py` & `fern_vocode-0.0.3/src/vocode/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/plan_type.py` & `fern_vocode-0.0.3/src/vocode/types/plan_type.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/rime_voice.py` & `fern_vocode-0.0.3/src/vocode/types/rime_voice.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/rime_voice_params.py` & `fern_vocode-0.0.3/src/vocode/types/rime_voice_params.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/rime_voice_update_params.py` & `fern_vocode-0.0.3/src/vocode/types/rime_voice_update_params.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/undefined.py` & `fern_vocode-0.0.3/src/vocode/types/undefined.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/usage.py` & `fern_vocode-0.0.3/src/vocode/types/usage.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/validation_error.py` & `fern_vocode-0.0.3/src/vocode/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/voice_type.py` & `fern_vocode-0.0.3/src/vocode/types/voice_type.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/webhook.py` & `fern_vocode-0.0.3/src/vocode/types/webhook.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/webhook_params.py` & `fern_vocode-0.0.3/src/vocode/types/webhook_params.py`

 * *Files identical despite different names*

### Comparing `fern_vocode-0.0.2/src/vocode/types/webhook_update_params.py` & `fern_vocode-0.0.3/src/vocode/types/webhook_update_params.py`

 * *Files identical despite different names*

