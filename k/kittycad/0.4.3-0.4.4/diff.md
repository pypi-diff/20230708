# Comparing `tmp/kittycad-0.4.3.tar.gz` & `tmp/kittycad-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kittycad-0.4.3.tar", max compression
+gzip compressed data, was "kittycad-0.4.4.tar", max compression
```

## Comparing `kittycad-0.4.3.tar` & `kittycad-0.4.4.tar`

### file list

```diff
@@ -1,230 +1,240 @@
--rw-r--r--   0        0        0     1065 2023-05-26 19:40:36.890207 kittycad-0.4.3/LICENSE
--rw-r--r--   0        0        0      875 2023-05-26 19:40:36.890207 kittycad-0.4.3/README.md
--rw-r--r--   0        0        0       48 2023-05-26 19:40:37.658231 kittycad-0.4.3/kittycad/__init__.py
--rw-r--r--   0        0        0       47 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/__init__.py
--rw-r--r--   0        0        0      119 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/ai/__init__.py
--rw-r--r--   0        0        0     3781 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/ai/create_image_to_3d.py
--rw-r--r--   0        0        0     3559 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/ai/create_text_to_3d.py
--rw-r--r--   0        0        0      199 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_calls/__init__.py
--rw-r--r--   0        0        0     3110 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_calls/get_api_call.py
--rw-r--r--   0        0        0     2799 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_calls/get_api_call_for_user.py
--rw-r--r--   0        0        0     3243 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_calls/get_api_call_metrics.py
--rw-r--r--   0        0        0     6149 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_calls/get_async_operation.py
--rw-r--r--   0        0        0     4236 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_calls/list_api_calls.py
--rw-r--r--   0        0        0     5005 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_calls/list_api_calls_for_user.py
--rw-r--r--   0        0        0     4815 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_calls/list_async_operations.py
--rw-r--r--   0        0        0     4351 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_calls/user_list_api_calls.py
--rw-r--r--   0        0        0      352 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_tokens/__init__.py
--rw-r--r--   0        0        0     2573 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_tokens/create_api_token_for_user.py
--rw-r--r--   0        0        0     2879 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_tokens/delete_api_token_for_user.py
--rw-r--r--   0        0        0     2784 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_tokens/get_api_token_for_user.py
--rw-r--r--   0        0        0     4284 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/api_tokens/list_api_tokens_for_user.py
--rw-r--r--   0        0        0      116 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/apps/__init__.py
--rw-r--r--   0        0        0     2597 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/apps/apps_github_callback.py
--rw-r--r--   0        0        0     2911 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/apps/apps_github_consent.py
--rw-r--r--   0        0        0     2338 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/apps/apps_github_webhook.py
--rw-r--r--   0        0        0      156 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/beta/__init__.py
--rw-r--r--   0        0        0      118 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/constant/__init__.py
--rw-r--r--   0        0        0     2758 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/constant/get_physics_constant.py
--rw-r--r--   0        0        0      161 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/executor/__init__.py
--rw-r--r--   0        0        0     1781 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/executor/create_executor_term.py
--rw-r--r--   0        0        0     3195 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/executor/create_file_execution.py
--rw-r--r--   0        0        0      233 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/file/__init__.py
--rw-r--r--   0        0        0     4635 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/file/create_file_center_of_mass.py
--rw-r--r--   0        0        0     4461 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/file/create_file_conversion.py
--rw-r--r--   0        0        0     1962 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/file/create_file_conversion_with_base64_helper.py
--rw-r--r--   0        0        0     5162 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/file/create_file_density.py
--rw-r--r--   0        0        0     5290 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/file/create_file_mass.py
--rw-r--r--   0        0        0     4559 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/file/create_file_surface_area.py
--rw-r--r--   0        0        0     4487 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/file/create_file_volume.py
--rw-r--r--   0        0        0     1341 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/file/get_file_conversion_with_base64_helper.py
--rw-r--r--   0        0        0      133 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/hidden/__init__.py
--rw-r--r--   0        0        0     2729 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/hidden/auth_email.py
--rw-r--r--   0        0        0     3220 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/hidden/auth_email_callback.py
--rw-r--r--   0        0        0     2139 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/hidden/logout.py
--rw-r--r--   0        0        0      105 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/meta/__init__.py
--rw-r--r--   0        0        0     2383 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/meta/get_ai_plugin_manifest.py
--rw-r--r--   0        0        0     2629 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/meta/get_metadata.py
--rw-r--r--   0        0        0     2564 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/meta/get_openai_schema.py
--rw-r--r--   0        0        0     2193 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/meta/get_schema.py
--rw-r--r--   0        0        0     2245 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/meta/ping.py
--rw-r--r--   0        0        0      144 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/modeling/__init__.py
--rw-r--r--   0        0        0     2794 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/modeling/cmd.py
--rw-r--r--   0        0        0     2701 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/modeling/cmd_batch.py
--rw-r--r--   0        0        0     1995 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/modeling/modeling_commands_ws.py
--rw-r--r--   0        0        0      123 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/oauth2/__init__.py
--rw-r--r--   0        0        0      117 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/__init__.py
--rw-r--r--   0        0        0     2956 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/create_payment_information_for_user.py
--rw-r--r--   0        0        0     2638 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/create_payment_intent_for_user.py
--rw-r--r--   0        0        0     2431 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/delete_payment_information_for_user.py
--rw-r--r--   0        0        0     2486 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/delete_payment_method_for_user.py
--rw-r--r--   0        0        0     2655 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/get_payment_balance_for_user.py
--rw-r--r--   0        0        0     2681 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/get_payment_information_for_user.py
--rw-r--r--   0        0        0     2616 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/list_invoices_for_user.py
--rw-r--r--   0        0        0     2684 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/list_payment_methods_for_user.py
--rw-r--r--   0        0        0     2954 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/update_payment_information_for_user.py
--rw-r--r--   0        0        0     2483 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/payments/validate_customer_tax_information_for_user.py
--rw-r--r--   0        0        0      101 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/__init__.py
--rw-r--r--   0        0        0     3679 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_angle_unit_conversion.py
--rw-r--r--   0        0        0     3653 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_area_unit_conversion.py
--rw-r--r--   0        0        0     3729 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_current_unit_conversion.py
--rw-r--r--   0        0        0     3703 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_energy_unit_conversion.py
--rw-r--r--   0        0        0     3677 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_force_unit_conversion.py
--rw-r--r--   0        0        0     3781 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_frequency_unit_conversion.py
--rw-r--r--   0        0        0     3703 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_length_unit_conversion.py
--rw-r--r--   0        0        0     3651 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_mass_unit_conversion.py
--rw-r--r--   0        0        0     3677 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_power_unit_conversion.py
--rw-r--r--   0        0        0     3755 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_pressure_unit_conversion.py
--rw-r--r--   0        0        0     3833 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_temperature_unit_conversion.py
--rw-r--r--   0        0        0     3703 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_torque_unit_conversion.py
--rw-r--r--   0        0        0     3703 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/unit/get_volume_unit_conversion.py
--rw-r--r--   0        0        0      297 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/__init__.py
--rw-r--r--   0        0        0     2579 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/delete_user_self.py
--rw-r--r--   0        0        0     2757 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/get_session_for_user.py
--rw-r--r--   0        0        0     3061 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/get_user.py
--rw-r--r--   0        0        0     3185 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/get_user_extended.py
--rw-r--r--   0        0        0     2480 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/get_user_front_hash_self.py
--rw-r--r--   0        0        0     2506 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/get_user_onboarding_self.py
--rw-r--r--   0        0        0     2523 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/get_user_self.py
--rw-r--r--   0        0        0     2629 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/get_user_self_extended.py
--rw-r--r--   0        0        0     4105 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/list_users.py
--rw-r--r--   0        0        0     4187 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/list_users_extended.py
--rw-r--r--   0        0        0     2779 2023-05-26 19:40:37.662231 kittycad-0.4.3/kittycad/api/users/update_user_self.py
--rw-r--r--   0        0        0     2297 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/client.py
--rw-r--r--   0        0        0     5250 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/client_test.py
--rw-r--r--   0        0        0    99150 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/examples_test.py
--rw-r--r--   0        0        0     5856 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/__init__.py
--rw-r--r--   0        0        0      322 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/account_provider.py
--rw-r--r--   0        0        0     2249 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/ai_plugin_api.py
--rw-r--r--   0        0        0      242 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/ai_plugin_api_type.py
--rw-r--r--   0        0        0     2440 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/ai_plugin_auth.py
--rw-r--r--   0        0        0      413 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/ai_plugin_auth_type.py
--rw-r--r--   0        0        0      287 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/ai_plugin_http_auth_type.py
--rw-r--r--   0        0        0     4685 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/ai_plugin_manifest.py
--rw-r--r--   0        0        0     1720 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/api_call_query_group.py
--rw-r--r--   0        0        0      777 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/api_call_query_group_by.py
--rw-r--r--   0        0        0      620 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/api_call_status.py
--rw-r--r--   0        0        0     8574 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/api_call_with_price.py
--rw-r--r--   0        0        0     2128 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/api_call_with_price_results_page.py
--rw-r--r--   0        0        0     3455 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/api_token.py
--rw-r--r--   0        0        0     2004 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/api_token_results_page.py
--rw-r--r--   0        0        0     1447 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/app_client_info.py
--rw-r--r--   0        0        0     5909 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/async_api_call.py
--rw-r--r--   0        0        0    34857 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/async_api_call_output.py
--rw-r--r--   0        0        0     2066 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/async_api_call_results_page.py
--rw-r--r--   0        0        0      648 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/async_api_call_type.py
--rw-r--r--   0        0        0     2127 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/billing_info.py
--rw-r--r--   0        0        0     1479 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/cache_metadata.py
--rw-r--r--   0        0        0     3353 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/card_details.py
--rw-r--r--   0        0        0     2697 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/cluster.py
--rw-r--r--   0        0        0      229 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/code_language.py
--rw-r--r--   0        0        0     2244 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/code_output.py
--rw-r--r--   0        0        0     1732 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/commit.py
--rw-r--r--   0        0        0    14343 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/connection.py
--rw-r--r--   0        0        0    13513 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/country_code.py
--rw-r--r--   0        0        0      507 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/created_at_sort_mode.py
--rw-r--r--   0        0        0     8623 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/currency.py
--rw-r--r--   0        0        0     4298 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/customer.py
--rw-r--r--   0        0        0     4468 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/customer_balance.py
--rw-r--r--   0        0        0     2412 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/device_access_token_request_form.py
--rw-r--r--   0        0        0     1580 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/device_auth_request_form.py
--rw-r--r--   0        0        0     1606 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/device_auth_verify_params.py
--rw-r--r--   0        0        0    21264 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/docker_system_info.py
--rw-r--r--   0        0        0     1789 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/email_authentication_form.py
--rw-r--r--   0        0        0     3847 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/engine_metadata.py
--rw-r--r--   0        0        0      529 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/environment.py
--rw-r--r--   0        0        0     1930 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/error.py
--rw-r--r--   0        0        0     2715 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/executor_metadata.py
--rw-r--r--   0        0        0     6069 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/extended_user.py
--rw-r--r--   0        0        0     2060 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/extended_user_results_page.py
--rw-r--r--   0        0        0     1940 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/extrude.py
--rw-r--r--   0        0        0     5862 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/file_center_of_mass.py
--rw-r--r--   0        0        0     6222 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/file_conversion.py
--rw-r--r--   0        0        0     5887 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/file_density.py
--rw-r--r--   0        0        0     1369 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/file_export_format.py
--rw-r--r--   0        0        0     1306 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/file_import_format.py
--rw-r--r--   0        0        0     5869 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/file_mass.py
--rw-r--r--   0        0        0     5684 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/file_surface_area.py
--rw-r--r--   0        0        0     1513 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/file_system_metadata.py
--rw-r--r--   0        0        0     5590 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/file_volume.py
--rw-r--r--   0        0        0     2304 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/gateway.py
--rw-r--r--   0        0        0      187 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/image_type.py
--rw-r--r--   0        0        0     2228 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/index_info.py
--rw-r--r--   0        0        0     8273 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/invoice.py
--rw-r--r--   0        0        0     2888 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/invoice_line_item.py
--rw-r--r--   0        0        0      563 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/invoice_status.py
--rw-r--r--   0        0        0     2666 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/jetstream.py
--rw-r--r--   0        0        0     1907 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/jetstream_api_stats.py
--rw-r--r--   0        0        0     2212 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/jetstream_config.py
--rw-r--r--   0        0        0     3174 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/jetstream_stats.py
--rw-r--r--   0        0        0     2125 2023-05-26 19:40:37.666231 kittycad-0.4.3/kittycad/models/leaf_node.py
--rw-r--r--   0        0        0     2007 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/line3d.py
--rw-r--r--   0        0        0     1337 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/mesh.py
--rw-r--r--   0        0        0     1923 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/meta_cluster_info.py
--rw-r--r--   0        0        0     5025 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/metadata.py
--rw-r--r--   0        0        0     1788 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/method.py
--rw-r--r--   0        0        0     1726 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/modeling_cmd.py
--rw-r--r--   0        0        0       76 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/modeling_cmd_id.py
--rw-r--r--   0        0        0     2456 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/modeling_cmd_req.py
--rw-r--r--   0        0        0     1752 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/modeling_cmd_req_batch.py
--rw-r--r--   0        0        0     2399 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/modeling_error.py
--rw-r--r--   0        0        0     1878 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/modeling_outcome.py
--rw-r--r--   0        0        0     1511 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/modeling_outcomes.py
--rw-r--r--   0        0        0     3081 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/new_address.py
--rw-r--r--   0        0        0     2038 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/o_auth2_client_info.py
--rw-r--r--   0        0        0      415 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/o_auth2_grant_type.py
--rw-r--r--   0        0        0     2509 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/onboarding.py
--rw-r--r--   0        0        0     1646 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/output_file.py
--rw-r--r--   0        0        0     1527 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/payment_intent.py
--rw-r--r--   0        0        0     3753 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/payment_method.py
--rw-r--r--   0        0        0     2267 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/payment_method_card_checks.py
--rw-r--r--   0        0        0      294 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/payment_method_type.py
--rw-r--r--   0        0        0     5586 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/physics_constant.py
--rw-r--r--   0        0        0     4448 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/physics_constant_name.py
--rw-r--r--   0        0        0     2809 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/plugins_info.py
--rw-r--r--   0        0        0     1530 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/point2d.py
--rw-r--r--   0        0        0     1691 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/point3d.py
--rw-r--r--   0        0        0     1498 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/point_e_metadata.py
--rw-r--r--   0        0        0     1432 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/pong.py
--rw-r--r--   0        0        0     4187 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/registry_service_config.py
--rw-r--r--   0        0        0     2034 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/runtime.py
--rw-r--r--   0        0        0     3855 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/session.py
--rw-r--r--   0        0        0      214 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/system_info_cgroup_driver_enum.py
--rw-r--r--   0        0        0      175 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/system_info_cgroup_version_enum.py
--rw-r--r--   0        0        0     1663 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/system_info_default_address_pools.py
--rw-r--r--   0        0        0      213 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/system_info_isolation_enum.py
--rw-r--r--   0        0        0      377 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_angle.py
--rw-r--r--   0        0        0     6324 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_angle_conversion.py
--rw-r--r--   0        0        0     1937 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_area.py
--rw-r--r--   0        0        0     6311 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_area_conversion.py
--rw-r--r--   0        0        0      623 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_current.py
--rw-r--r--   0        0        0     6350 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_current_conversion.py
--rw-r--r--   0        0        0      934 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_energy.py
--rw-r--r--   0        0        0     6337 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_energy_conversion.py
--rw-r--r--   0        0        0      916 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_force.py
--rw-r--r--   0        0        0     6324 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_force_conversion.py
--rw-r--r--   0        0        0      997 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_frequency.py
--rw-r--r--   0        0        0     6376 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_frequency_conversion.py
--rw-r--r--   0        0        0     1522 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_length.py
--rw-r--r--   0        0        0     6337 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_length_conversion.py
--rw-r--r--   0        0        0     1754 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_mass.py
--rw-r--r--   0        0        0     6311 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_mass_conversion.py
--rw-r--r--   0        0        0     1014 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_power.py
--rw-r--r--   0        0        0     6324 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_power_conversion.py
--rw-r--r--   0        0        0      973 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_pressure.py
--rw-r--r--   0        0        0     6363 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_pressure_conversion.py
--rw-r--r--   0        0        0      593 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_temperature.py
--rw-r--r--   0        0        0     6402 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_temperature_conversion.py
--rw-r--r--   0        0        0      415 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_torque.py
--rw-r--r--   0        0        0     6337 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_torque_conversion.py
--rw-r--r--   0        0        0     2355 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_volume.py
--rw-r--r--   0        0        0     6337 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/unit_volume_conversion.py
--rw-r--r--   0        0        0     2577 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/update_user.py
--rw-r--r--   0        0        0     5084 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/user.py
--rw-r--r--   0        0        0     1942 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/user_results_page.py
--rw-r--r--   0        0        0       67 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/uuid.py
--rw-r--r--   0        0        0     3448 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/models/verification_token.py
--rw-r--r--   0        0        0       26 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/py.typed
--rw-r--r--   0        0        0     1049 2023-05-26 19:40:37.670232 kittycad-0.4.3/kittycad/types.py
--rw-r--r--   0        0        0     2472 2023-05-26 19:40:37.670232 kittycad-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 kittycad-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-08 02:25:21.114181 kittycad-0.4.4/LICENSE
+-rw-r--r--   0        0        0      875 2023-07-08 02:25:21.114181 kittycad-0.4.4/README.md
+-rw-r--r--   0        0        0       48 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/__init__.py
+-rw-r--r--   0        0        0      119 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/ai/__init__.py
+-rw-r--r--   0        0        0     3781 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/ai/create_image_to_3d.py
+-rw-r--r--   0        0        0     3559 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/ai/create_text_to_3d.py
+-rw-r--r--   0        0        0      199 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_calls/__init__.py
+-rw-r--r--   0        0        0     3110 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_calls/get_api_call.py
+-rw-r--r--   0        0        0     2799 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_calls/get_api_call_for_user.py
+-rw-r--r--   0        0        0     3243 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_calls/get_api_call_metrics.py
+-rw-r--r--   0        0        0     6149 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_calls/get_async_operation.py
+-rw-r--r--   0        0        0     4236 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_calls/list_api_calls.py
+-rw-r--r--   0        0        0     5005 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_calls/list_api_calls_for_user.py
+-rw-r--r--   0        0        0     4815 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_calls/list_async_operations.py
+-rw-r--r--   0        0        0     4351 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_calls/user_list_api_calls.py
+-rw-r--r--   0        0        0      352 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_tokens/__init__.py
+-rw-r--r--   0        0        0     2573 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_tokens/create_api_token_for_user.py
+-rw-r--r--   0        0        0     2879 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_tokens/delete_api_token_for_user.py
+-rw-r--r--   0        0        0     2784 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_tokens/get_api_token_for_user.py
+-rw-r--r--   0        0        0     4284 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/api_tokens/list_api_tokens_for_user.py
+-rw-r--r--   0        0        0      116 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/apps/__init__.py
+-rw-r--r--   0        0        0     2597 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/apps/apps_github_callback.py
+-rw-r--r--   0        0        0     2911 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/apps/apps_github_consent.py
+-rw-r--r--   0        0        0     2338 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/apps/apps_github_webhook.py
+-rw-r--r--   0        0        0      156 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/beta/__init__.py
+-rw-r--r--   0        0        0      118 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/constant/__init__.py
+-rw-r--r--   0        0        0     2758 2023-07-08 02:25:21.846171 kittycad-0.4.4/kittycad/api/constant/get_physics_constant.py
+-rw-r--r--   0        0        0      161 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/executor/__init__.py
+-rw-r--r--   0        0        0     1781 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/executor/create_executor_term.py
+-rw-r--r--   0        0        0     3195 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/executor/create_file_execution.py
+-rw-r--r--   0        0        0      233 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/file/__init__.py
+-rw-r--r--   0        0        0     4635 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/file/create_file_center_of_mass.py
+-rw-r--r--   0        0        0     4653 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/file/create_file_conversion.py
+-rw-r--r--   0        0        0     1962 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/file/create_file_conversion_with_base64_helper.py
+-rw-r--r--   0        0        0     5162 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/file/create_file_density.py
+-rw-r--r--   0        0        0     5290 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/file/create_file_mass.py
+-rw-r--r--   0        0        0     4559 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/file/create_file_surface_area.py
+-rw-r--r--   0        0        0     4487 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/file/create_file_volume.py
+-rw-r--r--   0        0        0     1341 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/file/get_file_conversion_with_base64_helper.py
+-rw-r--r--   0        0        0      133 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/hidden/__init__.py
+-rw-r--r--   0        0        0     2729 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/hidden/auth_email.py
+-rw-r--r--   0        0        0     3220 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/hidden/auth_email_callback.py
+-rw-r--r--   0        0        0     2139 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/hidden/logout.py
+-rw-r--r--   0        0        0      105 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/meta/__init__.py
+-rw-r--r--   0        0        0     2383 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/meta/get_ai_plugin_manifest.py
+-rw-r--r--   0        0        0     2629 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/meta/get_metadata.py
+-rw-r--r--   0        0        0     2564 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/meta/get_openai_schema.py
+-rw-r--r--   0        0        0     2193 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/meta/get_schema.py
+-rw-r--r--   0        0        0     2245 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/meta/ping.py
+-rw-r--r--   0        0        0      144 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/modeling/__init__.py
+-rw-r--r--   0        0        0     2794 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/modeling/cmd.py
+-rw-r--r--   0        0        0     2701 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/modeling/cmd_batch.py
+-rw-r--r--   0        0        0     1995 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/modeling/modeling_commands_ws.py
+-rw-r--r--   0        0        0      123 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/oauth2/__init__.py
+-rw-r--r--   0        0        0      117 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/__init__.py
+-rw-r--r--   0        0        0     2956 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/create_payment_information_for_user.py
+-rw-r--r--   0        0        0     2638 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/create_payment_intent_for_user.py
+-rw-r--r--   0        0        0     2431 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/delete_payment_information_for_user.py
+-rw-r--r--   0        0        0     2486 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/delete_payment_method_for_user.py
+-rw-r--r--   0        0        0     2655 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/get_payment_balance_for_user.py
+-rw-r--r--   0        0        0     2681 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/get_payment_information_for_user.py
+-rw-r--r--   0        0        0     2616 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/list_invoices_for_user.py
+-rw-r--r--   0        0        0     2684 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/list_payment_methods_for_user.py
+-rw-r--r--   0        0        0     2954 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/update_payment_information_for_user.py
+-rw-r--r--   0        0        0     2483 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/payments/validate_customer_tax_information_for_user.py
+-rw-r--r--   0        0        0      101 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/__init__.py
+-rw-r--r--   0        0        0     3679 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_angle_unit_conversion.py
+-rw-r--r--   0        0        0     3653 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_area_unit_conversion.py
+-rw-r--r--   0        0        0     3729 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_current_unit_conversion.py
+-rw-r--r--   0        0        0     3703 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_energy_unit_conversion.py
+-rw-r--r--   0        0        0     3677 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_force_unit_conversion.py
+-rw-r--r--   0        0        0     3781 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_frequency_unit_conversion.py
+-rw-r--r--   0        0        0     3703 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_length_unit_conversion.py
+-rw-r--r--   0        0        0     3651 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_mass_unit_conversion.py
+-rw-r--r--   0        0        0     3677 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_power_unit_conversion.py
+-rw-r--r--   0        0        0     3755 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_pressure_unit_conversion.py
+-rw-r--r--   0        0        0     3833 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_temperature_unit_conversion.py
+-rw-r--r--   0        0        0     3703 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_torque_unit_conversion.py
+-rw-r--r--   0        0        0     3703 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/unit/get_volume_unit_conversion.py
+-rw-r--r--   0        0        0      297 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/__init__.py
+-rw-r--r--   0        0        0     2579 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/delete_user_self.py
+-rw-r--r--   0        0        0     2757 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/get_session_for_user.py
+-rw-r--r--   0        0        0     3061 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/get_user.py
+-rw-r--r--   0        0        0     3185 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/get_user_extended.py
+-rw-r--r--   0        0        0     2480 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/get_user_front_hash_self.py
+-rw-r--r--   0        0        0     2506 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/get_user_onboarding_self.py
+-rw-r--r--   0        0        0     2523 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/get_user_self.py
+-rw-r--r--   0        0        0     2629 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/get_user_self_extended.py
+-rw-r--r--   0        0        0     4105 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/list_users.py
+-rw-r--r--   0        0        0     4187 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/list_users_extended.py
+-rw-r--r--   0        0        0     2779 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/api/users/update_user_self.py
+-rw-r--r--   0        0        0     2297 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/client.py
+-rw-r--r--   0        0        0     5250 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/client_test.py
+-rw-r--r--   0        0        0    96653 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/examples_test.py
+-rw-r--r--   0        0        0     6234 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/__init__.py
+-rw-r--r--   0        0        0      322 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/account_provider.py
+-rw-r--r--   0        0        0     2258 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/ai_plugin_api.py
+-rw-r--r--   0        0        0      242 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/ai_plugin_api_type.py
+-rw-r--r--   0        0        0     2452 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/ai_plugin_auth.py
+-rw-r--r--   0        0        0      413 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/ai_plugin_auth_type.py
+-rw-r--r--   0        0        0      287 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/ai_plugin_http_auth_type.py
+-rw-r--r--   0        0        0     4685 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/ai_plugin_manifest.py
+-rw-r--r--   0        0        0     1720 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/api_call_query_group.py
+-rw-r--r--   0        0        0      777 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/api_call_query_group_by.py
+-rw-r--r--   0        0        0      620 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/api_call_status.py
+-rw-r--r--   0        0        0     8592 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/api_call_with_price.py
+-rw-r--r--   0        0        0     2128 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/api_call_with_price_results_page.py
+-rw-r--r--   0        0        0     3455 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/api_token.py
+-rw-r--r--   0        0        0     2004 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/api_token_results_page.py
+-rw-r--r--   0        0        0     1447 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/app_client_info.py
+-rw-r--r--   0        0        0     5928 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/async_api_call.py
+-rw-r--r--   0        0        0    36592 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/async_api_call_output.py
+-rw-r--r--   0        0        0     2066 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/async_api_call_results_page.py
+-rw-r--r--   0        0        0      648 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/async_api_call_type.py
+-rw-r--r--   0        0        0      421 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/axis.py
+-rw-r--r--   0        0        0     2247 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/axis_direction_pair.py
+-rw-r--r--   0        0        0     2127 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/billing_info.py
+-rw-r--r--   0        0        0     1479 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/cache_metadata.py
+-rw-r--r--   0        0        0      440 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/camera_drag_interaction_type.py
+-rw-r--r--   0        0        0     3353 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/card_details.py
+-rw-r--r--   0        0        0     2697 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/cluster.py
+-rw-r--r--   0        0        0      409 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/code_language.py
+-rw-r--r--   0        0        0     2244 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/code_output.py
+-rw-r--r--   0        0        0     1732 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/commit.py
+-rw-r--r--   0        0        0    14343 2023-07-08 02:25:21.850171 kittycad-0.4.4/kittycad/models/connection.py
+-rw-r--r--   0        0        0    13513 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/country_code.py
+-rw-r--r--   0        0        0     2120 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/coupon.py
+-rw-r--r--   0        0        0      507 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/created_at_sort_mode.py
+-rw-r--r--   0        0        0     8623 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/currency.py
+-rw-r--r--   0        0        0     4314 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/customer.py
+-rw-r--r--   0        0        0     4468 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/customer_balance.py
+-rw-r--r--   0        0        0     2421 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/device_access_token_request_form.py
+-rw-r--r--   0        0        0     1580 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/device_auth_request_form.py
+-rw-r--r--   0        0        0     1606 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/device_auth_verify_params.py
+-rw-r--r--   0        0        0      327 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/direction.py
+-rw-r--r--   0        0        0     1684 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/discount.py
+-rw-r--r--   0        0        0    21264 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/docker_system_info.py
+-rw-r--r--   0        0        0     1789 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/email_authentication_form.py
+-rw-r--r--   0        0        0     3860 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/engine_metadata.py
+-rw-r--r--   0        0        0      529 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/environment.py
+-rw-r--r--   0        0        0     1930 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/error.py
+-rw-r--r--   0        0        0     2728 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/executor_metadata.py
+-rw-r--r--   0        0        0     6069 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/extended_user.py
+-rw-r--r--   0        0        0     2060 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/extended_user_results_page.py
+-rw-r--r--   0        0        0     2120 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/extrude.py
+-rw-r--r--   0        0        0     5881 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/file_center_of_mass.py
+-rw-r--r--   0        0        0     7862 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/file_conversion.py
+-rw-r--r--   0        0        0     5906 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/file_density.py
+-rw-r--r--   0        0        0     1400 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/file_export_format.py
+-rw-r--r--   0        0        0     1140 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/file_import_format.py
+-rw-r--r--   0        0        0     5888 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/file_mass.py
+-rw-r--r--   0        0        0     5703 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/file_surface_area.py
+-rw-r--r--   0        0        0     1513 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/file_system_metadata.py
+-rw-r--r--   0        0        0     5609 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/file_volume.py
+-rw-r--r--   0        0        0     2304 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/gateway.py
+-rw-r--r--   0        0        0      187 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/image_type.py
+-rw-r--r--   0        0        0     2228 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/index_info.py
+-rw-r--r--   0        0        0     6676 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/input_format.py
+-rw-r--r--   0        0        0     8822 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/invoice.py
+-rw-r--r--   0        0        0     2904 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/invoice_line_item.py
+-rw-r--r--   0        0        0      563 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/invoice_status.py
+-rw-r--r--   0        0        0     2666 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/jetstream.py
+-rw-r--r--   0        0        0     1907 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/jetstream_api_stats.py
+-rw-r--r--   0        0        0     2212 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/jetstream_config.py
+-rw-r--r--   0        0        0     3174 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/jetstream_stats.py
+-rw-r--r--   0        0        0     2125 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/leaf_node.py
+-rw-r--r--   0        0        0     1337 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/mesh.py
+-rw-r--r--   0        0        0     1923 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/meta_cluster_info.py
+-rw-r--r--   0        0        0     5038 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/metadata.py
+-rw-r--r--   0        0        0     1788 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/method.py
+-rw-r--r--   0        0        0    12269 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/modeling_cmd.py
+-rw-r--r--   0        0        0       76 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/modeling_cmd_id.py
+-rw-r--r--   0        0        0     2456 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/modeling_cmd_req.py
+-rw-r--r--   0        0        0     1752 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/modeling_cmd_req_batch.py
+-rw-r--r--   0        0        0     2399 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/modeling_error.py
+-rw-r--r--   0        0        0     1878 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/modeling_outcome.py
+-rw-r--r--   0        0        0     1511 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/modeling_outcomes.py
+-rw-r--r--   0        0        0     3094 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/new_address.py
+-rw-r--r--   0        0        0     2038 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/o_auth2_client_info.py
+-rw-r--r--   0        0        0      415 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/o_auth2_grant_type.py
+-rw-r--r--   0        0        0     2509 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/onboarding.py
+-rw-r--r--   0        0        0     1646 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/output_file.py
+-rw-r--r--   0        0        0     7715 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/output_format.py
+-rw-r--r--   0        0        0     6144 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/path_segment.py
+-rw-r--r--   0        0        0     1527 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/payment_intent.py
+-rw-r--r--   0        0        0     3760 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/payment_method.py
+-rw-r--r--   0        0        0     2267 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/payment_method_card_checks.py
+-rw-r--r--   0        0        0      294 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/payment_method_type.py
+-rw-r--r--   0        0        0     5602 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/physics_constant.py
+-rw-r--r--   0        0        0     4448 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/physics_constant_name.py
+-rw-r--r--   0        0        0     2809 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/plugins_info.py
+-rw-r--r--   0        0        0     1530 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/point2d.py
+-rw-r--r--   0        0        0     1691 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/point3d.py
+-rw-r--r--   0        0        0     1498 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/point_e_metadata.py
+-rw-r--r--   0        0        0     1432 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/pong.py
+-rw-r--r--   0        0        0     4187 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/registry_service_config.py
+-rw-r--r--   0        0        0     2034 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/runtime.py
+-rw-r--r--   0        0        0     3855 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/session.py
+-rw-r--r--   0        0        0      656 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/storage.py
+-rw-r--r--   0        0        0     2349 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/system.py
+-rw-r--r--   0        0        0      214 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/system_info_cgroup_driver_enum.py
+-rw-r--r--   0        0        0      175 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/system_info_cgroup_version_enum.py
+-rw-r--r--   0        0        0     1663 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/system_info_default_address_pools.py
+-rw-r--r--   0        0        0      213 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/system_info_isolation_enum.py
+-rw-r--r--   0        0        0      377 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_angle.py
+-rw-r--r--   0        0        0     6365 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_angle_conversion.py
+-rw-r--r--   0        0        0     1937 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_area.py
+-rw-r--r--   0        0        0     6354 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_area_conversion.py
+-rw-r--r--   0        0        0      623 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_current.py
+-rw-r--r--   0        0        0     6387 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_current_conversion.py
+-rw-r--r--   0        0        0      934 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_energy.py
+-rw-r--r--   0        0        0     6376 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_energy_conversion.py
+-rw-r--r--   0        0        0      916 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_force.py
+-rw-r--r--   0        0        0     6365 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_force_conversion.py
+-rw-r--r--   0        0        0      997 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_frequency.py
+-rw-r--r--   0        0        0     6409 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_frequency_conversion.py
+-rw-r--r--   0        0        0     1522 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_length.py
+-rw-r--r--   0        0        0     6376 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_length_conversion.py
+-rw-r--r--   0        0        0     1754 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_mass.py
+-rw-r--r--   0        0        0     6354 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_mass_conversion.py
+-rw-r--r--   0        0        0     1014 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_power.py
+-rw-r--r--   0        0        0     6365 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_power_conversion.py
+-rw-r--r--   0        0        0      973 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_pressure.py
+-rw-r--r--   0        0        0     6398 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_pressure_conversion.py
+-rw-r--r--   0        0        0      593 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_temperature.py
+-rw-r--r--   0        0        0     6431 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_temperature_conversion.py
+-rw-r--r--   0        0        0      415 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_torque.py
+-rw-r--r--   0        0        0     6376 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_torque_conversion.py
+-rw-r--r--   0        0        0     2355 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_volume.py
+-rw-r--r--   0        0        0     6376 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/unit_volume_conversion.py
+-rw-r--r--   0        0        0     2577 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/update_user.py
+-rw-r--r--   0        0        0     5084 2023-07-08 02:25:21.854171 kittycad-0.4.4/kittycad/models/user.py
+-rw-r--r--   0        0        0     1942 2023-07-08 02:25:21.858171 kittycad-0.4.4/kittycad/models/user_results_page.py
+-rw-r--r--   0        0        0       67 2023-07-08 02:25:21.858171 kittycad-0.4.4/kittycad/models/uuid.py
+-rw-r--r--   0        0        0     3448 2023-07-08 02:25:21.858171 kittycad-0.4.4/kittycad/models/verification_token.py
+-rw-r--r--   0        0        0       26 2023-07-08 02:25:21.858171 kittycad-0.4.4/kittycad/py.typed
+-rw-r--r--   0        0        0     1049 2023-07-08 02:25:21.858171 kittycad-0.4.4/kittycad/types.py
+-rw-r--r--   0        0        0     2472 2023-07-08 02:25:21.858171 kittycad-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 kittycad-0.4.4/PKG-INFO
```

### Comparing `kittycad-0.4.3/LICENSE` & `kittycad-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/README.md` & `kittycad-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/ai/create_image_to_3d.py` & `kittycad-0.4.4/kittycad/api/ai/create_image_to_3d.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/ai/create_text_to_3d.py` & `kittycad-0.4.4/kittycad/api/ai/create_text_to_3d.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/api_calls/get_api_call.py` & `kittycad-0.4.4/kittycad/api/api_calls/get_api_call.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/api_calls/get_api_call_for_user.py` & `kittycad-0.4.4/kittycad/api/api_calls/get_api_call_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/api_calls/get_api_call_metrics.py` & `kittycad-0.4.4/kittycad/api/api_calls/get_api_call_metrics.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/api_calls/get_async_operation.py` & `kittycad-0.4.4/kittycad/api/api_calls/get_async_operation.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/api_calls/list_api_calls.py` & `kittycad-0.4.4/kittycad/api/api_calls/list_api_calls.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/api_calls/list_api_calls_for_user.py` & `kittycad-0.4.4/kittycad/api/api_calls/list_api_calls_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/api_calls/list_async_operations.py` & `kittycad-0.4.4/kittycad/api/api_calls/list_async_operations.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/api_calls/user_list_api_calls.py` & `kittycad-0.4.4/kittycad/api/api_calls/user_list_api_calls.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/api_tokens/create_api_token_for_user.py` & `kittycad-0.4.4/kittycad/api/api_tokens/create_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/api_tokens/delete_api_token_for_user.py` & `kittycad-0.4.4/kittycad/api/api_tokens/delete_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/api_tokens/get_api_token_for_user.py` & `kittycad-0.4.4/kittycad/api/api_tokens/get_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/api_tokens/list_api_tokens_for_user.py` & `kittycad-0.4.4/kittycad/api/api_tokens/list_api_tokens_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/apps/apps_github_callback.py` & `kittycad-0.4.4/kittycad/api/apps/apps_github_callback.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/apps/apps_github_consent.py` & `kittycad-0.4.4/kittycad/api/apps/apps_github_consent.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/apps/apps_github_webhook.py` & `kittycad-0.4.4/kittycad/api/apps/apps_github_webhook.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/constant/get_physics_constant.py` & `kittycad-0.4.4/kittycad/api/constant/get_physics_constant.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/executor/create_executor_term.py` & `kittycad-0.4.4/kittycad/api/executor/create_executor_term.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/executor/create_file_execution.py` & `kittycad-0.4.4/kittycad/api/executor/create_file_execution.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/file/create_file_center_of_mass.py` & `kittycad-0.4.4/kittycad/api/file/create_file_center_of_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/file/create_file_conversion.py` & `kittycad-0.4.4/kittycad/api/file/create_file_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,16 @@
 def sync(
     output_format: FileExportFormat,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Optional[Union[FileConversion, Error]]:
-    """Convert a CAD file from one format to another. If the file being converted is larger than 25MB, it will be performed asynchronously.
+    """If you wish to specify the conversion options, use the `/file/conversion` endpoint instead.
+    Convert a CAD file from one format to another. If the file being converted is larger than 25MB, it will be performed asynchronously.
     If the conversion is performed synchronously, the contents of the converted file (`output`) will be returned as a base64 encoded string.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return sync_detailed(
         output_format=output_format,
         src_format=src_format,
         body=body,
@@ -123,15 +124,16 @@
 async def asyncio(
     output_format: FileExportFormat,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Optional[Union[FileConversion, Error]]:
-    """Convert a CAD file from one format to another. If the file being converted is larger than 25MB, it will be performed asynchronously.
+    """If you wish to specify the conversion options, use the `/file/conversion` endpoint instead.
+    Convert a CAD file from one format to another. If the file being converted is larger than 25MB, it will be performed asynchronously.
     If the conversion is performed synchronously, the contents of the converted file (`output`) will be returned as a base64 encoded string.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             output_format=output_format,
             src_format=src_format,
```

### Comparing `kittycad-0.4.3/kittycad/api/file/create_file_conversion_with_base64_helper.py` & `kittycad-0.4.4/kittycad/api/file/create_file_conversion_with_base64_helper.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/file/create_file_density.py` & `kittycad-0.4.4/kittycad/api/file/create_file_density.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/file/create_file_mass.py` & `kittycad-0.4.4/kittycad/api/file/create_file_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/file/create_file_surface_area.py` & `kittycad-0.4.4/kittycad/api/file/create_file_surface_area.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/file/create_file_volume.py` & `kittycad-0.4.4/kittycad/api/file/create_file_volume.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/file/get_file_conversion_with_base64_helper.py` & `kittycad-0.4.4/kittycad/api/file/get_file_conversion_with_base64_helper.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/hidden/auth_email.py` & `kittycad-0.4.4/kittycad/api/hidden/auth_email.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/hidden/auth_email_callback.py` & `kittycad-0.4.4/kittycad/api/hidden/auth_email_callback.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/hidden/logout.py` & `kittycad-0.4.4/kittycad/api/hidden/logout.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/meta/get_ai_plugin_manifest.py` & `kittycad-0.4.4/kittycad/api/meta/get_ai_plugin_manifest.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/meta/get_metadata.py` & `kittycad-0.4.4/kittycad/api/meta/get_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/meta/get_openai_schema.py` & `kittycad-0.4.4/kittycad/api/meta/get_openai_schema.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/meta/get_schema.py` & `kittycad-0.4.4/kittycad/api/meta/get_schema.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/meta/ping.py` & `kittycad-0.4.4/kittycad/api/meta/ping.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/modeling/cmd.py` & `kittycad-0.4.4/kittycad/api/modeling/cmd.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/modeling/cmd_batch.py` & `kittycad-0.4.4/kittycad/api/modeling/cmd_batch.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/modeling/modeling_commands_ws.py` & `kittycad-0.4.4/kittycad/api/modeling/modeling_commands_ws.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/payments/create_payment_information_for_user.py` & `kittycad-0.4.4/kittycad/api/payments/create_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/payments/create_payment_intent_for_user.py` & `kittycad-0.4.4/kittycad/api/payments/create_payment_intent_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/payments/delete_payment_information_for_user.py` & `kittycad-0.4.4/kittycad/api/payments/delete_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/payments/delete_payment_method_for_user.py` & `kittycad-0.4.4/kittycad/api/payments/delete_payment_method_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/payments/get_payment_balance_for_user.py` & `kittycad-0.4.4/kittycad/api/payments/get_payment_balance_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/payments/get_payment_information_for_user.py` & `kittycad-0.4.4/kittycad/api/payments/get_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/payments/list_invoices_for_user.py` & `kittycad-0.4.4/kittycad/api/payments/list_invoices_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/payments/list_payment_methods_for_user.py` & `kittycad-0.4.4/kittycad/api/payments/list_payment_methods_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/payments/update_payment_information_for_user.py` & `kittycad-0.4.4/kittycad/api/payments/update_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/payments/validate_customer_tax_information_for_user.py` & `kittycad-0.4.4/kittycad/api/payments/validate_customer_tax_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/unit/get_angle_unit_conversion.py` & `kittycad-0.4.4/kittycad/api/unit/get_angle_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/unit/get_area_unit_conversion.py` & `kittycad-0.4.4/kittycad/api/unit/get_area_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/unit/get_current_unit_conversion.py` & `kittycad-0.4.4/kittycad/api/unit/get_current_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/unit/get_energy_unit_conversion.py` & `kittycad-0.4.4/kittycad/api/unit/get_energy_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/unit/get_force_unit_conversion.py` & `kittycad-0.4.4/kittycad/api/unit/get_force_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/unit/get_frequency_unit_conversion.py` & `kittycad-0.4.4/kittycad/api/unit/get_frequency_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/unit/get_length_unit_conversion.py` & `kittycad-0.4.4/kittycad/api/unit/get_length_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/unit/get_mass_unit_conversion.py` & `kittycad-0.4.4/kittycad/api/unit/get_mass_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/unit/get_power_unit_conversion.py` & `kittycad-0.4.4/kittycad/api/unit/get_power_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/unit/get_pressure_unit_conversion.py` & `kittycad-0.4.4/kittycad/api/unit/get_pressure_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/unit/get_temperature_unit_conversion.py` & `kittycad-0.4.4/kittycad/api/unit/get_temperature_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/unit/get_torque_unit_conversion.py` & `kittycad-0.4.4/kittycad/api/unit/get_torque_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/unit/get_volume_unit_conversion.py` & `kittycad-0.4.4/kittycad/api/unit/get_volume_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/users/delete_user_self.py` & `kittycad-0.4.4/kittycad/api/users/delete_user_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/users/get_session_for_user.py` & `kittycad-0.4.4/kittycad/api/users/get_session_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/users/get_user.py` & `kittycad-0.4.4/kittycad/api/users/get_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/users/get_user_extended.py` & `kittycad-0.4.4/kittycad/api/users/get_user_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/users/get_user_front_hash_self.py` & `kittycad-0.4.4/kittycad/api/users/get_user_front_hash_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/users/get_user_onboarding_self.py` & `kittycad-0.4.4/kittycad/api/users/get_user_onboarding_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/users/get_user_self.py` & `kittycad-0.4.4/kittycad/api/users/get_user_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/users/get_user_self_extended.py` & `kittycad-0.4.4/kittycad/api/users/get_user_self_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/users/list_users.py` & `kittycad-0.4.4/kittycad/api/users/list_users.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/users/list_users_extended.py` & `kittycad-0.4.4/kittycad/api/users/list_users_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/api/users/update_user_self.py` & `kittycad-0.4.4/kittycad/api/users/update_user_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/client.py` & `kittycad-0.4.4/kittycad/client.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/client_test.py` & `kittycad-0.4.4/kittycad/client_test.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/examples_test.py` & `kittycad-0.4.4/kittycad/examples_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,20 +138,19 @@
 from kittycad.models.billing_info import BillingInfo
 from kittycad.models.code_language import CodeLanguage
 from kittycad.models.created_at_sort_mode import CreatedAtSortMode
 from kittycad.models.email_authentication_form import EmailAuthenticationForm
 from kittycad.models.file_export_format import FileExportFormat
 from kittycad.models.file_import_format import FileImportFormat
 from kittycad.models.image_type import ImageType
-from kittycad.models.line3d import Line3d
+from kittycad.models.modeling_cmd import ModelingCmd
 from kittycad.models.modeling_cmd_id import ModelingCmdId
 from kittycad.models.modeling_cmd_req import ModelingCmdReq
 from kittycad.models.modeling_cmd_req_batch import ModelingCmdReqBatch
 from kittycad.models.physics_constant_name import PhysicsConstantName
-from kittycad.models.point3d import Point3d
 from kittycad.models.unit_angle import UnitAngle
 from kittycad.models.unit_area import UnitArea
 from kittycad.models.unit_current import UnitCurrent
 from kittycad.models.unit_energy import UnitEnergy
 from kittycad.models.unit_force import UnitForce
 from kittycad.models.unit_frequency import UnitFrequency
 from kittycad.models.unit_length import UnitLength
@@ -1399,47 +1398,25 @@
 def test_cmd():
     # Create our client.
     client = ClientFromEnv()
 
     cmd.sync(
         client=client,
         body=ModelingCmdReq(
-            cmd=Line3d(
-                from_=Point3d(
-                    x=3.14,
-                    y=3.14,
-                    z=3.14,
-                ),
-                to=Point3d(
-                    x=3.14,
-                    y=3.14,
-                    z=3.14,
-                ),
-            ),
+            cmd=ModelingCmd.START_PATH,
             cmd_id=ModelingCmdId("<uuid>"),
             file_id="<string>",
         ),
     )
 
     # OR if you need more info (e.g. status_code)
     cmd.sync_detailed(
         client=client,
         body=ModelingCmdReq(
-            cmd=Line3d(
-                from_=Point3d(
-                    x=3.14,
-                    y=3.14,
-                    z=3.14,
-                ),
-                to=Point3d(
-                    x=3.14,
-                    y=3.14,
-                    z=3.14,
-                ),
-            ),
+            cmd=ModelingCmd.START_PATH,
             cmd_id=ModelingCmdId("<uuid>"),
             file_id="<string>",
         ),
     )
 
 
 # OR run async
@@ -1448,47 +1425,25 @@
 async def test_cmd_async():
     # Create our client.
     client = ClientFromEnv()
 
     await cmd.asyncio(
         client=client,
         body=ModelingCmdReq(
-            cmd=Line3d(
-                from_=Point3d(
-                    x=3.14,
-                    y=3.14,
-                    z=3.14,
-                ),
-                to=Point3d(
-                    x=3.14,
-                    y=3.14,
-                    z=3.14,
-                ),
-            ),
+            cmd=ModelingCmd.START_PATH,
             cmd_id=ModelingCmdId("<uuid>"),
             file_id="<string>",
         ),
     )
 
     # OR run async with more info
     await cmd.asyncio_detailed(
         client=client,
         body=ModelingCmdReq(
-            cmd=Line3d(
-                from_=Point3d(
-                    x=3.14,
-                    y=3.14,
-                    z=3.14,
-                ),
-                to=Point3d(
-                    x=3.14,
-                    y=3.14,
-                    z=3.14,
-                ),
-            ),
+            cmd=ModelingCmd.START_PATH,
             cmd_id=ModelingCmdId("<uuid>"),
             file_id="<string>",
         ),
     )
 
 
 @pytest.mark.skip
@@ -1497,26 +1452,15 @@
     client = ClientFromEnv()
 
     result: Optional[Union[ModelingOutcomes, Error]] = cmd_batch.sync(
         client=client,
         body=ModelingCmdReqBatch(
             cmds={
                 "<string>": ModelingCmdReq(
-                    cmd=Line3d(
-                        from_=Point3d(
-                            x=3.14,
-                            y=3.14,
-                            z=3.14,
-                        ),
-                        to=Point3d(
-                            x=3.14,
-                            y=3.14,
-                            z=3.14,
-                        ),
-                    ),
+                    cmd=ModelingCmd.START_PATH,
                     cmd_id=ModelingCmdId("<uuid>"),
                     file_id="<string>",
                 )
             },
             file_id="<string>",
         ),
     )
@@ -1532,26 +1476,15 @@
     response: Response[
         Optional[Union[ModelingOutcomes, Error]]
     ] = cmd_batch.sync_detailed(
         client=client,
         body=ModelingCmdReqBatch(
             cmds={
                 "<string>": ModelingCmdReq(
-                    cmd=Line3d(
-                        from_=Point3d(
-                            x=3.14,
-                            y=3.14,
-                            z=3.14,
-                        ),
-                        to=Point3d(
-                            x=3.14,
-                            y=3.14,
-                            z=3.14,
-                        ),
-                    ),
+                    cmd=ModelingCmd.START_PATH,
                     cmd_id=ModelingCmdId("<uuid>"),
                     file_id="<string>",
                 )
             },
             file_id="<string>",
         ),
     )
@@ -1565,26 +1498,15 @@
     client = ClientFromEnv()
 
     result: Optional[Union[ModelingOutcomes, Error]] = await cmd_batch.asyncio(
         client=client,
         body=ModelingCmdReqBatch(
             cmds={
                 "<string>": ModelingCmdReq(
-                    cmd=Line3d(
-                        from_=Point3d(
-                            x=3.14,
-                            y=3.14,
-                            z=3.14,
-                        ),
-                        to=Point3d(
-                            x=3.14,
-                            y=3.14,
-                            z=3.14,
-                        ),
-                    ),
+                    cmd=ModelingCmd.START_PATH,
                     cmd_id=ModelingCmdId("<uuid>"),
                     file_id="<string>",
                 )
             },
             file_id="<string>",
         ),
     )
@@ -1593,26 +1515,15 @@
     response: Response[
         Optional[Union[ModelingOutcomes, Error]]
     ] = await cmd_batch.asyncio_detailed(
         client=client,
         body=ModelingCmdReqBatch(
             cmds={
                 "<string>": ModelingCmdReq(
-                    cmd=Line3d(
-                        from_=Point3d(
-                            x=3.14,
-                            y=3.14,
-                            z=3.14,
-                        ),
-                        to=Point3d(
-                            x=3.14,
-                            y=3.14,
-                            z=3.14,
-                        ),
-                    ),
+                    cmd=ModelingCmd.START_PATH,
                     cmd_id=ModelingCmdId("<uuid>"),
                     file_id="<string>",
                 )
             },
             file_id="<string>",
         ),
     )
```

### Comparing `kittycad-0.4.3/kittycad/models/__init__.py` & `kittycad-0.4.4/kittycad/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,30 +15,36 @@
 from .api_token import ApiToken
 from .api_token_results_page import ApiTokenResultsPage
 from .app_client_info import AppClientInfo
 from .async_api_call import AsyncApiCall
 from .async_api_call_output import AsyncApiCallOutput
 from .async_api_call_results_page import AsyncApiCallResultsPage
 from .async_api_call_type import AsyncApiCallType
+from .axis import Axis
+from .axis_direction_pair import AxisDirectionPair
 from .billing_info import BillingInfo
 from .cache_metadata import CacheMetadata
+from .camera_drag_interaction_type import CameraDragInteractionType
 from .card_details import CardDetails
 from .cluster import Cluster
 from .code_language import CodeLanguage
 from .code_output import CodeOutput
 from .commit import Commit
 from .connection import Connection
 from .country_code import CountryCode
+from .coupon import Coupon
 from .created_at_sort_mode import CreatedAtSortMode
 from .currency import Currency
 from .customer import Customer
 from .customer_balance import CustomerBalance
 from .device_access_token_request_form import DeviceAccessTokenRequestForm
 from .device_auth_request_form import DeviceAuthRequestForm
 from .device_auth_verify_params import DeviceAuthVerifyParams
+from .direction import Direction
+from .discount import Discount
 from .docker_system_info import DockerSystemInfo
 from .email_authentication_form import EmailAuthenticationForm
 from .engine_metadata import EngineMetadata
 from .environment import Environment
 from .error import Error
 from .executor_metadata import ExecutorMetadata
 from .extended_user import ExtendedUser
@@ -52,23 +58,23 @@
 from .file_mass import FileMass
 from .file_surface_area import FileSurfaceArea
 from .file_system_metadata import FileSystemMetadata
 from .file_volume import FileVolume
 from .gateway import Gateway
 from .image_type import ImageType
 from .index_info import IndexInfo
+from .input_format import InputFormat
 from .invoice import Invoice
 from .invoice_line_item import InvoiceLineItem
 from .invoice_status import InvoiceStatus
 from .jetstream import Jetstream
 from .jetstream_api_stats import JetstreamApiStats
 from .jetstream_config import JetstreamConfig
 from .jetstream_stats import JetstreamStats
 from .leaf_node import LeafNode
-from .line3d import Line3d
 from .mesh import Mesh
 from .meta_cluster_info import MetaClusterInfo
 from .metadata import Metadata
 from .method import Method
 from .modeling_cmd import ModelingCmd
 from .modeling_cmd_id import ModelingCmdId
 from .modeling_cmd_req import ModelingCmdReq
@@ -77,28 +83,32 @@
 from .modeling_outcome import ModelingOutcome
 from .modeling_outcomes import ModelingOutcomes
 from .new_address import NewAddress
 from .o_auth2_client_info import OAuth2ClientInfo
 from .o_auth2_grant_type import OAuth2GrantType
 from .onboarding import Onboarding
 from .output_file import OutputFile
+from .output_format import OutputFormat
+from .path_segment import PathSegment
 from .payment_intent import PaymentIntent
 from .payment_method import PaymentMethod
 from .payment_method_card_checks import PaymentMethodCardChecks
 from .payment_method_type import PaymentMethodType
 from .physics_constant import PhysicsConstant
 from .physics_constant_name import PhysicsConstantName
 from .plugins_info import PluginsInfo
 from .point2d import Point2d
 from .point3d import Point3d
 from .point_e_metadata import PointEMetadata
 from .pong import Pong
 from .registry_service_config import RegistryServiceConfig
 from .runtime import Runtime
 from .session import Session
+from .storage import Storage
+from .system import System
 from .system_info_cgroup_driver_enum import SystemInfoCgroupDriverEnum
 from .system_info_cgroup_version_enum import SystemInfoCgroupVersionEnum
 from .system_info_default_address_pools import SystemInfoDefaultAddressPools
 from .system_info_isolation_enum import SystemInfoIsolationEnum
 from .unit_angle import UnitAngle
 from .unit_angle_conversion import UnitAngleConversion
 from .unit_area import UnitArea
```

### Comparing `kittycad-0.4.3/kittycad/models/ai_plugin_api.py` & `kittycad-0.4.4/kittycad/models/ai_plugin_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         is_user_authenticated = d.pop("is_user_authenticated", UNSET)
 
         _type = d.pop("type", UNSET)
         type: Union[Unset, AiPluginApiType]
         if isinstance(_type, Unset):
             type = UNSET
         else:
-            type = AiPluginApiType(_type)
+            type = _type  # type: ignore[arg-type]
 
         url = d.pop("url", UNSET)
 
         ai_plugin_api = cls(
             is_user_authenticated=is_user_authenticated,
             type=type,
             url=url,
```

### Comparing `kittycad-0.4.3/kittycad/models/ai_plugin_auth.py` & `kittycad-0.4.4/kittycad/models/ai_plugin_auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,22 +38,22 @@
     def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
         d = src_dict.copy()
         _authorization_type = d.pop("authorization_type", UNSET)
         authorization_type: Union[Unset, AiPluginHttpAuthType]
         if isinstance(_authorization_type, Unset):
             authorization_type = UNSET
         else:
-            authorization_type = AiPluginHttpAuthType(_authorization_type)
+            authorization_type = _authorization_type  # type: ignore[arg-type]
 
         _type = d.pop("type", UNSET)
         type: Union[Unset, AiPluginAuthType]
         if isinstance(_type, Unset):
             type = UNSET
         else:
-            type = AiPluginAuthType(_type)
+            type = _type  # type: ignore[arg-type]
 
         ai_plugin_auth = cls(
             authorization_type=authorization_type,
             type=type,
         )
 
         ai_plugin_auth.additional_properties = d
```

### Comparing `kittycad-0.4.3/kittycad/models/ai_plugin_manifest.py` & `kittycad-0.4.4/kittycad/models/ai_plugin_manifest.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/api_call_query_group.py` & `kittycad-0.4.4/kittycad/models/api_call_query_group.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/api_call_query_group_by.py` & `kittycad-0.4.4/kittycad/models/api_call_query_group_by.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/api_call_status.py` & `kittycad-0.4.4/kittycad/models/api_call_status.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/api_call_with_price.py` & `kittycad-0.4.4/kittycad/models/api_call_with_price.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         litterbox = d.pop("litterbox", UNSET)
 
         _method = d.pop("method", UNSET)
         method: Union[Unset, Method]
         if isinstance(_method, Unset):
             method = UNSET
         else:
-            method = Method(_method)
+            method = _method  # type: ignore[arg-type]
 
         minutes = d.pop("minutes", UNSET)
 
         origin = d.pop("origin", UNSET)
 
         price = d.pop("price", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/api_call_with_price_results_page.py` & `kittycad-0.4.4/kittycad/models/api_call_with_price_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/api_token.py` & `kittycad-0.4.4/kittycad/models/api_token.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/api_token_results_page.py` & `kittycad-0.4.4/kittycad/models/api_token_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/app_client_info.py` & `kittycad-0.4.4/kittycad/models/app_client_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/async_api_call.py` & `kittycad-0.4.4/kittycad/models/async_api_call.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,22 +121,22 @@
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         _type = d.pop("type", UNSET)
         type: Union[Unset, AsyncApiCallType]
         if isinstance(_type, Unset):
             type = UNSET
         else:
-            type = AsyncApiCallType(_type)
+            type = _type  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
```

### Comparing `kittycad-0.4.3/kittycad/models/async_api_call_output.py` & `kittycad-0.4.4/kittycad/models/async_api_call_output.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.file_export_format import FileExportFormat
 from ..models.file_import_format import FileImportFormat
+from ..models.input_format import InputFormat
+from ..models.output_format import OutputFormat
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
 F = TypeVar("F", bound="FileConversion")
 
 
 @attr.s(auto_attribs=True)
@@ -19,15 +21,18 @@
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     output: Union[Unset, str] = UNSET
     output_format: Union[Unset, FileExportFormat] = UNSET
+    output_format_options: Union[Unset, OutputFormat] = UNSET
+    outputs: Union[Unset, Any] = UNSET
     src_format: Union[Unset, FileImportFormat] = UNSET
+    src_format_options: Union[Unset, InputFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     type: Union[Unset, str] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -40,16 +45,21 @@
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
         output = self.output
         if not isinstance(self.output_format, Unset):
             output_format = self.output_format
+        if not isinstance(self.output_format_options, Unset):
+            output_format_options = self.output_format_options
+        outputs = self.outputs
         if not isinstance(self.src_format, Unset):
             src_format = self.src_format
+        if not isinstance(self.src_format_options, Unset):
+            src_format_options = self.src_format_options
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         type = self.type
         updated_at: Union[Unset, str] = UNSET
@@ -68,16 +78,22 @@
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
         if output is not UNSET:
             field_dict["output"] = output
         if output_format is not UNSET:
             field_dict["output_format"] = output_format
+        if output_format_options is not UNSET:
+            field_dict["output_format_options"] = output_format_options
+        if outputs is not UNSET:
+            field_dict["outputs"] = outputs
         if src_format is not UNSET:
             field_dict["src_format"] = src_format
+        if src_format_options is not UNSET:
+            field_dict["src_format_options"] = src_format_options
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if type is not UNSET:
             field_dict["type"] = type
         if updated_at is not UNSET:
@@ -116,36 +132,51 @@
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, FileExportFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = FileExportFormat(_output_format)
+            output_format = _output_format  # type: ignore[arg-type]
 
+        _output_format_options = d.pop("output_format_options", UNSET)
+        output_format_options: Union[Unset, OutputFormat]
+        if isinstance(_output_format_options, Unset):
+            output_format_options = UNSET
+        else:
+            output_format_options = OutputFormat(_output_format_options)
+
+        outputs = d.pop("outputs", UNSET)
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = FileImportFormat(_src_format)
+            src_format = _src_format  # type: ignore[arg-type]
+
+        _src_format_options = d.pop("src_format_options", UNSET)
+        src_format_options: Union[Unset, InputFormat]
+        if isinstance(_src_format_options, Unset):
+            src_format_options = UNSET
+        else:
+            src_format_options = InputFormat(_src_format_options)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         type = d.pop("type", UNSET)
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
@@ -157,15 +188,18 @@
         file_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             output=output,
             output_format=output_format,
+            output_format_options=output_format_options,
+            outputs=outputs,
             src_format=src_format,
+            src_format_options=src_format_options,
             started_at=started_at,
             status=status,
             type=type,
             updated_at=updated_at,
             user_id=user_id,
         )
 
@@ -292,29 +326,29 @@
             id = Uuid(_id)
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = FileImportFormat(_src_format)
+            src_format = _src_format  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         type = d.pop("type", UNSET)
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
@@ -464,29 +498,29 @@
         material_density = d.pop("material_density", UNSET)
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = FileImportFormat(_src_format)
+            src_format = _src_format  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         type = d.pop("type", UNSET)
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
@@ -629,29 +663,29 @@
             id = Uuid(_id)
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = FileImportFormat(_src_format)
+            src_format = _src_format  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         type = d.pop("type", UNSET)
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
@@ -803,29 +837,29 @@
         material_mass = d.pop("material_mass", UNSET)
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = FileImportFormat(_src_format)
+            src_format = _src_format  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         type = d.pop("type", UNSET)
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
@@ -968,29 +1002,29 @@
             id = Uuid(_id)
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = FileImportFormat(_src_format)
+            src_format = _src_format  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         surface_area = d.pop("surface_area", UNSET)
 
         type = d.pop("type", UNSET)
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
```

### Comparing `kittycad-0.4.3/kittycad/models/async_api_call_results_page.py` & `kittycad-0.4.4/kittycad/models/async_api_call_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/async_api_call_type.py` & `kittycad-0.4.4/kittycad/models/async_api_call_type.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/billing_info.py` & `kittycad-0.4.4/kittycad/models/billing_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.new_address import NewAddress
 from ..types import UNSET, Unset
 
-X = TypeVar("X", bound="BillingInfo")
+L = TypeVar("L", bound="BillingInfo")
 
 
 @attr.s(auto_attribs=True)
 class BillingInfo:
     """The billing information for payments."""  # noqa: E501
 
     address: Union[Unset, NewAddress] = UNSET
@@ -33,15 +33,15 @@
             field_dict["name"] = name
         if phone is not UNSET:
             field_dict["phone"] = phone
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[X], src_dict: Dict[str, Any]) -> X:
+    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
         d = src_dict.copy()
         _address = d.pop("address", UNSET)
         address: Union[Unset, NewAddress]
         if isinstance(_address, Unset):
             address = UNSET
         else:
             address = NewAddress(_address)
```

### Comparing `kittycad-0.4.3/kittycad/models/cache_metadata.py` & `kittycad-0.4.4/kittycad/models/cache_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-L = TypeVar("L", bound="CacheMetadata")
+B = TypeVar("B", bound="CacheMetadata")
 
 
 @attr.s(auto_attribs=True)
 class CacheMetadata:
     """Metadata about our cache.
 
     This is mostly used for internal purposes and debugging."""  # noqa: E501
@@ -25,15 +25,15 @@
         field_dict.update({})
         if ok is not UNSET:
             field_dict["ok"] = ok
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
+    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
         d = src_dict.copy()
         ok = d.pop("ok", UNSET)
 
         cache_metadata = cls(
             ok=ok,
         )
```

### Comparing `kittycad-0.4.3/kittycad/models/card_details.py` & `kittycad-0.4.4/kittycad/models/card_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.payment_method_card_checks import PaymentMethodCardChecks
 from ..types import UNSET, Unset
 
-B = TypeVar("B", bound="CardDetails")
+N = TypeVar("N", bound="CardDetails")
 
 
 @attr.s(auto_attribs=True)
 class CardDetails:
     """The card details of a payment method."""  # noqa: E501
 
     brand: Union[Unset, str] = UNSET
@@ -53,15 +53,15 @@
             field_dict["funding"] = funding
         if last4 is not UNSET:
             field_dict["last4"] = last4
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
+    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
         d = src_dict.copy()
         brand = d.pop("brand", UNSET)
 
         _checks = d.pop("checks", UNSET)
         checks: Union[Unset, PaymentMethodCardChecks]
         if isinstance(_checks, Unset):
             checks = UNSET
```

### Comparing `kittycad-0.4.3/kittycad/models/cluster.py` & `kittycad-0.4.4/kittycad/models/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-N = TypeVar("N", bound="Cluster")
+E = TypeVar("E", bound="Cluster")
 
 
 @attr.s(auto_attribs=True)
 class Cluster:
     """Cluster information."""  # noqa: E501
 
     addr: Union[Unset, str] = UNSET
@@ -45,15 +45,15 @@
             field_dict["tls_timeout"] = tls_timeout
         if urls is not UNSET:
             field_dict["urls"] = urls
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
+    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
         d = src_dict.copy()
         addr = d.pop("addr", UNSET)
 
         auth_timeout = d.pop("auth_timeout", UNSET)
 
         cluster_port = d.pop("cluster_port", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/code_output.py` & `kittycad-0.4.4/kittycad/models/code_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-E = TypeVar("E", bound="CodeOutput")
+T = TypeVar("T", bound="CodeOutput")
 
 
 @attr.s(auto_attribs=True)
 class CodeOutput:
     """Output of the code being executed."""  # noqa: E501
 
     from ..models.output_file import OutputFile
@@ -37,15 +37,15 @@
             field_dict["stderr"] = stderr
         if stdout is not UNSET:
             field_dict["stdout"] = stdout
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         from ..models.output_file import OutputFile
 
         output_files = cast(List[OutputFile], d.pop("output_files", UNSET))
 
         stderr = d.pop("stderr", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/commit.py` & `kittycad-0.4.4/kittycad/models/commit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Commit")
+L = TypeVar("L", bound="Commit")
 
 
 @attr.s(auto_attribs=True)
 class Commit:
     """Commit holds the Git-commit (SHA1) that a binary was built from, as reported in the version-string of external tools, such as `containerd`, or `runC`."""  # noqa: E501
 
     expected: Union[Unset, str] = UNSET
@@ -27,15 +27,15 @@
             field_dict["expected"] = expected
         if id is not UNSET:
             field_dict["id"] = id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
         d = src_dict.copy()
         expected = d.pop("expected", UNSET)
 
         id = d.pop("id", UNSET)
 
         commit = cls(
             expected=expected,
```

### Comparing `kittycad-0.4.3/kittycad/models/connection.py` & `kittycad-0.4.4/kittycad/models/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from ..models.cluster import Cluster
 from ..models.gateway import Gateway
 from ..models.jetstream import Jetstream
 from ..models.leaf_node import LeafNode
 from ..types import UNSET, Unset
 
-L = TypeVar("L", bound="Connection")
+M = TypeVar("M", bound="Connection")
 
 
 @attr.s(auto_attribs=True)
 class Connection:
     """Metadata about a pub-sub connection.
 
     This is mostly used for internal purposes and debugging."""  # noqa: E501
@@ -221,15 +221,15 @@
             field_dict["version"] = version
         if write_deadline is not UNSET:
             field_dict["write_deadline"] = write_deadline
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
+    def from_dict(cls: Type[M], src_dict: Dict[str, Any]) -> M:
         d = src_dict.copy()
         auth_timeout = d.pop("auth_timeout", UNSET)
 
         _cluster = d.pop("cluster", UNSET)
         cluster: Union[Unset, Cluster]
         if isinstance(_cluster, Unset):
             cluster = UNSET
```

### Comparing `kittycad-0.4.3/kittycad/models/country_code.py` & `kittycad-0.4.4/kittycad/models/country_code.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/currency.py` & `kittycad-0.4.4/kittycad/models/currency.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/customer.py` & `kittycad-0.4.4/kittycad/models/customer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import attr
 from dateutil.parser import isoparse
 
 from ..models.currency import Currency
 from ..models.new_address import NewAddress
 from ..types import UNSET, Unset
 
-M = TypeVar("M", bound="Customer")
+J = TypeVar("J", bound="Customer")
 
 
 @attr.s(auto_attribs=True)
 class Customer:
     """The resource representing a payment "Customer"."""  # noqa: E501
 
     address: Union[Unset, NewAddress] = UNSET
@@ -67,15 +67,15 @@
             field_dict["name"] = name
         if phone is not UNSET:
             field_dict["phone"] = phone
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[M], src_dict: Dict[str, Any]) -> M:
+    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
         d = src_dict.copy()
         _address = d.pop("address", UNSET)
         address: Union[Unset, NewAddress]
         if isinstance(_address, Unset):
             address = UNSET
         else:
             address = NewAddress(_address)
@@ -90,15 +90,15 @@
             created_at = isoparse(_created_at)
 
         _currency = d.pop("currency", UNSET)
         currency: Union[Unset, Currency]
         if isinstance(_currency, Unset):
             currency = UNSET
         else:
-            currency = Currency(_currency)
+            currency = _currency  # type: ignore[arg-type]
 
         delinquent = d.pop("delinquent", UNSET)
 
         email = d.pop("email", UNSET)
 
         id = d.pop("id", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/customer_balance.py` & `kittycad-0.4.4/kittycad/models/customer_balance.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-N = TypeVar("N", bound="CustomerBalance")
+V = TypeVar("V", bound="CustomerBalance")
 
 
 @attr.s(auto_attribs=True)
 class CustomerBalance:
     """A balance for a user.
 
     This holds information about the financial balance for the user."""  # noqa: E501
@@ -60,15 +60,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
+    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
         d = src_dict.copy()
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
```

### Comparing `kittycad-0.4.3/kittycad/models/device_access_token_request_form.py` & `kittycad-0.4.4/kittycad/models/device_access_token_request_form.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.o_auth2_grant_type import OAuth2GrantType
 from ..types import UNSET, Unset
 
-J = TypeVar("J", bound="DeviceAccessTokenRequestForm")
+F = TypeVar("F", bound="DeviceAccessTokenRequestForm")
 
 
 @attr.s(auto_attribs=True)
 class DeviceAccessTokenRequestForm:
     """The form for a device access token request."""  # noqa: E501
 
     client_id: Union[Unset, str] = UNSET
@@ -33,26 +33,26 @@
             field_dict["device_code"] = device_code
         if grant_type is not UNSET:
             field_dict["grant_type"] = grant_type
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
+    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
         d = src_dict.copy()
         client_id = d.pop("client_id", UNSET)
 
         device_code = d.pop("device_code", UNSET)
 
         _grant_type = d.pop("grant_type", UNSET)
         grant_type: Union[Unset, OAuth2GrantType]
         if isinstance(_grant_type, Unset):
             grant_type = UNSET
         else:
-            grant_type = OAuth2GrantType(_grant_type)
+            grant_type = _grant_type  # type: ignore[arg-type]
 
         device_access_token_request_form = cls(
             client_id=client_id,
             device_code=device_code,
             grant_type=grant_type,
         )
```

### Comparing `kittycad-0.4.3/kittycad/models/device_auth_request_form.py` & `kittycad-0.4.4/kittycad/models/device_auth_request_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/device_auth_verify_params.py` & `kittycad-0.4.4/kittycad/models/device_auth_verify_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-F = TypeVar("F", bound="DeviceAuthVerifyParams")
+J = TypeVar("J", bound="DeviceAuthVerifyParams")
 
 
 @attr.s(auto_attribs=True)
 class DeviceAuthVerifyParams:
     """The request parameters to verify the `user_code` for the OAuth 2.0 Device Authorization Grant."""  # noqa: E501
 
     user_code: Union[Unset, str] = UNSET
@@ -23,15 +23,15 @@
         field_dict.update({})
         if user_code is not UNSET:
             field_dict["user_code"] = user_code
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
+    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
         d = src_dict.copy()
         user_code = d.pop("user_code", UNSET)
 
         device_auth_verify_params = cls(
             user_code=user_code,
         )
```

### Comparing `kittycad-0.4.3/kittycad/models/docker_system_info.py` & `kittycad-0.4.4/kittycad/models/docker_system_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ..models.plugins_info import PluginsInfo
 from ..models.registry_service_config import RegistryServiceConfig
 from ..models.system_info_cgroup_driver_enum import SystemInfoCgroupDriverEnum
 from ..models.system_info_cgroup_version_enum import SystemInfoCgroupVersionEnum
 from ..models.system_info_isolation_enum import SystemInfoIsolationEnum
 from ..types import UNSET, Unset
 
-V = TypeVar("V", bound="DockerSystemInfo")
+L = TypeVar("L", bound="DockerSystemInfo")
 
 
 @attr.s(auto_attribs=True)
 class DockerSystemInfo:
     """Docker system info."""  # noqa: E501
 
     architecture: Union[Unset, str] = UNSET
@@ -289,15 +289,15 @@
             field_dict["system_time"] = system_time
         if warnings is not UNSET:
             field_dict["warnings"] = warnings
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
+    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
         d = src_dict.copy()
         architecture = d.pop("architecture", UNSET)
 
         bridge_nf_ip6tables = d.pop("bridge_nf_ip6tables", UNSET)
 
         bridge_nf_iptables = d.pop("bridge_nf_iptables", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/email_authentication_form.py` & `kittycad-0.4.4/kittycad/models/email_authentication_form.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-J = TypeVar("J", bound="EmailAuthenticationForm")
+E = TypeVar("E", bound="EmailAuthenticationForm")
 
 
 @attr.s(auto_attribs=True)
 class EmailAuthenticationForm:
     """The body of the form for email authentication."""  # noqa: E501
 
     callback_url: Union[Unset, str] = UNSET
@@ -27,15 +27,15 @@
             field_dict["callback_url"] = callback_url
         if email is not UNSET:
             field_dict["email"] = email
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
+    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
         d = src_dict.copy()
         callback_url = d.pop("callback_url", UNSET)
 
         email = d.pop("email", UNSET)
 
         email_authentication_form = cls(
             callback_url=callback_url,
```

### Comparing `kittycad-0.4.3/kittycad/models/engine_metadata.py` & `kittycad-0.4.4/kittycad/models/engine_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..models.cache_metadata import CacheMetadata
 from ..models.connection import Connection
 from ..models.environment import Environment
 from ..models.file_system_metadata import FileSystemMetadata
 from ..types import UNSET, Unset
 
-V = TypeVar("V", bound="EngineMetadata")
+Y = TypeVar("Y", bound="EngineMetadata")
 
 
 @attr.s(auto_attribs=True)
 class EngineMetadata:
     """Metadata about our currently running server.
 
     This is mostly used for internal purposes and debugging."""  # noqa: E501
@@ -53,15 +53,15 @@
             field_dict["git_hash"] = git_hash
         if pubsub is not UNSET:
             field_dict["pubsub"] = pubsub
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
+    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
         d = src_dict.copy()
         async_jobs_running = d.pop("async_jobs_running", UNSET)
 
         _cache = d.pop("cache", UNSET)
         cache: Union[Unset, CacheMetadata]
         if isinstance(_cache, Unset):
             cache = UNSET
@@ -69,15 +69,15 @@
             cache = CacheMetadata(_cache)
 
         _environment = d.pop("environment", UNSET)
         environment: Union[Unset, Environment]
         if isinstance(_environment, Unset):
             environment = UNSET
         else:
-            environment = Environment(_environment)
+            environment = _environment  # type: ignore[arg-type]
 
         _fs = d.pop("fs", UNSET)
         fs: Union[Unset, FileSystemMetadata]
         if isinstance(_fs, Unset):
             fs = UNSET
         else:
             fs = FileSystemMetadata(_fs)
```

### Comparing `kittycad-0.4.3/kittycad/models/environment.py` & `kittycad-0.4.4/kittycad/models/environment.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/error.py` & `kittycad-0.4.4/kittycad/models/error.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-L = TypeVar("L", bound="Error")
+H = TypeVar("H", bound="Error")
 
 
 @attr.s(auto_attribs=True)
 class Error:
     """Error information from a response."""  # noqa: E501
 
     error_code: Union[Unset, str] = UNSET
@@ -31,15 +31,15 @@
             field_dict["message"] = message
         if request_id is not UNSET:
             field_dict["request_id"] = request_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         error_code = d.pop("error_code", UNSET)
 
         message = d.pop("message", UNSET)
 
         request_id = d.pop("request_id", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/executor_metadata.py` & `kittycad-0.4.4/kittycad/models/executor_metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import attr
 
 from ..models.docker_system_info import DockerSystemInfo
 from ..models.environment import Environment
 from ..types import UNSET, Unset
 
-E = TypeVar("E", bound="ExecutorMetadata")
+T = TypeVar("T", bound="ExecutorMetadata")
 
 
 @attr.s(auto_attribs=True)
 class ExecutorMetadata:
     """Metadata about our currently running server.
 
     This is mostly used for internal purposes and debugging."""  # noqa: E501
@@ -37,29 +37,29 @@
             field_dict["environment"] = environment
         if git_hash is not UNSET:
             field_dict["git_hash"] = git_hash
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _docker_info = d.pop("docker_info", UNSET)
         docker_info: Union[Unset, DockerSystemInfo]
         if isinstance(_docker_info, Unset):
             docker_info = UNSET
         else:
             docker_info = DockerSystemInfo(_docker_info)
 
         _environment = d.pop("environment", UNSET)
         environment: Union[Unset, Environment]
         if isinstance(_environment, Unset):
             environment = UNSET
         else:
-            environment = Environment(_environment)
+            environment = _environment  # type: ignore[arg-type]
 
         git_hash = d.pop("git_hash", UNSET)
 
         executor_metadata = cls(
             docker_info=docker_info,
             environment=environment,
             git_hash=git_hash,
```

### Comparing `kittycad-0.4.3/kittycad/models/extended_user.py` & `kittycad-0.4.4/kittycad/models/extended_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
-Y = TypeVar("Y", bound="ExtendedUser")
+M = TypeVar("M", bound="ExtendedUser")
 
 
 @attr.s(auto_attribs=True)
 class ExtendedUser:
     """Extended user information.
 
     This is mostly used for internal purposes. It returns a mapping of the user's information, including that of our third party services we use for users: MailChimp, Stripe, and Front"""  # noqa: E501
@@ -93,15 +93,15 @@
             field_dict["stripe_id"] = stripe_id
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
+    def from_dict(cls: Type[M], src_dict: Dict[str, Any]) -> M:
         d = src_dict.copy()
         company = d.pop("company", UNSET)
 
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
```

### Comparing `kittycad-0.4.3/kittycad/models/extended_user_results_page.py` & `kittycad-0.4.4/kittycad/models/extended_user_results_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="ExtendedUserResultsPage")
+B = TypeVar("B", bound="ExtendedUserResultsPage")
 
 
 @attr.s(auto_attribs=True)
 class ExtendedUserResultsPage:
     """A single page of results"""  # noqa: E501
 
     from ..models.extended_user import ExtendedUser
@@ -33,15 +33,15 @@
             field_dict["items"] = items
         if next_page is not UNSET:
             field_dict["next_page"] = next_page
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
         d = src_dict.copy()
         from ..models.extended_user import ExtendedUser
 
         items = cast(List[ExtendedUser], d.pop("items", UNSET))
 
         next_page = d.pop("next_page", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/extrude.py` & `kittycad-0.4.4/kittycad/models/extrude.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,61 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.modeling_cmd_id import ModelingCmdId
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Extrude")
+S = TypeVar("S", bound="Extrude")
 
 
 @attr.s(auto_attribs=True)
 class Extrude:
     """Command for extruding a solid."""  # noqa: E501
 
+    cap: Union[Unset, bool] = False
     distance: Union[Unset, float] = UNSET
     target: Union[Unset, ModelingCmdId] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        cap = self.cap
         distance = self.distance
         if not isinstance(self.target, Unset):
             target = self.target
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
+        if cap is not UNSET:
+            field_dict["cap"] = cap
         if distance is not UNSET:
             field_dict["distance"] = distance
         if target is not UNSET:
             field_dict["target"] = target
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
         d = src_dict.copy()
+        cap = d.pop("cap", UNSET)
+
         distance = d.pop("distance", UNSET)
 
         _target = d.pop("target", UNSET)
         target: Union[Unset, ModelingCmdId]
         if isinstance(_target, Unset):
             target = UNSET
         else:
             target = ModelingCmdId(_target)
 
         extrude = cls(
+            cap=cap,
             distance=distance,
             target=target,
         )
 
         extrude.additional_properties = d
         return extrude
```

### Comparing `kittycad-0.4.3/kittycad/models/file_center_of_mass.py` & `kittycad-0.4.4/kittycad/models/file_center_of_mass.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.file_import_format import FileImportFormat
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-M = TypeVar("M", bound="FileCenterOfMass")
+A = TypeVar("A", bound="FileCenterOfMass")
 
 
 @attr.s(auto_attribs=True)
 class FileCenterOfMass:
     """A file center of mass result."""  # noqa: E501
 
     center_of_mass: Union[Unset, List[float]] = UNSET
@@ -76,15 +76,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[M], src_dict: Dict[str, Any]) -> M:
+    def from_dict(cls: Type[A], src_dict: Dict[str, Any]) -> A:
         d = src_dict.copy()
         center_of_mass = cast(List[float], d.pop("center_of_mass", UNSET))
 
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
@@ -108,29 +108,29 @@
             id = Uuid(_id)
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = FileImportFormat(_src_format)
+            src_format = _src_format  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
```

### Comparing `kittycad-0.4.3/kittycad/models/file_conversion.py` & `kittycad-0.4.4/kittycad/models/file_density.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.file_export_format import FileExportFormat
 from ..models.file_import_format import FileImportFormat
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-B = TypeVar("B", bound="FileConversion")
+E = TypeVar("E", bound="FileDensity")
 
 
 @attr.s(auto_attribs=True)
-class FileConversion:
-    """A file conversion."""  # noqa: E501
+class FileDensity:
+    """A file density result."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
+    density: Union[Unset, float] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
-    output: Union[Unset, str] = UNSET
-    output_format: Union[Unset, FileExportFormat] = UNSET
+    material_mass: Union[Unset, float] = UNSET
     src_format: Union[Unset, FileImportFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -34,19 +33,18 @@
     def to_dict(self) -> Dict[str, Any]:
         completed_at: Union[Unset, str] = UNSET
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
+        density = self.density
         error = self.error
         id = self.id
-        output = self.output
-        if not isinstance(self.output_format, Unset):
-            output_format = self.output_format
+        material_mass = self.material_mass
         if not isinstance(self.src_format, Unset):
             src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
@@ -58,37 +56,37 @@
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
             field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
+        if density is not UNSET:
+            field_dict["density"] = density
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
-        if output is not UNSET:
-            field_dict["output"] = output
-        if output_format is not UNSET:
-            field_dict["output_format"] = output_format
+        if material_mass is not UNSET:
+            field_dict["material_mass"] = material_mass
         if src_format is not UNSET:
             field_dict["src_format"] = src_format
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
+    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -96,78 +94,73 @@
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
+        density = d.pop("density", UNSET)
+
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
             id = Uuid(_id)
 
-        output = d.pop("output", UNSET)
-
-        _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, FileExportFormat]
-        if isinstance(_output_format, Unset):
-            output_format = UNSET
-        else:
-            output_format = FileExportFormat(_output_format)
+        material_mass = d.pop("material_mass", UNSET)
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = FileImportFormat(_src_format)
+            src_format = _src_format  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        file_conversion = cls(
+        file_density = cls(
             completed_at=completed_at,
             created_at=created_at,
+            density=density,
             error=error,
             id=id,
-            output=output,
-            output_format=output_format,
+            material_mass=material_mass,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        file_conversion.additional_properties = d
-        return file_conversion
+        file_density.additional_properties = d
+        return file_density
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.3/kittycad/models/file_density.py` & `kittycad-0.4.4/kittycad/models/file_mass.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.file_import_format import FileImportFormat
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-S = TypeVar("S", bound="FileDensity")
+G = TypeVar("G", bound="FileMass")
 
 
 @attr.s(auto_attribs=True)
-class FileDensity:
-    """A file density result."""  # noqa: E501
+class FileMass:
+    """A file mass result."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
-    density: Union[Unset, float] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
-    material_mass: Union[Unset, float] = UNSET
+    mass: Union[Unset, float] = UNSET
+    material_density: Union[Unset, float] = UNSET
     src_format: Union[Unset, FileImportFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -33,18 +33,18 @@
     def to_dict(self) -> Dict[str, Any]:
         completed_at: Union[Unset, str] = UNSET
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
-        density = self.density
         error = self.error
         id = self.id
-        material_mass = self.material_mass
+        mass = self.mass
+        material_density = self.material_density
         if not isinstance(self.src_format, Unset):
             src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
@@ -56,37 +56,37 @@
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
             field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
-        if density is not UNSET:
-            field_dict["density"] = density
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
-        if material_mass is not UNSET:
-            field_dict["material_mass"] = material_mass
+        if mass is not UNSET:
+            field_dict["mass"] = mass
+        if material_density is not UNSET:
+            field_dict["material_density"] = material_density
         if src_format is not UNSET:
             field_dict["src_format"] = src_format
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
+    def from_dict(cls: Type[G], src_dict: Dict[str, Any]) -> G:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -94,73 +94,73 @@
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        density = d.pop("density", UNSET)
-
         error = d.pop("error", UNSET)
 
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
             id = Uuid(_id)
 
-        material_mass = d.pop("material_mass", UNSET)
+        mass = d.pop("mass", UNSET)
+
+        material_density = d.pop("material_density", UNSET)
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = FileImportFormat(_src_format)
+            src_format = _src_format  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        file_density = cls(
+        file_mass = cls(
             completed_at=completed_at,
             created_at=created_at,
-            density=density,
             error=error,
             id=id,
-            material_mass=material_mass,
+            mass=mass,
+            material_density=material_density,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        file_density.additional_properties = d
-        return file_density
+        file_mass.additional_properties = d
+        return file_mass
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.3/kittycad/models/file_export_format.py` & `kittycad-0.4.4/kittycad/models/file_export_format.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,17 @@
     DAE = "dae"
     """# The DXF file format. <https://en.wikipedia.org/wiki/AutoCAD_DXF> """  # noqa: E501
     DXF = "dxf"
     """# The FBX file format. <https://en.wikipedia.org/wiki/FBX> """  # noqa: E501
     FBX = "fbx"
     """# The FBX file format (in binary). <https://en.wikipedia.org/wiki/FBX> """  # noqa: E501
     FBXB = "fbxb"
-    """# The OBJ file format. A zip file containing both the obj file itself and its associated mtl file for full processing. <https://en.wikipedia.org/wiki/Wavefront_.obj_file>> The OBJ file format. <https://en.wikipedia.org/wiki/Wavefront_.obj_file> It may or may not have an an attached material (mtl // mtllib) within the file, but we interact with it as if it does not. """  # noqa: E501
+    """# glTF 2.0. We refer to this as glTF since that is how our customers refer to it, although by default it will be in binary format and thus technically (glb). """  # noqa: E501
+    GLTF = "gltf"
+    """# The OBJ file format. <https://en.wikipedia.org/wiki/Wavefront_.obj_file> It may or may not have an an attached material (mtl // mtllib) within the file, but we interact with it as if it does not. """  # noqa: E501
     OBJ = "obj"
     """# The PLY file format. <https://en.wikipedia.org/wiki/PLY_(file_format)> """  # noqa: E501
     PLY = "ply"
     """# The STEP file format. <https://en.wikipedia.org/wiki/ISO_10303-21> """  # noqa: E501
     STEP = "step"
     """# The STL file format. <https://en.wikipedia.org/wiki/STL_(file_format)> """  # noqa: E501
     STL = "stl"
```

### Comparing `kittycad-0.4.3/kittycad/models/file_import_format.py` & `kittycad-0.4.4/kittycad/models/file_import_format.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
     """# The COLLADA/DAE file format. <https://en.wikipedia.org/wiki/COLLADA> """  # noqa: E501
     DAE = "dae"
     """# The DXF file format. <https://en.wikipedia.org/wiki/AutoCAD_DXF> """  # noqa: E501
     DXF = "dxf"
     """# The FBX file format. <https://en.wikipedia.org/wiki/FBX> """  # noqa: E501
     FBX = "fbx"
-    """# The OBJ file format. A zip file containing both the obj file itself and its associated mtl file for full processing. <https://en.wikipedia.org/wiki/Wavefront_.obj_file>> """  # noqa: E501
-    OBJ_ZIP = "obj_zip"
+    """# glTF 2.0. """  # noqa: E501
+    GLTF = "gltf"
     """# The OBJ file format. <https://en.wikipedia.org/wiki/Wavefront_.obj_file> It may or may not have an an attached material (mtl // mtllib) within the file, but we interact with it as if it does not. """  # noqa: E501
     OBJ = "obj"
     """# The PLY file format. <https://en.wikipedia.org/wiki/PLY_(file_format)> """  # noqa: E501
     PLY = "ply"
     """# The STEP file format. <https://en.wikipedia.org/wiki/ISO_10303-21> """  # noqa: E501
     STEP = "step"
     """# The STL file format. <https://en.wikipedia.org/wiki/STL_(file_format)> """  # noqa: E501
```

### Comparing `kittycad-0.4.3/kittycad/models/file_mass.py` & `kittycad-0.4.4/kittycad/models/file_volume.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,88 +5,84 @@
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.file_import_format import FileImportFormat
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-A = TypeVar("A", bound="FileMass")
+L = TypeVar("L", bound="FileVolume")
 
 
 @attr.s(auto_attribs=True)
-class FileMass:
-    """A file mass result."""  # noqa: E501
+class FileVolume:
+    """A file volume result."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
-    mass: Union[Unset, float] = UNSET
-    material_density: Union[Unset, float] = UNSET
     src_format: Union[Unset, FileImportFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
+    volume: Union[Unset, float] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         completed_at: Union[Unset, str] = UNSET
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
-        mass = self.mass
-        material_density = self.material_density
         if not isinstance(self.src_format, Unset):
             src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
+        volume = self.volume
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
             field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
-        if mass is not UNSET:
-            field_dict["mass"] = mass
-        if material_density is not UNSET:
-            field_dict["material_density"] = material_density
         if src_format is not UNSET:
             field_dict["src_format"] = src_format
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
+        if volume is not UNSET:
+            field_dict["volume"] = volume
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[A], src_dict: Dict[str, Any]) -> A:
+    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -103,64 +99,61 @@
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
             id = Uuid(_id)
 
-        mass = d.pop("mass", UNSET)
-
-        material_density = d.pop("material_density", UNSET)
-
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = FileImportFormat(_src_format)
+            src_format = _src_format  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        file_mass = cls(
+        volume = d.pop("volume", UNSET)
+
+        file_volume = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
-            mass=mass,
-            material_density=material_density,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
+            volume=volume,
         )
 
-        file_mass.additional_properties = d
-        return file_mass
+        file_volume.additional_properties = d
+        return file_volume
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.3/kittycad/models/file_surface_area.py` & `kittycad-0.4.4/kittycad/models/file_surface_area.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.file_import_format import FileImportFormat
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="FileSurfaceArea")
+J = TypeVar("J", bound="FileSurfaceArea")
 
 
 @attr.s(auto_attribs=True)
 class FileSurfaceArea:
     """A file surface area result."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -74,15 +74,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -104,29 +104,29 @@
             id = Uuid(_id)
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = FileImportFormat(_src_format)
+            src_format = _src_format  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         surface_area = d.pop("surface_area", UNSET)
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
```

### Comparing `kittycad-0.4.3/kittycad/models/file_system_metadata.py` & `kittycad-0.4.4/kittycad/models/file_system_metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-E = TypeVar("E", bound="FileSystemMetadata")
+R = TypeVar("R", bound="FileSystemMetadata")
 
 
 @attr.s(auto_attribs=True)
 class FileSystemMetadata:
     """Metadata about our file system.
 
     This is mostly used for internal purposes and debugging."""  # noqa: E501
@@ -25,15 +25,15 @@
         field_dict.update({})
         if ok is not UNSET:
             field_dict["ok"] = ok
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
+    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
         d = src_dict.copy()
         ok = d.pop("ok", UNSET)
 
         file_system_metadata = cls(
             ok=ok,
         )
```

### Comparing `kittycad-0.4.3/kittycad/models/file_volume.py` & `kittycad-0.4.4/kittycad/models/physics_constant.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,96 +1,103 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.file_import_format import FileImportFormat
+from ..models.physics_constant_name import PhysicsConstantName
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-G = TypeVar("G", bound="FileVolume")
+H = TypeVar("H", bound="PhysicsConstant")
 
 
 @attr.s(auto_attribs=True)
-class FileVolume:
-    """A file volume result."""  # noqa: E501
+class PhysicsConstant:
+    """A physics constant."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
+    constant: Union[Unset, PhysicsConstantName] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
-    src_format: Union[Unset, FileImportFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
-    volume: Union[Unset, float] = UNSET
+    value: Union[Unset, float] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         completed_at: Union[Unset, str] = UNSET
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
+        if not isinstance(self.constant, Unset):
+            constant = self.constant
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
-        if not isinstance(self.src_format, Unset):
-            src_format = self.src_format
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
-        volume = self.volume
+        value = self.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
             field_dict["completed_at"] = completed_at
+        if constant is not UNSET:
+            field_dict["constant"] = constant
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
-        if src_format is not UNSET:
-            field_dict["src_format"] = src_format
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
-        if volume is not UNSET:
-            field_dict["volume"] = volume
+        if value is not UNSET:
+            field_dict["value"] = value
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[G], src_dict: Dict[str, Any]) -> G:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
 
+        _constant = d.pop("constant", UNSET)
+        constant: Union[Unset, PhysicsConstantName]
+        if isinstance(_constant, Unset):
+            constant = UNSET
+        else:
+            constant = _constant  # type: ignore[arg-type]
+
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
@@ -99,61 +106,54 @@
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
             id = Uuid(_id)
 
-        _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, FileImportFormat]
-        if isinstance(_src_format, Unset):
-            src_format = UNSET
-        else:
-            src_format = FileImportFormat(_src_format)
-
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        volume = d.pop("volume", UNSET)
+        value = d.pop("value", UNSET)
 
-        file_volume = cls(
+        physics_constant = cls(
             completed_at=completed_at,
+            constant=constant,
             created_at=created_at,
             error=error,
             id=id,
-            src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
-            volume=volume,
+            value=value,
         )
 
-        file_volume.additional_properties = d
-        return file_volume
+        physics_constant.additional_properties = d
+        return physics_constant
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.3/kittycad/models/gateway.py` & `kittycad-0.4.4/kittycad/models/gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-J = TypeVar("J", bound="Gateway")
+Y = TypeVar("Y", bound="Gateway")
 
 
 @attr.s(auto_attribs=True)
 class Gateway:
     """Gateway information."""  # noqa: E501
 
     auth_timeout: Union[Unset, int] = UNSET
@@ -39,15 +39,15 @@
             field_dict["port"] = port
         if tls_timeout is not UNSET:
             field_dict["tls_timeout"] = tls_timeout
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
+    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
         d = src_dict.copy()
         auth_timeout = d.pop("auth_timeout", UNSET)
 
         host = d.pop("host", UNSET)
 
         name = d.pop("name", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/index_info.py` & `kittycad-0.4.4/kittycad/models/index_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-R = TypeVar("R", bound="IndexInfo")
+H = TypeVar("H", bound="IndexInfo")
 
 
 @attr.s(auto_attribs=True)
 class IndexInfo:
     """IndexInfo contains information about a registry."""  # noqa: E501
 
     mirrors: Union[Unset, List[str]] = UNSET
@@ -37,15 +37,15 @@
             field_dict["official"] = official
         if secure is not UNSET:
             field_dict["secure"] = secure
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         mirrors = cast(List[str], d.pop("mirrors", UNSET))
 
         name = d.pop("name", UNSET)
 
         official = d.pop("official", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/invoice.py` & `kittycad-0.4.4/kittycad/models/invoice.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import attr
 from dateutil.parser import isoparse
 
 from ..models.currency import Currency
 from ..models.invoice_status import InvoiceStatus
 from ..types import UNSET, Unset
 
-L = TypeVar("L", bound="Invoice")
+P = TypeVar("P", bound="Invoice")
 
 
 @attr.s(auto_attribs=True)
 class Invoice:
     """An invoice."""  # noqa: E501
 
     amount_due: Union[Unset, float] = UNSET
@@ -22,14 +22,17 @@
     attempted: Union[Unset, bool] = False
     created_at: Union[Unset, datetime.datetime] = UNSET
     currency: Union[Unset, Currency] = UNSET
     customer_email: Union[Unset, str] = UNSET
     customer_id: Union[Unset, str] = UNSET
     default_payment_method: Union[Unset, str] = UNSET
     description: Union[Unset, str] = UNSET
+    from ..models.discount import Discount
+
+    discounts: Union[Unset, List[Discount]] = UNSET
     id: Union[Unset, str] = UNSET
     from ..models.invoice_line_item import InvoiceLineItem
 
     lines: Union[Unset, List[InvoiceLineItem]] = UNSET
     metadata: Union[Unset, Any] = UNSET
     number: Union[Unset, str] = UNSET
     paid: Union[Unset, bool] = False
@@ -55,14 +58,19 @@
             created_at = self.created_at.isoformat()
         if not isinstance(self.currency, Unset):
             currency = self.currency
         customer_email = self.customer_email
         customer_id = self.customer_id
         default_payment_method = self.default_payment_method
         description = self.description
+        from ..models.discount import Discount
+
+        discounts: Union[Unset, List[Discount]] = UNSET
+        if not isinstance(self.discounts, Unset):
+            discounts = self.discounts
         id = self.id
         from ..models.invoice_line_item import InvoiceLineItem
 
         lines: Union[Unset, List[InvoiceLineItem]] = UNSET
         if not isinstance(self.lines, Unset):
             lines = self.lines
         metadata = self.metadata
@@ -99,14 +107,16 @@
             field_dict["customer_email"] = customer_email
         if customer_id is not UNSET:
             field_dict["customer_id"] = customer_id
         if default_payment_method is not UNSET:
             field_dict["default_payment_method"] = default_payment_method
         if description is not UNSET:
             field_dict["description"] = description
+        if discounts is not UNSET:
+            field_dict["discounts"] = discounts
         if id is not UNSET:
             field_dict["id"] = id
         if lines is not UNSET:
             field_dict["lines"] = lines
         if metadata is not UNSET:
             field_dict["metadata"] = metadata
         if number is not UNSET:
@@ -129,15 +139,15 @@
             field_dict["total"] = total
         if url is not UNSET:
             field_dict["url"] = url
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
+    def from_dict(cls: Type[P], src_dict: Dict[str, Any]) -> P:
         d = src_dict.copy()
         amount_due = d.pop("amount_due", UNSET)
 
         amount_paid = d.pop("amount_paid", UNSET)
 
         amount_remaining = d.pop("amount_remaining", UNSET)
 
@@ -153,24 +163,28 @@
             created_at = isoparse(_created_at)
 
         _currency = d.pop("currency", UNSET)
         currency: Union[Unset, Currency]
         if isinstance(_currency, Unset):
             currency = UNSET
         else:
-            currency = Currency(_currency)
+            currency = _currency  # type: ignore[arg-type]
 
         customer_email = d.pop("customer_email", UNSET)
 
         customer_id = d.pop("customer_id", UNSET)
 
         default_payment_method = d.pop("default_payment_method", UNSET)
 
         description = d.pop("description", UNSET)
 
+        from ..models.discount import Discount
+
+        discounts = cast(List[Discount], d.pop("discounts", UNSET))
+
         id = d.pop("id", UNSET)
 
         from ..models.invoice_line_item import InvoiceLineItem
 
         lines = cast(List[InvoiceLineItem], d.pop("lines", UNSET))
 
         metadata = d.pop("metadata", UNSET)
@@ -185,15 +199,15 @@
         statement_descriptor = d.pop("statement_descriptor", UNSET)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, InvoiceStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = InvoiceStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         subtotal = d.pop("subtotal", UNSET)
 
         tax = d.pop("tax", UNSET)
 
         total = d.pop("total", UNSET)
 
@@ -207,14 +221,15 @@
             attempted=attempted,
             created_at=created_at,
             currency=currency,
             customer_email=customer_email,
             customer_id=customer_id,
             default_payment_method=default_payment_method,
             description=description,
+            discounts=discounts,
             id=id,
             lines=lines,
             metadata=metadata,
             number=number,
             paid=paid,
             pdf=pdf,
             receipt_number=receipt_number,
```

### Comparing `kittycad-0.4.3/kittycad/models/invoice_line_item.py` & `kittycad-0.4.4/kittycad/models/invoice_line_item.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.currency import Currency
 from ..types import UNSET, Unset
 
-Y = TypeVar("Y", bound="InvoiceLineItem")
+C = TypeVar("C", bound="InvoiceLineItem")
 
 
 @attr.s(auto_attribs=True)
 class InvoiceLineItem:
     """An invoice line item."""  # noqa: E501
 
     amount: Union[Unset, float] = UNSET
@@ -45,24 +45,24 @@
             field_dict["invoice_item"] = invoice_item
         if metadata is not UNSET:
             field_dict["metadata"] = metadata
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
+    def from_dict(cls: Type[C], src_dict: Dict[str, Any]) -> C:
         d = src_dict.copy()
         amount = d.pop("amount", UNSET)
 
         _currency = d.pop("currency", UNSET)
         currency: Union[Unset, Currency]
         if isinstance(_currency, Unset):
             currency = UNSET
         else:
-            currency = Currency(_currency)
+            currency = _currency  # type: ignore[arg-type]
 
         description = d.pop("description", UNSET)
 
         id = d.pop("id", UNSET)
 
         invoice_item = d.pop("invoice_item", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/invoice_status.py` & `kittycad-0.4.4/kittycad/models/invoice_status.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/jetstream.py` & `kittycad-0.4.4/kittycad/models/jetstream.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import attr
 
 from ..models.jetstream_config import JetstreamConfig
 from ..models.jetstream_stats import JetstreamStats
 from ..models.meta_cluster_info import MetaClusterInfo
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="Jetstream")
+U = TypeVar("U", bound="Jetstream")
 
 
 @attr.s(auto_attribs=True)
 class Jetstream:
     """Jetstream information."""  # noqa: E501
 
     config: Union[Unset, JetstreamConfig] = UNSET
@@ -37,15 +37,15 @@
             field_dict["meta"] = meta
         if stats is not UNSET:
             field_dict["stats"] = stats
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[U], src_dict: Dict[str, Any]) -> U:
         d = src_dict.copy()
         _config = d.pop("config", UNSET)
         config: Union[Unset, JetstreamConfig]
         if isinstance(_config, Unset):
             config = UNSET
         else:
             config = JetstreamConfig(_config)
```

### Comparing `kittycad-0.4.3/kittycad/models/jetstream_api_stats.py` & `kittycad-0.4.4/kittycad/models/jetstream_api_stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-K = TypeVar("K", bound="JetstreamApiStats")
+S = TypeVar("S", bound="JetstreamApiStats")
 
 
 @attr.s(auto_attribs=True)
 class JetstreamApiStats:
     """Jetstream API statistics."""  # noqa: E501
 
     errors: Union[Unset, int] = UNSET
@@ -31,15 +31,15 @@
             field_dict["inflight"] = inflight
         if total is not UNSET:
             field_dict["total"] = total
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
+    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
         d = src_dict.copy()
         errors = d.pop("errors", UNSET)
 
         inflight = d.pop("inflight", UNSET)
 
         total = d.pop("total", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/jetstream_config.py` & `kittycad-0.4.4/kittycad/models/jetstream_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-V = TypeVar("V", bound="JetstreamConfig")
+K = TypeVar("K", bound="JetstreamConfig")
 
 
 @attr.s(auto_attribs=True)
 class JetstreamConfig:
     """Jetstream configuration."""  # noqa: E501
 
     domain: Union[Unset, str] = UNSET
@@ -35,15 +35,15 @@
             field_dict["max_storage"] = max_storage
         if store_dir is not UNSET:
             field_dict["store_dir"] = store_dir
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
+    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
         d = src_dict.copy()
         domain = d.pop("domain", UNSET)
 
         max_memory = d.pop("max_memory", UNSET)
 
         max_storage = d.pop("max_storage", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/jetstream_stats.py` & `kittycad-0.4.4/kittycad/models/jetstream_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.jetstream_api_stats import JetstreamApiStats
 from ..types import UNSET, Unset
 
-R = TypeVar("R", bound="JetstreamStats")
+Q = TypeVar("Q", bound="JetstreamStats")
 
 
 @attr.s(auto_attribs=True)
 class JetstreamStats:
     """Jetstream statistics."""  # noqa: E501
 
     accounts: Union[Unset, int] = UNSET
@@ -49,15 +49,15 @@
             field_dict["reserved_store"] = reserved_store
         if store is not UNSET:
             field_dict["store"] = store
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
+    def from_dict(cls: Type[Q], src_dict: Dict[str, Any]) -> Q:
         d = src_dict.copy()
         accounts = d.pop("accounts", UNSET)
 
         _api = d.pop("api", UNSET)
         api: Union[Unset, JetstreamApiStats]
         if isinstance(_api, Unset):
             api = UNSET
```

### Comparing `kittycad-0.4.3/kittycad/models/leaf_node.py` & `kittycad-0.4.4/kittycad/models/leaf_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-N = TypeVar("N", bound="LeafNode")
+F = TypeVar("F", bound="LeafNode")
 
 
 @attr.s(auto_attribs=True)
 class LeafNode:
     """Leaf node information."""  # noqa: E501
 
     auth_timeout: Union[Unset, int] = UNSET
@@ -35,15 +35,15 @@
             field_dict["port"] = port
         if tls_timeout is not UNSET:
             field_dict["tls_timeout"] = tls_timeout
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
+    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
         d = src_dict.copy()
         auth_timeout = d.pop("auth_timeout", UNSET)
 
         host = d.pop("host", UNSET)
 
         port = d.pop("port", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/line3d.py` & `kittycad-0.4.4/kittycad/models/pong.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,46 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.point3d import Point3d
 from ..types import UNSET, Unset
 
-P = TypeVar("P", bound="Line3d")
+F = TypeVar("F", bound="Pong")
 
 
 @attr.s(auto_attribs=True)
-class Line3d:
-    """Command for adding a line."""  # noqa: E501
+class Pong:
+    """The response from the `/ping` endpoint."""  # noqa: E501
 
-    from_: Union[Unset, Point3d] = UNSET
-    to: Union[Unset, Point3d] = UNSET
+    message: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        if not isinstance(self.from_, Unset):
-            from_ = self.from_
-        if not isinstance(self.to, Unset):
-            to = self.to
+        message = self.message
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if from_ is not UNSET:
-            field_dict["from"] = from_
-        if to is not UNSET:
-            field_dict["to"] = to
+        if message is not UNSET:
+            field_dict["message"] = message
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[P], src_dict: Dict[str, Any]) -> P:
+    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
         d = src_dict.copy()
-        _from_ = d.pop("from", UNSET)
-        from_: Union[Unset, Point3d]
-        if isinstance(_from_, Unset):
-            from_ = UNSET
-        else:
-            from_ = Point3d(_from_)
-
-        _to = d.pop("to", UNSET)
-        to: Union[Unset, Point3d]
-        if isinstance(_to, Unset):
-            to = UNSET
-        else:
-            to = Point3d(_to)
-
-        line3d = cls(
-            from_=from_,
-            to=to,
+        message = d.pop("message", UNSET)
+
+        pong = cls(
+            message=message,
         )
 
-        line3d.additional_properties = d
-        return line3d
+        pong.additional_properties = d
+        return pong
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.3/kittycad/models/mesh.py` & `kittycad-0.4.4/kittycad/models/mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-C = TypeVar("C", bound="Mesh")
+H = TypeVar("H", bound="Mesh")
 
 
 @attr.s(auto_attribs=True)
 class Mesh:
     mesh: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -21,15 +21,15 @@
         field_dict.update({})
         if mesh is not UNSET:
             field_dict["mesh"] = mesh
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[C], src_dict: Dict[str, Any]) -> C:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         mesh = d.pop("mesh", UNSET)
 
         mesh = cls(
             mesh=mesh,
         )
```

### Comparing `kittycad-0.4.3/kittycad/models/meta_cluster_info.py` & `kittycad-0.4.4/kittycad/models/meta_cluster_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-U = TypeVar("U", bound="MetaClusterInfo")
+N = TypeVar("N", bound="MetaClusterInfo")
 
 
 @attr.s(auto_attribs=True)
 class MetaClusterInfo:
     """Jetstream statistics."""  # noqa: E501
 
     cluster_size: Union[Unset, int] = UNSET
@@ -31,15 +31,15 @@
             field_dict["leader"] = leader
         if name is not UNSET:
             field_dict["name"] = name
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[U], src_dict: Dict[str, Any]) -> U:
+    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
         d = src_dict.copy()
         cluster_size = d.pop("cluster_size", UNSET)
 
         leader = d.pop("leader", UNSET)
 
         name = d.pop("name", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/metadata.py` & `kittycad-0.4.4/kittycad/models/metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ..models.engine_metadata import EngineMetadata
 from ..models.environment import Environment
 from ..models.executor_metadata import ExecutorMetadata
 from ..models.file_system_metadata import FileSystemMetadata
 from ..models.point_e_metadata import PointEMetadata
 from ..types import UNSET, Unset
 
-S = TypeVar("S", bound="Metadata")
+H = TypeVar("H", bound="Metadata")
 
 
 @attr.s(auto_attribs=True)
 class Metadata:
     """Metadata about our currently running server.
 
     This is mostly used for internal purposes and debugging."""  # noqa: E501
@@ -67,15 +67,15 @@
             field_dict["point_e"] = point_e
         if pubsub is not UNSET:
             field_dict["pubsub"] = pubsub
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         _cache = d.pop("cache", UNSET)
         cache: Union[Unset, CacheMetadata]
         if isinstance(_cache, Unset):
             cache = UNSET
         else:
             cache = CacheMetadata(_cache)
@@ -88,15 +88,15 @@
             engine = EngineMetadata(_engine)
 
         _environment = d.pop("environment", UNSET)
         environment: Union[Unset, Environment]
         if isinstance(_environment, Unset):
             environment = UNSET
         else:
-            environment = Environment(_environment)
+            environment = _environment  # type: ignore[arg-type]
 
         _executor = d.pop("executor", UNSET)
         executor: Union[Unset, ExecutorMetadata]
         if isinstance(_executor, Unset):
             executor = UNSET
         else:
             executor = ExecutorMetadata(_executor)
```

### Comparing `kittycad-0.4.3/kittycad/models/method.py` & `kittycad-0.4.4/kittycad/models/method.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/modeling_cmd.py` & `kittycad-0.4.4/kittycad/models/point2d.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,53 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.point2d import Point2d
 from ..types import UNSET, Unset
-from .extrude import Extrude
-from .line3d import Line3d
 
-AddLine = Line3d
-
-
-K = TypeVar("K", bound="SelectionClick")
+E = TypeVar("E", bound="Point2d")
 
 
 @attr.s(auto_attribs=True)
-class SelectionClick:
-    at: Union[Unset, Point2d] = UNSET
+class Point2d:
+    """A point in 2D space"""  # noqa: E501
+
+    x: Union[Unset, float] = UNSET
+    y: Union[Unset, float] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        if not isinstance(self.at, Unset):
-            at = self.at
+        x = self.x
+        y = self.y
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if at is not UNSET:
-            field_dict["at"] = at
+        if x is not UNSET:
+            field_dict["x"] = x
+        if y is not UNSET:
+            field_dict["y"] = y
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
+    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
         d = src_dict.copy()
-        _at = d.pop("at", UNSET)
-        at: Union[Unset, Point2d]
-        if isinstance(_at, Unset):
-            at = UNSET
-        else:
-            at = Point2d(_at)
+        x = d.pop("x", UNSET)
 
-        selection_click = cls(
-            at=at,
+        y = d.pop("y", UNSET)
+
+        point2d = cls(
+            x=x,
+            y=y,
         )
 
-        selection_click.additional_properties = d
-        return selection_click
+        point2d.additional_properties = d
+        return point2d
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
@@ -59,10 +56,7 @@
         self.additional_properties[key] = value
 
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
-
-
-ModelingCmd = Union[AddLine, Extrude, SelectionClick]
```

### Comparing `kittycad-0.4.3/kittycad/models/modeling_cmd_req.py` & `kittycad-0.4.4/kittycad/models/modeling_cmd_req.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import attr
 
 from ..models.modeling_cmd import ModelingCmd
 from ..models.modeling_cmd_id import ModelingCmdId
 from ..types import UNSET, Unset
 
-Q = TypeVar("Q", bound="ModelingCmdReq")
+C = TypeVar("C", bound="ModelingCmdReq")
 
 
 @attr.s(auto_attribs=True)
 class ModelingCmdReq:
     """A graphics command submitted to the KittyCAD engine via the Modeling API."""  # noqa: E501
 
     cmd: Union[Unset, ModelingCmd] = UNSET
@@ -35,15 +35,15 @@
             field_dict["cmd_id"] = cmd_id
         if file_id is not UNSET:
             field_dict["file_id"] = file_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Q], src_dict: Dict[str, Any]) -> Q:
+    def from_dict(cls: Type[C], src_dict: Dict[str, Any]) -> C:
         d = src_dict.copy()
         _cmd = d.pop("cmd", UNSET)
         cmd: Union[Unset, ModelingCmd]
         if isinstance(_cmd, Unset):
             cmd = UNSET
         else:
             cmd = _cmd  # type: ignore[arg-type]
```

### Comparing `kittycad-0.4.3/kittycad/models/modeling_cmd_req_batch.py` & `kittycad-0.4.4/kittycad/models/modeling_cmd_req_batch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-F = TypeVar("F", bound="ModelingCmdReqBatch")
+R = TypeVar("R", bound="ModelingCmdReqBatch")
 
 
 @attr.s(auto_attribs=True)
 class ModelingCmdReqBatch:
     """A batch set of graphics commands submitted to the KittyCAD engine via the Modeling API."""  # noqa: E501
 
     cmds: Union[Unset, Any] = UNSET
@@ -27,15 +27,15 @@
             field_dict["cmds"] = cmds
         if file_id is not UNSET:
             field_dict["file_id"] = file_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
+    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
         d = src_dict.copy()
         cmds = d.pop("cmds", UNSET)
         file_id = d.pop("file_id", UNSET)
 
         modeling_cmd_req_batch = cls(
             cmds=cmds,
             file_id=file_id,
```

### Comparing `kittycad-0.4.3/kittycad/models/modeling_error.py` & `kittycad-0.4.4/kittycad/models/modeling_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="ModelingError")
+C = TypeVar("C", bound="ModelingError")
 
 
 @attr.s(auto_attribs=True)
 class ModelingError:
     """Why a command submitted to the Modeling API failed."""  # noqa: E501
 
     error_code: Union[Unset, str] = UNSET
@@ -35,15 +35,15 @@
             field_dict["internal_message"] = internal_message
         if status_code is not UNSET:
             field_dict["status_code"] = status_code
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[C], src_dict: Dict[str, Any]) -> C:
         d = src_dict.copy()
         error_code = d.pop("error_code", UNSET)
 
         external_message = d.pop("external_message", UNSET)
 
         internal_message = d.pop("internal_message", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/modeling_outcome.py` & `kittycad-0.4.4/kittycad/models/modeling_outcome.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Success = Any
 
 
 Error = ModelingError
 
 
-N = TypeVar("N", bound="Cancelled")
+E = TypeVar("E", bound="Cancelled")
 
 
 @attr.s(auto_attribs=True)
 class Cancelled:
     what_failed: Union[Unset, ModelingCmdId] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -30,15 +30,15 @@
         field_dict.update({})
         if what_failed is not UNSET:
             field_dict["what_failed"] = what_failed
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
+    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
         d = src_dict.copy()
         _what_failed = d.pop("what_failed", UNSET)
         what_failed: Union[Unset, ModelingCmdId]
         if isinstance(_what_failed, Unset):
             what_failed = UNSET
         else:
             what_failed = ModelingCmdId(_what_failed)
```

### Comparing `kittycad-0.4.3/kittycad/models/modeling_outcomes.py` & `kittycad-0.4.4/kittycad/models/modeling_outcomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="ModelingOutcomes")
+M = TypeVar("M", bound="ModelingOutcomes")
 
 
 @attr.s(auto_attribs=True)
 class ModelingOutcomes:
     """The result from a batch of modeling commands."""  # noqa: E501
 
     outcomes: Union[Unset, Any] = UNSET
@@ -23,15 +23,15 @@
         field_dict.update({})
         if outcomes is not UNSET:
             field_dict["outcomes"] = outcomes
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[M], src_dict: Dict[str, Any]) -> M:
         d = src_dict.copy()
         outcomes = d.pop("outcomes", UNSET)
 
         modeling_outcomes = cls(
             outcomes=outcomes,
         )
```

### Comparing `kittycad-0.4.3/kittycad/models/new_address.py` & `kittycad-0.4.4/kittycad/models/new_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.country_code import CountryCode
 from ..types import UNSET, Unset
 
-B = TypeVar("B", bound="NewAddress")
+S = TypeVar("S", bound="NewAddress")
 
 
 @attr.s(auto_attribs=True)
 class NewAddress:
     """The struct that is used to create a new record. This is automatically generated and has all the same fields as the main struct only it is missing the `id`."""  # noqa: E501
 
     city: Union[Unset, str] = UNSET
@@ -49,24 +49,24 @@
             field_dict["user_id"] = user_id
         if zip is not UNSET:
             field_dict["zip"] = zip
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
+    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
         d = src_dict.copy()
         city = d.pop("city", UNSET)
 
         _country = d.pop("country", UNSET)
         country: Union[Unset, CountryCode]
         if isinstance(_country, Unset):
             country = UNSET
         else:
-            country = CountryCode(_country)
+            country = _country  # type: ignore[arg-type]
 
         state = d.pop("state", UNSET)
 
         street1 = d.pop("street1", UNSET)
 
         street2 = d.pop("street2", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/o_auth2_client_info.py` & `kittycad-0.4.4/kittycad/models/o_auth2_client_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-B = TypeVar("B", bound="OAuth2ClientInfo")
+L = TypeVar("L", bound="OAuth2ClientInfo")
 
 
 @attr.s(auto_attribs=True)
 class OAuth2ClientInfo:
     """Information about an OAuth 2.0 client."""  # noqa: E501
 
     csrf_token: Union[Unset, str] = UNSET
@@ -31,15 +31,15 @@
             field_dict["pkce_code_verifier"] = pkce_code_verifier
         if url is not UNSET:
             field_dict["url"] = url
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
+    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
         d = src_dict.copy()
         csrf_token = d.pop("csrf_token", UNSET)
 
         pkce_code_verifier = d.pop("pkce_code_verifier", UNSET)
 
         url = d.pop("url", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/onboarding.py` & `kittycad-0.4.4/kittycad/models/onboarding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-P = TypeVar("P", bound="Onboarding")
+T = TypeVar("T", bound="Onboarding")
 
 
 @attr.s(auto_attribs=True)
 class Onboarding:
     """Onboarding details"""  # noqa: E501
 
     first_call_from__their_machine_date: Union[Unset, str] = UNSET
@@ -33,15 +33,15 @@
             field_dict["first_litterbox_execute_date"] = first_litterbox_execute_date
         if first_token_date is not UNSET:
             field_dict["first_token_date"] = first_token_date
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[P], src_dict: Dict[str, Any]) -> P:
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         first_call_from__their_machine_date = d.pop(
             "first_call_from_their_machine_date", UNSET
         )
 
         first_litterbox_execute_date = d.pop("first_litterbox_execute_date", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/output_file.py` & `kittycad-0.4.4/kittycad/models/output_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-J = TypeVar("J", bound="OutputFile")
+E = TypeVar("E", bound="OutputFile")
 
 
 @attr.s(auto_attribs=True)
 class OutputFile:
     """Output file contents."""  # noqa: E501
 
     contents: Union[Unset, str] = UNSET
@@ -27,15 +27,15 @@
             field_dict["contents"] = contents
         if name is not UNSET:
             field_dict["name"] = name
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
+    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
         d = src_dict.copy()
         contents = d.pop("contents", UNSET)
 
         name = d.pop("name", UNSET)
 
         output_file = cls(
             contents=contents,
```

### Comparing `kittycad-0.4.3/kittycad/models/payment_intent.py` & `kittycad-0.4.4/kittycad/models/payment_intent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="PaymentIntent")
+L = TypeVar("L", bound="PaymentIntent")
 
 
 @attr.s(auto_attribs=True)
 class PaymentIntent:
     """A payment intent response."""  # noqa: E501
 
     client_secret: Union[Unset, str] = UNSET
@@ -23,15 +23,15 @@
         field_dict.update({})
         if client_secret is not UNSET:
             field_dict["client_secret"] = client_secret
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
         d = src_dict.copy()
         client_secret = d.pop("client_secret", UNSET)
 
         payment_intent = cls(
             client_secret=client_secret,
         )
```

### Comparing `kittycad-0.4.3/kittycad/models/payment_method.py` & `kittycad-0.4.4/kittycad/models/payment_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dateutil.parser import isoparse
 
 from ..models.billing_info import BillingInfo
 from ..models.card_details import CardDetails
 from ..models.payment_method_type import PaymentMethodType
 from ..types import UNSET, Unset
 
-V = TypeVar("V", bound="PaymentMethod")
+N = TypeVar("N", bound="PaymentMethod")
 
 
 @attr.s(auto_attribs=True)
 class PaymentMethod:
     """A payment method."""  # noqa: E501
 
     billing_info: Union[Unset, BillingInfo] = UNSET
@@ -53,15 +53,15 @@
             field_dict["metadata"] = metadata
         if type is not UNSET:
             field_dict["type"] = type
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
+    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
         d = src_dict.copy()
         _billing_info = d.pop("billing_info", UNSET)
         billing_info: Union[Unset, BillingInfo]
         if isinstance(_billing_info, Unset):
             billing_info = UNSET
         else:
             billing_info = BillingInfo(_billing_info)
@@ -84,15 +84,15 @@
 
         metadata = d.pop("metadata", UNSET)
         _type = d.pop("type", UNSET)
         type: Union[Unset, PaymentMethodType]
         if isinstance(_type, Unset):
             type = UNSET
         else:
-            type = PaymentMethodType(_type)
+            type = _type  # type: ignore[arg-type]
 
         payment_method = cls(
             billing_info=billing_info,
             card=card,
             created_at=created_at,
             id=id,
             metadata=metadata,
```

### Comparing `kittycad-0.4.3/kittycad/models/payment_method_card_checks.py` & `kittycad-0.4.4/kittycad/models/payment_method_card_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-C = TypeVar("C", bound="PaymentMethodCardChecks")
+N = TypeVar("N", bound="PaymentMethodCardChecks")
 
 
 @attr.s(auto_attribs=True)
 class PaymentMethodCardChecks:
     """Card checks."""  # noqa: E501
 
     address_line1_check: Union[Unset, str] = UNSET
@@ -31,15 +31,15 @@
             field_dict["address_postal_code_check"] = address_postal_code_check
         if cvc_check is not UNSET:
             field_dict["cvc_check"] = cvc_check
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[C], src_dict: Dict[str, Any]) -> C:
+    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
         d = src_dict.copy()
         address_line1_check = d.pop("address_line1_check", UNSET)
 
         address_postal_code_check = d.pop("address_postal_code_check", UNSET)
 
         cvc_check = d.pop("cvc_check", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/physics_constant.py` & `kittycad-0.4.4/kittycad/models/unit_pressure_conversion.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,103 +1,105 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.physics_constant_name import PhysicsConstantName
+from ..models.unit_pressure import UnitPressure
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-R = TypeVar("R", bound="PhysicsConstant")
+A = TypeVar("A", bound="UnitPressureConversion")
 
 
 @attr.s(auto_attribs=True)
-class PhysicsConstant:
-    """A physics constant."""  # noqa: E501
+class UnitPressureConversion:
+    """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
-    constant: Union[Unset, PhysicsConstantName] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
+    input: Union[Unset, float] = UNSET
+    input_unit: Union[Unset, UnitPressure] = UNSET
+    output: Union[Unset, float] = UNSET
+    output_unit: Union[Unset, UnitPressure] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
-    value: Union[Unset, float] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         completed_at: Union[Unset, str] = UNSET
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
-        if not isinstance(self.constant, Unset):
-            constant = self.constant
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
+        input = self.input
+        if not isinstance(self.input_unit, Unset):
+            input_unit = self.input_unit
+        output = self.output
+        if not isinstance(self.output_unit, Unset):
+            output_unit = self.output_unit
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
         user_id = self.user_id
-        value = self.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if completed_at is not UNSET:
             field_dict["completed_at"] = completed_at
-        if constant is not UNSET:
-            field_dict["constant"] = constant
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
+        if input is not UNSET:
+            field_dict["input"] = input
+        if input_unit is not UNSET:
+            field_dict["input_unit"] = input_unit
+        if output is not UNSET:
+            field_dict["output"] = output
+        if output_unit is not UNSET:
+            field_dict["output_unit"] = output_unit
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
-        if value is not UNSET:
-            field_dict["value"] = value
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
+    def from_dict(cls: Type[A], src_dict: Dict[str, Any]) -> A:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
 
-        _constant = d.pop("constant", UNSET)
-        constant: Union[Unset, PhysicsConstantName]
-        if isinstance(_constant, Unset):
-            constant = UNSET
-        else:
-            constant = PhysicsConstantName(_constant)
-
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
@@ -106,54 +108,72 @@
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
             id = Uuid(_id)
 
+        input = d.pop("input", UNSET)
+
+        _input_unit = d.pop("input_unit", UNSET)
+        input_unit: Union[Unset, UnitPressure]
+        if isinstance(_input_unit, Unset):
+            input_unit = UNSET
+        else:
+            input_unit = _input_unit  # type: ignore[arg-type]
+
+        output = d.pop("output", UNSET)
+
+        _output_unit = d.pop("output_unit", UNSET)
+        output_unit: Union[Unset, UnitPressure]
+        if isinstance(_output_unit, Unset):
+            output_unit = UNSET
+        else:
+            output_unit = _output_unit  # type: ignore[arg-type]
+
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        value = d.pop("value", UNSET)
-
-        physics_constant = cls(
+        unit_pressure_conversion = cls(
             completed_at=completed_at,
-            constant=constant,
             created_at=created_at,
             error=error,
             id=id,
+            input=input,
+            input_unit=input_unit,
+            output=output,
+            output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
-            value=value,
         )
 
-        physics_constant.additional_properties = d
-        return physics_constant
+        unit_pressure_conversion.additional_properties = d
+        return unit_pressure_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.3/kittycad/models/physics_constant_name.py` & `kittycad-0.4.4/kittycad/models/physics_constant_name.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/plugins_info.py` & `kittycad-0.4.4/kittycad/models/plugins_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-C = TypeVar("C", bound="PluginsInfo")
+V = TypeVar("V", bound="PluginsInfo")
 
 
 @attr.s(auto_attribs=True)
 class PluginsInfo:
     """Available plugins per type.
 
     **Note**: Only unmanaged (V1) plugins are included in this list. V1 plugins are \"lazily\" loaded, and are not returned in this list if there is no resource using the plugin."""  # noqa: E501
@@ -45,15 +45,15 @@
             field_dict["network"] = network
         if volume is not UNSET:
             field_dict["volume"] = volume
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[C], src_dict: Dict[str, Any]) -> C:
+    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
         d = src_dict.copy()
         authorization = cast(List[str], d.pop("authorization", UNSET))
 
         log = cast(List[str], d.pop("log", UNSET))
 
         network = cast(List[str], d.pop("network", UNSET))
```

### Comparing `kittycad-0.4.3/kittycad/models/point2d.py` & `kittycad-0.4.4/kittycad/models/point3d.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,60 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-E = TypeVar("E", bound="Point2d")
+T = TypeVar("T", bound="Point3d")
 
 
 @attr.s(auto_attribs=True)
-class Point2d:
-    """A point in 2D space"""  # noqa: E501
+class Point3d:
+    """A point in 3D space"""  # noqa: E501
 
     x: Union[Unset, float] = UNSET
     y: Union[Unset, float] = UNSET
+    z: Union[Unset, float] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         x = self.x
         y = self.y
+        z = self.z
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if x is not UNSET:
             field_dict["x"] = x
         if y is not UNSET:
             field_dict["y"] = y
+        if z is not UNSET:
+            field_dict["z"] = z
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         x = d.pop("x", UNSET)
 
         y = d.pop("y", UNSET)
 
-        point2d = cls(
+        z = d.pop("z", UNSET)
+
+        point3d = cls(
             x=x,
             y=y,
+            z=z,
         )
 
-        point2d.additional_properties = d
-        return point2d
+        point3d.additional_properties = d
+        return point3d
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.3/kittycad/models/point3d.py` & `kittycad-0.4.4/kittycad/models/system_info_default_address_pools.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,51 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-M = TypeVar("M", bound="Point3d")
+U = TypeVar("U", bound="SystemInfoDefaultAddressPools")
 
 
 @attr.s(auto_attribs=True)
-class Point3d:
-    """A point in 3D space"""  # noqa: E501
-
-    x: Union[Unset, float] = UNSET
-    y: Union[Unset, float] = UNSET
-    z: Union[Unset, float] = UNSET
+class SystemInfoDefaultAddressPools:
+    base: Union[Unset, str] = UNSET
+    size: Union[Unset, int] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        x = self.x
-        y = self.y
-        z = self.z
+        base = self.base
+        size = self.size
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if x is not UNSET:
-            field_dict["x"] = x
-        if y is not UNSET:
-            field_dict["y"] = y
-        if z is not UNSET:
-            field_dict["z"] = z
+        if base is not UNSET:
+            field_dict["base"] = base
+        if size is not UNSET:
+            field_dict["size"] = size
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[M], src_dict: Dict[str, Any]) -> M:
+    def from_dict(cls: Type[U], src_dict: Dict[str, Any]) -> U:
         d = src_dict.copy()
-        x = d.pop("x", UNSET)
-
-        y = d.pop("y", UNSET)
+        base = d.pop("base", UNSET)
 
-        z = d.pop("z", UNSET)
+        size = d.pop("size", UNSET)
 
-        point3d = cls(
-            x=x,
-            y=y,
-            z=z,
+        system_info_default_address_pools = cls(
+            base=base,
+            size=size,
         )
 
-        point3d.additional_properties = d
-        return point3d
+        system_info_default_address_pools.additional_properties = d
+        return system_info_default_address_pools
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.3/kittycad/models/point_e_metadata.py` & `kittycad-0.4.4/kittycad/models/point_e_metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-S = TypeVar("S", bound="PointEMetadata")
+Q = TypeVar("Q", bound="PointEMetadata")
 
 
 @attr.s(auto_attribs=True)
 class PointEMetadata:
     """Metadata about our point-e instance.
 
     This is mostly used for internal purposes and debugging."""  # noqa: E501
@@ -25,15 +25,15 @@
         field_dict.update({})
         if ok is not UNSET:
             field_dict["ok"] = ok
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
+    def from_dict(cls: Type[Q], src_dict: Dict[str, Any]) -> Q:
         d = src_dict.copy()
         ok = d.pop("ok", UNSET)
 
         point_e_metadata = cls(
             ok=ok,
         )
```

### Comparing `kittycad-0.4.3/kittycad/models/pong.py` & `kittycad-0.4.4/kittycad/models/discount.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.coupon import Coupon
 from ..types import UNSET, Unset
 
-L = TypeVar("L", bound="Pong")
+V = TypeVar("V", bound="Discount")
 
 
 @attr.s(auto_attribs=True)
-class Pong:
-    """The response from the `/ping` endpoint."""  # noqa: E501
+class Discount:
+    """The resource representing a Discount."""  # noqa: E501
 
-    message: Union[Unset, str] = UNSET
+    coupon: Union[Unset, Coupon] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        message = self.message
+        if not isinstance(self.coupon, Unset):
+            coupon = self.coupon
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if message is not UNSET:
-            field_dict["message"] = message
+        if coupon is not UNSET:
+            field_dict["coupon"] = coupon
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
+    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
         d = src_dict.copy()
-        message = d.pop("message", UNSET)
+        _coupon = d.pop("coupon", UNSET)
+        coupon: Union[Unset, Coupon]
+        if isinstance(_coupon, Unset):
+            coupon = UNSET
+        else:
+            coupon = Coupon(_coupon)
 
-        pong = cls(
-            message=message,
+        discount = cls(
+            coupon=coupon,
         )
 
-        pong.additional_properties = d
-        return pong
+        discount.additional_properties = d
+        return discount
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.3/kittycad/models/registry_service_config.py` & `kittycad-0.4.4/kittycad/models/registry_service_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RegistryServiceConfig")
+D = TypeVar("D", bound="RegistryServiceConfig")
 
 
 @attr.s(auto_attribs=True)
 class RegistryServiceConfig:
     """RegistryServiceConfig stores daemon registry services configuration."""  # noqa: E501
 
     allow_nondistributable_artifacts_cid_rs: Union[Unset, List[str]] = UNSET
@@ -55,15 +55,15 @@
             field_dict["insecure_registry_cid_rs"] = insecure_registry_cid_rs
         if mirrors is not UNSET:
             field_dict["mirrors"] = mirrors
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[D], src_dict: Dict[str, Any]) -> D:
         d = src_dict.copy()
         allow_nondistributable_artifacts_cid_rs = cast(
             List[str], d.pop("allow_nondistributable_artifacts_cid_rs", UNSET)
         )
 
         allow_nondistributable_artifacts_hostnames = cast(
             List[str], d.pop("allow_nondistributable_artifacts_hostnames", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/runtime.py` & `kittycad-0.4.4/kittycad/models/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-E = TypeVar("E", bound="Runtime")
+J = TypeVar("J", bound="Runtime")
 
 
 @attr.s(auto_attribs=True)
 class Runtime:
     """Runtime describes an [OCI compliant](https://github.com/opencontainers/runtime-spec) runtime.  The runtime is invoked by the daemon via the `containerd` daemon. OCI runtimes act as an interface to the Linux kernel namespaces, cgroups, and SELinux."""  # noqa: E501
 
     path: Union[Unset, str] = UNSET
@@ -29,15 +29,15 @@
             field_dict["path"] = path
         if runtime_args is not UNSET:
             field_dict["runtime_args"] = runtime_args
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
+    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
         d = src_dict.copy()
         path = d.pop("path", UNSET)
 
         runtime_args = cast(List[str], d.pop("runtime_args", UNSET))
 
         runtime = cls(
             path=path,
```

### Comparing `kittycad-0.4.3/kittycad/models/session.py` & `kittycad-0.4.4/kittycad/models/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-D = TypeVar("D", bound="Session")
+F = TypeVar("F", bound="Session")
 
 
 @attr.s(auto_attribs=True)
 class Session:
     """An authentication session.
 
     For our UIs, these are automatically created by Next.js."""  # noqa: E501
@@ -54,15 +54,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[D], src_dict: Dict[str, Any]) -> D:
+    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
         d = src_dict.copy()
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
```

### Comparing `kittycad-0.4.3/kittycad/models/system_info_default_address_pools.py` & `kittycad-0.4.4/kittycad/models/system.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,72 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.axis_direction_pair import AxisDirectionPair
 from ..types import UNSET, Unset
 
-Y = TypeVar("Y", bound="SystemInfoDefaultAddressPools")
+V = TypeVar("V", bound="System")
 
 
 @attr.s(auto_attribs=True)
-class SystemInfoDefaultAddressPools:
-    base: Union[Unset, str] = UNSET
-    size: Union[Unset, int] = UNSET
+class System:
+    """Co-ordinate system definition.
+
+    The `up` axis must be orthogonal to the `forward` axis.
+
+    See [cglearn.eu] for background reading.
+
+    [cglearn.eu](https://cglearn.eu/pub/computer-graphics/introduction-to-geometry#material-coordinate-systems-1)"""  # noqa: E501
+
+    forward: Union[Unset, AxisDirectionPair] = UNSET
+    up: Union[Unset, AxisDirectionPair] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        base = self.base
-        size = self.size
+        if not isinstance(self.forward, Unset):
+            forward = self.forward
+        if not isinstance(self.up, Unset):
+            up = self.up
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if base is not UNSET:
-            field_dict["base"] = base
-        if size is not UNSET:
-            field_dict["size"] = size
+        if forward is not UNSET:
+            field_dict["forward"] = forward
+        if up is not UNSET:
+            field_dict["up"] = up
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
+    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
         d = src_dict.copy()
-        base = d.pop("base", UNSET)
-
-        size = d.pop("size", UNSET)
-
-        system_info_default_address_pools = cls(
-            base=base,
-            size=size,
+        _forward = d.pop("forward", UNSET)
+        forward: Union[Unset, AxisDirectionPair]
+        if isinstance(_forward, Unset):
+            forward = UNSET
+        else:
+            forward = AxisDirectionPair(_forward)
+
+        _up = d.pop("up", UNSET)
+        up: Union[Unset, AxisDirectionPair]
+        if isinstance(_up, Unset):
+            up = UNSET
+        else:
+            up = AxisDirectionPair(_up)
+
+        system = cls(
+            forward=forward,
+            up=up,
         )
 
-        system_info_default_address_pools.additional_properties = d
-        return system_info_default_address_pools
+        system.additional_properties = d
+        return system
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.3/kittycad/models/unit_angle_conversion.py` & `kittycad-0.4.4/kittycad/models/unit_angle_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_angle import UnitAngle
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-Y = TypeVar("Y", bound="UnitAngleConversion")
+F = TypeVar("F", bound="UnitAngleConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitAngleConversion:
     """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -83,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
+    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -115,38 +115,38 @@
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
         input_unit: Union[Unset, UnitAngle]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
         else:
-            input_unit = UnitAngle(_input_unit)
+            input_unit = _input_unit  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_unit = d.pop("output_unit", UNSET)
         output_unit: Union[Unset, UnitAngle]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
-            output_unit = UnitAngle(_output_unit)
+            output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
```

### Comparing `kittycad-0.4.3/kittycad/models/unit_area.py` & `kittycad-0.4.4/kittycad/models/unit_area.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/unit_area_conversion.py` & `kittycad-0.4.4/kittycad/models/unit_area_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_area import UnitArea
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-D = TypeVar("D", bound="UnitAreaConversion")
+Y = TypeVar("Y", bound="UnitAreaConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitAreaConversion:
     """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -83,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[D], src_dict: Dict[str, Any]) -> D:
+    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -115,38 +115,38 @@
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
         input_unit: Union[Unset, UnitArea]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
         else:
-            input_unit = UnitArea(_input_unit)
+            input_unit = _input_unit  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_unit = d.pop("output_unit", UNSET)
         output_unit: Union[Unset, UnitArea]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
-            output_unit = UnitArea(_output_unit)
+            output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
```

### Comparing `kittycad-0.4.3/kittycad/models/unit_current.py` & `kittycad-0.4.4/kittycad/models/unit_current.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/unit_current_conversion.py` & `kittycad-0.4.4/kittycad/models/unit_current_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,38 +115,38 @@
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
         input_unit: Union[Unset, UnitCurrent]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
         else:
-            input_unit = UnitCurrent(_input_unit)
+            input_unit = _input_unit  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_unit = d.pop("output_unit", UNSET)
         output_unit: Union[Unset, UnitCurrent]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
-            output_unit = UnitCurrent(_output_unit)
+            output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
```

### Comparing `kittycad-0.4.3/kittycad/models/unit_energy.py` & `kittycad-0.4.4/kittycad/models/unit_energy.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/unit_energy_conversion.py` & `kittycad-0.4.4/kittycad/models/unit_energy_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_energy import UnitEnergy
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-Z = TypeVar("Z", bound="UnitEnergyConversion")
+P = TypeVar("P", bound="UnitEnergyConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitEnergyConversion:
     """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -83,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Z], src_dict: Dict[str, Any]) -> Z:
+    def from_dict(cls: Type[P], src_dict: Dict[str, Any]) -> P:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -115,38 +115,38 @@
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
         input_unit: Union[Unset, UnitEnergy]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
         else:
-            input_unit = UnitEnergy(_input_unit)
+            input_unit = _input_unit  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_unit = d.pop("output_unit", UNSET)
         output_unit: Union[Unset, UnitEnergy]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
-            output_unit = UnitEnergy(_output_unit)
+            output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
```

### Comparing `kittycad-0.4.3/kittycad/models/unit_force.py` & `kittycad-0.4.4/kittycad/models/unit_force.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/unit_force_conversion.py` & `kittycad-0.4.4/kittycad/models/unit_force_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_force import UnitForce
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-G = TypeVar("G", bound="UnitForceConversion")
+Y = TypeVar("Y", bound="UnitForceConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitForceConversion:
     """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -83,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[G], src_dict: Dict[str, Any]) -> G:
+    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -115,38 +115,38 @@
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
         input_unit: Union[Unset, UnitForce]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
         else:
-            input_unit = UnitForce(_input_unit)
+            input_unit = _input_unit  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_unit = d.pop("output_unit", UNSET)
         output_unit: Union[Unset, UnitForce]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
-            output_unit = UnitForce(_output_unit)
+            output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
```

### Comparing `kittycad-0.4.3/kittycad/models/unit_frequency.py` & `kittycad-0.4.4/kittycad/models/unit_frequency.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/unit_frequency_conversion.py` & `kittycad-0.4.4/kittycad/models/unit_frequency_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,38 +115,38 @@
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
         input_unit: Union[Unset, UnitFrequency]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
         else:
-            input_unit = UnitFrequency(_input_unit)
+            input_unit = _input_unit  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_unit = d.pop("output_unit", UNSET)
         output_unit: Union[Unset, UnitFrequency]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
-            output_unit = UnitFrequency(_output_unit)
+            output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
```

### Comparing `kittycad-0.4.3/kittycad/models/unit_length.py` & `kittycad-0.4.4/kittycad/models/unit_length.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/unit_length_conversion.py` & `kittycad-0.4.4/kittycad/models/unit_length_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_length import UnitLength
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-N = TypeVar("N", bound="UnitLengthConversion")
+K = TypeVar("K", bound="UnitLengthConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitLengthConversion:
     """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -83,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
+    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -115,38 +115,38 @@
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
         input_unit: Union[Unset, UnitLength]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
         else:
-            input_unit = UnitLength(_input_unit)
+            input_unit = _input_unit  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_unit = d.pop("output_unit", UNSET)
         output_unit: Union[Unset, UnitLength]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
-            output_unit = UnitLength(_output_unit)
+            output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
```

### Comparing `kittycad-0.4.3/kittycad/models/unit_mass.py` & `kittycad-0.4.4/kittycad/models/unit_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/unit_mass_conversion.py` & `kittycad-0.4.4/kittycad/models/unit_volume_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_mass import UnitMass
+from ..models.unit_volume import UnitVolume
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-N = TypeVar("N", bound="UnitMassConversion")
+B = TypeVar("B", bound="UnitVolumeConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitMassConversion:
+class UnitVolumeConversion:
     """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
-    input_unit: Union[Unset, UnitMass] = UNSET
+    input_unit: Union[Unset, UnitVolume] = UNSET
     output: Union[Unset, float] = UNSET
-    output_unit: Union[Unset, UnitMass] = UNSET
+    output_unit: Union[Unset, UnitVolume] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -83,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
+    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -111,69 +111,69 @@
             id = UNSET
         else:
             id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
-        input_unit: Union[Unset, UnitMass]
+        input_unit: Union[Unset, UnitVolume]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
         else:
-            input_unit = UnitMass(_input_unit)
+            input_unit = _input_unit  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_unit = d.pop("output_unit", UNSET)
-        output_unit: Union[Unset, UnitMass]
+        output_unit: Union[Unset, UnitVolume]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
-            output_unit = UnitMass(_output_unit)
+            output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_mass_conversion = cls(
+        unit_volume_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             input_unit=input_unit,
             output=output,
             output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_mass_conversion.additional_properties = d
-        return unit_mass_conversion
+        unit_volume_conversion.additional_properties = d
+        return unit_volume_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.3/kittycad/models/unit_power.py` & `kittycad-0.4.4/kittycad/models/unit_power.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/unit_power_conversion.py` & `kittycad-0.4.4/kittycad/models/unit_torque_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_power import UnitPower
+from ..models.unit_torque import UnitTorque
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="UnitPowerConversion")
+W = TypeVar("W", bound="UnitTorqueConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitPowerConversion:
+class UnitTorqueConversion:
     """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
-    input_unit: Union[Unset, UnitPower] = UNSET
+    input_unit: Union[Unset, UnitTorque] = UNSET
     output: Union[Unset, float] = UNSET
-    output_unit: Union[Unset, UnitPower] = UNSET
+    output_unit: Union[Unset, UnitTorque] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -83,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[W], src_dict: Dict[str, Any]) -> W:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -111,69 +111,69 @@
             id = UNSET
         else:
             id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
-        input_unit: Union[Unset, UnitPower]
+        input_unit: Union[Unset, UnitTorque]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
         else:
-            input_unit = UnitPower(_input_unit)
+            input_unit = _input_unit  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_unit = d.pop("output_unit", UNSET)
-        output_unit: Union[Unset, UnitPower]
+        output_unit: Union[Unset, UnitTorque]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
-            output_unit = UnitPower(_output_unit)
+            output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_power_conversion = cls(
+        unit_torque_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             input_unit=input_unit,
             output=output,
             output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_power_conversion.additional_properties = d
-        return unit_power_conversion
+        unit_torque_conversion.additional_properties = d
+        return unit_torque_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.3/kittycad/models/unit_pressure.py` & `kittycad-0.4.4/kittycad/models/unit_pressure.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/unit_pressure_conversion.py` & `kittycad-0.4.4/kittycad/models/unit_temperature_conversion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_pressure import UnitPressure
+from ..models.unit_temperature import UnitTemperature
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-V = TypeVar("V", bound="UnitPressureConversion")
+R = TypeVar("R", bound="UnitTemperatureConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitPressureConversion:
+class UnitTemperatureConversion:
     """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
-    input_unit: Union[Unset, UnitPressure] = UNSET
+    input_unit: Union[Unset, UnitTemperature] = UNSET
     output: Union[Unset, float] = UNSET
-    output_unit: Union[Unset, UnitPressure] = UNSET
+    output_unit: Union[Unset, UnitTemperature] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -83,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
+    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -111,69 +111,69 @@
             id = UNSET
         else:
             id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
-        input_unit: Union[Unset, UnitPressure]
+        input_unit: Union[Unset, UnitTemperature]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
         else:
-            input_unit = UnitPressure(_input_unit)
+            input_unit = _input_unit  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_unit = d.pop("output_unit", UNSET)
-        output_unit: Union[Unset, UnitPressure]
+        output_unit: Union[Unset, UnitTemperature]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
-            output_unit = UnitPressure(_output_unit)
+            output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_pressure_conversion = cls(
+        unit_temperature_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             input_unit=input_unit,
             output=output,
             output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_pressure_conversion.additional_properties = d
-        return unit_pressure_conversion
+        unit_temperature_conversion.additional_properties = d
+        return unit_temperature_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.3/kittycad/models/unit_temperature.py` & `kittycad-0.4.4/kittycad/models/unit_temperature.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/unit_temperature_conversion.py` & `kittycad-0.4.4/kittycad/models/unit_power_conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_temperature import UnitTemperature
+from ..models.unit_power import UnitPower
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-E = TypeVar("E", bound="UnitTemperatureConversion")
+H = TypeVar("H", bound="UnitPowerConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitTemperatureConversion:
+class UnitPowerConversion:
     """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
-    input_unit: Union[Unset, UnitTemperature] = UNSET
+    input_unit: Union[Unset, UnitPower] = UNSET
     output: Union[Unset, float] = UNSET
-    output_unit: Union[Unset, UnitTemperature] = UNSET
+    output_unit: Union[Unset, UnitPower] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -83,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -111,69 +111,69 @@
             id = UNSET
         else:
             id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
-        input_unit: Union[Unset, UnitTemperature]
+        input_unit: Union[Unset, UnitPower]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
         else:
-            input_unit = UnitTemperature(_input_unit)
+            input_unit = _input_unit  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_unit = d.pop("output_unit", UNSET)
-        output_unit: Union[Unset, UnitTemperature]
+        output_unit: Union[Unset, UnitPower]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
-            output_unit = UnitTemperature(_output_unit)
+            output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_temperature_conversion = cls(
+        unit_power_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             input_unit=input_unit,
             output=output,
             output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_temperature_conversion.additional_properties = d
-        return unit_temperature_conversion
+        unit_power_conversion.additional_properties = d
+        return unit_power_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.3/kittycad/models/unit_torque_conversion.py` & `kittycad-0.4.4/kittycad/models/unit_mass_conversion.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_torque import UnitTorque
+from ..models.unit_mass import UnitMass
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitTorqueConversion")
+N = TypeVar("N", bound="UnitMassConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitTorqueConversion:
+class UnitMassConversion:
     """Result of converting between units."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
-    input_unit: Union[Unset, UnitTorque] = UNSET
+    input_unit: Union[Unset, UnitMass] = UNSET
     output: Union[Unset, float] = UNSET
-    output_unit: Union[Unset, UnitTorque] = UNSET
+    output_unit: Union[Unset, UnitMass] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -83,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -111,69 +111,69 @@
             id = UNSET
         else:
             id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         _input_unit = d.pop("input_unit", UNSET)
-        input_unit: Union[Unset, UnitTorque]
+        input_unit: Union[Unset, UnitMass]
         if isinstance(_input_unit, Unset):
             input_unit = UNSET
         else:
-            input_unit = UnitTorque(_input_unit)
+            input_unit = _input_unit  # type: ignore[arg-type]
 
         output = d.pop("output", UNSET)
 
         _output_unit = d.pop("output_unit", UNSET)
-        output_unit: Union[Unset, UnitTorque]
+        output_unit: Union[Unset, UnitMass]
         if isinstance(_output_unit, Unset):
             output_unit = UNSET
         else:
-            output_unit = UnitTorque(_output_unit)
+            output_unit = _output_unit  # type: ignore[arg-type]
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_torque_conversion = cls(
+        unit_mass_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             input_unit=input_unit,
             output=output,
             output_unit=output_unit,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_torque_conversion.additional_properties = d
-        return unit_torque_conversion
+        unit_mass_conversion.additional_properties = d
+        return unit_mass_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.3/kittycad/models/unit_volume.py` & `kittycad-0.4.4/kittycad/models/unit_volume.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/kittycad/models/unit_volume_conversion.py` & `kittycad-0.4.4/kittycad/models/file_conversion.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_volume import UnitVolume
+from ..models.file_export_format import FileExportFormat
+from ..models.file_import_format import FileImportFormat
+from ..models.input_format import InputFormat
+from ..models.output_format import OutputFormat
 from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-Q = TypeVar("Q", bound="UnitVolumeConversion")
+H = TypeVar("H", bound="FileConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitVolumeConversion:
-    """Result of converting between units."""  # noqa: E501
+class FileConversion:
+    """A file conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
-    input: Union[Unset, float] = UNSET
-    input_unit: Union[Unset, UnitVolume] = UNSET
-    output: Union[Unset, float] = UNSET
-    output_unit: Union[Unset, UnitVolume] = UNSET
+    output: Union[Unset, str] = UNSET
+    output_format: Union[Unset, FileExportFormat] = UNSET
+    output_format_options: Union[Unset, OutputFormat] = UNSET
+    outputs: Union[Unset, Any] = UNSET
+    src_format: Union[Unset, FileImportFormat] = UNSET
+    src_format_options: Union[Unset, InputFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -36,20 +41,24 @@
         if not isinstance(self.completed_at, Unset):
             completed_at = self.completed_at.isoformat()
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
         error = self.error
         id = self.id
-        input = self.input
-        if not isinstance(self.input_unit, Unset):
-            input_unit = self.input_unit
         output = self.output
-        if not isinstance(self.output_unit, Unset):
-            output_unit = self.output_unit
+        if not isinstance(self.output_format, Unset):
+            output_format = self.output_format
+        if not isinstance(self.output_format_options, Unset):
+            output_format_options = self.output_format_options
+        outputs = self.outputs
+        if not isinstance(self.src_format, Unset):
+            src_format = self.src_format
+        if not isinstance(self.src_format_options, Unset):
+            src_format_options = self.src_format_options
         started_at: Union[Unset, str] = UNSET
         if not isinstance(self.started_at, Unset):
             started_at = self.started_at.isoformat()
         if not isinstance(self.status, Unset):
             status = self.status
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
@@ -63,35 +72,39 @@
             field_dict["completed_at"] = completed_at
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
         if error is not UNSET:
             field_dict["error"] = error
         if id is not UNSET:
             field_dict["id"] = id
-        if input is not UNSET:
-            field_dict["input"] = input
-        if input_unit is not UNSET:
-            field_dict["input_unit"] = input_unit
         if output is not UNSET:
             field_dict["output"] = output
-        if output_unit is not UNSET:
-            field_dict["output_unit"] = output_unit
+        if output_format is not UNSET:
+            field_dict["output_format"] = output_format
+        if output_format_options is not UNSET:
+            field_dict["output_format_options"] = output_format_options
+        if outputs is not UNSET:
+            field_dict["outputs"] = outputs
+        if src_format is not UNSET:
+            field_dict["src_format"] = src_format
+        if src_format_options is not UNSET:
+            field_dict["src_format_options"] = src_format_options
         if started_at is not UNSET:
             field_dict["started_at"] = started_at
         if status is not UNSET:
             field_dict["status"] = status
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Q], src_dict: Dict[str, Any]) -> Q:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -108,72 +121,87 @@
         _id = d.pop("id", UNSET)
         id: Union[Unset, Uuid]
         if isinstance(_id, Unset):
             id = UNSET
         else:
             id = Uuid(_id)
 
-        input = d.pop("input", UNSET)
-
-        _input_unit = d.pop("input_unit", UNSET)
-        input_unit: Union[Unset, UnitVolume]
-        if isinstance(_input_unit, Unset):
-            input_unit = UNSET
-        else:
-            input_unit = UnitVolume(_input_unit)
-
         output = d.pop("output", UNSET)
 
-        _output_unit = d.pop("output_unit", UNSET)
-        output_unit: Union[Unset, UnitVolume]
-        if isinstance(_output_unit, Unset):
-            output_unit = UNSET
+        _output_format = d.pop("output_format", UNSET)
+        output_format: Union[Unset, FileExportFormat]
+        if isinstance(_output_format, Unset):
+            output_format = UNSET
+        else:
+            output_format = _output_format  # type: ignore[arg-type]
+
+        _output_format_options = d.pop("output_format_options", UNSET)
+        output_format_options: Union[Unset, OutputFormat]
+        if isinstance(_output_format_options, Unset):
+            output_format_options = UNSET
+        else:
+            output_format_options = OutputFormat(_output_format_options)
+
+        outputs = d.pop("outputs", UNSET)
+        _src_format = d.pop("src_format", UNSET)
+        src_format: Union[Unset, FileImportFormat]
+        if isinstance(_src_format, Unset):
+            src_format = UNSET
+        else:
+            src_format = _src_format  # type: ignore[arg-type]
+
+        _src_format_options = d.pop("src_format_options", UNSET)
+        src_format_options: Union[Unset, InputFormat]
+        if isinstance(_src_format_options, Unset):
+            src_format_options = UNSET
         else:
-            output_unit = UnitVolume(_output_unit)
+            src_format_options = InputFormat(_src_format_options)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ApiCallStatus]
         if isinstance(_status, Unset):
             status = UNSET
         else:
-            status = ApiCallStatus(_status)
+            status = _status  # type: ignore[arg-type]
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_volume_conversion = cls(
+        file_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
-            input=input,
-            input_unit=input_unit,
             output=output,
-            output_unit=output_unit,
+            output_format=output_format,
+            output_format_options=output_format_options,
+            outputs=outputs,
+            src_format=src_format,
+            src_format_options=src_format_options,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_volume_conversion.additional_properties = d
-        return unit_volume_conversion
+        file_conversion.additional_properties = d
+        return file_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.3/kittycad/models/update_user.py` & `kittycad-0.4.4/kittycad/models/update_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-F = TypeVar("F", bound="UpdateUser")
+K = TypeVar("K", bound="UpdateUser")
 
 
 @attr.s(auto_attribs=True)
 class UpdateUser:
     """The user-modifiable parts of a User."""  # noqa: E501
 
     company: Union[Unset, str] = UNSET
@@ -43,15 +43,15 @@
             field_dict["last_name"] = last_name
         if phone is not UNSET:
             field_dict["phone"] = phone
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
+    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
         d = src_dict.copy()
         company = d.pop("company", UNSET)
 
         discord = d.pop("discord", UNSET)
 
         first_name = d.pop("first_name", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/user.py` & `kittycad-0.4.4/kittycad/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
-D = TypeVar("D", bound="User")
+K = TypeVar("K", bound="User")
 
 
 @attr.s(auto_attribs=True)
 class User:
     """A user."""  # noqa: E501
 
     company: Union[Unset, str] = UNSET
@@ -79,15 +79,15 @@
             field_dict["phone"] = phone
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[D], src_dict: Dict[str, Any]) -> D:
+    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
         d = src_dict.copy()
         company = d.pop("company", UNSET)
 
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
```

### Comparing `kittycad-0.4.3/kittycad/models/user_results_page.py` & `kittycad-0.4.4/kittycad/models/user_results_page.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-J = TypeVar("J", bound="UserResultsPage")
+H = TypeVar("H", bound="UserResultsPage")
 
 
 @attr.s(auto_attribs=True)
 class UserResultsPage:
     """A single page of results"""  # noqa: E501
 
     from ..models.user import User
@@ -33,15 +33,15 @@
             field_dict["items"] = items
         if next_page is not UNSET:
             field_dict["next_page"] = next_page
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         from ..models.user import User
 
         items = cast(List[User], d.pop("items", UNSET))
 
         next_page = d.pop("next_page", UNSET)
```

### Comparing `kittycad-0.4.3/kittycad/models/verification_token.py` & `kittycad-0.4.4/kittycad/models/verification_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
-F = TypeVar("F", bound="VerificationToken")
+C = TypeVar("C", bound="VerificationToken")
 
 
 @attr.s(auto_attribs=True)
 class VerificationToken:
     """A verification token for a user.
 
     This is typically used to verify a user's email address."""  # noqa: E501
@@ -49,15 +49,15 @@
             field_dict["identifier"] = identifier
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
+    def from_dict(cls: Type[C], src_dict: Dict[str, Any]) -> C:
         d = src_dict.copy()
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
```

### Comparing `kittycad-0.4.3/kittycad/types.py` & `kittycad-0.4.4/kittycad/types.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.3/pyproject.toml` & `kittycad-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kittycad"
-version = "0.4.3"
+version = "0.4.4"
 description = "A client library for accessing KittyCAD"
 
 authors = []
 
 readme = "README.md"
 packages = [
     {include = "kittycad"},
@@ -21,20 +21,20 @@
 autoclasstoc = "^1.6.0"
 black = "^22.0.0"
 isort = "^5.12.0"
 jsonpatch = "^1.32"
 mypy = "^1.2.0"
 openapi-parser = "^0.2.6"
 openapi-spec-validator = "^0.5.6"
-prance = "^0.22.11"
+prance = "^23.6.21"
 pyenchant = "^3.2.2"
 pytest = "^7.0.1"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.0.0"
-ruff = "^0.0.270"
+ruff = "^0.0.277"
 Sphinx = "^6.2.1"
 sphinx-autoapi = "^2.0.1"
 sphinx-autodoc-typehints = "^1.12.0"
 sphinxcontrib-spelling = "^8.0.0"
 sphinx-copybutton = "^0.5.2"
 sphinxext-opengraph = "^0.8.2"
 sphinx-rtd-theme = "^1.0.0"
```

### Comparing `kittycad-0.4.3/PKG-INFO` & `kittycad-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kittycad
-Version: 0.4.3
+Version: 0.4.4
 Summary: A client library for accessing KittyCAD
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

