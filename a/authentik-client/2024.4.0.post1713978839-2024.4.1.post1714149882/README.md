# Comparing `tmp/authentik_client-2024.4.0.post1713978839.tar.gz` & `tmp/authentik_client-2024.4.1.post1714149882.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authentik_client-2024.4.0.post1713978839.tar", max compression
+gzip compressed data, was "authentik_client-2024.4.1.post1714149882.tar", max compression
```

## Comparing `authentik_client-2024.4.0.post1713978839.tar` & `authentik_client-2024.4.1.post1714149882.tar`

### file list

```diff
@@ -1,595 +1,595 @@
--rw-r--r--   0        0        0   143943 2024-04-24 17:14:13.267741 authentik_client-2024.4.0.post1713978839/README.md
--rw-r--r--   0        0        0    48482 2024-04-24 17:14:13.283741 authentik_client-2024.4.0.post1713978839/authentik_client/__init__.py
--rw-r--r--   0        0        0     1170 2024-04-24 17:14:13.287742 authentik_client-2024.4.0.post1713978839/authentik_client/api/__init__.py
--rw-r--r--   0        0        0    97518 2024-04-24 17:14:12.923737 authentik_client-2024.4.0.post1713978839/authentik_client/api/admin_api.py
--rw-r--r--   0        0        0   700271 2024-04-24 17:14:12.943737 authentik_client-2024.4.0.post1713978839/authentik_client/api/authenticators_api.py
--rw-r--r--   0        0        0   701197 2024-04-24 17:14:12.971737 authentik_client-2024.4.0.post1713978839/authentik_client/api/core_api.py
--rw-r--r--   0        0        0   116805 2024-04-24 17:14:12.987738 authentik_client-2024.4.0.post1713978839/authentik_client/api/crypto_api.py
--rw-r--r--   0        0        0   107946 2024-04-24 17:14:12.995738 authentik_client-2024.4.0.post1713978839/authentik_client/api/enterprise_api.py
--rw-r--r--   0        0        0   408008 2024-04-24 17:14:13.007738 authentik_client-2024.4.0.post1713978839/authentik_client/api/events_api.py
--rw-r--r--   0        0        0   280806 2024-04-24 17:14:13.023738 authentik_client-2024.4.0.post1713978839/authentik_client/api/flows_api.py
--rw-r--r--   0        0        0   101134 2024-04-24 17:14:13.031738 authentik_client-2024.4.0.post1713978839/authentik_client/api/managed_api.py
--rw-r--r--   0        0        0   135649 2024-04-24 17:14:13.043738 authentik_client-2024.4.0.post1713978839/authentik_client/api/oauth2_api.py
--rw-r--r--   0        0        0   413301 2024-04-24 17:14:13.055739 authentik_client-2024.4.0.post1713978839/authentik_client/api/outposts_api.py
--rw-r--r--   0        0        0   725201 2024-04-24 17:14:13.079739 authentik_client-2024.4.0.post1713978839/authentik_client/api/policies_api.py
--rw-r--r--   0        0        0   552586 2024-04-24 17:14:13.099739 authentik_client-2024.4.0.post1713978839/authentik_client/api/propertymappings_api.py
--rw-r--r--   0        0        0   718066 2024-04-24 17:14:13.123739 authentik_client-2024.4.0.post1713978839/authentik_client/api/providers_api.py
--rw-r--r--   0        0        0   150485 2024-04-24 17:14:13.135740 authentik_client-2024.4.0.post1713978839/authentik_client/api/rac_api.py
--rw-r--r--   0        0        0   207550 2024-04-24 17:14:13.147740 authentik_client-2024.4.0.post1713978839/authentik_client/api/rbac_api.py
--rw-r--r--   0        0        0    10391 2024-04-24 17:14:13.155740 authentik_client-2024.4.0.post1713978839/authentik_client/api/root_api.py
--rw-r--r--   0        0        0    11845 2024-04-24 17:14:13.159740 authentik_client-2024.4.0.post1713978839/authentik_client/api/schema_api.py
--rw-r--r--   0        0        0  1037225 2024-04-24 17:14:13.191740 authentik_client-2024.4.0.post1713978839/authentik_client/api/sources_api.py
--rw-r--r--   0        0        0  1945986 2024-04-24 17:14:13.235741 authentik_client-2024.4.0.post1713978839/authentik_client/api/stages_api.py
--rw-r--r--   0        0        0   157909 2024-04-24 17:14:13.255741 authentik_client-2024.4.0.post1713978839/authentik_client/api/tenants_api.py
--rw-r--r--   0        0        0    25779 2024-04-24 17:14:13.287742 authentik_client-2024.4.0.post1713978839/authentik_client/api_client.py
--rw-r--r--   0        0        0      652 2024-04-24 17:14:13.287742 authentik_client-2024.4.0.post1713978839/authentik_client/api_response.py
--rw-r--r--   0        0        0    14724 2024-04-24 17:14:13.279741 authentik_client-2024.4.0.post1713978839/authentik_client/configuration.py
--rw-r--r--   0        0        0     5934 2024-04-24 17:14:13.287742 authentik_client-2024.4.0.post1713978839/authentik_client/exceptions.py
--rw-r--r--   0        0        0    46784 2024-04-24 17:14:13.283741 authentik_client-2024.4.0.post1713978839/authentik_client/models/__init__.py
--rw-r--r--   0        0        0     4513 2024-04-24 17:14:09.987701 authentik_client-2024.4.0.post1713978839/authentik_client/models/access_denied_challenge.py
--rw-r--r--   0        0        0     2482 2024-04-24 17:14:10.003701 authentik_client-2024.4.0.post1713978839/authentik_client/models/app.py
--rw-r--r--   0        0        0     4230 2024-04-24 17:14:10.007701 authentik_client-2024.4.0.post1713978839/authentik_client/models/app_enum.py
--rw-r--r--   0        0        0     2702 2024-04-24 17:14:10.019701 authentik_client-2024.4.0.post1713978839/authentik_client/models/apple_challenge_response_request.py
--rw-r--r--   0        0        0     4508 2024-04-24 17:14:10.027701 authentik_client-2024.4.0.post1713978839/authentik_client/models/apple_login_challenge.py
--rw-r--r--   0        0        0     6686 2024-04-24 17:14:10.039702 authentik_client-2024.4.0.post1713978839/authentik_client/models/application.py
--rw-r--r--   0        0        0     4473 2024-04-24 17:14:10.047702 authentik_client-2024.4.0.post1713978839/authentik_client/models/application_request.py
--rw-r--r--   0        0        0      711 2024-04-24 17:14:10.051702 authentik_client-2024.4.0.post1713978839/authentik_client/models/auth_mode_enum.py
--rw-r--r--   0        0        0      709 2024-04-24 17:14:10.055702 authentik_client-2024.4.0.post1713978839/authentik_client/models/auth_type_enum.py
--rw-r--r--   0        0        0     5195 2024-04-24 17:14:10.059702 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticated_session.py
--rw-r--r--   0        0        0     3064 2024-04-24 17:14:10.067702 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticated_session_asn.py
--rw-r--r--   0        0        0     2826 2024-04-24 17:14:10.075702 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticated_session_geo_ip.py
--rw-r--r--   0        0        0     3865 2024-04-24 17:14:10.079702 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticated_session_user_agent.py
--rw-r--r--   0        0        0     2646 2024-04-24 17:14:10.087702 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticated_session_user_agent_device.py
--rw-r--r--   0        0        0     2792 2024-04-24 17:14:10.095702 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticated_session_user_agent_os.py
--rw-r--r--   0        0        0     2725 2024-04-24 17:14:10.099702 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticated_session_user_agent_user_agent.py
--rw-r--r--   0        0        0      895 2024-04-24 17:14:10.103702 authentik_client-2024.4.0.post1713978839/authentik_client/models/authentication_enum.py
--rw-r--r--   0        0        0      782 2024-04-24 17:14:10.107702 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_attachment_enum.py
--rw-r--r--   0        0        0     4686 2024-04-24 17:14:10.115702 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_duo_challenge.py
--rw-r--r--   0        0        0     2743 2024-04-24 17:14:10.123703 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_duo_challenge_response_request.py
--rw-r--r--   0        0        0     5327 2024-04-24 17:14:10.131703 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_duo_stage.py
--rw-r--r--   0        0        0     2768 2024-04-24 17:14:10.135703 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_duo_stage_device_import_response.py
--rw-r--r--   0        0        0     2785 2024-04-24 17:14:10.143703 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py
--rw-r--r--   0        0        0     4744 2024-04-24 17:14:10.151703 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_duo_stage_request.py
--rw-r--r--   0        0        0     4594 2024-04-24 17:14:10.159703 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_sms_challenge.py
--rw-r--r--   0        0        0     3022 2024-04-24 17:14:10.167703 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_sms_challenge_response_request.py
--rw-r--r--   0        0        0     6409 2024-04-24 17:14:10.175703 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_sms_stage.py
--rw-r--r--   0        0        0     5595 2024-04-24 17:14:10.183703 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_sms_stage_request.py
--rw-r--r--   0        0        0     4474 2024-04-24 17:14:10.191703 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_static_challenge.py
--rw-r--r--   0        0        0     2761 2024-04-24 17:14:10.195704 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_static_challenge_response_request.py
--rw-r--r--   0        0        0     5363 2024-04-24 17:14:10.203704 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_static_stage.py
--rw-r--r--   0        0        0     4392 2024-04-24 17:14:10.211704 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_static_stage_request.py
--rw-r--r--   0        0        0     4468 2024-04-24 17:14:10.219704 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_totp_challenge.py
--rw-r--r--   0        0        0     2858 2024-04-24 17:14:10.223704 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_totp_challenge_response_request.py
--rw-r--r--   0        0        0     5132 2024-04-24 17:14:10.231704 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_totp_stage.py
--rw-r--r--   0        0        0     4201 2024-04-24 17:14:10.235704 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_totp_stage_request.py
--rw-r--r--   0        0        0     6722 2024-04-24 17:14:10.243704 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_validate_stage.py
--rw-r--r--   0        0        0     4893 2024-04-24 17:14:10.251704 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_validate_stage_request.py
--rw-r--r--   0        0        0     5717 2024-04-24 17:14:10.255704 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_validation_challenge.py
--rw-r--r--   0        0        0     3805 2024-04-24 17:14:10.263704 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_validation_challenge_response_request.py
--rw-r--r--   0        0        0     4499 2024-04-24 17:14:10.267704 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_web_authn_challenge.py
--rw-r--r--   0        0        0     2852 2024-04-24 17:14:10.275704 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_web_authn_challenge_response_request.py
--rw-r--r--   0        0        0     7081 2024-04-24 17:14:10.279705 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_web_authn_stage.py
--rw-r--r--   0        0        0     5302 2024-04-24 17:14:10.283705 authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_web_authn_stage_request.py
--rw-r--r--   0        0        0     2718 2024-04-24 17:14:10.287705 authentik_client-2024.4.0.post1713978839/authentik_client/models/auto_submit_challenge_response_request.py
--rw-r--r--   0        0        0     4388 2024-04-24 17:14:10.295705 authentik_client-2024.4.0.post1713978839/authentik_client/models/autosubmit_challenge.py
--rw-r--r--   0        0        0      950 2024-04-24 17:14:10.299705 authentik_client-2024.4.0.post1713978839/authentik_client/models/backends_enum.py
--rw-r--r--   0        0        0      748 2024-04-24 17:14:10.299705 authentik_client-2024.4.0.post1713978839/authentik_client/models/binding_type_enum.py
--rw-r--r--   0        0        0     2995 2024-04-24 17:14:10.303705 authentik_client-2024.4.0.post1713978839/authentik_client/models/blueprint_file.py
--rw-r--r--   0        0        0     4453 2024-04-24 17:14:10.307705 authentik_client-2024.4.0.post1713978839/authentik_client/models/blueprint_instance.py
--rw-r--r--   0        0        0     3208 2024-04-24 17:14:10.315705 authentik_client-2024.4.0.post1713978839/authentik_client/models/blueprint_instance_request.py
--rw-r--r--   0        0        0      836 2024-04-24 17:14:10.315705 authentik_client-2024.4.0.post1713978839/authentik_client/models/blueprint_instance_status_enum.py
--rw-r--r--   0        0        0     6255 2024-04-24 17:14:10.319705 authentik_client-2024.4.0.post1713978839/authentik_client/models/brand.py
--rw-r--r--   0        0        0     6307 2024-04-24 17:14:10.327705 authentik_client-2024.4.0.post1713978839/authentik_client/models/brand_request.py
--rw-r--r--   0        0        0     2501 2024-04-24 17:14:10.331705 authentik_client-2024.4.0.post1713978839/authentik_client/models/cache.py
--rw-r--r--   0        0        0      875 2024-04-24 17:14:10.335705 authentik_client-2024.4.0.post1713978839/authentik_client/models/capabilities_enum.py
--rw-r--r--   0        0        0     4476 2024-04-24 17:14:10.339705 authentik_client-2024.4.0.post1713978839/authentik_client/models/captcha_challenge.py
--rw-r--r--   0        0        0     2797 2024-04-24 17:14:10.343705 authentik_client-2024.4.0.post1713978839/authentik_client/models/captcha_challenge_response_request.py
--rw-r--r--   0        0        0     4438 2024-04-24 17:14:10.347705 authentik_client-2024.4.0.post1713978839/authentik_client/models/captcha_stage.py
--rw-r--r--   0        0        0     3774 2024-04-24 17:14:10.351705 authentik_client-2024.4.0.post1713978839/authentik_client/models/captcha_stage_request.py
--rw-r--r--   0        0        0     2522 2024-04-24 17:14:10.363705 authentik_client-2024.4.0.post1713978839/authentik_client/models/certificate_data.py
--rw-r--r--   0        0        0     2861 2024-04-24 17:14:10.371706 authentik_client-2024.4.0.post1713978839/authentik_client/models/certificate_generation_request.py
--rw-r--r--   0        0        0     6655 2024-04-24 17:14:10.375706 authentik_client-2024.4.0.post1713978839/authentik_client/models/certificate_key_pair.py
--rw-r--r--   0        0        0     2989 2024-04-24 17:14:10.379706 authentik_client-2024.4.0.post1713978839/authentik_client/models/certificate_key_pair_request.py
--rw-r--r--   0        0        0      747 2024-04-24 17:14:10.383706 authentik_client-2024.4.0.post1713978839/authentik_client/models/challenge_choices.py
--rw-r--r--   0        0        0    24236 2024-04-24 17:14:10.391706 authentik_client-2024.4.0.post1713978839/authentik_client/models/challenge_types.py
--rw-r--r--   0        0        0      729 2024-04-24 17:14:10.391706 authentik_client-2024.4.0.post1713978839/authentik_client/models/client_type_enum.py
--rw-r--r--   0        0        0     3539 2024-04-24 17:14:10.399706 authentik_client-2024.4.0.post1713978839/authentik_client/models/config.py
--rw-r--r--   0        0        0     4021 2024-04-24 17:14:10.403706 authentik_client-2024.4.0.post1713978839/authentik_client/models/connection_token.py
--rw-r--r--   0        0        0     2662 2024-04-24 17:14:10.403706 authentik_client-2024.4.0.post1713978839/authentik_client/models/connection_token_request.py
--rw-r--r--   0        0        0     5736 2024-04-24 17:14:10.411706 authentik_client-2024.4.0.post1713978839/authentik_client/models/consent_challenge.py
--rw-r--r--   0        0        0     2838 2024-04-24 17:14:10.415706 authentik_client-2024.4.0.post1713978839/authentik_client/models/consent_challenge_response_request.py
--rw-r--r--   0        0        0     2513 2024-04-24 17:14:10.419706 authentik_client-2024.4.0.post1713978839/authentik_client/models/consent_permission.py
--rw-r--r--   0        0        0     4511 2024-04-24 17:14:10.423706 authentik_client-2024.4.0.post1713978839/authentik_client/models/consent_stage.py
--rw-r--r--   0        0        0      783 2024-04-24 17:14:10.423706 authentik_client-2024.4.0.post1713978839/authentik_client/models/consent_stage_mode_enum.py
--rw-r--r--   0        0        0     3569 2024-04-24 17:14:10.427706 authentik_client-2024.4.0.post1713978839/authentik_client/models/consent_stage_request.py
--rw-r--r--   0        0        0     2891 2024-04-24 17:14:10.431707 authentik_client-2024.4.0.post1713978839/authentik_client/models/contextual_flow_info.py
--rw-r--r--   0        0        0      879 2024-04-24 17:14:10.435706 authentik_client-2024.4.0.post1713978839/authentik_client/models/contextual_flow_info_layout_enum.py
--rw-r--r--   0        0        0     2657 2024-04-24 17:14:10.439706 authentik_client-2024.4.0.post1713978839/authentik_client/models/coordinate.py
--rw-r--r--   0        0        0     4704 2024-04-24 17:14:10.443707 authentik_client-2024.4.0.post1713978839/authentik_client/models/current_brand.py
--rw-r--r--   0        0        0      771 2024-04-24 17:14:10.443707 authentik_client-2024.4.0.post1713978839/authentik_client/models/denied_action_enum.py
--rw-r--r--   0        0        0     4200 2024-04-24 17:14:10.447707 authentik_client-2024.4.0.post1713978839/authentik_client/models/deny_stage.py
--rw-r--r--   0        0        0     3230 2024-04-24 17:14:10.451707 authentik_client-2024.4.0.post1713978839/authentik_client/models/deny_stage_request.py
--rw-r--r--   0        0        0     3522 2024-04-24 17:14:10.459707 authentik_client-2024.4.0.post1713978839/authentik_client/models/device.py
--rw-r--r--   0        0        0     2657 2024-04-24 17:14:10.463707 authentik_client-2024.4.0.post1713978839/authentik_client/models/device_challenge.py
--rw-r--r--   0        0        0     2792 2024-04-24 17:14:10.467707 authentik_client-2024.4.0.post1713978839/authentik_client/models/device_challenge_request.py
--rw-r--r--   0        0        0      780 2024-04-24 17:14:10.471707 authentik_client-2024.4.0.post1713978839/authentik_client/models/device_classes_enum.py
--rw-r--r--   0        0        0     1244 2024-04-24 17:14:10.475707 authentik_client-2024.4.0.post1713978839/authentik_client/models/digest_algorithm_enum.py
--rw-r--r--   0        0        0      695 2024-04-24 17:14:10.479707 authentik_client-2024.4.0.post1713978839/authentik_client/models/digits_enum.py
--rw-r--r--   0        0        0     4969 2024-04-24 17:14:10.479707 authentik_client-2024.4.0.post1713978839/authentik_client/models/docker_service_connection.py
--rw-r--r--   0        0        0     4087 2024-04-24 17:14:10.483707 authentik_client-2024.4.0.post1713978839/authentik_client/models/docker_service_connection_request.py
--rw-r--r--   0        0        0     2847 2024-04-24 17:14:10.487707 authentik_client-2024.4.0.post1713978839/authentik_client/models/domain.py
--rw-r--r--   0        0        0     2746 2024-04-24 17:14:10.491707 authentik_client-2024.4.0.post1713978839/authentik_client/models/domain_request.py
--rw-r--r--   0        0        0     4155 2024-04-24 17:14:10.495707 authentik_client-2024.4.0.post1713978839/authentik_client/models/dummy_challenge.py
--rw-r--r--   0        0        0     2681 2024-04-24 17:14:10.499707 authentik_client-2024.4.0.post1713978839/authentik_client/models/dummy_challenge_response_request.py
--rw-r--r--   0        0        0     4515 2024-04-24 17:14:10.503707 authentik_client-2024.4.0.post1713978839/authentik_client/models/dummy_policy.py
--rw-r--r--   0        0        0     3237 2024-04-24 17:14:10.507707 authentik_client-2024.4.0.post1713978839/authentik_client/models/dummy_policy_request.py
--rw-r--r--   0        0        0     4213 2024-04-24 17:14:10.511707 authentik_client-2024.4.0.post1713978839/authentik_client/models/dummy_stage.py
--rw-r--r--   0        0        0     3232 2024-04-24 17:14:10.515707 authentik_client-2024.4.0.post1713978839/authentik_client/models/dummy_stage_request.py
--rw-r--r--   0        0        0     2720 2024-04-24 17:14:10.519708 authentik_client-2024.4.0.post1713978839/authentik_client/models/duo_device.py
--rw-r--r--   0        0        0     2575 2024-04-24 17:14:10.523707 authentik_client-2024.4.0.post1713978839/authentik_client/models/duo_device_enrollment_status.py
--rw-r--r--   0        0        0     2619 2024-04-24 17:14:10.523707 authentik_client-2024.4.0.post1713978839/authentik_client/models/duo_device_request.py
--rw-r--r--   0        0        0      748 2024-04-24 17:14:10.527708 authentik_client-2024.4.0.post1713978839/authentik_client/models/duo_response_enum.py
--rw-r--r--   0        0        0     4090 2024-04-24 17:14:10.531708 authentik_client-2024.4.0.post1713978839/authentik_client/models/email_challenge.py
--rw-r--r--   0        0        0     2770 2024-04-24 17:14:10.539708 authentik_client-2024.4.0.post1713978839/authentik_client/models/email_challenge_response_request.py
--rw-r--r--   0        0        0     5902 2024-04-24 17:14:10.543708 authentik_client-2024.4.0.post1713978839/authentik_client/models/email_stage.py
--rw-r--r--   0        0        0     5121 2024-04-24 17:14:10.551708 authentik_client-2024.4.0.post1713978839/authentik_client/models/email_stage_request.py
--rw-r--r--   0        0        0     4707 2024-04-24 17:14:10.559708 authentik_client-2024.4.0.post1713978839/authentik_client/models/endpoint.py
--rw-r--r--   0        0        0     3678 2024-04-24 17:14:10.567708 authentik_client-2024.4.0.post1713978839/authentik_client/models/endpoint_request.py
--rw-r--r--   0        0        0     2530 2024-04-24 17:14:10.571708 authentik_client-2024.4.0.post1713978839/authentik_client/models/error_detail.py
--rw-r--r--   0        0        0     3309 2024-04-24 17:14:10.579708 authentik_client-2024.4.0.post1713978839/authentik_client/models/error_reporting_config.py
--rw-r--r--   0        0        0     4129 2024-04-24 17:14:10.583708 authentik_client-2024.4.0.post1713978839/authentik_client/models/event.py
--rw-r--r--   0        0        0     1730 2024-04-24 17:14:10.587708 authentik_client-2024.4.0.post1713978839/authentik_client/models/event_actions.py
--rw-r--r--   0        0        0     6006 2024-04-24 17:14:10.595708 authentik_client-2024.4.0.post1713978839/authentik_client/models/event_matcher_policy.py
--rw-r--r--   0        0        0     4807 2024-04-24 17:14:10.599708 authentik_client-2024.4.0.post1713978839/authentik_client/models/event_matcher_policy_request.py
--rw-r--r--   0        0        0     3990 2024-04-24 17:14:10.607709 authentik_client-2024.4.0.post1713978839/authentik_client/models/event_request.py
--rw-r--r--   0        0        0     2697 2024-04-24 17:14:10.611709 authentik_client-2024.4.0.post1713978839/authentik_client/models/event_top_per_user.py
--rw-r--r--   0        0        0     3926 2024-04-24 17:14:10.619709 authentik_client-2024.4.0.post1713978839/authentik_client/models/expiring_base_grant_model.py
--rw-r--r--   0        0        0     4191 2024-04-24 17:14:10.627709 authentik_client-2024.4.0.post1713978839/authentik_client/models/expression_policy.py
--rw-r--r--   0        0        0     2992 2024-04-24 17:14:10.635709 authentik_client-2024.4.0.post1713978839/authentik_client/models/expression_policy_request.py
--rw-r--r--   0        0        0     4524 2024-04-24 17:14:10.647709 authentik_client-2024.4.0.post1713978839/authentik_client/models/extra_role_object_permission.py
--rw-r--r--   0        0        0     4524 2024-04-24 17:14:10.655709 authentik_client-2024.4.0.post1713978839/authentik_client/models/extra_user_object_permission.py
--rw-r--r--   0        0        0     2519 2024-04-24 17:14:10.663709 authentik_client-2024.4.0.post1713978839/authentik_client/models/file_path_request.py
--rw-r--r--   0        0        0     6047 2024-04-24 17:14:10.671709 authentik_client-2024.4.0.post1713978839/authentik_client/models/flow.py
--rw-r--r--   0        0        0    25850 2024-04-24 17:14:10.679710 authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_challenge_response_request.py
--rw-r--r--   0        0        0      934 2024-04-24 17:14:10.679710 authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_designation_enum.py
--rw-r--r--   0        0        0     2533 2024-04-24 17:14:10.691710 authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_diagram.py
--rw-r--r--   0        0        0     4505 2024-04-24 17:14:10.699710 authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_error_challenge.py
--rw-r--r--   0        0        0     3111 2024-04-24 17:14:10.715710 authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_import_result.py
--rw-r--r--   0        0        0     3418 2024-04-24 17:14:10.723710 authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_inspection.py
--rw-r--r--   0        0        0     3875 2024-04-24 17:14:10.727710 authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_inspector_plan.py
--rw-r--r--   0        0        0      837 2024-04-24 17:14:10.731710 authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_layout_enum.py
--rw-r--r--   0        0        0     4741 2024-04-24 17:14:10.739710 authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_request.py
--rw-r--r--   0        0        0     5223 2024-04-24 17:14:10.743710 authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_set.py
--rw-r--r--   0        0        0     4459 2024-04-24 17:14:10.751710 authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_set_request.py
--rw-r--r--   0        0        0     4763 2024-04-24 17:14:10.759710 authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_stage_binding.py
--rw-r--r--   0        0        0     3983 2024-04-24 17:14:10.763711 authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_stage_binding_request.py
--rw-r--r--   0        0        0     2641 2024-04-24 17:14:10.771710 authentik_client-2024.4.0.post1713978839/authentik_client/models/footer_link.py
--rw-r--r--   0        0        0     2531 2024-04-24 17:14:10.775711 authentik_client-2024.4.0.post1713978839/authentik_client/models/generic_error.py
--rw-r--r--   0        0        0      865 2024-04-24 17:14:10.779711 authentik_client-2024.4.0.post1713978839/authentik_client/models/geoip_binding_enum.py
--rw-r--r--   0        0        0     5445 2024-04-24 17:14:10.783711 authentik_client-2024.4.0.post1713978839/authentik_client/models/group.py
--rw-r--r--   0        0        0     4209 2024-04-24 17:14:10.799711 authentik_client-2024.4.0.post1713978839/authentik_client/models/group_member.py
--rw-r--r--   0        0        0     4006 2024-04-24 17:14:10.807711 authentik_client-2024.4.0.post1713978839/authentik_client/models/group_member_request.py
--rw-r--r--   0        0        0     3347 2024-04-24 17:14:10.811711 authentik_client-2024.4.0.post1713978839/authentik_client/models/group_request.py
--rw-r--r--   0        0        0     6080 2024-04-24 17:14:10.819711 authentik_client-2024.4.0.post1713978839/authentik_client/models/identification_challenge.py
--rw-r--r--   0        0        0     3174 2024-04-24 17:14:10.823711 authentik_client-2024.4.0.post1713978839/authentik_client/models/identification_challenge_response_request.py
--rw-r--r--   0        0        0     7503 2024-04-24 17:14:10.827711 authentik_client-2024.4.0.post1713978839/authentik_client/models/identification_stage.py
--rw-r--r--   0        0        0     6533 2024-04-24 17:14:10.831711 authentik_client-2024.4.0.post1713978839/authentik_client/models/identification_stage_request.py
--rw-r--r--   0        0        0     2438 2024-04-24 17:14:10.835711 authentik_client-2024.4.0.post1713978839/authentik_client/models/install_id.py
--rw-r--r--   0        0        0      771 2024-04-24 17:14:10.839712 authentik_client-2024.4.0.post1713978839/authentik_client/models/intent_enum.py
--rw-r--r--   0        0        0      800 2024-04-24 17:14:10.839712 authentik_client-2024.4.0.post1713978839/authentik_client/models/invalid_response_action_enum.py
--rw-r--r--   0        0        0     4878 2024-04-24 17:14:10.843711 authentik_client-2024.4.0.post1713978839/authentik_client/models/invitation.py
--rw-r--r--   0        0        0     3895 2024-04-24 17:14:10.847711 authentik_client-2024.4.0.post1713978839/authentik_client/models/invitation_request.py
--rw-r--r--   0        0        0     4508 2024-04-24 17:14:10.851712 authentik_client-2024.4.0.post1713978839/authentik_client/models/invitation_stage.py
--rw-r--r--   0        0        0     3527 2024-04-24 17:14:10.855712 authentik_client-2024.4.0.post1713978839/authentik_client/models/invitation_stage_request.py
--rw-r--r--   0        0        0      729 2024-04-24 17:14:10.859712 authentik_client-2024.4.0.post1713978839/authentik_client/models/issuer_mode_enum.py
--rw-r--r--   0        0        0     4386 2024-04-24 17:14:10.863712 authentik_client-2024.4.0.post1713978839/authentik_client/models/kubernetes_service_connection.py
--rw-r--r--   0        0        0     3454 2024-04-24 17:14:10.863712 authentik_client-2024.4.0.post1713978839/authentik_client/models/kubernetes_service_connection_request.py
--rw-r--r--   0        0        0     2811 2024-04-24 17:14:10.871712 authentik_client-2024.4.0.post1713978839/authentik_client/models/ldap_debug.py
--rw-r--r--   0        0        0     5765 2024-04-24 17:14:10.875712 authentik_client-2024.4.0.post1713978839/authentik_client/models/ldap_outpost_config.py
--rw-r--r--   0        0        0     4378 2024-04-24 17:14:10.875712 authentik_client-2024.4.0.post1713978839/authentik_client/models/ldap_property_mapping.py
--rw-r--r--   0        0        0     3478 2024-04-24 17:14:10.879712 authentik_client-2024.4.0.post1713978839/authentik_client/models/ldap_property_mapping_request.py
--rw-r--r--   0        0        0     8694 2024-04-24 17:14:10.883712 authentik_client-2024.4.0.post1713978839/authentik_client/models/ldap_provider.py
--rw-r--r--   0        0        0     6192 2024-04-24 17:14:10.887712 authentik_client-2024.4.0.post1713978839/authentik_client/models/ldap_provider_request.py
--rw-r--r--   0        0        0    11791 2024-04-24 17:14:10.895712 authentik_client-2024.4.0.post1713978839/authentik_client/models/ldap_source.py
--rw-r--r--   0        0        0     9542 2024-04-24 17:14:10.899712 authentik_client-2024.4.0.post1713978839/authentik_client/models/ldap_source_request.py
--rw-r--r--   0        0        0     3129 2024-04-24 17:14:10.903712 authentik_client-2024.4.0.post1713978839/authentik_client/models/ldap_sync_status.py
--rw-r--r--   0        0        0      726 2024-04-24 17:14:10.867712 authentik_client-2024.4.0.post1713978839/authentik_client/models/ldapapi_access_mode.py
--rw-r--r--   0        0        0     3278 2024-04-24 17:14:10.907712 authentik_client-2024.4.0.post1713978839/authentik_client/models/license.py
--rw-r--r--   0        0        0     2897 2024-04-24 17:14:10.911712 authentik_client-2024.4.0.post1713978839/authentik_client/models/license_forecast.py
--rw-r--r--   0        0        0     2509 2024-04-24 17:14:10.915712 authentik_client-2024.4.0.post1713978839/authentik_client/models/license_request.py
--rw-r--r--   0        0        0     3222 2024-04-24 17:14:10.919712 authentik_client-2024.4.0.post1713978839/authentik_client/models/license_summary.py
--rw-r--r--   0        0        0     2411 2024-04-24 17:14:10.923712 authentik_client-2024.4.0.post1713978839/authentik_client/models/link.py
--rw-r--r--   0        0        0     2882 2024-04-24 17:14:10.927713 authentik_client-2024.4.0.post1713978839/authentik_client/models/log_event.py
--rw-r--r--   0        0        0      843 2024-04-24 17:14:10.927713 authentik_client-2024.4.0.post1713978839/authentik_client/models/log_level_enum.py
--rw-r--r--   0        0        0     6520 2024-04-24 17:14:10.935713 authentik_client-2024.4.0.post1713978839/authentik_client/models/login_challenge_types.py
--rw-r--r--   0        0        0     4171 2024-04-24 17:14:10.939713 authentik_client-2024.4.0.post1713978839/authentik_client/models/login_metrics.py
--rw-r--r--   0        0        0     3192 2024-04-24 17:14:10.943713 authentik_client-2024.4.0.post1713978839/authentik_client/models/login_source.py
--rw-r--r--   0        0        0     2513 2024-04-24 17:14:10.947713 authentik_client-2024.4.0.post1713978839/authentik_client/models/metadata.py
--rw-r--r--   0        0        0     7604 2024-04-24 17:14:10.951713 authentik_client-2024.4.0.post1713978839/authentik_client/models/model_enum.py
--rw-r--r--   0        0        0     9828 2024-04-24 17:14:10.955713 authentik_client-2024.4.0.post1713978839/authentik_client/models/model_request.py
--rw-r--r--   0        0        0     1559 2024-04-24 17:14:10.955713 authentik_client-2024.4.0.post1713978839/authentik_client/models/name_id_policy_enum.py
--rw-r--r--   0        0        0      831 2024-04-24 17:14:10.959713 authentik_client-2024.4.0.post1713978839/authentik_client/models/network_binding_enum.py
--rw-r--r--   0        0        0      764 2024-04-24 17:14:10.959713 authentik_client-2024.4.0.post1713978839/authentik_client/models/not_configured_action_enum.py
--rw-r--r--   0        0        0     3479 2024-04-24 17:14:10.963713 authentik_client-2024.4.0.post1713978839/authentik_client/models/notification.py
--rw-r--r--   0        0        0     2858 2024-04-24 17:14:10.963713 authentik_client-2024.4.0.post1713978839/authentik_client/models/notification_request.py
--rw-r--r--   0        0        0     4010 2024-04-24 17:14:10.967713 authentik_client-2024.4.0.post1713978839/authentik_client/models/notification_rule.py
--rw-r--r--   0        0        0     3549 2024-04-24 17:14:10.971713 authentik_client-2024.4.0.post1713978839/authentik_client/models/notification_rule_request.py
--rw-r--r--   0        0        0     3760 2024-04-24 17:14:10.975713 authentik_client-2024.4.0.post1713978839/authentik_client/models/notification_transport.py
--rw-r--r--   0        0        0      818 2024-04-24 17:14:10.975713 authentik_client-2024.4.0.post1713978839/authentik_client/models/notification_transport_mode_enum.py
--rw-r--r--   0        0        0     3500 2024-04-24 17:14:10.979713 authentik_client-2024.4.0.post1713978839/authentik_client/models/notification_transport_request.py
--rw-r--r--   0        0        0     2503 2024-04-24 17:14:10.983713 authentik_client-2024.4.0.post1713978839/authentik_client/models/notification_transport_test.py
--rw-r--r--   0        0        0     2707 2024-04-24 17:14:10.987713 authentik_client-2024.4.0.post1713978839/authentik_client/models/notification_webhook_mapping.py
--rw-r--r--   0        0        0     2717 2024-04-24 17:14:10.991713 authentik_client-2024.4.0.post1713978839/authentik_client/models/notification_webhook_mapping_request.py
--rw-r--r--   0        0        0     8888 2024-04-24 17:14:10.995713 authentik_client-2024.4.0.post1713978839/authentik_client/models/o_auth2_provider.py
--rw-r--r--   0        0        0     6654 2024-04-24 17:14:10.999713 authentik_client-2024.4.0.post1713978839/authentik_client/models/o_auth2_provider_request.py
--rw-r--r--   0        0        0     3482 2024-04-24 17:14:11.003713 authentik_client-2024.4.0.post1713978839/authentik_client/models/o_auth2_provider_setup_urls.py
--rw-r--r--   0        0        0     4164 2024-04-24 17:14:11.007713 authentik_client-2024.4.0.post1713978839/authentik_client/models/o_auth_device_code_challenge.py
--rw-r--r--   0        0        0     2846 2024-04-24 17:14:11.011714 authentik_client-2024.4.0.post1713978839/authentik_client/models/o_auth_device_code_challenge_response_request.py
--rw-r--r--   0        0        0     4213 2024-04-24 17:14:11.015714 authentik_client-2024.4.0.post1713978839/authentik_client/models/o_auth_device_code_finish_challenge.py
--rw-r--r--   0        0        0     2816 2024-04-24 17:14:11.019714 authentik_client-2024.4.0.post1713978839/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py
--rw-r--r--   0        0        0    10563 2024-04-24 17:14:11.023714 authentik_client-2024.4.0.post1713978839/authentik_client/models/o_auth_source.py
--rw-r--r--   0        0        0     8013 2024-04-24 17:14:11.027714 authentik_client-2024.4.0.post1713978839/authentik_client/models/o_auth_source_request.py
--rw-r--r--   0        0        0     3922 2024-04-24 17:14:11.031714 authentik_client-2024.4.0.post1713978839/authentik_client/models/open_id_connect_configuration.py
--rw-r--r--   0        0        0     5545 2024-04-24 17:14:11.035714 authentik_client-2024.4.0.post1713978839/authentik_client/models/outpost.py
--rw-r--r--   0        0        0     2541 2024-04-24 17:14:11.039714 authentik_client-2024.4.0.post1713978839/authentik_client/models/outpost_default_config.py
--rw-r--r--   0        0        0     3755 2024-04-24 17:14:11.043714 authentik_client-2024.4.0.post1713978839/authentik_client/models/outpost_health.py
--rw-r--r--   0        0        0     4050 2024-04-24 17:14:11.047714 authentik_client-2024.4.0.post1713978839/authentik_client/models/outpost_request.py
--rw-r--r--   0        0        0      752 2024-04-24 17:14:11.051714 authentik_client-2024.4.0.post1713978839/authentik_client/models/outpost_type_enum.py
--rw-r--r--   0        0        0     3322 2024-04-24 17:14:11.055714 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_application_list.py
--rw-r--r--   0        0        0     3395 2024-04-24 17:14:11.055714 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_authenticated_session_list.py
--rw-r--r--   0        0        0     3404 2024-04-24 17:14:11.059714 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_authenticator_duo_stage_list.py
--rw-r--r--   0        0        0     3404 2024-04-24 17:14:11.063714 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_authenticator_sms_stage_list.py
--rw-r--r--   0        0        0     3428 2024-04-24 17:14:11.067714 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_authenticator_static_stage_list.py
--rw-r--r--   0        0        0     3412 2024-04-24 17:14:11.071714 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_authenticator_totp_stage_list.py
--rw-r--r--   0        0        0     3444 2024-04-24 17:14:11.075714 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_authenticator_validate_stage_list.py
--rw-r--r--   0        0        0     3445 2024-04-24 17:14:11.079714 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_authenticator_web_authn_stage_list.py
--rw-r--r--   0        0        0     3371 2024-04-24 17:14:11.083714 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_blueprint_instance_list.py
--rw-r--r--   0        0        0     3274 2024-04-24 17:14:11.087715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_brand_list.py
--rw-r--r--   0        0        0     3331 2024-04-24 17:14:11.091714 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_captcha_stage_list.py
--rw-r--r--   0        0        0     3380 2024-04-24 17:14:11.095715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_certificate_key_pair_list.py
--rw-r--r--   0        0        0     3355 2024-04-24 17:14:11.099715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_connection_token_list.py
--rw-r--r--   0        0        0     3331 2024-04-24 17:14:11.103715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_consent_stage_list.py
--rw-r--r--   0        0        0     3307 2024-04-24 17:14:11.107715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_deny_stage_list.py
--rw-r--r--   0        0        0     3420 2024-04-24 17:14:11.111715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_docker_service_connection_list.py
--rw-r--r--   0        0        0     3282 2024-04-24 17:14:11.115715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_domain_list.py
--rw-r--r--   0        0        0     3323 2024-04-24 17:14:11.119715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_dummy_policy_list.py
--rw-r--r--   0        0        0     3315 2024-04-24 17:14:11.123715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_dummy_stage_list.py
--rw-r--r--   0        0        0     3307 2024-04-24 17:14:11.127715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_duo_device_list.py
--rw-r--r--   0        0        0     3315 2024-04-24 17:14:11.131715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_email_stage_list.py
--rw-r--r--   0        0        0     3298 2024-04-24 17:14:11.135715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_endpoint_list.py
--rw-r--r--   0        0        0     3274 2024-04-24 17:14:11.139715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_event_list.py
--rw-r--r--   0        0        0     3380 2024-04-24 17:14:11.139715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_event_matcher_policy_list.py
--rw-r--r--   0        0        0     3413 2024-04-24 17:14:11.143715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_expiring_base_grant_model_list.py
--rw-r--r--   0        0        0     3363 2024-04-24 17:14:11.147715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_expression_policy_list.py
--rw-r--r--   0        0        0     3437 2024-04-24 17:14:11.151715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_extra_role_object_permission_list.py
--rw-r--r--   0        0        0     3437 2024-04-24 17:14:11.155715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_extra_user_object_permission_list.py
--rw-r--r--   0        0        0     3266 2024-04-24 17:14:11.159715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_flow_list.py
--rw-r--r--   0        0        0     3364 2024-04-24 17:14:11.163715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_flow_stage_binding_list.py
--rw-r--r--   0        0        0     3274 2024-04-24 17:14:11.167715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_group_list.py
--rw-r--r--   0        0        0     3387 2024-04-24 17:14:11.171716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_identification_stage_list.py
--rw-r--r--   0        0        0     3314 2024-04-24 17:14:11.179715 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_invitation_list.py
--rw-r--r--   0        0        0     3355 2024-04-24 17:14:11.183716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_invitation_stage_list.py
--rw-r--r--   0        0        0     3452 2024-04-24 17:14:11.183716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_kubernetes_service_connection_list.py
--rw-r--r--   0        0        0     3372 2024-04-24 17:14:11.187716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_ldap_outpost_config_list.py
--rw-r--r--   0        0        0     3388 2024-04-24 17:14:11.191716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_ldap_property_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-24 17:14:11.195716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_ldap_provider_list.py
--rw-r--r--   0        0        0     3315 2024-04-24 17:14:11.199716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_ldap_source_list.py
--rw-r--r--   0        0        0     3290 2024-04-24 17:14:11.199716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_license_list.py
--rw-r--r--   0        0        0     3330 2024-04-24 17:14:11.203716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_notification_list.py
--rw-r--r--   0        0        0     3363 2024-04-24 17:14:11.207716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_notification_rule_list.py
--rw-r--r--   0        0        0     3403 2024-04-24 17:14:11.211716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_notification_transport_list.py
--rw-r--r--   0        0        0     3444 2024-04-24 17:14:11.215716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_notification_webhook_mapping_list.py
--rw-r--r--   0        0        0     3348 2024-04-24 17:14:11.219716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_o_auth2_provider_list.py
--rw-r--r--   0        0        0     3324 2024-04-24 17:14:11.219716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_o_auth_source_list.py
--rw-r--r--   0        0        0     3290 2024-04-24 17:14:11.223716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_outpost_list.py
--rw-r--r--   0        0        0     3396 2024-04-24 17:14:11.227716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_password_expiry_policy_list.py
--rw-r--r--   0        0        0     3347 2024-04-24 17:14:11.231716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_password_policy_list.py
--rw-r--r--   0        0        0     3339 2024-04-24 17:14:11.235716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_password_stage_list.py
--rw-r--r--   0        0        0     3314 2024-04-24 17:14:11.239716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_permission_list.py
--rw-r--r--   0        0        0     3396 2024-04-24 17:14:11.243716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_plex_source_connection_list.py
--rw-r--r--   0        0        0     3315 2024-04-24 17:14:11.247717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_plex_source_list.py
--rw-r--r--   0        0        0     3339 2024-04-24 17:14:11.251716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_policy_binding_list.py
--rw-r--r--   0        0        0     3282 2024-04-24 17:14:11.255716 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_policy_list.py
--rw-r--r--   0        0        0     3282 2024-04-24 17:14:11.263717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_prompt_list.py
--rw-r--r--   0        0        0     3323 2024-04-24 17:14:11.263717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_prompt_stage_list.py
--rw-r--r--   0        0        0     3355 2024-04-24 17:14:11.267717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_property_mapping_list.py
--rw-r--r--   0        0        0     3298 2024-04-24 17:14:11.271717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_provider_list.py
--rw-r--r--   0        0        0     3380 2024-04-24 17:14:11.275717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_proxy_outpost_config_list.py
--rw-r--r--   0        0        0     3339 2024-04-24 17:14:11.275717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_proxy_provider_list.py
--rw-r--r--   0        0        0     3380 2024-04-24 17:14:11.279717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_rac_property_mapping_list.py
--rw-r--r--   0        0        0     3323 2024-04-24 17:14:11.283717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_rac_provider_list.py
--rw-r--r--   0        0        0     3388 2024-04-24 17:14:11.287717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_radius_outpost_config_list.py
--rw-r--r--   0        0        0     3347 2024-04-24 17:14:11.291717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_radius_provider_list.py
--rw-r--r--   0        0        0     3314 2024-04-24 17:14:11.295717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_reputation_list.py
--rw-r--r--   0        0        0     3363 2024-04-24 17:14:11.299717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_reputation_policy_list.py
--rw-r--r--   0        0        0     3461 2024-04-24 17:14:11.299717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_role_assigned_object_permission_list.py
--rw-r--r--   0        0        0     3266 2024-04-24 17:14:11.303717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_role_list.py
--rw-r--r--   0        0        0     3388 2024-04-24 17:14:11.307717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_saml_property_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-24 17:14:11.311717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_saml_provider_list.py
--rw-r--r--   0        0        0     3315 2024-04-24 17:14:11.315717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_saml_source_list.py
--rw-r--r--   0        0        0     3323 2024-04-24 17:14:11.319717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_scim_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-24 17:14:11.319717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_scim_provider_list.py
--rw-r--r--   0        0        0     3356 2024-04-24 17:14:11.323717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_scim_source_group_list.py
--rw-r--r--   0        0        0     3315 2024-04-24 17:14:11.327717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_scim_source_list.py
--rw-r--r--   0        0        0     3348 2024-04-24 17:14:11.331717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_scim_source_user_list.py
--rw-r--r--   0        0        0     3331 2024-04-24 17:14:11.339717 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_scope_mapping_list.py
--rw-r--r--   0        0        0     3371 2024-04-24 17:14:11.343718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_service_connection_list.py
--rw-r--r--   0        0        0     3307 2024-04-24 17:14:11.335718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_sms_device_list.py
--rw-r--r--   0        0        0     3282 2024-04-24 17:14:11.343718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_source_list.py
--rw-r--r--   0        0        0     3323 2024-04-24 17:14:11.347718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_source_stage_list.py
--rw-r--r--   0        0        0     3274 2024-04-24 17:14:11.351718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_stage_list.py
--rw-r--r--   0        0        0     3331 2024-04-24 17:14:11.355718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_static_device_list.py
--rw-r--r--   0        0        0     3315 2024-04-24 17:14:11.359718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_system_task_list.py
--rw-r--r--   0        0        0     3282 2024-04-24 17:14:11.367718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_tenant_list.py
--rw-r--r--   0        0        0     3274 2024-04-24 17:14:11.367718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_token_list.py
--rw-r--r--   0        0        0     3315 2024-04-24 17:14:11.371718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_token_model_list.py
--rw-r--r--   0        0        0     3315 2024-04-24 17:14:11.363718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_totp_device_list.py
--rw-r--r--   0        0        0     3461 2024-04-24 17:14:11.375718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_user_assigned_object_permission_list.py
--rw-r--r--   0        0        0     3323 2024-04-24 17:14:11.379718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_user_consent_list.py
--rw-r--r--   0        0        0     3356 2024-04-24 17:14:11.383718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_user_delete_stage_list.py
--rw-r--r--   0        0        0     3266 2024-04-24 17:14:11.387718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_user_list.py
--rw-r--r--   0        0        0     3348 2024-04-24 17:14:11.387718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_user_login_stage_list.py
--rw-r--r--   0        0        0     3356 2024-04-24 17:14:11.391718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_user_logout_stage_list.py
--rw-r--r--   0        0        0     3438 2024-04-24 17:14:11.395718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_user_o_auth_source_connection_list.py
--rw-r--r--   0        0        0     3429 2024-04-24 17:14:11.399718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_user_saml_source_connection_list.py
--rw-r--r--   0        0        0     3396 2024-04-24 17:14:11.403718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_user_source_connection_list.py
--rw-r--r--   0        0        0     3348 2024-04-24 17:14:11.407718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_user_write_stage_list.py
--rw-r--r--   0        0        0     3348 2024-04-24 17:14:11.407718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_web_authn_device_list.py
--rw-r--r--   0        0        0     3381 2024-04-24 17:14:11.411718 authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_web_authn_device_type_list.py
--rw-r--r--   0        0        0     3076 2024-04-24 17:14:11.415718 authentik_client-2024.4.0.post1713978839/authentik_client/models/pagination.py
--rw-r--r--   0        0        0     4454 2024-04-24 17:14:11.419719 authentik_client-2024.4.0.post1713978839/authentik_client/models/password_challenge.py
--rw-r--r--   0        0        0     2819 2024-04-24 17:14:11.427719 authentik_client-2024.4.0.post1713978839/authentik_client/models/password_challenge_response_request.py
--rw-r--r--   0        0        0     4377 2024-04-24 17:14:11.427719 authentik_client-2024.4.0.post1713978839/authentik_client/models/password_expiry_policy.py
--rw-r--r--   0        0        0     3099 2024-04-24 17:14:11.431719 authentik_client-2024.4.0.post1713978839/authentik_client/models/password_expiry_policy_request.py
--rw-r--r--   0        0        0     6428 2024-04-24 17:14:11.435719 authentik_client-2024.4.0.post1713978839/authentik_client/models/password_policy.py
--rw-r--r--   0        0        0     5239 2024-04-24 17:14:11.439719 authentik_client-2024.4.0.post1713978839/authentik_client/models/password_policy_request.py
--rw-r--r--   0        0        0     5274 2024-04-24 17:14:11.443719 authentik_client-2024.4.0.post1713978839/authentik_client/models/password_stage.py
--rw-r--r--   0        0        0     4264 2024-04-24 17:14:11.447719 authentik_client-2024.4.0.post1713978839/authentik_client/models/password_stage_request.py
--rw-r--r--   0        0        0     4594 2024-04-24 17:14:11.451719 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_application_request.py
--rw-r--r--   0        0        0     4833 2024-04-24 17:14:11.451719 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_authenticator_duo_stage_request.py
--rw-r--r--   0        0        0     5701 2024-04-24 17:14:11.455719 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_authenticator_sms_stage_request.py
--rw-r--r--   0        0        0     4430 2024-04-24 17:14:11.459719 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_authenticator_static_stage_request.py
--rw-r--r--   0        0        0     4256 2024-04-24 17:14:11.463719 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_authenticator_totp_stage_request.py
--rw-r--r--   0        0        0     4931 2024-04-24 17:14:11.467719 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_authenticator_validate_stage_request.py
--rw-r--r--   0        0        0     5340 2024-04-24 17:14:11.471719 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_authenticator_web_authn_stage_request.py
--rw-r--r--   0        0        0     3246 2024-04-24 17:14:11.475719 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_blueprint_instance_request.py
--rw-r--r--   0        0        0     6352 2024-04-24 17:14:11.475719 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_brand_request.py
--rw-r--r--   0        0        0     3860 2024-04-24 17:14:11.479719 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_captcha_stage_request.py
--rw-r--r--   0        0        0     3051 2024-04-24 17:14:11.483719 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_certificate_key_pair_request.py
--rw-r--r--   0        0        0     2717 2024-04-24 17:14:11.487719 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_connection_token_request.py
--rw-r--r--   0        0        0     3607 2024-04-24 17:14:11.491719 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_consent_stage_request.py
--rw-r--r--   0        0        0     3268 2024-04-24 17:14:11.495720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_deny_stage_request.py
--rw-r--r--   0        0        0     4149 2024-04-24 17:14:11.499719 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_docker_service_connection_request.py
--rw-r--r--   0        0        0     2801 2024-04-24 17:14:11.499719 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_domain_request.py
--rw-r--r--   0        0        0     3275 2024-04-24 17:14:11.503720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_dummy_policy_request.py
--rw-r--r--   0        0        0     3270 2024-04-24 17:14:11.507720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_dummy_stage_request.py
--rw-r--r--   0        0        0     2674 2024-04-24 17:14:11.511720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_duo_device_request.py
--rw-r--r--   0        0        0     5159 2024-04-24 17:14:11.511720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_email_stage_request.py
--rw-r--r--   0        0        0     3784 2024-04-24 17:14:11.515720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_endpoint_request.py
--rw-r--r--   0        0        0     4845 2024-04-24 17:14:11.519720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_event_matcher_policy_request.py
--rw-r--r--   0        0        0     4045 2024-04-24 17:14:11.523720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_event_request.py
--rw-r--r--   0        0        0     3047 2024-04-24 17:14:11.527720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_expression_policy_request.py
--rw-r--r--   0        0        0     4903 2024-04-24 17:14:11.531720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_flow_request.py
--rw-r--r--   0        0        0     4055 2024-04-24 17:14:11.535720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_flow_stage_binding_request.py
--rw-r--r--   0        0        0     3385 2024-04-24 17:14:11.535720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_group_request.py
--rw-r--r--   0        0        0     6571 2024-04-24 17:14:11.539720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_identification_stage_request.py
--rw-r--r--   0        0        0     3985 2024-04-24 17:14:11.543720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_invitation_request.py
--rw-r--r--   0        0        0     3565 2024-04-24 17:14:11.547720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_invitation_stage_request.py
--rw-r--r--   0        0        0     3492 2024-04-24 17:14:11.551720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_kubernetes_service_connection_request.py
--rw-r--r--   0        0        0     3550 2024-04-24 17:14:11.555720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_ldap_property_mapping_request.py
--rw-r--r--   0        0        0     6254 2024-04-24 17:14:11.559720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_ldap_provider_request.py
--rw-r--r--   0        0        0     9697 2024-04-24 17:14:11.563720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_ldap_source_request.py
--rw-r--r--   0        0        0     2557 2024-04-24 17:14:11.563720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_license_request.py
--rw-r--r--   0        0        0     2879 2024-04-24 17:14:11.567720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_notification_request.py
--rw-r--r--   0        0        0     3587 2024-04-24 17:14:11.567720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_notification_rule_request.py
--rw-r--r--   0        0        0     3538 2024-04-24 17:14:11.571720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_notification_transport_request.py
--rw-r--r--   0        0        0     2782 2024-04-24 17:14:11.575720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_notification_webhook_mapping_request.py
--rw-r--r--   0        0        0     6716 2024-04-24 17:14:11.575720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_o_auth2_provider_request.py
--rw-r--r--   0        0        0     8185 2024-04-24 17:14:11.579721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_o_auth_source_request.py
--rw-r--r--   0        0        0     4139 2024-04-24 17:14:11.579721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_outpost_request.py
--rw-r--r--   0        0        0     3154 2024-04-24 17:14:11.583721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_password_expiry_policy_request.py
--rw-r--r--   0        0        0     5277 2024-04-24 17:14:11.587720 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_password_policy_request.py
--rw-r--r--   0        0        0     4326 2024-04-24 17:14:11.591721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_password_stage_request.py
--rw-r--r--   0        0        0     2922 2024-04-24 17:14:11.595721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_permission_assign_request.py
--rw-r--r--   0        0        0     2784 2024-04-24 17:14:11.599721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_plex_source_connection_request.py
--rw-r--r--   0        0        0     5905 2024-04-24 17:14:11.603721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_plex_source_request.py
--rw-r--r--   0        0        0     4286 2024-04-24 17:14:11.603721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_policy_binding_request.py
--rw-r--r--   0        0        0     5023 2024-04-24 17:14:11.607721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_prompt_request.py
--rw-r--r--   0        0        0     3406 2024-04-24 17:14:11.611721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_prompt_stage_request.py
--rw-r--r--   0        0        0     6907 2024-04-24 17:14:11.615721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_proxy_provider_request.py
--rw-r--r--   0        0        0     3495 2024-04-24 17:14:11.619721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_rac_property_mapping_request.py
--rw-r--r--   0        0        0     4413 2024-04-24 17:14:11.623721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_rac_provider_request.py
--rw-r--r--   0        0        0     4563 2024-04-24 17:14:11.627721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_radius_provider_request.py
--rw-r--r--   0        0        0     3276 2024-04-24 17:14:11.627721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_reputation_policy_request.py
--rw-r--r--   0        0        0     2565 2024-04-24 17:14:11.631721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_role_request.py
--rw-r--r--   0        0        0     3901 2024-04-24 17:14:11.635721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_saml_property_mapping_request.py
--rw-r--r--   0        0        0     7539 2024-04-24 17:14:11.639721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_saml_provider_request.py
--rw-r--r--   0        0        0     8676 2024-04-24 17:14:11.639721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_saml_source_request.py
--rw-r--r--   0        0        0     3364 2024-04-24 17:14:11.643721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_scim_mapping_request.py
--rw-r--r--   0        0        0     3888 2024-04-24 17:14:11.647721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_scim_provider_request.py
--rw-r--r--   0        0        0     3095 2024-04-24 17:14:11.647721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_scim_source_group_request.py
--rw-r--r--   0        0        0     3829 2024-04-24 17:14:11.651721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_scim_source_request.py
--rw-r--r--   0        0        0     3098 2024-04-24 17:14:11.651721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_scim_source_user_request.py
--rw-r--r--   0        0        0     3819 2024-04-24 17:14:11.659721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_scope_mapping_request.py
--rw-r--r--   0        0        0     5079 2024-04-24 17:14:11.663721 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_settings_request.py
--rw-r--r--   0        0        0     2674 2024-04-24 17:14:11.655722 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_sms_device_request.py
--rw-r--r--   0        0        0     3562 2024-04-24 17:14:11.667722 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_source_stage_request.py
--rw-r--r--   0        0        0     2686 2024-04-24 17:14:11.667722 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_static_device_request.py
--rw-r--r--   0        0        0     2820 2024-04-24 17:14:11.675722 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_tenant_request.py
--rw-r--r--   0        0        0     4419 2024-04-24 17:14:11.679722 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_token_request.py
--rw-r--r--   0        0        0     2678 2024-04-24 17:14:11.671722 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_totp_device_request.py
--rw-r--r--   0        0        0     3167 2024-04-24 17:14:11.683722 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_user_delete_stage_request.py
--rw-r--r--   0        0        0     4766 2024-04-24 17:14:11.687722 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_user_login_stage_request.py
--rw-r--r--   0        0        0     3167 2024-04-24 17:14:11.687722 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_user_logout_stage_request.py
--rw-r--r--   0        0        0     3109 2024-04-24 17:14:11.691722 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_user_o_auth_source_connection_request.py
--rw-r--r--   0        0        0     3934 2024-04-24 17:14:11.691722 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_user_request.py
--rw-r--r--   0        0        0     2733 2024-04-24 17:14:11.695722 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_user_saml_source_connection_request.py
--rw-r--r--   0        0        0     4450 2024-04-24 17:14:11.699722 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_user_write_stage_request.py
--rw-r--r--   0        0        0     2625 2024-04-24 17:14:11.703722 authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_web_authn_device_request.py
--rw-r--r--   0        0        0     3548 2024-04-24 17:14:11.703722 authentik_client-2024.4.0.post1713978839/authentik_client/models/permission.py
--rw-r--r--   0        0        0     2884 2024-04-24 17:14:11.711722 authentik_client-2024.4.0.post1713978839/authentik_client/models/permission_assign_request.py
--rw-r--r--   0        0        0     4315 2024-04-24 17:14:11.711722 authentik_client-2024.4.0.post1713978839/authentik_client/models/plex_authentication_challenge.py
--rw-r--r--   0        0        0     2726 2024-04-24 17:14:11.715722 authentik_client-2024.4.0.post1713978839/authentik_client/models/plex_authentication_challenge_response_request.py
--rw-r--r--   0        0        0     7752 2024-04-24 17:14:11.719722 authentik_client-2024.4.0.post1713978839/authentik_client/models/plex_source.py
--rw-r--r--   0        0        0     3265 2024-04-24 17:14:11.719722 authentik_client-2024.4.0.post1713978839/authentik_client/models/plex_source_connection.py
--rw-r--r--   0        0        0     2719 2024-04-24 17:14:11.723722 authentik_client-2024.4.0.post1713978839/authentik_client/models/plex_source_connection_request.py
--rw-r--r--   0        0        0     5760 2024-04-24 17:14:11.727722 authentik_client-2024.4.0.post1713978839/authentik_client/models/plex_source_request.py
--rw-r--r--   0        0        0     2576 2024-04-24 17:14:11.727722 authentik_client-2024.4.0.post1713978839/authentik_client/models/plex_token_redeem_request.py
--rw-r--r--   0        0        0     4055 2024-04-24 17:14:11.731722 authentik_client-2024.4.0.post1713978839/authentik_client/models/policy.py
--rw-r--r--   0        0        0     5643 2024-04-24 17:14:11.735722 authentik_client-2024.4.0.post1713978839/authentik_client/models/policy_binding.py
--rw-r--r--   0        0        0     4231 2024-04-24 17:14:11.735722 authentik_client-2024.4.0.post1713978839/authentik_client/models/policy_binding_request.py
--rw-r--r--   0        0        0      711 2024-04-24 17:14:11.739722 authentik_client-2024.4.0.post1713978839/authentik_client/models/policy_engine_mode.py
--rw-r--r--   0        0        0     2817 2024-04-24 17:14:11.739722 authentik_client-2024.4.0.post1713978839/authentik_client/models/policy_request.py
--rw-r--r--   0        0        0     2583 2024-04-24 17:14:11.743723 authentik_client-2024.4.0.post1713978839/authentik_client/models/policy_test_request.py
--rw-r--r--   0        0        0     3281 2024-04-24 17:14:11.747722 authentik_client-2024.4.0.post1713978839/authentik_client/models/policy_test_result.py
--rw-r--r--   0        0        0     4885 2024-04-24 17:14:11.747722 authentik_client-2024.4.0.post1713978839/authentik_client/models/prompt.py
--rw-r--r--   0        0        0     4649 2024-04-24 17:14:11.751723 authentik_client-2024.4.0.post1713978839/authentik_client/models/prompt_challenge.py
--rw-r--r--   0        0        0     3325 2024-04-24 17:14:11.755723 authentik_client-2024.4.0.post1713978839/authentik_client/models/prompt_challenge_response_request.py
--rw-r--r--   0        0        0     4927 2024-04-24 17:14:11.755723 authentik_client-2024.4.0.post1713978839/authentik_client/models/prompt_request.py
--rw-r--r--   0        0        0     4321 2024-04-24 17:14:11.759723 authentik_client-2024.4.0.post1713978839/authentik_client/models/prompt_stage.py
--rw-r--r--   0        0        0     3351 2024-04-24 17:14:11.763723 authentik_client-2024.4.0.post1713978839/authentik_client/models/prompt_stage_request.py
--rw-r--r--   0        0        0     1185 2024-04-24 17:14:11.763723 authentik_client-2024.4.0.post1713978839/authentik_client/models/prompt_type_enum.py
--rw-r--r--   0        0        0     4264 2024-04-24 17:14:11.767723 authentik_client-2024.4.0.post1713978839/authentik_client/models/property_mapping.py
--rw-r--r--   0        0        0     2610 2024-04-24 17:14:11.767723 authentik_client-2024.4.0.post1713978839/authentik_client/models/property_mapping_preview.py
--rw-r--r--   0        0        0     2744 2024-04-24 17:14:11.771723 authentik_client-2024.4.0.post1713978839/authentik_client/models/property_mapping_test_result.py
--rw-r--r--   0        0        0      715 2024-04-24 17:14:11.771723 authentik_client-2024.4.0.post1713978839/authentik_client/models/protocol_enum.py
--rw-r--r--   0        0        0     5722 2024-04-24 17:14:11.775723 authentik_client-2024.4.0.post1713978839/authentik_client/models/provider.py
--rw-r--r--   0        0        0      713 2024-04-24 17:14:11.775723 authentik_client-2024.4.0.post1713978839/authentik_client/models/provider_enum.py
--rw-r--r--   0        0        0     1314 2024-04-24 17:14:11.779723 authentik_client-2024.4.0.post1713978839/authentik_client/models/provider_model_enum.py
--rw-r--r--   0        0        0     3397 2024-04-24 17:14:11.783723 authentik_client-2024.4.0.post1713978839/authentik_client/models/provider_request.py
--rw-r--r--   0        0        0     1009 2024-04-24 17:14:11.783723 authentik_client-2024.4.0.post1713978839/authentik_client/models/provider_type_enum.py
--rw-r--r--   0        0        0      754 2024-04-24 17:14:11.783723 authentik_client-2024.4.0.post1713978839/authentik_client/models/proxy_mode.py
--rw-r--r--   0        0        0     7819 2024-04-24 17:14:11.787723 authentik_client-2024.4.0.post1713978839/authentik_client/models/proxy_outpost_config.py
--rw-r--r--   0        0        0     9552 2024-04-24 17:14:11.787723 authentik_client-2024.4.0.post1713978839/authentik_client/models/proxy_provider.py
--rw-r--r--   0        0        0     6828 2024-04-24 17:14:11.791723 authentik_client-2024.4.0.post1713978839/authentik_client/models/proxy_provider_request.py
--rw-r--r--   0        0        0     4407 2024-04-24 17:14:11.795723 authentik_client-2024.4.0.post1713978839/authentik_client/models/rac_property_mapping.py
--rw-r--r--   0        0        0     3440 2024-04-24 17:14:11.795723 authentik_client-2024.4.0.post1713978839/authentik_client/models/rac_property_mapping_request.py
--rw-r--r--   0        0        0     6813 2024-04-24 17:14:11.799723 authentik_client-2024.4.0.post1713978839/authentik_client/models/rac_provider.py
--rw-r--r--   0        0        0     4351 2024-04-24 17:14:11.803723 authentik_client-2024.4.0.post1713978839/authentik_client/models/rac_provider_request.py
--rw-r--r--   0        0        0     3833 2024-04-24 17:14:11.803723 authentik_client-2024.4.0.post1713978839/authentik_client/models/radius_outpost_config.py
--rw-r--r--   0        0        0     6924 2024-04-24 17:14:11.807723 authentik_client-2024.4.0.post1713978839/authentik_client/models/radius_provider.py
--rw-r--r--   0        0        0     4501 2024-04-24 17:14:11.807723 authentik_client-2024.4.0.post1713978839/authentik_client/models/radius_provider_request.py
--rw-r--r--   0        0        0     4184 2024-04-24 17:14:11.811723 authentik_client-2024.4.0.post1713978839/authentik_client/models/redirect_challenge.py
--rw-r--r--   0        0        0     3642 2024-04-24 17:14:11.815723 authentik_client-2024.4.0.post1713978839/authentik_client/models/reputation.py
--rw-r--r--   0        0        0     4516 2024-04-24 17:14:11.815723 authentik_client-2024.4.0.post1713978839/authentik_client/models/reputation_policy.py
--rw-r--r--   0        0        0     3238 2024-04-24 17:14:11.819723 authentik_client-2024.4.0.post1713978839/authentik_client/models/reputation_policy_request.py
--rw-r--r--   0        0        0      795 2024-04-24 17:14:11.819723 authentik_client-2024.4.0.post1713978839/authentik_client/models/resident_key_requirement_enum.py
--rw-r--r--   0        0        0     2618 2024-04-24 17:14:11.823723 authentik_client-2024.4.0.post1713978839/authentik_client/models/role.py
--rw-r--r--   0        0        0     3333 2024-04-24 17:14:11.823723 authentik_client-2024.4.0.post1713978839/authentik_client/models/role_assigned_object_permission.py
--rw-r--r--   0        0        0     3293 2024-04-24 17:14:11.827724 authentik_client-2024.4.0.post1713978839/authentik_client/models/role_object_permission.py
--rw-r--r--   0        0        0     2517 2024-04-24 17:14:11.827724 authentik_client-2024.4.0.post1713978839/authentik_client/models/role_request.py
--rw-r--r--   0        0        0     2712 2024-04-24 17:14:11.831724 authentik_client-2024.4.0.post1713978839/authentik_client/models/saml_metadata.py
--rw-r--r--   0        0        0     4718 2024-04-24 17:14:11.835724 authentik_client-2024.4.0.post1713978839/authentik_client/models/saml_property_mapping.py
--rw-r--r--   0        0        0     3829 2024-04-24 17:14:11.835724 authentik_client-2024.4.0.post1713978839/authentik_client/models/saml_property_mapping_request.py
--rw-r--r--   0        0        0    11056 2024-04-24 17:14:11.839724 authentik_client-2024.4.0.post1713978839/authentik_client/models/saml_provider.py
--rw-r--r--   0        0        0     7460 2024-04-24 17:14:11.843724 authentik_client-2024.4.0.post1713978839/authentik_client/models/saml_provider_request.py
--rw-r--r--   0        0        0    10563 2024-04-24 17:14:11.843724 authentik_client-2024.4.0.post1713978839/authentik_client/models/saml_source.py
--rw-r--r--   0        0        0     8507 2024-04-24 17:14:11.847724 authentik_client-2024.4.0.post1713978839/authentik_client/models/saml_source_request.py
--rw-r--r--   0        0        0     4248 2024-04-24 17:14:11.851724 authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_mapping.py
--rw-r--r--   0        0        0     3309 2024-04-24 17:14:11.851724 authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_mapping_request.py
--rw-r--r--   0        0        0     5454 2024-04-24 17:14:11.855724 authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_provider.py
--rw-r--r--   0        0        0     3802 2024-04-24 17:14:11.859724 authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_provider_request.py
--rw-r--r--   0        0        0     5999 2024-04-24 17:14:11.859724 authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_source.py
--rw-r--r--   0        0        0     3369 2024-04-24 17:14:11.863724 authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_source_group.py
--rw-r--r--   0        0        0     3023 2024-04-24 17:14:11.867724 authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_source_group_request.py
--rw-r--r--   0        0        0     3708 2024-04-24 17:14:11.867724 authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_source_request.py
--rw-r--r--   0        0        0     3370 2024-04-24 17:14:11.871724 authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_source_user.py
--rw-r--r--   0        0        0     3026 2024-04-24 17:14:11.871724 authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_source_user_request.py
--rw-r--r--   0        0        0     3131 2024-04-24 17:14:11.875724 authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_sync_status.py
--rw-r--r--   0        0        0     4629 2024-04-24 17:14:11.883724 authentik_client-2024.4.0.post1713978839/authentik_client/models/scope_mapping.py
--rw-r--r--   0        0        0     3740 2024-04-24 17:14:11.883724 authentik_client-2024.4.0.post1713978839/authentik_client/models/scope_mapping_request.py
--rw-r--r--   0        0        0     2738 2024-04-24 17:14:11.887724 authentik_client-2024.4.0.post1713978839/authentik_client/models/selectable_stage.py
--rw-r--r--   0        0        0     3773 2024-04-24 17:14:11.887724 authentik_client-2024.4.0.post1713978839/authentik_client/models/service_connection.py
--rw-r--r--   0        0        0     2776 2024-04-24 17:14:11.891724 authentik_client-2024.4.0.post1713978839/authentik_client/models/service_connection_request.py
--rw-r--r--   0        0        0     2731 2024-04-24 17:14:11.891724 authentik_client-2024.4.0.post1713978839/authentik_client/models/service_connection_state.py
--rw-r--r--   0        0        0     3178 2024-04-24 17:14:11.895724 authentik_client-2024.4.0.post1713978839/authentik_client/models/session_user.py
--rw-r--r--   0        0        0     4931 2024-04-24 17:14:11.895724 authentik_client-2024.4.0.post1713978839/authentik_client/models/settings.py
--rw-r--r--   0        0        0     5058 2024-04-24 17:14:11.899724 authentik_client-2024.4.0.post1713978839/authentik_client/models/settings_request.py
--rw-r--r--   0        0        0      733 2024-04-24 17:14:11.899724 authentik_client-2024.4.0.post1713978839/authentik_client/models/severity_enum.py
--rw-r--r--   0        0        0     4175 2024-04-24 17:14:11.899724 authentik_client-2024.4.0.post1713978839/authentik_client/models/shell_challenge.py
--rw-r--r--   0        0        0     1492 2024-04-24 17:14:11.903725 authentik_client-2024.4.0.post1713978839/authentik_client/models/signature_algorithm_enum.py
--rw-r--r--   0        0        0     2906 2024-04-24 17:14:11.879724 authentik_client-2024.4.0.post1713978839/authentik_client/models/sms_device.py
--rw-r--r--   0        0        0     2619 2024-04-24 17:14:11.879724 authentik_client-2024.4.0.post1713978839/authentik_client/models/sms_device_request.py
--rw-r--r--   0        0        0     6945 2024-04-24 17:14:11.903725 authentik_client-2024.4.0.post1713978839/authentik_client/models/source.py
--rw-r--r--   0        0        0     4836 2024-04-24 17:14:11.907724 authentik_client-2024.4.0.post1713978839/authentik_client/models/source_request.py
--rw-r--r--   0        0        0     4438 2024-04-24 17:14:11.907724 authentik_client-2024.4.0.post1713978839/authentik_client/models/source_stage.py
--rw-r--r--   0        0        0     3507 2024-04-24 17:14:11.911725 authentik_client-2024.4.0.post1713978839/authentik_client/models/source_stage_request.py
--rw-r--r--   0        0        0     5355 2024-04-24 17:14:11.911725 authentik_client-2024.4.0.post1713978839/authentik_client/models/source_type.py
--rw-r--r--   0        0        0      714 2024-04-24 17:14:11.915725 authentik_client-2024.4.0.post1713978839/authentik_client/models/sp_binding_enum.py
--rw-r--r--   0        0        0     4070 2024-04-24 17:14:11.915725 authentik_client-2024.4.0.post1713978839/authentik_client/models/stage.py
--rw-r--r--   0        0        0     3437 2024-04-24 17:14:11.919725 authentik_client-2024.4.0.post1713978839/authentik_client/models/stage_prompt.py
--rw-r--r--   0        0        0     3089 2024-04-24 17:14:11.919725 authentik_client-2024.4.0.post1713978839/authentik_client/models/stage_request.py
--rw-r--r--   0        0        0     3385 2024-04-24 17:14:11.923725 authentik_client-2024.4.0.post1713978839/authentik_client/models/static_device.py
--rw-r--r--   0        0        0     2631 2024-04-24 17:14:11.923725 authentik_client-2024.4.0.post1713978839/authentik_client/models/static_device_request.py
--rw-r--r--   0        0        0     2546 2024-04-24 17:14:11.923725 authentik_client-2024.4.0.post1713978839/authentik_client/models/static_device_token.py
--rw-r--r--   0        0        0     2581 2024-04-24 17:14:11.927725 authentik_client-2024.4.0.post1713978839/authentik_client/models/static_device_token_request.py
--rw-r--r--   0        0        0      846 2024-04-24 17:14:11.927725 authentik_client-2024.4.0.post1713978839/authentik_client/models/sub_mode_enum.py
--rw-r--r--   0        0        0     4463 2024-04-24 17:14:11.931725 authentik_client-2024.4.0.post1713978839/authentik_client/models/system_info.py
--rw-r--r--   0        0        0     2934 2024-04-24 17:14:11.931725 authentik_client-2024.4.0.post1713978839/authentik_client/models/system_info_runtime.py
--rw-r--r--   0        0        0     4286 2024-04-24 17:14:11.935725 authentik_client-2024.4.0.post1713978839/authentik_client/models/system_task.py
--rw-r--r--   0        0        0      789 2024-04-24 17:14:11.935725 authentik_client-2024.4.0.post1713978839/authentik_client/models/system_task_status_enum.py
--rw-r--r--   0        0        0     2872 2024-04-24 17:14:11.947725 authentik_client-2024.4.0.post1713978839/authentik_client/models/tenant.py
--rw-r--r--   0        0        0     2589 2024-04-24 17:14:11.947725 authentik_client-2024.4.0.post1713978839/authentik_client/models/tenant_admin_group_request_request.py
--rw-r--r--   0        0        0     2705 2024-04-24 17:14:11.951725 authentik_client-2024.4.0.post1713978839/authentik_client/models/tenant_recovery_key_request_request.py
--rw-r--r--   0        0        0     2599 2024-04-24 17:14:11.951725 authentik_client-2024.4.0.post1713978839/authentik_client/models/tenant_recovery_key_response.py
--rw-r--r--   0        0        0     2765 2024-04-24 17:14:11.955725 authentik_client-2024.4.0.post1713978839/authentik_client/models/tenant_request.py
--rw-r--r--   0        0        0     4802 2024-04-24 17:14:11.955725 authentik_client-2024.4.0.post1713978839/authentik_client/models/token.py
--rw-r--r--   0        0        0     4198 2024-04-24 17:14:11.959725 authentik_client-2024.4.0.post1713978839/authentik_client/models/token_model.py
--rw-r--r--   0        0        0     4329 2024-04-24 17:14:11.963725 authentik_client-2024.4.0.post1713978839/authentik_client/models/token_request.py
--rw-r--r--   0        0        0     2521 2024-04-24 17:14:11.963725 authentik_client-2024.4.0.post1713978839/authentik_client/models/token_set_key_request.py
--rw-r--r--   0        0        0     2494 2024-04-24 17:14:11.967725 authentik_client-2024.4.0.post1713978839/authentik_client/models/token_view.py
--rw-r--r--   0        0        0     2724 2024-04-24 17:14:11.939725 authentik_client-2024.4.0.post1713978839/authentik_client/models/totp_device.py
--rw-r--r--   0        0        0     2623 2024-04-24 17:14:11.939725 authentik_client-2024.4.0.post1713978839/authentik_client/models/totp_device_request.py
--rw-r--r--   0        0        0     3389 2024-04-24 17:14:11.967725 authentik_client-2024.4.0.post1713978839/authentik_client/models/transaction_application_request.py
--rw-r--r--   0        0        0     2595 2024-04-24 17:14:11.971725 authentik_client-2024.4.0.post1713978839/authentik_client/models/transaction_application_response.py
--rw-r--r--   0        0        0     2936 2024-04-24 17:14:11.971725 authentik_client-2024.4.0.post1713978839/authentik_client/models/type_create.py
--rw-r--r--   0        0        0      730 2024-04-24 17:14:11.975725 authentik_client-2024.4.0.post1713978839/authentik_client/models/ui_theme_enum.py
--rw-r--r--   0        0        0     2808 2024-04-24 17:14:11.975725 authentik_client-2024.4.0.post1713978839/authentik_client/models/used_by.py
--rw-r--r--   0        0        0      795 2024-04-24 17:14:11.979725 authentik_client-2024.4.0.post1713978839/authentik_client/models/used_by_action_enum.py
--rw-r--r--   0        0        0     5459 2024-04-24 17:14:11.979725 authentik_client-2024.4.0.post1713978839/authentik_client/models/user.py
--rw-r--r--   0        0        0     2458 2024-04-24 17:14:11.983725 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_account_request.py
--rw-r--r--   0        0        0     4946 2024-04-24 17:14:11.987726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_assigned_object_permission.py
--rw-r--r--   0        0        0     3828 2024-04-24 17:14:11.991726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_consent.py
--rw-r--r--   0        0        0      811 2024-04-24 17:14:11.991726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_creation_mode_enum.py
--rw-r--r--   0        0        0     4110 2024-04-24 17:14:11.995725 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_delete_stage.py
--rw-r--r--   0        0        0     3129 2024-04-24 17:14:11.999726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_delete_stage_request.py
--rw-r--r--   0        0        0      735 2024-04-24 17:14:11.999726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_fields_enum.py
--rw-r--r--   0        0        0     3909 2024-04-24 17:14:12.003726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_group.py
--rw-r--r--   0        0        0     3193 2024-04-24 17:14:12.007726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_group_request.py
--rw-r--r--   0        0        0     4334 2024-04-24 17:14:12.011726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_login_challenge.py
--rw-r--r--   0        0        0     2805 2024-04-24 17:14:12.015726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_login_challenge_response_request.py
--rw-r--r--   0        0        0     5631 2024-04-24 17:14:12.015726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_login_stage.py
--rw-r--r--   0        0        0     4728 2024-04-24 17:14:12.019726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_login_stage_request.py
--rw-r--r--   0        0        0     4110 2024-04-24 17:14:12.023726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_logout_stage.py
--rw-r--r--   0        0        0     3129 2024-04-24 17:14:12.027726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_logout_stage_request.py
--rw-r--r--   0        0        0      853 2024-04-24 17:14:12.027726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_matching_mode_enum.py
--rw-r--r--   0        0        0     4160 2024-04-24 17:14:12.031726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_metrics.py
--rw-r--r--   0        0        0     3188 2024-04-24 17:14:12.035726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_o_auth_source_connection.py
--rw-r--r--   0        0        0     3054 2024-04-24 17:14:12.039726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_o_auth_source_connection_request.py
--rw-r--r--   0        0        0     3293 2024-04-24 17:14:12.039726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_object_permission.py
--rw-r--r--   0        0        0     2557 2024-04-24 17:14:12.043726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_password_set_request.py
--rw-r--r--   0        0        0     2491 2024-04-24 17:14:12.047726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_path.py
--rw-r--r--   0        0        0     3872 2024-04-24 17:14:12.051726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_request.py
--rw-r--r--   0        0        0     3107 2024-04-24 17:14:12.051726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_saml_source_connection.py
--rw-r--r--   0        0        0     2668 2024-04-24 17:14:12.055726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_saml_source_connection_request.py
--rw-r--r--   0        0        0     5465 2024-04-24 17:14:12.059726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_self.py
--rw-r--r--   0        0        0     2629 2024-04-24 17:14:12.059726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_self_groups.py
--rw-r--r--   0        0        0     3074 2024-04-24 17:14:12.059726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_service_account_request.py
--rw-r--r--   0        0        0     2844 2024-04-24 17:14:12.063727 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_service_account_response.py
--rw-r--r--   0        0        0     2866 2024-04-24 17:14:12.063727 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_setting.py
--rw-r--r--   0        0        0     3245 2024-04-24 17:14:12.067726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_source_connection.py
--rw-r--r--   0        0        0      817 2024-04-24 17:14:12.067726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_type_enum.py
--rw-r--r--   0        0        0      777 2024-04-24 17:14:12.067726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_verification_enum.py
--rw-r--r--   0        0        0     5382 2024-04-24 17:14:12.071726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_write_stage.py
--rw-r--r--   0        0        0     4412 2024-04-24 17:14:12.071726 authentik_client-2024.4.0.post1713978839/authentik_client/models/user_write_stage_request.py
--rw-r--r--   0        0        0     3197 2024-04-24 17:14:12.075727 authentik_client-2024.4.0.post1713978839/authentik_client/models/validation_error.py
--rw-r--r--   0        0        0     3589 2024-04-24 17:14:12.075727 authentik_client-2024.4.0.post1713978839/authentik_client/models/version.py
--rw-r--r--   0        0        0     3786 2024-04-24 17:14:12.075727 authentik_client-2024.4.0.post1713978839/authentik_client/models/web_authn_device.py
--rw-r--r--   0        0        0     2577 2024-04-24 17:14:12.079727 authentik_client-2024.4.0.post1713978839/authentik_client/models/web_authn_device_request.py
--rw-r--r--   0        0        0     2562 2024-04-24 17:14:12.079727 authentik_client-2024.4.0.post1713978839/authentik_client/models/web_authn_device_type.py
--rw-r--r--   0        0        0     2669 2024-04-24 17:14:12.083727 authentik_client-2024.4.0.post1713978839/authentik_client/models/web_authn_device_type_request.py
--rw-r--r--   0        0        0     2410 2024-04-24 17:14:12.083727 authentik_client-2024.4.0.post1713978839/authentik_client/models/workers.py
--rw-r--r--   0        0        0        0 2024-04-24 17:14:13.271741 authentik_client-2024.4.0.post1713978839/authentik_client/py.typed
--rw-r--r--   0        0        0     9196 2024-04-24 17:14:13.287742 authentik_client-2024.4.0.post1713978839/authentik_client/rest.py
--rw-r--r--   0        0        0     1936 2024-04-24 17:14:13.271741 authentik_client-2024.4.0.post1713978839/pyproject.toml
--rw-r--r--   0        0        0   144895 1970-01-01 00:00:00.000000 authentik_client-2024.4.0.post1713978839/PKG-INFO
+-rw-r--r--   0        0        0   143943 2024-04-26 16:44:55.750353 authentik_client-2024.4.1.post1714149882/README.md
+-rw-r--r--   0        0        0    48482 2024-04-26 16:44:55.758353 authentik_client-2024.4.1.post1714149882/authentik_client/__init__.py
+-rw-r--r--   0        0        0     1170 2024-04-26 16:44:55.762353 authentik_client-2024.4.1.post1714149882/authentik_client/api/__init__.py
+-rw-r--r--   0        0        0    97518 2024-04-26 16:44:55.434354 authentik_client-2024.4.1.post1714149882/authentik_client/api/admin_api.py
+-rw-r--r--   0        0        0   700271 2024-04-26 16:44:55.466354 authentik_client-2024.4.1.post1714149882/authentik_client/api/authenticators_api.py
+-rw-r--r--   0        0        0   701197 2024-04-26 16:44:55.494354 authentik_client-2024.4.1.post1714149882/authentik_client/api/core_api.py
+-rw-r--r--   0        0        0   116805 2024-04-26 16:44:55.506354 authentik_client-2024.4.1.post1714149882/authentik_client/api/crypto_api.py
+-rw-r--r--   0        0        0   107946 2024-04-26 16:44:55.518354 authentik_client-2024.4.1.post1714149882/authentik_client/api/enterprise_api.py
+-rw-r--r--   0        0        0   408008 2024-04-26 16:44:55.530354 authentik_client-2024.4.1.post1714149882/authentik_client/api/events_api.py
+-rw-r--r--   0        0        0   280806 2024-04-26 16:44:55.546354 authentik_client-2024.4.1.post1714149882/authentik_client/api/flows_api.py
+-rw-r--r--   0        0        0   101134 2024-04-26 16:44:55.558354 authentik_client-2024.4.1.post1714149882/authentik_client/api/managed_api.py
+-rw-r--r--   0        0        0   135649 2024-04-26 16:44:55.566354 authentik_client-2024.4.1.post1714149882/authentik_client/api/oauth2_api.py
+-rw-r--r--   0        0        0   413301 2024-04-26 16:44:55.578354 authentik_client-2024.4.1.post1714149882/authentik_client/api/outposts_api.py
+-rw-r--r--   0        0        0   725201 2024-04-26 16:44:55.598354 authentik_client-2024.4.1.post1714149882/authentik_client/api/policies_api.py
+-rw-r--r--   0        0        0   552586 2024-04-26 16:44:55.614354 authentik_client-2024.4.1.post1714149882/authentik_client/api/propertymappings_api.py
+-rw-r--r--   0        0        0   718066 2024-04-26 16:44:55.634354 authentik_client-2024.4.1.post1714149882/authentik_client/api/providers_api.py
+-rw-r--r--   0        0        0   150485 2024-04-26 16:44:55.646354 authentik_client-2024.4.1.post1714149882/authentik_client/api/rac_api.py
+-rw-r--r--   0        0        0   207550 2024-04-26 16:44:55.658354 authentik_client-2024.4.1.post1714149882/authentik_client/api/rbac_api.py
+-rw-r--r--   0        0        0    10391 2024-04-26 16:44:55.662354 authentik_client-2024.4.1.post1714149882/authentik_client/api/root_api.py
+-rw-r--r--   0        0        0    11845 2024-04-26 16:44:55.670354 authentik_client-2024.4.1.post1714149882/authentik_client/api/schema_api.py
+-rw-r--r--   0        0        0  1037225 2024-04-26 16:44:55.690353 authentik_client-2024.4.1.post1714149882/authentik_client/api/sources_api.py
+-rw-r--r--   0        0        0  1945986 2024-04-26 16:44:55.726354 authentik_client-2024.4.1.post1714149882/authentik_client/api/stages_api.py
+-rw-r--r--   0        0        0   157909 2024-04-26 16:44:55.742353 authentik_client-2024.4.1.post1714149882/authentik_client/api/tenants_api.py
+-rw-r--r--   0        0        0    25779 2024-04-26 16:44:55.766353 authentik_client-2024.4.1.post1714149882/authentik_client/api_client.py
+-rw-r--r--   0        0        0      652 2024-04-26 16:44:55.766353 authentik_client-2024.4.1.post1714149882/authentik_client/api_response.py
+-rw-r--r--   0        0        0    14724 2024-04-26 16:44:55.758353 authentik_client-2024.4.1.post1714149882/authentik_client/configuration.py
+-rw-r--r--   0        0        0     5934 2024-04-26 16:44:55.762353 authentik_client-2024.4.1.post1714149882/authentik_client/exceptions.py
+-rw-r--r--   0        0        0    46784 2024-04-26 16:44:55.762353 authentik_client-2024.4.1.post1714149882/authentik_client/models/__init__.py
+-rw-r--r--   0        0        0     4513 2024-04-26 16:44:52.750361 authentik_client-2024.4.1.post1714149882/authentik_client/models/access_denied_challenge.py
+-rw-r--r--   0        0        0     2482 2024-04-26 16:44:52.762361 authentik_client-2024.4.1.post1714149882/authentik_client/models/app.py
+-rw-r--r--   0        0        0     4230 2024-04-26 16:44:52.770361 authentik_client-2024.4.1.post1714149882/authentik_client/models/app_enum.py
+-rw-r--r--   0        0        0     2702 2024-04-26 16:44:52.778361 authentik_client-2024.4.1.post1714149882/authentik_client/models/apple_challenge_response_request.py
+-rw-r--r--   0        0        0     4508 2024-04-26 16:44:52.790361 authentik_client-2024.4.1.post1714149882/authentik_client/models/apple_login_challenge.py
+-rw-r--r--   0        0        0     6686 2024-04-26 16:44:52.802361 authentik_client-2024.4.1.post1714149882/authentik_client/models/application.py
+-rw-r--r--   0        0        0     4473 2024-04-26 16:44:52.810361 authentik_client-2024.4.1.post1714149882/authentik_client/models/application_request.py
+-rw-r--r--   0        0        0      711 2024-04-26 16:44:52.814361 authentik_client-2024.4.1.post1714149882/authentik_client/models/auth_mode_enum.py
+-rw-r--r--   0        0        0      709 2024-04-26 16:44:52.818361 authentik_client-2024.4.1.post1714149882/authentik_client/models/auth_type_enum.py
+-rw-r--r--   0        0        0     5195 2024-04-26 16:44:52.822361 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticated_session.py
+-rw-r--r--   0        0        0     3064 2024-04-26 16:44:52.830361 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticated_session_asn.py
+-rw-r--r--   0        0        0     2826 2024-04-26 16:44:52.834361 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticated_session_geo_ip.py
+-rw-r--r--   0        0        0     3865 2024-04-26 16:44:52.842361 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticated_session_user_agent.py
+-rw-r--r--   0        0        0     2646 2024-04-26 16:44:52.850361 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticated_session_user_agent_device.py
+-rw-r--r--   0        0        0     2792 2024-04-26 16:44:52.854361 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticated_session_user_agent_os.py
+-rw-r--r--   0        0        0     2725 2024-04-26 16:44:52.858361 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticated_session_user_agent_user_agent.py
+-rw-r--r--   0        0        0      895 2024-04-26 16:44:52.862361 authentik_client-2024.4.1.post1714149882/authentik_client/models/authentication_enum.py
+-rw-r--r--   0        0        0      782 2024-04-26 16:44:52.866361 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_attachment_enum.py
+-rw-r--r--   0        0        0     4686 2024-04-26 16:44:52.874361 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_duo_challenge.py
+-rw-r--r--   0        0        0     2743 2024-04-26 16:44:52.878361 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_duo_challenge_response_request.py
+-rw-r--r--   0        0        0     5327 2024-04-26 16:44:52.886361 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_duo_stage.py
+-rw-r--r--   0        0        0     2768 2024-04-26 16:44:52.890360 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_duo_stage_device_import_response.py
+-rw-r--r--   0        0        0     2785 2024-04-26 16:44:52.894361 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py
+-rw-r--r--   0        0        0     4744 2024-04-26 16:44:52.902361 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_duo_stage_request.py
+-rw-r--r--   0        0        0     4594 2024-04-26 16:44:52.906360 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_sms_challenge.py
+-rw-r--r--   0        0        0     3022 2024-04-26 16:44:52.914360 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_sms_challenge_response_request.py
+-rw-r--r--   0        0        0     6409 2024-04-26 16:44:52.918361 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_sms_stage.py
+-rw-r--r--   0        0        0     5595 2024-04-26 16:44:52.926360 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_sms_stage_request.py
+-rw-r--r--   0        0        0     4474 2024-04-26 16:44:52.930360 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_static_challenge.py
+-rw-r--r--   0        0        0     2761 2024-04-26 16:44:52.938361 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_static_challenge_response_request.py
+-rw-r--r--   0        0        0     5363 2024-04-26 16:44:52.942360 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_static_stage.py
+-rw-r--r--   0        0        0     4392 2024-04-26 16:44:52.946360 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_static_stage_request.py
+-rw-r--r--   0        0        0     4468 2024-04-26 16:44:52.954360 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_totp_challenge.py
+-rw-r--r--   0        0        0     2858 2024-04-26 16:44:52.958360 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_totp_challenge_response_request.py
+-rw-r--r--   0        0        0     5132 2024-04-26 16:44:52.966360 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_totp_stage.py
+-rw-r--r--   0        0        0     4201 2024-04-26 16:44:52.970360 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_totp_stage_request.py
+-rw-r--r--   0        0        0     6722 2024-04-26 16:44:52.998360 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_validate_stage.py
+-rw-r--r--   0        0        0     4893 2024-04-26 16:44:53.006360 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_validate_stage_request.py
+-rw-r--r--   0        0        0     5717 2024-04-26 16:44:53.014360 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_validation_challenge.py
+-rw-r--r--   0        0        0     3805 2024-04-26 16:44:53.018360 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_validation_challenge_response_request.py
+-rw-r--r--   0        0        0     4499 2024-04-26 16:44:53.026360 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_web_authn_challenge.py
+-rw-r--r--   0        0        0     2852 2024-04-26 16:44:53.030360 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_web_authn_challenge_response_request.py
+-rw-r--r--   0        0        0     7081 2024-04-26 16:44:53.034360 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_web_authn_stage.py
+-rw-r--r--   0        0        0     5302 2024-04-26 16:44:53.038360 authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_web_authn_stage_request.py
+-rw-r--r--   0        0        0     2718 2024-04-26 16:44:53.042360 authentik_client-2024.4.1.post1714149882/authentik_client/models/auto_submit_challenge_response_request.py
+-rw-r--r--   0        0        0     4388 2024-04-26 16:44:53.046360 authentik_client-2024.4.1.post1714149882/authentik_client/models/autosubmit_challenge.py
+-rw-r--r--   0        0        0      950 2024-04-26 16:44:53.050360 authentik_client-2024.4.1.post1714149882/authentik_client/models/backends_enum.py
+-rw-r--r--   0        0        0      748 2024-04-26 16:44:53.050360 authentik_client-2024.4.1.post1714149882/authentik_client/models/binding_type_enum.py
+-rw-r--r--   0        0        0     2995 2024-04-26 16:44:53.054360 authentik_client-2024.4.1.post1714149882/authentik_client/models/blueprint_file.py
+-rw-r--r--   0        0        0     4453 2024-04-26 16:44:53.058360 authentik_client-2024.4.1.post1714149882/authentik_client/models/blueprint_instance.py
+-rw-r--r--   0        0        0     3208 2024-04-26 16:44:53.062360 authentik_client-2024.4.1.post1714149882/authentik_client/models/blueprint_instance_request.py
+-rw-r--r--   0        0        0      836 2024-04-26 16:44:53.066360 authentik_client-2024.4.1.post1714149882/authentik_client/models/blueprint_instance_status_enum.py
+-rw-r--r--   0        0        0     6255 2024-04-26 16:44:53.066360 authentik_client-2024.4.1.post1714149882/authentik_client/models/brand.py
+-rw-r--r--   0        0        0     6307 2024-04-26 16:44:53.070360 authentik_client-2024.4.1.post1714149882/authentik_client/models/brand_request.py
+-rw-r--r--   0        0        0     2501 2024-04-26 16:44:53.074360 authentik_client-2024.4.1.post1714149882/authentik_client/models/cache.py
+-rw-r--r--   0        0        0      875 2024-04-26 16:44:53.078360 authentik_client-2024.4.1.post1714149882/authentik_client/models/capabilities_enum.py
+-rw-r--r--   0        0        0     4476 2024-04-26 16:44:53.082360 authentik_client-2024.4.1.post1714149882/authentik_client/models/captcha_challenge.py
+-rw-r--r--   0        0        0     2797 2024-04-26 16:44:53.086360 authentik_client-2024.4.1.post1714149882/authentik_client/models/captcha_challenge_response_request.py
+-rw-r--r--   0        0        0     4438 2024-04-26 16:44:53.090360 authentik_client-2024.4.1.post1714149882/authentik_client/models/captcha_stage.py
+-rw-r--r--   0        0        0     3774 2024-04-26 16:44:53.094360 authentik_client-2024.4.1.post1714149882/authentik_client/models/captcha_stage_request.py
+-rw-r--r--   0        0        0     2522 2024-04-26 16:44:53.098360 authentik_client-2024.4.1.post1714149882/authentik_client/models/certificate_data.py
+-rw-r--r--   0        0        0     2861 2024-04-26 16:44:53.102360 authentik_client-2024.4.1.post1714149882/authentik_client/models/certificate_generation_request.py
+-rw-r--r--   0        0        0     6655 2024-04-26 16:44:53.106360 authentik_client-2024.4.1.post1714149882/authentik_client/models/certificate_key_pair.py
+-rw-r--r--   0        0        0     2989 2024-04-26 16:44:53.110360 authentik_client-2024.4.1.post1714149882/authentik_client/models/certificate_key_pair_request.py
+-rw-r--r--   0        0        0      747 2024-04-26 16:44:53.110360 authentik_client-2024.4.1.post1714149882/authentik_client/models/challenge_choices.py
+-rw-r--r--   0        0        0    24236 2024-04-26 16:44:53.118360 authentik_client-2024.4.1.post1714149882/authentik_client/models/challenge_types.py
+-rw-r--r--   0        0        0      729 2024-04-26 16:44:53.122360 authentik_client-2024.4.1.post1714149882/authentik_client/models/client_type_enum.py
+-rw-r--r--   0        0        0     3539 2024-04-26 16:44:53.126360 authentik_client-2024.4.1.post1714149882/authentik_client/models/config.py
+-rw-r--r--   0        0        0     4021 2024-04-26 16:44:53.130360 authentik_client-2024.4.1.post1714149882/authentik_client/models/connection_token.py
+-rw-r--r--   0        0        0     2662 2024-04-26 16:44:53.130360 authentik_client-2024.4.1.post1714149882/authentik_client/models/connection_token_request.py
+-rw-r--r--   0        0        0     5736 2024-04-26 16:44:53.138360 authentik_client-2024.4.1.post1714149882/authentik_client/models/consent_challenge.py
+-rw-r--r--   0        0        0     2838 2024-04-26 16:44:53.142360 authentik_client-2024.4.1.post1714149882/authentik_client/models/consent_challenge_response_request.py
+-rw-r--r--   0        0        0     2513 2024-04-26 16:44:53.142360 authentik_client-2024.4.1.post1714149882/authentik_client/models/consent_permission.py
+-rw-r--r--   0        0        0     4511 2024-04-26 16:44:53.146360 authentik_client-2024.4.1.post1714149882/authentik_client/models/consent_stage.py
+-rw-r--r--   0        0        0      783 2024-04-26 16:44:53.150360 authentik_client-2024.4.1.post1714149882/authentik_client/models/consent_stage_mode_enum.py
+-rw-r--r--   0        0        0     3569 2024-04-26 16:44:53.154360 authentik_client-2024.4.1.post1714149882/authentik_client/models/consent_stage_request.py
+-rw-r--r--   0        0        0     2891 2024-04-26 16:44:53.158360 authentik_client-2024.4.1.post1714149882/authentik_client/models/contextual_flow_info.py
+-rw-r--r--   0        0        0      879 2024-04-26 16:44:53.162360 authentik_client-2024.4.1.post1714149882/authentik_client/models/contextual_flow_info_layout_enum.py
+-rw-r--r--   0        0        0     2657 2024-04-26 16:44:53.166360 authentik_client-2024.4.1.post1714149882/authentik_client/models/coordinate.py
+-rw-r--r--   0        0        0     4704 2024-04-26 16:44:53.170360 authentik_client-2024.4.1.post1714149882/authentik_client/models/current_brand.py
+-rw-r--r--   0        0        0      771 2024-04-26 16:44:53.174360 authentik_client-2024.4.1.post1714149882/authentik_client/models/denied_action_enum.py
+-rw-r--r--   0        0        0     4200 2024-04-26 16:44:53.178360 authentik_client-2024.4.1.post1714149882/authentik_client/models/deny_stage.py
+-rw-r--r--   0        0        0     3230 2024-04-26 16:44:53.182360 authentik_client-2024.4.1.post1714149882/authentik_client/models/deny_stage_request.py
+-rw-r--r--   0        0        0     3522 2024-04-26 16:44:53.186360 authentik_client-2024.4.1.post1714149882/authentik_client/models/device.py
+-rw-r--r--   0        0        0     2657 2024-04-26 16:44:53.194360 authentik_client-2024.4.1.post1714149882/authentik_client/models/device_challenge.py
+-rw-r--r--   0        0        0     2792 2024-04-26 16:44:53.198360 authentik_client-2024.4.1.post1714149882/authentik_client/models/device_challenge_request.py
+-rw-r--r--   0        0        0      780 2024-04-26 16:44:53.202360 authentik_client-2024.4.1.post1714149882/authentik_client/models/device_classes_enum.py
+-rw-r--r--   0        0        0     1244 2024-04-26 16:44:53.206360 authentik_client-2024.4.1.post1714149882/authentik_client/models/digest_algorithm_enum.py
+-rw-r--r--   0        0        0      695 2024-04-26 16:44:53.210360 authentik_client-2024.4.1.post1714149882/authentik_client/models/digits_enum.py
+-rw-r--r--   0        0        0     4969 2024-04-26 16:44:53.210360 authentik_client-2024.4.1.post1714149882/authentik_client/models/docker_service_connection.py
+-rw-r--r--   0        0        0     4087 2024-04-26 16:44:53.214360 authentik_client-2024.4.1.post1714149882/authentik_client/models/docker_service_connection_request.py
+-rw-r--r--   0        0        0     2847 2024-04-26 16:44:53.218360 authentik_client-2024.4.1.post1714149882/authentik_client/models/domain.py
+-rw-r--r--   0        0        0     2746 2024-04-26 16:44:53.222360 authentik_client-2024.4.1.post1714149882/authentik_client/models/domain_request.py
+-rw-r--r--   0        0        0     4155 2024-04-26 16:44:53.226360 authentik_client-2024.4.1.post1714149882/authentik_client/models/dummy_challenge.py
+-rw-r--r--   0        0        0     2681 2024-04-26 16:44:53.230360 authentik_client-2024.4.1.post1714149882/authentik_client/models/dummy_challenge_response_request.py
+-rw-r--r--   0        0        0     4515 2024-04-26 16:44:53.234360 authentik_client-2024.4.1.post1714149882/authentik_client/models/dummy_policy.py
+-rw-r--r--   0        0        0     3237 2024-04-26 16:44:53.238360 authentik_client-2024.4.1.post1714149882/authentik_client/models/dummy_policy_request.py
+-rw-r--r--   0        0        0     4213 2024-04-26 16:44:53.242360 authentik_client-2024.4.1.post1714149882/authentik_client/models/dummy_stage.py
+-rw-r--r--   0        0        0     3232 2024-04-26 16:44:53.246360 authentik_client-2024.4.1.post1714149882/authentik_client/models/dummy_stage_request.py
+-rw-r--r--   0        0        0     2720 2024-04-26 16:44:53.250360 authentik_client-2024.4.1.post1714149882/authentik_client/models/duo_device.py
+-rw-r--r--   0        0        0     2575 2024-04-26 16:44:53.250360 authentik_client-2024.4.1.post1714149882/authentik_client/models/duo_device_enrollment_status.py
+-rw-r--r--   0        0        0     2619 2024-04-26 16:44:53.254360 authentik_client-2024.4.1.post1714149882/authentik_client/models/duo_device_request.py
+-rw-r--r--   0        0        0      748 2024-04-26 16:44:53.258360 authentik_client-2024.4.1.post1714149882/authentik_client/models/duo_response_enum.py
+-rw-r--r--   0        0        0     4090 2024-04-26 16:44:53.262360 authentik_client-2024.4.1.post1714149882/authentik_client/models/email_challenge.py
+-rw-r--r--   0        0        0     2770 2024-04-26 16:44:53.266360 authentik_client-2024.4.1.post1714149882/authentik_client/models/email_challenge_response_request.py
+-rw-r--r--   0        0        0     5902 2024-04-26 16:44:53.270360 authentik_client-2024.4.1.post1714149882/authentik_client/models/email_stage.py
+-rw-r--r--   0        0        0     5121 2024-04-26 16:44:53.274360 authentik_client-2024.4.1.post1714149882/authentik_client/models/email_stage_request.py
+-rw-r--r--   0        0        0     4707 2024-04-26 16:44:53.278360 authentik_client-2024.4.1.post1714149882/authentik_client/models/endpoint.py
+-rw-r--r--   0        0        0     3678 2024-04-26 16:44:53.282359 authentik_client-2024.4.1.post1714149882/authentik_client/models/endpoint_request.py
+-rw-r--r--   0        0        0     2530 2024-04-26 16:44:53.290360 authentik_client-2024.4.1.post1714149882/authentik_client/models/error_detail.py
+-rw-r--r--   0        0        0     3309 2024-04-26 16:44:53.290360 authentik_client-2024.4.1.post1714149882/authentik_client/models/error_reporting_config.py
+-rw-r--r--   0        0        0     4129 2024-04-26 16:44:53.294360 authentik_client-2024.4.1.post1714149882/authentik_client/models/event.py
+-rw-r--r--   0        0        0     1730 2024-04-26 16:44:53.298359 authentik_client-2024.4.1.post1714149882/authentik_client/models/event_actions.py
+-rw-r--r--   0        0        0     6006 2024-04-26 16:44:53.302359 authentik_client-2024.4.1.post1714149882/authentik_client/models/event_matcher_policy.py
+-rw-r--r--   0        0        0     4807 2024-04-26 16:44:53.306360 authentik_client-2024.4.1.post1714149882/authentik_client/models/event_matcher_policy_request.py
+-rw-r--r--   0        0        0     3990 2024-04-26 16:44:53.310360 authentik_client-2024.4.1.post1714149882/authentik_client/models/event_request.py
+-rw-r--r--   0        0        0     2697 2024-04-26 16:44:53.314360 authentik_client-2024.4.1.post1714149882/authentik_client/models/event_top_per_user.py
+-rw-r--r--   0        0        0     3926 2024-04-26 16:44:53.318359 authentik_client-2024.4.1.post1714149882/authentik_client/models/expiring_base_grant_model.py
+-rw-r--r--   0        0        0     4191 2024-04-26 16:44:53.322359 authentik_client-2024.4.1.post1714149882/authentik_client/models/expression_policy.py
+-rw-r--r--   0        0        0     2992 2024-04-26 16:44:53.326359 authentik_client-2024.4.1.post1714149882/authentik_client/models/expression_policy_request.py
+-rw-r--r--   0        0        0     4524 2024-04-26 16:44:53.330360 authentik_client-2024.4.1.post1714149882/authentik_client/models/extra_role_object_permission.py
+-rw-r--r--   0        0        0     4524 2024-04-26 16:44:53.334360 authentik_client-2024.4.1.post1714149882/authentik_client/models/extra_user_object_permission.py
+-rw-r--r--   0        0        0     2519 2024-04-26 16:44:53.338359 authentik_client-2024.4.1.post1714149882/authentik_client/models/file_path_request.py
+-rw-r--r--   0        0        0     6047 2024-04-26 16:44:53.346359 authentik_client-2024.4.1.post1714149882/authentik_client/models/flow.py
+-rw-r--r--   0        0        0    25850 2024-04-26 16:44:53.350359 authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_challenge_response_request.py
+-rw-r--r--   0        0        0      934 2024-04-26 16:44:53.354359 authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_designation_enum.py
+-rw-r--r--   0        0        0     2533 2024-04-26 16:44:53.358359 authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_diagram.py
+-rw-r--r--   0        0        0     4505 2024-04-26 16:44:53.362359 authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_error_challenge.py
+-rw-r--r--   0        0        0     3111 2024-04-26 16:44:53.370359 authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_import_result.py
+-rw-r--r--   0        0        0     3418 2024-04-26 16:44:53.374359 authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_inspection.py
+-rw-r--r--   0        0        0     3875 2024-04-26 16:44:53.374359 authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_inspector_plan.py
+-rw-r--r--   0        0        0      837 2024-04-26 16:44:53.378359 authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_layout_enum.py
+-rw-r--r--   0        0        0     4741 2024-04-26 16:44:53.382359 authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_request.py
+-rw-r--r--   0        0        0     5223 2024-04-26 16:44:53.386359 authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_set.py
+-rw-r--r--   0        0        0     4459 2024-04-26 16:44:53.386359 authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_set_request.py
+-rw-r--r--   0        0        0     4763 2024-04-26 16:44:53.390359 authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_stage_binding.py
+-rw-r--r--   0        0        0     3983 2024-04-26 16:44:53.394359 authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_stage_binding_request.py
+-rw-r--r--   0        0        0     2641 2024-04-26 16:44:53.398359 authentik_client-2024.4.1.post1714149882/authentik_client/models/footer_link.py
+-rw-r--r--   0        0        0     2531 2024-04-26 16:44:53.398359 authentik_client-2024.4.1.post1714149882/authentik_client/models/generic_error.py
+-rw-r--r--   0        0        0      865 2024-04-26 16:44:53.402359 authentik_client-2024.4.1.post1714149882/authentik_client/models/geoip_binding_enum.py
+-rw-r--r--   0        0        0     5445 2024-04-26 16:44:53.406359 authentik_client-2024.4.1.post1714149882/authentik_client/models/group.py
+-rw-r--r--   0        0        0     4209 2024-04-26 16:44:53.410359 authentik_client-2024.4.1.post1714149882/authentik_client/models/group_member.py
+-rw-r--r--   0        0        0     4006 2024-04-26 16:44:53.414359 authentik_client-2024.4.1.post1714149882/authentik_client/models/group_member_request.py
+-rw-r--r--   0        0        0     3347 2024-04-26 16:44:53.418359 authentik_client-2024.4.1.post1714149882/authentik_client/models/group_request.py
+-rw-r--r--   0        0        0     6080 2024-04-26 16:44:53.426359 authentik_client-2024.4.1.post1714149882/authentik_client/models/identification_challenge.py
+-rw-r--r--   0        0        0     3174 2024-04-26 16:44:53.430359 authentik_client-2024.4.1.post1714149882/authentik_client/models/identification_challenge_response_request.py
+-rw-r--r--   0        0        0     7503 2024-04-26 16:44:53.430359 authentik_client-2024.4.1.post1714149882/authentik_client/models/identification_stage.py
+-rw-r--r--   0        0        0     6533 2024-04-26 16:44:53.438359 authentik_client-2024.4.1.post1714149882/authentik_client/models/identification_stage_request.py
+-rw-r--r--   0        0        0     2438 2024-04-26 16:44:53.442359 authentik_client-2024.4.1.post1714149882/authentik_client/models/install_id.py
+-rw-r--r--   0        0        0      771 2024-04-26 16:44:53.442359 authentik_client-2024.4.1.post1714149882/authentik_client/models/intent_enum.py
+-rw-r--r--   0        0        0      800 2024-04-26 16:44:53.446359 authentik_client-2024.4.1.post1714149882/authentik_client/models/invalid_response_action_enum.py
+-rw-r--r--   0        0        0     4878 2024-04-26 16:44:53.450359 authentik_client-2024.4.1.post1714149882/authentik_client/models/invitation.py
+-rw-r--r--   0        0        0     3895 2024-04-26 16:44:53.454359 authentik_client-2024.4.1.post1714149882/authentik_client/models/invitation_request.py
+-rw-r--r--   0        0        0     4508 2024-04-26 16:44:53.454359 authentik_client-2024.4.1.post1714149882/authentik_client/models/invitation_stage.py
+-rw-r--r--   0        0        0     3527 2024-04-26 16:44:53.458359 authentik_client-2024.4.1.post1714149882/authentik_client/models/invitation_stage_request.py
+-rw-r--r--   0        0        0      729 2024-04-26 16:44:53.462359 authentik_client-2024.4.1.post1714149882/authentik_client/models/issuer_mode_enum.py
+-rw-r--r--   0        0        0     4386 2024-04-26 16:44:53.462359 authentik_client-2024.4.1.post1714149882/authentik_client/models/kubernetes_service_connection.py
+-rw-r--r--   0        0        0     3454 2024-04-26 16:44:53.466359 authentik_client-2024.4.1.post1714149882/authentik_client/models/kubernetes_service_connection_request.py
+-rw-r--r--   0        0        0     2811 2024-04-26 16:44:53.470359 authentik_client-2024.4.1.post1714149882/authentik_client/models/ldap_debug.py
+-rw-r--r--   0        0        0     5765 2024-04-26 16:44:53.474359 authentik_client-2024.4.1.post1714149882/authentik_client/models/ldap_outpost_config.py
+-rw-r--r--   0        0        0     4378 2024-04-26 16:44:53.478359 authentik_client-2024.4.1.post1714149882/authentik_client/models/ldap_property_mapping.py
+-rw-r--r--   0        0        0     3478 2024-04-26 16:44:53.478359 authentik_client-2024.4.1.post1714149882/authentik_client/models/ldap_property_mapping_request.py
+-rw-r--r--   0        0        0     8694 2024-04-26 16:44:53.482359 authentik_client-2024.4.1.post1714149882/authentik_client/models/ldap_provider.py
+-rw-r--r--   0        0        0     6192 2024-04-26 16:44:53.482359 authentik_client-2024.4.1.post1714149882/authentik_client/models/ldap_provider_request.py
+-rw-r--r--   0        0        0    11791 2024-04-26 16:44:53.486359 authentik_client-2024.4.1.post1714149882/authentik_client/models/ldap_source.py
+-rw-r--r--   0        0        0     9542 2024-04-26 16:44:53.490359 authentik_client-2024.4.1.post1714149882/authentik_client/models/ldap_source_request.py
+-rw-r--r--   0        0        0     3129 2024-04-26 16:44:53.494359 authentik_client-2024.4.1.post1714149882/authentik_client/models/ldap_sync_status.py
+-rw-r--r--   0        0        0      726 2024-04-26 16:44:53.466359 authentik_client-2024.4.1.post1714149882/authentik_client/models/ldapapi_access_mode.py
+-rw-r--r--   0        0        0     3278 2024-04-26 16:44:53.498359 authentik_client-2024.4.1.post1714149882/authentik_client/models/license.py
+-rw-r--r--   0        0        0     2897 2024-04-26 16:44:53.502359 authentik_client-2024.4.1.post1714149882/authentik_client/models/license_forecast.py
+-rw-r--r--   0        0        0     2509 2024-04-26 16:44:53.506359 authentik_client-2024.4.1.post1714149882/authentik_client/models/license_request.py
+-rw-r--r--   0        0        0     3222 2024-04-26 16:44:53.510359 authentik_client-2024.4.1.post1714149882/authentik_client/models/license_summary.py
+-rw-r--r--   0        0        0     2411 2024-04-26 16:44:53.510359 authentik_client-2024.4.1.post1714149882/authentik_client/models/link.py
+-rw-r--r--   0        0        0     2882 2024-04-26 16:44:53.514359 authentik_client-2024.4.1.post1714149882/authentik_client/models/log_event.py
+-rw-r--r--   0        0        0      843 2024-04-26 16:44:53.514359 authentik_client-2024.4.1.post1714149882/authentik_client/models/log_level_enum.py
+-rw-r--r--   0        0        0     6520 2024-04-26 16:44:53.518359 authentik_client-2024.4.1.post1714149882/authentik_client/models/login_challenge_types.py
+-rw-r--r--   0        0        0     4171 2024-04-26 16:44:53.522359 authentik_client-2024.4.1.post1714149882/authentik_client/models/login_metrics.py
+-rw-r--r--   0        0        0     3192 2024-04-26 16:44:53.522359 authentik_client-2024.4.1.post1714149882/authentik_client/models/login_source.py
+-rw-r--r--   0        0        0     2513 2024-04-26 16:44:53.526359 authentik_client-2024.4.1.post1714149882/authentik_client/models/metadata.py
+-rw-r--r--   0        0        0     7604 2024-04-26 16:44:53.526359 authentik_client-2024.4.1.post1714149882/authentik_client/models/model_enum.py
+-rw-r--r--   0        0        0     9828 2024-04-26 16:44:53.530359 authentik_client-2024.4.1.post1714149882/authentik_client/models/model_request.py
+-rw-r--r--   0        0        0     1559 2024-04-26 16:44:53.530359 authentik_client-2024.4.1.post1714149882/authentik_client/models/name_id_policy_enum.py
+-rw-r--r--   0        0        0      831 2024-04-26 16:44:53.534359 authentik_client-2024.4.1.post1714149882/authentik_client/models/network_binding_enum.py
+-rw-r--r--   0        0        0      764 2024-04-26 16:44:53.534359 authentik_client-2024.4.1.post1714149882/authentik_client/models/not_configured_action_enum.py
+-rw-r--r--   0        0        0     3479 2024-04-26 16:44:53.538359 authentik_client-2024.4.1.post1714149882/authentik_client/models/notification.py
+-rw-r--r--   0        0        0     2858 2024-04-26 16:44:53.542359 authentik_client-2024.4.1.post1714149882/authentik_client/models/notification_request.py
+-rw-r--r--   0        0        0     4010 2024-04-26 16:44:53.542359 authentik_client-2024.4.1.post1714149882/authentik_client/models/notification_rule.py
+-rw-r--r--   0        0        0     3549 2024-04-26 16:44:53.546359 authentik_client-2024.4.1.post1714149882/authentik_client/models/notification_rule_request.py
+-rw-r--r--   0        0        0     3760 2024-04-26 16:44:53.550359 authentik_client-2024.4.1.post1714149882/authentik_client/models/notification_transport.py
+-rw-r--r--   0        0        0      818 2024-04-26 16:44:53.554359 authentik_client-2024.4.1.post1714149882/authentik_client/models/notification_transport_mode_enum.py
+-rw-r--r--   0        0        0     3500 2024-04-26 16:44:53.558359 authentik_client-2024.4.1.post1714149882/authentik_client/models/notification_transport_request.py
+-rw-r--r--   0        0        0     2503 2024-04-26 16:44:53.562359 authentik_client-2024.4.1.post1714149882/authentik_client/models/notification_transport_test.py
+-rw-r--r--   0        0        0     2707 2024-04-26 16:44:53.566359 authentik_client-2024.4.1.post1714149882/authentik_client/models/notification_webhook_mapping.py
+-rw-r--r--   0        0        0     2717 2024-04-26 16:44:53.570359 authentik_client-2024.4.1.post1714149882/authentik_client/models/notification_webhook_mapping_request.py
+-rw-r--r--   0        0        0     8888 2024-04-26 16:44:53.574359 authentik_client-2024.4.1.post1714149882/authentik_client/models/o_auth2_provider.py
+-rw-r--r--   0        0        0     6654 2024-04-26 16:44:53.578359 authentik_client-2024.4.1.post1714149882/authentik_client/models/o_auth2_provider_request.py
+-rw-r--r--   0        0        0     3482 2024-04-26 16:44:53.582359 authentik_client-2024.4.1.post1714149882/authentik_client/models/o_auth2_provider_setup_urls.py
+-rw-r--r--   0        0        0     4164 2024-04-26 16:44:53.586359 authentik_client-2024.4.1.post1714149882/authentik_client/models/o_auth_device_code_challenge.py
+-rw-r--r--   0        0        0     2846 2024-04-26 16:44:53.590359 authentik_client-2024.4.1.post1714149882/authentik_client/models/o_auth_device_code_challenge_response_request.py
+-rw-r--r--   0        0        0     4213 2024-04-26 16:44:53.594359 authentik_client-2024.4.1.post1714149882/authentik_client/models/o_auth_device_code_finish_challenge.py
+-rw-r--r--   0        0        0     2816 2024-04-26 16:44:53.598359 authentik_client-2024.4.1.post1714149882/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py
+-rw-r--r--   0        0        0    10563 2024-04-26 16:44:53.602359 authentik_client-2024.4.1.post1714149882/authentik_client/models/o_auth_source.py
+-rw-r--r--   0        0        0     8013 2024-04-26 16:44:53.610359 authentik_client-2024.4.1.post1714149882/authentik_client/models/o_auth_source_request.py
+-rw-r--r--   0        0        0     3922 2024-04-26 16:44:53.614359 authentik_client-2024.4.1.post1714149882/authentik_client/models/open_id_connect_configuration.py
+-rw-r--r--   0        0        0     5545 2024-04-26 16:44:53.618359 authentik_client-2024.4.1.post1714149882/authentik_client/models/outpost.py
+-rw-r--r--   0        0        0     2541 2024-04-26 16:44:53.622359 authentik_client-2024.4.1.post1714149882/authentik_client/models/outpost_default_config.py
+-rw-r--r--   0        0        0     3755 2024-04-26 16:44:53.626359 authentik_client-2024.4.1.post1714149882/authentik_client/models/outpost_health.py
+-rw-r--r--   0        0        0     4050 2024-04-26 16:44:53.626359 authentik_client-2024.4.1.post1714149882/authentik_client/models/outpost_request.py
+-rw-r--r--   0        0        0      752 2024-04-26 16:44:53.630359 authentik_client-2024.4.1.post1714149882/authentik_client/models/outpost_type_enum.py
+-rw-r--r--   0        0        0     3322 2024-04-26 16:44:53.634359 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_application_list.py
+-rw-r--r--   0        0        0     3395 2024-04-26 16:44:53.638359 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_authenticated_session_list.py
+-rw-r--r--   0        0        0     3404 2024-04-26 16:44:53.646359 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_authenticator_duo_stage_list.py
+-rw-r--r--   0        0        0     3404 2024-04-26 16:44:53.646359 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_authenticator_sms_stage_list.py
+-rw-r--r--   0        0        0     3428 2024-04-26 16:44:53.650359 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_authenticator_static_stage_list.py
+-rw-r--r--   0        0        0     3412 2024-04-26 16:44:53.654359 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_authenticator_totp_stage_list.py
+-rw-r--r--   0        0        0     3444 2024-04-26 16:44:53.658359 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_authenticator_validate_stage_list.py
+-rw-r--r--   0        0        0     3445 2024-04-26 16:44:53.662359 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_authenticator_web_authn_stage_list.py
+-rw-r--r--   0        0        0     3371 2024-04-26 16:44:53.666359 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_blueprint_instance_list.py
+-rw-r--r--   0        0        0     3274 2024-04-26 16:44:53.670359 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_brand_list.py
+-rw-r--r--   0        0        0     3331 2024-04-26 16:44:53.674359 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_captcha_stage_list.py
+-rw-r--r--   0        0        0     3380 2024-04-26 16:44:53.678359 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_certificate_key_pair_list.py
+-rw-r--r--   0        0        0     3355 2024-04-26 16:44:53.682359 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_connection_token_list.py
+-rw-r--r--   0        0        0     3331 2024-04-26 16:44:53.686359 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_consent_stage_list.py
+-rw-r--r--   0        0        0     3307 2024-04-26 16:44:53.690358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_deny_stage_list.py
+-rw-r--r--   0        0        0     3420 2024-04-26 16:44:53.694358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_docker_service_connection_list.py
+-rw-r--r--   0        0        0     3282 2024-04-26 16:44:53.698359 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_domain_list.py
+-rw-r--r--   0        0        0     3323 2024-04-26 16:44:53.702359 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_dummy_policy_list.py
+-rw-r--r--   0        0        0     3315 2024-04-26 16:44:53.706359 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_dummy_stage_list.py
+-rw-r--r--   0        0        0     3307 2024-04-26 16:44:53.710358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_duo_device_list.py
+-rw-r--r--   0        0        0     3315 2024-04-26 16:44:53.710358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_email_stage_list.py
+-rw-r--r--   0        0        0     3298 2024-04-26 16:44:53.714358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_endpoint_list.py
+-rw-r--r--   0        0        0     3274 2024-04-26 16:44:53.718358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_event_list.py
+-rw-r--r--   0        0        0     3380 2024-04-26 16:44:53.722359 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_event_matcher_policy_list.py
+-rw-r--r--   0        0        0     3413 2024-04-26 16:44:53.726359 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_expiring_base_grant_model_list.py
+-rw-r--r--   0        0        0     3363 2024-04-26 16:44:53.730358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_expression_policy_list.py
+-rw-r--r--   0        0        0     3437 2024-04-26 16:44:53.734358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_extra_role_object_permission_list.py
+-rw-r--r--   0        0        0     3437 2024-04-26 16:44:53.738358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_extra_user_object_permission_list.py
+-rw-r--r--   0        0        0     3266 2024-04-26 16:44:53.742358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_flow_list.py
+-rw-r--r--   0        0        0     3364 2024-04-26 16:44:53.746358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_flow_stage_binding_list.py
+-rw-r--r--   0        0        0     3274 2024-04-26 16:44:53.750358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_group_list.py
+-rw-r--r--   0        0        0     3387 2024-04-26 16:44:53.750358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_identification_stage_list.py
+-rw-r--r--   0        0        0     3314 2024-04-26 16:44:53.754358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_invitation_list.py
+-rw-r--r--   0        0        0     3355 2024-04-26 16:44:53.758358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_invitation_stage_list.py
+-rw-r--r--   0        0        0     3452 2024-04-26 16:44:53.762358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_kubernetes_service_connection_list.py
+-rw-r--r--   0        0        0     3372 2024-04-26 16:44:53.766358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_ldap_outpost_config_list.py
+-rw-r--r--   0        0        0     3388 2024-04-26 16:44:53.770358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_ldap_property_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-26 16:44:53.770358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_ldap_provider_list.py
+-rw-r--r--   0        0        0     3315 2024-04-26 16:44:53.774358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_ldap_source_list.py
+-rw-r--r--   0        0        0     3290 2024-04-26 16:44:53.778358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_license_list.py
+-rw-r--r--   0        0        0     3330 2024-04-26 16:44:53.782358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_notification_list.py
+-rw-r--r--   0        0        0     3363 2024-04-26 16:44:53.786358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_notification_rule_list.py
+-rw-r--r--   0        0        0     3403 2024-04-26 16:44:53.786358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_notification_transport_list.py
+-rw-r--r--   0        0        0     3444 2024-04-26 16:44:53.790358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_notification_webhook_mapping_list.py
+-rw-r--r--   0        0        0     3348 2024-04-26 16:44:53.794358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_o_auth2_provider_list.py
+-rw-r--r--   0        0        0     3324 2024-04-26 16:44:53.798358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_o_auth_source_list.py
+-rw-r--r--   0        0        0     3290 2024-04-26 16:44:53.802358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_outpost_list.py
+-rw-r--r--   0        0        0     3396 2024-04-26 16:44:53.806358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_password_expiry_policy_list.py
+-rw-r--r--   0        0        0     3347 2024-04-26 16:44:53.806358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_password_policy_list.py
+-rw-r--r--   0        0        0     3339 2024-04-26 16:44:53.810358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_password_stage_list.py
+-rw-r--r--   0        0        0     3314 2024-04-26 16:44:53.814358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_permission_list.py
+-rw-r--r--   0        0        0     3396 2024-04-26 16:44:53.818358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_plex_source_connection_list.py
+-rw-r--r--   0        0        0     3315 2024-04-26 16:44:53.822358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_plex_source_list.py
+-rw-r--r--   0        0        0     3339 2024-04-26 16:44:53.822358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_policy_binding_list.py
+-rw-r--r--   0        0        0     3282 2024-04-26 16:44:53.826358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_policy_list.py
+-rw-r--r--   0        0        0     3282 2024-04-26 16:44:53.830358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_prompt_list.py
+-rw-r--r--   0        0        0     3323 2024-04-26 16:44:53.834358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_prompt_stage_list.py
+-rw-r--r--   0        0        0     3355 2024-04-26 16:44:53.838358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_property_mapping_list.py
+-rw-r--r--   0        0        0     3298 2024-04-26 16:44:53.842358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_provider_list.py
+-rw-r--r--   0        0        0     3380 2024-04-26 16:44:53.842358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_proxy_outpost_config_list.py
+-rw-r--r--   0        0        0     3339 2024-04-26 16:44:53.846358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_proxy_provider_list.py
+-rw-r--r--   0        0        0     3380 2024-04-26 16:44:53.850358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_rac_property_mapping_list.py
+-rw-r--r--   0        0        0     3323 2024-04-26 16:44:53.854358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_rac_provider_list.py
+-rw-r--r--   0        0        0     3388 2024-04-26 16:44:53.858358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_radius_outpost_config_list.py
+-rw-r--r--   0        0        0     3347 2024-04-26 16:44:53.862358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_radius_provider_list.py
+-rw-r--r--   0        0        0     3314 2024-04-26 16:44:53.862358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_reputation_list.py
+-rw-r--r--   0        0        0     3363 2024-04-26 16:44:53.866358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_reputation_policy_list.py
+-rw-r--r--   0        0        0     3461 2024-04-26 16:44:53.870358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_role_assigned_object_permission_list.py
+-rw-r--r--   0        0        0     3266 2024-04-26 16:44:53.874358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_role_list.py
+-rw-r--r--   0        0        0     3388 2024-04-26 16:44:53.878358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_saml_property_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-26 16:44:53.882358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_saml_provider_list.py
+-rw-r--r--   0        0        0     3315 2024-04-26 16:44:53.886358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_saml_source_list.py
+-rw-r--r--   0        0        0     3323 2024-04-26 16:44:53.886358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_scim_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-26 16:44:53.890358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_scim_provider_list.py
+-rw-r--r--   0        0        0     3356 2024-04-26 16:44:53.894358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_scim_source_group_list.py
+-rw-r--r--   0        0        0     3315 2024-04-26 16:44:53.898358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_scim_source_list.py
+-rw-r--r--   0        0        0     3348 2024-04-26 16:44:53.902358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_scim_source_user_list.py
+-rw-r--r--   0        0        0     3331 2024-04-26 16:44:53.906358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_scope_mapping_list.py
+-rw-r--r--   0        0        0     3371 2024-04-26 16:44:53.910358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_service_connection_list.py
+-rw-r--r--   0        0        0     3307 2024-04-26 16:44:53.902358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_sms_device_list.py
+-rw-r--r--   0        0        0     3282 2024-04-26 16:44:53.914358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_source_list.py
+-rw-r--r--   0        0        0     3323 2024-04-26 16:44:53.918358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_source_stage_list.py
+-rw-r--r--   0        0        0     3274 2024-04-26 16:44:53.922358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_stage_list.py
+-rw-r--r--   0        0        0     3331 2024-04-26 16:44:53.922358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_static_device_list.py
+-rw-r--r--   0        0        0     3315 2024-04-26 16:44:53.926358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_system_task_list.py
+-rw-r--r--   0        0        0     3282 2024-04-26 16:44:53.934358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_tenant_list.py
+-rw-r--r--   0        0        0     3274 2024-04-26 16:44:53.938358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_token_list.py
+-rw-r--r--   0        0        0     3315 2024-04-26 16:44:53.942358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_token_model_list.py
+-rw-r--r--   0        0        0     3315 2024-04-26 16:44:53.930358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_totp_device_list.py
+-rw-r--r--   0        0        0     3461 2024-04-26 16:44:53.946358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_user_assigned_object_permission_list.py
+-rw-r--r--   0        0        0     3323 2024-04-26 16:44:53.950358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_user_consent_list.py
+-rw-r--r--   0        0        0     3356 2024-04-26 16:44:53.954358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_user_delete_stage_list.py
+-rw-r--r--   0        0        0     3266 2024-04-26 16:44:53.954358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_user_list.py
+-rw-r--r--   0        0        0     3348 2024-04-26 16:44:53.958358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_user_login_stage_list.py
+-rw-r--r--   0        0        0     3356 2024-04-26 16:44:53.962358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_user_logout_stage_list.py
+-rw-r--r--   0        0        0     3438 2024-04-26 16:44:53.966358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_user_o_auth_source_connection_list.py
+-rw-r--r--   0        0        0     3429 2024-04-26 16:44:53.970358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_user_saml_source_connection_list.py
+-rw-r--r--   0        0        0     3396 2024-04-26 16:44:53.970358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_user_source_connection_list.py
+-rw-r--r--   0        0        0     3348 2024-04-26 16:44:53.974358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_user_write_stage_list.py
+-rw-r--r--   0        0        0     3348 2024-04-26 16:44:53.978358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_web_authn_device_list.py
+-rw-r--r--   0        0        0     3381 2024-04-26 16:44:53.982358 authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_web_authn_device_type_list.py
+-rw-r--r--   0        0        0     3076 2024-04-26 16:44:53.986358 authentik_client-2024.4.1.post1714149882/authentik_client/models/pagination.py
+-rw-r--r--   0        0        0     4454 2024-04-26 16:44:53.990358 authentik_client-2024.4.1.post1714149882/authentik_client/models/password_challenge.py
+-rw-r--r--   0        0        0     2819 2024-04-26 16:44:53.990358 authentik_client-2024.4.1.post1714149882/authentik_client/models/password_challenge_response_request.py
+-rw-r--r--   0        0        0     4377 2024-04-26 16:44:53.994358 authentik_client-2024.4.1.post1714149882/authentik_client/models/password_expiry_policy.py
+-rw-r--r--   0        0        0     3099 2024-04-26 16:44:53.998358 authentik_client-2024.4.1.post1714149882/authentik_client/models/password_expiry_policy_request.py
+-rw-r--r--   0        0        0     6428 2024-04-26 16:44:54.002358 authentik_client-2024.4.1.post1714149882/authentik_client/models/password_policy.py
+-rw-r--r--   0        0        0     5239 2024-04-26 16:44:54.002358 authentik_client-2024.4.1.post1714149882/authentik_client/models/password_policy_request.py
+-rw-r--r--   0        0        0     5274 2024-04-26 16:44:54.006358 authentik_client-2024.4.1.post1714149882/authentik_client/models/password_stage.py
+-rw-r--r--   0        0        0     4264 2024-04-26 16:44:54.010358 authentik_client-2024.4.1.post1714149882/authentik_client/models/password_stage_request.py
+-rw-r--r--   0        0        0     4594 2024-04-26 16:44:54.014358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_application_request.py
+-rw-r--r--   0        0        0     4833 2024-04-26 16:44:54.014358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_authenticator_duo_stage_request.py
+-rw-r--r--   0        0        0     5701 2024-04-26 16:44:54.018358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_authenticator_sms_stage_request.py
+-rw-r--r--   0        0        0     4430 2024-04-26 16:44:54.022358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_authenticator_static_stage_request.py
+-rw-r--r--   0        0        0     4256 2024-04-26 16:44:54.026358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_authenticator_totp_stage_request.py
+-rw-r--r--   0        0        0     4931 2024-04-26 16:44:54.026358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_authenticator_validate_stage_request.py
+-rw-r--r--   0        0        0     5340 2024-04-26 16:44:54.030358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_authenticator_web_authn_stage_request.py
+-rw-r--r--   0        0        0     3246 2024-04-26 16:44:54.030358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_blueprint_instance_request.py
+-rw-r--r--   0        0        0     6352 2024-04-26 16:44:54.034358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_brand_request.py
+-rw-r--r--   0        0        0     3860 2024-04-26 16:44:54.034358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_captcha_stage_request.py
+-rw-r--r--   0        0        0     3051 2024-04-26 16:44:54.038358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_certificate_key_pair_request.py
+-rw-r--r--   0        0        0     2717 2024-04-26 16:44:54.038358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_connection_token_request.py
+-rw-r--r--   0        0        0     3607 2024-04-26 16:44:54.042358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_consent_stage_request.py
+-rw-r--r--   0        0        0     3268 2024-04-26 16:44:54.046358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_deny_stage_request.py
+-rw-r--r--   0        0        0     4149 2024-04-26 16:44:54.046358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_docker_service_connection_request.py
+-rw-r--r--   0        0        0     2801 2024-04-26 16:44:54.050358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_domain_request.py
+-rw-r--r--   0        0        0     3275 2024-04-26 16:44:54.050358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_dummy_policy_request.py
+-rw-r--r--   0        0        0     3270 2024-04-26 16:44:54.054358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_dummy_stage_request.py
+-rw-r--r--   0        0        0     2674 2024-04-26 16:44:54.058358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_duo_device_request.py
+-rw-r--r--   0        0        0     5159 2024-04-26 16:44:54.058358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_email_stage_request.py
+-rw-r--r--   0        0        0     3784 2024-04-26 16:44:54.062358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_endpoint_request.py
+-rw-r--r--   0        0        0     4845 2024-04-26 16:44:54.066358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_event_matcher_policy_request.py
+-rw-r--r--   0        0        0     4045 2024-04-26 16:44:54.070358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_event_request.py
+-rw-r--r--   0        0        0     3047 2024-04-26 16:44:54.074358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_expression_policy_request.py
+-rw-r--r--   0        0        0     4903 2024-04-26 16:44:54.078358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_flow_request.py
+-rw-r--r--   0        0        0     4055 2024-04-26 16:44:54.078358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_flow_stage_binding_request.py
+-rw-r--r--   0        0        0     3385 2024-04-26 16:44:54.082358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_group_request.py
+-rw-r--r--   0        0        0     6571 2024-04-26 16:44:54.086357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_identification_stage_request.py
+-rw-r--r--   0        0        0     3985 2024-04-26 16:44:54.090358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_invitation_request.py
+-rw-r--r--   0        0        0     3565 2024-04-26 16:44:54.094358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_invitation_stage_request.py
+-rw-r--r--   0        0        0     3492 2024-04-26 16:44:54.098358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_kubernetes_service_connection_request.py
+-rw-r--r--   0        0        0     3550 2024-04-26 16:44:54.102357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_ldap_property_mapping_request.py
+-rw-r--r--   0        0        0     6254 2024-04-26 16:44:54.102357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_ldap_provider_request.py
+-rw-r--r--   0        0        0     9697 2024-04-26 16:44:54.106357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_ldap_source_request.py
+-rw-r--r--   0        0        0     2557 2024-04-26 16:44:54.106357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_license_request.py
+-rw-r--r--   0        0        0     2879 2024-04-26 16:44:54.110357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_notification_request.py
+-rw-r--r--   0        0        0     3587 2024-04-26 16:44:54.110357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_notification_rule_request.py
+-rw-r--r--   0        0        0     3538 2024-04-26 16:44:54.114358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_notification_transport_request.py
+-rw-r--r--   0        0        0     2782 2024-04-26 16:44:54.118358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_notification_webhook_mapping_request.py
+-rw-r--r--   0        0        0     6716 2024-04-26 16:44:54.118358 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_o_auth2_provider_request.py
+-rw-r--r--   0        0        0     8185 2024-04-26 16:44:54.122357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_o_auth_source_request.py
+-rw-r--r--   0        0        0     4139 2024-04-26 16:44:54.126357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_outpost_request.py
+-rw-r--r--   0        0        0     3154 2024-04-26 16:44:54.130357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_password_expiry_policy_request.py
+-rw-r--r--   0        0        0     5277 2024-04-26 16:44:54.134357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_password_policy_request.py
+-rw-r--r--   0        0        0     4326 2024-04-26 16:44:54.138357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_password_stage_request.py
+-rw-r--r--   0        0        0     2922 2024-04-26 16:44:54.138357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_permission_assign_request.py
+-rw-r--r--   0        0        0     2784 2024-04-26 16:44:54.142357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_plex_source_connection_request.py
+-rw-r--r--   0        0        0     5905 2024-04-26 16:44:54.146357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_plex_source_request.py
+-rw-r--r--   0        0        0     4286 2024-04-26 16:44:54.150357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_policy_binding_request.py
+-rw-r--r--   0        0        0     5023 2024-04-26 16:44:54.154357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_prompt_request.py
+-rw-r--r--   0        0        0     3406 2024-04-26 16:44:54.154357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_prompt_stage_request.py
+-rw-r--r--   0        0        0     6907 2024-04-26 16:44:54.158357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_proxy_provider_request.py
+-rw-r--r--   0        0        0     3495 2024-04-26 16:44:54.158357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_rac_property_mapping_request.py
+-rw-r--r--   0        0        0     4413 2024-04-26 16:44:54.162357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_rac_provider_request.py
+-rw-r--r--   0        0        0     4563 2024-04-26 16:44:54.162357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_radius_provider_request.py
+-rw-r--r--   0        0        0     3276 2024-04-26 16:44:54.166357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_reputation_policy_request.py
+-rw-r--r--   0        0        0     2565 2024-04-26 16:44:54.166357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_role_request.py
+-rw-r--r--   0        0        0     3901 2024-04-26 16:44:54.170357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_saml_property_mapping_request.py
+-rw-r--r--   0        0        0     7539 2024-04-26 16:44:54.174357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_saml_provider_request.py
+-rw-r--r--   0        0        0     8676 2024-04-26 16:44:54.178357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_saml_source_request.py
+-rw-r--r--   0        0        0     3364 2024-04-26 16:44:54.178357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_scim_mapping_request.py
+-rw-r--r--   0        0        0     3888 2024-04-26 16:44:54.182357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_scim_provider_request.py
+-rw-r--r--   0        0        0     3095 2024-04-26 16:44:54.182357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_scim_source_group_request.py
+-rw-r--r--   0        0        0     3829 2024-04-26 16:44:54.186357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_scim_source_request.py
+-rw-r--r--   0        0        0     3098 2024-04-26 16:44:54.186357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_scim_source_user_request.py
+-rw-r--r--   0        0        0     3819 2024-04-26 16:44:54.194357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_scope_mapping_request.py
+-rw-r--r--   0        0        0     5079 2024-04-26 16:44:54.194357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_settings_request.py
+-rw-r--r--   0        0        0     2674 2024-04-26 16:44:54.190357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_sms_device_request.py
+-rw-r--r--   0        0        0     3562 2024-04-26 16:44:54.202357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_source_stage_request.py
+-rw-r--r--   0        0        0     2686 2024-04-26 16:44:54.206357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_static_device_request.py
+-rw-r--r--   0        0        0     2820 2024-04-26 16:44:54.210357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_tenant_request.py
+-rw-r--r--   0        0        0     4419 2024-04-26 16:44:54.210357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_token_request.py
+-rw-r--r--   0        0        0     2678 2024-04-26 16:44:54.206357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_totp_device_request.py
+-rw-r--r--   0        0        0     3167 2024-04-26 16:44:54.214357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_user_delete_stage_request.py
+-rw-r--r--   0        0        0     4766 2024-04-26 16:44:54.218357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_user_login_stage_request.py
+-rw-r--r--   0        0        0     3167 2024-04-26 16:44:54.218357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_user_logout_stage_request.py
+-rw-r--r--   0        0        0     3109 2024-04-26 16:44:54.222357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_user_o_auth_source_connection_request.py
+-rw-r--r--   0        0        0     3934 2024-04-26 16:44:54.226357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_user_request.py
+-rw-r--r--   0        0        0     2733 2024-04-26 16:44:54.226357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_user_saml_source_connection_request.py
+-rw-r--r--   0        0        0     4450 2024-04-26 16:44:54.230357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_user_write_stage_request.py
+-rw-r--r--   0        0        0     2625 2024-04-26 16:44:54.230357 authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_web_authn_device_request.py
+-rw-r--r--   0        0        0     3548 2024-04-26 16:44:54.234357 authentik_client-2024.4.1.post1714149882/authentik_client/models/permission.py
+-rw-r--r--   0        0        0     2884 2024-04-26 16:44:54.238357 authentik_client-2024.4.1.post1714149882/authentik_client/models/permission_assign_request.py
+-rw-r--r--   0        0        0     4315 2024-04-26 16:44:54.238357 authentik_client-2024.4.1.post1714149882/authentik_client/models/plex_authentication_challenge.py
+-rw-r--r--   0        0        0     2726 2024-04-26 16:44:54.242357 authentik_client-2024.4.1.post1714149882/authentik_client/models/plex_authentication_challenge_response_request.py
+-rw-r--r--   0        0        0     7752 2024-04-26 16:44:54.246357 authentik_client-2024.4.1.post1714149882/authentik_client/models/plex_source.py
+-rw-r--r--   0        0        0     3265 2024-04-26 16:44:54.246357 authentik_client-2024.4.1.post1714149882/authentik_client/models/plex_source_connection.py
+-rw-r--r--   0        0        0     2719 2024-04-26 16:44:54.250357 authentik_client-2024.4.1.post1714149882/authentik_client/models/plex_source_connection_request.py
+-rw-r--r--   0        0        0     5760 2024-04-26 16:44:54.254357 authentik_client-2024.4.1.post1714149882/authentik_client/models/plex_source_request.py
+-rw-r--r--   0        0        0     2576 2024-04-26 16:44:54.254357 authentik_client-2024.4.1.post1714149882/authentik_client/models/plex_token_redeem_request.py
+-rw-r--r--   0        0        0     4055 2024-04-26 16:44:54.258357 authentik_client-2024.4.1.post1714149882/authentik_client/models/policy.py
+-rw-r--r--   0        0        0     5643 2024-04-26 16:44:54.262357 authentik_client-2024.4.1.post1714149882/authentik_client/models/policy_binding.py
+-rw-r--r--   0        0        0     4231 2024-04-26 16:44:54.262357 authentik_client-2024.4.1.post1714149882/authentik_client/models/policy_binding_request.py
+-rw-r--r--   0        0        0      711 2024-04-26 16:44:54.266357 authentik_client-2024.4.1.post1714149882/authentik_client/models/policy_engine_mode.py
+-rw-r--r--   0        0        0     2817 2024-04-26 16:44:54.266357 authentik_client-2024.4.1.post1714149882/authentik_client/models/policy_request.py
+-rw-r--r--   0        0        0     2583 2024-04-26 16:44:54.270357 authentik_client-2024.4.1.post1714149882/authentik_client/models/policy_test_request.py
+-rw-r--r--   0        0        0     3281 2024-04-26 16:44:54.270357 authentik_client-2024.4.1.post1714149882/authentik_client/models/policy_test_result.py
+-rw-r--r--   0        0        0     4885 2024-04-26 16:44:54.274357 authentik_client-2024.4.1.post1714149882/authentik_client/models/prompt.py
+-rw-r--r--   0        0        0     4649 2024-04-26 16:44:54.274357 authentik_client-2024.4.1.post1714149882/authentik_client/models/prompt_challenge.py
+-rw-r--r--   0        0        0     3325 2024-04-26 16:44:54.278357 authentik_client-2024.4.1.post1714149882/authentik_client/models/prompt_challenge_response_request.py
+-rw-r--r--   0        0        0     4927 2024-04-26 16:44:54.282357 authentik_client-2024.4.1.post1714149882/authentik_client/models/prompt_request.py
+-rw-r--r--   0        0        0     4321 2024-04-26 16:44:54.282357 authentik_client-2024.4.1.post1714149882/authentik_client/models/prompt_stage.py
+-rw-r--r--   0        0        0     3351 2024-04-26 16:44:54.286357 authentik_client-2024.4.1.post1714149882/authentik_client/models/prompt_stage_request.py
+-rw-r--r--   0        0        0     1185 2024-04-26 16:44:54.286357 authentik_client-2024.4.1.post1714149882/authentik_client/models/prompt_type_enum.py
+-rw-r--r--   0        0        0     4264 2024-04-26 16:44:54.286357 authentik_client-2024.4.1.post1714149882/authentik_client/models/property_mapping.py
+-rw-r--r--   0        0        0     2610 2024-04-26 16:44:54.290357 authentik_client-2024.4.1.post1714149882/authentik_client/models/property_mapping_preview.py
+-rw-r--r--   0        0        0     2744 2024-04-26 16:44:54.290357 authentik_client-2024.4.1.post1714149882/authentik_client/models/property_mapping_test_result.py
+-rw-r--r--   0        0        0      715 2024-04-26 16:44:54.294357 authentik_client-2024.4.1.post1714149882/authentik_client/models/protocol_enum.py
+-rw-r--r--   0        0        0     5722 2024-04-26 16:44:54.294357 authentik_client-2024.4.1.post1714149882/authentik_client/models/provider.py
+-rw-r--r--   0        0        0      713 2024-04-26 16:44:54.298357 authentik_client-2024.4.1.post1714149882/authentik_client/models/provider_enum.py
+-rw-r--r--   0        0        0     1314 2024-04-26 16:44:54.298357 authentik_client-2024.4.1.post1714149882/authentik_client/models/provider_model_enum.py
+-rw-r--r--   0        0        0     3397 2024-04-26 16:44:54.298357 authentik_client-2024.4.1.post1714149882/authentik_client/models/provider_request.py
+-rw-r--r--   0        0        0     1009 2024-04-26 16:44:54.302357 authentik_client-2024.4.1.post1714149882/authentik_client/models/provider_type_enum.py
+-rw-r--r--   0        0        0      754 2024-04-26 16:44:54.302357 authentik_client-2024.4.1.post1714149882/authentik_client/models/proxy_mode.py
+-rw-r--r--   0        0        0     7819 2024-04-26 16:44:54.302357 authentik_client-2024.4.1.post1714149882/authentik_client/models/proxy_outpost_config.py
+-rw-r--r--   0        0        0     9552 2024-04-26 16:44:54.306357 authentik_client-2024.4.1.post1714149882/authentik_client/models/proxy_provider.py
+-rw-r--r--   0        0        0     6828 2024-04-26 16:44:54.306357 authentik_client-2024.4.1.post1714149882/authentik_client/models/proxy_provider_request.py
+-rw-r--r--   0        0        0     4407 2024-04-26 16:44:54.310357 authentik_client-2024.4.1.post1714149882/authentik_client/models/rac_property_mapping.py
+-rw-r--r--   0        0        0     3440 2024-04-26 16:44:54.310357 authentik_client-2024.4.1.post1714149882/authentik_client/models/rac_property_mapping_request.py
+-rw-r--r--   0        0        0     6813 2024-04-26 16:44:54.314357 authentik_client-2024.4.1.post1714149882/authentik_client/models/rac_provider.py
+-rw-r--r--   0        0        0     4351 2024-04-26 16:44:54.314357 authentik_client-2024.4.1.post1714149882/authentik_client/models/rac_provider_request.py
+-rw-r--r--   0        0        0     3833 2024-04-26 16:44:54.318357 authentik_client-2024.4.1.post1714149882/authentik_client/models/radius_outpost_config.py
+-rw-r--r--   0        0        0     6924 2024-04-26 16:44:54.318357 authentik_client-2024.4.1.post1714149882/authentik_client/models/radius_provider.py
+-rw-r--r--   0        0        0     4501 2024-04-26 16:44:54.322357 authentik_client-2024.4.1.post1714149882/authentik_client/models/radius_provider_request.py
+-rw-r--r--   0        0        0     4184 2024-04-26 16:44:54.322357 authentik_client-2024.4.1.post1714149882/authentik_client/models/redirect_challenge.py
+-rw-r--r--   0        0        0     3642 2024-04-26 16:44:54.326357 authentik_client-2024.4.1.post1714149882/authentik_client/models/reputation.py
+-rw-r--r--   0        0        0     4516 2024-04-26 16:44:54.326357 authentik_client-2024.4.1.post1714149882/authentik_client/models/reputation_policy.py
+-rw-r--r--   0        0        0     3238 2024-04-26 16:44:54.330357 authentik_client-2024.4.1.post1714149882/authentik_client/models/reputation_policy_request.py
+-rw-r--r--   0        0        0      795 2024-04-26 16:44:54.330357 authentik_client-2024.4.1.post1714149882/authentik_client/models/resident_key_requirement_enum.py
+-rw-r--r--   0        0        0     2618 2024-04-26 16:44:54.330357 authentik_client-2024.4.1.post1714149882/authentik_client/models/role.py
+-rw-r--r--   0        0        0     3333 2024-04-26 16:44:54.334357 authentik_client-2024.4.1.post1714149882/authentik_client/models/role_assigned_object_permission.py
+-rw-r--r--   0        0        0     3293 2024-04-26 16:44:54.334357 authentik_client-2024.4.1.post1714149882/authentik_client/models/role_object_permission.py
+-rw-r--r--   0        0        0     2517 2024-04-26 16:44:54.338357 authentik_client-2024.4.1.post1714149882/authentik_client/models/role_request.py
+-rw-r--r--   0        0        0     2712 2024-04-26 16:44:54.338357 authentik_client-2024.4.1.post1714149882/authentik_client/models/saml_metadata.py
+-rw-r--r--   0        0        0     4718 2024-04-26 16:44:54.342357 authentik_client-2024.4.1.post1714149882/authentik_client/models/saml_property_mapping.py
+-rw-r--r--   0        0        0     3829 2024-04-26 16:44:54.346357 authentik_client-2024.4.1.post1714149882/authentik_client/models/saml_property_mapping_request.py
+-rw-r--r--   0        0        0    11056 2024-04-26 16:44:54.350357 authentik_client-2024.4.1.post1714149882/authentik_client/models/saml_provider.py
+-rw-r--r--   0        0        0     7460 2024-04-26 16:44:54.350357 authentik_client-2024.4.1.post1714149882/authentik_client/models/saml_provider_request.py
+-rw-r--r--   0        0        0    10563 2024-04-26 16:44:54.354357 authentik_client-2024.4.1.post1714149882/authentik_client/models/saml_source.py
+-rw-r--r--   0        0        0     8507 2024-04-26 16:44:54.358357 authentik_client-2024.4.1.post1714149882/authentik_client/models/saml_source_request.py
+-rw-r--r--   0        0        0     4248 2024-04-26 16:44:54.362357 authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_mapping.py
+-rw-r--r--   0        0        0     3309 2024-04-26 16:44:54.366357 authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_mapping_request.py
+-rw-r--r--   0        0        0     5454 2024-04-26 16:44:54.366357 authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_provider.py
+-rw-r--r--   0        0        0     3802 2024-04-26 16:44:54.370357 authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_provider_request.py
+-rw-r--r--   0        0        0     5999 2024-04-26 16:44:54.374357 authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_source.py
+-rw-r--r--   0        0        0     3369 2024-04-26 16:44:54.374357 authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_source_group.py
+-rw-r--r--   0        0        0     3023 2024-04-26 16:44:54.378357 authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_source_group_request.py
+-rw-r--r--   0        0        0     3708 2024-04-26 16:44:54.382357 authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_source_request.py
+-rw-r--r--   0        0        0     3370 2024-04-26 16:44:54.386357 authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_source_user.py
+-rw-r--r--   0        0        0     3026 2024-04-26 16:44:54.386357 authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_source_user_request.py
+-rw-r--r--   0        0        0     3131 2024-04-26 16:44:54.390357 authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_sync_status.py
+-rw-r--r--   0        0        0     4629 2024-04-26 16:44:54.398357 authentik_client-2024.4.1.post1714149882/authentik_client/models/scope_mapping.py
+-rw-r--r--   0        0        0     3740 2024-04-26 16:44:54.402357 authentik_client-2024.4.1.post1714149882/authentik_client/models/scope_mapping_request.py
+-rw-r--r--   0        0        0     2738 2024-04-26 16:44:54.406357 authentik_client-2024.4.1.post1714149882/authentik_client/models/selectable_stage.py
+-rw-r--r--   0        0        0     3773 2024-04-26 16:44:54.406357 authentik_client-2024.4.1.post1714149882/authentik_client/models/service_connection.py
+-rw-r--r--   0        0        0     2776 2024-04-26 16:44:54.410357 authentik_client-2024.4.1.post1714149882/authentik_client/models/service_connection_request.py
+-rw-r--r--   0        0        0     2731 2024-04-26 16:44:54.414357 authentik_client-2024.4.1.post1714149882/authentik_client/models/service_connection_state.py
+-rw-r--r--   0        0        0     3178 2024-04-26 16:44:54.418357 authentik_client-2024.4.1.post1714149882/authentik_client/models/session_user.py
+-rw-r--r--   0        0        0     4931 2024-04-26 16:44:54.418357 authentik_client-2024.4.1.post1714149882/authentik_client/models/settings.py
+-rw-r--r--   0        0        0     5058 2024-04-26 16:44:54.422357 authentik_client-2024.4.1.post1714149882/authentik_client/models/settings_request.py
+-rw-r--r--   0        0        0      733 2024-04-26 16:44:54.422357 authentik_client-2024.4.1.post1714149882/authentik_client/models/severity_enum.py
+-rw-r--r--   0        0        0     4175 2024-04-26 16:44:54.426357 authentik_client-2024.4.1.post1714149882/authentik_client/models/shell_challenge.py
+-rw-r--r--   0        0        0     1492 2024-04-26 16:44:54.426357 authentik_client-2024.4.1.post1714149882/authentik_client/models/signature_algorithm_enum.py
+-rw-r--r--   0        0        0     2906 2024-04-26 16:44:54.394357 authentik_client-2024.4.1.post1714149882/authentik_client/models/sms_device.py
+-rw-r--r--   0        0        0     2619 2024-04-26 16:44:54.398357 authentik_client-2024.4.1.post1714149882/authentik_client/models/sms_device_request.py
+-rw-r--r--   0        0        0     6945 2024-04-26 16:44:54.430357 authentik_client-2024.4.1.post1714149882/authentik_client/models/source.py
+-rw-r--r--   0        0        0     4836 2024-04-26 16:44:54.430357 authentik_client-2024.4.1.post1714149882/authentik_client/models/source_request.py
+-rw-r--r--   0        0        0     4438 2024-04-26 16:44:54.434357 authentik_client-2024.4.1.post1714149882/authentik_client/models/source_stage.py
+-rw-r--r--   0        0        0     3507 2024-04-26 16:44:54.434357 authentik_client-2024.4.1.post1714149882/authentik_client/models/source_stage_request.py
+-rw-r--r--   0        0        0     5355 2024-04-26 16:44:54.438357 authentik_client-2024.4.1.post1714149882/authentik_client/models/source_type.py
+-rw-r--r--   0        0        0      714 2024-04-26 16:44:54.442357 authentik_client-2024.4.1.post1714149882/authentik_client/models/sp_binding_enum.py
+-rw-r--r--   0        0        0     4070 2024-04-26 16:44:54.442357 authentik_client-2024.4.1.post1714149882/authentik_client/models/stage.py
+-rw-r--r--   0        0        0     3437 2024-04-26 16:44:54.446357 authentik_client-2024.4.1.post1714149882/authentik_client/models/stage_prompt.py
+-rw-r--r--   0        0        0     3089 2024-04-26 16:44:54.446357 authentik_client-2024.4.1.post1714149882/authentik_client/models/stage_request.py
+-rw-r--r--   0        0        0     3385 2024-04-26 16:44:54.450357 authentik_client-2024.4.1.post1714149882/authentik_client/models/static_device.py
+-rw-r--r--   0        0        0     2631 2024-04-26 16:44:54.454357 authentik_client-2024.4.1.post1714149882/authentik_client/models/static_device_request.py
+-rw-r--r--   0        0        0     2546 2024-04-26 16:44:54.454357 authentik_client-2024.4.1.post1714149882/authentik_client/models/static_device_token.py
+-rw-r--r--   0        0        0     2581 2024-04-26 16:44:54.458357 authentik_client-2024.4.1.post1714149882/authentik_client/models/static_device_token_request.py
+-rw-r--r--   0        0        0      846 2024-04-26 16:44:54.458357 authentik_client-2024.4.1.post1714149882/authentik_client/models/sub_mode_enum.py
+-rw-r--r--   0        0        0     4463 2024-04-26 16:44:54.462357 authentik_client-2024.4.1.post1714149882/authentik_client/models/system_info.py
+-rw-r--r--   0        0        0     2934 2024-04-26 16:44:54.462357 authentik_client-2024.4.1.post1714149882/authentik_client/models/system_info_runtime.py
+-rw-r--r--   0        0        0     4286 2024-04-26 16:44:54.466357 authentik_client-2024.4.1.post1714149882/authentik_client/models/system_task.py
+-rw-r--r--   0        0        0      789 2024-04-26 16:44:54.466357 authentik_client-2024.4.1.post1714149882/authentik_client/models/system_task_status_enum.py
+-rw-r--r--   0        0        0     2872 2024-04-26 16:44:54.470357 authentik_client-2024.4.1.post1714149882/authentik_client/models/tenant.py
+-rw-r--r--   0        0        0     2589 2024-04-26 16:44:54.474357 authentik_client-2024.4.1.post1714149882/authentik_client/models/tenant_admin_group_request_request.py
+-rw-r--r--   0        0        0     2705 2024-04-26 16:44:54.474357 authentik_client-2024.4.1.post1714149882/authentik_client/models/tenant_recovery_key_request_request.py
+-rw-r--r--   0        0        0     2599 2024-04-26 16:44:54.478356 authentik_client-2024.4.1.post1714149882/authentik_client/models/tenant_recovery_key_response.py
+-rw-r--r--   0        0        0     2765 2024-04-26 16:44:54.482357 authentik_client-2024.4.1.post1714149882/authentik_client/models/tenant_request.py
+-rw-r--r--   0        0        0     4802 2024-04-26 16:44:54.486357 authentik_client-2024.4.1.post1714149882/authentik_client/models/token.py
+-rw-r--r--   0        0        0     4198 2024-04-26 16:44:54.486357 authentik_client-2024.4.1.post1714149882/authentik_client/models/token_model.py
+-rw-r--r--   0        0        0     4329 2024-04-26 16:44:54.490357 authentik_client-2024.4.1.post1714149882/authentik_client/models/token_request.py
+-rw-r--r--   0        0        0     2521 2024-04-26 16:44:54.490357 authentik_client-2024.4.1.post1714149882/authentik_client/models/token_set_key_request.py
+-rw-r--r--   0        0        0     2494 2024-04-26 16:44:54.494356 authentik_client-2024.4.1.post1714149882/authentik_client/models/token_view.py
+-rw-r--r--   0        0        0     2724 2024-04-26 16:44:54.466357 authentik_client-2024.4.1.post1714149882/authentik_client/models/totp_device.py
+-rw-r--r--   0        0        0     2623 2024-04-26 16:44:54.470357 authentik_client-2024.4.1.post1714149882/authentik_client/models/totp_device_request.py
+-rw-r--r--   0        0        0     3389 2024-04-26 16:44:54.498356 authentik_client-2024.4.1.post1714149882/authentik_client/models/transaction_application_request.py
+-rw-r--r--   0        0        0     2595 2024-04-26 16:44:54.502356 authentik_client-2024.4.1.post1714149882/authentik_client/models/transaction_application_response.py
+-rw-r--r--   0        0        0     2936 2024-04-26 16:44:54.506357 authentik_client-2024.4.1.post1714149882/authentik_client/models/type_create.py
+-rw-r--r--   0        0        0      730 2024-04-26 16:44:54.506357 authentik_client-2024.4.1.post1714149882/authentik_client/models/ui_theme_enum.py
+-rw-r--r--   0        0        0     2808 2024-04-26 16:44:54.510357 authentik_client-2024.4.1.post1714149882/authentik_client/models/used_by.py
+-rw-r--r--   0        0        0      795 2024-04-26 16:44:54.510357 authentik_client-2024.4.1.post1714149882/authentik_client/models/used_by_action_enum.py
+-rw-r--r--   0        0        0     5459 2024-04-26 16:44:54.514356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user.py
+-rw-r--r--   0        0        0     2458 2024-04-26 16:44:54.514356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_account_request.py
+-rw-r--r--   0        0        0     4946 2024-04-26 16:44:54.518356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_assigned_object_permission.py
+-rw-r--r--   0        0        0     3828 2024-04-26 16:44:54.518356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_consent.py
+-rw-r--r--   0        0        0      811 2024-04-26 16:44:54.522356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_creation_mode_enum.py
+-rw-r--r--   0        0        0     4110 2024-04-26 16:44:54.522356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_delete_stage.py
+-rw-r--r--   0        0        0     3129 2024-04-26 16:44:54.526357 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_delete_stage_request.py
+-rw-r--r--   0        0        0      735 2024-04-26 16:44:54.526357 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_fields_enum.py
+-rw-r--r--   0        0        0     3909 2024-04-26 16:44:54.530357 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_group.py
+-rw-r--r--   0        0        0     3193 2024-04-26 16:44:54.530357 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_group_request.py
+-rw-r--r--   0        0        0     4334 2024-04-26 16:44:54.534356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_login_challenge.py
+-rw-r--r--   0        0        0     2805 2024-04-26 16:44:54.538356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_login_challenge_response_request.py
+-rw-r--r--   0        0        0     5631 2024-04-26 16:44:54.538356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_login_stage.py
+-rw-r--r--   0        0        0     4728 2024-04-26 16:44:54.542356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_login_stage_request.py
+-rw-r--r--   0        0        0     4110 2024-04-26 16:44:54.546356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_logout_stage.py
+-rw-r--r--   0        0        0     3129 2024-04-26 16:44:54.546356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_logout_stage_request.py
+-rw-r--r--   0        0        0      853 2024-04-26 16:44:54.550356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_matching_mode_enum.py
+-rw-r--r--   0        0        0     4160 2024-04-26 16:44:54.550356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_metrics.py
+-rw-r--r--   0        0        0     3188 2024-04-26 16:44:54.554356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_o_auth_source_connection.py
+-rw-r--r--   0        0        0     3054 2024-04-26 16:44:54.554356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_o_auth_source_connection_request.py
+-rw-r--r--   0        0        0     3293 2024-04-26 16:44:54.558356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_object_permission.py
+-rw-r--r--   0        0        0     2557 2024-04-26 16:44:54.562356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_password_set_request.py
+-rw-r--r--   0        0        0     2491 2024-04-26 16:44:54.562356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_path.py
+-rw-r--r--   0        0        0     3872 2024-04-26 16:44:54.566356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_request.py
+-rw-r--r--   0        0        0     3107 2024-04-26 16:44:54.566356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_saml_source_connection.py
+-rw-r--r--   0        0        0     2668 2024-04-26 16:44:54.570356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_saml_source_connection_request.py
+-rw-r--r--   0        0        0     5465 2024-04-26 16:44:54.574356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_self.py
+-rw-r--r--   0        0        0     2629 2024-04-26 16:44:54.574356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_self_groups.py
+-rw-r--r--   0        0        0     3074 2024-04-26 16:44:54.578356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_service_account_request.py
+-rw-r--r--   0        0        0     2844 2024-04-26 16:44:54.578356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_service_account_response.py
+-rw-r--r--   0        0        0     2866 2024-04-26 16:44:54.582356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_setting.py
+-rw-r--r--   0        0        0     3245 2024-04-26 16:44:54.586356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_source_connection.py
+-rw-r--r--   0        0        0      817 2024-04-26 16:44:54.586356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_type_enum.py
+-rw-r--r--   0        0        0      777 2024-04-26 16:44:54.586356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_verification_enum.py
+-rw-r--r--   0        0        0     5382 2024-04-26 16:44:54.590356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_write_stage.py
+-rw-r--r--   0        0        0     4412 2024-04-26 16:44:54.594356 authentik_client-2024.4.1.post1714149882/authentik_client/models/user_write_stage_request.py
+-rw-r--r--   0        0        0     3197 2024-04-26 16:44:54.594356 authentik_client-2024.4.1.post1714149882/authentik_client/models/validation_error.py
+-rw-r--r--   0        0        0     3589 2024-04-26 16:44:54.598356 authentik_client-2024.4.1.post1714149882/authentik_client/models/version.py
+-rw-r--r--   0        0        0     3786 2024-04-26 16:44:54.598356 authentik_client-2024.4.1.post1714149882/authentik_client/models/web_authn_device.py
+-rw-r--r--   0        0        0     2577 2024-04-26 16:44:54.602356 authentik_client-2024.4.1.post1714149882/authentik_client/models/web_authn_device_request.py
+-rw-r--r--   0        0        0     2562 2024-04-26 16:44:54.606356 authentik_client-2024.4.1.post1714149882/authentik_client/models/web_authn_device_type.py
+-rw-r--r--   0        0        0     2669 2024-04-26 16:44:54.606356 authentik_client-2024.4.1.post1714149882/authentik_client/models/web_authn_device_type_request.py
+-rw-r--r--   0        0        0     2410 2024-04-26 16:44:54.610356 authentik_client-2024.4.1.post1714149882/authentik_client/models/workers.py
+-rw-r--r--   0        0        0        0 2024-04-26 16:44:55.758353 authentik_client-2024.4.1.post1714149882/authentik_client/py.typed
+-rw-r--r--   0        0        0     9196 2024-04-26 16:44:55.766353 authentik_client-2024.4.1.post1714149882/authentik_client/rest.py
+-rw-r--r--   0        0        0     1936 2024-04-26 16:44:55.754353 authentik_client-2024.4.1.post1714149882/pyproject.toml
+-rw-r--r--   0        0        0   144895 1970-01-01 00:00:00.000000 authentik_client-2024.4.1.post1714149882/PKG-INFO
```

### Comparing `authentik_client-2024.4.0.post1713978839/README.md` & `authentik_client-2024.4.1.post1714149882/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # authentik-client
 Making authentication simple.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2024.4.0
-- Package version: 2024.4.0-1713978839
+- API version: 2024.4.1
+- Package version: 2024.4.1-1714149882
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/__init__.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "2024.4.0-1713978839"
+__version__ = "2024.4.1-1714149882"
 
 # import apis into sdk package
 from authentik_client.api.admin_api import AdminApi
 from authentik_client.api.authenticators_api import AuthenticatorsApi
 from authentik_client.api.core_api import CoreApi
 from authentik_client.api.crypto_api import CryptoApi
 from authentik_client.api.enterprise_api import EnterpriseApi
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/__init__.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/admin_api.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/admin_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/authenticators_api.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/authenticators_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/core_api.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/core_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/crypto_api.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/crypto_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/enterprise_api.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/enterprise_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/events_api.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/events_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/flows_api.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/flows_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/managed_api.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/managed_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/oauth2_api.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/oauth2_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/outposts_api.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/outposts_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/policies_api.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/policies_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/propertymappings_api.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/propertymappings_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/providers_api.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/providers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/rac_api.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/rac_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/rbac_api.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/rbac_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/root_api.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/root_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/schema_api.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/schema_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/sources_api.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/sources_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/stages_api.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/stages_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api/tenants_api.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api/tenants_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api_client.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2024.4.0-1713978839/python'
+        self.user_agent = 'OpenAPI-Generator/2024.4.1-1714149882/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/api_response.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/api_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/configuration.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -374,16 +374,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2024.4.0\n"\
-               "SDK Package Version: 2024.4.0-1713978839".\
+               "Version of the API: 2024.4.1\n"\
+               "SDK Package Version: 2024.4.1-1714149882".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/exceptions.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/__init__.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/access_denied_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/access_denied_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/app.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/app_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/app_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/apple_challenge_response_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/apple_challenge_response_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/apple_login_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/apple_login_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/application.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/application_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/application_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/auth_mode_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/auth_mode_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/auth_type_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/auth_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticated_session.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticated_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticated_session_asn.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticated_session_asn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticated_session_geo_ip.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticated_session_geo_ip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticated_session_user_agent.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticated_session_user_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticated_session_user_agent_device.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticated_session_user_agent_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticated_session_user_agent_os.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticated_session_user_agent_os.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticated_session_user_agent_user_agent.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticated_session_user_agent_user_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authentication_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authentication_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_attachment_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_attachment_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_duo_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_duo_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_duo_challenge_response_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_duo_challenge_response_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_duo_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_duo_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_duo_stage_device_import_response.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_duo_stage_device_import_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_duo_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_duo_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_sms_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_sms_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_sms_challenge_response_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_sms_challenge_response_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_sms_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_sms_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_sms_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_sms_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_static_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_static_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_static_challenge_response_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_static_challenge_response_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_static_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_static_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_static_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_static_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_totp_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_totp_challenge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_totp_challenge_response_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_totp_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_totp_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_totp_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_totp_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_totp_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_validate_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_validate_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_validate_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_validate_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_validation_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_validation_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_validation_challenge_response_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_validation_challenge_response_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_web_authn_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_web_authn_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_web_authn_challenge_response_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_web_authn_challenge_response_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_web_authn_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_web_authn_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/authenticator_web_authn_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/authenticator_web_authn_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/auto_submit_challenge_response_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/auto_submit_challenge_response_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/autosubmit_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/autosubmit_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/backends_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/backends_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/binding_type_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/binding_type_enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/blueprint_file.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/blueprint_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/blueprint_instance.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/blueprint_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/blueprint_instance_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/blueprint_instance_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/blueprint_instance_status_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/blueprint_instance_status_enum.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/brand.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/brand.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/brand_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/brand_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/cache.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/capabilities_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/capabilities_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/captcha_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/captcha_challenge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/captcha_challenge_response_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/captcha_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/captcha_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/captcha_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/captcha_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/captcha_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/certificate_data.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/certificate_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/certificate_generation_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/certificate_generation_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/certificate_key_pair.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/certificate_key_pair.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/certificate_key_pair_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/certificate_key_pair_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/challenge_choices.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/challenge_choices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/challenge_types.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/challenge_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/client_type_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/client_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/config.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/connection_token.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/connection_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/connection_token_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/connection_token_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/consent_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/consent_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/consent_challenge_response_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/consent_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/consent_permission.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/consent_permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/consent_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/consent_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/consent_stage_mode_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/consent_stage_mode_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/consent_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/consent_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/contextual_flow_info.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/contextual_flow_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/contextual_flow_info_layout_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/contextual_flow_info_layout_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/coordinate.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/coordinate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/current_brand.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/current_brand.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/denied_action_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/denied_action_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/deny_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/deny_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/deny_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/deny_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/device.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/device_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/device_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/device_challenge_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/device_challenge_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/device_classes_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/device_classes_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/digest_algorithm_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/digest_algorithm_enum.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/digits_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/digits_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/docker_service_connection.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/docker_service_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/docker_service_connection_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/docker_service_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/domain.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/domain_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/domain_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/dummy_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/dummy_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/dummy_challenge_response_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/dummy_challenge_response_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/dummy_policy.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/dummy_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/dummy_policy_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/dummy_policy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/dummy_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/dummy_stage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/dummy_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/dummy_stage_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/duo_device.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/duo_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/duo_device_enrollment_status.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/duo_device_enrollment_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/duo_device_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/duo_device_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/duo_response_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/duo_response_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/email_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/email_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/email_challenge_response_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/email_challenge_response_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/email_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/email_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/email_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/email_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/endpoint.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/endpoint_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/endpoint_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/error_detail.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/error_detail.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/error_reporting_config.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/error_reporting_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/event.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/event_actions.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/event_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/event_matcher_policy.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/event_matcher_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/event_matcher_policy_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/event_matcher_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/event_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/event_top_per_user.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/event_top_per_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/expiring_base_grant_model.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/expiring_base_grant_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/expression_policy.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/expression_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/expression_policy_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/expression_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/extra_role_object_permission.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/extra_role_object_permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/extra_user_object_permission.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/extra_user_object_permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/file_path_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/file_path_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/flow.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_challenge_response_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_designation_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_designation_enum.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_diagram.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/link.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -19,20 +19,20 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class FlowDiagram(BaseModel):
+class Link(BaseModel):
     """
-    response of the flow's diagram action
+    Returns a single link
     """ # noqa: E501
-    diagram: StrictStr
-    __properties: ClassVar[List[str]] = ["diagram"]
+    link: StrictStr
+    __properties: ClassVar[List[str]] = ["link"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,47 +44,45 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of FlowDiagram from a JSON string"""
+        """Create an instance of Link from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
-        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "diagram",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of FlowDiagram from a dict"""
+        """Create an instance of Link from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "diagram": obj.get("diagram")
+            "link": obj.get("link")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_error_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_error_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_import_result.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_import_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_inspection.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_inspection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_inspector_plan.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_inspector_plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_layout_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_layout_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_set.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_set_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_set_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_stage_binding.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_stage_binding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/flow_stage_binding_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/flow_stage_binding_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/footer_link.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/footer_link.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/generic_error.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/generic_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/geoip_binding_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/geoip_binding_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/group.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/group_member.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/group_member.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/group_member_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/group_member_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/group_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/identification_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/identification_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/identification_challenge_response_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/identification_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/identification_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/identification_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/identification_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/identification_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/install_id.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/install_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/intent_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/intent_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/invalid_response_action_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/invalid_response_action_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/invitation.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/invitation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/invitation_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/invitation_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/invitation_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/invitation_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/invitation_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/invitation_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/issuer_mode_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/issuer_mode_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/kubernetes_service_connection.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/kubernetes_service_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/kubernetes_service_connection_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/kubernetes_service_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/ldap_debug.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/ldap_debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/ldap_outpost_config.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/ldap_outpost_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/ldap_property_mapping.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/ldap_property_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/ldap_property_mapping_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/ldap_property_mapping_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/ldap_provider.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/ldap_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/ldap_provider_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/ldap_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/ldap_source.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/ldap_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/ldap_source_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/ldap_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/ldap_sync_status.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/ldap_sync_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/ldapapi_access_mode.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/ldapapi_access_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/license.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/license.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/license_forecast.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/license_forecast.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/license_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/license_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/license_summary.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/license_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/link.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/token_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -19,20 +19,20 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Link(BaseModel):
+class TokenView(BaseModel):
     """
-    Returns a single link
+    Show token's current key
     """ # noqa: E501
-    link: StrictStr
-    __properties: ClassVar[List[str]] = ["link"]
+    key: StrictStr
+    __properties: ClassVar[List[str]] = ["key"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,45 +44,47 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Link from a JSON string"""
+        """Create an instance of TokenView from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
+        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
+            "key",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Link from a dict"""
+        """Create an instance of TokenView from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "link": obj.get("link")
+            "key": obj.get("key")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/log_event.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/log_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/log_level_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/log_level_enum.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/login_challenge_types.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/login_challenge_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/login_metrics.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/login_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/login_source.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/login_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/metadata.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/model_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/model_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/model_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/model_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/name_id_policy_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/name_id_policy_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/network_binding_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/network_binding_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/not_configured_action_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/not_configured_action_enum.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/notification.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/notification_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/notification_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/notification_rule.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/notification_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/notification_rule_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/notification_rule_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/notification_transport.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/notification_transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/notification_transport_mode_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/notification_transport_mode_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/notification_transport_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/notification_transport_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/notification_transport_test.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/notification_transport_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/notification_webhook_mapping.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/notification_webhook_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/notification_webhook_mapping_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/notification_webhook_mapping_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/o_auth2_provider.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/o_auth2_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/o_auth2_provider_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/o_auth2_provider_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/o_auth2_provider_setup_urls.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/o_auth2_provider_setup_urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/o_auth_device_code_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/o_auth_device_code_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/o_auth_device_code_challenge_response_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/o_auth_device_code_challenge_response_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/o_auth_device_code_finish_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/o_auth_device_code_finish_challenge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/o_auth_source.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/o_auth_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/o_auth_source_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/o_auth_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/open_id_connect_configuration.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/open_id_connect_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/outpost.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/outpost.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/outpost_default_config.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/outpost_default_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/outpost_health.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/outpost_health.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/outpost_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/outpost_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/outpost_type_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/outpost_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_application_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_application_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_authenticated_session_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_authenticated_session_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_authenticator_duo_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_authenticator_duo_stage_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_authenticator_sms_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_authenticator_sms_stage_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_authenticator_static_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_authenticator_static_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_authenticator_totp_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_authenticator_totp_stage_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_authenticator_validate_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_authenticator_validate_stage_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_authenticator_web_authn_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_authenticator_web_authn_stage_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_blueprint_instance_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_blueprint_instance_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_brand_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_brand_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_captcha_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_captcha_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_certificate_key_pair_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_certificate_key_pair_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_connection_token_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_connection_token_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_consent_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_consent_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_deny_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_deny_stage_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_docker_service_connection_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_docker_service_connection_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_domain_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_domain_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_dummy_policy_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_dummy_policy_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_dummy_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_dummy_stage_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_duo_device_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_duo_device_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_email_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_email_stage_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_endpoint_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_endpoint_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_event_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_event_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_event_matcher_policy_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_event_matcher_policy_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_expiring_base_grant_model_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_expiring_base_grant_model_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_expression_policy_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_expression_policy_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_extra_role_object_permission_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_extra_role_object_permission_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_extra_user_object_permission_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_extra_user_object_permission_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_flow_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_flow_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_flow_stage_binding_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_flow_stage_binding_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_group_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_group_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_identification_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_identification_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_invitation_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_invitation_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_invitation_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_invitation_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_kubernetes_service_connection_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_kubernetes_service_connection_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_ldap_outpost_config_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_ldap_outpost_config_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_ldap_property_mapping_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_ldap_property_mapping_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_ldap_provider_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_ldap_provider_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_ldap_source_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_ldap_source_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_license_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_license_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_notification_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_notification_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_notification_rule_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_notification_rule_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_notification_transport_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_notification_transport_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_notification_webhook_mapping_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_notification_webhook_mapping_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_o_auth2_provider_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_o_auth2_provider_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_o_auth_source_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_o_auth_source_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_outpost_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_outpost_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_password_expiry_policy_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_password_expiry_policy_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_password_policy_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_password_policy_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_password_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_password_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_permission_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_permission_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_plex_source_connection_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_plex_source_connection_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_plex_source_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_plex_source_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_policy_binding_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_policy_binding_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_policy_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_policy_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_prompt_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_prompt_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_prompt_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_prompt_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_property_mapping_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_property_mapping_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_provider_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_provider_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_proxy_outpost_config_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_proxy_outpost_config_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_proxy_provider_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_proxy_provider_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_rac_property_mapping_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_rac_property_mapping_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_rac_provider_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_rac_provider_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_radius_outpost_config_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_radius_outpost_config_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_radius_provider_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_radius_provider_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_reputation_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_reputation_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_reputation_policy_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_reputation_policy_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_role_assigned_object_permission_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_role_assigned_object_permission_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_role_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_role_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_saml_property_mapping_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_saml_property_mapping_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_saml_provider_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_saml_provider_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_saml_source_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_saml_source_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_scim_mapping_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_scim_mapping_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_scim_provider_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_scim_provider_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_scim_source_group_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_scim_source_group_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_scim_source_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_scim_source_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_scim_source_user_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_scim_source_user_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_scope_mapping_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_scope_mapping_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_service_connection_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_service_connection_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_sms_device_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_sms_device_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_source_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_source_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_source_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_source_stage_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_stage_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_static_device_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_static_device_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_system_task_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_system_task_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_tenant_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_tenant_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_token_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_token_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_token_model_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_token_model_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_totp_device_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_totp_device_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_user_assigned_object_permission_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_user_assigned_object_permission_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_user_consent_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_user_consent_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_user_delete_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_user_delete_stage_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_user_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_user_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_user_login_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_user_login_stage_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_user_logout_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_user_logout_stage_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_user_o_auth_source_connection_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_user_o_auth_source_connection_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_user_saml_source_connection_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_user_saml_source_connection_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_user_source_connection_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_user_source_connection_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_user_write_stage_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_user_write_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_web_authn_device_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_web_authn_device_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/paginated_web_authn_device_type_list.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/paginated_web_authn_device_type_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/pagination.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/password_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/password_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/password_challenge_response_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/password_challenge_response_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/password_expiry_policy.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/password_expiry_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/password_expiry_policy_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/password_expiry_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/password_policy.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/password_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/password_policy_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/password_policy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/password_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/password_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/password_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/password_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_application_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_application_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_authenticator_duo_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_authenticator_duo_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_authenticator_sms_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_authenticator_sms_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_authenticator_static_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_authenticator_static_stage_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_authenticator_totp_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_authenticator_totp_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_authenticator_validate_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_authenticator_validate_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_authenticator_web_authn_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_authenticator_web_authn_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_blueprint_instance_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_blueprint_instance_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_brand_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_brand_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_captcha_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_captcha_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_certificate_key_pair_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_certificate_key_pair_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_connection_token_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_connection_token_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_consent_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_consent_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_deny_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_deny_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_docker_service_connection_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_docker_service_connection_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_domain_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_domain_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_dummy_policy_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_dummy_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_dummy_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_dummy_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_duo_device_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_duo_device_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_email_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_email_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_endpoint_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_endpoint_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_event_matcher_policy_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_event_matcher_policy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_event_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_expression_policy_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_expression_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_flow_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_flow_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_flow_stage_binding_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_flow_stage_binding_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_group_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_group_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_identification_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_identification_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_invitation_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_invitation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_invitation_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_invitation_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_kubernetes_service_connection_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_kubernetes_service_connection_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_ldap_property_mapping_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_ldap_property_mapping_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_ldap_provider_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_ldap_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_ldap_source_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_ldap_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_license_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_license_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_notification_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_notification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_notification_rule_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_notification_rule_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_notification_transport_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_notification_transport_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_notification_webhook_mapping_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_notification_webhook_mapping_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_o_auth2_provider_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_o_auth2_provider_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_o_auth_source_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_o_auth_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_outpost_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_outpost_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_password_expiry_policy_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_password_expiry_policy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_password_policy_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_password_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_password_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_password_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_permission_assign_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_permission_assign_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_plex_source_connection_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_plex_source_connection_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_plex_source_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_plex_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_policy_binding_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_policy_binding_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_prompt_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_prompt_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_prompt_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_prompt_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_proxy_provider_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_proxy_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_rac_property_mapping_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_rac_property_mapping_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_rac_provider_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_rac_provider_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_radius_provider_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_radius_provider_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_reputation_policy_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_reputation_policy_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_role_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_role_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_saml_property_mapping_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_saml_property_mapping_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_saml_provider_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_saml_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_saml_source_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_saml_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_scim_mapping_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_scim_mapping_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_scim_provider_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_scim_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_scim_source_group_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_scim_source_group_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_scim_source_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_scim_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_scim_source_user_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_scim_source_user_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_scope_mapping_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_scope_mapping_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_settings_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/settings_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -20,15 +20,15 @@
 
 from pydantic import BaseModel, ConfigDict, Field, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PatchedSettingsRequest(BaseModel):
+class SettingsRequest(BaseModel):
     """
     Settings Serializer
     """ # noqa: E501
     avatars: Optional[Annotated[str, Field(min_length=1, strict=True)]] = Field(default=None, description="Configure how authentik should show avatars for users.")
     default_user_change_name: Optional[StrictBool] = Field(default=None, description="Enable the ability for users to change their name.")
     default_user_change_email: Optional[StrictBool] = Field(default=None, description="Enable the ability for users to change their email address.")
     default_user_change_username: Optional[StrictBool] = Field(default=None, description="Enable the ability for users to change their username.")
@@ -54,15 +54,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PatchedSettingsRequest from a JSON string"""
+        """Create an instance of SettingsRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -84,15 +84,15 @@
         if self.footer_links is None and "footer_links" in self.model_fields_set:
             _dict['footer_links'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PatchedSettingsRequest from a dict"""
+        """Create an instance of SettingsRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_sms_device_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_sms_device_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_source_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_source_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_static_device_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_static_device_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_tenant_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_tenant_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_token_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_token_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_totp_device_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_totp_device_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_user_delete_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_user_delete_stage_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_user_login_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_user_login_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_user_logout_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_user_logout_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_user_o_auth_source_connection_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_user_o_auth_source_connection_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_user_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_user_saml_source_connection_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_user_saml_source_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_user_write_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_user_write_stage_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/patched_web_authn_device_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_web_authn_device_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/permission.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/permission_assign_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/permission_assign_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/plex_authentication_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/plex_authentication_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/plex_authentication_challenge_response_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/plex_authentication_challenge_response_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/plex_source.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/plex_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/plex_source_connection.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/plex_source_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/plex_source_connection_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/plex_source_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/plex_source_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/plex_source_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/plex_token_redeem_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/plex_token_redeem_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/policy.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/policy_binding.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/policy_binding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/policy_binding_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/policy_binding_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/policy_engine_mode.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/policy_engine_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/policy_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/policy_test_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/policy_test_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/policy_test_result.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/policy_test_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/prompt.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/prompt_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/prompt_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/prompt_challenge_response_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/prompt_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/prompt_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/prompt_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/prompt_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/prompt_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/prompt_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/prompt_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/prompt_type_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/prompt_type_enum.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/property_mapping.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/property_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/property_mapping_preview.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/property_mapping_preview.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/property_mapping_test_result.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/property_mapping_test_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/protocol_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/protocol_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/provider.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/provider_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/provider_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/provider_model_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/provider_model_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/provider_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/provider_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/provider_type_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/provider_type_enum.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/proxy_mode.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/proxy_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/proxy_outpost_config.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/proxy_outpost_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/proxy_provider.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/proxy_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/proxy_provider_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/proxy_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/rac_property_mapping.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/rac_property_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/rac_property_mapping_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/rac_property_mapping_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/rac_provider.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/rac_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/rac_provider_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/rac_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/radius_outpost_config.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/radius_outpost_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/radius_provider.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/radius_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/radius_provider_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/radius_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/redirect_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/redirect_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/reputation.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/reputation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/reputation_policy.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/reputation_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/reputation_policy_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/reputation_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/resident_key_requirement_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/resident_key_requirement_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/role.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/role_assigned_object_permission.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/role_assigned_object_permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/role_object_permission.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/role_object_permission.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/role_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/role_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/saml_metadata.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/saml_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/saml_property_mapping.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/saml_property_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/saml_property_mapping_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/saml_property_mapping_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/saml_provider.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/saml_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/saml_provider_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/saml_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/saml_source.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/saml_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/saml_source_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/saml_source_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_mapping.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_mapping_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_mapping_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_provider.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_provider_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_provider_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_source.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_source_group.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_source_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_source_group_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_source_group_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_source_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_source_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_source_user.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_source_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_source_user_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_source_user_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/scim_sync_status.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/scim_sync_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/scope_mapping.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/scope_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/scope_mapping_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/scope_mapping_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/selectable_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/selectable_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/service_connection.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/service_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/service_connection_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/service_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/service_connection_state.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/service_connection_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/session_user.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/session_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/settings.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/settings_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/patched_settings_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -20,15 +20,15 @@
 
 from pydantic import BaseModel, ConfigDict, Field, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SettingsRequest(BaseModel):
+class PatchedSettingsRequest(BaseModel):
     """
     Settings Serializer
     """ # noqa: E501
     avatars: Optional[Annotated[str, Field(min_length=1, strict=True)]] = Field(default=None, description="Configure how authentik should show avatars for users.")
     default_user_change_name: Optional[StrictBool] = Field(default=None, description="Enable the ability for users to change their name.")
     default_user_change_email: Optional[StrictBool] = Field(default=None, description="Enable the ability for users to change their email address.")
     default_user_change_username: Optional[StrictBool] = Field(default=None, description="Enable the ability for users to change their username.")
@@ -54,15 +54,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SettingsRequest from a JSON string"""
+        """Create an instance of PatchedSettingsRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -84,15 +84,15 @@
         if self.footer_links is None and "footer_links" in self.model_fields_set:
             _dict['footer_links'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SettingsRequest from a dict"""
+        """Create an instance of PatchedSettingsRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/severity_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_fields_enum.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class SeverityEnum(str, Enum):
+class UserFieldsEnum(str, Enum):
     """
-    SeverityEnum
+    UserFieldsEnum
     """
 
     """
     allowed enum values
     """
-    NOTICE = 'notice'
-    WARNING = 'warning'
-    ALERT = 'alert'
+    EMAIL = 'email'
+    USERNAME = 'username'
+    UPN = 'upn'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of SeverityEnum from a JSON string"""
+        """Create an instance of UserFieldsEnum from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/shell_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/shell_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/signature_algorithm_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/signature_algorithm_enum.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/sms_device.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/sms_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/sms_device_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/sms_device_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/source.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/source_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/source_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/source_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/source_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/source_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/source_type.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/source_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/sp_binding_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/sp_binding_enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/stage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/stage_prompt.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/stage_prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/static_device.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/static_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/static_device_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/static_device_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/static_device_token.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/static_device_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/static_device_token_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/static_device_token_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/sub_mode_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/sub_mode_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/system_info.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/system_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/system_info_runtime.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/system_info_runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/system_task.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/system_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/system_task_status_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/system_task_status_enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/tenant.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/tenant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/tenant_admin_group_request_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/tenant_admin_group_request_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/tenant_recovery_key_request_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/tenant_recovery_key_request_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/tenant_recovery_key_response.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/tenant_recovery_key_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/tenant_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/tenant_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/token.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/token_model.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/token_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/token_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/token_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/token_set_key_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/token_set_key_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/token_view.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_account_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TokenView(BaseModel):
+class UserAccountRequest(BaseModel):
     """
-    Show token's current key
+    Account adding/removing operations
     """ # noqa: E501
-    key: StrictStr
-    __properties: ClassVar[List[str]] = ["key"]
+    pk: StrictInt
+    __properties: ClassVar[List[str]] = ["pk"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,47 +44,45 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TokenView from a JSON string"""
+        """Create an instance of UserAccountRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
-        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "key",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TokenView from a dict"""
+        """Create an instance of UserAccountRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "key": obj.get("key")
+            "pk": obj.get("pk")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/totp_device.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/totp_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/totp_device_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/totp_device_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/transaction_application_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/transaction_application_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/transaction_application_response.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/transaction_application_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/type_create.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/type_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/ui_theme_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/ui_theme_enum.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/used_by.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/used_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/used_by_action_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/used_by_action_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_account_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_saml_source_connection_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt
+from pydantic import BaseModel, ConfigDict, Field, StrictInt
 from typing import Any, ClassVar, Dict, List
+from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UserAccountRequest(BaseModel):
+class UserSAMLSourceConnectionRequest(BaseModel):
     """
-    Account adding/removing operations
+    SAML Source Serializer
     """ # noqa: E501
-    pk: StrictInt
-    __properties: ClassVar[List[str]] = ["pk"]
+    user: StrictInt
+    identifier: Annotated[str, Field(min_length=1, strict=True)]
+    __properties: ClassVar[List[str]] = ["user", "identifier"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UserAccountRequest from a JSON string"""
+        """Create an instance of UserSAMLSourceConnectionRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,20 +71,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UserAccountRequest from a dict"""
+        """Create an instance of UserSAMLSourceConnectionRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "pk": obj.get("pk")
+            "user": obj.get("user"),
+            "identifier": obj.get("identifier")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_assigned_object_permission.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_assigned_object_permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_consent.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_consent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_creation_mode_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_creation_mode_enum.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_delete_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_delete_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_delete_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_delete_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_fields_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_verification_enum.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class UserFieldsEnum(str, Enum):
+class UserVerificationEnum(str, Enum):
     """
-    UserFieldsEnum
+    UserVerificationEnum
     """
 
     """
     allowed enum values
     """
-    EMAIL = 'email'
-    USERNAME = 'username'
-    UPN = 'upn'
+    REQUIRED = 'required'
+    PREFERRED = 'preferred'
+    DISCOURAGED = 'discouraged'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of UserFieldsEnum from a JSON string"""
+        """Create an instance of UserVerificationEnum from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_group.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_group_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_group_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_login_challenge.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_login_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_login_challenge_response_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_login_challenge_response_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_login_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_login_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_login_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_login_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_logout_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_logout_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_logout_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_logout_stage_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_matching_mode_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_matching_mode_enum.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_metrics.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_o_auth_source_connection.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_o_auth_source_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_o_auth_source_connection_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_o_auth_source_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_object_permission.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_object_permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_password_set_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_password_set_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_path.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_saml_source_connection.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_saml_source_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_saml_source_connection_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/web_authn_device_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictInt
+from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UserSAMLSourceConnectionRequest(BaseModel):
+class WebAuthnDeviceRequest(BaseModel):
     """
-    SAML Source Serializer
+    Serializer for WebAuthn authenticator devices
     """ # noqa: E501
-    user: StrictInt
-    identifier: Annotated[str, Field(min_length=1, strict=True)]
-    __properties: ClassVar[List[str]] = ["user", "identifier"]
+    name: Annotated[str, Field(min_length=1, strict=True, max_length=200)]
+    __properties: ClassVar[List[str]] = ["name"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UserSAMLSourceConnectionRequest from a JSON string"""
+        """Create an instance of WebAuthnDeviceRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,21 +70,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UserSAMLSourceConnectionRequest from a dict"""
+        """Create an instance of WebAuthnDeviceRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "user": obj.get("user"),
-            "identifier": obj.get("identifier")
+            "name": obj.get("name")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_self.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_self.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_self_groups.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_self_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_service_account_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_service_account_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_service_account_response.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_service_account_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_setting.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_setting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_source_connection.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_source_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_type_enum.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_write_stage.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_write_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/user_write_stage_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/user_write_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/validation_error.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/validation_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/version.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/web_authn_device.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/web_authn_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/web_authn_device_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/web_authn_device_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
-from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class WebAuthnDeviceRequest(BaseModel):
+class WebAuthnDeviceType(BaseModel):
     """
-    Serializer for WebAuthn authenticator devices
+    WebAuthnDeviceType Serializer
     """ # noqa: E501
-    name: Annotated[str, Field(min_length=1, strict=True, max_length=200)]
-    __properties: ClassVar[List[str]] = ["name"]
+    aaguid: StrictStr
+    description: StrictStr
+    __properties: ClassVar[List[str]] = ["aaguid", "description"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of WebAuthnDeviceRequest from a JSON string"""
+        """Create an instance of WebAuthnDeviceType from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,20 +70,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of WebAuthnDeviceRequest from a dict"""
+        """Create an instance of WebAuthnDeviceType from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name")
+            "aaguid": obj.get("aaguid"),
+            "description": obj.get("description")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/web_authn_device_type.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/web_authn_device_type_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List
+from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class WebAuthnDeviceType(BaseModel):
+class WebAuthnDeviceTypeRequest(BaseModel):
     """
     WebAuthnDeviceType Serializer
     """ # noqa: E501
     aaguid: StrictStr
-    description: StrictStr
+    description: Annotated[str, Field(min_length=1, strict=True)]
     __properties: ClassVar[List[str]] = ["aaguid", "description"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -45,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of WebAuthnDeviceType from a JSON string"""
+        """Create an instance of WebAuthnDeviceTypeRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,15 +71,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of WebAuthnDeviceType from a dict"""
+        """Create an instance of WebAuthnDeviceTypeRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/models/web_authn_device_type_request.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/models/workers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List
-from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class WebAuthnDeviceTypeRequest(BaseModel):
+class Workers(BaseModel):
     """
-    WebAuthnDeviceType Serializer
+    Workers
     """ # noqa: E501
-    aaguid: StrictStr
-    description: Annotated[str, Field(min_length=1, strict=True)]
-    __properties: ClassVar[List[str]] = ["aaguid", "description"]
+    count: StrictInt
+    __properties: ClassVar[List[str]] = ["count"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of WebAuthnDeviceTypeRequest from a JSON string"""
+        """Create an instance of Workers from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,21 +69,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of WebAuthnDeviceTypeRequest from a dict"""
+        """Create an instance of Workers from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "aaguid": obj.get("aaguid"),
-            "description": obj.get("description")
+            "count": obj.get("count")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.0.post1713978839/authentik_client/rest.py` & `authentik_client-2024.4.1.post1714149882/authentik_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.0
+    The version of the OpenAPI document: 2024.4.1
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.0.post1713978839/pyproject.toml` & `authentik_client-2024.4.1.post1714149882/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "authentik_client"
-version = "2024.4.0-1713978839"
+version = "2024.4.1-1714149882"
 description = "authentik"
 authors = ["authentik Team <hello@goauthentik.io>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/goauthentik/authentik"
 keywords = ["OpenAPI", "OpenAPI-Generator", "authentik"]
 include = ["authentik_client/py.typed"]
```

### Comparing `authentik_client-2024.4.0.post1713978839/PKG-INFO` & `authentik_client-2024.4.1.post1714149882/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authentik_client
-Version: 2024.4.0.post1713978839
+Version: 2024.4.1.post1714149882
 Summary: authentik
 Home-page: https://github.com/goauthentik/authentik
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,authentik
 Author: authentik Team
 Author-email: hello@goauthentik.io
 Requires-Python: >=3.7,<4.0
@@ -24,16 +24,16 @@
 Description-Content-Type: text/markdown
 
 # authentik-client
 Making authentication simple.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2024.4.0
-- Package version: 2024.4.0-1713978839
+- API version: 2024.4.1
+- Package version: 2024.4.1-1714149882
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
```

