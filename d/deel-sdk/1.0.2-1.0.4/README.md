# Comparing `tmp/deel_sdk-1.0.2.tar.gz` & `tmp/deel_sdk-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deel_sdk-1.0.2.tar", last modified: Thu Apr 18 09:08:17 2024, max compression
+gzip compressed data, was "deel_sdk-1.0.4.tar", last modified: Fri Apr 26 16:02:16 2024, max compression
```

## Comparing `deel_sdk-1.0.2.tar` & `deel_sdk-1.0.4.tar`

### file list

```diff
@@ -1,462 +1,487 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.208049 deel_sdk-1.0.2/
--rw-r--r--   0 runner    (1001) runner    (1001)     1057 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) runner    (1001)   188973 2024-04-18 09:08:17.208049 deel_sdk-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)   188767 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/README.md
--rw-r--r--   0 runner    (1001) runner    (1001)      343 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-04-18 09:08:17.208049 deel_sdk-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.088049 deel_sdk-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.092049 deel_sdk-1.0.2/src/deel_sdk/
--rw-r--r--   0 runner    (1001) runner    (1001)      125 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.096048 deel_sdk-1.0.2/src/deel_sdk/hooks/
--rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/hooks/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      918 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/hooks/hook.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.192049 deel_sdk-1.0.2/src/deel_sdk/models/
--rw-r--r--   0 runner    (1001) runner    (1001)    24919 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      516 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/add_worker_bank_account_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      408 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/additional_eor_info_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1314 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/address.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1049 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/adjustment_category.py
--rw-r--r--   0 runner    (1001) runner    (1001)      482 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/adjustment_created_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      849 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/adjustment_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2484 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/adjustment_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      517 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/adjustment_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1302 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/adjustment_to_update.py
--rw-r--r--   0 runner    (1001) runner    (1001)      517 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/adjustment_to_update_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      529 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/adjustments_categories_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      504 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/adjustments_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      659 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/admin_user.py
--rw-r--r--   0 runner    (1001) runner    (1001)      505 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/admin_user_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      570 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/admin_user_create_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)      696 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/admin_users_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2400 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/agreement.py
--rw-r--r--   0 runner    (1001) runner    (1001)      753 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/agreement_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      484 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/alternate_email_item.py
--rw-r--r--   0 runner    (1001) runner    (1001)      338 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/attachment_file_ref.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1254 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/bank_account_added.py
--rw-r--r--   0 runner    (1001) runner    (1001)      476 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/bank_account_added_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1639 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/bank_account_guide.py
--rw-r--r--   0 runner    (1001) runner    (1001)      510 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/bank_account_guide_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      699 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/bank_account_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)      450 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/bank_account_to_add.py
--rw-r--r--   0 runner    (1001) runner    (1001)      511 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/bank_account_to_add_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      696 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/bank_account_updated.py
--rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/bank_account_updated_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      600 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/bank_account_value_allowed.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10358 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/base.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3817 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/basic_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6686 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/basic_invoice_adjustment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1092 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/basic_legal_entity.py
--rw-r--r--   0 runner    (1001) runner    (1001)      426 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/basic_organization.py
--rw-r--r--   0 runner    (1001) runner    (1001)      410 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/basic_team.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6231 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/basic_timesheet.py
--rw-r--r--   0 runner    (1001) runner    (1001)      712 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/benefit_contribution_type_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      650 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/benefit_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1246 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/breakdown_costs_quote.py
--rw-r--r--   0 runner    (1001) runner    (1001)      916 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/calculate_final_payment_calculation_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)      838 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/candidate_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2215 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/candidate_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      509 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/candidate_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2372 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/candidate_to_patch.py
--rw-r--r--   0 runner    (1001) runner    (1001)      502 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/candidate_to_patch_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      552 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/client_of_basic_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1456 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/client_of_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1354 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/client_of_contract_legal_entity_5.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1661 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/compensation_details_of_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3460 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/compensation_details_of_contract_to_create_shared.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6134 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)      418 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      450 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_container_ongoing_time_based.py
--rw-r--r--   0 runner    (1001) runner    (1001)      456 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_container_pay_as_you_go_time_based.py
--rw-r--r--   0 runner    (1001) runner    (1001)      446 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_container_payg_milestones.py
--rw-r--r--   0 runner    (1001) runner    (1001)      436 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_container_payg_tasks.py
--rw-r--r--   0 runner    (1001) runner    (1001)      631 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_custom_field.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5768 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_details_to_amend.py
--rw-r--r--   0 runner    (1001) runner    (1001)      547 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_document_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      424 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_external_id_to_patch.py
--rw-r--r--   0 runner    (1001) runner    (1001)      465 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_invitation_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      547 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_invitation_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      637 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1125 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_signature_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      540 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_signature_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2449 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      730 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_template.py
--rw-r--r--   0 runner    (1001) runner    (1001)      621 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_template_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      598 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_template_summary.py
--rw-r--r--   0 runner    (1001) runner    (1001)      661 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_termination_result.py
--rw-r--r--   0 runner    (1001) runner    (1001)      539 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_termination_result_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      581 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_amend_details_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1034 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      831 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      591 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_container_ongoing_time_based.py
--rw-r--r--   0 runner    (1001) runner    (1001)      624 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_container_pay_as_you_go_time_based.py
--rw-r--r--   0 runner    (1001) runner    (1001)      576 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_container_payg_milestones.py
--rw-r--r--   0 runner    (1001) runner    (1001)      541 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_container_payg_tasks.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12535 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_ongoing_time_based.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12652 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_pay_as_you_go_time_based.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9026 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_payg_milestones.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8731 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_payg_tasks.py
--rw-r--r--   0 runner    (1001) runner    (1001)      951 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_terminate.py
--rw-r--r--   0 runner    (1001) runner    (1001)      497 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_terminate_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1827 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_type_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      673 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_type_enum_for_estimate.py
--rw-r--r--   0 runner    (1001) runner    (1001)      667 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_who_reports_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      620 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contracts_sort_by_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1068 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contribution.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1020 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/cost_quote.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1368 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/country.py
--rw-r--r--   0 runner    (1001) runner    (1001)      453 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/country_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/create_admin_user_response_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1731 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/create_people_timeoff.py
--rw-r--r--   0 runner    (1001) runner    (1001)      431 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/create_public_token.py
--rw-r--r--   0 runner    (1001) runner    (1001)      483 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/create_public_token_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2762 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/create_timeoff.py
--rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/create_timeoff_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1942 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/create_webhook_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)      417 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/currency.py
--rw-r--r--   0 runner    (1001) runner    (1001)      460 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/currency_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1206 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/deel_invoice.py
--rw-r--r--   0 runner    (1001) runner    (1001)      716 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/deel_invoice_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      546 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/departments.py
--rw-r--r--   0 runner    (1001) runner    (1001)      473 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/departments_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      549 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/download_worker_documents_by_id_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      556 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/email.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9643 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee.py
--rw-r--r--   0 runner    (1001) runner    (1001)      570 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_agreement_download_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      660 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_agreement_download_object.py
--rw-r--r--   0 runner    (1001) runner    (1001)      386 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_contract_signature_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      597 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_contract_signature_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1796 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_payslips_list.py
--rw-r--r--   0 runner    (1001) runner    (1001)      538 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_payslips_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1078 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_tax_documents_list.py
--rw-r--r--   0 runner    (1001) runner    (1001)      567 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_tax_documents_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      621 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      553 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_creation_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      651 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_entitlements_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3302 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_entitlements_item.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6384 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_item.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8435 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_item_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)      619 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_policies_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2975 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_policies_item.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5398 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7421 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employment_detail.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1396 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employment_details_of_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2006 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_client_timeoff_requests.py
--rw-r--r--   0 runner    (1001) runner    (1001)      720 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_client_timeoffs.py
--rw-r--r--   0 runner    (1001) runner    (1001)      483 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_client_timeoffs_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5189 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_contract_benefits.py
--rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_contract_benefits_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9155 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_contract_created.py
--rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_contract_created_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13172 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_contract_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      498 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_contract_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13924 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_country_validations.py
--rw-r--r--   0 runner    (1001) runner    (1001)      511 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_country_validations_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1468 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_employee_cost_calculation_request_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)      635 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_employee_cost_calculation_request_body_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5990 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_employee_cost_calculation_response_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4905 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_entitlement_list_item.py
--rw-r--r--   0 runner    (1001) runner    (1001)      603 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_entitlements.py
--rw-r--r--   0 runner    (1001) runner    (1001)      504 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_entitlements_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1232 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_field.py
--rw-r--r--   0 runner    (1001) runner    (1001)      937 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_holidays_rollover_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)      496 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_payslip_download_url_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      466 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_payslips_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6621 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_quote_base.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5045 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_timeoffs_base_item.py
--rw-r--r--   0 runner    (1001) runner    (1001)      530 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_timeoffs_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1724 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_timeoffs_employee_item.py
--rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_timeoffs_item_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      676 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/equity_stakeholder.py
--rw-r--r--   0 runner    (1001) runner    (1001)      669 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/equity_stakeholders_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6024 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/estimate_first_payment.py
--rw-r--r--   0 runner    (1001) runner    (1001)      538 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/estimate_first_payment_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      582 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/file_attachment_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/file_object.py
--rw-r--r--   0 runner    (1001) runner    (1001)      879 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/file_ref_type_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3134 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/final_payment_calculated.py
--rw-r--r--   0 runner    (1001) runner    (1001)      518 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/final_payment_calculated_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      437 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/first_payment_date.py
--rw-r--r--   0 runner    (1001) runner    (1001)      628 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/generic_result_created.py
--rw-r--r--   0 runner    (1001) runner    (1001)      852 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/generic_result_created_with_id.py
--rw-r--r--   0 runner    (1001) runner    (1001)      643 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/generic_result_deleted.py
--rw-r--r--   0 runner    (1001) runner    (1001)      628 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/generic_result_updated.py
--rw-r--r--   0 runner    (1001) runner    (1001)      303 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/get_contract_list_currencies.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1238 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/get_employee_compliance_document_template_download_link_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3160 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/get_employee_compliance_documents_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/get_invoice_list_entities.py
--rw-r--r--   0 runner    (1001) runner    (1001)      301 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/get_payment_list_currencies.py
--rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/get_payment_list_entities.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5154 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/global_payroll_g2_n_report.py
--rw-r--r--   0 runner    (1001) runner    (1001)      554 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/global_payroll_g2_n_report_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      990 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_client.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7507 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_created.py
--rw-r--r--   0 runner    (1001) runner    (1001)      483 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_created_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      638 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_salary_scale_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      685 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_salary_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      617 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_status_type_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5709 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      491 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      551 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_address_to_update_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      716 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_address_update_data.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1372 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_address_updated.py
--rw-r--r--   0 runner    (1001) runner    (1001)      533 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_address_updated_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      586 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_compensation_to_update_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      932 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_compensation_update_data.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1584 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_compensation_updated.py
--rw-r--r--   0 runner    (1001) runner    (1001)      602 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_compensation_updated_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      579 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_information_to_update_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2033 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_information_update_data.py
--rw-r--r--   0 runner    (1001) runner    (1001)      577 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_information_updated_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      523 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_pto_to_update_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      620 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_pto_update_data.py
--rw-r--r--   0 runner    (1001) runner    (1001)      544 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_payroll_event_report_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      845 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_payroll_event_reports.py
--rw-r--r--   0 runner    (1001) runner    (1001)      494 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_payslip_download_url_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      464 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_payslips_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5236 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/health_insurance_provider.py
--rw-r--r--   0 runner    (1001) runner    (1001)      653 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hiring_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      414 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hr_document_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)      542 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hr_verification_letters_and_documents_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      505 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hris_compensation.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1948 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hris_contract_full_time.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2155 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hris_contract_part_time.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3477 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hris_direct_employee.py
--rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hris_direct_employee_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1109 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hris_direct_employee_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3797 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hris_direct_employee_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)      509 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hris_job_information_title_id.py
--rw-r--r--   0 runner    (1001) runner    (1001)      521 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hris_job_information_title_name.py
--rw-r--r--   0 runner    (1001) runner    (1001)      485 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hris_team_information.py
--rw-r--r--   0 runner    (1001) runner    (1001)      241 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/identifier_value.py
--rw-r--r--   0 runner    (1001) runner    (1001)      882 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/input_to_create_file_ref.py
--rw-r--r--   0 runner    (1001) runner    (1001)      462 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/input_to_create_pgo_task.py
--rw-r--r--   0 runner    (1001) runner    (1001)      533 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/input_to_patch_contract_external_id.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8507 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/internal_people.py
--rw-r--r--   0 runner    (1001) runner    (1001)      495 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/internal_people_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      673 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invitations_of_basic_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2311 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice.py
--rw-r--r--   0 runner    (1001) runner    (1001)      503 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_attachment_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1336 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_created.py
--rw-r--r--   0 runner    (1001) runner    (1001)      566 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_created_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      798 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1229 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_review_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      583 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_review_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1553 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_reviews_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      590 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_reviews_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      949 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1640 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      576 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1840 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_to_create_with_file.py
--rw-r--r--   0 runner    (1001) runner    (1001)      548 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_to_update.py
--rw-r--r--   0 runner    (1001) runner    (1001)      576 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_to_update_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3514 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_type_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1131 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_type_to_create_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      507 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_download_link_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      347 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_download_object.py
--rw-r--r--   0 runner    (1001) runner    (1001)      687 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      961 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      545 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/job_title.py
--rw-r--r--   0 runner    (1001) runner    (1001)      805 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/job_title_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      576 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/legal_entity_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      572 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/legal_entity_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2378 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/letter_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1056 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/marital_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      728 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/meta_data_of_contract_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2541 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/milestone.py
--rw-r--r--   0 runner    (1001) runner    (1001)      425 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/milestone_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      467 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/milestone_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      589 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/milestone_properties.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1196 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/milestone_review_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      526 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/milestone_review_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1354 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/milestone_reviews_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      533 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/milestone_reviews_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      492 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/milestone_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      800 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/milestone_to_create_form_with_file.py
--rw-r--r--   0 runner    (1001) runner    (1001)      427 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/monthly_payment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2261 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/off_cycle_payment.py
--rw-r--r--   0 runner    (1001) runner    (1001)      469 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/off_cycle_payment_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      511 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/off_cycle_payment_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      804 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/off_cycle_payment_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      563 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/off_cycle_payment_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      514 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/organization_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      385 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/output_to_create_file_ref.py
--rw-r--r--   0 runner    (1001) runner    (1001)      513 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/output_to_create_file_ref_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      423 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/page_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)      359 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/page_info_without_cursor.py
--rw-r--r--   0 runner    (1001) runner    (1001)      601 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/page_info_without_cursor_new.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2010 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/patch_webhook_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1828 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6179 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payment_break_down.py
--rw-r--r--   0 runner    (1001) runner    (1001)      510 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payment_break_down_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      450 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payment_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      589 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payment_method.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1794 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payment_method_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      664 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payment_object.py
--rw-r--r--   0 runner    (1001) runner    (1001)      561 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payment_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      854 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payment_worker.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4715 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payroll_adjustment.py
--rw-r--r--   0 runner    (1001) runner    (1001)      307 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payslip_download_url.py
--rw-r--r--   0 runner    (1001) runner    (1001)      645 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payslips.py
--rw-r--r--   0 runner    (1001) runner    (1001)      913 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/pension_eor_contract_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1290 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/pension_provider.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10185 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/people_by_id_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      736 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/people_client_legal_entity.py
--rw-r--r--   0 runner    (1001) runner    (1001)      750 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/people_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      624 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/people_custom_field.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4291 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/people_me.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1095 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/people_payment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1801 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/people_sort_by_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2067 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/people_time_off_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1567 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/pgo_task.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1282 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/pgo_task_reviews_by_id_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1537 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/pgo_task_reviews_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1105 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/pgo_task_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2885 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/premium_result_added.py
--rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/premium_result_added_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2487 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/premium_to_add.py
--rw-r--r--   0 runner    (1001) runner    (1001)      448 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/premium_to_add_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3499 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/pro_rata.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1008 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/profile_type_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      313 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/public_token.py
--rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/public_token_created_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      586 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_by_id_reviews_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      556 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_reviews_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/request_custom_verification_letter_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2920 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/request_custom_verification_letter_with_file.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2999 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/requester_time_off.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1029 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/response_estimate_first_payment.py
--rw-r--r--   0 runner    (1001) runner    (1001)      561 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/response_estimate_first_payment_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      914 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/salary_frequency_scale_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      835 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/seniority.py
--rw-r--r--   0 runner    (1001) runner    (1001)      508 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/seniority_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      774 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/seniority_required.py
--rw-r--r--   0 runner    (1001) runner    (1001)      764 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/signatures_of_basic_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1129 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/signatures_of_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)      514 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/sort_dir_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      465 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/state_of_country.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1132 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/task_created.py
--rw-r--r--   0 runner    (1001) runner    (1001)      440 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/task_created_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      448 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/task_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      552 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/team.py
--rw-r--r--   0 runner    (1001) runner    (1001)      458 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/team_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      571 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/team_of_basic_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)      561 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/team_of_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)      620 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timeoff_review.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1270 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timeoff_review_internal.py
--rw-r--r--   0 runner    (1001) runner    (1001)      458 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timeoff_to_review_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      515 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timeoff_to_review_internal_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      361 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timeoff_type_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1006 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timeoffs_attachments_item.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1300 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timeoffs_profile.py
--rw-r--r--   0 runner    (1001) runner    (1001)      662 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timeoffs_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      648 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timeoffs_type_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6364 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet.py
--rw-r--r--   0 runner    (1001) runner    (1001)      529 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_approver.py
--rw-r--r--   0 runner    (1001) runner    (1001)      425 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      249 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_id_items.py
--rw-r--r--   0 runner    (1001) runner    (1001)      711 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1196 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_review_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      526 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_review_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1520 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_reviews_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      533 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_reviews_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      939 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_shared_properties.py
--rw-r--r--   0 runner    (1001) runner    (1001)      911 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      608 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1125 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_to_create_container_with_file.py
--rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_to_update.py
--rw-r--r--   0 runner    (1001) runner    (1001)      568 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_to_update_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      538 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/update_worker_department.py
--rw-r--r--   0 runner    (1001) runner    (1001)      518 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/update_worker_department_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      606 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/update_worker_working_location.py
--rw-r--r--   0 runner    (1001) runner    (1001)      554 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/update_worker_working_location_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      911 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/upload_employee_compliance_document_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      406 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/upload_employee_compliance_document_file_container.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.192049 deel_sdk-1.0.2/src/deel_sdk/models/utils/
--rw-r--r--   0 runner    (1001) runner    (1001)     2636 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/utils/cast_models.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2642 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/utils/json_map.py
--rw-r--r--   0 runner    (1001) runner    (1001)      933 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/validation_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)      662 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/validation_type_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      625 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/webhook_event_type_list_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1682 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/webhook_event_type_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2910 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/webhook_item.py
--rw-r--r--   0 runner    (1001) runner    (1001)      438 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/webhook_item_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)      472 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/webhook_list_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)      951 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/week_days_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      776 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/work_statement_cycle_end_type_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      895 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/work_statement_cycle_scale_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      666 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/work_statement_payment_due_type_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      988 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/work_statement_scale_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5945 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_bank_account_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5328 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_bank_account_to_add.py
--rw-r--r--   0 runner    (1001) runner    (1001)      548 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_bank_accounts_info_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1317 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_document.py
--rw-r--r--   0 runner    (1001) runner    (1001)      618 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_document_download_link.py
--rw-r--r--   0 runner    (1001) runner    (1001)      526 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_documents_by_id_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      806 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_legal_entity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1237 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_of_basic_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3079 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_of_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)      495 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_termination.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1140 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_termination_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)      511 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_termination_body_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      482 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_termination_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      555 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/working_locations.py
--rw-r--r--   0 runner    (1001) runner    (1001)      509 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/working_locations_container.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.192049 deel_sdk-1.0.2/src/deel_sdk/net/
--rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.196049 deel_sdk-1.0.2/src/deel_sdk/net/environment/
--rw-r--r--   0 runner    (1001) runner    (1001)       96 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/environment/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      396 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/environment/environment.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.196049 deel_sdk-1.0.2/src/deel_sdk/net/headers/
--rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/headers/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1184 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/headers/access_token_auth.py
--rw-r--r--   0 runner    (1001) runner    (1001)      225 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/headers/base_header.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.196049 deel_sdk-1.0.2/src/deel_sdk/net/request_chain/
--rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/request_chain/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.196049 deel_sdk-1.0.2/src/deel_sdk/net/request_chain/handlers/
--rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/request_chain/handlers/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1221 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/request_chain/handlers/base_handler.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1704 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/request_chain/handlers/hook_handler.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2578 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/request_chain/handlers/http_handler.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2442 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/request_chain/handlers/retry_handler.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1835 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/request_chain/request_chain.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.200049 deel_sdk-1.0.2/src/deel_sdk/net/transport/
--rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/transport/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2704 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/transport/request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1652 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/transport/request_error.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2308 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/transport/response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8604 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/transport/serializer.py
--rw-r--r--   0 runner    (1001) runner    (1001)      681 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/transport/utils.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5111 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/sdk.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.204048 deel_sdk-1.0.2/src/deel_sdk/services/
--rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8524 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/accounting.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7738 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/adjustments.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2587 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/candidates.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1641 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/carta.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12960 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/contractors.py
--rw-r--r--   0 runner    (1001) runner    (1001)    22150 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/contracts.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7352 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/eor.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18979 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/global_payroll.py
--rw-r--r--   0 runner    (1001) runner    (1001)    17186 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/invoices.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5044 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/lookups.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2584 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/managers.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8032 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/milestones.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4151 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/off_cycle_payments.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5621 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/organizations.py
--rw-r--r--   0 runner    (1001) runner    (1001)    22375 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/partner_managed.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18569 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/people.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7063 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/tasks.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8293 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/time_off.py
--rw-r--r--   0 runner    (1001) runner    (1001)    14070 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/timesheets.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1385 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/token.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.204048 deel_sdk-1.0.2/src/deel_sdk/services/utils/
--rw-r--r--   0 runner    (1001) runner    (1001)     2256 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/utils/base_service.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1603 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/utils/default_headers.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8007 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/utils/validator.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5237 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/webhooks.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.204048 deel_sdk-1.0.2/src/deel_sdk.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)   188973 2024-04-18 09:08:17.000000 deel_sdk-1.0.2/src/deel_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)    21372 2024-04-18 09:08:17.000000 deel_sdk-1.0.2/src/deel_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-04-18 09:08:17.000000 deel_sdk-1.0.2/src/deel_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       17 2024-04-18 09:08:17.000000 deel_sdk-1.0.2/src/deel_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        9 2024-04-18 09:08:17.000000 deel_sdk-1.0.2/src/deel_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-26 16:02:16.356751 deel_sdk-1.0.4/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1057 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) runner    (1001)   216859 2024-04-26 16:02:16.356751 deel_sdk-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)   216653 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) runner    (1001)      343 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-04-26 16:02:16.356751 deel_sdk-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-26 16:02:16.236750 deel_sdk-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-26 16:02:16.240750 deel_sdk-1.0.4/src/deel_sdk/
+-rw-r--r--   0 runner    (1001) runner    (1001)      125 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-26 16:02:16.240750 deel_sdk-1.0.4/src/deel_sdk/hooks/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      962 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/hooks/hook.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-26 16:02:16.344751 deel_sdk-1.0.4/src/deel_sdk/models/
+-rw-r--r--   0 runner    (1001) runner    (1001)    26333 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      516 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/add_worker_bank_account_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      408 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/additional_eor_info_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1314 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/address.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1049 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/adjustment_category.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      482 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/adjustment_created_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      849 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/adjustment_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2484 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/adjustment_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      517 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/adjustment_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1302 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/adjustment_to_update.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      517 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/adjustment_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      529 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/adjustments_categories_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      504 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/adjustments_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      659 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/admin_user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      505 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/admin_user_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      570 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/admin_user_create_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      696 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/admin_users_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2400 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/agreement.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      753 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/agreement_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      484 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/alternate_email_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      338 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/attachment_file_ref.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1254 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/bank_account_added.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      476 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/bank_account_added_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1639 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/bank_account_guide.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      510 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/bank_account_guide_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      699 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/bank_account_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      450 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/bank_account_to_add.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      511 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/bank_account_to_add_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      696 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/bank_account_updated.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/bank_account_updated_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      600 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/bank_account_value_allowed.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10358 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/base.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3817 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/basic_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6686 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/basic_invoice_adjustment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1092 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/basic_legal_entity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      426 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/basic_organization.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      410 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/basic_team.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6231 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/basic_timesheet.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      712 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/benefit_contribution_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      650 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/benefit_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1246 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/breakdown_costs_quote.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      916 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/calculate_final_payment_calculation_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      838 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/candidate_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2215 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/candidate_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      509 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/candidate_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2372 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/candidate_to_patch.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      502 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/candidate_to_patch_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      552 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/client_of_basic_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1456 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/client_of_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1354 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/client_of_contract_legal_entity_1.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1661 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/compensation_details_of_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3460 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/compensation_details_of_contract_to_create_shared.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6134 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      418 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      450 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_container_ongoing_time_based.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      456 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_container_pay_as_you_go_time_based.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      446 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_container_payg_milestones.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      436 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_container_payg_tasks.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      631 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_custom_field.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5768 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_details_to_amend.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      547 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_document_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      424 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_external_id_to_patch.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      465 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_invitation_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      547 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_invitation_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      637 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1125 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_signature_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      540 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_signature_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2449 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      730 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_template.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      621 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_template_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      598 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_template_summary.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      661 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_termination_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      539 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_termination_result_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      581 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_to_amend_details_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1034 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      831 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      591 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_to_create_container_ongoing_time_based.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      624 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_to_create_container_pay_as_you_go_time_based.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      576 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_to_create_container_payg_milestones.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      541 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_to_create_container_payg_tasks.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12696 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_to_create_ongoing_time_based.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12813 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_to_create_pay_as_you_go_time_based.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9187 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_to_create_payg_milestones.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8892 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_to_create_payg_tasks.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      951 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_to_terminate.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      497 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_to_terminate_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1827 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      673 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_type_enum_for_estimate.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      667 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contract_who_reports_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      620 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contracts_sort_by_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1068 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/contribution.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1020 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/cost_quote.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1368 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/country.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      453 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/country_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/create_admin_user_response_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1731 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/create_people_timeoff.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      431 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/create_public_token.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      483 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/create_public_token_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2762 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/create_timeoff.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/create_timeoff_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1942 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/create_webhook_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      871 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/created_exercise_equity_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1595 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/created_role_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      417 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/currency.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      460 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/currency_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      484 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/custom_field_item_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4136 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/custom_field_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5637 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/custom_field_values_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      520 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/custom_fields_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8637 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/custom_fields_object.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1206 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/deel_invoice.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      716 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/deel_invoice_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      546 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/departments.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      473 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/departments_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      549 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/download_worker_documents_by_id_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      556 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/email.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9643 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/employee.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      570 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/employee_agreement_download_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      660 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/employee_agreement_download_object.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      386 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/employee_contract_signature_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      597 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/employee_contract_signature_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1796 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/employee_payslips_list.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      538 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/employee_payslips_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1078 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/employee_tax_documents_list.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      567 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/employee_tax_documents_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      621 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/employee_timeoffs_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      553 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/employee_timeoffs_creation_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      651 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/employee_timeoffs_entitlements_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3302 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/employee_timeoffs_entitlements_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6384 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/employee_timeoffs_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8435 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/employee_timeoffs_item_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      619 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/employee_timeoffs_policies_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2975 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/employee_timeoffs_policies_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5398 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/employment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7421 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/employment_detail.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1396 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/employment_details_of_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2006 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_client_timeoff_requests.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      720 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_client_timeoffs.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      483 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_client_timeoffs_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5189 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_contract_benefits.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_contract_benefits_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9155 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_contract_created.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_contract_created_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13172 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_contract_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      498 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_contract_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13924 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_country_validations.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      511 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_country_validations_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1468 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_employee_cost_calculation_request_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      635 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_employee_cost_calculation_request_body_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5990 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_employee_cost_calculation_response_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4905 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_entitlement_list_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      603 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_entitlements.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      504 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_entitlements_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1232 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_field.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      937 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_holidays_rollover_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      496 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_payslip_download_url_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      466 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_payslips_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6621 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_quote_base.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5045 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_timeoffs_base_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      530 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_timeoffs_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1724 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_timeoffs_employee_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/eor_timeoffs_item_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      676 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/equity_stakeholder.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      669 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/equity_stakeholders_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6024 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/estimate_first_payment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      538 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/estimate_first_payment_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3508 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/exercise_equity_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      417 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/exercise_equity_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      582 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/file_attachment_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/file_object.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      879 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/file_ref_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3134 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/final_payment_calculated.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      518 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/final_payment_calculated_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      437 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/first_payment_date.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      628 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/generic_result_created.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      852 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/generic_result_created_with_id.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      643 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/generic_result_deleted.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      628 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/generic_result_updated.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2822 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/get_all_org_structures_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      303 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/get_contract_list_currencies.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1238 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/get_employee_compliance_document_template_download_link_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3160 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/get_employee_compliance_documents_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3033 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/get_hris_position_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/get_invoice_list_entities.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2784 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/get_org_structure_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      301 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/get_payment_list_currencies.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/get_payment_list_entities.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      474 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/get_roles_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1035 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/get_roles_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5154 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/global_payroll_g2_n_report.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      554 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/global_payroll_g2_n_report_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      990 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_client.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7507 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_contract_created.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      483 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_contract_created_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      638 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_contract_salary_scale_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      685 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_contract_salary_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      617 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_contract_status_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5709 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_contract_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      491 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_contract_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      551 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_address_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      716 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_address_update_data.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1372 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_address_updated.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      533 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_address_updated_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      586 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_compensation_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      932 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_compensation_update_data.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1584 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_compensation_updated.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      602 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_compensation_updated_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      579 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_information_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2033 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_information_update_data.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      577 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_information_updated_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      523 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_pto_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      620 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_pto_update_data.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      544 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_payroll_event_report_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      845 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_payroll_event_reports.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      494 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_payslip_download_url_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      464 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/gp_payslips_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5236 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/health_insurance_provider.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      653 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/hiring_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      414 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/hr_document_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      542 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/hr_verification_letters_and_documents_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      505 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/hris_compensation.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1948 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/hris_contract_full_time.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2155 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/hris_contract_part_time.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3477 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/hris_direct_employee.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/hris_direct_employee_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1109 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/hris_direct_employee_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3797 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/hris_direct_employee_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      509 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/hris_job_information_title_id.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      521 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/hris_job_information_title_name.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2683 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/hris_position_to_change_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      485 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/hris_team_information.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      241 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/identifier_value.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      882 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/input_to_create_file_ref.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      462 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/input_to_create_pgo_task.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      533 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/input_to_patch_contract_external_id.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8507 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/internal_people.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      495 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/internal_people_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      673 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invitations_of_basic_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2331 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      503 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_attachment_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1336 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_created.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      566 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_created_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      798 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1229 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_review_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      583 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_review_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1553 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_reviews_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      590 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_reviews_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      949 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1640 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      576 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1840 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_to_create_with_file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      548 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_to_update.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      576 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3514 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1131 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_type_to_create_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      507 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice_download_link_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      347 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice_download_object.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      687 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      961 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/invoice_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      545 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/job_title.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      805 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/job_title_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      576 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/legal_entity_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      572 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/legal_entity_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2378 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/letter_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1056 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/marital_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      728 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/meta_data_of_contract_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2541 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/milestone.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      425 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/milestone_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      467 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/milestone_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      589 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/milestone_properties.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1196 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/milestone_review_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      526 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/milestone_review_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1513 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/milestone_reviews_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      533 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/milestone_reviews_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      492 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/milestone_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      800 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/milestone_to_create_form_with_file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      427 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/monthly_payment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2261 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/off_cycle_payment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      469 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/off_cycle_payment_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      511 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/off_cycle_payment_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      804 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/off_cycle_payment_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      563 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/off_cycle_payment_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2153 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/org_structure_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1601 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/org_structure_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      514 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/organization_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      385 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/output_to_create_file_ref.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      513 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/output_to_create_file_ref_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      423 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/page_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      359 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/page_info_without_cursor.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      601 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/page_info_without_cursor_new.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2010 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/patch_webhook_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1828 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/payment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6179 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/payment_break_down.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      510 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/payment_break_down_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      450 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/payment_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      589 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/payment_method.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1794 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/payment_method_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      664 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/payment_object.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      561 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/payment_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      854 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/payment_worker.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4715 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/payroll_adjustment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      307 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/payslip_download_url.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      645 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/payslips.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      913 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/pension_eor_contract_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1290 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/pension_provider.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10185 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/people_by_id_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      736 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/people_client_legal_entity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      750 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/people_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      624 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/people_custom_field.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4291 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/people_me.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1095 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/people_payment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1801 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/people_sort_by_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2067 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/people_time_off_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1567 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/pgo_task.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1282 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/pgo_task_reviews_by_id_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1537 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/pgo_task_reviews_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1105 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/pgo_task_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2885 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/premium_result_added.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/premium_result_added_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2487 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/premium_to_add.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      448 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/premium_to_add_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3499 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/pro_rata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1008 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/profile_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      313 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/public_token.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/public_token_created_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      586 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_by_id_reviews_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      556 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_reviews_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/request_custom_verification_letter_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2920 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/request_custom_verification_letter_with_file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2999 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/requester_time_off.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1029 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/response_estimate_first_payment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      561 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/response_estimate_first_payment_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1475 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/role_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1279 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/role_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      914 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/salary_frequency_scale_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      835 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/seniority.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      508 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/seniority_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      774 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/seniority_required.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      764 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/signatures_of_basic_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1129 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/signatures_of_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      514 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/sort_dir_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      465 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/state_of_country.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1132 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/task_created.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      440 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/task_created_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      448 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/task_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      552 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/team.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      458 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/team_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      571 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/team_of_basic_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      561 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/team_of_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      620 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timeoff_review.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1270 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timeoff_review_internal.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      458 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timeoff_to_review_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      515 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timeoff_to_review_internal_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      361 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timeoff_type_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1006 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timeoffs_attachments_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1300 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timeoffs_profile.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      662 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timeoffs_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      648 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timeoffs_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6364 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timesheet.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      529 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timesheet_approver.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      425 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timesheet_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      249 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timesheet_id_items.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      711 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timesheet_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1196 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timesheet_review_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      526 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timesheet_review_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1520 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timesheet_reviews_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      533 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timesheet_reviews_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      939 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timesheet_shared_properties.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      911 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timesheet_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      608 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timesheet_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1125 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timesheet_to_create_container_with_file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timesheet_to_update.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      568 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/timesheet_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      538 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/update_worker_department.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      518 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/update_worker_department_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      606 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/update_worker_working_location.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      554 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/update_worker_working_location_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      871 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/updated_exercise_equity_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1238 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/updated_role_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      911 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/upload_employee_compliance_document_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      406 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/upload_employee_compliance_document_file_container.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-26 16:02:16.344751 deel_sdk-1.0.4/src/deel_sdk/models/utils/
+-rw-r--r--   0 runner    (1001) runner    (1001)     2636 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/utils/cast_models.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2642 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/utils/json_map.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      933 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/validation_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      662 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/validation_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      625 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/webhook_event_type_list_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1682 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/webhook_event_type_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2910 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/webhook_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      438 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/webhook_item_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      472 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/webhook_list_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      951 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/week_days_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      776 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/work_statement_cycle_end_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      895 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/work_statement_cycle_scale_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      666 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/work_statement_payment_due_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      988 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/work_statement_scale_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5945 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/worker_bank_account_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5328 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/worker_bank_account_to_add.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      548 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/worker_bank_accounts_info_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1317 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/worker_document.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      618 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/worker_document_download_link.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      526 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/worker_documents_by_id_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      806 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/worker_legal_entity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1237 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/worker_of_basic_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3079 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/worker_of_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      495 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/worker_termination.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1140 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/worker_termination_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      511 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/worker_termination_body_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      482 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/worker_termination_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      555 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/working_locations.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      509 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/models/working_locations_container.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-26 16:02:16.344751 deel_sdk-1.0.4/src/deel_sdk/net/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/net/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-26 16:02:16.344751 deel_sdk-1.0.4/src/deel_sdk/net/environment/
+-rw-r--r--   0 runner    (1001) runner    (1001)       96 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/net/environment/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      396 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/net/environment/environment.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-26 16:02:16.344751 deel_sdk-1.0.4/src/deel_sdk/net/headers/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/net/headers/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1184 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/net/headers/access_token_auth.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      225 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/net/headers/base_header.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-26 16:02:16.344751 deel_sdk-1.0.4/src/deel_sdk/net/request_chain/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/net/request_chain/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-26 16:02:16.348751 deel_sdk-1.0.4/src/deel_sdk/net/request_chain/handlers/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/net/request_chain/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1221 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/net/request_chain/handlers/base_handler.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1704 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/net/request_chain/handlers/hook_handler.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2578 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/net/request_chain/handlers/http_handler.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2442 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/net/request_chain/handlers/retry_handler.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1835 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/net/request_chain/request_chain.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-26 16:02:16.348751 deel_sdk-1.0.4/src/deel_sdk/net/transport/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/net/transport/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2704 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/net/transport/request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1652 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/net/transport/request_error.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2308 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/net/transport/response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8604 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/net/transport/serializer.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      681 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/net/transport/utils.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6101 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/sdk.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-26 16:02:16.356751 deel_sdk-1.0.4/src/deel_sdk/services/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8524 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/accounting.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7738 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/adjustments.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2587 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/candidates.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1641 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/carta.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12960 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/contractors.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    24651 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/contracts.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10540 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/custom_fields.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7352 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/eor.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18979 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/global_payroll.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3178 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/hris_organizations.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    17186 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/invoices.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5044 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/lookups.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2584 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/managers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8032 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/milestones.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4151 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/off_cycle_payments.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8318 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/organization_structure.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5621 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/organizations.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    22375 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/partner_managed.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18569 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/people.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2216 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/positions.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7063 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/tasks.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8293 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/time_off.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    14070 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/timesheets.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1385 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/token.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-26 16:02:16.356751 deel_sdk-1.0.4/src/deel_sdk/services/utils/
+-rw-r--r--   0 runner    (1001) runner    (1001)     2471 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/utils/base_service.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1603 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/utils/default_headers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8007 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/utils/validator.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5237 2024-04-26 16:01:45.000000 deel_sdk-1.0.4/src/deel_sdk/services/webhooks.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-26 16:02:16.356751 deel_sdk-1.0.4/src/deel_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)   216859 2024-04-26 16:02:16.000000 deel_sdk-1.0.4/src/deel_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)    22624 2024-04-26 16:02:16.000000 deel_sdk-1.0.4/src/deel_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-04-26 16:02:16.000000 deel_sdk-1.0.4/src/deel_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       17 2024-04-26 16:02:16.000000 deel_sdk-1.0.4/src/deel_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        9 2024-04-26 16:02:16.000000 deel_sdk-1.0.4/src/deel_sdk.egg-info/top_level.txt
```

### Comparing `deel_sdk-1.0.2/LICENSE` & `deel_sdk-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/PKG-INFO` & `deel_sdk-1.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: deel-sdk
-Version: 1.0.2
+Version: 1.0.4
 Summary: Deel REST API
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
-# DeelSdk Python SDK 1.0.2
+# DeelSdk Python SDK 1.0.4
 
 A Python SDK for DeelSdk.
 
 - API version: 1.25.0
-- SDK version: 1.0.2
+- SDK version: 1.0.4
 
 Deel REST API
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Authentication](#authentication)
@@ -102,37 +102,41 @@
 
 You cannot create an instance of a Union type itself. Instead, pass an instance of one of the types in the Union, or a dictionary that can be converted to one of those types.
 
 ## Services
 
 A list of all SDK services. Click on the service name to access its corresponding service methods.
 
-| Service                                             |
-| :-------------------------------------------------- |
-| [AccountingService](#accountingservice)             |
-| [ManagersService](#managersservice)                 |
-| [PeopleService](#peopleservice)                     |
-| [EorService](#eorservice)                           |
-| [GlobalPayrollService](#globalpayrollservice)       |
-| [ContractorsService](#contractorsservice)           |
-| [AdjustmentsService](#adjustmentsservice)           |
-| [CandidatesService](#candidatesservice)             |
-| [PartnerManagedService](#partnermanagedservice)     |
-| [ContractsService](#contractsservice)               |
-| [TasksService](#tasksservice)                       |
-| [TimesheetsService](#timesheetsservice)             |
-| [MilestonesService](#milestonesservice)             |
-| [OffCyclePaymentsService](#offcyclepaymentsservice) |
-| [TimeOffService](#timeoffservice)                   |
-| [InvoicesService](#invoicesservice)                 |
-| [OrganizationsService](#organizationsservice)       |
-| [LookupsService](#lookupsservice)                   |
-| [WebhooksService](#webhooksservice)                 |
-| [TokenService](#tokenservice)                       |
-| [CartaService](#cartaservice)                       |
+| Service                                                       |
+| :------------------------------------------------------------ |
+| [AccountingService](#accountingservice)                       |
+| [CustomFieldsService](#customfieldsservice)                   |
+| [HrisOrganizationsService](#hrisorganizationsservice)         |
+| [ContractsService](#contractsservice)                         |
+| [OrganizationStructureService](#organizationstructureservice) |
+| [PositionsService](#positionsservice)                         |
+| [ManagersService](#managersservice)                           |
+| [PeopleService](#peopleservice)                               |
+| [EorService](#eorservice)                                     |
+| [GlobalPayrollService](#globalpayrollservice)                 |
+| [ContractorsService](#contractorsservice)                     |
+| [AdjustmentsService](#adjustmentsservice)                     |
+| [CandidatesService](#candidatesservice)                       |
+| [PartnerManagedService](#partnermanagedservice)               |
+| [TasksService](#tasksservice)                                 |
+| [TimesheetsService](#timesheetsservice)                       |
+| [MilestonesService](#milestonesservice)                       |
+| [OffCyclePaymentsService](#offcyclepaymentsservice)           |
+| [TimeOffService](#timeoffservice)                             |
+| [InvoicesService](#invoicesservice)                           |
+| [OrganizationsService](#organizationsservice)                 |
+| [LookupsService](#lookupsservice)                             |
+| [WebhooksService](#webhooksservice)                           |
+| [TokenService](#tokenservice)                                 |
+| [CartaService](#cartaservice)                                 |
 
 ### AccountingService
 
 A list of all methods in the `AccountingService` service. Click on the method name to view detailed information about that method.
 
 | Methods                                                                 | Description                                                                                                            |
 | :---------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------- |
@@ -162,23 +166,25 @@
 
 `InvoiceListContainer`
 
 **Example Usage Code Snippet**
 
 ```py
 from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import GetInvoiceListEntities
+from deel_sdk.models.get_invoice_list_entities import List[LegalEntityType]
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
-entities=GetInvoiceListEntities(**[
+entities=List[LegalEntityType](
+    [
     "individual"
-])
+]
+)
 
 result = sdk.accounting.get_invoice_list(
     issued_from_date="issued_from_date",
     issued_to_date="issued_to_date",
     entities=entities,
     limit=10,
     offset=808037660.53
@@ -274,26 +280,31 @@
 
 `PaymentListContainer`
 
 **Example Usage Code Snippet**
 
 ```py
 from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import GetPaymentListCurrencies, GetPaymentListEntities
+from deel_sdk.models.get_payment_list_currencies import List[str]
+from deel_sdk.models.get_payment_list_entities import List[LegalEntityType]
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
-currencies=GetPaymentListCurrencies(**[
+currencies=List[str](
+    [
     "GBP"
-])
-entities=GetPaymentListEntities(**[
+]
+)
+entities=List[LegalEntityType](
+    [
     "individual"
-])
+]
+)
 
 result = sdk.accounting.get_payment_list(
     date_from="1999-12-31",
     date_to="1999-12-31",
     currencies=currencies,
     entities=entities
 )
@@ -328,14 +339,1569 @@
 )
 
 result = sdk.accounting.get_payments_break_down_by_id(payment_id="payment_id")
 
 print(result)
 ```
 
+### CustomFieldsService
+
+A list of all methods in the `CustomFieldsService` service. Click on the method name to view detailed information about that method.
+
+| Methods                                                                               | Description                                                                                                                                        |
+| :------------------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------- |
+| [get_custom_fields_from_people](#get_custom_fields_from_people)                       | Fetch all custom fields associated with People records, offering additional personalized information.                                              |
+| [get_custom_field_from_people_by_id](#get_custom_field_from_people_by_id)             | Access details of a specific custom field by using the custom field ID to enrich individual personnel records.                                     |
+| [get_custom_field_values_from_worker](#get_custom_field_values_from_worker)           | Obtain all custom field values associated with a specific worker, facilitating detailed data retrieval for administrative or operational purposes. |
+| [upsert_custom_field_value_from_worker](#upsert_custom_field_value_from_worker)       | Add or update custom field values for a specific worker, ensuring their profile is up-to-date with the latest information.                         |
+| [delete_custom_field_value_from_worker](#delete_custom_field_value_from_worker)       | Delete a specific custom field value from a worker's profile, removing outdated or unnecessary information.                                        |
+| [get_custom_fields_from_contracts](#get_custom_fields_from_contracts)                 | Fetch all custom fields associated with contracts, providing additional data necessary for contract management.                                    |
+| [get_custom_field_from_contracts_by_id](#get_custom_field_from_contracts_by_id)       | Access details of a specific custom field associated with a contract to manage contract-specific attributes effectively.                           |
+| [get_custom_field_values_from_contract](#get_custom_field_values_from_contract)       | Obtain all custom field values for a specific contract, enhancing contract management with detailed, custom-configured data.                       |
+| [upsert_custom_field_value_from_contracts](#upsert_custom_field_value_from_contracts) | Add or update custom field values for a specific contract, ensuring all contract details are current and relevant.                                 |
+| [delete_contract_custom_field](#delete_contract_custom_field)                         | Delete a specific custom field’s value from a contract, streamlining contract data management by removing redundant or outdated information.       |
+
+#### **get_custom_fields_from_people**
+
+Fetch all custom fields associated with People records, offering additional personalized information.
+
+- HTTP Method: `GET`
+- Endpoint: `/people/custom_fields`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+
+**Return Type**
+
+`CustomFieldsListContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.get_custom_fields_from_people()
+
+print(result)
+```
+
+#### **get_custom_field_from_people_by_id**
+
+Access details of a specific custom field by using the custom field ID to enrich individual personnel records.
+
+- HTTP Method: `GET`
+- Endpoint: `/people/custom_fields/{field_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| field_id | str | ✅ | Access details of a specific custom field by using the custom field ID to enrich individual personnel records. |
+
+**Return Type**
+
+`CustomFieldItemContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.get_custom_field_from_people_by_id(field_id="field_id")
+
+print(result)
+```
+
+#### **get_custom_field_values_from_worker**
+
+Obtain all custom field values associated with a specific worker, facilitating detailed data retrieval for administrative or operational purposes.
+
+- HTTP Method: `GET`
+- Endpoint: `/people/{worker_id}/custom_fields`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| worker_id | str | ✅ | Obtain all custom field values associated with a specific worker, facilitating detailed data retrieval for administrative or operational purposes. |
+
+**Return Type**
+
+`CustomFieldValuesContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.get_custom_field_values_from_worker(worker_id="worker_id")
+
+print(result)
+```
+
+#### **upsert_custom_field_value_from_worker**
+
+Add or update custom field values for a specific worker, ensuring their profile is up-to-date with the latest information.
+
+- HTTP Method: `PUT`
+- Endpoint: `/people/{worker_id}/custom_fields`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | CustomFieldToUpdateContainer | ✅ | The request body. |
+| worker_id | str | ✅ | Add or update custom field values for a specific worker, ensuring their profile is up-to-date with the latest information. |
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import CustomFieldToUpdateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = CustomFieldToUpdateContainer(
+    id_="id",
+    data={
+        "value": "value"
+    }
+)
+
+result = sdk.custom_fields.upsert_custom_field_value_from_worker(
+    request_body=request_body,
+    worker_id="worker_id"
+)
+
+print(result)
+```
+
+#### **delete_custom_field_value_from_worker**
+
+Delete a specific custom field value from a worker's profile, removing outdated or unnecessary information.
+
+- HTTP Method: `DELETE`
+- Endpoint: `/people/{worker_id}/custom_fields/{field_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| worker_id | str | ✅ | Delete a specific custom field value from a worker's profile, removing outdated or unnecessary information. |
+| field_id | str | ✅ | Delete a specific custom field value from a worker's profile, removing outdated or unnecessary information. |
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.delete_custom_field_value_from_worker(
+    worker_id="worker_id",
+    field_id="field_id"
+)
+
+print(result)
+```
+
+#### **get_custom_fields_from_contracts**
+
+Fetch all custom fields associated with contracts, providing additional data necessary for contract management.
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts/custom_fields`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+
+**Return Type**
+
+`CustomFieldsListContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.get_custom_fields_from_contracts()
+
+print(result)
+```
+
+#### **get_custom_field_from_contracts_by_id**
+
+Access details of a specific custom field associated with a contract to manage contract-specific attributes effectively.
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts/custom_fields/{field_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| field_id | str | ✅ | Access details of a specific custom field associated with a contract to manage contract-specific attributes effectively. |
+
+**Return Type**
+
+`CustomFieldItemContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.get_custom_field_from_contracts_by_id(field_id="field_id")
+
+print(result)
+```
+
+#### **get_custom_field_values_from_contract**
+
+Obtain all custom field values for a specific contract, enhancing contract management with detailed, custom-configured data.
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts/{contract_id}/custom_fields`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Obtain all custom field values for a specific contract, enhancing contract management with detailed, custom-configured data. |
+
+**Return Type**
+
+`CustomFieldValuesContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.get_custom_field_values_from_contract(contract_id="contract_id")
+
+print(result)
+```
+
+#### **upsert_custom_field_value_from_contracts**
+
+Add or update custom field values for a specific contract, ensuring all contract details are current and relevant.
+
+- HTTP Method: `PUT`
+- Endpoint: `/contracts/{contract_id}/custom_fields`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | CustomFieldToUpdateContainer | ✅ | The request body. |
+| contract_id | str | ✅ | Add or update custom field values for a specific contract, ensuring all contract details are current and relevant. |
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import CustomFieldToUpdateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = CustomFieldToUpdateContainer(
+    id_="id",
+    data={
+        "value": "value"
+    }
+)
+
+result = sdk.custom_fields.upsert_custom_field_value_from_contracts(
+    request_body=request_body,
+    contract_id="contract_id"
+)
+
+print(result)
+```
+
+#### **delete_contract_custom_field**
+
+Delete a specific custom field’s value from a contract, streamlining contract data management by removing redundant or outdated information.
+
+- HTTP Method: `DELETE`
+- Endpoint: `/contracts/{contract_id}/custom_fields/{field_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Delete a specific custom field’s value from a contract, streamlining contract data management by removing redundant or outdated information. |
+| field_id | str | ✅ | Delete a specific custom field’s value from a contract, streamlining contract data management by removing redundant or outdated information. |
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.delete_contract_custom_field(
+    contract_id="contract_id",
+    field_id="field_id"
+)
+
+print(result)
+```
+
+### HrisOrganizationsService
+
+A list of all methods in the `HrisOrganizationsService` service. Click on the method name to view detailed information about that method.
+
+| Methods                                               | Description                                |
+| :---------------------------------------------------- | :----------------------------------------- |
+| [get_organization_roles](#get_organization_roles)     | Get the roles of the current organization. |
+| [create_organization_role](#create_organization_role) | Create organization custom role.           |
+| [update_organization_role](#update_organization_role) | Update organization custom role.           |
+
+#### **get_organization_roles**
+
+Get the roles of the current organization.
+
+- HTTP Method: `GET`
+- Endpoint: `/roles`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+
+**Return Type**
+
+`GetRolesContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.hris_organizations.get_organization_roles()
+
+print(result)
+```
+
+#### **create_organization_role**
+
+Create organization custom role.
+
+- HTTP Method: `POST`
+- Endpoint: `/roles`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | RoleToCreateContainer | ✅ | The request body. |
+
+**Return Type**
+
+`CreatedRoleContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import RoleToCreateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = RoleToCreateContainer(
+    data={
+        "name": "name",
+        "scope": "ORGANIZATION",
+        "description": "description",
+        "permission_sets": [
+            "permissionSets"
+        ],
+        "hris_org_structure_id": "hrisOrgStructureId"
+    }
+)
+
+result = sdk.hris_organizations.create_organization_role(request_body=request_body)
+
+print(result)
+```
+
+#### **update_organization_role**
+
+Update organization custom role.
+
+- HTTP Method: `PATCH`
+- Endpoint: `/roles/{role_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | RoleToUpdateContainer | ✅ | The request body. |
+| role_id | str | ✅ | Update organization custom role. |
+
+**Return Type**
+
+`UpdatedRoleContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import RoleToUpdateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = RoleToUpdateContainer(
+    data={
+        "name": "name",
+        "description": "description",
+        "permission_sets": [
+            "permissionSets"
+        ]
+    }
+)
+
+result = sdk.hris_organizations.update_organization_role(
+    request_body=request_body,
+    role_id="role_id"
+)
+
+print(result)
+```
+
+### ContractsService
+
+A list of all methods in the `ContractsService` service. Click on the method name to view detailed information about that method.
+
+| Methods                                                                     | Description                                                                                                                                                                                                          |
+| :-------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| [request_exercise_equity](#request_exercise_equity)                         | Create a request to exercise equity.                                                                                                                                                                                 |
+| [approve_exercise_equity](#approve_exercise_equity)                         | Approve an equity exercise.                                                                                                                                                                                          |
+| [get_contract_list](#get_contract_list)                                     | Retrieve a list of contracts.                                                                                                                                                                                        |
+| [get_contract_by_id](#get_contract_by_id)                                   | Retrieve a single contract.                                                                                                                                                                                          |
+| [attach_external_id](#attach_external_id)                                   | Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later. |
+| [add_contract_document](#add_contract_document)                             | Attach a file to contract document.                                                                                                                                                                                  |
+| [edit_contract_document](#edit_contract_document)                           | Overwrite the file currently attached to contract document.                                                                                                                                                          |
+| [get_alternate_emails_by_contract_id](#get_alternate_emails_by_contract_id) | Returns an array of alternate email objects                                                                                                                                                                          |
+| [sign_contract](#sign_contract)                                             | Sign a contract as a client.                                                                                                                                                                                         |
+| [invite_to_sign_contract](#invite_to_sign_contract)                         | Invite a worker to sign the contract. Worker will be notified via email.                                                                                                                                             |
+| [uninvite_to_sign_contract](#uninvite_to_sign_contract)                     | Remove invite in order to re-invite a worker to sign the contract.                                                                                                                                                   |
+| [calculate_final_payment](#calculate_final_payment)                         | Calculate the final payment due to the contractor when ending the contract.                                                                                                                                          |
+| [post_contract_estimate](#post_contract_estimate)                           | First payment is calculated from the number of working/calendar days between their start date and the start of the payment cycle.                                                                                    |
+| [get_contract_templates](#get_contract_templates)                           | Retrieve a list of contract templates in your organization.                                                                                                                                                          |
+| [get_worker_documents_by_id](#get_worker_documents_by_id)                   | Retrieve a list of documents of a worker.                                                                                                                                                                            |
+| [get_download_worker_documents_by_id](#get_download_worker_documents_by_id) | Get the download link of worker document.                                                                                                                                                                            |
+
+#### **request_exercise_equity**
+
+Create a request to exercise equity.
+
+- HTTP Method: `POST`
+- Endpoint: `/equity/exercise`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | ExerciseEquityToCreateContainer | ✅ | The request body. |
+
+**Return Type**
+
+`CreatedExerciseEquityContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import ExerciseEquityToCreateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = ExerciseEquityToCreateContainer(
+    fmv="fmv",
+    quantity=8.76,
+    issuer_id="issuer_id",
+    worker_id="worker_id",
+    address_zip="address_zip",
+    exercise_id="exercise_id",
+    address_city="address_city",
+    address_state="address_state",
+    address_street="address_street",
+    stakeholder_id="stakeholder_id",
+    address_country="address_country",
+    option_grant_id="option_grant_id",
+    fmv_currency_code="fmv_currency_code",
+    stakeholder_email="stakeholder_email",
+    option_grant_issue="option_grant_issue",
+    option_grant_label="option_grant_label",
+    option_grant_currency="option_grant_currency",
+    option_grant_issue_date="option_grant_issue_date",
+    option_grant_expiry_date="option_grant_expiry_date",
+    stakeholder_relationship="stakeholder_relationship",
+    option_grant_strike_price="option_grant_strike_price"
+)
+
+result = sdk.contracts.request_exercise_equity(request_body=request_body)
+
+print(result)
+```
+
+#### **approve_exercise_equity**
+
+Approve an equity exercise.
+
+- HTTP Method: `PATCH`
+- Endpoint: `/equity/exercise/{exercise_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | ExerciseEquityToUpdateContainer | ✅ | The request body. |
+| exercise_id | str | ✅ | Approve an equity exercise. |
+
+**Return Type**
+
+`UpdatedExerciseEquityContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import ExerciseEquityToUpdateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = ExerciseEquityToUpdateContainer(
+    employer_approval="employer_approval"
+)
+
+result = sdk.contracts.approve_exercise_equity(
+    request_body=request_body,
+    exercise_id="exercise_id"
+)
+
+print(result)
+```
+
+#### **get_contract_list**
+
+Retrieve a list of contracts.
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| after_cursor | str | ❌ | Retrieve a list of contracts. |
+| limit | float | ❌ | Retrieve a list of contracts. |
+| order_direction | SortDirEnum | ❌ | Retrieve a list of contracts. |
+| types | List[ContractTypeEnum] | ❌ | Retrieve a list of contracts. |
+| statuses | List[ContractStatusEnum] | ❌ | Retrieve a list of contracts. |
+| team_id | str | ❌ | Retrieve a list of contracts. |
+| external_id | str | ❌ | Retrieve a list of contracts. |
+| countries | List[str] | ❌ | Retrieve a list of contracts. |
+| currencies | GetContractListCurrencies | ❌ | Retrieve a list of contracts. |
+| search | str | ❌ | Retrieve a list of contracts. |
+| sort_by | ContractsSortByEnum | ❌ | Retrieve a list of contracts. |
+
+**Return Type**
+
+`ContractListContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import SortDirEnum, ContractsSortByEnum
+from deel_sdk.models.get_contract_list_currencies import List[str]
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+types=[
+    "ongoing_time_based"
+]
+statuses=[
+    "new"
+]
+countries=[
+    "US"
+]
+currencies=List[str](
+    [
+    "GBP"
+]
+)
+
+result = sdk.contracts.get_contract_list(
+    after_cursor="after_cursor",
+    limit=10,
+    order_direction="asc",
+    types=types,
+    statuses=statuses,
+    team_id="team_id",
+    external_id="external_id",
+    countries=countries,
+    currencies=currencies,
+    search="search",
+    sort_by="contract_title"
+)
+
+print(result)
+```
+
+#### **get_contract_by_id**
+
+Retrieve a single contract.
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts/{contract_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Retrieve a single contract. |
+
+**Return Type**
+
+`ContractContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.get_contract_by_id(contract_id="contract_id")
+
+print(result)
+```
+
+#### **attach_external_id**
+
+Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later.
+
+- HTTP Method: `PATCH`
+- Endpoint: `/contracts/{contract_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | InputToPatchContractExternalId | ✅ | The request body. |
+| contract_id | str | ✅ | Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later. |
+
+**Return Type**
+
+`GenericResultCreated`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import InputToPatchContractExternalId
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = InputToPatchContractExternalId(
+    data={
+        "external_id": "external_id"
+    }
+)
+
+result = sdk.contracts.attach_external_id(
+    request_body=request_body,
+    contract_id="contract_id"
+)
+
+print(result)
+```
+
+#### **add_contract_document**
+
+Attach a file to contract document.
+
+- HTTP Method: `POST`
+- Endpoint: `/contracts/{contract_id}/documents`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | dict | ❌ | The request body. |
+| contract_id | str | ✅ | Attach a file to contract document. |
+
+**Return Type**
+
+`ContractDocumentContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import FileObject
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = {
+    "file": "file"
+}
+
+result = sdk.contracts.add_contract_document(
+    request_body=request_body,
+    contract_id="contract_id"
+)
+
+print(result)
+```
+
+#### **edit_contract_document**
+
+Overwrite the file currently attached to contract document.
+
+- HTTP Method: `PUT`
+- Endpoint: `/contracts/{contract_id}/documents`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | dict | ❌ | The request body. |
+| contract_id | str | ✅ | Overwrite the file currently attached to contract document. |
+
+**Return Type**
+
+`ContractDocumentContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import FileObject
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = {
+    "file": "file"
+}
+
+result = sdk.contracts.edit_contract_document(
+    request_body=request_body,
+    contract_id="contract_id"
+)
+
+print(result)
+```
+
+#### **get_alternate_emails_by_contract_id**
+
+Returns an array of alternate email objects
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts/{contract_id}/alternate_emails`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Returns an array of alternate email objects |
+
+**Return Type**
+
+`List[AlternateEmailItem]`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.get_alternate_emails_by_contract_id(contract_id="contract_id")
+
+print(result)
+```
+
+#### **sign_contract**
+
+Sign a contract as a client.
+
+- HTTP Method: `POST`
+- Endpoint: `/contracts/{contract_id}/signatures`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | ContractSignatureToCreateContainer | ✅ | The request body. |
+| contract_id | str | ✅ | Sign a contract as a client. |
+
+**Return Type**
+
+`GenericResultCreated`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import ContractSignatureToCreateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = ContractSignatureToCreateContainer(
+    data={
+        "client_signature": "dolor enim in",
+        "contract_template_id": 2.41
+    }
+)
+
+result = sdk.contracts.sign_contract(
+    request_body=request_body,
+    contract_id="contract_id"
+)
+
+print(result)
+```
+
+#### **invite_to_sign_contract**
+
+Invite a worker to sign the contract. Worker will be notified via email.
+
+- HTTP Method: `POST`
+- Endpoint: `/contracts/{contract_id}/invitations`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | ContractInvitationToCreateContainer | ✅ | The request body. |
+| contract_id | str | ✅ | Invite a worker to sign the contract. Worker will be notified via email. |
+
+**Return Type**
+
+`GenericResultCreated`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import ContractInvitationToCreateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = ContractInvitationToCreateContainer(
+    data={
+        "email": "eiusmod",
+        "message": "nulla off"
+    }
+)
+
+result = sdk.contracts.invite_to_sign_contract(
+    request_body=request_body,
+    contract_id="contract_id"
+)
+
+print(result)
+```
+
+#### **uninvite_to_sign_contract**
+
+Remove invite in order to re-invite a worker to sign the contract.
+
+- HTTP Method: `DELETE`
+- Endpoint: `/contracts/{contract_id}/invitations`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Remove invite in order to re-invite a worker to sign the contract. |
+
+**Return Type**
+
+`GenericResultDeleted`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.uninvite_to_sign_contract(contract_id="contract_id")
+
+print(result)
+```
+
+#### **calculate_final_payment**
+
+Calculate the final payment due to the contractor when ending the contract.
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts/{contract_id}/final-payments`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Calculate the final payment due to the contractor when ending the contract. |
+| end_date | str | ❌ | Calculate the final payment due to the contractor when ending the contract. |
+| calculation_type | CalculateFinalPaymentCalculationType | ❌ | Calculate the final payment due to the contractor when ending the contract. |
+| workweek_start | str | ❌ | Calculate the final payment due to the contractor when ending the contract. |
+| workweek_end | str | ❌ | Calculate the final payment due to the contractor when ending the contract. |
+
+**Return Type**
+
+`FinalPaymentCalculatedContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import CalculateFinalPaymentCalculationType
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.calculate_final_payment(
+    contract_id="contract_id",
+    end_date="1999-12-31",
+    calculation_type="CUSTOM_AMOUNT",
+    workweek_start="workweek_start",
+    workweek_end="workweek_end"
+)
+
+print(result)
+```
+
+#### **post_contract_estimate**
+
+First payment is calculated from the number of working/calendar days between their start date and the start of the payment cycle.
+
+- HTTP Method: `POST`
+- Endpoint: `/contracts/estimate`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | EstimateFirstPaymentContainer | ✅ | The request body. |
+
+**Return Type**
+
+`ResponseEstimateFirstPaymentContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import EstimateFirstPaymentContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = EstimateFirstPaymentContainer(
+    data={
+        "type_": "ongoing_time_based",
+        "country_code": "US",
+        "start_date": "1999-12-31",
+        "compensation_details": {
+            "amount": 2500,
+            "currency_code": "GBP",
+            "scale": "weekly",
+            "cycle_end": 20.71,
+            "cycle_end_type": "DAY_OF_WEEK",
+            "payment_due_type": "REGULAR",
+            "payment_due_days": 16.18,
+            "calculation_type": "CUSTOM_AMOUNT",
+            "work_week_start": "Sunday",
+            "work_week_end": "Sunday"
+        }
+    }
+)
+
+result = sdk.contracts.post_contract_estimate(request_body=request_body)
+
+print(result)
+```
+
+#### **get_contract_templates**
+
+Retrieve a list of contract templates in your organization.
+
+- HTTP Method: `GET`
+- Endpoint: `/contract-templates`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+
+**Return Type**
+
+`ContractTemplateListContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.get_contract_templates()
+
+print(result)
+```
+
+#### **get_worker_documents_by_id**
+
+Retrieve a list of documents of a worker.
+
+- HTTP Method: `GET`
+- Endpoint: `/workers/{worker_id}/documents`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| worker_id | str | ✅ | Retrieve a list of documents of a worker. |
+
+**Return Type**
+
+`WorkerDocumentsByIdContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.get_worker_documents_by_id(worker_id="worker_id")
+
+print(result)
+```
+
+#### **get_download_worker_documents_by_id**
+
+Get the download link of worker document.
+
+- HTTP Method: `GET`
+- Endpoint: `/workers/{worker_id}/documents/{document_id}/download`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| worker_id | str | ✅ | Get the download link of worker document. |
+| document_id | float | ✅ | Get the download link of worker document. |
+
+**Return Type**
+
+`DownloadWorkerDocumentsByIdContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.get_download_worker_documents_by_id(
+    worker_id="worker_id",
+    document_id=6.05
+)
+
+print(result)
+```
+
+### OrganizationStructureService
+
+A list of all methods in the `OrganizationStructureService` service. Click on the method name to view detailed information about that method.
+
+| Methods                                                         | Description                                     |
+| :-------------------------------------------------------------- | :---------------------------------------------- |
+| [get_all_org_structures](#get_all_org_structures)               | Fetch all Org Structures from the Organization. |
+| [create_org_structure](#create_org_structure)                   | Create a new HRIS Organization Structure.       |
+| [get_org_structure](#get_org_structure)                         | Fetch an Org Structure from the Organization.   |
+| [update_org_structure](#update_org_structure)                   | Update an existing Organization structure.      |
+| [delete_org_structure](#delete_org_structure)                   | Delete an Org Structure from the Organization.  |
+| [get_external_org_structure](#get_external_org_structure)       | Fetch an Org Structure from the Organization.   |
+| [update_external_org_structure](#update_external_org_structure) | Update an existing Organization structure.      |
+| [delete_external_org_structure](#delete_external_org_structure) | Delete an Org Structure from the Organization.  |
+
+#### **get_all_org_structures**
+
+Fetch all Org Structures from the Organization.
+
+- HTTP Method: `GET`
+- Endpoint: `/hris/organization_structures`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+
+**Return Type**
+
+`GetAllOrgStructuresContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.organization_structure.get_all_org_structures()
+
+print(result)
+```
+
+#### **create_org_structure**
+
+Create a new HRIS Organization Structure.
+
+- HTTP Method: `POST`
+- Endpoint: `/hris/organization_structures`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | OrgStructureToCreateContainer | ✅ | The request body. |
+
+**Return Type**
+
+`GetAllOrgStructuresContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import OrgStructureToCreateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = OrgStructureToCreateContainer(
+    data={
+        "name": "name",
+        "teams": [
+            {
+                "name": "name",
+                "external_id": "external_id"
+            }
+        ],
+        "external_id": "external_id",
+        "enable_roles": True,
+        "is_multiple_select": True
+    }
+)
+
+result = sdk.organization_structure.create_org_structure(request_body=request_body)
+
+print(result)
+```
+
+#### **get_org_structure**
+
+Fetch an Org Structure from the Organization.
+
+- HTTP Method: `GET`
+- Endpoint: `/hris/organization_structures/{hrisOrgStr_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| hris_org_str_id | str | ✅ | Fetch an Org Structure from the Organization. |
+
+**Return Type**
+
+`GetOrgStructureContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.organization_structure.get_org_structure(hris_org_str_id="hrisOrgStr_id")
+
+print(result)
+```
+
+#### **update_org_structure**
+
+Update an existing Organization structure.
+
+- HTTP Method: `PATCH`
+- Endpoint: `/hris/organization_structures/{hrisOrgStr_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | OrgStructureToUpdateContainer | ✅ | The request body. |
+| hris_org_str_id | str | ✅ | Update an existing Organization structure. |
+
+**Return Type**
+
+`any`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import OrgStructureToUpdateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = OrgStructureToUpdateContainer(
+    data={
+        "name": "name",
+        "teams": [
+            {}
+        ],
+        "external_id": "external_id",
+        "enable_roles": False,
+        "is_multiselect": True
+    }
+)
+
+result = sdk.organization_structure.update_org_structure(
+    request_body=request_body,
+    hris_org_str_id="hrisOrgStr_id"
+)
+
+print(result)
+```
+
+#### **delete_org_structure**
+
+Delete an Org Structure from the Organization.
+
+- HTTP Method: `DELETE`
+- Endpoint: `/hris/organization_structures/{hrisOrgStr_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| hris_org_str_id | str | ✅ | Delete an Org Structure from the Organization. |
+
+**Return Type**
+
+`any`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.organization_structure.delete_org_structure(hris_org_str_id="hrisOrgStr_id")
+
+print(result)
+```
+
+#### **get_external_org_structure**
+
+Fetch an Org Structure from the Organization.
+
+- HTTP Method: `GET`
+- Endpoint: `/hris/organization_structures/external/{external_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| external_id | str | ✅ | Fetch an Org Structure from the Organization. |
+
+**Return Type**
+
+`GetOrgStructureContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.organization_structure.get_external_org_structure(external_id="external_id")
+
+print(result)
+```
+
+#### **update_external_org_structure**
+
+Update an existing Organization structure.
+
+- HTTP Method: `PATCH`
+- Endpoint: `/hris/organization_structures/external/{external_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | OrgStructureToUpdateContainer | ✅ | The request body. |
+| external_id | str | ✅ | Update an existing Organization structure. |
+
+**Return Type**
+
+`any`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import OrgStructureToUpdateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = OrgStructureToUpdateContainer(
+    data={
+        "name": "name",
+        "teams": [
+            {}
+        ],
+        "external_id": "external_id",
+        "enable_roles": False,
+        "is_multiselect": True
+    }
+)
+
+result = sdk.organization_structure.update_external_org_structure(
+    request_body=request_body,
+    external_id="external_id"
+)
+
+print(result)
+```
+
+#### **delete_external_org_structure**
+
+Delete an Org Structure from the Organization.
+
+- HTTP Method: `DELETE`
+- Endpoint: `/hris/organization_structures/external/{external_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| external_id | str | ✅ | Delete an Org Structure from the Organization. |
+
+**Return Type**
+
+`any`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.organization_structure.delete_external_org_structure(external_id="external_id")
+
+print(result)
+```
+
+### PositionsService
+
+A list of all methods in the `PositionsService` service. Click on the method name to view detailed information about that method.
+
+| Methods                                             | Description                                         |
+| :-------------------------------------------------- | :-------------------------------------------------- |
+| [get_positions](#get_positions)                     | HRIS Positions from a HrisProfile.                  |
+| [apply_changes_positions](#apply_changes_positions) | Apply add, edit, and delete operations to profiles. |
+
+#### **get_positions**
+
+HRIS Positions from a HrisProfile.
+
+- HTTP Method: `GET`
+- Endpoint: `/hris/positions/profile/{hrisProfile_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| hris_profile_id | str | ✅ | HRIS Positions from a HrisProfile. |
+
+**Return Type**
+
+`GetHrisPositionContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.positions.get_positions(hris_profile_id="hrisProfile_id")
+
+print(result)
+```
+
+#### **apply_changes_positions**
+
+Apply add, edit, and delete operations to profiles.
+
+- HTTP Method: `POST`
+- Endpoint: `/hris/positions/apply_changes`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | HrisPositionToChangeContainer | ✅ | The request body. |
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import HrisPositionToChangeContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = HrisPositionToChangeContainer(
+    data={
+        "add": [
+            {
+                "role_id": "role_id",
+                "team_id": "team_id",
+                "is_supportive": True
+            }
+        ],
+        "edit": [
+            {
+                "id_": "id",
+                "role_id": "role_id",
+                "is_supportive": False
+            }
+        ],
+        "delete": [
+            {
+                "id_": "id"
+            }
+        ],
+        "profile_id": "profile_id"
+    }
+)
+
+result = sdk.positions.apply_changes_positions(request_body=request_body)
+
+print(result)
+```
+
 ### ManagersService
 
 A list of all methods in the `ManagersService` service. Click on the method name to view detailed information about that method.
 
 | Methods                           | Description                        |
 | :-------------------------------- | :--------------------------------- |
 | [get_managers](#get_managers)     | List all organization managers.    |
@@ -399,21 +1965,21 @@
 from deel_sdk.models import AdminUserCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = AdminUserCreateContainer(**{
-    "data": {
-        "first_name": "dolore",
-        "last_name": "proi",
+request_body = AdminUserCreateContainer(
+    data={
+        "first_name": "mo",
+        "last_name": "Exce",
         "email": "email"
     }
-})
+)
 
 result = sdk.managers.create_manager(request_body=request_body)
 
 print(result)
 ```
 
 ### PeopleService
@@ -460,49 +2026,49 @@
 from deel_sdk.models import HrisDirectEmployee
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = HrisDirectEmployee(**{
-    "employee_details": {
+request_body = HrisDirectEmployee(
+    employee_details={
         "first_name": "John",
         "last_name": "Doe",
         "email": "john.doe@domain.com",
         "work_email": "john.doe@domain.com",
         "nationality": "CA",
         "country": "BR",
         "state": "AC"
     },
-    "team_information": {
-        "team_id": 9.77,
-        "legal_entity_id": 2.18
+    team_information={
+        "team_id": 9.17,
+        "legal_entity_id": 1.13
     },
-    "job_information": {
-        "seniority_id": 9.22,
-        "job_title_id": 6.5
+    job_information={
+        "seniority_id": 2.01,
+        "job_title_id": 6.94
     },
-    "compensation": {
-        "gross_annual_salary": 7.15,
+    compensation={
+        "gross_annual_salary": 4.71,
         "currency": "USD"
     },
-    "contract": {
+    contract={
         "contract_oid": "pdcMQe0cXCCXWTkqkdytw",
         "start_date": "1999-12-31",
-        "employee_number": 9.02,
+        "employee_number": 0.96,
         "end_date": "1999-12-31",
         "employment_type": "PART_TIME",
-        "part_time_percentage": 21.67
+        "part_time_percentage": 63.32
     },
-    "vacation_info": {
+    vacation_info={
         "vacation_accrual_start_date": "vacation_accrual_start_date",
-        "vacation_yearly_policy": 171.07
+        "vacation_yearly_policy": 214.98
     }
-})
+)
 
 result = sdk.people.create_direct_employee(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_internal_people_list**
@@ -529,16 +2095,16 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.people.get_internal_people_list(
-    offset=978653984.34,
-    limit=43.45
+    offset=664489591.67,
+    limit=128.61
 )
 
 print(result)
 ```
 
 #### **get_people_list**
 
@@ -569,16 +2135,16 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.people.get_people_list(
-    offset=44334375.53,
-    limit=105.69,
+    offset=772862704.51,
+    limit=142.31,
     search="search",
     sort_by="id",
     sort_order="asc",
     hiring_statuses="active"
 )
 
 print(result)
@@ -639,19 +2205,19 @@
 from deel_sdk.models import UpdateWorkerDepartmentContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = UpdateWorkerDepartmentContainer(**{
-    "data": {
+request_body = UpdateWorkerDepartmentContainer(
+    data={
         "department_id": "00000000-0000-0000-0000-000000000000"
     }
-})
+)
 
 result = sdk.people.update_people_department(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -681,19 +2247,19 @@
 from deel_sdk.models import UpdateWorkerWorkingLocationContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = UpdateWorkerWorkingLocationContainer(**{
-    "data": {
+request_body = UpdateWorkerWorkingLocationContainer(
+    data={
         "working_location_id": "00000000-0000-0000-0000-000000000000"
     }
-})
+)
 
 result = sdk.people.update_people_working_location(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -941,20 +2507,20 @@
 from deel_sdk.models import TimeoffToReviewInternalContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TimeoffToReviewInternalContainer(**{
-    "data": {
+request_body = TimeoffToReviewInternalContainer(
+    data={
         "status": "APPROVED",
         "reason": "Approved because there are no conflicts."
     }
-})
+)
 
 result = sdk.people.review_time_offs_for_employee(
     request_body=request_body,
     timeoff_id="timeoff_id",
     worker_id="worker_id"
 )
 
@@ -1125,27 +2691,27 @@
 from deel_sdk.models import EorEmployeeCostCalculationRequestBodyContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = EorEmployeeCostCalculationRequestBodyContainer(**{
-    "data": {
+request_body = EorEmployeeCostCalculationRequestBodyContainer(
+    data={
         "salary": 50000,
         "country": "Germany",
         "currency": "EUR",
         "benefits": [
             {
                 "provider_id": "00000000-0000-0000-0000-000000000000",
                 "plan_id": "00000000-0000-0000-0000-000000000000"
             }
         ]
     }
-})
+)
 
 result = sdk.eor.calculate_eor_employment_cost(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_eor_contract_benefits**
@@ -1202,16 +2768,16 @@
 from deel_sdk.models import EorContractToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = EorContractToCreateContainer(**{
-    "data": {
+request_body = EorContractToCreateContainer(
+    data={
         "employee": {
             "first_name": "Jane",
             "last_name": "Doe",
             "email": "employee@email.com",
             "nationality": "US",
             "address": {
                 "street": "Deel Street 500",
@@ -1224,49 +2790,49 @@
         "employment": {
             "country": "US",
             "state": "state",
             "type_": "Full-time",
             "work_visa_required": False,
             "start_date": "1999-12-31",
             "end_date": "1999-12-31",
-            "probation_period": 6.17,
+            "probation_period": 1.47,
             "scope_of_work": "scope_of_work",
             "time_off_type": "STANDARD",
-            "holidays": 5.67
+            "holidays": 0.98
         },
         "job_title": "job_title",
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "client": {
             "legal_entity": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "compensation_details": {
-            "salary": 5.95,
+            "salary": 3.09,
             "currency": "currency",
-            "variable_compensation": 3.49,
+            "variable_compensation": 6.88,
             "variable_compensation_type": "PERCENTAGE"
         },
         "quote_additional_fields": {
             "gender": "gender",
             "worker_type": "Skilled",
             "dob": "dob"
         },
         "health_plan_id": "health_plan_id",
         "pension": {
             "id_": "id",
             "contribution": "contribution"
         }
     }
-})
+)
 
 result = sdk.eor.create_eor_contract(request_body=request_body)
 
 print(result)
 ```
 
 ### GlobalPayrollService
@@ -1314,55 +2880,55 @@
 from deel_sdk.models import GpContractToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = GpContractToCreateContainer(**{
-    "data": {
+request_body = GpContractToCreateContainer(
+    data={
         "employee": {
             "first_name": "Jane",
             "last_name": "Doe",
-            "email": "culpa Lorem inc",
-            "work_email": "in do L",
+            "email": "esse no",
+            "work_email": "ipsum cillum c",
             "nationality": "US",
             "employee_number": "100",
             "address": {
                 "street": "Deel Street 500",
                 "city": "Denver",
                 "state": "CO",
                 "zip": "44000",
                 "country": "US"
             }
         },
         "employment": {
             "type_": "Full-time",
             "start_date": "1999-12-31",
             "holidays": {
-                "allowance": 5.28,
+                "allowance": 4.86,
                 "start_date": "1999-12-31"
             }
         },
         "job_title": "job_title",
         "client": {
             "legal_entity": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "compensation_details": {
             "scale": "YEAR",
-            "salary": 8.05,
+            "salary": 5.64,
             "currency": "GBP"
         }
     }
-})
+)
 
 result = sdk.global_payroll.create_gp_contract(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_worker_payslips**
@@ -1420,21 +2986,21 @@
 from deel_sdk.models import GpEmployeeAddressToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = GpEmployeeAddressToUpdateContainer(**{
-    "data": {
+request_body = GpEmployeeAddressToUpdateContainer(
+    data={
         "city": "London",
         "street": "123 Deel Street",
         "zip": "12345"
     }
-})
+)
 
 result = sdk.global_payroll.update_gp_employee_address(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -1495,16 +3061,16 @@
 from deel_sdk.models import AddWorkerBankAccountContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = AddWorkerBankAccountContainer(**{
-    "data": {
+request_body = AddWorkerBankAccountContainer(
+    data={
         "full_name": "John Doe",
         "phone": "+1234567890",
         "address_line1": "1234 Main St",
         "address_line2": "Apartment 101",
         "city": "Springfield",
         "province_state": "Ontario",
         "postal": "12345",
@@ -1521,15 +3087,15 @@
         "bank_branch_name": "Main Street Branch",
         "iban": "GB29NWBK60161331926819",
         "email": "john.doe@example.com",
         "rib_number": "12345678901",
         "account_type": "12345678901",
         "ach_routing_number": "12345678901"
     }
-})
+)
 
 result = sdk.global_payroll.add_gp_bank_account(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -1560,16 +3126,16 @@
 from deel_sdk.models import AddWorkerBankAccountContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = AddWorkerBankAccountContainer(**{
-    "data": {
+request_body = AddWorkerBankAccountContainer(
+    data={
         "full_name": "John Doe",
         "phone": "+1234567890",
         "address_line1": "1234 Main St",
         "address_line2": "Apartment 101",
         "city": "Springfield",
         "province_state": "Ontario",
         "postal": "12345",
@@ -1586,15 +3152,15 @@
         "bank_branch_name": "Main Street Branch",
         "iban": "GB29NWBK60161331926819",
         "email": "john.doe@example.com",
         "rib_number": "12345678901",
         "account_type": "12345678901",
         "ach_routing_number": "12345678901"
     }
-})
+)
 
 result = sdk.global_payroll.patch_gp_bank_account(
     request_body=request_body,
     worker_id="worker_id",
     bank_id="bank_id"
 )
 
@@ -1656,21 +3222,21 @@
 from deel_sdk.models import GpEmployeeCompensationToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = GpEmployeeCompensationToUpdateContainer(**{
-    "data": {
+request_body = GpEmployeeCompensationToUpdateContainer(
+    data={
         "scale": "YEAR",
         "salary": 50000,
         "effective_date": "1999-12-31"
     }
-})
+)
 
 result = sdk.global_payroll.update_gp_employee_compensation(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -1700,20 +3266,20 @@
 from deel_sdk.models import GpEmployeePtoToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = GpEmployeePtoToUpdateContainer(**{
-    "data": {
+request_body = GpEmployeePtoToUpdateContainer(
+    data={
         "accrual_start_date": "1999-12-31",
         "yearly_allowance": "15"
     }
-})
+)
 
 result = sdk.global_payroll.update_gp_employee_pto(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -1743,25 +3309,25 @@
 from deel_sdk.models import GpEmployeeInformationToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = GpEmployeeInformationToUpdateContainer(**{
-    "data": {
+request_body = GpEmployeeInformationToUpdateContainer(
+    data={
         "first_name": "Jane",
         "middle_name": "Jay",
         "last_name": "Doe",
         "date_of_birth": "1999-12-31",
         "gender": "gender",
         "marital_status": "Single",
         "employee_number": "employee_number"
     }
-})
+)
 
 result = sdk.global_payroll.update_gp_employee_information(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -1924,23 +3490,23 @@
 from deel_sdk.models import WorkerTerminationBodyContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = WorkerTerminationBodyContainer(**{
-    "data": {
+request_body = WorkerTerminationBodyContainer(
+    data={
         "desired_end_date": "2023-12-31",
         "last_date_of_work": "2023-12-31",
         "message": "Termination reason",
         "is_voluntary": True,
         "severance": {}
     }
-})
+)
 
 result = sdk.global_payroll.request_termination(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -1986,16 +3552,16 @@
 from deel_sdk.models import ContractToCreateContainerPayAsYouGoTimeBased
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToCreateContainerPayAsYouGoTimeBased(**{
-    "data": {
+request_body = ContractToCreateContainerPayAsYouGoTimeBased(
+    data={
         "title": "title",
         "country_code": "US",
         "state_code": "state_code",
         "scope_of_work": "scope_of_work",
         "special_clause": "special_clause",
         "termination_date": "1999-12-31",
         "client": {
@@ -2003,50 +3569,50 @@
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
-            "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "sedDuis officia est laborum in"
+            "id_": "id",
+            "name": "in labore officia non veniam"
         },
         "seniority": {
-            "id_": "00000000-0000-0000-0000-000000000000"
+            "id_": 5.48
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "occae",
+            "expected_email": "adipisicing",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "pay_as_you_go_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 2.6,
+            "amount": 0.13,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
             "first_payment_date": "1999-12-31",
             "first_payment": 500,
             "notice_period": 15,
             "scale": "hourly"
         }
     }
-})
+)
 
 result = sdk.contractors.create_contract_time_based(request_body=request_body)
 
 print(result)
 ```
 
 #### **create_contract_task_based**
@@ -2072,16 +3638,16 @@
 from deel_sdk.models import ContractToCreateContainerPaygTasks
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToCreateContainerPaygTasks(**{
-    "data": {
+request_body = ContractToCreateContainerPaygTasks(
+    data={
         "title": "title",
         "country_code": "US",
         "state_code": "state_code",
         "scope_of_work": "scope_of_work",
         "special_clause": "special_clause",
         "termination_date": "1999-12-31",
         "client": {
@@ -2089,29 +3655,29 @@
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
-            "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "enim irure dolore magna"
+            "id_": "id",
+            "name": "irure"
         },
         "seniority": {
-            "id_": "00000000-0000-0000-0000-000000000000"
+            "id_": 5.89
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "Duis nulla oc",
+            "expected_email": "in Ex",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "payg_tasks",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 100,
@@ -2123,15 +3689,15 @@
             "payment_due_days": 7,
             "pay_before_weekends": True,
             "first_payment_date": "1999-12-31",
             "first_payment": 500,
             "notice_period": 15
         }
     }
-})
+)
 
 result = sdk.contractors.create_contract_task_based(request_body=request_body)
 
 print(result)
 ```
 
 #### **create_contract_milestone_based**
@@ -2157,16 +3723,16 @@
 from deel_sdk.models import ContractToCreateContainerPaygMilestones
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToCreateContainerPaygMilestones(**{
-    "data": {
+request_body = ContractToCreateContainerPaygMilestones(
+    data={
         "title": "title",
         "country_code": "US",
         "state_code": "state_code",
         "scope_of_work": "scope_of_work",
         "special_clause": "special_clause",
         "termination_date": "1999-12-31",
         "client": {
@@ -2174,29 +3740,29 @@
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
-            "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "et dolore"
+            "id_": "id",
+            "name": "pariatur"
         },
         "seniority": {
-            "id_": "00000000-0000-0000-0000-000000000000"
+            "id_": 8.01
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "sint ",
+            "expected_email": "aute dolor",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "payg_milestones",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 100,
@@ -2208,15 +3774,15 @@
             "payment_due_days": 7,
             "pay_before_weekends": True,
             "first_payment_date": "1999-12-31",
             "first_payment": 500,
             "notice_period": 15
         }
     }
-})
+)
 
 result = sdk.contractors.create_contract_milestone_based(request_body=request_body)
 
 print(result)
 ```
 
 #### **create_contract_fixed_rate**
@@ -2242,16 +3808,16 @@
 from deel_sdk.models import ContractToCreateContainerOngoingTimeBased
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToCreateContainerOngoingTimeBased(**{
-    "data": {
+request_body = ContractToCreateContainerOngoingTimeBased(
+    data={
         "title": "title",
         "country_code": "US",
         "state_code": "state_code",
         "scope_of_work": "scope_of_work",
         "special_clause": "special_clause",
         "termination_date": "1999-12-31",
         "client": {
@@ -2259,50 +3825,50 @@
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
-            "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "cillum"
+            "id_": "id",
+            "name": "proident fugiat est aliquip elit"
         },
         "seniority": {
-            "id_": "00000000-0000-0000-0000-000000000000"
+            "id_": 6.6
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "Lorem sint et",
+            "expected_email": "nisiet lab",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "ongoing_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 7.36,
+            "amount": 9.2,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
             "first_payment_date": "1999-12-31",
             "first_payment": 500,
             "notice_period": 15,
             "scale": "hourly"
         }
     }
-})
+)
 
 result = sdk.contractors.create_contract_fixed_rate(request_body=request_body)
 
 print(result)
 ```
 
 #### **create_contract**
@@ -2328,16 +3894,16 @@
 from deel_sdk.models import ContractToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToCreateContainer(**{
-    "data": {
+request_body = ContractToCreateContainer(
+    data={
         "title": "title",
         "country_code": "US",
         "state_code": "state_code",
         "scope_of_work": "scope_of_work",
         "special_clause": "special_clause",
         "termination_date": "1999-12-31",
         "client": {
@@ -2345,50 +3911,50 @@
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
-            "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "sedDuis officia est laborum in"
+            "id_": "id",
+            "name": "in labore officia non veniam"
         },
         "seniority": {
-            "id_": "00000000-0000-0000-0000-000000000000"
+            "id_": 5.48
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "occae",
+            "expected_email": "adipisicing",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "pay_as_you_go_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 2.6,
+            "amount": 0.13,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
             "first_payment_date": "1999-12-31",
             "first_payment": 500,
             "notice_period": 15,
             "scale": "hourly"
         }
     }
-})
+)
 
 result = sdk.contractors.create_contract(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_contract_preview**
@@ -2451,35 +4017,35 @@
 from deel_sdk.models import ContractToAmendDetailsContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToAmendDetailsContainer(**{
-    "data": {
+request_body = ContractToAmendDetailsContainer(
+    data={
         "amount": 100,
         "currency_code": "GBP",
         "scale": "hourly",
         "effective_date": "1999-12-31",
         "first_payment_date": "1999-12-31",
-        "first_payment": 0.24,
+        "first_payment": 4.5,
         "frequency": "weekly",
-        "cycle_end": 24.94,
+        "cycle_end": 3.38,
         "cycle_end_type": "DAY_OF_WEEK",
         "payment_due_type": "REGULAR",
-        "payment_due_days": 0.92,
-        "pay_before_weekends": True,
+        "payment_due_days": 83.14,
+        "pay_before_weekends": False,
         "job_title_name": "3D Designer",
         "job_title_id": "00000000-0000-0000-0000-000000000000",
         "seniority_id": "00000000-0000-0000-0000-000000000000",
         "special_clause": "special_clause",
         "scope_of_work": "scope_of_work"
     }
-})
+)
 
 result = sdk.contractors.amend_contract_details(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -2509,21 +4075,21 @@
 from deel_sdk.models import ContractToTerminateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToTerminateContainer(**{
-    "data": {
+request_body = ContractToTerminateContainer(
+    data={
         "completion_date": "1999-12-31",
         "terminate_now": True,
         "message": "message"
     }
-})
+)
 
 result = sdk.contractors.terminate_contract(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -2553,20 +4119,20 @@
 from deel_sdk.models import PremiumToAddContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = PremiumToAddContainer(**{
-    "data": {
+request_body = PremiumToAddContainer(
+    data={
         "agreement_reflects_relation": True,
         "contractor_characteristics": True
     }
-})
+)
 
 result = sdk.contractors.add_premium(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -2647,20 +4213,20 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = {
     "data": {
         "contract_id": "m3jk2j",
-        "amount": "cupidatat exe",
+        "amount": "labore",
         "date_of_adjustment": "1999-12-31",
         "title": "Your title here",
         "description": "Your description here",
         "cycle_reference": "my_cycle_reference",
-        "file": "qu",
+        "file": "ut",
         "adjustment_category_id": "c9cf4c2c0165f48f494415390c3b49",
         "move_next_cycle": True,
         "vendor": "Vendor",
         "country": "US"
     }
 }
 
@@ -2724,22 +4290,22 @@
 from deel_sdk.models import AdjustmentToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = AdjustmentToUpdateContainer(**{
-    "data": {
-        "amount": "ut velit in",
+request_body = AdjustmentToUpdateContainer(
+    data={
+        "amount": "ad aute d",
         "title": "Your title here",
         "description": "Your description here",
-        "file": "incididunt "
+        "file": "in ulla"
     }
-})
+)
 
 result = sdk.adjustments.update_adjustment(
     request_body=request_body,
     adjustment_id="adjustment_id"
 )
 
 print(result)
@@ -2829,19 +4395,19 @@
 from deel_sdk.models import InputToCreateFileRef
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = InputToCreateFileRef(**{
-    "data": {
+request_body = InputToCreateFileRef(
+    data={
         "content_type": "application/pdf"
     }
-})
+)
 
 result = sdk.adjustments.create_file_ref(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_adjustments**
@@ -2913,29 +4479,29 @@
 from deel_sdk.models import CandidateToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CandidateToCreateContainer(**{
-    "data": {
+request_body = CandidateToCreateContainer(
+    data={
         "id_": "id",
         "first_name": "John",
         "last_name": "Doe",
         "status": "offer-accepted",
         "start_date": "1999-12-31",
         "link": "link",
         "job_title": "3D Designer",
-        "email": "dolore",
+        "email": "do te",
         "nationality": "US",
         "country": "US",
         "state": "AL"
     }
-})
+)
 
 result = sdk.candidates.add_candidate(request_body=request_body)
 
 print(result)
 ```
 
 #### **patch_candidate**
@@ -2962,28 +4528,28 @@
 from deel_sdk.models import CandidateToPatchContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CandidateToPatchContainer(**{
-    "data": {
+request_body = CandidateToPatchContainer(
+    data={
         "first_name": "John",
         "last_name": "Doe",
         "status": "offer-accepted",
         "start_date": "1999-12-31",
         "job_title": "3D Designer",
         "link": "link",
-        "email": "Excepteur nu",
+        "email": "dolor",
         "nationality": "US",
         "country": "US",
         "state": "AL"
     }
-})
+)
 
 result = sdk.candidates.patch_candidate(
     request_body=request_body,
     candidate_id="candidate_id"
 )
 
 print(result)
@@ -3037,17 +4603,17 @@
 from deel_sdk.models import AdditionalEorInfoContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = AdditionalEorInfoContainer(**{
-    "data": ""
-})
+request_body = AdditionalEorInfoContainer(
+    data=""
+)
 
 result = sdk.partner_managed.add_employee_additional_information(
     request_body=request_body,
     employee_id="employee_id",
     contract_id="contract_id"
 )
 
@@ -3079,19 +4645,19 @@
 from deel_sdk.models import EmployeeContractSignatureToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = EmployeeContractSignatureToCreateContainer(**{
-    "data": {
-        "signature": "aliqua sed comm"
+request_body = EmployeeContractSignatureToCreateContainer(
+    data={
+        "signature": "cil"
     }
-})
+)
 
 result = sdk.partner_managed.sign_employee_contract(
     request_body=request_body,
     employee_id="employee_id",
     contract_id="contract_id"
 )
 
@@ -3123,21 +4689,21 @@
 from deel_sdk.models import RequestCustomVerificationLetterContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = RequestCustomVerificationLetterContainer(**{
-    "data": {
-        "description": "magnaest ea con",
+request_body = RequestCustomVerificationLetterContainer(
+    data={
+        "description": "ipsum suntullam",
         "include_qr_code": True,
         "type_": "VISA_APPLICATION_FOR_PERSONAL_TRIP"
     }
-})
+)
 
 result = sdk.partner_managed.request_custom_verification_letter(
     request_body=request_body,
     employee_id="employee_id",
     contract_id="contract_id"
 )
 
@@ -3206,15 +4772,15 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.partner_managed.download_hr_verification_letters_and_documents(
     employee_id="employee_id",
     contract_id="contract_id",
-    document_id=1.72
+    document_id=2.54
 )
 
 print(result)
 ```
 
 #### **get_offer_letter_preview**
 
@@ -3378,22 +4944,22 @@
 from deel_sdk.models import BankAccountToAddContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = BankAccountToAddContainer(**{
-    "data": [
+request_body = BankAccountToAddContainer(
+    data=[
         {
             "key": "key",
             "value": "value"
         }
     ]
-})
+)
 
 result = sdk.partner_managed.add_bank_account(
     request_body=request_body,
     employee_id="employee_id"
 )
 
 print(result)
@@ -3424,22 +4990,22 @@
 from deel_sdk.models import BankAccountToAddContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = BankAccountToAddContainer(**{
-    "data": [
+request_body = BankAccountToAddContainer(
+    data=[
         {
             "key": "key",
             "value": "value"
         }
     ]
-})
+)
 
 result = sdk.partner_managed.patch_bank_account(
     request_body=request_body,
     employee_id="employee_id",
     bank_id="bank_id"
 )
 
@@ -3540,15 +5106,15 @@
 request_body = {
     "file": "file"
 }
 
 result = sdk.partner_managed.upload_employee_compliance_document(
     request_body=request_body,
     employee_id="employee_id",
-    document_id=1.36
+    document_id=7.6
 )
 
 print(result)
 ```
 
 #### **get_employee_compliance_document_template**
 
@@ -3575,15 +5141,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.partner_managed.get_employee_compliance_document_template(
     employee_id="employee_id",
-    document_id=5.91
+    document_id=4.09
 )
 
 print(result)
 ```
 
 #### **get_employee_tax_documents**
 
@@ -3612,592 +5178,14 @@
 )
 
 result = sdk.partner_managed.get_employee_tax_documents(employee_id="employee_id")
 
 print(result)
 ```
 
-### ContractsService
-
-A list of all methods in the `ContractsService` service. Click on the method name to view detailed information about that method.
-
-| Methods                                                                     | Description                                                                                                                                                                                                          |
-| :-------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| [get_contract_list](#get_contract_list)                                     | Retrieve a list of contracts.                                                                                                                                                                                        |
-| [get_contract_by_id](#get_contract_by_id)                                   | Retrieve a single contract.                                                                                                                                                                                          |
-| [attach_external_id](#attach_external_id)                                   | Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later. |
-| [add_contract_document](#add_contract_document)                             | Attach a file to contract document.                                                                                                                                                                                  |
-| [edit_contract_document](#edit_contract_document)                           | Overwrite the file currently attached to contract document.                                                                                                                                                          |
-| [get_alternate_emails_by_contract_id](#get_alternate_emails_by_contract_id) | Returns an array of alternate email objects                                                                                                                                                                          |
-| [sign_contract](#sign_contract)                                             | Sign a contract as a client.                                                                                                                                                                                         |
-| [invite_to_sign_contract](#invite_to_sign_contract)                         | Invite a worker to sign the contract. Worker will be notified via email.                                                                                                                                             |
-| [uninvite_to_sign_contract](#uninvite_to_sign_contract)                     | Remove invite in order to re-invite a worker to sign the contract.                                                                                                                                                   |
-| [calculate_final_payment](#calculate_final_payment)                         | Calculate the final payment due to the contractor when ending the contract.                                                                                                                                          |
-| [post_contract_estimate](#post_contract_estimate)                           | First payment is calculated from the number of working/calendar days between their start date and the start of the payment cycle.                                                                                    |
-| [get_contract_templates](#get_contract_templates)                           | Retrieve a list of contract templates in your organization.                                                                                                                                                          |
-| [get_worker_documents_by_id](#get_worker_documents_by_id)                   | Retrieve a list of documents of a worker.                                                                                                                                                                            |
-| [get_download_worker_documents_by_id](#get_download_worker_documents_by_id) | Get the download link of worker document.                                                                                                                                                                            |
-
-#### **get_contract_list**
-
-Retrieve a list of contracts.
-
-- HTTP Method: `GET`
-- Endpoint: `/contracts`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| after_cursor | str | ❌ | Retrieve a list of contracts. |
-| limit | float | ❌ | Retrieve a list of contracts. |
-| order_direction | SortDirEnum | ❌ | Retrieve a list of contracts. |
-| types | List[ContractTypeEnum] | ❌ | Retrieve a list of contracts. |
-| statuses | List[ContractStatusEnum] | ❌ | Retrieve a list of contracts. |
-| team_id | str | ❌ | Retrieve a list of contracts. |
-| external_id | str | ❌ | Retrieve a list of contracts. |
-| countries | List[str] | ❌ | Retrieve a list of contracts. |
-| currencies | GetContractListCurrencies | ❌ | Retrieve a list of contracts. |
-| search | str | ❌ | Retrieve a list of contracts. |
-| sort_by | ContractsSortByEnum | ❌ | Retrieve a list of contracts. |
-
-**Return Type**
-
-`ContractListContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import SortDirEnum, GetContractListCurrencies, ContractsSortByEnum
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-types=[
-    "ongoing_time_based"
-]
-statuses=[
-    "new"
-]
-countries=[
-    "US"
-]
-currencies=GetContractListCurrencies(**[
-    "GBP"
-])
-
-result = sdk.contracts.get_contract_list(
-    after_cursor="after_cursor",
-    limit=10,
-    order_direction="asc",
-    types=types,
-    statuses=statuses,
-    team_id="team_id",
-    external_id="external_id",
-    countries=countries,
-    currencies=currencies,
-    search="search",
-    sort_by="contract_title"
-)
-
-print(result)
-```
-
-#### **get_contract_by_id**
-
-Retrieve a single contract.
-
-- HTTP Method: `GET`
-- Endpoint: `/contracts/{contract_id}`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| contract_id | str | ✅ | Retrieve a single contract. |
-
-**Return Type**
-
-`ContractContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.get_contract_by_id(contract_id="contract_id")
-
-print(result)
-```
-
-#### **attach_external_id**
-
-Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later.
-
-- HTTP Method: `PATCH`
-- Endpoint: `/contracts/{contract_id}`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | InputToPatchContractExternalId | ✅ | The request body. |
-| contract_id | str | ✅ | Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later. |
-
-**Return Type**
-
-`GenericResultCreated`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import InputToPatchContractExternalId
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-request_body = InputToPatchContractExternalId(**{
-    "data": {
-        "external_id": "external_id"
-    }
-})
-
-result = sdk.contracts.attach_external_id(
-    request_body=request_body,
-    contract_id="contract_id"
-)
-
-print(result)
-```
-
-#### **add_contract_document**
-
-Attach a file to contract document.
-
-- HTTP Method: `POST`
-- Endpoint: `/contracts/{contract_id}/documents`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | dict | ❌ | The request body. |
-| contract_id | str | ✅ | Attach a file to contract document. |
-
-**Return Type**
-
-`ContractDocumentContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import FileObject
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-request_body = {
-    "file": "file"
-}
-
-result = sdk.contracts.add_contract_document(
-    request_body=request_body,
-    contract_id="contract_id"
-)
-
-print(result)
-```
-
-#### **edit_contract_document**
-
-Overwrite the file currently attached to contract document.
-
-- HTTP Method: `PUT`
-- Endpoint: `/contracts/{contract_id}/documents`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | dict | ❌ | The request body. |
-| contract_id | str | ✅ | Overwrite the file currently attached to contract document. |
-
-**Return Type**
-
-`ContractDocumentContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import FileObject
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-request_body = {
-    "file": "file"
-}
-
-result = sdk.contracts.edit_contract_document(
-    request_body=request_body,
-    contract_id="contract_id"
-)
-
-print(result)
-```
-
-#### **get_alternate_emails_by_contract_id**
-
-Returns an array of alternate email objects
-
-- HTTP Method: `GET`
-- Endpoint: `/contracts/{contract_id}/alternate_emails`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| contract_id | str | ✅ | Returns an array of alternate email objects |
-
-**Return Type**
-
-`List[AlternateEmailItem]`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.get_alternate_emails_by_contract_id(contract_id="contract_id")
-
-print(result)
-```
-
-#### **sign_contract**
-
-Sign a contract as a client.
-
-- HTTP Method: `POST`
-- Endpoint: `/contracts/{contract_id}/signatures`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | ContractSignatureToCreateContainer | ✅ | The request body. |
-| contract_id | str | ✅ | Sign a contract as a client. |
-
-**Return Type**
-
-`GenericResultCreated`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import ContractSignatureToCreateContainer
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-request_body = ContractSignatureToCreateContainer(**{
-    "data": {
-        "client_signature": "ea exercitat",
-        "contract_template_id": 8.35
-    }
-})
-
-result = sdk.contracts.sign_contract(
-    request_body=request_body,
-    contract_id="contract_id"
-)
-
-print(result)
-```
-
-#### **invite_to_sign_contract**
-
-Invite a worker to sign the contract. Worker will be notified via email.
-
-- HTTP Method: `POST`
-- Endpoint: `/contracts/{contract_id}/invitations`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | ContractInvitationToCreateContainer | ✅ | The request body. |
-| contract_id | str | ✅ | Invite a worker to sign the contract. Worker will be notified via email. |
-
-**Return Type**
-
-`GenericResultCreated`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import ContractInvitationToCreateContainer
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-request_body = ContractInvitationToCreateContainer(**{
-    "data": {
-        "email": "eiusm",
-        "message": "officia ut"
-    }
-})
-
-result = sdk.contracts.invite_to_sign_contract(
-    request_body=request_body,
-    contract_id="contract_id"
-)
-
-print(result)
-```
-
-#### **uninvite_to_sign_contract**
-
-Remove invite in order to re-invite a worker to sign the contract.
-
-- HTTP Method: `DELETE`
-- Endpoint: `/contracts/{contract_id}/invitations`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| contract_id | str | ✅ | Remove invite in order to re-invite a worker to sign the contract. |
-
-**Return Type**
-
-`GenericResultDeleted`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.uninvite_to_sign_contract(contract_id="contract_id")
-
-print(result)
-```
-
-#### **calculate_final_payment**
-
-Calculate the final payment due to the contractor when ending the contract.
-
-- HTTP Method: `GET`
-- Endpoint: `/contracts/{contract_id}/final-payments`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| contract_id | str | ✅ | Calculate the final payment due to the contractor when ending the contract. |
-| end_date | str | ❌ | Calculate the final payment due to the contractor when ending the contract. |
-| calculation_type | CalculateFinalPaymentCalculationType | ❌ | Calculate the final payment due to the contractor when ending the contract. |
-| workweek_start | str | ❌ | Calculate the final payment due to the contractor when ending the contract. |
-| workweek_end | str | ❌ | Calculate the final payment due to the contractor when ending the contract. |
-
-**Return Type**
-
-`FinalPaymentCalculatedContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import CalculateFinalPaymentCalculationType
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.calculate_final_payment(
-    contract_id="contract_id",
-    end_date="1999-12-31",
-    calculation_type="CUSTOM_AMOUNT",
-    workweek_start="workweek_start",
-    workweek_end="workweek_end"
-)
-
-print(result)
-```
-
-#### **post_contract_estimate**
-
-First payment is calculated from the number of working/calendar days between their start date and the start of the payment cycle.
-
-- HTTP Method: `POST`
-- Endpoint: `/contracts/estimate`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | EstimateFirstPaymentContainer | ✅ | The request body. |
-
-**Return Type**
-
-`ResponseEstimateFirstPaymentContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import EstimateFirstPaymentContainer
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-request_body = EstimateFirstPaymentContainer(**{
-    "data": {
-        "type_": "ongoing_time_based",
-        "country_code": "US",
-        "start_date": "1999-12-31",
-        "compensation_details": {
-            "amount": 2500,
-            "currency_code": "GBP",
-            "scale": "weekly",
-            "cycle_end": 30.28,
-            "cycle_end_type": "DAY_OF_WEEK",
-            "payment_due_type": "REGULAR",
-            "payment_due_days": 11.81,
-            "calculation_type": "CUSTOM_AMOUNT",
-            "work_week_start": "Sunday",
-            "work_week_end": "Sunday"
-        }
-    }
-})
-
-result = sdk.contracts.post_contract_estimate(request_body=request_body)
-
-print(result)
-```
-
-#### **get_contract_templates**
-
-Retrieve a list of contract templates in your organization.
-
-- HTTP Method: `GET`
-- Endpoint: `/contract-templates`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-
-**Return Type**
-
-`ContractTemplateListContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.get_contract_templates()
-
-print(result)
-```
-
-#### **get_worker_documents_by_id**
-
-Retrieve a list of documents of a worker.
-
-- HTTP Method: `GET`
-- Endpoint: `/workers/{worker_id}/documents`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| worker_id | str | ✅ | Retrieve a list of documents of a worker. |
-
-**Return Type**
-
-`WorkerDocumentsByIdContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.get_worker_documents_by_id(worker_id="worker_id")
-
-print(result)
-```
-
-#### **get_download_worker_documents_by_id**
-
-Get the download link of worker document.
-
-- HTTP Method: `GET`
-- Endpoint: `/workers/{worker_id}/documents/{document_id}/download`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| worker_id | str | ✅ | Get the download link of worker document. |
-| document_id | float | ✅ | Get the download link of worker document. |
-
-**Return Type**
-
-`DownloadWorkerDocumentsByIdContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.get_download_worker_documents_by_id(
-    worker_id="worker_id",
-    document_id=8.43
-)
-
-print(result)
-```
-
 ### TasksService
 
 A list of all methods in the `TasksService` service. Click on the method name to view detailed information about that method.
 
 | Methods                                               | Description                                                     |
 | :---------------------------------------------------- | :-------------------------------------------------------------- |
 | [get_tasks_by_contract](#get_tasks_by_contract)       | Retrieve a list of tasks for a given contract.                  |
@@ -4261,25 +5249,25 @@
 from deel_sdk.models import InputToCreatePgoTask
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = InputToCreatePgoTask(**{
-    "data": {
+request_body = InputToCreatePgoTask(
+    data={
         "amount": "123.45",
         "date_submitted": "1999-12-31",
         "description": "Make the button pop.",
         "attachment": {
             "filename": "filename",
             "key": "key"
         }
     }
-})
+)
 
 result = sdk.tasks.create_contract_pgo_tak(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -4309,23 +5297,23 @@
 from deel_sdk.models import RequestBodyToCreatePgoTaskReviewsReviewsContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = RequestBodyToCreatePgoTaskReviewsReviewsContainer(**{
-    "data": {
+request_body = RequestBodyToCreatePgoTaskReviewsReviewsContainer(
+    data={
         "status": "approved",
         "reason": "Great work.",
         "ids": [
             "00000000-0000-0000-0000-000000000000"
         ]
     }
-})
+)
 
 result = sdk.tasks.create_task_many_review(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -4356,20 +5344,20 @@
 from deel_sdk.models import RequestBodyToCreatePgoTaskReviewsByIdReviewsContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = RequestBodyToCreatePgoTaskReviewsByIdReviewsContainer(**{
-    "data": {
+request_body = RequestBodyToCreatePgoTaskReviewsByIdReviewsContainer(
+    data={
         "status": "approved",
         "reason": "Excited!"
     }
-})
+)
 
 result = sdk.tasks.create_task_review_by_id(
     request_body=request_body,
     contract_id="contract_id",
     task_id="task_id"
 )
 
@@ -4471,15 +5459,15 @@
     contract_id="contract_id",
     contract_types=contract_types,
     statuses=statuses,
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=99,
-    offset=564786626.18
+    offset=38650248.43
 )
 
 print(result)
 ```
 
 #### **get_timesheets**
 
@@ -4524,15 +5512,15 @@
     contract_id="contract_id",
     contract_types=contract_types,
     statuses=statuses,
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=99,
-    offset=911169937.96
+    offset=530446812.74
 )
 
 print(result)
 ```
 
 #### **create_timesheet**
 
@@ -4557,22 +5545,22 @@
 from deel_sdk.models import TimesheetToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TimesheetToCreateContainer(**{
-    "data": {
+request_body = TimesheetToCreateContainer(
+    data={
         "contract_id": "contract_id",
         "description": "description",
         "date_submitted": "1999-12-31",
         "quantity": 2
     }
-})
+)
 
 result = sdk.timesheets.create_timesheet(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_timesheet_by_id**
@@ -4630,20 +5618,20 @@
 from deel_sdk.models import TimesheetToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TimesheetToUpdateContainer(**{
-    "data": {
+request_body = TimesheetToUpdateContainer(
+    data={
         "description": "description",
-        "quantity": 3.77
+        "quantity": 8.4
     }
-})
+)
 
 result = sdk.timesheets.update_timesheet_by_id(
     request_body=request_body,
     timesheet_id="timesheet_id"
 )
 
 print(result)
@@ -4708,20 +5696,20 @@
 from deel_sdk.models import TimesheetReviewToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TimesheetReviewToCreateContainer(**{
-    "data": {
+request_body = TimesheetReviewToCreateContainer(
+    data={
         "status": "approved",
         "reason": "reason"
     }
-})
+)
 
 result = sdk.timesheets.create_timesheet_review(
     request_body=request_body,
     timesheet_id="timesheet_id"
 )
 
 print(result)
@@ -4750,23 +5738,23 @@
 from deel_sdk.models import TimesheetReviewsToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TimesheetReviewsToCreateContainer(**{
-    "data": {
+request_body = TimesheetReviewsToCreateContainer(
+    data={
         "status": "approved",
         "reason": "reason",
         "ids": [
-            1.77
+            8.09
         ]
     }
-})
+)
 
 result = sdk.timesheets.create_timesheet_reviews(request_body=request_body)
 
 print(result)
 ```
 
 ### MilestonesService
@@ -4837,21 +5825,21 @@
 from deel_sdk.models import MilestoneToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = MilestoneToCreateContainer(**{
-    "data": {
+request_body = MilestoneToCreateContainer(
+    data={
         "amount": "900.00",
         "title": "Sprint 2",
         "description": "Sprint #2"
     }
-})
+)
 
 result = sdk.milestones.create_milestone(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -4952,20 +5940,20 @@
 from deel_sdk.models import MilestoneReviewToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = MilestoneReviewToCreateContainer(**{
-    "data": {
+request_body = MilestoneReviewToCreateContainer(
+    data={
         "status": "approved",
         "reason": "reason"
     }
-})
+)
 
 result = sdk.milestones.create_milestone_review(
     request_body=request_body,
     contract_id="contract_id",
     milestone_id="milestone_id"
 )
 
@@ -4996,23 +5984,23 @@
 from deel_sdk.models import MilestoneReviewsToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = MilestoneReviewsToCreateContainer(**{
-    "data": {
+request_body = MilestoneReviewsToCreateContainer(
+    data={
         "status": "approved",
         "reason": "reason",
         "ids": [
-            6.78
+            "00000000-0000-0000-0000-000000000000"
         ]
     }
-})
+)
 
 result = sdk.milestones.create_milestone_reviews(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -5083,21 +6071,21 @@
 from deel_sdk.models import OffCyclePaymentToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = OffCyclePaymentToCreateContainer(**{
-    "data": {
+request_body = OffCyclePaymentToCreateContainer(
+    data={
         "date_submitted": "1999-12-31",
         "amount": 2500,
         "description": "description"
     }
-})
+)
 
 result = sdk.off_cycle_payments.create_off_cycle_payment(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -5207,26 +6195,26 @@
 from deel_sdk.models import CreateTimeoffContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CreateTimeoffContainer(**{
-    "data": {
+request_body = CreateTimeoffContainer(
+    data={
         "type_": "VACATION",
         "start_date": "2022-09-03T00:00:00.000Z",
         "end_date": "2022-09-05T00:00:00.000Z",
         "with_multiple_dates": True,
         "reason": "Holiday",
-        "is_start_date_half_day": True,
+        "is_start_date_half_day": False,
         "is_end_date_half_day": False,
         "other_timeoff_name": "Birthday"
     }
-})
+)
 
 result = sdk.time_off.create_eor_time_offs(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -5257,26 +6245,26 @@
 from deel_sdk.models import CreateTimeoffContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CreateTimeoffContainer(**{
-    "data": {
+request_body = CreateTimeoffContainer(
+    data={
         "type_": "VACATION",
         "start_date": "2022-09-03T00:00:00.000Z",
         "end_date": "2022-09-05T00:00:00.000Z",
         "with_multiple_dates": True,
         "reason": "Holiday",
-        "is_start_date_half_day": True,
+        "is_start_date_half_day": False,
         "is_end_date_half_day": False,
         "other_timeoff_name": "Birthday"
     }
-})
+)
 
 result = sdk.time_off.edit_eor_time_offs(
     request_body=request_body,
     contract_id="contract_id",
     timeoff_id="timeoff_id"
 )
 
@@ -5403,20 +6391,20 @@
 from deel_sdk.models import TimeoffToReviewContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TimeoffToReviewContainer(**{
-    "data": {
+request_body = TimeoffToReviewContainer(
+    data={
         "is_approved": True,
         "denial_reason": "Not allowed for this day."
     }
-})
+)
 
 result = sdk.time_off.review_timeoff(
     request_body=request_body,
     timeoff_id="timeoff_id"
 )
 
 print(result)
@@ -5487,15 +6475,15 @@
     types=types,
     statuses=statuses,
     invoice_id="invoice_id",
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=10,
-    offset=226515477.25
+    offset=893166763.24
 )
 
 print(result)
 ```
 
 #### **get_invoice_adjustments**
 
@@ -5547,15 +6535,15 @@
     types=types,
     statuses=statuses,
     invoice_id="invoice_id",
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=10,
-    offset=240522187.51
+    offset=114760289.77
 )
 
 print(result)
 ```
 
 #### **create_invoice_adjustment**
 
@@ -5581,24 +6569,24 @@
 from deel_sdk.models import InvoiceAdjustmentToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = InvoiceAdjustmentToCreateContainer(**{
-    "data": {
+request_body = InvoiceAdjustmentToCreateContainer(
+    data={
         "contract_id": "contract_id",
         "date_submitted": "1999-12-31",
         "type_": "bonus",
         "amount": 2500,
         "description": "Bonus for being awesome.",
-        "payment_cycle_id": 6.69
+        "payment_cycle_id": 7.22
     }
-})
+)
 
 result = sdk.invoices.create_invoice_adjustment(
     request_body=request_body,
     recurring=False
 )
 
 print(result)
@@ -5628,20 +6616,20 @@
 from deel_sdk.models import InvoiceAdjustmentToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = InvoiceAdjustmentToUpdateContainer(**{
-    "data": {
-        "description": "sunt laborum Duis exercitation id",
-        "amount": 9.39
+request_body = InvoiceAdjustmentToUpdateContainer(
+    data={
+        "description": "nostrud ad ullamco dolor",
+        "amount": 9.38
     }
-})
+)
 
 result = sdk.invoices.update_invoice_adjustment_by_id(
     request_body=request_body,
     invoice_adjustment_id="invoice_adjustment_id"
 )
 
 print(result)
@@ -5706,20 +6694,20 @@
 from deel_sdk.models import InvoiceAdjustmentReviewToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = InvoiceAdjustmentReviewToCreateContainer(**{
-    "data": {
+request_body = InvoiceAdjustmentReviewToCreateContainer(
+    data={
         "status": "approved",
         "reason": "reason"
     }
-})
+)
 
 result = sdk.invoices.create_invoice_adjustment_review(
     request_body=request_body,
     invoice_adjustment_id="invoice_adjustment_id"
 )
 
 print(result)
@@ -5748,23 +6736,23 @@
 from deel_sdk.models import InvoiceAdjustmentReviewsToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = InvoiceAdjustmentReviewsToCreateContainer(**{
-    "data": {
+request_body = InvoiceAdjustmentReviewsToCreateContainer(
+    data={
         "status": "approved",
         "reason": "reason",
         "ids": [
-            1.77
+            8.09
         ]
     }
-})
+)
 
 result = sdk.invoices.create_invoice_adjustment_reviews(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_invoice_adjustments_attachment**
@@ -6233,25 +7221,25 @@
 from deel_sdk.models import CreateWebhookRequest
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CreateWebhookRequest(**{
-    "name": "My first webhook.",
-    "description": "I like it very much.",
-    "status": "enabled",
-    "url": "https://mywebhook.com",
-    "signing_key": "signing_key",
-    "api_version": "v2",
-    "events": [
+request_body = CreateWebhookRequest(
+    name="My first webhook.",
+    description="I like it very much.",
+    status="enabled",
+    url="https://mywebhook.com",
+    signing_key="signing_key",
+    api_version="v2",
+    events=[
         "events"
     ]
-})
+)
 
 result = sdk.webhooks.create_webhook(request_body=request_body)
 
 print(result)
 ```
 
 #### **webhook_controller_get_by_id**
@@ -6309,25 +7297,25 @@
 from deel_sdk.models import PatchWebhookRequest
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = PatchWebhookRequest(**{
-    "name": "Demo webhook",
-    "description": "My first webhook",
-    "status": "enabled",
-    "url": "https://mywebhook.com/listening",
-    "signing_key": "signing_key",
-    "api_version": "v2",
-    "events": [
+request_body = PatchWebhookRequest(
+    name="Demo webhook",
+    description="My first webhook",
+    status="enabled",
+    url="https://mywebhook.com/listening",
+    signing_key="signing_key",
+    api_version="v2",
+    events=[
         "events"
     ]
-})
+)
 
 result = sdk.webhooks.webhook_controller_edit_by_id(
     request_body=request_body,
     id_="id"
 )
 
 print(result)
@@ -6421,21 +7409,21 @@
 from deel_sdk.models import CreatePublicTokenContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CreatePublicTokenContainer(**{
-    "data": {
+request_body = CreatePublicTokenContainer(
+    data={
         "scope": [
             "contracts:read"
         ]
     }
-})
+)
 
 result = sdk.token.create_public_token(request_body=request_body)
 
 print(result)
 ```
 
 ### CartaService
```

### Comparing `deel_sdk-1.0.2/README.md` & `deel_sdk-1.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# DeelSdk Python SDK 1.0.2
+# DeelSdk Python SDK 1.0.4
 
 A Python SDK for DeelSdk.
 
 - API version: 1.25.0
-- SDK version: 1.0.2
+- SDK version: 1.0.4
 
 Deel REST API
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Authentication](#authentication)
@@ -92,37 +92,41 @@
 
 You cannot create an instance of a Union type itself. Instead, pass an instance of one of the types in the Union, or a dictionary that can be converted to one of those types.
 
 ## Services
 
 A list of all SDK services. Click on the service name to access its corresponding service methods.
 
-| Service                                             |
-| :-------------------------------------------------- |
-| [AccountingService](#accountingservice)             |
-| [ManagersService](#managersservice)                 |
-| [PeopleService](#peopleservice)                     |
-| [EorService](#eorservice)                           |
-| [GlobalPayrollService](#globalpayrollservice)       |
-| [ContractorsService](#contractorsservice)           |
-| [AdjustmentsService](#adjustmentsservice)           |
-| [CandidatesService](#candidatesservice)             |
-| [PartnerManagedService](#partnermanagedservice)     |
-| [ContractsService](#contractsservice)               |
-| [TasksService](#tasksservice)                       |
-| [TimesheetsService](#timesheetsservice)             |
-| [MilestonesService](#milestonesservice)             |
-| [OffCyclePaymentsService](#offcyclepaymentsservice) |
-| [TimeOffService](#timeoffservice)                   |
-| [InvoicesService](#invoicesservice)                 |
-| [OrganizationsService](#organizationsservice)       |
-| [LookupsService](#lookupsservice)                   |
-| [WebhooksService](#webhooksservice)                 |
-| [TokenService](#tokenservice)                       |
-| [CartaService](#cartaservice)                       |
+| Service                                                       |
+| :------------------------------------------------------------ |
+| [AccountingService](#accountingservice)                       |
+| [CustomFieldsService](#customfieldsservice)                   |
+| [HrisOrganizationsService](#hrisorganizationsservice)         |
+| [ContractsService](#contractsservice)                         |
+| [OrganizationStructureService](#organizationstructureservice) |
+| [PositionsService](#positionsservice)                         |
+| [ManagersService](#managersservice)                           |
+| [PeopleService](#peopleservice)                               |
+| [EorService](#eorservice)                                     |
+| [GlobalPayrollService](#globalpayrollservice)                 |
+| [ContractorsService](#contractorsservice)                     |
+| [AdjustmentsService](#adjustmentsservice)                     |
+| [CandidatesService](#candidatesservice)                       |
+| [PartnerManagedService](#partnermanagedservice)               |
+| [TasksService](#tasksservice)                                 |
+| [TimesheetsService](#timesheetsservice)                       |
+| [MilestonesService](#milestonesservice)                       |
+| [OffCyclePaymentsService](#offcyclepaymentsservice)           |
+| [TimeOffService](#timeoffservice)                             |
+| [InvoicesService](#invoicesservice)                           |
+| [OrganizationsService](#organizationsservice)                 |
+| [LookupsService](#lookupsservice)                             |
+| [WebhooksService](#webhooksservice)                           |
+| [TokenService](#tokenservice)                                 |
+| [CartaService](#cartaservice)                                 |
 
 ### AccountingService
 
 A list of all methods in the `AccountingService` service. Click on the method name to view detailed information about that method.
 
 | Methods                                                                 | Description                                                                                                            |
 | :---------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------- |
@@ -152,23 +156,25 @@
 
 `InvoiceListContainer`
 
 **Example Usage Code Snippet**
 
 ```py
 from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import GetInvoiceListEntities
+from deel_sdk.models.get_invoice_list_entities import List[LegalEntityType]
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
-entities=GetInvoiceListEntities(**[
+entities=List[LegalEntityType](
+    [
     "individual"
-])
+]
+)
 
 result = sdk.accounting.get_invoice_list(
     issued_from_date="issued_from_date",
     issued_to_date="issued_to_date",
     entities=entities,
     limit=10,
     offset=808037660.53
@@ -264,26 +270,31 @@
 
 `PaymentListContainer`
 
 **Example Usage Code Snippet**
 
 ```py
 from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import GetPaymentListCurrencies, GetPaymentListEntities
+from deel_sdk.models.get_payment_list_currencies import List[str]
+from deel_sdk.models.get_payment_list_entities import List[LegalEntityType]
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
-currencies=GetPaymentListCurrencies(**[
+currencies=List[str](
+    [
     "GBP"
-])
-entities=GetPaymentListEntities(**[
+]
+)
+entities=List[LegalEntityType](
+    [
     "individual"
-])
+]
+)
 
 result = sdk.accounting.get_payment_list(
     date_from="1999-12-31",
     date_to="1999-12-31",
     currencies=currencies,
     entities=entities
 )
@@ -318,14 +329,1569 @@
 )
 
 result = sdk.accounting.get_payments_break_down_by_id(payment_id="payment_id")
 
 print(result)
 ```
 
+### CustomFieldsService
+
+A list of all methods in the `CustomFieldsService` service. Click on the method name to view detailed information about that method.
+
+| Methods                                                                               | Description                                                                                                                                        |
+| :------------------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------- |
+| [get_custom_fields_from_people](#get_custom_fields_from_people)                       | Fetch all custom fields associated with People records, offering additional personalized information.                                              |
+| [get_custom_field_from_people_by_id](#get_custom_field_from_people_by_id)             | Access details of a specific custom field by using the custom field ID to enrich individual personnel records.                                     |
+| [get_custom_field_values_from_worker](#get_custom_field_values_from_worker)           | Obtain all custom field values associated with a specific worker, facilitating detailed data retrieval for administrative or operational purposes. |
+| [upsert_custom_field_value_from_worker](#upsert_custom_field_value_from_worker)       | Add or update custom field values for a specific worker, ensuring their profile is up-to-date with the latest information.                         |
+| [delete_custom_field_value_from_worker](#delete_custom_field_value_from_worker)       | Delete a specific custom field value from a worker's profile, removing outdated or unnecessary information.                                        |
+| [get_custom_fields_from_contracts](#get_custom_fields_from_contracts)                 | Fetch all custom fields associated with contracts, providing additional data necessary for contract management.                                    |
+| [get_custom_field_from_contracts_by_id](#get_custom_field_from_contracts_by_id)       | Access details of a specific custom field associated with a contract to manage contract-specific attributes effectively.                           |
+| [get_custom_field_values_from_contract](#get_custom_field_values_from_contract)       | Obtain all custom field values for a specific contract, enhancing contract management with detailed, custom-configured data.                       |
+| [upsert_custom_field_value_from_contracts](#upsert_custom_field_value_from_contracts) | Add or update custom field values for a specific contract, ensuring all contract details are current and relevant.                                 |
+| [delete_contract_custom_field](#delete_contract_custom_field)                         | Delete a specific custom field’s value from a contract, streamlining contract data management by removing redundant or outdated information.       |
+
+#### **get_custom_fields_from_people**
+
+Fetch all custom fields associated with People records, offering additional personalized information.
+
+- HTTP Method: `GET`
+- Endpoint: `/people/custom_fields`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+
+**Return Type**
+
+`CustomFieldsListContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.get_custom_fields_from_people()
+
+print(result)
+```
+
+#### **get_custom_field_from_people_by_id**
+
+Access details of a specific custom field by using the custom field ID to enrich individual personnel records.
+
+- HTTP Method: `GET`
+- Endpoint: `/people/custom_fields/{field_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| field_id | str | ✅ | Access details of a specific custom field by using the custom field ID to enrich individual personnel records. |
+
+**Return Type**
+
+`CustomFieldItemContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.get_custom_field_from_people_by_id(field_id="field_id")
+
+print(result)
+```
+
+#### **get_custom_field_values_from_worker**
+
+Obtain all custom field values associated with a specific worker, facilitating detailed data retrieval for administrative or operational purposes.
+
+- HTTP Method: `GET`
+- Endpoint: `/people/{worker_id}/custom_fields`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| worker_id | str | ✅ | Obtain all custom field values associated with a specific worker, facilitating detailed data retrieval for administrative or operational purposes. |
+
+**Return Type**
+
+`CustomFieldValuesContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.get_custom_field_values_from_worker(worker_id="worker_id")
+
+print(result)
+```
+
+#### **upsert_custom_field_value_from_worker**
+
+Add or update custom field values for a specific worker, ensuring their profile is up-to-date with the latest information.
+
+- HTTP Method: `PUT`
+- Endpoint: `/people/{worker_id}/custom_fields`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | CustomFieldToUpdateContainer | ✅ | The request body. |
+| worker_id | str | ✅ | Add or update custom field values for a specific worker, ensuring their profile is up-to-date with the latest information. |
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import CustomFieldToUpdateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = CustomFieldToUpdateContainer(
+    id_="id",
+    data={
+        "value": "value"
+    }
+)
+
+result = sdk.custom_fields.upsert_custom_field_value_from_worker(
+    request_body=request_body,
+    worker_id="worker_id"
+)
+
+print(result)
+```
+
+#### **delete_custom_field_value_from_worker**
+
+Delete a specific custom field value from a worker's profile, removing outdated or unnecessary information.
+
+- HTTP Method: `DELETE`
+- Endpoint: `/people/{worker_id}/custom_fields/{field_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| worker_id | str | ✅ | Delete a specific custom field value from a worker's profile, removing outdated or unnecessary information. |
+| field_id | str | ✅ | Delete a specific custom field value from a worker's profile, removing outdated or unnecessary information. |
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.delete_custom_field_value_from_worker(
+    worker_id="worker_id",
+    field_id="field_id"
+)
+
+print(result)
+```
+
+#### **get_custom_fields_from_contracts**
+
+Fetch all custom fields associated with contracts, providing additional data necessary for contract management.
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts/custom_fields`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+
+**Return Type**
+
+`CustomFieldsListContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.get_custom_fields_from_contracts()
+
+print(result)
+```
+
+#### **get_custom_field_from_contracts_by_id**
+
+Access details of a specific custom field associated with a contract to manage contract-specific attributes effectively.
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts/custom_fields/{field_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| field_id | str | ✅ | Access details of a specific custom field associated with a contract to manage contract-specific attributes effectively. |
+
+**Return Type**
+
+`CustomFieldItemContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.get_custom_field_from_contracts_by_id(field_id="field_id")
+
+print(result)
+```
+
+#### **get_custom_field_values_from_contract**
+
+Obtain all custom field values for a specific contract, enhancing contract management with detailed, custom-configured data.
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts/{contract_id}/custom_fields`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Obtain all custom field values for a specific contract, enhancing contract management with detailed, custom-configured data. |
+
+**Return Type**
+
+`CustomFieldValuesContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.get_custom_field_values_from_contract(contract_id="contract_id")
+
+print(result)
+```
+
+#### **upsert_custom_field_value_from_contracts**
+
+Add or update custom field values for a specific contract, ensuring all contract details are current and relevant.
+
+- HTTP Method: `PUT`
+- Endpoint: `/contracts/{contract_id}/custom_fields`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | CustomFieldToUpdateContainer | ✅ | The request body. |
+| contract_id | str | ✅ | Add or update custom field values for a specific contract, ensuring all contract details are current and relevant. |
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import CustomFieldToUpdateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = CustomFieldToUpdateContainer(
+    id_="id",
+    data={
+        "value": "value"
+    }
+)
+
+result = sdk.custom_fields.upsert_custom_field_value_from_contracts(
+    request_body=request_body,
+    contract_id="contract_id"
+)
+
+print(result)
+```
+
+#### **delete_contract_custom_field**
+
+Delete a specific custom field’s value from a contract, streamlining contract data management by removing redundant or outdated information.
+
+- HTTP Method: `DELETE`
+- Endpoint: `/contracts/{contract_id}/custom_fields/{field_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Delete a specific custom field’s value from a contract, streamlining contract data management by removing redundant or outdated information. |
+| field_id | str | ✅ | Delete a specific custom field’s value from a contract, streamlining contract data management by removing redundant or outdated information. |
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.delete_contract_custom_field(
+    contract_id="contract_id",
+    field_id="field_id"
+)
+
+print(result)
+```
+
+### HrisOrganizationsService
+
+A list of all methods in the `HrisOrganizationsService` service. Click on the method name to view detailed information about that method.
+
+| Methods                                               | Description                                |
+| :---------------------------------------------------- | :----------------------------------------- |
+| [get_organization_roles](#get_organization_roles)     | Get the roles of the current organization. |
+| [create_organization_role](#create_organization_role) | Create organization custom role.           |
+| [update_organization_role](#update_organization_role) | Update organization custom role.           |
+
+#### **get_organization_roles**
+
+Get the roles of the current organization.
+
+- HTTP Method: `GET`
+- Endpoint: `/roles`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+
+**Return Type**
+
+`GetRolesContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.hris_organizations.get_organization_roles()
+
+print(result)
+```
+
+#### **create_organization_role**
+
+Create organization custom role.
+
+- HTTP Method: `POST`
+- Endpoint: `/roles`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | RoleToCreateContainer | ✅ | The request body. |
+
+**Return Type**
+
+`CreatedRoleContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import RoleToCreateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = RoleToCreateContainer(
+    data={
+        "name": "name",
+        "scope": "ORGANIZATION",
+        "description": "description",
+        "permission_sets": [
+            "permissionSets"
+        ],
+        "hris_org_structure_id": "hrisOrgStructureId"
+    }
+)
+
+result = sdk.hris_organizations.create_organization_role(request_body=request_body)
+
+print(result)
+```
+
+#### **update_organization_role**
+
+Update organization custom role.
+
+- HTTP Method: `PATCH`
+- Endpoint: `/roles/{role_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | RoleToUpdateContainer | ✅ | The request body. |
+| role_id | str | ✅ | Update organization custom role. |
+
+**Return Type**
+
+`UpdatedRoleContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import RoleToUpdateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = RoleToUpdateContainer(
+    data={
+        "name": "name",
+        "description": "description",
+        "permission_sets": [
+            "permissionSets"
+        ]
+    }
+)
+
+result = sdk.hris_organizations.update_organization_role(
+    request_body=request_body,
+    role_id="role_id"
+)
+
+print(result)
+```
+
+### ContractsService
+
+A list of all methods in the `ContractsService` service. Click on the method name to view detailed information about that method.
+
+| Methods                                                                     | Description                                                                                                                                                                                                          |
+| :-------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| [request_exercise_equity](#request_exercise_equity)                         | Create a request to exercise equity.                                                                                                                                                                                 |
+| [approve_exercise_equity](#approve_exercise_equity)                         | Approve an equity exercise.                                                                                                                                                                                          |
+| [get_contract_list](#get_contract_list)                                     | Retrieve a list of contracts.                                                                                                                                                                                        |
+| [get_contract_by_id](#get_contract_by_id)                                   | Retrieve a single contract.                                                                                                                                                                                          |
+| [attach_external_id](#attach_external_id)                                   | Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later. |
+| [add_contract_document](#add_contract_document)                             | Attach a file to contract document.                                                                                                                                                                                  |
+| [edit_contract_document](#edit_contract_document)                           | Overwrite the file currently attached to contract document.                                                                                                                                                          |
+| [get_alternate_emails_by_contract_id](#get_alternate_emails_by_contract_id) | Returns an array of alternate email objects                                                                                                                                                                          |
+| [sign_contract](#sign_contract)                                             | Sign a contract as a client.                                                                                                                                                                                         |
+| [invite_to_sign_contract](#invite_to_sign_contract)                         | Invite a worker to sign the contract. Worker will be notified via email.                                                                                                                                             |
+| [uninvite_to_sign_contract](#uninvite_to_sign_contract)                     | Remove invite in order to re-invite a worker to sign the contract.                                                                                                                                                   |
+| [calculate_final_payment](#calculate_final_payment)                         | Calculate the final payment due to the contractor when ending the contract.                                                                                                                                          |
+| [post_contract_estimate](#post_contract_estimate)                           | First payment is calculated from the number of working/calendar days between their start date and the start of the payment cycle.                                                                                    |
+| [get_contract_templates](#get_contract_templates)                           | Retrieve a list of contract templates in your organization.                                                                                                                                                          |
+| [get_worker_documents_by_id](#get_worker_documents_by_id)                   | Retrieve a list of documents of a worker.                                                                                                                                                                            |
+| [get_download_worker_documents_by_id](#get_download_worker_documents_by_id) | Get the download link of worker document.                                                                                                                                                                            |
+
+#### **request_exercise_equity**
+
+Create a request to exercise equity.
+
+- HTTP Method: `POST`
+- Endpoint: `/equity/exercise`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | ExerciseEquityToCreateContainer | ✅ | The request body. |
+
+**Return Type**
+
+`CreatedExerciseEquityContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import ExerciseEquityToCreateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = ExerciseEquityToCreateContainer(
+    fmv="fmv",
+    quantity=8.76,
+    issuer_id="issuer_id",
+    worker_id="worker_id",
+    address_zip="address_zip",
+    exercise_id="exercise_id",
+    address_city="address_city",
+    address_state="address_state",
+    address_street="address_street",
+    stakeholder_id="stakeholder_id",
+    address_country="address_country",
+    option_grant_id="option_grant_id",
+    fmv_currency_code="fmv_currency_code",
+    stakeholder_email="stakeholder_email",
+    option_grant_issue="option_grant_issue",
+    option_grant_label="option_grant_label",
+    option_grant_currency="option_grant_currency",
+    option_grant_issue_date="option_grant_issue_date",
+    option_grant_expiry_date="option_grant_expiry_date",
+    stakeholder_relationship="stakeholder_relationship",
+    option_grant_strike_price="option_grant_strike_price"
+)
+
+result = sdk.contracts.request_exercise_equity(request_body=request_body)
+
+print(result)
+```
+
+#### **approve_exercise_equity**
+
+Approve an equity exercise.
+
+- HTTP Method: `PATCH`
+- Endpoint: `/equity/exercise/{exercise_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | ExerciseEquityToUpdateContainer | ✅ | The request body. |
+| exercise_id | str | ✅ | Approve an equity exercise. |
+
+**Return Type**
+
+`UpdatedExerciseEquityContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import ExerciseEquityToUpdateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = ExerciseEquityToUpdateContainer(
+    employer_approval="employer_approval"
+)
+
+result = sdk.contracts.approve_exercise_equity(
+    request_body=request_body,
+    exercise_id="exercise_id"
+)
+
+print(result)
+```
+
+#### **get_contract_list**
+
+Retrieve a list of contracts.
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| after_cursor | str | ❌ | Retrieve a list of contracts. |
+| limit | float | ❌ | Retrieve a list of contracts. |
+| order_direction | SortDirEnum | ❌ | Retrieve a list of contracts. |
+| types | List[ContractTypeEnum] | ❌ | Retrieve a list of contracts. |
+| statuses | List[ContractStatusEnum] | ❌ | Retrieve a list of contracts. |
+| team_id | str | ❌ | Retrieve a list of contracts. |
+| external_id | str | ❌ | Retrieve a list of contracts. |
+| countries | List[str] | ❌ | Retrieve a list of contracts. |
+| currencies | GetContractListCurrencies | ❌ | Retrieve a list of contracts. |
+| search | str | ❌ | Retrieve a list of contracts. |
+| sort_by | ContractsSortByEnum | ❌ | Retrieve a list of contracts. |
+
+**Return Type**
+
+`ContractListContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import SortDirEnum, ContractsSortByEnum
+from deel_sdk.models.get_contract_list_currencies import List[str]
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+types=[
+    "ongoing_time_based"
+]
+statuses=[
+    "new"
+]
+countries=[
+    "US"
+]
+currencies=List[str](
+    [
+    "GBP"
+]
+)
+
+result = sdk.contracts.get_contract_list(
+    after_cursor="after_cursor",
+    limit=10,
+    order_direction="asc",
+    types=types,
+    statuses=statuses,
+    team_id="team_id",
+    external_id="external_id",
+    countries=countries,
+    currencies=currencies,
+    search="search",
+    sort_by="contract_title"
+)
+
+print(result)
+```
+
+#### **get_contract_by_id**
+
+Retrieve a single contract.
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts/{contract_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Retrieve a single contract. |
+
+**Return Type**
+
+`ContractContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.get_contract_by_id(contract_id="contract_id")
+
+print(result)
+```
+
+#### **attach_external_id**
+
+Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later.
+
+- HTTP Method: `PATCH`
+- Endpoint: `/contracts/{contract_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | InputToPatchContractExternalId | ✅ | The request body. |
+| contract_id | str | ✅ | Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later. |
+
+**Return Type**
+
+`GenericResultCreated`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import InputToPatchContractExternalId
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = InputToPatchContractExternalId(
+    data={
+        "external_id": "external_id"
+    }
+)
+
+result = sdk.contracts.attach_external_id(
+    request_body=request_body,
+    contract_id="contract_id"
+)
+
+print(result)
+```
+
+#### **add_contract_document**
+
+Attach a file to contract document.
+
+- HTTP Method: `POST`
+- Endpoint: `/contracts/{contract_id}/documents`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | dict | ❌ | The request body. |
+| contract_id | str | ✅ | Attach a file to contract document. |
+
+**Return Type**
+
+`ContractDocumentContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import FileObject
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = {
+    "file": "file"
+}
+
+result = sdk.contracts.add_contract_document(
+    request_body=request_body,
+    contract_id="contract_id"
+)
+
+print(result)
+```
+
+#### **edit_contract_document**
+
+Overwrite the file currently attached to contract document.
+
+- HTTP Method: `PUT`
+- Endpoint: `/contracts/{contract_id}/documents`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | dict | ❌ | The request body. |
+| contract_id | str | ✅ | Overwrite the file currently attached to contract document. |
+
+**Return Type**
+
+`ContractDocumentContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import FileObject
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = {
+    "file": "file"
+}
+
+result = sdk.contracts.edit_contract_document(
+    request_body=request_body,
+    contract_id="contract_id"
+)
+
+print(result)
+```
+
+#### **get_alternate_emails_by_contract_id**
+
+Returns an array of alternate email objects
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts/{contract_id}/alternate_emails`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Returns an array of alternate email objects |
+
+**Return Type**
+
+`List[AlternateEmailItem]`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.get_alternate_emails_by_contract_id(contract_id="contract_id")
+
+print(result)
+```
+
+#### **sign_contract**
+
+Sign a contract as a client.
+
+- HTTP Method: `POST`
+- Endpoint: `/contracts/{contract_id}/signatures`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | ContractSignatureToCreateContainer | ✅ | The request body. |
+| contract_id | str | ✅ | Sign a contract as a client. |
+
+**Return Type**
+
+`GenericResultCreated`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import ContractSignatureToCreateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = ContractSignatureToCreateContainer(
+    data={
+        "client_signature": "dolor enim in",
+        "contract_template_id": 2.41
+    }
+)
+
+result = sdk.contracts.sign_contract(
+    request_body=request_body,
+    contract_id="contract_id"
+)
+
+print(result)
+```
+
+#### **invite_to_sign_contract**
+
+Invite a worker to sign the contract. Worker will be notified via email.
+
+- HTTP Method: `POST`
+- Endpoint: `/contracts/{contract_id}/invitations`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | ContractInvitationToCreateContainer | ✅ | The request body. |
+| contract_id | str | ✅ | Invite a worker to sign the contract. Worker will be notified via email. |
+
+**Return Type**
+
+`GenericResultCreated`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import ContractInvitationToCreateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = ContractInvitationToCreateContainer(
+    data={
+        "email": "eiusmod",
+        "message": "nulla off"
+    }
+)
+
+result = sdk.contracts.invite_to_sign_contract(
+    request_body=request_body,
+    contract_id="contract_id"
+)
+
+print(result)
+```
+
+#### **uninvite_to_sign_contract**
+
+Remove invite in order to re-invite a worker to sign the contract.
+
+- HTTP Method: `DELETE`
+- Endpoint: `/contracts/{contract_id}/invitations`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Remove invite in order to re-invite a worker to sign the contract. |
+
+**Return Type**
+
+`GenericResultDeleted`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.uninvite_to_sign_contract(contract_id="contract_id")
+
+print(result)
+```
+
+#### **calculate_final_payment**
+
+Calculate the final payment due to the contractor when ending the contract.
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts/{contract_id}/final-payments`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Calculate the final payment due to the contractor when ending the contract. |
+| end_date | str | ❌ | Calculate the final payment due to the contractor when ending the contract. |
+| calculation_type | CalculateFinalPaymentCalculationType | ❌ | Calculate the final payment due to the contractor when ending the contract. |
+| workweek_start | str | ❌ | Calculate the final payment due to the contractor when ending the contract. |
+| workweek_end | str | ❌ | Calculate the final payment due to the contractor when ending the contract. |
+
+**Return Type**
+
+`FinalPaymentCalculatedContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import CalculateFinalPaymentCalculationType
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.calculate_final_payment(
+    contract_id="contract_id",
+    end_date="1999-12-31",
+    calculation_type="CUSTOM_AMOUNT",
+    workweek_start="workweek_start",
+    workweek_end="workweek_end"
+)
+
+print(result)
+```
+
+#### **post_contract_estimate**
+
+First payment is calculated from the number of working/calendar days between their start date and the start of the payment cycle.
+
+- HTTP Method: `POST`
+- Endpoint: `/contracts/estimate`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | EstimateFirstPaymentContainer | ✅ | The request body. |
+
+**Return Type**
+
+`ResponseEstimateFirstPaymentContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import EstimateFirstPaymentContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = EstimateFirstPaymentContainer(
+    data={
+        "type_": "ongoing_time_based",
+        "country_code": "US",
+        "start_date": "1999-12-31",
+        "compensation_details": {
+            "amount": 2500,
+            "currency_code": "GBP",
+            "scale": "weekly",
+            "cycle_end": 20.71,
+            "cycle_end_type": "DAY_OF_WEEK",
+            "payment_due_type": "REGULAR",
+            "payment_due_days": 16.18,
+            "calculation_type": "CUSTOM_AMOUNT",
+            "work_week_start": "Sunday",
+            "work_week_end": "Sunday"
+        }
+    }
+)
+
+result = sdk.contracts.post_contract_estimate(request_body=request_body)
+
+print(result)
+```
+
+#### **get_contract_templates**
+
+Retrieve a list of contract templates in your organization.
+
+- HTTP Method: `GET`
+- Endpoint: `/contract-templates`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+
+**Return Type**
+
+`ContractTemplateListContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.get_contract_templates()
+
+print(result)
+```
+
+#### **get_worker_documents_by_id**
+
+Retrieve a list of documents of a worker.
+
+- HTTP Method: `GET`
+- Endpoint: `/workers/{worker_id}/documents`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| worker_id | str | ✅ | Retrieve a list of documents of a worker. |
+
+**Return Type**
+
+`WorkerDocumentsByIdContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.get_worker_documents_by_id(worker_id="worker_id")
+
+print(result)
+```
+
+#### **get_download_worker_documents_by_id**
+
+Get the download link of worker document.
+
+- HTTP Method: `GET`
+- Endpoint: `/workers/{worker_id}/documents/{document_id}/download`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| worker_id | str | ✅ | Get the download link of worker document. |
+| document_id | float | ✅ | Get the download link of worker document. |
+
+**Return Type**
+
+`DownloadWorkerDocumentsByIdContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.get_download_worker_documents_by_id(
+    worker_id="worker_id",
+    document_id=6.05
+)
+
+print(result)
+```
+
+### OrganizationStructureService
+
+A list of all methods in the `OrganizationStructureService` service. Click on the method name to view detailed information about that method.
+
+| Methods                                                         | Description                                     |
+| :-------------------------------------------------------------- | :---------------------------------------------- |
+| [get_all_org_structures](#get_all_org_structures)               | Fetch all Org Structures from the Organization. |
+| [create_org_structure](#create_org_structure)                   | Create a new HRIS Organization Structure.       |
+| [get_org_structure](#get_org_structure)                         | Fetch an Org Structure from the Organization.   |
+| [update_org_structure](#update_org_structure)                   | Update an existing Organization structure.      |
+| [delete_org_structure](#delete_org_structure)                   | Delete an Org Structure from the Organization.  |
+| [get_external_org_structure](#get_external_org_structure)       | Fetch an Org Structure from the Organization.   |
+| [update_external_org_structure](#update_external_org_structure) | Update an existing Organization structure.      |
+| [delete_external_org_structure](#delete_external_org_structure) | Delete an Org Structure from the Organization.  |
+
+#### **get_all_org_structures**
+
+Fetch all Org Structures from the Organization.
+
+- HTTP Method: `GET`
+- Endpoint: `/hris/organization_structures`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+
+**Return Type**
+
+`GetAllOrgStructuresContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.organization_structure.get_all_org_structures()
+
+print(result)
+```
+
+#### **create_org_structure**
+
+Create a new HRIS Organization Structure.
+
+- HTTP Method: `POST`
+- Endpoint: `/hris/organization_structures`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | OrgStructureToCreateContainer | ✅ | The request body. |
+
+**Return Type**
+
+`GetAllOrgStructuresContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import OrgStructureToCreateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = OrgStructureToCreateContainer(
+    data={
+        "name": "name",
+        "teams": [
+            {
+                "name": "name",
+                "external_id": "external_id"
+            }
+        ],
+        "external_id": "external_id",
+        "enable_roles": True,
+        "is_multiple_select": True
+    }
+)
+
+result = sdk.organization_structure.create_org_structure(request_body=request_body)
+
+print(result)
+```
+
+#### **get_org_structure**
+
+Fetch an Org Structure from the Organization.
+
+- HTTP Method: `GET`
+- Endpoint: `/hris/organization_structures/{hrisOrgStr_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| hris_org_str_id | str | ✅ | Fetch an Org Structure from the Organization. |
+
+**Return Type**
+
+`GetOrgStructureContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.organization_structure.get_org_structure(hris_org_str_id="hrisOrgStr_id")
+
+print(result)
+```
+
+#### **update_org_structure**
+
+Update an existing Organization structure.
+
+- HTTP Method: `PATCH`
+- Endpoint: `/hris/organization_structures/{hrisOrgStr_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | OrgStructureToUpdateContainer | ✅ | The request body. |
+| hris_org_str_id | str | ✅ | Update an existing Organization structure. |
+
+**Return Type**
+
+`any`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import OrgStructureToUpdateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = OrgStructureToUpdateContainer(
+    data={
+        "name": "name",
+        "teams": [
+            {}
+        ],
+        "external_id": "external_id",
+        "enable_roles": False,
+        "is_multiselect": True
+    }
+)
+
+result = sdk.organization_structure.update_org_structure(
+    request_body=request_body,
+    hris_org_str_id="hrisOrgStr_id"
+)
+
+print(result)
+```
+
+#### **delete_org_structure**
+
+Delete an Org Structure from the Organization.
+
+- HTTP Method: `DELETE`
+- Endpoint: `/hris/organization_structures/{hrisOrgStr_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| hris_org_str_id | str | ✅ | Delete an Org Structure from the Organization. |
+
+**Return Type**
+
+`any`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.organization_structure.delete_org_structure(hris_org_str_id="hrisOrgStr_id")
+
+print(result)
+```
+
+#### **get_external_org_structure**
+
+Fetch an Org Structure from the Organization.
+
+- HTTP Method: `GET`
+- Endpoint: `/hris/organization_structures/external/{external_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| external_id | str | ✅ | Fetch an Org Structure from the Organization. |
+
+**Return Type**
+
+`GetOrgStructureContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.organization_structure.get_external_org_structure(external_id="external_id")
+
+print(result)
+```
+
+#### **update_external_org_structure**
+
+Update an existing Organization structure.
+
+- HTTP Method: `PATCH`
+- Endpoint: `/hris/organization_structures/external/{external_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | OrgStructureToUpdateContainer | ✅ | The request body. |
+| external_id | str | ✅ | Update an existing Organization structure. |
+
+**Return Type**
+
+`any`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import OrgStructureToUpdateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = OrgStructureToUpdateContainer(
+    data={
+        "name": "name",
+        "teams": [
+            {}
+        ],
+        "external_id": "external_id",
+        "enable_roles": False,
+        "is_multiselect": True
+    }
+)
+
+result = sdk.organization_structure.update_external_org_structure(
+    request_body=request_body,
+    external_id="external_id"
+)
+
+print(result)
+```
+
+#### **delete_external_org_structure**
+
+Delete an Org Structure from the Organization.
+
+- HTTP Method: `DELETE`
+- Endpoint: `/hris/organization_structures/external/{external_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| external_id | str | ✅ | Delete an Org Structure from the Organization. |
+
+**Return Type**
+
+`any`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.organization_structure.delete_external_org_structure(external_id="external_id")
+
+print(result)
+```
+
+### PositionsService
+
+A list of all methods in the `PositionsService` service. Click on the method name to view detailed information about that method.
+
+| Methods                                             | Description                                         |
+| :-------------------------------------------------- | :-------------------------------------------------- |
+| [get_positions](#get_positions)                     | HRIS Positions from a HrisProfile.                  |
+| [apply_changes_positions](#apply_changes_positions) | Apply add, edit, and delete operations to profiles. |
+
+#### **get_positions**
+
+HRIS Positions from a HrisProfile.
+
+- HTTP Method: `GET`
+- Endpoint: `/hris/positions/profile/{hrisProfile_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| hris_profile_id | str | ✅ | HRIS Positions from a HrisProfile. |
+
+**Return Type**
+
+`GetHrisPositionContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.positions.get_positions(hris_profile_id="hrisProfile_id")
+
+print(result)
+```
+
+#### **apply_changes_positions**
+
+Apply add, edit, and delete operations to profiles.
+
+- HTTP Method: `POST`
+- Endpoint: `/hris/positions/apply_changes`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | HrisPositionToChangeContainer | ✅ | The request body. |
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import HrisPositionToChangeContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = HrisPositionToChangeContainer(
+    data={
+        "add": [
+            {
+                "role_id": "role_id",
+                "team_id": "team_id",
+                "is_supportive": True
+            }
+        ],
+        "edit": [
+            {
+                "id_": "id",
+                "role_id": "role_id",
+                "is_supportive": False
+            }
+        ],
+        "delete": [
+            {
+                "id_": "id"
+            }
+        ],
+        "profile_id": "profile_id"
+    }
+)
+
+result = sdk.positions.apply_changes_positions(request_body=request_body)
+
+print(result)
+```
+
 ### ManagersService
 
 A list of all methods in the `ManagersService` service. Click on the method name to view detailed information about that method.
 
 | Methods                           | Description                        |
 | :-------------------------------- | :--------------------------------- |
 | [get_managers](#get_managers)     | List all organization managers.    |
@@ -389,21 +1955,21 @@
 from deel_sdk.models import AdminUserCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = AdminUserCreateContainer(**{
-    "data": {
-        "first_name": "dolore",
-        "last_name": "proi",
+request_body = AdminUserCreateContainer(
+    data={
+        "first_name": "mo",
+        "last_name": "Exce",
         "email": "email"
     }
-})
+)
 
 result = sdk.managers.create_manager(request_body=request_body)
 
 print(result)
 ```
 
 ### PeopleService
@@ -450,49 +2016,49 @@
 from deel_sdk.models import HrisDirectEmployee
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = HrisDirectEmployee(**{
-    "employee_details": {
+request_body = HrisDirectEmployee(
+    employee_details={
         "first_name": "John",
         "last_name": "Doe",
         "email": "john.doe@domain.com",
         "work_email": "john.doe@domain.com",
         "nationality": "CA",
         "country": "BR",
         "state": "AC"
     },
-    "team_information": {
-        "team_id": 9.77,
-        "legal_entity_id": 2.18
+    team_information={
+        "team_id": 9.17,
+        "legal_entity_id": 1.13
     },
-    "job_information": {
-        "seniority_id": 9.22,
-        "job_title_id": 6.5
+    job_information={
+        "seniority_id": 2.01,
+        "job_title_id": 6.94
     },
-    "compensation": {
-        "gross_annual_salary": 7.15,
+    compensation={
+        "gross_annual_salary": 4.71,
         "currency": "USD"
     },
-    "contract": {
+    contract={
         "contract_oid": "pdcMQe0cXCCXWTkqkdytw",
         "start_date": "1999-12-31",
-        "employee_number": 9.02,
+        "employee_number": 0.96,
         "end_date": "1999-12-31",
         "employment_type": "PART_TIME",
-        "part_time_percentage": 21.67
+        "part_time_percentage": 63.32
     },
-    "vacation_info": {
+    vacation_info={
         "vacation_accrual_start_date": "vacation_accrual_start_date",
-        "vacation_yearly_policy": 171.07
+        "vacation_yearly_policy": 214.98
     }
-})
+)
 
 result = sdk.people.create_direct_employee(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_internal_people_list**
@@ -519,16 +2085,16 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.people.get_internal_people_list(
-    offset=978653984.34,
-    limit=43.45
+    offset=664489591.67,
+    limit=128.61
 )
 
 print(result)
 ```
 
 #### **get_people_list**
 
@@ -559,16 +2125,16 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.people.get_people_list(
-    offset=44334375.53,
-    limit=105.69,
+    offset=772862704.51,
+    limit=142.31,
     search="search",
     sort_by="id",
     sort_order="asc",
     hiring_statuses="active"
 )
 
 print(result)
@@ -629,19 +2195,19 @@
 from deel_sdk.models import UpdateWorkerDepartmentContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = UpdateWorkerDepartmentContainer(**{
-    "data": {
+request_body = UpdateWorkerDepartmentContainer(
+    data={
         "department_id": "00000000-0000-0000-0000-000000000000"
     }
-})
+)
 
 result = sdk.people.update_people_department(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -671,19 +2237,19 @@
 from deel_sdk.models import UpdateWorkerWorkingLocationContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = UpdateWorkerWorkingLocationContainer(**{
-    "data": {
+request_body = UpdateWorkerWorkingLocationContainer(
+    data={
         "working_location_id": "00000000-0000-0000-0000-000000000000"
     }
-})
+)
 
 result = sdk.people.update_people_working_location(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -931,20 +2497,20 @@
 from deel_sdk.models import TimeoffToReviewInternalContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TimeoffToReviewInternalContainer(**{
-    "data": {
+request_body = TimeoffToReviewInternalContainer(
+    data={
         "status": "APPROVED",
         "reason": "Approved because there are no conflicts."
     }
-})
+)
 
 result = sdk.people.review_time_offs_for_employee(
     request_body=request_body,
     timeoff_id="timeoff_id",
     worker_id="worker_id"
 )
 
@@ -1115,27 +2681,27 @@
 from deel_sdk.models import EorEmployeeCostCalculationRequestBodyContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = EorEmployeeCostCalculationRequestBodyContainer(**{
-    "data": {
+request_body = EorEmployeeCostCalculationRequestBodyContainer(
+    data={
         "salary": 50000,
         "country": "Germany",
         "currency": "EUR",
         "benefits": [
             {
                 "provider_id": "00000000-0000-0000-0000-000000000000",
                 "plan_id": "00000000-0000-0000-0000-000000000000"
             }
         ]
     }
-})
+)
 
 result = sdk.eor.calculate_eor_employment_cost(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_eor_contract_benefits**
@@ -1192,16 +2758,16 @@
 from deel_sdk.models import EorContractToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = EorContractToCreateContainer(**{
-    "data": {
+request_body = EorContractToCreateContainer(
+    data={
         "employee": {
             "first_name": "Jane",
             "last_name": "Doe",
             "email": "employee@email.com",
             "nationality": "US",
             "address": {
                 "street": "Deel Street 500",
@@ -1214,49 +2780,49 @@
         "employment": {
             "country": "US",
             "state": "state",
             "type_": "Full-time",
             "work_visa_required": False,
             "start_date": "1999-12-31",
             "end_date": "1999-12-31",
-            "probation_period": 6.17,
+            "probation_period": 1.47,
             "scope_of_work": "scope_of_work",
             "time_off_type": "STANDARD",
-            "holidays": 5.67
+            "holidays": 0.98
         },
         "job_title": "job_title",
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "client": {
             "legal_entity": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "compensation_details": {
-            "salary": 5.95,
+            "salary": 3.09,
             "currency": "currency",
-            "variable_compensation": 3.49,
+            "variable_compensation": 6.88,
             "variable_compensation_type": "PERCENTAGE"
         },
         "quote_additional_fields": {
             "gender": "gender",
             "worker_type": "Skilled",
             "dob": "dob"
         },
         "health_plan_id": "health_plan_id",
         "pension": {
             "id_": "id",
             "contribution": "contribution"
         }
     }
-})
+)
 
 result = sdk.eor.create_eor_contract(request_body=request_body)
 
 print(result)
 ```
 
 ### GlobalPayrollService
@@ -1304,55 +2870,55 @@
 from deel_sdk.models import GpContractToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = GpContractToCreateContainer(**{
-    "data": {
+request_body = GpContractToCreateContainer(
+    data={
         "employee": {
             "first_name": "Jane",
             "last_name": "Doe",
-            "email": "culpa Lorem inc",
-            "work_email": "in do L",
+            "email": "esse no",
+            "work_email": "ipsum cillum c",
             "nationality": "US",
             "employee_number": "100",
             "address": {
                 "street": "Deel Street 500",
                 "city": "Denver",
                 "state": "CO",
                 "zip": "44000",
                 "country": "US"
             }
         },
         "employment": {
             "type_": "Full-time",
             "start_date": "1999-12-31",
             "holidays": {
-                "allowance": 5.28,
+                "allowance": 4.86,
                 "start_date": "1999-12-31"
             }
         },
         "job_title": "job_title",
         "client": {
             "legal_entity": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "compensation_details": {
             "scale": "YEAR",
-            "salary": 8.05,
+            "salary": 5.64,
             "currency": "GBP"
         }
     }
-})
+)
 
 result = sdk.global_payroll.create_gp_contract(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_worker_payslips**
@@ -1410,21 +2976,21 @@
 from deel_sdk.models import GpEmployeeAddressToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = GpEmployeeAddressToUpdateContainer(**{
-    "data": {
+request_body = GpEmployeeAddressToUpdateContainer(
+    data={
         "city": "London",
         "street": "123 Deel Street",
         "zip": "12345"
     }
-})
+)
 
 result = sdk.global_payroll.update_gp_employee_address(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -1485,16 +3051,16 @@
 from deel_sdk.models import AddWorkerBankAccountContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = AddWorkerBankAccountContainer(**{
-    "data": {
+request_body = AddWorkerBankAccountContainer(
+    data={
         "full_name": "John Doe",
         "phone": "+1234567890",
         "address_line1": "1234 Main St",
         "address_line2": "Apartment 101",
         "city": "Springfield",
         "province_state": "Ontario",
         "postal": "12345",
@@ -1511,15 +3077,15 @@
         "bank_branch_name": "Main Street Branch",
         "iban": "GB29NWBK60161331926819",
         "email": "john.doe@example.com",
         "rib_number": "12345678901",
         "account_type": "12345678901",
         "ach_routing_number": "12345678901"
     }
-})
+)
 
 result = sdk.global_payroll.add_gp_bank_account(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -1550,16 +3116,16 @@
 from deel_sdk.models import AddWorkerBankAccountContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = AddWorkerBankAccountContainer(**{
-    "data": {
+request_body = AddWorkerBankAccountContainer(
+    data={
         "full_name": "John Doe",
         "phone": "+1234567890",
         "address_line1": "1234 Main St",
         "address_line2": "Apartment 101",
         "city": "Springfield",
         "province_state": "Ontario",
         "postal": "12345",
@@ -1576,15 +3142,15 @@
         "bank_branch_name": "Main Street Branch",
         "iban": "GB29NWBK60161331926819",
         "email": "john.doe@example.com",
         "rib_number": "12345678901",
         "account_type": "12345678901",
         "ach_routing_number": "12345678901"
     }
-})
+)
 
 result = sdk.global_payroll.patch_gp_bank_account(
     request_body=request_body,
     worker_id="worker_id",
     bank_id="bank_id"
 )
 
@@ -1646,21 +3212,21 @@
 from deel_sdk.models import GpEmployeeCompensationToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = GpEmployeeCompensationToUpdateContainer(**{
-    "data": {
+request_body = GpEmployeeCompensationToUpdateContainer(
+    data={
         "scale": "YEAR",
         "salary": 50000,
         "effective_date": "1999-12-31"
     }
-})
+)
 
 result = sdk.global_payroll.update_gp_employee_compensation(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -1690,20 +3256,20 @@
 from deel_sdk.models import GpEmployeePtoToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = GpEmployeePtoToUpdateContainer(**{
-    "data": {
+request_body = GpEmployeePtoToUpdateContainer(
+    data={
         "accrual_start_date": "1999-12-31",
         "yearly_allowance": "15"
     }
-})
+)
 
 result = sdk.global_payroll.update_gp_employee_pto(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -1733,25 +3299,25 @@
 from deel_sdk.models import GpEmployeeInformationToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = GpEmployeeInformationToUpdateContainer(**{
-    "data": {
+request_body = GpEmployeeInformationToUpdateContainer(
+    data={
         "first_name": "Jane",
         "middle_name": "Jay",
         "last_name": "Doe",
         "date_of_birth": "1999-12-31",
         "gender": "gender",
         "marital_status": "Single",
         "employee_number": "employee_number"
     }
-})
+)
 
 result = sdk.global_payroll.update_gp_employee_information(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -1914,23 +3480,23 @@
 from deel_sdk.models import WorkerTerminationBodyContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = WorkerTerminationBodyContainer(**{
-    "data": {
+request_body = WorkerTerminationBodyContainer(
+    data={
         "desired_end_date": "2023-12-31",
         "last_date_of_work": "2023-12-31",
         "message": "Termination reason",
         "is_voluntary": True,
         "severance": {}
     }
-})
+)
 
 result = sdk.global_payroll.request_termination(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -1976,16 +3542,16 @@
 from deel_sdk.models import ContractToCreateContainerPayAsYouGoTimeBased
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToCreateContainerPayAsYouGoTimeBased(**{
-    "data": {
+request_body = ContractToCreateContainerPayAsYouGoTimeBased(
+    data={
         "title": "title",
         "country_code": "US",
         "state_code": "state_code",
         "scope_of_work": "scope_of_work",
         "special_clause": "special_clause",
         "termination_date": "1999-12-31",
         "client": {
@@ -1993,50 +3559,50 @@
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
-            "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "sedDuis officia est laborum in"
+            "id_": "id",
+            "name": "in labore officia non veniam"
         },
         "seniority": {
-            "id_": "00000000-0000-0000-0000-000000000000"
+            "id_": 5.48
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "occae",
+            "expected_email": "adipisicing",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "pay_as_you_go_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 2.6,
+            "amount": 0.13,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
             "first_payment_date": "1999-12-31",
             "first_payment": 500,
             "notice_period": 15,
             "scale": "hourly"
         }
     }
-})
+)
 
 result = sdk.contractors.create_contract_time_based(request_body=request_body)
 
 print(result)
 ```
 
 #### **create_contract_task_based**
@@ -2062,16 +3628,16 @@
 from deel_sdk.models import ContractToCreateContainerPaygTasks
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToCreateContainerPaygTasks(**{
-    "data": {
+request_body = ContractToCreateContainerPaygTasks(
+    data={
         "title": "title",
         "country_code": "US",
         "state_code": "state_code",
         "scope_of_work": "scope_of_work",
         "special_clause": "special_clause",
         "termination_date": "1999-12-31",
         "client": {
@@ -2079,29 +3645,29 @@
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
-            "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "enim irure dolore magna"
+            "id_": "id",
+            "name": "irure"
         },
         "seniority": {
-            "id_": "00000000-0000-0000-0000-000000000000"
+            "id_": 5.89
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "Duis nulla oc",
+            "expected_email": "in Ex",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "payg_tasks",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 100,
@@ -2113,15 +3679,15 @@
             "payment_due_days": 7,
             "pay_before_weekends": True,
             "first_payment_date": "1999-12-31",
             "first_payment": 500,
             "notice_period": 15
         }
     }
-})
+)
 
 result = sdk.contractors.create_contract_task_based(request_body=request_body)
 
 print(result)
 ```
 
 #### **create_contract_milestone_based**
@@ -2147,16 +3713,16 @@
 from deel_sdk.models import ContractToCreateContainerPaygMilestones
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToCreateContainerPaygMilestones(**{
-    "data": {
+request_body = ContractToCreateContainerPaygMilestones(
+    data={
         "title": "title",
         "country_code": "US",
         "state_code": "state_code",
         "scope_of_work": "scope_of_work",
         "special_clause": "special_clause",
         "termination_date": "1999-12-31",
         "client": {
@@ -2164,29 +3730,29 @@
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
-            "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "et dolore"
+            "id_": "id",
+            "name": "pariatur"
         },
         "seniority": {
-            "id_": "00000000-0000-0000-0000-000000000000"
+            "id_": 8.01
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "sint ",
+            "expected_email": "aute dolor",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "payg_milestones",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 100,
@@ -2198,15 +3764,15 @@
             "payment_due_days": 7,
             "pay_before_weekends": True,
             "first_payment_date": "1999-12-31",
             "first_payment": 500,
             "notice_period": 15
         }
     }
-})
+)
 
 result = sdk.contractors.create_contract_milestone_based(request_body=request_body)
 
 print(result)
 ```
 
 #### **create_contract_fixed_rate**
@@ -2232,16 +3798,16 @@
 from deel_sdk.models import ContractToCreateContainerOngoingTimeBased
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToCreateContainerOngoingTimeBased(**{
-    "data": {
+request_body = ContractToCreateContainerOngoingTimeBased(
+    data={
         "title": "title",
         "country_code": "US",
         "state_code": "state_code",
         "scope_of_work": "scope_of_work",
         "special_clause": "special_clause",
         "termination_date": "1999-12-31",
         "client": {
@@ -2249,50 +3815,50 @@
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
-            "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "cillum"
+            "id_": "id",
+            "name": "proident fugiat est aliquip elit"
         },
         "seniority": {
-            "id_": "00000000-0000-0000-0000-000000000000"
+            "id_": 6.6
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "Lorem sint et",
+            "expected_email": "nisiet lab",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "ongoing_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 7.36,
+            "amount": 9.2,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
             "first_payment_date": "1999-12-31",
             "first_payment": 500,
             "notice_period": 15,
             "scale": "hourly"
         }
     }
-})
+)
 
 result = sdk.contractors.create_contract_fixed_rate(request_body=request_body)
 
 print(result)
 ```
 
 #### **create_contract**
@@ -2318,16 +3884,16 @@
 from deel_sdk.models import ContractToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToCreateContainer(**{
-    "data": {
+request_body = ContractToCreateContainer(
+    data={
         "title": "title",
         "country_code": "US",
         "state_code": "state_code",
         "scope_of_work": "scope_of_work",
         "special_clause": "special_clause",
         "termination_date": "1999-12-31",
         "client": {
@@ -2335,50 +3901,50 @@
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
-            "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "sedDuis officia est laborum in"
+            "id_": "id",
+            "name": "in labore officia non veniam"
         },
         "seniority": {
-            "id_": "00000000-0000-0000-0000-000000000000"
+            "id_": 5.48
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "occae",
+            "expected_email": "adipisicing",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "pay_as_you_go_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 2.6,
+            "amount": 0.13,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
             "first_payment_date": "1999-12-31",
             "first_payment": 500,
             "notice_period": 15,
             "scale": "hourly"
         }
     }
-})
+)
 
 result = sdk.contractors.create_contract(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_contract_preview**
@@ -2441,35 +4007,35 @@
 from deel_sdk.models import ContractToAmendDetailsContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToAmendDetailsContainer(**{
-    "data": {
+request_body = ContractToAmendDetailsContainer(
+    data={
         "amount": 100,
         "currency_code": "GBP",
         "scale": "hourly",
         "effective_date": "1999-12-31",
         "first_payment_date": "1999-12-31",
-        "first_payment": 0.24,
+        "first_payment": 4.5,
         "frequency": "weekly",
-        "cycle_end": 24.94,
+        "cycle_end": 3.38,
         "cycle_end_type": "DAY_OF_WEEK",
         "payment_due_type": "REGULAR",
-        "payment_due_days": 0.92,
-        "pay_before_weekends": True,
+        "payment_due_days": 83.14,
+        "pay_before_weekends": False,
         "job_title_name": "3D Designer",
         "job_title_id": "00000000-0000-0000-0000-000000000000",
         "seniority_id": "00000000-0000-0000-0000-000000000000",
         "special_clause": "special_clause",
         "scope_of_work": "scope_of_work"
     }
-})
+)
 
 result = sdk.contractors.amend_contract_details(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -2499,21 +4065,21 @@
 from deel_sdk.models import ContractToTerminateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToTerminateContainer(**{
-    "data": {
+request_body = ContractToTerminateContainer(
+    data={
         "completion_date": "1999-12-31",
         "terminate_now": True,
         "message": "message"
     }
-})
+)
 
 result = sdk.contractors.terminate_contract(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -2543,20 +4109,20 @@
 from deel_sdk.models import PremiumToAddContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = PremiumToAddContainer(**{
-    "data": {
+request_body = PremiumToAddContainer(
+    data={
         "agreement_reflects_relation": True,
         "contractor_characteristics": True
     }
-})
+)
 
 result = sdk.contractors.add_premium(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -2637,20 +4203,20 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = {
     "data": {
         "contract_id": "m3jk2j",
-        "amount": "cupidatat exe",
+        "amount": "labore",
         "date_of_adjustment": "1999-12-31",
         "title": "Your title here",
         "description": "Your description here",
         "cycle_reference": "my_cycle_reference",
-        "file": "qu",
+        "file": "ut",
         "adjustment_category_id": "c9cf4c2c0165f48f494415390c3b49",
         "move_next_cycle": True,
         "vendor": "Vendor",
         "country": "US"
     }
 }
 
@@ -2714,22 +4280,22 @@
 from deel_sdk.models import AdjustmentToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = AdjustmentToUpdateContainer(**{
-    "data": {
-        "amount": "ut velit in",
+request_body = AdjustmentToUpdateContainer(
+    data={
+        "amount": "ad aute d",
         "title": "Your title here",
         "description": "Your description here",
-        "file": "incididunt "
+        "file": "in ulla"
     }
-})
+)
 
 result = sdk.adjustments.update_adjustment(
     request_body=request_body,
     adjustment_id="adjustment_id"
 )
 
 print(result)
@@ -2819,19 +4385,19 @@
 from deel_sdk.models import InputToCreateFileRef
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = InputToCreateFileRef(**{
-    "data": {
+request_body = InputToCreateFileRef(
+    data={
         "content_type": "application/pdf"
     }
-})
+)
 
 result = sdk.adjustments.create_file_ref(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_adjustments**
@@ -2903,29 +4469,29 @@
 from deel_sdk.models import CandidateToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CandidateToCreateContainer(**{
-    "data": {
+request_body = CandidateToCreateContainer(
+    data={
         "id_": "id",
         "first_name": "John",
         "last_name": "Doe",
         "status": "offer-accepted",
         "start_date": "1999-12-31",
         "link": "link",
         "job_title": "3D Designer",
-        "email": "dolore",
+        "email": "do te",
         "nationality": "US",
         "country": "US",
         "state": "AL"
     }
-})
+)
 
 result = sdk.candidates.add_candidate(request_body=request_body)
 
 print(result)
 ```
 
 #### **patch_candidate**
@@ -2952,28 +4518,28 @@
 from deel_sdk.models import CandidateToPatchContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CandidateToPatchContainer(**{
-    "data": {
+request_body = CandidateToPatchContainer(
+    data={
         "first_name": "John",
         "last_name": "Doe",
         "status": "offer-accepted",
         "start_date": "1999-12-31",
         "job_title": "3D Designer",
         "link": "link",
-        "email": "Excepteur nu",
+        "email": "dolor",
         "nationality": "US",
         "country": "US",
         "state": "AL"
     }
-})
+)
 
 result = sdk.candidates.patch_candidate(
     request_body=request_body,
     candidate_id="candidate_id"
 )
 
 print(result)
@@ -3027,17 +4593,17 @@
 from deel_sdk.models import AdditionalEorInfoContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = AdditionalEorInfoContainer(**{
-    "data": ""
-})
+request_body = AdditionalEorInfoContainer(
+    data=""
+)
 
 result = sdk.partner_managed.add_employee_additional_information(
     request_body=request_body,
     employee_id="employee_id",
     contract_id="contract_id"
 )
 
@@ -3069,19 +4635,19 @@
 from deel_sdk.models import EmployeeContractSignatureToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = EmployeeContractSignatureToCreateContainer(**{
-    "data": {
-        "signature": "aliqua sed comm"
+request_body = EmployeeContractSignatureToCreateContainer(
+    data={
+        "signature": "cil"
     }
-})
+)
 
 result = sdk.partner_managed.sign_employee_contract(
     request_body=request_body,
     employee_id="employee_id",
     contract_id="contract_id"
 )
 
@@ -3113,21 +4679,21 @@
 from deel_sdk.models import RequestCustomVerificationLetterContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = RequestCustomVerificationLetterContainer(**{
-    "data": {
-        "description": "magnaest ea con",
+request_body = RequestCustomVerificationLetterContainer(
+    data={
+        "description": "ipsum suntullam",
         "include_qr_code": True,
         "type_": "VISA_APPLICATION_FOR_PERSONAL_TRIP"
     }
-})
+)
 
 result = sdk.partner_managed.request_custom_verification_letter(
     request_body=request_body,
     employee_id="employee_id",
     contract_id="contract_id"
 )
 
@@ -3196,15 +4762,15 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.partner_managed.download_hr_verification_letters_and_documents(
     employee_id="employee_id",
     contract_id="contract_id",
-    document_id=1.72
+    document_id=2.54
 )
 
 print(result)
 ```
 
 #### **get_offer_letter_preview**
 
@@ -3368,22 +4934,22 @@
 from deel_sdk.models import BankAccountToAddContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = BankAccountToAddContainer(**{
-    "data": [
+request_body = BankAccountToAddContainer(
+    data=[
         {
             "key": "key",
             "value": "value"
         }
     ]
-})
+)
 
 result = sdk.partner_managed.add_bank_account(
     request_body=request_body,
     employee_id="employee_id"
 )
 
 print(result)
@@ -3414,22 +4980,22 @@
 from deel_sdk.models import BankAccountToAddContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = BankAccountToAddContainer(**{
-    "data": [
+request_body = BankAccountToAddContainer(
+    data=[
         {
             "key": "key",
             "value": "value"
         }
     ]
-})
+)
 
 result = sdk.partner_managed.patch_bank_account(
     request_body=request_body,
     employee_id="employee_id",
     bank_id="bank_id"
 )
 
@@ -3530,15 +5096,15 @@
 request_body = {
     "file": "file"
 }
 
 result = sdk.partner_managed.upload_employee_compliance_document(
     request_body=request_body,
     employee_id="employee_id",
-    document_id=1.36
+    document_id=7.6
 )
 
 print(result)
 ```
 
 #### **get_employee_compliance_document_template**
 
@@ -3565,15 +5131,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.partner_managed.get_employee_compliance_document_template(
     employee_id="employee_id",
-    document_id=5.91
+    document_id=4.09
 )
 
 print(result)
 ```
 
 #### **get_employee_tax_documents**
 
@@ -3602,592 +5168,14 @@
 )
 
 result = sdk.partner_managed.get_employee_tax_documents(employee_id="employee_id")
 
 print(result)
 ```
 
-### ContractsService
-
-A list of all methods in the `ContractsService` service. Click on the method name to view detailed information about that method.
-
-| Methods                                                                     | Description                                                                                                                                                                                                          |
-| :-------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| [get_contract_list](#get_contract_list)                                     | Retrieve a list of contracts.                                                                                                                                                                                        |
-| [get_contract_by_id](#get_contract_by_id)                                   | Retrieve a single contract.                                                                                                                                                                                          |
-| [attach_external_id](#attach_external_id)                                   | Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later. |
-| [add_contract_document](#add_contract_document)                             | Attach a file to contract document.                                                                                                                                                                                  |
-| [edit_contract_document](#edit_contract_document)                           | Overwrite the file currently attached to contract document.                                                                                                                                                          |
-| [get_alternate_emails_by_contract_id](#get_alternate_emails_by_contract_id) | Returns an array of alternate email objects                                                                                                                                                                          |
-| [sign_contract](#sign_contract)                                             | Sign a contract as a client.                                                                                                                                                                                         |
-| [invite_to_sign_contract](#invite_to_sign_contract)                         | Invite a worker to sign the contract. Worker will be notified via email.                                                                                                                                             |
-| [uninvite_to_sign_contract](#uninvite_to_sign_contract)                     | Remove invite in order to re-invite a worker to sign the contract.                                                                                                                                                   |
-| [calculate_final_payment](#calculate_final_payment)                         | Calculate the final payment due to the contractor when ending the contract.                                                                                                                                          |
-| [post_contract_estimate](#post_contract_estimate)                           | First payment is calculated from the number of working/calendar days between their start date and the start of the payment cycle.                                                                                    |
-| [get_contract_templates](#get_contract_templates)                           | Retrieve a list of contract templates in your organization.                                                                                                                                                          |
-| [get_worker_documents_by_id](#get_worker_documents_by_id)                   | Retrieve a list of documents of a worker.                                                                                                                                                                            |
-| [get_download_worker_documents_by_id](#get_download_worker_documents_by_id) | Get the download link of worker document.                                                                                                                                                                            |
-
-#### **get_contract_list**
-
-Retrieve a list of contracts.
-
-- HTTP Method: `GET`
-- Endpoint: `/contracts`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| after_cursor | str | ❌ | Retrieve a list of contracts. |
-| limit | float | ❌ | Retrieve a list of contracts. |
-| order_direction | SortDirEnum | ❌ | Retrieve a list of contracts. |
-| types | List[ContractTypeEnum] | ❌ | Retrieve a list of contracts. |
-| statuses | List[ContractStatusEnum] | ❌ | Retrieve a list of contracts. |
-| team_id | str | ❌ | Retrieve a list of contracts. |
-| external_id | str | ❌ | Retrieve a list of contracts. |
-| countries | List[str] | ❌ | Retrieve a list of contracts. |
-| currencies | GetContractListCurrencies | ❌ | Retrieve a list of contracts. |
-| search | str | ❌ | Retrieve a list of contracts. |
-| sort_by | ContractsSortByEnum | ❌ | Retrieve a list of contracts. |
-
-**Return Type**
-
-`ContractListContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import SortDirEnum, GetContractListCurrencies, ContractsSortByEnum
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-types=[
-    "ongoing_time_based"
-]
-statuses=[
-    "new"
-]
-countries=[
-    "US"
-]
-currencies=GetContractListCurrencies(**[
-    "GBP"
-])
-
-result = sdk.contracts.get_contract_list(
-    after_cursor="after_cursor",
-    limit=10,
-    order_direction="asc",
-    types=types,
-    statuses=statuses,
-    team_id="team_id",
-    external_id="external_id",
-    countries=countries,
-    currencies=currencies,
-    search="search",
-    sort_by="contract_title"
-)
-
-print(result)
-```
-
-#### **get_contract_by_id**
-
-Retrieve a single contract.
-
-- HTTP Method: `GET`
-- Endpoint: `/contracts/{contract_id}`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| contract_id | str | ✅ | Retrieve a single contract. |
-
-**Return Type**
-
-`ContractContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.get_contract_by_id(contract_id="contract_id")
-
-print(result)
-```
-
-#### **attach_external_id**
-
-Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later.
-
-- HTTP Method: `PATCH`
-- Endpoint: `/contracts/{contract_id}`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | InputToPatchContractExternalId | ✅ | The request body. |
-| contract_id | str | ✅ | Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later. |
-
-**Return Type**
-
-`GenericResultCreated`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import InputToPatchContractExternalId
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-request_body = InputToPatchContractExternalId(**{
-    "data": {
-        "external_id": "external_id"
-    }
-})
-
-result = sdk.contracts.attach_external_id(
-    request_body=request_body,
-    contract_id="contract_id"
-)
-
-print(result)
-```
-
-#### **add_contract_document**
-
-Attach a file to contract document.
-
-- HTTP Method: `POST`
-- Endpoint: `/contracts/{contract_id}/documents`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | dict | ❌ | The request body. |
-| contract_id | str | ✅ | Attach a file to contract document. |
-
-**Return Type**
-
-`ContractDocumentContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import FileObject
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-request_body = {
-    "file": "file"
-}
-
-result = sdk.contracts.add_contract_document(
-    request_body=request_body,
-    contract_id="contract_id"
-)
-
-print(result)
-```
-
-#### **edit_contract_document**
-
-Overwrite the file currently attached to contract document.
-
-- HTTP Method: `PUT`
-- Endpoint: `/contracts/{contract_id}/documents`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | dict | ❌ | The request body. |
-| contract_id | str | ✅ | Overwrite the file currently attached to contract document. |
-
-**Return Type**
-
-`ContractDocumentContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import FileObject
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-request_body = {
-    "file": "file"
-}
-
-result = sdk.contracts.edit_contract_document(
-    request_body=request_body,
-    contract_id="contract_id"
-)
-
-print(result)
-```
-
-#### **get_alternate_emails_by_contract_id**
-
-Returns an array of alternate email objects
-
-- HTTP Method: `GET`
-- Endpoint: `/contracts/{contract_id}/alternate_emails`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| contract_id | str | ✅ | Returns an array of alternate email objects |
-
-**Return Type**
-
-`List[AlternateEmailItem]`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.get_alternate_emails_by_contract_id(contract_id="contract_id")
-
-print(result)
-```
-
-#### **sign_contract**
-
-Sign a contract as a client.
-
-- HTTP Method: `POST`
-- Endpoint: `/contracts/{contract_id}/signatures`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | ContractSignatureToCreateContainer | ✅ | The request body. |
-| contract_id | str | ✅ | Sign a contract as a client. |
-
-**Return Type**
-
-`GenericResultCreated`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import ContractSignatureToCreateContainer
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-request_body = ContractSignatureToCreateContainer(**{
-    "data": {
-        "client_signature": "ea exercitat",
-        "contract_template_id": 8.35
-    }
-})
-
-result = sdk.contracts.sign_contract(
-    request_body=request_body,
-    contract_id="contract_id"
-)
-
-print(result)
-```
-
-#### **invite_to_sign_contract**
-
-Invite a worker to sign the contract. Worker will be notified via email.
-
-- HTTP Method: `POST`
-- Endpoint: `/contracts/{contract_id}/invitations`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | ContractInvitationToCreateContainer | ✅ | The request body. |
-| contract_id | str | ✅ | Invite a worker to sign the contract. Worker will be notified via email. |
-
-**Return Type**
-
-`GenericResultCreated`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import ContractInvitationToCreateContainer
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-request_body = ContractInvitationToCreateContainer(**{
-    "data": {
-        "email": "eiusm",
-        "message": "officia ut"
-    }
-})
-
-result = sdk.contracts.invite_to_sign_contract(
-    request_body=request_body,
-    contract_id="contract_id"
-)
-
-print(result)
-```
-
-#### **uninvite_to_sign_contract**
-
-Remove invite in order to re-invite a worker to sign the contract.
-
-- HTTP Method: `DELETE`
-- Endpoint: `/contracts/{contract_id}/invitations`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| contract_id | str | ✅ | Remove invite in order to re-invite a worker to sign the contract. |
-
-**Return Type**
-
-`GenericResultDeleted`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.uninvite_to_sign_contract(contract_id="contract_id")
-
-print(result)
-```
-
-#### **calculate_final_payment**
-
-Calculate the final payment due to the contractor when ending the contract.
-
-- HTTP Method: `GET`
-- Endpoint: `/contracts/{contract_id}/final-payments`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| contract_id | str | ✅ | Calculate the final payment due to the contractor when ending the contract. |
-| end_date | str | ❌ | Calculate the final payment due to the contractor when ending the contract. |
-| calculation_type | CalculateFinalPaymentCalculationType | ❌ | Calculate the final payment due to the contractor when ending the contract. |
-| workweek_start | str | ❌ | Calculate the final payment due to the contractor when ending the contract. |
-| workweek_end | str | ❌ | Calculate the final payment due to the contractor when ending the contract. |
-
-**Return Type**
-
-`FinalPaymentCalculatedContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import CalculateFinalPaymentCalculationType
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.calculate_final_payment(
-    contract_id="contract_id",
-    end_date="1999-12-31",
-    calculation_type="CUSTOM_AMOUNT",
-    workweek_start="workweek_start",
-    workweek_end="workweek_end"
-)
-
-print(result)
-```
-
-#### **post_contract_estimate**
-
-First payment is calculated from the number of working/calendar days between their start date and the start of the payment cycle.
-
-- HTTP Method: `POST`
-- Endpoint: `/contracts/estimate`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | EstimateFirstPaymentContainer | ✅ | The request body. |
-
-**Return Type**
-
-`ResponseEstimateFirstPaymentContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import EstimateFirstPaymentContainer
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-request_body = EstimateFirstPaymentContainer(**{
-    "data": {
-        "type_": "ongoing_time_based",
-        "country_code": "US",
-        "start_date": "1999-12-31",
-        "compensation_details": {
-            "amount": 2500,
-            "currency_code": "GBP",
-            "scale": "weekly",
-            "cycle_end": 30.28,
-            "cycle_end_type": "DAY_OF_WEEK",
-            "payment_due_type": "REGULAR",
-            "payment_due_days": 11.81,
-            "calculation_type": "CUSTOM_AMOUNT",
-            "work_week_start": "Sunday",
-            "work_week_end": "Sunday"
-        }
-    }
-})
-
-result = sdk.contracts.post_contract_estimate(request_body=request_body)
-
-print(result)
-```
-
-#### **get_contract_templates**
-
-Retrieve a list of contract templates in your organization.
-
-- HTTP Method: `GET`
-- Endpoint: `/contract-templates`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-
-**Return Type**
-
-`ContractTemplateListContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.get_contract_templates()
-
-print(result)
-```
-
-#### **get_worker_documents_by_id**
-
-Retrieve a list of documents of a worker.
-
-- HTTP Method: `GET`
-- Endpoint: `/workers/{worker_id}/documents`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| worker_id | str | ✅ | Retrieve a list of documents of a worker. |
-
-**Return Type**
-
-`WorkerDocumentsByIdContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.get_worker_documents_by_id(worker_id="worker_id")
-
-print(result)
-```
-
-#### **get_download_worker_documents_by_id**
-
-Get the download link of worker document.
-
-- HTTP Method: `GET`
-- Endpoint: `/workers/{worker_id}/documents/{document_id}/download`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| worker_id | str | ✅ | Get the download link of worker document. |
-| document_id | float | ✅ | Get the download link of worker document. |
-
-**Return Type**
-
-`DownloadWorkerDocumentsByIdContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.get_download_worker_documents_by_id(
-    worker_id="worker_id",
-    document_id=8.43
-)
-
-print(result)
-```
-
 ### TasksService
 
 A list of all methods in the `TasksService` service. Click on the method name to view detailed information about that method.
 
 | Methods                                               | Description                                                     |
 | :---------------------------------------------------- | :-------------------------------------------------------------- |
 | [get_tasks_by_contract](#get_tasks_by_contract)       | Retrieve a list of tasks for a given contract.                  |
@@ -4251,25 +5239,25 @@
 from deel_sdk.models import InputToCreatePgoTask
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = InputToCreatePgoTask(**{
-    "data": {
+request_body = InputToCreatePgoTask(
+    data={
         "amount": "123.45",
         "date_submitted": "1999-12-31",
         "description": "Make the button pop.",
         "attachment": {
             "filename": "filename",
             "key": "key"
         }
     }
-})
+)
 
 result = sdk.tasks.create_contract_pgo_tak(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -4299,23 +5287,23 @@
 from deel_sdk.models import RequestBodyToCreatePgoTaskReviewsReviewsContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = RequestBodyToCreatePgoTaskReviewsReviewsContainer(**{
-    "data": {
+request_body = RequestBodyToCreatePgoTaskReviewsReviewsContainer(
+    data={
         "status": "approved",
         "reason": "Great work.",
         "ids": [
             "00000000-0000-0000-0000-000000000000"
         ]
     }
-})
+)
 
 result = sdk.tasks.create_task_many_review(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -4346,20 +5334,20 @@
 from deel_sdk.models import RequestBodyToCreatePgoTaskReviewsByIdReviewsContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = RequestBodyToCreatePgoTaskReviewsByIdReviewsContainer(**{
-    "data": {
+request_body = RequestBodyToCreatePgoTaskReviewsByIdReviewsContainer(
+    data={
         "status": "approved",
         "reason": "Excited!"
     }
-})
+)
 
 result = sdk.tasks.create_task_review_by_id(
     request_body=request_body,
     contract_id="contract_id",
     task_id="task_id"
 )
 
@@ -4461,15 +5449,15 @@
     contract_id="contract_id",
     contract_types=contract_types,
     statuses=statuses,
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=99,
-    offset=564786626.18
+    offset=38650248.43
 )
 
 print(result)
 ```
 
 #### **get_timesheets**
 
@@ -4514,15 +5502,15 @@
     contract_id="contract_id",
     contract_types=contract_types,
     statuses=statuses,
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=99,
-    offset=911169937.96
+    offset=530446812.74
 )
 
 print(result)
 ```
 
 #### **create_timesheet**
 
@@ -4547,22 +5535,22 @@
 from deel_sdk.models import TimesheetToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TimesheetToCreateContainer(**{
-    "data": {
+request_body = TimesheetToCreateContainer(
+    data={
         "contract_id": "contract_id",
         "description": "description",
         "date_submitted": "1999-12-31",
         "quantity": 2
     }
-})
+)
 
 result = sdk.timesheets.create_timesheet(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_timesheet_by_id**
@@ -4620,20 +5608,20 @@
 from deel_sdk.models import TimesheetToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TimesheetToUpdateContainer(**{
-    "data": {
+request_body = TimesheetToUpdateContainer(
+    data={
         "description": "description",
-        "quantity": 3.77
+        "quantity": 8.4
     }
-})
+)
 
 result = sdk.timesheets.update_timesheet_by_id(
     request_body=request_body,
     timesheet_id="timesheet_id"
 )
 
 print(result)
@@ -4698,20 +5686,20 @@
 from deel_sdk.models import TimesheetReviewToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TimesheetReviewToCreateContainer(**{
-    "data": {
+request_body = TimesheetReviewToCreateContainer(
+    data={
         "status": "approved",
         "reason": "reason"
     }
-})
+)
 
 result = sdk.timesheets.create_timesheet_review(
     request_body=request_body,
     timesheet_id="timesheet_id"
 )
 
 print(result)
@@ -4740,23 +5728,23 @@
 from deel_sdk.models import TimesheetReviewsToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TimesheetReviewsToCreateContainer(**{
-    "data": {
+request_body = TimesheetReviewsToCreateContainer(
+    data={
         "status": "approved",
         "reason": "reason",
         "ids": [
-            1.77
+            8.09
         ]
     }
-})
+)
 
 result = sdk.timesheets.create_timesheet_reviews(request_body=request_body)
 
 print(result)
 ```
 
 ### MilestonesService
@@ -4827,21 +5815,21 @@
 from deel_sdk.models import MilestoneToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = MilestoneToCreateContainer(**{
-    "data": {
+request_body = MilestoneToCreateContainer(
+    data={
         "amount": "900.00",
         "title": "Sprint 2",
         "description": "Sprint #2"
     }
-})
+)
 
 result = sdk.milestones.create_milestone(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -4942,20 +5930,20 @@
 from deel_sdk.models import MilestoneReviewToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = MilestoneReviewToCreateContainer(**{
-    "data": {
+request_body = MilestoneReviewToCreateContainer(
+    data={
         "status": "approved",
         "reason": "reason"
     }
-})
+)
 
 result = sdk.milestones.create_milestone_review(
     request_body=request_body,
     contract_id="contract_id",
     milestone_id="milestone_id"
 )
 
@@ -4986,23 +5974,23 @@
 from deel_sdk.models import MilestoneReviewsToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = MilestoneReviewsToCreateContainer(**{
-    "data": {
+request_body = MilestoneReviewsToCreateContainer(
+    data={
         "status": "approved",
         "reason": "reason",
         "ids": [
-            6.78
+            "00000000-0000-0000-0000-000000000000"
         ]
     }
-})
+)
 
 result = sdk.milestones.create_milestone_reviews(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -5073,21 +6061,21 @@
 from deel_sdk.models import OffCyclePaymentToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = OffCyclePaymentToCreateContainer(**{
-    "data": {
+request_body = OffCyclePaymentToCreateContainer(
+    data={
         "date_submitted": "1999-12-31",
         "amount": 2500,
         "description": "description"
     }
-})
+)
 
 result = sdk.off_cycle_payments.create_off_cycle_payment(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -5197,26 +6185,26 @@
 from deel_sdk.models import CreateTimeoffContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CreateTimeoffContainer(**{
-    "data": {
+request_body = CreateTimeoffContainer(
+    data={
         "type_": "VACATION",
         "start_date": "2022-09-03T00:00:00.000Z",
         "end_date": "2022-09-05T00:00:00.000Z",
         "with_multiple_dates": True,
         "reason": "Holiday",
-        "is_start_date_half_day": True,
+        "is_start_date_half_day": False,
         "is_end_date_half_day": False,
         "other_timeoff_name": "Birthday"
     }
-})
+)
 
 result = sdk.time_off.create_eor_time_offs(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -5247,26 +6235,26 @@
 from deel_sdk.models import CreateTimeoffContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CreateTimeoffContainer(**{
-    "data": {
+request_body = CreateTimeoffContainer(
+    data={
         "type_": "VACATION",
         "start_date": "2022-09-03T00:00:00.000Z",
         "end_date": "2022-09-05T00:00:00.000Z",
         "with_multiple_dates": True,
         "reason": "Holiday",
-        "is_start_date_half_day": True,
+        "is_start_date_half_day": False,
         "is_end_date_half_day": False,
         "other_timeoff_name": "Birthday"
     }
-})
+)
 
 result = sdk.time_off.edit_eor_time_offs(
     request_body=request_body,
     contract_id="contract_id",
     timeoff_id="timeoff_id"
 )
 
@@ -5393,20 +6381,20 @@
 from deel_sdk.models import TimeoffToReviewContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TimeoffToReviewContainer(**{
-    "data": {
+request_body = TimeoffToReviewContainer(
+    data={
         "is_approved": True,
         "denial_reason": "Not allowed for this day."
     }
-})
+)
 
 result = sdk.time_off.review_timeoff(
     request_body=request_body,
     timeoff_id="timeoff_id"
 )
 
 print(result)
@@ -5477,15 +6465,15 @@
     types=types,
     statuses=statuses,
     invoice_id="invoice_id",
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=10,
-    offset=226515477.25
+    offset=893166763.24
 )
 
 print(result)
 ```
 
 #### **get_invoice_adjustments**
 
@@ -5537,15 +6525,15 @@
     types=types,
     statuses=statuses,
     invoice_id="invoice_id",
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=10,
-    offset=240522187.51
+    offset=114760289.77
 )
 
 print(result)
 ```
 
 #### **create_invoice_adjustment**
 
@@ -5571,24 +6559,24 @@
 from deel_sdk.models import InvoiceAdjustmentToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = InvoiceAdjustmentToCreateContainer(**{
-    "data": {
+request_body = InvoiceAdjustmentToCreateContainer(
+    data={
         "contract_id": "contract_id",
         "date_submitted": "1999-12-31",
         "type_": "bonus",
         "amount": 2500,
         "description": "Bonus for being awesome.",
-        "payment_cycle_id": 6.69
+        "payment_cycle_id": 7.22
     }
-})
+)
 
 result = sdk.invoices.create_invoice_adjustment(
     request_body=request_body,
     recurring=False
 )
 
 print(result)
@@ -5618,20 +6606,20 @@
 from deel_sdk.models import InvoiceAdjustmentToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = InvoiceAdjustmentToUpdateContainer(**{
-    "data": {
-        "description": "sunt laborum Duis exercitation id",
-        "amount": 9.39
+request_body = InvoiceAdjustmentToUpdateContainer(
+    data={
+        "description": "nostrud ad ullamco dolor",
+        "amount": 9.38
     }
-})
+)
 
 result = sdk.invoices.update_invoice_adjustment_by_id(
     request_body=request_body,
     invoice_adjustment_id="invoice_adjustment_id"
 )
 
 print(result)
@@ -5696,20 +6684,20 @@
 from deel_sdk.models import InvoiceAdjustmentReviewToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = InvoiceAdjustmentReviewToCreateContainer(**{
-    "data": {
+request_body = InvoiceAdjustmentReviewToCreateContainer(
+    data={
         "status": "approved",
         "reason": "reason"
     }
-})
+)
 
 result = sdk.invoices.create_invoice_adjustment_review(
     request_body=request_body,
     invoice_adjustment_id="invoice_adjustment_id"
 )
 
 print(result)
@@ -5738,23 +6726,23 @@
 from deel_sdk.models import InvoiceAdjustmentReviewsToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = InvoiceAdjustmentReviewsToCreateContainer(**{
-    "data": {
+request_body = InvoiceAdjustmentReviewsToCreateContainer(
+    data={
         "status": "approved",
         "reason": "reason",
         "ids": [
-            1.77
+            8.09
         ]
     }
-})
+)
 
 result = sdk.invoices.create_invoice_adjustment_reviews(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_invoice_adjustments_attachment**
@@ -6223,25 +7211,25 @@
 from deel_sdk.models import CreateWebhookRequest
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CreateWebhookRequest(**{
-    "name": "My first webhook.",
-    "description": "I like it very much.",
-    "status": "enabled",
-    "url": "https://mywebhook.com",
-    "signing_key": "signing_key",
-    "api_version": "v2",
-    "events": [
+request_body = CreateWebhookRequest(
+    name="My first webhook.",
+    description="I like it very much.",
+    status="enabled",
+    url="https://mywebhook.com",
+    signing_key="signing_key",
+    api_version="v2",
+    events=[
         "events"
     ]
-})
+)
 
 result = sdk.webhooks.create_webhook(request_body=request_body)
 
 print(result)
 ```
 
 #### **webhook_controller_get_by_id**
@@ -6299,25 +7287,25 @@
 from deel_sdk.models import PatchWebhookRequest
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = PatchWebhookRequest(**{
-    "name": "Demo webhook",
-    "description": "My first webhook",
-    "status": "enabled",
-    "url": "https://mywebhook.com/listening",
-    "signing_key": "signing_key",
-    "api_version": "v2",
-    "events": [
+request_body = PatchWebhookRequest(
+    name="Demo webhook",
+    description="My first webhook",
+    status="enabled",
+    url="https://mywebhook.com/listening",
+    signing_key="signing_key",
+    api_version="v2",
+    events=[
         "events"
     ]
-})
+)
 
 result = sdk.webhooks.webhook_controller_edit_by_id(
     request_body=request_body,
     id_="id"
 )
 
 print(result)
@@ -6411,21 +7399,21 @@
 from deel_sdk.models import CreatePublicTokenContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CreatePublicTokenContainer(**{
-    "data": {
+request_body = CreatePublicTokenContainer(
+    data={
         "scope": [
             "contracts:read"
         ]
     }
-})
+)
 
 result = sdk.token.create_public_token(request_body=request_body)
 
 print(result)
 ```
 
 ### CartaService
```

### Comparing `deel_sdk-1.0.2/src/deel_sdk/hooks/hook.py` & `deel_sdk-1.0.4/src/deel_sdk/hooks/hook.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,15 +22,17 @@
         return "Response(status={}, headers={}, body={})".format(
             self.status, self.headers, self.body
         )
 
 
 class DefaultHook:
 
-    def before_request(self, request: Request):
+    def before_request(self, request: Request, **kwargs):
         pass
 
-    def after_response(self, request: Request, response: Response):
+    def after_response(self, request: Request, response: Response, **kwargs):
         pass
 
-    def on_error(self, error: Exception, request: Request, response: Response):
+    def on_error(
+        self, error: Exception, request: Request, response: Response, **kwargs
+    ):
         pass
```

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/__init__.py` & `deel_sdk-1.0.4/src/deel_sdk/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,39 +4,84 @@
 from .get_invoice_list_entities import GetInvoiceListEntities
 from .deel_invoice_list_container import DeelInvoiceListContainer
 from .invoice_download_link_container import InvoiceDownloadLinkContainer
 from .payment_list_container import PaymentListContainer
 from .get_payment_list_currencies import GetPaymentListCurrencies
 from .get_payment_list_entities import GetPaymentListEntities
 from .payment_break_down_container import PaymentBreakDownContainer
+from .custom_fields_list_container import CustomFieldsListContainer
+from .custom_field_item_container import CustomFieldItemContainer
+from .custom_field_values_container import CustomFieldValuesContainer
+from .custom_field_to_update_container import CustomFieldToUpdateContainer
+from .get_roles_container import GetRolesContainer
+from .role_to_create_container import RoleToCreateContainer
+from .created_role_container import CreatedRoleContainer
+from .role_to_update_container import RoleToUpdateContainer
+from .updated_role_container import UpdatedRoleContainer
+from .exercise_equity_to_create_container import ExerciseEquityToCreateContainer
+from .created_exercise_equity_container import CreatedExerciseEquityContainer
+from .exercise_equity_to_update_container import ExerciseEquityToUpdateContainer
+from .updated_exercise_equity_container import UpdatedExerciseEquityContainer
+from .contract_list_container import ContractListContainer
+from .sort_dir_enum import SortDirEnum
+from .contract_type_enum import ContractTypeEnum
+from .contract_status_enum import ContractStatusEnum
+from .get_contract_list_currencies import GetContractListCurrencies
+from .contracts_sort_by_enum import ContractsSortByEnum
+from .contract_container import ContractContainer
+from .input_to_patch_contract_external_id import InputToPatchContractExternalId
+from .generic_result_created import GenericResultCreated
+from .file_object import FileObject
+from .contract_document_container import ContractDocumentContainer
+from .alternate_email_item import AlternateEmailItem
+from .contract_signature_to_create_container import ContractSignatureToCreateContainer
+from .generic_result_updated import GenericResultUpdated
+from .contract_invitation_to_create_container import ContractInvitationToCreateContainer
+from .generic_result_deleted import GenericResultDeleted
+from .final_payment_calculated_container import FinalPaymentCalculatedContainer
+from .calculate_final_payment_calculation_type import (
+    CalculateFinalPaymentCalculationType,
+)
+from .estimate_first_payment_container import EstimateFirstPaymentContainer
+from .response_estimate_first_payment_container import (
+    ResponseEstimateFirstPaymentContainer,
+)
+from .contract_template_list_container import ContractTemplateListContainer
+from .worker_documents_by_id_container import WorkerDocumentsByIdContainer
+from .download_worker_documents_by_id_container import (
+    DownloadWorkerDocumentsByIdContainer,
+)
+from .get_all_org_structures_container import GetAllOrgStructuresContainer
+from .org_structure_to_create_container import OrgStructureToCreateContainer
+from .get_org_structure_container import GetOrgStructureContainer
+from .org_structure_to_update_container import OrgStructureToUpdateContainer
+from .get_hris_position_container import GetHrisPositionContainer
+from .hris_position_to_change_container import HrisPositionToChangeContainer
 from .admin_users_container import AdminUsersContainer
 from .admin_user_create_container import AdminUserCreateContainer
 from .create_admin_user_response_container import CreateAdminUserResponseContainer
 from .hris_direct_employee import HrisDirectEmployee
 from .hris_direct_employee_container import HrisDirectEmployeeContainer
 from .internal_people_container import InternalPeopleContainer
 from .people_container import PeopleContainer
 from .people_sort_by_enum import PeopleSortByEnum
-from .sort_dir_enum import SortDirEnum
 from .hiring_status_enum import HiringStatusEnum
 from .people_by_id_container import PeopleByIdContainer
 from .update_worker_department_container import UpdateWorkerDepartmentContainer
-from .generic_result_updated import GenericResultUpdated
 from .update_worker_working_location_container import (
     UpdateWorkerWorkingLocationContainer,
 )
 from .people_me import PeopleMe
 from .employee_timeoffs_container import EmployeeTimeoffsContainer
 from .create_people_timeoff import CreatePeopleTimeoff
 from .employee_timeoffs_creation_container import EmployeeTimeoffsCreationContainer
 from .employee_timeoffs_entitlements_container import (
     EmployeeTimeoffsEntitlementsContainer,
 )
 from .people_time_off_container import PeopleTimeOffContainer
-from .generic_result_deleted import GenericResultDeleted
 from .timeoff_to_review_internal_container import TimeoffToReviewInternalContainer
 from .employee_timeoffs_policies_container import EmployeeTimeoffsPoliciesContainer
 from .eor_country_validations_container import EorCountryValidationsContainer
 from .eor_payslips_list_container import EorPayslipsListContainer
 from .eor_payslip_download_url_container import EorPayslipDownloadUrlContainer
 from .eor_employee_cost_calculation_request_body_container import (
     EorEmployeeCostCalculationRequestBodyContainer,
@@ -87,17 +132,15 @@
 )
 from .contract_container_payg_milestones import ContractContainerPaygMilestones
 from .contract_to_create_container_ongoing_time_based import (
     ContractToCreateContainerOngoingTimeBased,
 )
 from .contract_container_ongoing_time_based import ContractContainerOngoingTimeBased
 from .contract_to_create_container import ContractToCreateContainer
-from .contract_container import ContractContainer
 from .contract_to_amend_details_container import ContractToAmendDetailsContainer
-from .generic_result_created import GenericResultCreated
 from .contract_to_terminate_container import ContractToTerminateContainer
 from .contract_termination_result_container import ContractTerminationResultContainer
 from .premium_to_add_container import PremiumToAddContainer
 from .premium_result_added_container import PremiumResultAddedContainer
 from .adjustment_to_create_container import AdjustmentToCreateContainer
 from .adjustment_created_container import AdjustmentCreatedContainer
 from .adjustment_to_update_container import AdjustmentToUpdateContainer
@@ -133,38 +176,14 @@
 from .upload_employee_compliance_document_container import (
     UploadEmployeeComplianceDocumentContainer,
 )
 from .get_employee_compliance_document_template_download_link_container import (
     GetEmployeeComplianceDocumentTemplateDownloadLinkContainer,
 )
 from .employee_tax_documents_list_container import EmployeeTaxDocumentsListContainer
-from .contract_list_container import ContractListContainer
-from .contract_type_enum import ContractTypeEnum
-from .contract_status_enum import ContractStatusEnum
-from .get_contract_list_currencies import GetContractListCurrencies
-from .contracts_sort_by_enum import ContractsSortByEnum
-from .input_to_patch_contract_external_id import InputToPatchContractExternalId
-from .file_object import FileObject
-from .contract_document_container import ContractDocumentContainer
-from .alternate_email_item import AlternateEmailItem
-from .contract_signature_to_create_container import ContractSignatureToCreateContainer
-from .contract_invitation_to_create_container import ContractInvitationToCreateContainer
-from .final_payment_calculated_container import FinalPaymentCalculatedContainer
-from .calculate_final_payment_calculation_type import (
-    CalculateFinalPaymentCalculationType,
-)
-from .estimate_first_payment_container import EstimateFirstPaymentContainer
-from .response_estimate_first_payment_container import (
-    ResponseEstimateFirstPaymentContainer,
-)
-from .contract_template_list_container import ContractTemplateListContainer
-from .worker_documents_by_id_container import WorkerDocumentsByIdContainer
-from .download_worker_documents_by_id_container import (
-    DownloadWorkerDocumentsByIdContainer,
-)
 from .task_list_container import TaskListContainer
 from .input_to_create_pgo_task import InputToCreatePgoTask
 from .task_created_container import TaskCreatedContainer
 from .request_body_to_create_pgo_task_reviews_reviews_container import (
     RequestBodyToCreatePgoTaskReviewsReviewsContainer,
 )
 from .request_body_to_create_pgo_task_reviews_by_id_reviews_container import (
@@ -238,29 +257,71 @@
 from .payment_object import PaymentObject
 from .payment import Payment
 from .payment_method import PaymentMethod
 from .payment_status_enum import PaymentStatusEnum
 from .payment_worker import PaymentWorker
 from .payment_method_enum import PaymentMethodEnum
 from .payment_break_down import PaymentBreakDown
+from .custom_fields_object import CustomFieldsObject
+from .get_roles_item import GetRolesItem
+from .basic_contract import BasicContract
+from .page_info import PageInfo
+from .client_of_basic_contract import ClientOfBasicContract
+from .worker_of_basic_contract import WorkerOfBasicContract
+from .invitations_of_basic_contract import InvitationsOfBasicContract
+from .signatures_of_basic_contract import SignaturesOfBasicContract
+from .contract_who_reports_enum import ContractWhoReportsEnum
+from .team_of_basic_contract import TeamOfBasicContract
+from .identifier_value import IdentifierValue
+from .contract import Contract
+from .seniority import Seniority
+from .client_of_contract import ClientOfContract
+from .worker_of_contract import WorkerOfContract
+from .signatures_of_contract import SignaturesOfContract
+from .compensation_details_of_contract import CompensationDetailsOfContract
+from .employment_details_of_contract import EmploymentDetailsOfContract
+from .contract_template import ContractTemplate
+from .contract_custom_field import ContractCustomField
+from .eor_quote_base import EorQuoteBase
+from .team_of_contract import TeamOfContract
+from .client_of_contract_legal_entity_1 import ClientOfContractLegalEntity1
+from .worker_legal_entity import WorkerLegalEntity
+from .breakdown_costs_quote import BreakdownCostsQuote
+from .cost_quote import CostQuote
+from .contract_external_id_to_patch import ContractExternalIdToPatch
+from .file_attachment_info import FileAttachmentInfo
+from .contract_signature_to_create import ContractSignatureToCreate
+from .contract_invitation_to_create import ContractInvitationToCreate
+from .final_payment_calculated import FinalPaymentCalculated
+from .estimate_first_payment import EstimateFirstPayment
+from .contract_type_enum_for_estimate import ContractTypeEnumForEstimate
+from .work_statement_cycle_scale_enum import WorkStatementCycleScaleEnum
+from .work_statement_cycle_end_type_enum import WorkStatementCycleEndTypeEnum
+from .work_statement_payment_due_type_enum import WorkStatementPaymentDueTypeEnum
+from .week_days_enum import WeekDaysEnum
+from .response_estimate_first_payment import ResponseEstimateFirstPayment
+from .pro_rata import ProRata
+from .first_payment_date import FirstPaymentDate
+from .contract_template_summary import ContractTemplateSummary
+from .worker_document import WorkerDocument
+from .worker_document_download_link import WorkerDocumentDownloadLink
 from .admin_user import AdminUser
 from .admin_user_create_request import AdminUserCreateRequest
 from .hris_direct_employee_details import HrisDirectEmployeeDetails
 from .hris_team_information import HrisTeamInformation
 from .hris_compensation import HrisCompensation
 from .hris_job_information_title_id import HrisJobInformationTitleId
 from .hris_job_information_title_name import HrisJobInformationTitleName
 from .hris_contract_part_time import HrisContractPartTime
 from .hris_contract_full_time import HrisContractFullTime
 from .hris_direct_employee_response import HrisDirectEmployeeResponse
 from .internal_people import InternalPeople
 from .people_client_legal_entity import PeopleClientLegalEntity
 from .monthly_payment import MonthlyPayment
 from .employment import Employment
-from .identifier_value import IdentifierValue
 from .team import Team
 from .people_payment import PeoplePayment
 from .employee import Employee
 from .address import Address
 from .email import Email
 from .employment_detail import EmploymentDetail
 from .people_custom_field import PeopleCustomField
@@ -286,15 +347,14 @@
 from .eor_employee_cost_calculation_request_body import (
     EorEmployeeCostCalculationRequestBody,
 )
 from .eor_contract_benefits import EorContractBenefits
 from .eor_contract_to_create import EorContractToCreate
 from .pension_eor_contract_to_create import PensionEorContractToCreate
 from .eor_contract_created import EorContractCreated
-from .seniority import Seniority
 from .gp_contract_to_create import GpContractToCreate
 from .gp_client import GpClient
 from .gp_contract_status_type_enum import GpContractStatusTypeEnum
 from .gp_contract_created import GpContractCreated
 from .gp_employee_address_update_data import GpEmployeeAddressUpdateData
 from .gp_employee_address_updated import GpEmployeeAddressUpdated
 from .worker_bank_account_info import WorkerBankAccountInfo
@@ -314,35 +374,16 @@
 from .gp_payroll_event_reports import GpPayrollEventReports
 from .global_payroll_g2_n_report import GlobalPayrollG2NReport
 from .worker_termination_body import WorkerTerminationBody
 from .worker_termination import WorkerTermination
 from .contract_to_create_pay_as_you_go_time_based import (
     ContractToCreatePayAsYouGoTimeBased,
 )
-from .contract_who_reports_enum import ContractWhoReportsEnum
 from .meta_data_of_contract_to_create import MetaDataOfContractToCreate
-from .work_statement_cycle_scale_enum import WorkStatementCycleScaleEnum
-from .work_statement_cycle_end_type_enum import WorkStatementCycleEndTypeEnum
-from .work_statement_payment_due_type_enum import WorkStatementPaymentDueTypeEnum
 from .work_statement_scale_enum import WorkStatementScaleEnum
-from .contract import Contract
-from .client_of_contract import ClientOfContract
-from .worker_of_contract import WorkerOfContract
-from .invitations_of_basic_contract import InvitationsOfBasicContract
-from .signatures_of_contract import SignaturesOfContract
-from .compensation_details_of_contract import CompensationDetailsOfContract
-from .employment_details_of_contract import EmploymentDetailsOfContract
-from .contract_template import ContractTemplate
-from .contract_custom_field import ContractCustomField
-from .eor_quote_base import EorQuoteBase
-from .team_of_contract import TeamOfContract
-from .client_of_contract_legal_entity_5 import ClientOfContractLegalEntity5
-from .worker_legal_entity import WorkerLegalEntity
-from .breakdown_costs_quote import BreakdownCostsQuote
-from .cost_quote import CostQuote
 from .contract_to_create_payg_tasks import ContractToCreatePaygTasks
 from .compensation_details_of_contract_to_create_shared import (
     CompensationDetailsOfContractToCreateShared,
 )
 from .contract_to_create_payg_milestones import ContractToCreatePaygMilestones
 from .contract_to_create_ongoing_time_based import ContractToCreateOngoingTimeBased
 from .contract_to_create import ContractToCreate
@@ -366,34 +407,14 @@
 from .hr_document_info import HrDocumentInfo
 from .employee_agreement_download_object import EmployeeAgreementDownloadObject
 from .bank_account_to_add import BankAccountToAdd
 from .bank_account_added import BankAccountAdded
 from .bank_account_status import BankAccountStatus
 from .employee_payslips_list import EmployeePayslipsList
 from .employee_tax_documents_list import EmployeeTaxDocumentsList
-from .basic_contract import BasicContract
-from .page_info import PageInfo
-from .client_of_basic_contract import ClientOfBasicContract
-from .worker_of_basic_contract import WorkerOfBasicContract
-from .signatures_of_basic_contract import SignaturesOfBasicContract
-from .team_of_basic_contract import TeamOfBasicContract
-from .contract_external_id_to_patch import ContractExternalIdToPatch
-from .file_attachment_info import FileAttachmentInfo
-from .contract_signature_to_create import ContractSignatureToCreate
-from .contract_invitation_to_create import ContractInvitationToCreate
-from .final_payment_calculated import FinalPaymentCalculated
-from .estimate_first_payment import EstimateFirstPayment
-from .contract_type_enum_for_estimate import ContractTypeEnumForEstimate
-from .week_days_enum import WeekDaysEnum
-from .response_estimate_first_payment import ResponseEstimateFirstPayment
-from .pro_rata import ProRata
-from .first_payment_date import FirstPaymentDate
-from .contract_template_summary import ContractTemplateSummary
-from .worker_document import WorkerDocument
-from .worker_document_download_link import WorkerDocumentDownloadLink
 from .pgo_task import PgoTask
 from .pgo_task_to_create import PgoTaskToCreate
 from .task_created import TaskCreated
 from .pgo_task_reviews_to_create import PgoTaskReviewsToCreate
 from .pgo_task_reviews_by_id_to_create import PgoTaskReviewsByIdToCreate
 from .basic_timesheet import BasicTimesheet
 from .page_info_without_cursor import PageInfoWithoutCursor
```

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/add_worker_bank_account_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/add_worker_bank_account_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/address.py` & `deel_sdk-1.0.4/src/deel_sdk/models/address.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/adjustment_category.py` & `deel_sdk-1.0.4/src/deel_sdk/models/adjustment_category.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/adjustment_status_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/adjustment_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/adjustment_to_create.py` & `deel_sdk-1.0.4/src/deel_sdk/models/adjustment_to_create.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/adjustment_to_create_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/adjustment_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/adjustment_to_update.py` & `deel_sdk-1.0.4/src/deel_sdk/models/adjustment_to_update.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/adjustment_to_update_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/adjustment_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/adjustments_categories_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/adjustments_categories_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/admin_user.py` & `deel_sdk-1.0.4/src/deel_sdk/models/admin_user.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/admin_user_create_request.py` & `deel_sdk-1.0.4/src/deel_sdk/models/admin_user_create_request.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/admin_users_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/admin_users_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/agreement.py` & `deel_sdk-1.0.4/src/deel_sdk/models/agreement.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/agreement_list_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/agreement_list_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/bank_account_added.py` & `deel_sdk-1.0.4/src/deel_sdk/models/bank_account_added.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/bank_account_guide.py` & `deel_sdk-1.0.4/src/deel_sdk/models/bank_account_guide.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/bank_account_status.py` & `deel_sdk-1.0.4/src/deel_sdk/models/bank_account_status.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/bank_account_updated.py` & `deel_sdk-1.0.4/src/deel_sdk/models/bank_account_updated.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/bank_account_value_allowed.py` & `deel_sdk-1.0.4/src/deel_sdk/models/bank_account_value_allowed.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/base.py` & `deel_sdk-1.0.4/src/deel_sdk/models/base.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/basic_contract.py` & `deel_sdk-1.0.4/src/deel_sdk/models/basic_contract.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/basic_invoice_adjustment.py` & `deel_sdk-1.0.4/src/deel_sdk/models/basic_invoice_adjustment.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/basic_legal_entity.py` & `deel_sdk-1.0.4/src/deel_sdk/models/basic_legal_entity.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/basic_timesheet.py` & `deel_sdk-1.0.4/src/deel_sdk/models/basic_timesheet.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/benefit_contribution_type_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/benefit_contribution_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/benefit_status_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/benefit_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/breakdown_costs_quote.py` & `deel_sdk-1.0.4/src/deel_sdk/models/breakdown_costs_quote.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/calculate_final_payment_calculation_type.py` & `deel_sdk-1.0.4/src/deel_sdk/models/calculate_final_payment_calculation_type.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/candidate_status_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/candidate_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/candidate_to_create.py` & `deel_sdk-1.0.4/src/deel_sdk/models/candidate_to_create.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/candidate_to_patch.py` & `deel_sdk-1.0.4/src/deel_sdk/models/candidate_to_patch.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/client_of_basic_contract.py` & `deel_sdk-1.0.4/src/deel_sdk/models/client_of_basic_contract.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/client_of_contract.py` & `deel_sdk-1.0.4/src/deel_sdk/models/client_of_contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file was generated by liblab | https://liblab.com/
 
 from __future__ import annotations
 from .utils.json_map import JsonMap
 from .base import BaseModel
 from .identifier_value import IdentifierValue, IdentifierValueGuard
 from .team_of_contract import TeamOfContract
-from .client_of_contract_legal_entity_5 import ClientOfContractLegalEntity5
+from .client_of_contract_legal_entity_1 import ClientOfContractLegalEntity1
 
 
 @JsonMap({"id_": "id"})
 class ClientOfContract(BaseModel):
     """ClientOfContract
 
     :param id_: id_, defaults to None
@@ -17,28 +17,28 @@
     :param full_name: full_name, defaults to None
     :type full_name: str, optional
     :param email: User's email address., defaults to None
     :type email: str, optional
     :param team: team
     :type team: TeamOfContract
     :param legal_entity: legal_entity
-    :type legal_entity: ClientOfContractLegalEntity5
+    :type legal_entity: ClientOfContractLegalEntity1
     """
 
     def __init__(
         self,
         team: TeamOfContract,
-        legal_entity: ClientOfContractLegalEntity5,
+        legal_entity: ClientOfContractLegalEntity1,
         id_: IdentifierValue = None,
         full_name: str = None,
         email: str = None,
     ):
         if id_ is not None:
             self.id_ = IdentifierValueGuard.return_one_of(id_)
         if full_name is not None:
             self.full_name = full_name
         if email is not None:
             self.email = email
         self.team = self._define_object(team, TeamOfContract)
         self.legal_entity = self._define_object(
-            legal_entity, ClientOfContractLegalEntity5
+            legal_entity, ClientOfContractLegalEntity1
         )
```

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/client_of_contract_legal_entity_5.py` & `deel_sdk-1.0.4/src/deel_sdk/models/client_of_contract_legal_entity_1.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from .utils.json_map import JsonMap
 from .base import BaseModel
 from .identifier_value import IdentifierValue, IdentifierValueGuard
 from .legal_entity_type import LegalEntityType
 
 
 @JsonMap({"id_": "id", "type_": "type"})
-class ClientOfContractLegalEntity5(BaseModel):
-    """ClientOfContractLegalEntity5
+class ClientOfContractLegalEntity1(BaseModel):
+    """ClientOfContractLegalEntity1
 
     :param id_: id_
     :type id_: IdentifierValue
     :param name: name
     :type name: str
     :param email: User's email address.
     :type email: str
```

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/compensation_details_of_contract.py` & `deel_sdk-1.0.4/src/deel_sdk/models/compensation_details_of_contract.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/compensation_details_of_contract_to_create_shared.py` & `deel_sdk-1.0.4/src/deel_sdk/models/compensation_details_of_contract_to_create_shared.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_custom_field.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_custom_field.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_details_to_amend.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_details_to_amend.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_document_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_document_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_invitation_to_create_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_invitation_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_list_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_list_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_signature_to_create.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_signature_to_create.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_signature_to_create_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_signature_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_status_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_template.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_template.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_template_list_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_template_list_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_template_summary.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_template_summary.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_termination_result.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_termination_result.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_termination_result_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_termination_result_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_amend_details_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_to_amend_details_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_to_create.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_container_ongoing_time_based.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_to_create_container_ongoing_time_based.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_container_pay_as_you_go_time_based.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_to_create_container_pay_as_you_go_time_based.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_container_payg_milestones.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_to_create_container_payg_milestones.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_container_payg_tasks.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_to_create_container_payg_tasks.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_ongoing_time_based.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_to_create_ongoing_time_based.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # This file was generated by liblab | https://liblab.com/
 
 from __future__ import annotations
 from enum import Enum
+from typing import Union
 from .utils.json_map import JsonMap
 from .base import BaseModel
+from .base import OneOfBaseModel
 from .contract_who_reports_enum import ContractWhoReportsEnum
 from .meta_data_of_contract_to_create import MetaDataOfContractToCreate
 from .identifier_value import IdentifierValue, IdentifierValueGuard
 from .work_statement_cycle_scale_enum import WorkStatementCycleScaleEnum
 from .work_statement_cycle_end_type_enum import WorkStatementCycleEndTypeEnum
 from .work_statement_payment_due_type_enum import WorkStatementPaymentDueTypeEnum
 from .work_statement_scale_enum import WorkStatementScaleEnum
@@ -52,38 +54,45 @@
         self.team = self._define_object(team, ClientTeam5)
 
 
 @JsonMap({"id_": "id"})
 class ContractToCreateOngoingTimeBasedJobTitle(BaseModel):
     """Worker's job title. You can enter a custom job title or use a pre-defiled job title using the Id retrieved in job-titles endpoint.
 
-    :param id_: Unique identifier of this resource., defaults to None
+    :param id_: Job title ID., defaults to None
     :type id_: str, optional
     :param name: Job title. Please leave it blank when entering an Id., defaults to None
     :type name: str, optional
     """
 
     def __init__(self, id_: str = None, name: str = None):
         if id_ is not None:
             self.id_ = id_
         if name is not None:
             self.name = name
 
 
+class SeniorityId4Guard(OneOfBaseModel):
+    class_list = {"float": float, "str": str}
+
+
+SeniorityId4 = Union[float, str]
+
+
 @JsonMap({"id_": "id"})
 class ContractToCreateOngoingTimeBasedSeniority(BaseModel):
     """Job seniority level. Please use the seniority levels endpoint to retrieve the list of seniority levels.
 
-    :param id_: id_, defaults to None
-    :type id_: IdentifierValue, optional
+    :param id_: Seniority ID., defaults to None
+    :type id_: SeniorityId4, optional
     """
 
-    def __init__(self, id_: IdentifierValue = None):
+    def __init__(self, id_: SeniorityId4 = None):
         if id_ is not None:
-            self.id_ = IdentifierValueGuard.return_one_of(id_)
+            self.id_ = SeniorityId4Guard.return_one_of(id_)
 
 
 @JsonMap({})
 class ContractToCreateOngoingTimeBasedWorker(BaseModel):
     """Worker properties
 
     :param expected_email: Worker's email address.
```

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_pay_as_you_go_time_based.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_to_create_pay_as_you_go_time_based.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # This file was generated by liblab | https://liblab.com/
 
 from __future__ import annotations
 from enum import Enum
+from typing import Union
 from .utils.json_map import JsonMap
 from .base import BaseModel
+from .base import OneOfBaseModel
 from .contract_who_reports_enum import ContractWhoReportsEnum
 from .meta_data_of_contract_to_create import MetaDataOfContractToCreate
 from .identifier_value import IdentifierValue, IdentifierValueGuard
 from .work_statement_cycle_scale_enum import WorkStatementCycleScaleEnum
 from .work_statement_cycle_end_type_enum import WorkStatementCycleEndTypeEnum
 from .work_statement_payment_due_type_enum import WorkStatementPaymentDueTypeEnum
 from .work_statement_scale_enum import WorkStatementScaleEnum
 
 
 @JsonMap({"id_": "id"})
-class ClientLegalEntity4(BaseModel):
+class ClientLegalEntity5(BaseModel):
     """Choose the Deel legal entity for this contract. Use legal entity endpoint to retrieve a list of legal entities in your organization.
 
     :param id_: id_
     :type id_: IdentifierValue
     """
 
     def __init__(self, id_: IdentifierValue):
@@ -38,52 +40,59 @@
 
 
 @JsonMap({})
 class ContractToCreatePayAsYouGoTimeBasedClient(BaseModel):
     """ContractToCreatePayAsYouGoTimeBasedClient
 
     :param legal_entity: Choose the Deel legal entity for this contract. Use legal entity endpoint to retrieve a list of legal entities in your organization.
-    :type legal_entity: ClientLegalEntity4
+    :type legal_entity: ClientLegalEntity5
     :param team: Choose the Deel team for this contract. Use teams endpoint to retrieve a list of teams in your organization.
     :type team: ClientTeam2
     """
 
-    def __init__(self, legal_entity: ClientLegalEntity4, team: ClientTeam2):
-        self.legal_entity = self._define_object(legal_entity, ClientLegalEntity4)
+    def __init__(self, legal_entity: ClientLegalEntity5, team: ClientTeam2):
+        self.legal_entity = self._define_object(legal_entity, ClientLegalEntity5)
         self.team = self._define_object(team, ClientTeam2)
 
 
 @JsonMap({"id_": "id"})
 class ContractToCreatePayAsYouGoTimeBasedJobTitle(BaseModel):
     """Worker's job title. You can enter a custom job title or use a pre-defiled job title using the Id retrieved in job-titles endpoint.
 
-    :param id_: Unique identifier of this resource., defaults to None
+    :param id_: Job title ID., defaults to None
     :type id_: str, optional
     :param name: Job title. Please leave it blank when entering an Id., defaults to None
     :type name: str, optional
     """
 
     def __init__(self, id_: str = None, name: str = None):
         if id_ is not None:
             self.id_ = id_
         if name is not None:
             self.name = name
 
 
+class SeniorityId1Guard(OneOfBaseModel):
+    class_list = {"float": float, "str": str}
+
+
+SeniorityId1 = Union[float, str]
+
+
 @JsonMap({"id_": "id"})
 class ContractToCreatePayAsYouGoTimeBasedSeniority(BaseModel):
     """Job seniority level. Please use the seniority levels endpoint to retrieve the list of seniority levels.
 
-    :param id_: id_, defaults to None
-    :type id_: IdentifierValue, optional
+    :param id_: Seniority ID., defaults to None
+    :type id_: SeniorityId1, optional
     """
 
-    def __init__(self, id_: IdentifierValue = None):
+    def __init__(self, id_: SeniorityId1 = None):
         if id_ is not None:
-            self.id_ = IdentifierValueGuard.return_one_of(id_)
+            self.id_ = SeniorityId1Guard.return_one_of(id_)
 
 
 @JsonMap({})
 class ContractToCreatePayAsYouGoTimeBasedWorker(BaseModel):
     """Worker properties
 
     :param expected_email: Worker's email address.
```

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_payg_milestones.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_to_create_payg_milestones.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # This file was generated by liblab | https://liblab.com/
 
 from __future__ import annotations
 from enum import Enum
+from typing import Union
 from .utils.json_map import JsonMap
 from .base import BaseModel
+from .base import OneOfBaseModel
 from .contract_who_reports_enum import ContractWhoReportsEnum
 from .meta_data_of_contract_to_create import MetaDataOfContractToCreate
 from .compensation_details_of_contract_to_create_shared import (
     CompensationDetailsOfContractToCreateShared,
 )
 from .identifier_value import IdentifierValue, IdentifierValueGuard
 
@@ -51,38 +53,45 @@
         self.team = self._define_object(team, ClientTeam4)
 
 
 @JsonMap({"id_": "id"})
 class ContractToCreatePaygMilestonesJobTitle(BaseModel):
     """Worker's job title. You can enter a custom job title or use a pre-defiled job title using the Id retrieved in job-titles endpoint.
 
-    :param id_: Unique identifier of this resource., defaults to None
+    :param id_: Job title ID., defaults to None
     :type id_: str, optional
     :param name: Job title. Please leave it blank when entering an Id., defaults to None
     :type name: str, optional
     """
 
     def __init__(self, id_: str = None, name: str = None):
         if id_ is not None:
             self.id_ = id_
         if name is not None:
             self.name = name
 
 
+class SeniorityId3Guard(OneOfBaseModel):
+    class_list = {"float": float, "str": str}
+
+
+SeniorityId3 = Union[float, str]
+
+
 @JsonMap({"id_": "id"})
 class ContractToCreatePaygMilestonesSeniority(BaseModel):
     """Job seniority level. Please use the seniority levels endpoint to retrieve the list of seniority levels.
 
-    :param id_: id_, defaults to None
-    :type id_: IdentifierValue, optional
+    :param id_: Seniority ID., defaults to None
+    :type id_: SeniorityId3, optional
     """
 
-    def __init__(self, id_: IdentifierValue = None):
+    def __init__(self, id_: SeniorityId3 = None):
         if id_ is not None:
-            self.id_ = IdentifierValueGuard.return_one_of(id_)
+            self.id_ = SeniorityId3Guard.return_one_of(id_)
 
 
 @JsonMap({})
 class ContractToCreatePaygMilestonesWorker(BaseModel):
     """Worker properties
 
     :param expected_email: Worker's email address.
```

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_payg_tasks.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_to_create_payg_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # This file was generated by liblab | https://liblab.com/
 
 from __future__ import annotations
 from enum import Enum
+from typing import Union
 from .utils.json_map import JsonMap
 from .base import BaseModel
+from .base import OneOfBaseModel
 from .contract_who_reports_enum import ContractWhoReportsEnum
 from .meta_data_of_contract_to_create import MetaDataOfContractToCreate
 from .compensation_details_of_contract_to_create_shared import (
     CompensationDetailsOfContractToCreateShared,
 )
 from .identifier_value import IdentifierValue, IdentifierValueGuard
 
@@ -51,38 +53,45 @@
         self.team = self._define_object(team, ClientTeam3)
 
 
 @JsonMap({"id_": "id"})
 class ContractToCreatePaygTasksJobTitle(BaseModel):
     """Worker's job title. You can enter a custom job title or use a pre-defiled job title using the Id retrieved in job-titles endpoint.
 
-    :param id_: Unique identifier of this resource., defaults to None
+    :param id_: Job title ID., defaults to None
     :type id_: str, optional
     :param name: Job title. Please leave it blank when entering an Id., defaults to None
     :type name: str, optional
     """
 
     def __init__(self, id_: str = None, name: str = None):
         if id_ is not None:
             self.id_ = id_
         if name is not None:
             self.name = name
 
 
+class SeniorityId2Guard(OneOfBaseModel):
+    class_list = {"float": float, "str": str}
+
+
+SeniorityId2 = Union[float, str]
+
+
 @JsonMap({"id_": "id"})
 class ContractToCreatePaygTasksSeniority(BaseModel):
     """Job seniority level. Please use the seniority levels endpoint to retrieve the list of seniority levels.
 
-    :param id_: id_, defaults to None
-    :type id_: IdentifierValue, optional
+    :param id_: Seniority ID., defaults to None
+    :type id_: SeniorityId2, optional
     """
 
-    def __init__(self, id_: IdentifierValue = None):
+    def __init__(self, id_: SeniorityId2 = None):
         if id_ is not None:
-            self.id_ = IdentifierValueGuard.return_one_of(id_)
+            self.id_ = SeniorityId2Guard.return_one_of(id_)
 
 
 @JsonMap({})
 class ContractToCreatePaygTasksWorker(BaseModel):
     """Worker properties
 
     :param expected_email: Worker's email address.
```

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_terminate.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_to_terminate.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_type_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_type_enum_for_estimate.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_type_enum_for_estimate.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contract_who_reports_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contract_who_reports_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contracts_sort_by_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contracts_sort_by_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/contribution.py` & `deel_sdk-1.0.4/src/deel_sdk/models/contribution.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/cost_quote.py` & `deel_sdk-1.0.4/src/deel_sdk/models/cost_quote.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/country.py` & `deel_sdk-1.0.4/src/deel_sdk/models/country.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/create_people_timeoff.py` & `deel_sdk-1.0.4/src/deel_sdk/models/create_people_timeoff.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/create_timeoff.py` & `deel_sdk-1.0.4/src/deel_sdk/models/create_timeoff.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/create_webhook_request.py` & `deel_sdk-1.0.4/src/deel_sdk/models/create_webhook_request.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/deel_invoice.py` & `deel_sdk-1.0.4/src/deel_sdk/models/deel_invoice.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/deel_invoice_list_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/deel_invoice_list_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/departments.py` & `deel_sdk-1.0.4/src/deel_sdk/models/departments.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/download_worker_documents_by_id_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/download_worker_documents_by_id_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/email.py` & `deel_sdk-1.0.4/src/deel_sdk/models/email.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/employee.py` & `deel_sdk-1.0.4/src/deel_sdk/models/employee.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/employee_agreement_download_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/employee_agreement_download_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/employee_agreement_download_object.py` & `deel_sdk-1.0.4/src/deel_sdk/models/employee_agreement_download_object.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/employee_contract_signature_to_create_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/employee_contract_signature_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/employee_payslips_list.py` & `deel_sdk-1.0.4/src/deel_sdk/models/employee_payslips_list.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/employee_payslips_list_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/employee_payslips_list_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/employee_tax_documents_list.py` & `deel_sdk-1.0.4/src/deel_sdk/models/employee_tax_documents_list.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/employee_tax_documents_list_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/employee_tax_documents_list_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/employee_timeoffs_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_creation_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/employee_timeoffs_creation_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_entitlements_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/employee_timeoffs_entitlements_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_entitlements_item.py` & `deel_sdk-1.0.4/src/deel_sdk/models/employee_timeoffs_entitlements_item.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_item.py` & `deel_sdk-1.0.4/src/deel_sdk/models/employee_timeoffs_item.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_item_response.py` & `deel_sdk-1.0.4/src/deel_sdk/models/employee_timeoffs_item_response.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_policies_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/employee_timeoffs_policies_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_policies_item.py` & `deel_sdk-1.0.4/src/deel_sdk/models/employee_timeoffs_policies_item.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/employment.py` & `deel_sdk-1.0.4/src/deel_sdk/models/employment.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/employment_detail.py` & `deel_sdk-1.0.4/src/deel_sdk/models/employment_detail.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/employment_details_of_contract.py` & `deel_sdk-1.0.4/src/deel_sdk/models/employment_details_of_contract.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/eor_client_timeoff_requests.py` & `deel_sdk-1.0.4/src/deel_sdk/models/eor_client_timeoff_requests.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/eor_client_timeoffs.py` & `deel_sdk-1.0.4/src/deel_sdk/models/eor_client_timeoffs.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/eor_contract_benefits.py` & `deel_sdk-1.0.4/src/deel_sdk/models/eor_contract_benefits.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/eor_contract_benefits_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/eor_contract_benefits_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/eor_contract_created.py` & `deel_sdk-1.0.4/src/deel_sdk/models/eor_contract_created.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,16 +61,16 @@
         if probation_period is not None:
             self.probation_period = probation_period
         if calculated_holidays is not None:
             self.calculated_holidays = calculated_holidays
 
 
 @JsonMap({})
-class ClientLegalEntity2(BaseModel):
-    """ClientLegalEntity2
+class ClientLegalEntity3(BaseModel):
+    """ClientLegalEntity3
 
     :param name: Legal entity name., defaults to None
     :type name: str, optional
     """
 
     def __init__(self, name: str = None):
         if name is not None:
@@ -78,20 +78,20 @@
 
 
 @JsonMap({})
 class EorContractCreatedClient(BaseModel):
     """EorContractCreatedClient
 
     :param legal_entity: legal_entity, defaults to None
-    :type legal_entity: ClientLegalEntity2, optional
+    :type legal_entity: ClientLegalEntity3, optional
     """
 
-    def __init__(self, legal_entity: ClientLegalEntity2 = None):
+    def __init__(self, legal_entity: ClientLegalEntity3 = None):
         if legal_entity is not None:
-            self.legal_entity = self._define_object(legal_entity, ClientLegalEntity2)
+            self.legal_entity = self._define_object(legal_entity, ClientLegalEntity3)
 
 
 @JsonMap({})
 class EorContractCreatedCompensationDetails(BaseModel):
     """EorContractCreatedCompensationDetails
 
     :param salary: Gross annual salary., defaults to None
```

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/eor_contract_to_create.py` & `deel_sdk-1.0.4/src/deel_sdk/models/eor_contract_to_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,16 +189,16 @@
 
     def __init__(self, id_: IdentifierValue = None):
         if id_ is not None:
             self.id_ = IdentifierValueGuard.return_one_of(id_)
 
 
 @JsonMap({"id_": "id"})
-class ClientLegalEntity1(BaseModel):
-    """ClientLegalEntity1
+class ClientLegalEntity2(BaseModel):
+    """ClientLegalEntity2
 
     :param id_: id_, defaults to None
     :type id_: IdentifierValue, optional
     """
 
     def __init__(self, id_: IdentifierValue = None):
         if id_ is not None:
@@ -218,22 +218,22 @@
 
 
 @JsonMap({})
 class EorContractToCreateClient(BaseModel):
     """EorContractToCreateClient
 
     :param legal_entity: legal_entity, defaults to None
-    :type legal_entity: ClientLegalEntity1, optional
+    :type legal_entity: ClientLegalEntity2, optional
     :param team: team
     :type team: ClientTeam1
     """
 
-    def __init__(self, team: ClientTeam1, legal_entity: ClientLegalEntity1 = None):
+    def __init__(self, team: ClientTeam1, legal_entity: ClientLegalEntity2 = None):
         if legal_entity is not None:
-            self.legal_entity = self._define_object(legal_entity, ClientLegalEntity1)
+            self.legal_entity = self._define_object(legal_entity, ClientLegalEntity2)
         self.team = self._define_object(team, ClientTeam1)
 
 
 class VariableCompensationType(Enum):
     """An enumeration representing different categories.
 
     :cvar PERCENTAGE: "PERCENTAGE"
```

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/eor_country_validations.py` & `deel_sdk-1.0.4/src/deel_sdk/models/eor_country_validations.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/eor_employee_cost_calculation_request_body.py` & `deel_sdk-1.0.4/src/deel_sdk/models/eor_employee_cost_calculation_request_body.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/eor_employee_cost_calculation_request_body_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/eor_employee_cost_calculation_request_body_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/eor_employee_cost_calculation_response_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/eor_employee_cost_calculation_response_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/eor_entitlement_list_item.py` & `deel_sdk-1.0.4/src/deel_sdk/models/eor_entitlement_list_item.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/eor_entitlements.py` & `deel_sdk-1.0.4/src/deel_sdk/models/eor_entitlements.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/eor_field.py` & `deel_sdk-1.0.4/src/deel_sdk/models/eor_field.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/eor_holidays_rollover_type.py` & `deel_sdk-1.0.4/src/deel_sdk/models/eor_holidays_rollover_type.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/eor_quote_base.py` & `deel_sdk-1.0.4/src/deel_sdk/models/eor_quote_base.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/eor_timeoffs_base_item.py` & `deel_sdk-1.0.4/src/deel_sdk/models/eor_timeoffs_base_item.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/eor_timeoffs_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/eor_timeoffs_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/eor_timeoffs_employee_item.py` & `deel_sdk-1.0.4/src/deel_sdk/models/eor_timeoffs_employee_item.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/equity_stakeholder.py` & `deel_sdk-1.0.4/src/deel_sdk/models/equity_stakeholder.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/equity_stakeholders_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/equity_stakeholders_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/estimate_first_payment.py` & `deel_sdk-1.0.4/src/deel_sdk/models/estimate_first_payment.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/estimate_first_payment_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/estimate_first_payment_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/file_attachment_info.py` & `deel_sdk-1.0.4/src/deel_sdk/models/file_attachment_info.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/file_ref_type_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/file_ref_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/final_payment_calculated.py` & `deel_sdk-1.0.4/src/deel_sdk/models/final_payment_calculated.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/final_payment_calculated_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/final_payment_calculated_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/generic_result_created.py` & `deel_sdk-1.0.4/src/deel_sdk/models/generic_result_created.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/generic_result_created_with_id.py` & `deel_sdk-1.0.4/src/deel_sdk/models/generic_result_created_with_id.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/generic_result_deleted.py` & `deel_sdk-1.0.4/src/deel_sdk/models/generic_result_deleted.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/generic_result_updated.py` & `deel_sdk-1.0.4/src/deel_sdk/models/generic_result_updated.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/get_employee_compliance_document_template_download_link_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/get_employee_compliance_document_template_download_link_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/get_employee_compliance_documents_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/get_employee_compliance_documents_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/global_payroll_g2_n_report.py` & `deel_sdk-1.0.4/src/deel_sdk/models/global_payroll_g2_n_report.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/global_payroll_g2_n_report_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/global_payroll_g2_n_report_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_client.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_client.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_created.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_contract_created.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,16 +67,16 @@
         if work_visa_required is not None:
             self.work_visa_required = work_visa_required
         if holidays is not None:
             self.holidays = self._define_object(holidays, EmploymentHolidays2)
 
 
 @JsonMap({})
-class ClientLegalEntity3(BaseModel):
-    """ClientLegalEntity3
+class ClientLegalEntity4(BaseModel):
+    """ClientLegalEntity4
 
     :param name: Legal entity name., defaults to None
     :type name: str, optional
     """
 
     def __init__(self, name: str = None):
         if name is not None:
@@ -84,20 +84,20 @@
 
 
 @JsonMap({})
 class GpContractCreatedClient(BaseModel):
     """GpContractCreatedClient
 
     :param legal_entity: legal_entity, defaults to None
-    :type legal_entity: ClientLegalEntity3, optional
+    :type legal_entity: ClientLegalEntity4, optional
     """
 
-    def __init__(self, legal_entity: ClientLegalEntity3 = None):
+    def __init__(self, legal_entity: ClientLegalEntity4 = None):
         if legal_entity is not None:
-            self.legal_entity = self._define_object(legal_entity, ClientLegalEntity3)
+            self.legal_entity = self._define_object(legal_entity, ClientLegalEntity4)
 
 
 @JsonMap({})
 class GpContractCreatedCompensationDetails(BaseModel):
     """GpContractCreatedCompensationDetails
 
     :param salary: Gross annual/month salary., defaults to None
```

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_salary_scale_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_contract_salary_scale_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_salary_status_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_contract_salary_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_status_type_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_contract_status_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_to_create.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_contract_to_create.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_address_to_update_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_address_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_address_update_data.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_address_update_data.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_address_updated.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_address_updated.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_address_updated_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_address_updated_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_compensation_to_update_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_compensation_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_compensation_update_data.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_compensation_update_data.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_compensation_updated.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_compensation_updated.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_compensation_updated_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_compensation_updated_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_information_to_update_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_information_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_information_update_data.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_information_update_data.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_information_updated_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_information_updated_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_pto_to_update_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_pto_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_pto_update_data.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_employee_pto_update_data.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_payroll_event_report_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_payroll_event_report_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/gp_payroll_event_reports.py` & `deel_sdk-1.0.4/src/deel_sdk/models/gp_payroll_event_reports.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/health_insurance_provider.py` & `deel_sdk-1.0.4/src/deel_sdk/models/health_insurance_provider.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/hiring_status_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/hiring_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/hr_verification_letters_and_documents_list_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/hr_verification_letters_and_documents_list_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/hris_contract_full_time.py` & `deel_sdk-1.0.4/src/deel_sdk/models/hris_contract_full_time.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/hris_contract_part_time.py` & `deel_sdk-1.0.4/src/deel_sdk/models/hris_contract_part_time.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/hris_direct_employee.py` & `deel_sdk-1.0.4/src/deel_sdk/models/hris_direct_employee.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/hris_direct_employee_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/hris_direct_employee_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/hris_direct_employee_details.py` & `deel_sdk-1.0.4/src/deel_sdk/models/hris_direct_employee_details.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/hris_direct_employee_response.py` & `deel_sdk-1.0.4/src/deel_sdk/models/hris_direct_employee_response.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/hris_job_information_title_name.py` & `deel_sdk-1.0.4/src/deel_sdk/models/hris_job_information_title_name.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/input_to_create_file_ref.py` & `deel_sdk-1.0.4/src/deel_sdk/models/input_to_create_file_ref.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/input_to_patch_contract_external_id.py` & `deel_sdk-1.0.4/src/deel_sdk/models/input_to_patch_contract_external_id.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/internal_people.py` & `deel_sdk-1.0.4/src/deel_sdk/models/internal_people.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/invitations_of_basic_contract.py` & `deel_sdk-1.0.4/src/deel_sdk/models/invitations_of_basic_contract.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/invoice.py` & `deel_sdk-1.0.4/src/deel_sdk/models/invoice.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     :type is_overdue: bool
     :param issued_at: Long date-time format following ISO-8601
     :type issued_at: str
     :param vat_id: VAT identification number.
     :type vat_id: str
     :param due_date: Long date-time format following ISO-8601
     :type due_date: str
-    :param contract_id: Unique identifier of the contract.
+    :param contract_id: Unique identifier of the contract. #magic___^_^___line
     :type contract_id: str
     """
 
     def __init__(
         self,
         id_: str,
         status: InvoiceStatusEnum,
```

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_created.py` & `deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_created.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_created_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_created_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_list_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_list_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_review_to_create.py` & `deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_review_to_create.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_review_to_create_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_review_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_reviews_to_create.py` & `deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_reviews_to_create.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_reviews_to_create_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_reviews_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_status_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_to_create.py` & `deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_to_create.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_to_create_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_to_create_with_file.py` & `deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_to_create_with_file.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_to_update.py` & `deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_to_update.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_to_update_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_type_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_type_to_create_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/invoice_adjustment_type_to_create_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/invoice_list_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/invoice_list_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/invoice_status_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/invoice_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/job_title.py` & `deel_sdk-1.0.4/src/deel_sdk/models/job_title.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/job_title_list_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/job_title_list_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/legal_entity_list_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/legal_entity_list_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/legal_entity_type.py` & `deel_sdk-1.0.4/src/deel_sdk/models/legal_entity_type.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/letter_request.py` & `deel_sdk-1.0.4/src/deel_sdk/models/letter_request.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/marital_status_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/marital_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/meta_data_of_contract_to_create.py` & `deel_sdk-1.0.4/src/deel_sdk/models/meta_data_of_contract_to_create.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/milestone.py` & `deel_sdk-1.0.4/src/deel_sdk/models/milestone.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/milestone_properties.py` & `deel_sdk-1.0.4/src/deel_sdk/models/milestone_properties.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/milestone_review_to_create.py` & `deel_sdk-1.0.4/src/deel_sdk/models/milestone_review_to_create.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/milestone_review_to_create_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/milestone_review_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/milestone_reviews_to_create.py` & `deel_sdk-1.0.4/src/deel_sdk/models/timesheet_reviews_to_create.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # This file was generated by liblab | https://liblab.com/
 
+from __future__ import annotations
 from enum import Enum
 from typing import List
 from .utils.json_map import JsonMap
 from .base import BaseModel
+from .timesheet_id_items import TimesheetIdItems, TimesheetIdItemsGuard
 
 
-class MilestoneReviewsToCreateStatus(Enum):
+class TimesheetReviewsToCreateStatus(Enum):
     """An enumeration representing different categories.
 
     :cvar APPROVED: "approved"
     :vartype APPROVED: str
     :cvar DECLINED: "declined"
     :vartype DECLINED: str
     """
@@ -21,35 +23,35 @@
     def list():
         """Lists all category values.
 
         :return: A list of all category values.
         :rtype: list
         """
         return list(
-            map(lambda x: x.value, MilestoneReviewsToCreateStatus._member_map_.values())
+            map(lambda x: x.value, TimesheetReviewsToCreateStatus._member_map_.values())
         )
 
 
 @JsonMap({})
-class MilestoneReviewsToCreate(BaseModel):
-    """MilestoneReviewsToCreate
+class TimesheetReviewsToCreate(BaseModel):
+    """TimesheetReviewsToCreate
 
     :param status: status
-    :type status: MilestoneReviewsToCreateStatus
+    :type status: TimesheetReviewsToCreateStatus
     :param reason: reason, defaults to None
     :type reason: str, optional
     :param ids: ids
-    :type ids: List[float]
+    :type ids: List[TimesheetIdItems]
     """
 
     def __init__(
         self,
-        status: MilestoneReviewsToCreateStatus,
-        ids: List[float],
+        status: TimesheetReviewsToCreateStatus,
+        ids: List[TimesheetIdItems],
         reason: str = None,
     ):
         self.status = self._enum_matching(
-            status, MilestoneReviewsToCreateStatus.list(), "status"
+            status, TimesheetReviewsToCreateStatus.list(), "status"
         )
         if reason is not None:
             self.reason = reason
-        self.ids = ids
+        self.ids = self._define_list(ids, TimesheetIdItems)
```

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/milestone_reviews_to_create_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/milestone_reviews_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/milestone_to_create_form_with_file.py` & `deel_sdk-1.0.4/src/deel_sdk/models/milestone_to_create_form_with_file.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/off_cycle_payment.py` & `deel_sdk-1.0.4/src/deel_sdk/models/off_cycle_payment.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/off_cycle_payment_to_create.py` & `deel_sdk-1.0.4/src/deel_sdk/models/off_cycle_payment_to_create.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/off_cycle_payment_to_create_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/off_cycle_payment_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/organization_list_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/organization_list_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/output_to_create_file_ref_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/output_to_create_file_ref_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/page_info_without_cursor_new.py` & `deel_sdk-1.0.4/src/deel_sdk/models/page_info_without_cursor_new.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/patch_webhook_request.py` & `deel_sdk-1.0.4/src/deel_sdk/models/patch_webhook_request.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/payment.py` & `deel_sdk-1.0.4/src/deel_sdk/models/payment.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/payment_break_down.py` & `deel_sdk-1.0.4/src/deel_sdk/models/payment_break_down.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/payment_method.py` & `deel_sdk-1.0.4/src/deel_sdk/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/payment_method_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/payment_method_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/payment_object.py` & `deel_sdk-1.0.4/src/deel_sdk/models/payment_object.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/payment_status_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/payment_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/payment_worker.py` & `deel_sdk-1.0.4/src/deel_sdk/models/payment_worker.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/payroll_adjustment.py` & `deel_sdk-1.0.4/src/deel_sdk/models/payroll_adjustment.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/payslips.py` & `deel_sdk-1.0.4/src/deel_sdk/models/payslips.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/pension_eor_contract_to_create.py` & `deel_sdk-1.0.4/src/deel_sdk/models/pension_eor_contract_to_create.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/pension_provider.py` & `deel_sdk-1.0.4/src/deel_sdk/models/pension_provider.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/people_by_id_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/people_by_id_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/people_client_legal_entity.py` & `deel_sdk-1.0.4/src/deel_sdk/models/people_client_legal_entity.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/people_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/people_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/people_custom_field.py` & `deel_sdk-1.0.4/src/deel_sdk/models/people_custom_field.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/people_me.py` & `deel_sdk-1.0.4/src/deel_sdk/models/people_me.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/people_payment.py` & `deel_sdk-1.0.4/src/deel_sdk/models/people_payment.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/people_sort_by_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/people_sort_by_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/people_time_off_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/people_time_off_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/pgo_task.py` & `deel_sdk-1.0.4/src/deel_sdk/models/pgo_task.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/pgo_task_reviews_by_id_to_create.py` & `deel_sdk-1.0.4/src/deel_sdk/models/pgo_task_reviews_by_id_to_create.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/pgo_task_reviews_to_create.py` & `deel_sdk-1.0.4/src/deel_sdk/models/pgo_task_reviews_to_create.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/pgo_task_to_create.py` & `deel_sdk-1.0.4/src/deel_sdk/models/pgo_task_to_create.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/premium_result_added.py` & `deel_sdk-1.0.4/src/deel_sdk/models/premium_result_added.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/premium_to_add.py` & `deel_sdk-1.0.4/src/deel_sdk/models/premium_to_add.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/pro_rata.py` & `deel_sdk-1.0.4/src/deel_sdk/models/pro_rata.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/profile_type_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/profile_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_by_id_reviews_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_by_id_reviews_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_reviews_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_reviews_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/request_custom_verification_letter_with_file.py` & `deel_sdk-1.0.4/src/deel_sdk/models/request_custom_verification_letter_with_file.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/requester_time_off.py` & `deel_sdk-1.0.4/src/deel_sdk/models/requester_time_off.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/response_estimate_first_payment.py` & `deel_sdk-1.0.4/src/deel_sdk/models/response_estimate_first_payment.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/response_estimate_first_payment_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/response_estimate_first_payment_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/salary_frequency_scale_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/salary_frequency_scale_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/seniority.py` & `deel_sdk-1.0.4/src/deel_sdk/models/seniority.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/seniority_required.py` & `deel_sdk-1.0.4/src/deel_sdk/models/seniority_required.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/signatures_of_basic_contract.py` & `deel_sdk-1.0.4/src/deel_sdk/models/signatures_of_basic_contract.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/signatures_of_contract.py` & `deel_sdk-1.0.4/src/deel_sdk/models/signatures_of_contract.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/sort_dir_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/sort_dir_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/task_created.py` & `deel_sdk-1.0.4/src/deel_sdk/models/task_created.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/team.py` & `deel_sdk-1.0.4/src/deel_sdk/models/team.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/team_of_basic_contract.py` & `deel_sdk-1.0.4/src/deel_sdk/models/team_of_basic_contract.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/team_of_contract.py` & `deel_sdk-1.0.4/src/deel_sdk/models/team_of_contract.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/timeoff_review.py` & `deel_sdk-1.0.4/src/deel_sdk/models/timeoff_review.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/timeoff_review_internal.py` & `deel_sdk-1.0.4/src/deel_sdk/models/timeoff_review_internal.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/timeoff_to_review_internal_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/timeoff_to_review_internal_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/timeoffs_attachments_item.py` & `deel_sdk-1.0.4/src/deel_sdk/models/timeoffs_attachments_item.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/timeoffs_profile.py` & `deel_sdk-1.0.4/src/deel_sdk/models/timeoffs_profile.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/timeoffs_status_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/timeoffs_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/timeoffs_type_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/timeoffs_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/timesheet.py` & `deel_sdk-1.0.4/src/deel_sdk/models/timesheet.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_approver.py` & `deel_sdk-1.0.4/src/deel_sdk/models/timesheet_approver.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_list_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/timesheet_list_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_review_to_create.py` & `deel_sdk-1.0.4/src/deel_sdk/models/timesheet_review_to_create.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_review_to_create_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/timesheet_review_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_reviews_to_create_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/timesheet_reviews_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_shared_properties.py` & `deel_sdk-1.0.4/src/deel_sdk/models/timesheet_shared_properties.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_status_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/timesheet_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_to_create_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/timesheet_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_to_create_container_with_file.py` & `deel_sdk-1.0.4/src/deel_sdk/models/timesheet_to_create_container_with_file.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_to_update.py` & `deel_sdk-1.0.4/src/deel_sdk/models/timesheet_to_update.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_to_update_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/timesheet_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/update_worker_department.py` & `deel_sdk-1.0.4/src/deel_sdk/models/update_worker_department.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/update_worker_department_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/update_worker_department_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/update_worker_working_location.py` & `deel_sdk-1.0.4/src/deel_sdk/models/update_worker_working_location.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/update_worker_working_location_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/update_worker_working_location_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/upload_employee_compliance_document_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/upload_employee_compliance_document_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/utils/cast_models.py` & `deel_sdk-1.0.4/src/deel_sdk/models/utils/cast_models.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/utils/json_map.py` & `deel_sdk-1.0.4/src/deel_sdk/models/utils/json_map.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/validation_type.py` & `deel_sdk-1.0.4/src/deel_sdk/models/validation_type.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/validation_type_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/validation_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/webhook_event_type_list_response.py` & `deel_sdk-1.0.4/src/deel_sdk/models/webhook_event_type_list_response.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/webhook_event_type_response.py` & `deel_sdk-1.0.4/src/deel_sdk/models/webhook_event_type_response.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/webhook_item.py` & `deel_sdk-1.0.4/src/deel_sdk/models/webhook_item.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/week_days_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/week_days_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/work_statement_cycle_end_type_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/work_statement_cycle_end_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/work_statement_cycle_scale_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/work_statement_cycle_scale_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/work_statement_payment_due_type_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/work_statement_payment_due_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/work_statement_scale_enum.py` & `deel_sdk-1.0.4/src/deel_sdk/models/work_statement_scale_enum.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/worker_bank_account_info.py` & `deel_sdk-1.0.4/src/deel_sdk/models/worker_bank_account_info.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/worker_bank_account_to_add.py` & `deel_sdk-1.0.4/src/deel_sdk/models/worker_bank_account_to_add.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/worker_bank_accounts_info_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/worker_bank_accounts_info_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/worker_document.py` & `deel_sdk-1.0.4/src/deel_sdk/models/worker_document.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/worker_document_download_link.py` & `deel_sdk-1.0.4/src/deel_sdk/models/worker_document_download_link.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/worker_documents_by_id_container.py` & `deel_sdk-1.0.4/src/deel_sdk/models/worker_documents_by_id_container.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/worker_legal_entity.py` & `deel_sdk-1.0.4/src/deel_sdk/models/worker_legal_entity.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/worker_of_basic_contract.py` & `deel_sdk-1.0.4/src/deel_sdk/models/worker_of_basic_contract.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/worker_of_contract.py` & `deel_sdk-1.0.4/src/deel_sdk/models/worker_of_contract.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/worker_termination_body.py` & `deel_sdk-1.0.4/src/deel_sdk/models/worker_termination_body.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/models/working_locations.py` & `deel_sdk-1.0.4/src/deel_sdk/models/working_locations.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/net/headers/access_token_auth.py` & `deel_sdk-1.0.4/src/deel_sdk/net/headers/access_token_auth.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/net/request_chain/handlers/base_handler.py` & `deel_sdk-1.0.4/src/deel_sdk/net/request_chain/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/net/request_chain/handlers/hook_handler.py` & `deel_sdk-1.0.4/src/deel_sdk/net/request_chain/handlers/hook_handler.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/net/request_chain/handlers/http_handler.py` & `deel_sdk-1.0.4/src/deel_sdk/net/request_chain/handlers/http_handler.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/net/request_chain/handlers/retry_handler.py` & `deel_sdk-1.0.4/src/deel_sdk/net/request_chain/handlers/retry_handler.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/net/request_chain/request_chain.py` & `deel_sdk-1.0.4/src/deel_sdk/net/request_chain/request_chain.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/net/transport/request.py` & `deel_sdk-1.0.4/src/deel_sdk/net/transport/request.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/net/transport/request_error.py` & `deel_sdk-1.0.4/src/deel_sdk/net/transport/request_error.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/net/transport/response.py` & `deel_sdk-1.0.4/src/deel_sdk/net/transport/response.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/net/transport/serializer.py` & `deel_sdk-1.0.4/src/deel_sdk/net/transport/serializer.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/net/transport/utils.py` & `deel_sdk-1.0.4/src/deel_sdk/net/transport/utils.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/sdk.py` & `deel_sdk-1.0.4/src/deel_sdk/sdk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # This file was generated by liblab | https://liblab.com/
 
 from .services.accounting import AccountingService
+from .services.custom_fields import CustomFieldsService
+from .services.hris_organizations import HrisOrganizationsService
+from .services.contracts import ContractsService
+from .services.organization_structure import OrganizationStructureService
+from .services.positions import PositionsService
 from .services.managers import ManagersService
 from .services.people import PeopleService
 from .services.eor import EorService
 from .services.global_payroll import GlobalPayrollService
 from .services.contractors import ContractorsService
 from .services.adjustments import AdjustmentsService
 from .services.candidates import CandidatesService
 from .services.partner_managed import PartnerManagedService
-from .services.contracts import ContractsService
 from .services.tasks import TasksService
 from .services.timesheets import TimesheetsService
 from .services.milestones import MilestonesService
 from .services.off_cycle_payments import OffCyclePaymentsService
 from .services.time_off import TimeOffService
 from .services.invoices import InvoicesService
 from .services.organizations import OrganizationsService
@@ -28,23 +32,27 @@
     def __init__(
         self, access_token: str = None, base_url: str = Environment.DEFAULT.value
     ):
         """
         Initializes DeelSdk the SDK class.
         """
         self.accounting = AccountingService(base_url=base_url)
+        self.custom_fields = CustomFieldsService(base_url=base_url)
+        self.hris_organizations = HrisOrganizationsService(base_url=base_url)
+        self.contracts = ContractsService(base_url=base_url)
+        self.organization_structure = OrganizationStructureService(base_url=base_url)
+        self.positions = PositionsService(base_url=base_url)
         self.managers = ManagersService(base_url=base_url)
         self.people = PeopleService(base_url=base_url)
         self.eor = EorService(base_url=base_url)
         self.global_payroll = GlobalPayrollService(base_url=base_url)
         self.contractors = ContractorsService(base_url=base_url)
         self.adjustments = AdjustmentsService(base_url=base_url)
         self.candidates = CandidatesService(base_url=base_url)
         self.partner_managed = PartnerManagedService(base_url=base_url)
-        self.contracts = ContractsService(base_url=base_url)
         self.tasks = TasksService(base_url=base_url)
         self.timesheets = TimesheetsService(base_url=base_url)
         self.milestones = MilestonesService(base_url=base_url)
         self.off_cycle_payments = OffCyclePaymentsService(base_url=base_url)
         self.time_off = TimeOffService(base_url=base_url)
         self.invoices = InvoicesService(base_url=base_url)
         self.organizations = OrganizationsService(base_url=base_url)
@@ -55,23 +63,27 @@
         self.set_access_token(access_token)
 
     def set_base_url(self, base_url):
         """
         Sets the base URL for the entire SDK.
         """
         self.accounting.set_base_url(base_url)
+        self.custom_fields.set_base_url(base_url)
+        self.hris_organizations.set_base_url(base_url)
+        self.contracts.set_base_url(base_url)
+        self.organization_structure.set_base_url(base_url)
+        self.positions.set_base_url(base_url)
         self.managers.set_base_url(base_url)
         self.people.set_base_url(base_url)
         self.eor.set_base_url(base_url)
         self.global_payroll.set_base_url(base_url)
         self.contractors.set_base_url(base_url)
         self.adjustments.set_base_url(base_url)
         self.candidates.set_base_url(base_url)
         self.partner_managed.set_base_url(base_url)
-        self.contracts.set_base_url(base_url)
         self.tasks.set_base_url(base_url)
         self.timesheets.set_base_url(base_url)
         self.milestones.set_base_url(base_url)
         self.off_cycle_payments.set_base_url(base_url)
         self.time_off.set_base_url(base_url)
         self.invoices.set_base_url(base_url)
         self.organizations.set_base_url(base_url)
@@ -83,23 +95,27 @@
         return self
 
     def set_access_token(self, access_token: str):
         """
         Sets the access token for the entire SDK.
         """
         self.accounting.set_access_token(access_token)
+        self.custom_fields.set_access_token(access_token)
+        self.hris_organizations.set_access_token(access_token)
+        self.contracts.set_access_token(access_token)
+        self.organization_structure.set_access_token(access_token)
+        self.positions.set_access_token(access_token)
         self.managers.set_access_token(access_token)
         self.people.set_access_token(access_token)
         self.eor.set_access_token(access_token)
         self.global_payroll.set_access_token(access_token)
         self.contractors.set_access_token(access_token)
         self.adjustments.set_access_token(access_token)
         self.candidates.set_access_token(access_token)
         self.partner_managed.set_access_token(access_token)
-        self.contracts.set_access_token(access_token)
         self.tasks.set_access_token(access_token)
         self.timesheets.set_access_token(access_token)
         self.milestones.set_access_token(access_token)
         self.off_cycle_payments.set_access_token(access_token)
         self.time_off.set_access_token(access_token)
         self.invoices.set_access_token(access_token)
         self.organizations.set_access_token(access_token)
```

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/accounting.py` & `deel_sdk-1.0.4/src/deel_sdk/services/accounting.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/adjustments.py` & `deel_sdk-1.0.4/src/deel_sdk/services/adjustments.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/candidates.py` & `deel_sdk-1.0.4/src/deel_sdk/services/candidates.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/carta.py` & `deel_sdk-1.0.4/src/deel_sdk/services/carta.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/contractors.py` & `deel_sdk-1.0.4/src/deel_sdk/services/contractors.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/contracts.py` & `deel_sdk-1.0.4/src/deel_sdk/services/contracts.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,29 +2,33 @@
 
 from typing import List
 from .utils.validator import Validator
 from .utils.base_service import BaseService
 from ..net.transport.serializer import Serializer
 from ..models.worker_documents_by_id_container import WorkerDocumentsByIdContainer
 from ..models.utils.cast_models import cast_models
+from ..models.updated_exercise_equity_container import UpdatedExerciseEquityContainer
 from ..models.sort_dir_enum import SortDirEnum
 from ..models.response_estimate_first_payment_container import (
     ResponseEstimateFirstPaymentContainer,
 )
 from ..models.input_to_patch_contract_external_id import InputToPatchContractExternalId
 from ..models.get_contract_list_currencies import GetContractListCurrencies
 from ..models.generic_result_updated import GenericResultUpdated
 from ..models.generic_result_deleted import GenericResultDeleted
 from ..models.generic_result_created import GenericResultCreated
 from ..models.final_payment_calculated_container import FinalPaymentCalculatedContainer
 from ..models.file_object import FileObject
+from ..models.exercise_equity_to_update_container import ExerciseEquityToUpdateContainer
+from ..models.exercise_equity_to_create_container import ExerciseEquityToCreateContainer
 from ..models.estimate_first_payment_container import EstimateFirstPaymentContainer
 from ..models.download_worker_documents_by_id_container import (
     DownloadWorkerDocumentsByIdContainer,
 )
+from ..models.created_exercise_equity_container import CreatedExerciseEquityContainer
 from ..models.contracts_sort_by_enum import ContractsSortByEnum
 from ..models.contract_type_enum import ContractTypeEnum
 from ..models.contract_template_list_container import ContractTemplateListContainer
 from ..models.contract_status_enum import ContractStatusEnum
 from ..models.contract_signature_to_create_container import (
     ContractSignatureToCreateContainer,
 )
@@ -39,14 +43,77 @@
 )
 from ..models.alternate_email_item import AlternateEmailItem
 
 
 class ContractsService(BaseService):
 
     @cast_models
+    def request_exercise_equity(
+        self, request_body: ExerciseEquityToCreateContainer
+    ) -> CreatedExerciseEquityContainer:
+        """Create a request to exercise equity.
+
+        :param request_body: The request body.
+        :type request_body: ExerciseEquityToCreateContainer
+        ...
+        :raises RequestError: Raised when a request fails, with optional HTTP status code and details.
+        ...
+        :return: Successful operation.
+        :rtype: CreatedExerciseEquityContainer
+        """
+
+        Validator(ExerciseEquityToCreateContainer).validate(request_body)
+
+        serialized_request = (
+            Serializer(f"{self.base_url}/equity/exercise", self.get_default_headers())
+            .serialize()
+            .set_method("POST")
+            .set_body(request_body)
+        )
+
+        response = self.send_request(serialized_request)
+
+        return CreatedExerciseEquityContainer._unmap(response)
+
+    @cast_models
+    def approve_exercise_equity(
+        self, request_body: ExerciseEquityToUpdateContainer, exercise_id: str
+    ) -> UpdatedExerciseEquityContainer:
+        """Approve an equity exercise.
+
+        :param request_body: The request body.
+        :type request_body: ExerciseEquityToUpdateContainer
+        :param exercise_id: ID of the exercise.
+        :type exercise_id: str
+        ...
+        :raises RequestError: Raised when a request fails, with optional HTTP status code and details.
+        ...
+        :return: Successful operation.
+        :rtype: UpdatedExerciseEquityContainer
+        """
+
+        Validator(ExerciseEquityToUpdateContainer).validate(request_body)
+        Validator(str).validate(exercise_id)
+
+        serialized_request = (
+            Serializer(
+                f"{self.base_url}/equity/exercise/{{exercise_id}}",
+                self.get_default_headers(),
+            )
+            .add_path("exercise_id", exercise_id)
+            .serialize()
+            .set_method("PATCH")
+            .set_body(request_body)
+        )
+
+        response = self.send_request(serialized_request)
+
+        return UpdatedExerciseEquityContainer._unmap(response)
+
+    @cast_models
     def get_contract_list(
         self,
         after_cursor: str = None,
         limit: float = None,
         order_direction: SortDirEnum = None,
         types: List[ContractTypeEnum] = None,
         statuses: List[ContractStatusEnum] = None,
```

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/eor.py` & `deel_sdk-1.0.4/src/deel_sdk/services/eor.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/global_payroll.py` & `deel_sdk-1.0.4/src/deel_sdk/services/global_payroll.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/invoices.py` & `deel_sdk-1.0.4/src/deel_sdk/services/invoices.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/lookups.py` & `deel_sdk-1.0.4/src/deel_sdk/services/lookups.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/managers.py` & `deel_sdk-1.0.4/src/deel_sdk/services/managers.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/milestones.py` & `deel_sdk-1.0.4/src/deel_sdk/services/milestones.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/off_cycle_payments.py` & `deel_sdk-1.0.4/src/deel_sdk/services/off_cycle_payments.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/organizations.py` & `deel_sdk-1.0.4/src/deel_sdk/services/organizations.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/partner_managed.py` & `deel_sdk-1.0.4/src/deel_sdk/services/partner_managed.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/people.py` & `deel_sdk-1.0.4/src/deel_sdk/services/people.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/tasks.py` & `deel_sdk-1.0.4/src/deel_sdk/services/tasks.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/time_off.py` & `deel_sdk-1.0.4/src/deel_sdk/services/time_off.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/timesheets.py` & `deel_sdk-1.0.4/src/deel_sdk/services/timesheets.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/token.py` & `deel_sdk-1.0.4/src/deel_sdk/services/token.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/utils/base_service.py` & `deel_sdk-1.0.4/src/deel_sdk/services/utils/base_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,24 +24,20 @@
         """
         Initializes a BaseService instance.
 
         :param str base_url: The base URL for the service. Defaults to None.
         """
         self.base_url = base_url
         self._default_headers = DefaultHeaders()
-        self._request_handler = (
-            RequestChain()
-            .add_handler(RetryHandler())
-            .add_handler(HookHandler())
-            .add_handler(HttpHandler())
-        )
+
+        self._request_handler = self._get_request_handler()
 
     def set_access_token(self, access_token: str):
         """
-        Sets the access token for the entire SDK.
+        Sets the access token for the service.
         """
         self._default_headers.set_header(
             DefaultHeadersKeys.ACCESS_AUTH, AccessTokenAuth(access_token)
         )
 
         return self
 
@@ -70,7 +66,21 @@
         """
         Get the default headers.
 
         :return: A list of the default headers.
         :rtype: list
         """
         return self._default_headers.get_headers()
+
+    def _get_request_handler(self) -> RequestChain:
+        """
+        Get the request chain.
+
+        :return: The request chain.
+        :rtype: RequestChain
+        """
+        return (
+            RequestChain()
+            .add_handler(RetryHandler())
+            .add_handler(HookHandler())
+            .add_handler(HttpHandler())
+        )
```

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/utils/default_headers.py` & `deel_sdk-1.0.4/src/deel_sdk/services/utils/default_headers.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/utils/validator.py` & `deel_sdk-1.0.4/src/deel_sdk/services/utils/validator.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk/services/webhooks.py` & `deel_sdk-1.0.4/src/deel_sdk/services/webhooks.py`

 * *Files identical despite different names*

### Comparing `deel_sdk-1.0.2/src/deel_sdk.egg-info/PKG-INFO` & `deel_sdk-1.0.4/src/deel_sdk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: deel-sdk
-Version: 1.0.2
+Version: 1.0.4
 Summary: Deel REST API
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
-# DeelSdk Python SDK 1.0.2
+# DeelSdk Python SDK 1.0.4
 
 A Python SDK for DeelSdk.
 
 - API version: 1.25.0
-- SDK version: 1.0.2
+- SDK version: 1.0.4
 
 Deel REST API
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Authentication](#authentication)
@@ -102,37 +102,41 @@
 
 You cannot create an instance of a Union type itself. Instead, pass an instance of one of the types in the Union, or a dictionary that can be converted to one of those types.
 
 ## Services
 
 A list of all SDK services. Click on the service name to access its corresponding service methods.
 
-| Service                                             |
-| :-------------------------------------------------- |
-| [AccountingService](#accountingservice)             |
-| [ManagersService](#managersservice)                 |
-| [PeopleService](#peopleservice)                     |
-| [EorService](#eorservice)                           |
-| [GlobalPayrollService](#globalpayrollservice)       |
-| [ContractorsService](#contractorsservice)           |
-| [AdjustmentsService](#adjustmentsservice)           |
-| [CandidatesService](#candidatesservice)             |
-| [PartnerManagedService](#partnermanagedservice)     |
-| [ContractsService](#contractsservice)               |
-| [TasksService](#tasksservice)                       |
-| [TimesheetsService](#timesheetsservice)             |
-| [MilestonesService](#milestonesservice)             |
-| [OffCyclePaymentsService](#offcyclepaymentsservice) |
-| [TimeOffService](#timeoffservice)                   |
-| [InvoicesService](#invoicesservice)                 |
-| [OrganizationsService](#organizationsservice)       |
-| [LookupsService](#lookupsservice)                   |
-| [WebhooksService](#webhooksservice)                 |
-| [TokenService](#tokenservice)                       |
-| [CartaService](#cartaservice)                       |
+| Service                                                       |
+| :------------------------------------------------------------ |
+| [AccountingService](#accountingservice)                       |
+| [CustomFieldsService](#customfieldsservice)                   |
+| [HrisOrganizationsService](#hrisorganizationsservice)         |
+| [ContractsService](#contractsservice)                         |
+| [OrganizationStructureService](#organizationstructureservice) |
+| [PositionsService](#positionsservice)                         |
+| [ManagersService](#managersservice)                           |
+| [PeopleService](#peopleservice)                               |
+| [EorService](#eorservice)                                     |
+| [GlobalPayrollService](#globalpayrollservice)                 |
+| [ContractorsService](#contractorsservice)                     |
+| [AdjustmentsService](#adjustmentsservice)                     |
+| [CandidatesService](#candidatesservice)                       |
+| [PartnerManagedService](#partnermanagedservice)               |
+| [TasksService](#tasksservice)                                 |
+| [TimesheetsService](#timesheetsservice)                       |
+| [MilestonesService](#milestonesservice)                       |
+| [OffCyclePaymentsService](#offcyclepaymentsservice)           |
+| [TimeOffService](#timeoffservice)                             |
+| [InvoicesService](#invoicesservice)                           |
+| [OrganizationsService](#organizationsservice)                 |
+| [LookupsService](#lookupsservice)                             |
+| [WebhooksService](#webhooksservice)                           |
+| [TokenService](#tokenservice)                                 |
+| [CartaService](#cartaservice)                                 |
 
 ### AccountingService
 
 A list of all methods in the `AccountingService` service. Click on the method name to view detailed information about that method.
 
 | Methods                                                                 | Description                                                                                                            |
 | :---------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------- |
@@ -162,23 +166,25 @@
 
 `InvoiceListContainer`
 
 **Example Usage Code Snippet**
 
 ```py
 from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import GetInvoiceListEntities
+from deel_sdk.models.get_invoice_list_entities import List[LegalEntityType]
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
-entities=GetInvoiceListEntities(**[
+entities=List[LegalEntityType](
+    [
     "individual"
-])
+]
+)
 
 result = sdk.accounting.get_invoice_list(
     issued_from_date="issued_from_date",
     issued_to_date="issued_to_date",
     entities=entities,
     limit=10,
     offset=808037660.53
@@ -274,26 +280,31 @@
 
 `PaymentListContainer`
 
 **Example Usage Code Snippet**
 
 ```py
 from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import GetPaymentListCurrencies, GetPaymentListEntities
+from deel_sdk.models.get_payment_list_currencies import List[str]
+from deel_sdk.models.get_payment_list_entities import List[LegalEntityType]
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
-currencies=GetPaymentListCurrencies(**[
+currencies=List[str](
+    [
     "GBP"
-])
-entities=GetPaymentListEntities(**[
+]
+)
+entities=List[LegalEntityType](
+    [
     "individual"
-])
+]
+)
 
 result = sdk.accounting.get_payment_list(
     date_from="1999-12-31",
     date_to="1999-12-31",
     currencies=currencies,
     entities=entities
 )
@@ -328,14 +339,1569 @@
 )
 
 result = sdk.accounting.get_payments_break_down_by_id(payment_id="payment_id")
 
 print(result)
 ```
 
+### CustomFieldsService
+
+A list of all methods in the `CustomFieldsService` service. Click on the method name to view detailed information about that method.
+
+| Methods                                                                               | Description                                                                                                                                        |
+| :------------------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------- |
+| [get_custom_fields_from_people](#get_custom_fields_from_people)                       | Fetch all custom fields associated with People records, offering additional personalized information.                                              |
+| [get_custom_field_from_people_by_id](#get_custom_field_from_people_by_id)             | Access details of a specific custom field by using the custom field ID to enrich individual personnel records.                                     |
+| [get_custom_field_values_from_worker](#get_custom_field_values_from_worker)           | Obtain all custom field values associated with a specific worker, facilitating detailed data retrieval for administrative or operational purposes. |
+| [upsert_custom_field_value_from_worker](#upsert_custom_field_value_from_worker)       | Add or update custom field values for a specific worker, ensuring their profile is up-to-date with the latest information.                         |
+| [delete_custom_field_value_from_worker](#delete_custom_field_value_from_worker)       | Delete a specific custom field value from a worker's profile, removing outdated or unnecessary information.                                        |
+| [get_custom_fields_from_contracts](#get_custom_fields_from_contracts)                 | Fetch all custom fields associated with contracts, providing additional data necessary for contract management.                                    |
+| [get_custom_field_from_contracts_by_id](#get_custom_field_from_contracts_by_id)       | Access details of a specific custom field associated with a contract to manage contract-specific attributes effectively.                           |
+| [get_custom_field_values_from_contract](#get_custom_field_values_from_contract)       | Obtain all custom field values for a specific contract, enhancing contract management with detailed, custom-configured data.                       |
+| [upsert_custom_field_value_from_contracts](#upsert_custom_field_value_from_contracts) | Add or update custom field values for a specific contract, ensuring all contract details are current and relevant.                                 |
+| [delete_contract_custom_field](#delete_contract_custom_field)                         | Delete a specific custom field’s value from a contract, streamlining contract data management by removing redundant or outdated information.       |
+
+#### **get_custom_fields_from_people**
+
+Fetch all custom fields associated with People records, offering additional personalized information.
+
+- HTTP Method: `GET`
+- Endpoint: `/people/custom_fields`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+
+**Return Type**
+
+`CustomFieldsListContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.get_custom_fields_from_people()
+
+print(result)
+```
+
+#### **get_custom_field_from_people_by_id**
+
+Access details of a specific custom field by using the custom field ID to enrich individual personnel records.
+
+- HTTP Method: `GET`
+- Endpoint: `/people/custom_fields/{field_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| field_id | str | ✅ | Access details of a specific custom field by using the custom field ID to enrich individual personnel records. |
+
+**Return Type**
+
+`CustomFieldItemContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.get_custom_field_from_people_by_id(field_id="field_id")
+
+print(result)
+```
+
+#### **get_custom_field_values_from_worker**
+
+Obtain all custom field values associated with a specific worker, facilitating detailed data retrieval for administrative or operational purposes.
+
+- HTTP Method: `GET`
+- Endpoint: `/people/{worker_id}/custom_fields`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| worker_id | str | ✅ | Obtain all custom field values associated with a specific worker, facilitating detailed data retrieval for administrative or operational purposes. |
+
+**Return Type**
+
+`CustomFieldValuesContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.get_custom_field_values_from_worker(worker_id="worker_id")
+
+print(result)
+```
+
+#### **upsert_custom_field_value_from_worker**
+
+Add or update custom field values for a specific worker, ensuring their profile is up-to-date with the latest information.
+
+- HTTP Method: `PUT`
+- Endpoint: `/people/{worker_id}/custom_fields`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | CustomFieldToUpdateContainer | ✅ | The request body. |
+| worker_id | str | ✅ | Add or update custom field values for a specific worker, ensuring their profile is up-to-date with the latest information. |
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import CustomFieldToUpdateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = CustomFieldToUpdateContainer(
+    id_="id",
+    data={
+        "value": "value"
+    }
+)
+
+result = sdk.custom_fields.upsert_custom_field_value_from_worker(
+    request_body=request_body,
+    worker_id="worker_id"
+)
+
+print(result)
+```
+
+#### **delete_custom_field_value_from_worker**
+
+Delete a specific custom field value from a worker's profile, removing outdated or unnecessary information.
+
+- HTTP Method: `DELETE`
+- Endpoint: `/people/{worker_id}/custom_fields/{field_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| worker_id | str | ✅ | Delete a specific custom field value from a worker's profile, removing outdated or unnecessary information. |
+| field_id | str | ✅ | Delete a specific custom field value from a worker's profile, removing outdated or unnecessary information. |
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.delete_custom_field_value_from_worker(
+    worker_id="worker_id",
+    field_id="field_id"
+)
+
+print(result)
+```
+
+#### **get_custom_fields_from_contracts**
+
+Fetch all custom fields associated with contracts, providing additional data necessary for contract management.
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts/custom_fields`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+
+**Return Type**
+
+`CustomFieldsListContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.get_custom_fields_from_contracts()
+
+print(result)
+```
+
+#### **get_custom_field_from_contracts_by_id**
+
+Access details of a specific custom field associated with a contract to manage contract-specific attributes effectively.
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts/custom_fields/{field_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| field_id | str | ✅ | Access details of a specific custom field associated with a contract to manage contract-specific attributes effectively. |
+
+**Return Type**
+
+`CustomFieldItemContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.get_custom_field_from_contracts_by_id(field_id="field_id")
+
+print(result)
+```
+
+#### **get_custom_field_values_from_contract**
+
+Obtain all custom field values for a specific contract, enhancing contract management with detailed, custom-configured data.
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts/{contract_id}/custom_fields`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Obtain all custom field values for a specific contract, enhancing contract management with detailed, custom-configured data. |
+
+**Return Type**
+
+`CustomFieldValuesContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.get_custom_field_values_from_contract(contract_id="contract_id")
+
+print(result)
+```
+
+#### **upsert_custom_field_value_from_contracts**
+
+Add or update custom field values for a specific contract, ensuring all contract details are current and relevant.
+
+- HTTP Method: `PUT`
+- Endpoint: `/contracts/{contract_id}/custom_fields`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | CustomFieldToUpdateContainer | ✅ | The request body. |
+| contract_id | str | ✅ | Add or update custom field values for a specific contract, ensuring all contract details are current and relevant. |
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import CustomFieldToUpdateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = CustomFieldToUpdateContainer(
+    id_="id",
+    data={
+        "value": "value"
+    }
+)
+
+result = sdk.custom_fields.upsert_custom_field_value_from_contracts(
+    request_body=request_body,
+    contract_id="contract_id"
+)
+
+print(result)
+```
+
+#### **delete_contract_custom_field**
+
+Delete a specific custom field’s value from a contract, streamlining contract data management by removing redundant or outdated information.
+
+- HTTP Method: `DELETE`
+- Endpoint: `/contracts/{contract_id}/custom_fields/{field_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Delete a specific custom field’s value from a contract, streamlining contract data management by removing redundant or outdated information. |
+| field_id | str | ✅ | Delete a specific custom field’s value from a contract, streamlining contract data management by removing redundant or outdated information. |
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.custom_fields.delete_contract_custom_field(
+    contract_id="contract_id",
+    field_id="field_id"
+)
+
+print(result)
+```
+
+### HrisOrganizationsService
+
+A list of all methods in the `HrisOrganizationsService` service. Click on the method name to view detailed information about that method.
+
+| Methods                                               | Description                                |
+| :---------------------------------------------------- | :----------------------------------------- |
+| [get_organization_roles](#get_organization_roles)     | Get the roles of the current organization. |
+| [create_organization_role](#create_organization_role) | Create organization custom role.           |
+| [update_organization_role](#update_organization_role) | Update organization custom role.           |
+
+#### **get_organization_roles**
+
+Get the roles of the current organization.
+
+- HTTP Method: `GET`
+- Endpoint: `/roles`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+
+**Return Type**
+
+`GetRolesContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.hris_organizations.get_organization_roles()
+
+print(result)
+```
+
+#### **create_organization_role**
+
+Create organization custom role.
+
+- HTTP Method: `POST`
+- Endpoint: `/roles`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | RoleToCreateContainer | ✅ | The request body. |
+
+**Return Type**
+
+`CreatedRoleContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import RoleToCreateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = RoleToCreateContainer(
+    data={
+        "name": "name",
+        "scope": "ORGANIZATION",
+        "description": "description",
+        "permission_sets": [
+            "permissionSets"
+        ],
+        "hris_org_structure_id": "hrisOrgStructureId"
+    }
+)
+
+result = sdk.hris_organizations.create_organization_role(request_body=request_body)
+
+print(result)
+```
+
+#### **update_organization_role**
+
+Update organization custom role.
+
+- HTTP Method: `PATCH`
+- Endpoint: `/roles/{role_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | RoleToUpdateContainer | ✅ | The request body. |
+| role_id | str | ✅ | Update organization custom role. |
+
+**Return Type**
+
+`UpdatedRoleContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import RoleToUpdateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = RoleToUpdateContainer(
+    data={
+        "name": "name",
+        "description": "description",
+        "permission_sets": [
+            "permissionSets"
+        ]
+    }
+)
+
+result = sdk.hris_organizations.update_organization_role(
+    request_body=request_body,
+    role_id="role_id"
+)
+
+print(result)
+```
+
+### ContractsService
+
+A list of all methods in the `ContractsService` service. Click on the method name to view detailed information about that method.
+
+| Methods                                                                     | Description                                                                                                                                                                                                          |
+| :-------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| [request_exercise_equity](#request_exercise_equity)                         | Create a request to exercise equity.                                                                                                                                                                                 |
+| [approve_exercise_equity](#approve_exercise_equity)                         | Approve an equity exercise.                                                                                                                                                                                          |
+| [get_contract_list](#get_contract_list)                                     | Retrieve a list of contracts.                                                                                                                                                                                        |
+| [get_contract_by_id](#get_contract_by_id)                                   | Retrieve a single contract.                                                                                                                                                                                          |
+| [attach_external_id](#attach_external_id)                                   | Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later. |
+| [add_contract_document](#add_contract_document)                             | Attach a file to contract document.                                                                                                                                                                                  |
+| [edit_contract_document](#edit_contract_document)                           | Overwrite the file currently attached to contract document.                                                                                                                                                          |
+| [get_alternate_emails_by_contract_id](#get_alternate_emails_by_contract_id) | Returns an array of alternate email objects                                                                                                                                                                          |
+| [sign_contract](#sign_contract)                                             | Sign a contract as a client.                                                                                                                                                                                         |
+| [invite_to_sign_contract](#invite_to_sign_contract)                         | Invite a worker to sign the contract. Worker will be notified via email.                                                                                                                                             |
+| [uninvite_to_sign_contract](#uninvite_to_sign_contract)                     | Remove invite in order to re-invite a worker to sign the contract.                                                                                                                                                   |
+| [calculate_final_payment](#calculate_final_payment)                         | Calculate the final payment due to the contractor when ending the contract.                                                                                                                                          |
+| [post_contract_estimate](#post_contract_estimate)                           | First payment is calculated from the number of working/calendar days between their start date and the start of the payment cycle.                                                                                    |
+| [get_contract_templates](#get_contract_templates)                           | Retrieve a list of contract templates in your organization.                                                                                                                                                          |
+| [get_worker_documents_by_id](#get_worker_documents_by_id)                   | Retrieve a list of documents of a worker.                                                                                                                                                                            |
+| [get_download_worker_documents_by_id](#get_download_worker_documents_by_id) | Get the download link of worker document.                                                                                                                                                                            |
+
+#### **request_exercise_equity**
+
+Create a request to exercise equity.
+
+- HTTP Method: `POST`
+- Endpoint: `/equity/exercise`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | ExerciseEquityToCreateContainer | ✅ | The request body. |
+
+**Return Type**
+
+`CreatedExerciseEquityContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import ExerciseEquityToCreateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = ExerciseEquityToCreateContainer(
+    fmv="fmv",
+    quantity=8.76,
+    issuer_id="issuer_id",
+    worker_id="worker_id",
+    address_zip="address_zip",
+    exercise_id="exercise_id",
+    address_city="address_city",
+    address_state="address_state",
+    address_street="address_street",
+    stakeholder_id="stakeholder_id",
+    address_country="address_country",
+    option_grant_id="option_grant_id",
+    fmv_currency_code="fmv_currency_code",
+    stakeholder_email="stakeholder_email",
+    option_grant_issue="option_grant_issue",
+    option_grant_label="option_grant_label",
+    option_grant_currency="option_grant_currency",
+    option_grant_issue_date="option_grant_issue_date",
+    option_grant_expiry_date="option_grant_expiry_date",
+    stakeholder_relationship="stakeholder_relationship",
+    option_grant_strike_price="option_grant_strike_price"
+)
+
+result = sdk.contracts.request_exercise_equity(request_body=request_body)
+
+print(result)
+```
+
+#### **approve_exercise_equity**
+
+Approve an equity exercise.
+
+- HTTP Method: `PATCH`
+- Endpoint: `/equity/exercise/{exercise_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | ExerciseEquityToUpdateContainer | ✅ | The request body. |
+| exercise_id | str | ✅ | Approve an equity exercise. |
+
+**Return Type**
+
+`UpdatedExerciseEquityContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import ExerciseEquityToUpdateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = ExerciseEquityToUpdateContainer(
+    employer_approval="employer_approval"
+)
+
+result = sdk.contracts.approve_exercise_equity(
+    request_body=request_body,
+    exercise_id="exercise_id"
+)
+
+print(result)
+```
+
+#### **get_contract_list**
+
+Retrieve a list of contracts.
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| after_cursor | str | ❌ | Retrieve a list of contracts. |
+| limit | float | ❌ | Retrieve a list of contracts. |
+| order_direction | SortDirEnum | ❌ | Retrieve a list of contracts. |
+| types | List[ContractTypeEnum] | ❌ | Retrieve a list of contracts. |
+| statuses | List[ContractStatusEnum] | ❌ | Retrieve a list of contracts. |
+| team_id | str | ❌ | Retrieve a list of contracts. |
+| external_id | str | ❌ | Retrieve a list of contracts. |
+| countries | List[str] | ❌ | Retrieve a list of contracts. |
+| currencies | GetContractListCurrencies | ❌ | Retrieve a list of contracts. |
+| search | str | ❌ | Retrieve a list of contracts. |
+| sort_by | ContractsSortByEnum | ❌ | Retrieve a list of contracts. |
+
+**Return Type**
+
+`ContractListContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import SortDirEnum, ContractsSortByEnum
+from deel_sdk.models.get_contract_list_currencies import List[str]
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+types=[
+    "ongoing_time_based"
+]
+statuses=[
+    "new"
+]
+countries=[
+    "US"
+]
+currencies=List[str](
+    [
+    "GBP"
+]
+)
+
+result = sdk.contracts.get_contract_list(
+    after_cursor="after_cursor",
+    limit=10,
+    order_direction="asc",
+    types=types,
+    statuses=statuses,
+    team_id="team_id",
+    external_id="external_id",
+    countries=countries,
+    currencies=currencies,
+    search="search",
+    sort_by="contract_title"
+)
+
+print(result)
+```
+
+#### **get_contract_by_id**
+
+Retrieve a single contract.
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts/{contract_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Retrieve a single contract. |
+
+**Return Type**
+
+`ContractContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.get_contract_by_id(contract_id="contract_id")
+
+print(result)
+```
+
+#### **attach_external_id**
+
+Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later.
+
+- HTTP Method: `PATCH`
+- Endpoint: `/contracts/{contract_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | InputToPatchContractExternalId | ✅ | The request body. |
+| contract_id | str | ✅ | Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later. |
+
+**Return Type**
+
+`GenericResultCreated`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import InputToPatchContractExternalId
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = InputToPatchContractExternalId(
+    data={
+        "external_id": "external_id"
+    }
+)
+
+result = sdk.contracts.attach_external_id(
+    request_body=request_body,
+    contract_id="contract_id"
+)
+
+print(result)
+```
+
+#### **add_contract_document**
+
+Attach a file to contract document.
+
+- HTTP Method: `POST`
+- Endpoint: `/contracts/{contract_id}/documents`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | dict | ❌ | The request body. |
+| contract_id | str | ✅ | Attach a file to contract document. |
+
+**Return Type**
+
+`ContractDocumentContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import FileObject
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = {
+    "file": "file"
+}
+
+result = sdk.contracts.add_contract_document(
+    request_body=request_body,
+    contract_id="contract_id"
+)
+
+print(result)
+```
+
+#### **edit_contract_document**
+
+Overwrite the file currently attached to contract document.
+
+- HTTP Method: `PUT`
+- Endpoint: `/contracts/{contract_id}/documents`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | dict | ❌ | The request body. |
+| contract_id | str | ✅ | Overwrite the file currently attached to contract document. |
+
+**Return Type**
+
+`ContractDocumentContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import FileObject
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = {
+    "file": "file"
+}
+
+result = sdk.contracts.edit_contract_document(
+    request_body=request_body,
+    contract_id="contract_id"
+)
+
+print(result)
+```
+
+#### **get_alternate_emails_by_contract_id**
+
+Returns an array of alternate email objects
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts/{contract_id}/alternate_emails`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Returns an array of alternate email objects |
+
+**Return Type**
+
+`List[AlternateEmailItem]`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.get_alternate_emails_by_contract_id(contract_id="contract_id")
+
+print(result)
+```
+
+#### **sign_contract**
+
+Sign a contract as a client.
+
+- HTTP Method: `POST`
+- Endpoint: `/contracts/{contract_id}/signatures`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | ContractSignatureToCreateContainer | ✅ | The request body. |
+| contract_id | str | ✅ | Sign a contract as a client. |
+
+**Return Type**
+
+`GenericResultCreated`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import ContractSignatureToCreateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = ContractSignatureToCreateContainer(
+    data={
+        "client_signature": "dolor enim in",
+        "contract_template_id": 2.41
+    }
+)
+
+result = sdk.contracts.sign_contract(
+    request_body=request_body,
+    contract_id="contract_id"
+)
+
+print(result)
+```
+
+#### **invite_to_sign_contract**
+
+Invite a worker to sign the contract. Worker will be notified via email.
+
+- HTTP Method: `POST`
+- Endpoint: `/contracts/{contract_id}/invitations`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | ContractInvitationToCreateContainer | ✅ | The request body. |
+| contract_id | str | ✅ | Invite a worker to sign the contract. Worker will be notified via email. |
+
+**Return Type**
+
+`GenericResultCreated`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import ContractInvitationToCreateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = ContractInvitationToCreateContainer(
+    data={
+        "email": "eiusmod",
+        "message": "nulla off"
+    }
+)
+
+result = sdk.contracts.invite_to_sign_contract(
+    request_body=request_body,
+    contract_id="contract_id"
+)
+
+print(result)
+```
+
+#### **uninvite_to_sign_contract**
+
+Remove invite in order to re-invite a worker to sign the contract.
+
+- HTTP Method: `DELETE`
+- Endpoint: `/contracts/{contract_id}/invitations`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Remove invite in order to re-invite a worker to sign the contract. |
+
+**Return Type**
+
+`GenericResultDeleted`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.uninvite_to_sign_contract(contract_id="contract_id")
+
+print(result)
+```
+
+#### **calculate_final_payment**
+
+Calculate the final payment due to the contractor when ending the contract.
+
+- HTTP Method: `GET`
+- Endpoint: `/contracts/{contract_id}/final-payments`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Calculate the final payment due to the contractor when ending the contract. |
+| end_date | str | ❌ | Calculate the final payment due to the contractor when ending the contract. |
+| calculation_type | CalculateFinalPaymentCalculationType | ❌ | Calculate the final payment due to the contractor when ending the contract. |
+| workweek_start | str | ❌ | Calculate the final payment due to the contractor when ending the contract. |
+| workweek_end | str | ❌ | Calculate the final payment due to the contractor when ending the contract. |
+
+**Return Type**
+
+`FinalPaymentCalculatedContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import CalculateFinalPaymentCalculationType
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.calculate_final_payment(
+    contract_id="contract_id",
+    end_date="1999-12-31",
+    calculation_type="CUSTOM_AMOUNT",
+    workweek_start="workweek_start",
+    workweek_end="workweek_end"
+)
+
+print(result)
+```
+
+#### **post_contract_estimate**
+
+First payment is calculated from the number of working/calendar days between their start date and the start of the payment cycle.
+
+- HTTP Method: `POST`
+- Endpoint: `/contracts/estimate`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | EstimateFirstPaymentContainer | ✅ | The request body. |
+
+**Return Type**
+
+`ResponseEstimateFirstPaymentContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import EstimateFirstPaymentContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = EstimateFirstPaymentContainer(
+    data={
+        "type_": "ongoing_time_based",
+        "country_code": "US",
+        "start_date": "1999-12-31",
+        "compensation_details": {
+            "amount": 2500,
+            "currency_code": "GBP",
+            "scale": "weekly",
+            "cycle_end": 20.71,
+            "cycle_end_type": "DAY_OF_WEEK",
+            "payment_due_type": "REGULAR",
+            "payment_due_days": 16.18,
+            "calculation_type": "CUSTOM_AMOUNT",
+            "work_week_start": "Sunday",
+            "work_week_end": "Sunday"
+        }
+    }
+)
+
+result = sdk.contracts.post_contract_estimate(request_body=request_body)
+
+print(result)
+```
+
+#### **get_contract_templates**
+
+Retrieve a list of contract templates in your organization.
+
+- HTTP Method: `GET`
+- Endpoint: `/contract-templates`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+
+**Return Type**
+
+`ContractTemplateListContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.get_contract_templates()
+
+print(result)
+```
+
+#### **get_worker_documents_by_id**
+
+Retrieve a list of documents of a worker.
+
+- HTTP Method: `GET`
+- Endpoint: `/workers/{worker_id}/documents`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| worker_id | str | ✅ | Retrieve a list of documents of a worker. |
+
+**Return Type**
+
+`WorkerDocumentsByIdContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.get_worker_documents_by_id(worker_id="worker_id")
+
+print(result)
+```
+
+#### **get_download_worker_documents_by_id**
+
+Get the download link of worker document.
+
+- HTTP Method: `GET`
+- Endpoint: `/workers/{worker_id}/documents/{document_id}/download`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| worker_id | str | ✅ | Get the download link of worker document. |
+| document_id | float | ✅ | Get the download link of worker document. |
+
+**Return Type**
+
+`DownloadWorkerDocumentsByIdContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.contracts.get_download_worker_documents_by_id(
+    worker_id="worker_id",
+    document_id=6.05
+)
+
+print(result)
+```
+
+### OrganizationStructureService
+
+A list of all methods in the `OrganizationStructureService` service. Click on the method name to view detailed information about that method.
+
+| Methods                                                         | Description                                     |
+| :-------------------------------------------------------------- | :---------------------------------------------- |
+| [get_all_org_structures](#get_all_org_structures)               | Fetch all Org Structures from the Organization. |
+| [create_org_structure](#create_org_structure)                   | Create a new HRIS Organization Structure.       |
+| [get_org_structure](#get_org_structure)                         | Fetch an Org Structure from the Organization.   |
+| [update_org_structure](#update_org_structure)                   | Update an existing Organization structure.      |
+| [delete_org_structure](#delete_org_structure)                   | Delete an Org Structure from the Organization.  |
+| [get_external_org_structure](#get_external_org_structure)       | Fetch an Org Structure from the Organization.   |
+| [update_external_org_structure](#update_external_org_structure) | Update an existing Organization structure.      |
+| [delete_external_org_structure](#delete_external_org_structure) | Delete an Org Structure from the Organization.  |
+
+#### **get_all_org_structures**
+
+Fetch all Org Structures from the Organization.
+
+- HTTP Method: `GET`
+- Endpoint: `/hris/organization_structures`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+
+**Return Type**
+
+`GetAllOrgStructuresContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.organization_structure.get_all_org_structures()
+
+print(result)
+```
+
+#### **create_org_structure**
+
+Create a new HRIS Organization Structure.
+
+- HTTP Method: `POST`
+- Endpoint: `/hris/organization_structures`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | OrgStructureToCreateContainer | ✅ | The request body. |
+
+**Return Type**
+
+`GetAllOrgStructuresContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import OrgStructureToCreateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = OrgStructureToCreateContainer(
+    data={
+        "name": "name",
+        "teams": [
+            {
+                "name": "name",
+                "external_id": "external_id"
+            }
+        ],
+        "external_id": "external_id",
+        "enable_roles": True,
+        "is_multiple_select": True
+    }
+)
+
+result = sdk.organization_structure.create_org_structure(request_body=request_body)
+
+print(result)
+```
+
+#### **get_org_structure**
+
+Fetch an Org Structure from the Organization.
+
+- HTTP Method: `GET`
+- Endpoint: `/hris/organization_structures/{hrisOrgStr_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| hris_org_str_id | str | ✅ | Fetch an Org Structure from the Organization. |
+
+**Return Type**
+
+`GetOrgStructureContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.organization_structure.get_org_structure(hris_org_str_id="hrisOrgStr_id")
+
+print(result)
+```
+
+#### **update_org_structure**
+
+Update an existing Organization structure.
+
+- HTTP Method: `PATCH`
+- Endpoint: `/hris/organization_structures/{hrisOrgStr_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | OrgStructureToUpdateContainer | ✅ | The request body. |
+| hris_org_str_id | str | ✅ | Update an existing Organization structure. |
+
+**Return Type**
+
+`any`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import OrgStructureToUpdateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = OrgStructureToUpdateContainer(
+    data={
+        "name": "name",
+        "teams": [
+            {}
+        ],
+        "external_id": "external_id",
+        "enable_roles": False,
+        "is_multiselect": True
+    }
+)
+
+result = sdk.organization_structure.update_org_structure(
+    request_body=request_body,
+    hris_org_str_id="hrisOrgStr_id"
+)
+
+print(result)
+```
+
+#### **delete_org_structure**
+
+Delete an Org Structure from the Organization.
+
+- HTTP Method: `DELETE`
+- Endpoint: `/hris/organization_structures/{hrisOrgStr_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| hris_org_str_id | str | ✅ | Delete an Org Structure from the Organization. |
+
+**Return Type**
+
+`any`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.organization_structure.delete_org_structure(hris_org_str_id="hrisOrgStr_id")
+
+print(result)
+```
+
+#### **get_external_org_structure**
+
+Fetch an Org Structure from the Organization.
+
+- HTTP Method: `GET`
+- Endpoint: `/hris/organization_structures/external/{external_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| external_id | str | ✅ | Fetch an Org Structure from the Organization. |
+
+**Return Type**
+
+`GetOrgStructureContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.organization_structure.get_external_org_structure(external_id="external_id")
+
+print(result)
+```
+
+#### **update_external_org_structure**
+
+Update an existing Organization structure.
+
+- HTTP Method: `PATCH`
+- Endpoint: `/hris/organization_structures/external/{external_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | OrgStructureToUpdateContainer | ✅ | The request body. |
+| external_id | str | ✅ | Update an existing Organization structure. |
+
+**Return Type**
+
+`any`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import OrgStructureToUpdateContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = OrgStructureToUpdateContainer(
+    data={
+        "name": "name",
+        "teams": [
+            {}
+        ],
+        "external_id": "external_id",
+        "enable_roles": False,
+        "is_multiselect": True
+    }
+)
+
+result = sdk.organization_structure.update_external_org_structure(
+    request_body=request_body,
+    external_id="external_id"
+)
+
+print(result)
+```
+
+#### **delete_external_org_structure**
+
+Delete an Org Structure from the Organization.
+
+- HTTP Method: `DELETE`
+- Endpoint: `/hris/organization_structures/external/{external_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| external_id | str | ✅ | Delete an Org Structure from the Organization. |
+
+**Return Type**
+
+`any`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.organization_structure.delete_external_org_structure(external_id="external_id")
+
+print(result)
+```
+
+### PositionsService
+
+A list of all methods in the `PositionsService` service. Click on the method name to view detailed information about that method.
+
+| Methods                                             | Description                                         |
+| :-------------------------------------------------- | :-------------------------------------------------- |
+| [get_positions](#get_positions)                     | HRIS Positions from a HrisProfile.                  |
+| [apply_changes_positions](#apply_changes_positions) | Apply add, edit, and delete operations to profiles. |
+
+#### **get_positions**
+
+HRIS Positions from a HrisProfile.
+
+- HTTP Method: `GET`
+- Endpoint: `/hris/positions/profile/{hrisProfile_id}`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| hris_profile_id | str | ✅ | HRIS Positions from a HrisProfile. |
+
+**Return Type**
+
+`GetHrisPositionContainer`
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+result = sdk.positions.get_positions(hris_profile_id="hrisProfile_id")
+
+print(result)
+```
+
+#### **apply_changes_positions**
+
+Apply add, edit, and delete operations to profiles.
+
+- HTTP Method: `POST`
+- Endpoint: `/hris/positions/apply_changes`
+
+**Parameters**
+| Name | Type| Required | Description |
+| :-------- | :----------| :----------:| :----------|
+| request_body | HrisPositionToChangeContainer | ✅ | The request body. |
+
+**Example Usage Code Snippet**
+
+```py
+from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import HrisPositionToChangeContainer
+
+sdk = DeelSdk(
+    access_token="YOUR_ACCESS_TOKEN",
+    base_url=Environment.DEFAULT.value
+)
+
+request_body = HrisPositionToChangeContainer(
+    data={
+        "add": [
+            {
+                "role_id": "role_id",
+                "team_id": "team_id",
+                "is_supportive": True
+            }
+        ],
+        "edit": [
+            {
+                "id_": "id",
+                "role_id": "role_id",
+                "is_supportive": False
+            }
+        ],
+        "delete": [
+            {
+                "id_": "id"
+            }
+        ],
+        "profile_id": "profile_id"
+    }
+)
+
+result = sdk.positions.apply_changes_positions(request_body=request_body)
+
+print(result)
+```
+
 ### ManagersService
 
 A list of all methods in the `ManagersService` service. Click on the method name to view detailed information about that method.
 
 | Methods                           | Description                        |
 | :-------------------------------- | :--------------------------------- |
 | [get_managers](#get_managers)     | List all organization managers.    |
@@ -399,21 +1965,21 @@
 from deel_sdk.models import AdminUserCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = AdminUserCreateContainer(**{
-    "data": {
-        "first_name": "dolore",
-        "last_name": "proi",
+request_body = AdminUserCreateContainer(
+    data={
+        "first_name": "mo",
+        "last_name": "Exce",
         "email": "email"
     }
-})
+)
 
 result = sdk.managers.create_manager(request_body=request_body)
 
 print(result)
 ```
 
 ### PeopleService
@@ -460,49 +2026,49 @@
 from deel_sdk.models import HrisDirectEmployee
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = HrisDirectEmployee(**{
-    "employee_details": {
+request_body = HrisDirectEmployee(
+    employee_details={
         "first_name": "John",
         "last_name": "Doe",
         "email": "john.doe@domain.com",
         "work_email": "john.doe@domain.com",
         "nationality": "CA",
         "country": "BR",
         "state": "AC"
     },
-    "team_information": {
-        "team_id": 9.77,
-        "legal_entity_id": 2.18
+    team_information={
+        "team_id": 9.17,
+        "legal_entity_id": 1.13
     },
-    "job_information": {
-        "seniority_id": 9.22,
-        "job_title_id": 6.5
+    job_information={
+        "seniority_id": 2.01,
+        "job_title_id": 6.94
     },
-    "compensation": {
-        "gross_annual_salary": 7.15,
+    compensation={
+        "gross_annual_salary": 4.71,
         "currency": "USD"
     },
-    "contract": {
+    contract={
         "contract_oid": "pdcMQe0cXCCXWTkqkdytw",
         "start_date": "1999-12-31",
-        "employee_number": 9.02,
+        "employee_number": 0.96,
         "end_date": "1999-12-31",
         "employment_type": "PART_TIME",
-        "part_time_percentage": 21.67
+        "part_time_percentage": 63.32
     },
-    "vacation_info": {
+    vacation_info={
         "vacation_accrual_start_date": "vacation_accrual_start_date",
-        "vacation_yearly_policy": 171.07
+        "vacation_yearly_policy": 214.98
     }
-})
+)
 
 result = sdk.people.create_direct_employee(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_internal_people_list**
@@ -529,16 +2095,16 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.people.get_internal_people_list(
-    offset=978653984.34,
-    limit=43.45
+    offset=664489591.67,
+    limit=128.61
 )
 
 print(result)
 ```
 
 #### **get_people_list**
 
@@ -569,16 +2135,16 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.people.get_people_list(
-    offset=44334375.53,
-    limit=105.69,
+    offset=772862704.51,
+    limit=142.31,
     search="search",
     sort_by="id",
     sort_order="asc",
     hiring_statuses="active"
 )
 
 print(result)
@@ -639,19 +2205,19 @@
 from deel_sdk.models import UpdateWorkerDepartmentContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = UpdateWorkerDepartmentContainer(**{
-    "data": {
+request_body = UpdateWorkerDepartmentContainer(
+    data={
         "department_id": "00000000-0000-0000-0000-000000000000"
     }
-})
+)
 
 result = sdk.people.update_people_department(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -681,19 +2247,19 @@
 from deel_sdk.models import UpdateWorkerWorkingLocationContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = UpdateWorkerWorkingLocationContainer(**{
-    "data": {
+request_body = UpdateWorkerWorkingLocationContainer(
+    data={
         "working_location_id": "00000000-0000-0000-0000-000000000000"
     }
-})
+)
 
 result = sdk.people.update_people_working_location(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -941,20 +2507,20 @@
 from deel_sdk.models import TimeoffToReviewInternalContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TimeoffToReviewInternalContainer(**{
-    "data": {
+request_body = TimeoffToReviewInternalContainer(
+    data={
         "status": "APPROVED",
         "reason": "Approved because there are no conflicts."
     }
-})
+)
 
 result = sdk.people.review_time_offs_for_employee(
     request_body=request_body,
     timeoff_id="timeoff_id",
     worker_id="worker_id"
 )
 
@@ -1125,27 +2691,27 @@
 from deel_sdk.models import EorEmployeeCostCalculationRequestBodyContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = EorEmployeeCostCalculationRequestBodyContainer(**{
-    "data": {
+request_body = EorEmployeeCostCalculationRequestBodyContainer(
+    data={
         "salary": 50000,
         "country": "Germany",
         "currency": "EUR",
         "benefits": [
             {
                 "provider_id": "00000000-0000-0000-0000-000000000000",
                 "plan_id": "00000000-0000-0000-0000-000000000000"
             }
         ]
     }
-})
+)
 
 result = sdk.eor.calculate_eor_employment_cost(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_eor_contract_benefits**
@@ -1202,16 +2768,16 @@
 from deel_sdk.models import EorContractToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = EorContractToCreateContainer(**{
-    "data": {
+request_body = EorContractToCreateContainer(
+    data={
         "employee": {
             "first_name": "Jane",
             "last_name": "Doe",
             "email": "employee@email.com",
             "nationality": "US",
             "address": {
                 "street": "Deel Street 500",
@@ -1224,49 +2790,49 @@
         "employment": {
             "country": "US",
             "state": "state",
             "type_": "Full-time",
             "work_visa_required": False,
             "start_date": "1999-12-31",
             "end_date": "1999-12-31",
-            "probation_period": 6.17,
+            "probation_period": 1.47,
             "scope_of_work": "scope_of_work",
             "time_off_type": "STANDARD",
-            "holidays": 5.67
+            "holidays": 0.98
         },
         "job_title": "job_title",
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "client": {
             "legal_entity": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "compensation_details": {
-            "salary": 5.95,
+            "salary": 3.09,
             "currency": "currency",
-            "variable_compensation": 3.49,
+            "variable_compensation": 6.88,
             "variable_compensation_type": "PERCENTAGE"
         },
         "quote_additional_fields": {
             "gender": "gender",
             "worker_type": "Skilled",
             "dob": "dob"
         },
         "health_plan_id": "health_plan_id",
         "pension": {
             "id_": "id",
             "contribution": "contribution"
         }
     }
-})
+)
 
 result = sdk.eor.create_eor_contract(request_body=request_body)
 
 print(result)
 ```
 
 ### GlobalPayrollService
@@ -1314,55 +2880,55 @@
 from deel_sdk.models import GpContractToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = GpContractToCreateContainer(**{
-    "data": {
+request_body = GpContractToCreateContainer(
+    data={
         "employee": {
             "first_name": "Jane",
             "last_name": "Doe",
-            "email": "culpa Lorem inc",
-            "work_email": "in do L",
+            "email": "esse no",
+            "work_email": "ipsum cillum c",
             "nationality": "US",
             "employee_number": "100",
             "address": {
                 "street": "Deel Street 500",
                 "city": "Denver",
                 "state": "CO",
                 "zip": "44000",
                 "country": "US"
             }
         },
         "employment": {
             "type_": "Full-time",
             "start_date": "1999-12-31",
             "holidays": {
-                "allowance": 5.28,
+                "allowance": 4.86,
                 "start_date": "1999-12-31"
             }
         },
         "job_title": "job_title",
         "client": {
             "legal_entity": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "compensation_details": {
             "scale": "YEAR",
-            "salary": 8.05,
+            "salary": 5.64,
             "currency": "GBP"
         }
     }
-})
+)
 
 result = sdk.global_payroll.create_gp_contract(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_worker_payslips**
@@ -1420,21 +2986,21 @@
 from deel_sdk.models import GpEmployeeAddressToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = GpEmployeeAddressToUpdateContainer(**{
-    "data": {
+request_body = GpEmployeeAddressToUpdateContainer(
+    data={
         "city": "London",
         "street": "123 Deel Street",
         "zip": "12345"
     }
-})
+)
 
 result = sdk.global_payroll.update_gp_employee_address(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -1495,16 +3061,16 @@
 from deel_sdk.models import AddWorkerBankAccountContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = AddWorkerBankAccountContainer(**{
-    "data": {
+request_body = AddWorkerBankAccountContainer(
+    data={
         "full_name": "John Doe",
         "phone": "+1234567890",
         "address_line1": "1234 Main St",
         "address_line2": "Apartment 101",
         "city": "Springfield",
         "province_state": "Ontario",
         "postal": "12345",
@@ -1521,15 +3087,15 @@
         "bank_branch_name": "Main Street Branch",
         "iban": "GB29NWBK60161331926819",
         "email": "john.doe@example.com",
         "rib_number": "12345678901",
         "account_type": "12345678901",
         "ach_routing_number": "12345678901"
     }
-})
+)
 
 result = sdk.global_payroll.add_gp_bank_account(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -1560,16 +3126,16 @@
 from deel_sdk.models import AddWorkerBankAccountContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = AddWorkerBankAccountContainer(**{
-    "data": {
+request_body = AddWorkerBankAccountContainer(
+    data={
         "full_name": "John Doe",
         "phone": "+1234567890",
         "address_line1": "1234 Main St",
         "address_line2": "Apartment 101",
         "city": "Springfield",
         "province_state": "Ontario",
         "postal": "12345",
@@ -1586,15 +3152,15 @@
         "bank_branch_name": "Main Street Branch",
         "iban": "GB29NWBK60161331926819",
         "email": "john.doe@example.com",
         "rib_number": "12345678901",
         "account_type": "12345678901",
         "ach_routing_number": "12345678901"
     }
-})
+)
 
 result = sdk.global_payroll.patch_gp_bank_account(
     request_body=request_body,
     worker_id="worker_id",
     bank_id="bank_id"
 )
 
@@ -1656,21 +3222,21 @@
 from deel_sdk.models import GpEmployeeCompensationToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = GpEmployeeCompensationToUpdateContainer(**{
-    "data": {
+request_body = GpEmployeeCompensationToUpdateContainer(
+    data={
         "scale": "YEAR",
         "salary": 50000,
         "effective_date": "1999-12-31"
     }
-})
+)
 
 result = sdk.global_payroll.update_gp_employee_compensation(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -1700,20 +3266,20 @@
 from deel_sdk.models import GpEmployeePtoToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = GpEmployeePtoToUpdateContainer(**{
-    "data": {
+request_body = GpEmployeePtoToUpdateContainer(
+    data={
         "accrual_start_date": "1999-12-31",
         "yearly_allowance": "15"
     }
-})
+)
 
 result = sdk.global_payroll.update_gp_employee_pto(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -1743,25 +3309,25 @@
 from deel_sdk.models import GpEmployeeInformationToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = GpEmployeeInformationToUpdateContainer(**{
-    "data": {
+request_body = GpEmployeeInformationToUpdateContainer(
+    data={
         "first_name": "Jane",
         "middle_name": "Jay",
         "last_name": "Doe",
         "date_of_birth": "1999-12-31",
         "gender": "gender",
         "marital_status": "Single",
         "employee_number": "employee_number"
     }
-})
+)
 
 result = sdk.global_payroll.update_gp_employee_information(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -1924,23 +3490,23 @@
 from deel_sdk.models import WorkerTerminationBodyContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = WorkerTerminationBodyContainer(**{
-    "data": {
+request_body = WorkerTerminationBodyContainer(
+    data={
         "desired_end_date": "2023-12-31",
         "last_date_of_work": "2023-12-31",
         "message": "Termination reason",
         "is_voluntary": True,
         "severance": {}
     }
-})
+)
 
 result = sdk.global_payroll.request_termination(
     request_body=request_body,
     worker_id="worker_id"
 )
 
 print(result)
@@ -1986,16 +3552,16 @@
 from deel_sdk.models import ContractToCreateContainerPayAsYouGoTimeBased
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToCreateContainerPayAsYouGoTimeBased(**{
-    "data": {
+request_body = ContractToCreateContainerPayAsYouGoTimeBased(
+    data={
         "title": "title",
         "country_code": "US",
         "state_code": "state_code",
         "scope_of_work": "scope_of_work",
         "special_clause": "special_clause",
         "termination_date": "1999-12-31",
         "client": {
@@ -2003,50 +3569,50 @@
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
-            "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "sedDuis officia est laborum in"
+            "id_": "id",
+            "name": "in labore officia non veniam"
         },
         "seniority": {
-            "id_": "00000000-0000-0000-0000-000000000000"
+            "id_": 5.48
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "occae",
+            "expected_email": "adipisicing",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "pay_as_you_go_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 2.6,
+            "amount": 0.13,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
             "first_payment_date": "1999-12-31",
             "first_payment": 500,
             "notice_period": 15,
             "scale": "hourly"
         }
     }
-})
+)
 
 result = sdk.contractors.create_contract_time_based(request_body=request_body)
 
 print(result)
 ```
 
 #### **create_contract_task_based**
@@ -2072,16 +3638,16 @@
 from deel_sdk.models import ContractToCreateContainerPaygTasks
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToCreateContainerPaygTasks(**{
-    "data": {
+request_body = ContractToCreateContainerPaygTasks(
+    data={
         "title": "title",
         "country_code": "US",
         "state_code": "state_code",
         "scope_of_work": "scope_of_work",
         "special_clause": "special_clause",
         "termination_date": "1999-12-31",
         "client": {
@@ -2089,29 +3655,29 @@
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
-            "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "enim irure dolore magna"
+            "id_": "id",
+            "name": "irure"
         },
         "seniority": {
-            "id_": "00000000-0000-0000-0000-000000000000"
+            "id_": 5.89
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "Duis nulla oc",
+            "expected_email": "in Ex",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "payg_tasks",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 100,
@@ -2123,15 +3689,15 @@
             "payment_due_days": 7,
             "pay_before_weekends": True,
             "first_payment_date": "1999-12-31",
             "first_payment": 500,
             "notice_period": 15
         }
     }
-})
+)
 
 result = sdk.contractors.create_contract_task_based(request_body=request_body)
 
 print(result)
 ```
 
 #### **create_contract_milestone_based**
@@ -2157,16 +3723,16 @@
 from deel_sdk.models import ContractToCreateContainerPaygMilestones
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToCreateContainerPaygMilestones(**{
-    "data": {
+request_body = ContractToCreateContainerPaygMilestones(
+    data={
         "title": "title",
         "country_code": "US",
         "state_code": "state_code",
         "scope_of_work": "scope_of_work",
         "special_clause": "special_clause",
         "termination_date": "1999-12-31",
         "client": {
@@ -2174,29 +3740,29 @@
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
-            "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "et dolore"
+            "id_": "id",
+            "name": "pariatur"
         },
         "seniority": {
-            "id_": "00000000-0000-0000-0000-000000000000"
+            "id_": 8.01
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "sint ",
+            "expected_email": "aute dolor",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "payg_milestones",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 100,
@@ -2208,15 +3774,15 @@
             "payment_due_days": 7,
             "pay_before_weekends": True,
             "first_payment_date": "1999-12-31",
             "first_payment": 500,
             "notice_period": 15
         }
     }
-})
+)
 
 result = sdk.contractors.create_contract_milestone_based(request_body=request_body)
 
 print(result)
 ```
 
 #### **create_contract_fixed_rate**
@@ -2242,16 +3808,16 @@
 from deel_sdk.models import ContractToCreateContainerOngoingTimeBased
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToCreateContainerOngoingTimeBased(**{
-    "data": {
+request_body = ContractToCreateContainerOngoingTimeBased(
+    data={
         "title": "title",
         "country_code": "US",
         "state_code": "state_code",
         "scope_of_work": "scope_of_work",
         "special_clause": "special_clause",
         "termination_date": "1999-12-31",
         "client": {
@@ -2259,50 +3825,50 @@
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
-            "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "cillum"
+            "id_": "id",
+            "name": "proident fugiat est aliquip elit"
         },
         "seniority": {
-            "id_": "00000000-0000-0000-0000-000000000000"
+            "id_": 6.6
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "Lorem sint et",
+            "expected_email": "nisiet lab",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "ongoing_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 7.36,
+            "amount": 9.2,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
             "first_payment_date": "1999-12-31",
             "first_payment": 500,
             "notice_period": 15,
             "scale": "hourly"
         }
     }
-})
+)
 
 result = sdk.contractors.create_contract_fixed_rate(request_body=request_body)
 
 print(result)
 ```
 
 #### **create_contract**
@@ -2328,16 +3894,16 @@
 from deel_sdk.models import ContractToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToCreateContainer(**{
-    "data": {
+request_body = ContractToCreateContainer(
+    data={
         "title": "title",
         "country_code": "US",
         "state_code": "state_code",
         "scope_of_work": "scope_of_work",
         "special_clause": "special_clause",
         "termination_date": "1999-12-31",
         "client": {
@@ -2345,50 +3911,50 @@
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
-            "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "sedDuis officia est laborum in"
+            "id_": "id",
+            "name": "in labore officia non veniam"
         },
         "seniority": {
-            "id_": "00000000-0000-0000-0000-000000000000"
+            "id_": 5.48
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "occae",
+            "expected_email": "adipisicing",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "pay_as_you_go_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 2.6,
+            "amount": 0.13,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
             "first_payment_date": "1999-12-31",
             "first_payment": 500,
             "notice_period": 15,
             "scale": "hourly"
         }
     }
-})
+)
 
 result = sdk.contractors.create_contract(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_contract_preview**
@@ -2451,35 +4017,35 @@
 from deel_sdk.models import ContractToAmendDetailsContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToAmendDetailsContainer(**{
-    "data": {
+request_body = ContractToAmendDetailsContainer(
+    data={
         "amount": 100,
         "currency_code": "GBP",
         "scale": "hourly",
         "effective_date": "1999-12-31",
         "first_payment_date": "1999-12-31",
-        "first_payment": 0.24,
+        "first_payment": 4.5,
         "frequency": "weekly",
-        "cycle_end": 24.94,
+        "cycle_end": 3.38,
         "cycle_end_type": "DAY_OF_WEEK",
         "payment_due_type": "REGULAR",
-        "payment_due_days": 0.92,
-        "pay_before_weekends": True,
+        "payment_due_days": 83.14,
+        "pay_before_weekends": False,
         "job_title_name": "3D Designer",
         "job_title_id": "00000000-0000-0000-0000-000000000000",
         "seniority_id": "00000000-0000-0000-0000-000000000000",
         "special_clause": "special_clause",
         "scope_of_work": "scope_of_work"
     }
-})
+)
 
 result = sdk.contractors.amend_contract_details(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -2509,21 +4075,21 @@
 from deel_sdk.models import ContractToTerminateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = ContractToTerminateContainer(**{
-    "data": {
+request_body = ContractToTerminateContainer(
+    data={
         "completion_date": "1999-12-31",
         "terminate_now": True,
         "message": "message"
     }
-})
+)
 
 result = sdk.contractors.terminate_contract(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -2553,20 +4119,20 @@
 from deel_sdk.models import PremiumToAddContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = PremiumToAddContainer(**{
-    "data": {
+request_body = PremiumToAddContainer(
+    data={
         "agreement_reflects_relation": True,
         "contractor_characteristics": True
     }
-})
+)
 
 result = sdk.contractors.add_premium(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -2647,20 +4213,20 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = {
     "data": {
         "contract_id": "m3jk2j",
-        "amount": "cupidatat exe",
+        "amount": "labore",
         "date_of_adjustment": "1999-12-31",
         "title": "Your title here",
         "description": "Your description here",
         "cycle_reference": "my_cycle_reference",
-        "file": "qu",
+        "file": "ut",
         "adjustment_category_id": "c9cf4c2c0165f48f494415390c3b49",
         "move_next_cycle": True,
         "vendor": "Vendor",
         "country": "US"
     }
 }
 
@@ -2724,22 +4290,22 @@
 from deel_sdk.models import AdjustmentToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = AdjustmentToUpdateContainer(**{
-    "data": {
-        "amount": "ut velit in",
+request_body = AdjustmentToUpdateContainer(
+    data={
+        "amount": "ad aute d",
         "title": "Your title here",
         "description": "Your description here",
-        "file": "incididunt "
+        "file": "in ulla"
     }
-})
+)
 
 result = sdk.adjustments.update_adjustment(
     request_body=request_body,
     adjustment_id="adjustment_id"
 )
 
 print(result)
@@ -2829,19 +4395,19 @@
 from deel_sdk.models import InputToCreateFileRef
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = InputToCreateFileRef(**{
-    "data": {
+request_body = InputToCreateFileRef(
+    data={
         "content_type": "application/pdf"
     }
-})
+)
 
 result = sdk.adjustments.create_file_ref(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_adjustments**
@@ -2913,29 +4479,29 @@
 from deel_sdk.models import CandidateToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CandidateToCreateContainer(**{
-    "data": {
+request_body = CandidateToCreateContainer(
+    data={
         "id_": "id",
         "first_name": "John",
         "last_name": "Doe",
         "status": "offer-accepted",
         "start_date": "1999-12-31",
         "link": "link",
         "job_title": "3D Designer",
-        "email": "dolore",
+        "email": "do te",
         "nationality": "US",
         "country": "US",
         "state": "AL"
     }
-})
+)
 
 result = sdk.candidates.add_candidate(request_body=request_body)
 
 print(result)
 ```
 
 #### **patch_candidate**
@@ -2962,28 +4528,28 @@
 from deel_sdk.models import CandidateToPatchContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CandidateToPatchContainer(**{
-    "data": {
+request_body = CandidateToPatchContainer(
+    data={
         "first_name": "John",
         "last_name": "Doe",
         "status": "offer-accepted",
         "start_date": "1999-12-31",
         "job_title": "3D Designer",
         "link": "link",
-        "email": "Excepteur nu",
+        "email": "dolor",
         "nationality": "US",
         "country": "US",
         "state": "AL"
     }
-})
+)
 
 result = sdk.candidates.patch_candidate(
     request_body=request_body,
     candidate_id="candidate_id"
 )
 
 print(result)
@@ -3037,17 +4603,17 @@
 from deel_sdk.models import AdditionalEorInfoContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = AdditionalEorInfoContainer(**{
-    "data": ""
-})
+request_body = AdditionalEorInfoContainer(
+    data=""
+)
 
 result = sdk.partner_managed.add_employee_additional_information(
     request_body=request_body,
     employee_id="employee_id",
     contract_id="contract_id"
 )
 
@@ -3079,19 +4645,19 @@
 from deel_sdk.models import EmployeeContractSignatureToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = EmployeeContractSignatureToCreateContainer(**{
-    "data": {
-        "signature": "aliqua sed comm"
+request_body = EmployeeContractSignatureToCreateContainer(
+    data={
+        "signature": "cil"
     }
-})
+)
 
 result = sdk.partner_managed.sign_employee_contract(
     request_body=request_body,
     employee_id="employee_id",
     contract_id="contract_id"
 )
 
@@ -3123,21 +4689,21 @@
 from deel_sdk.models import RequestCustomVerificationLetterContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = RequestCustomVerificationLetterContainer(**{
-    "data": {
-        "description": "magnaest ea con",
+request_body = RequestCustomVerificationLetterContainer(
+    data={
+        "description": "ipsum suntullam",
         "include_qr_code": True,
         "type_": "VISA_APPLICATION_FOR_PERSONAL_TRIP"
     }
-})
+)
 
 result = sdk.partner_managed.request_custom_verification_letter(
     request_body=request_body,
     employee_id="employee_id",
     contract_id="contract_id"
 )
 
@@ -3206,15 +4772,15 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.partner_managed.download_hr_verification_letters_and_documents(
     employee_id="employee_id",
     contract_id="contract_id",
-    document_id=1.72
+    document_id=2.54
 )
 
 print(result)
 ```
 
 #### **get_offer_letter_preview**
 
@@ -3378,22 +4944,22 @@
 from deel_sdk.models import BankAccountToAddContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = BankAccountToAddContainer(**{
-    "data": [
+request_body = BankAccountToAddContainer(
+    data=[
         {
             "key": "key",
             "value": "value"
         }
     ]
-})
+)
 
 result = sdk.partner_managed.add_bank_account(
     request_body=request_body,
     employee_id="employee_id"
 )
 
 print(result)
@@ -3424,22 +4990,22 @@
 from deel_sdk.models import BankAccountToAddContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = BankAccountToAddContainer(**{
-    "data": [
+request_body = BankAccountToAddContainer(
+    data=[
         {
             "key": "key",
             "value": "value"
         }
     ]
-})
+)
 
 result = sdk.partner_managed.patch_bank_account(
     request_body=request_body,
     employee_id="employee_id",
     bank_id="bank_id"
 )
 
@@ -3540,15 +5106,15 @@
 request_body = {
     "file": "file"
 }
 
 result = sdk.partner_managed.upload_employee_compliance_document(
     request_body=request_body,
     employee_id="employee_id",
-    document_id=1.36
+    document_id=7.6
 )
 
 print(result)
 ```
 
 #### **get_employee_compliance_document_template**
 
@@ -3575,15 +5141,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.partner_managed.get_employee_compliance_document_template(
     employee_id="employee_id",
-    document_id=5.91
+    document_id=4.09
 )
 
 print(result)
 ```
 
 #### **get_employee_tax_documents**
 
@@ -3612,592 +5178,14 @@
 )
 
 result = sdk.partner_managed.get_employee_tax_documents(employee_id="employee_id")
 
 print(result)
 ```
 
-### ContractsService
-
-A list of all methods in the `ContractsService` service. Click on the method name to view detailed information about that method.
-
-| Methods                                                                     | Description                                                                                                                                                                                                          |
-| :-------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| [get_contract_list](#get_contract_list)                                     | Retrieve a list of contracts.                                                                                                                                                                                        |
-| [get_contract_by_id](#get_contract_by_id)                                   | Retrieve a single contract.                                                                                                                                                                                          |
-| [attach_external_id](#attach_external_id)                                   | Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later. |
-| [add_contract_document](#add_contract_document)                             | Attach a file to contract document.                                                                                                                                                                                  |
-| [edit_contract_document](#edit_contract_document)                           | Overwrite the file currently attached to contract document.                                                                                                                                                          |
-| [get_alternate_emails_by_contract_id](#get_alternate_emails_by_contract_id) | Returns an array of alternate email objects                                                                                                                                                                          |
-| [sign_contract](#sign_contract)                                             | Sign a contract as a client.                                                                                                                                                                                         |
-| [invite_to_sign_contract](#invite_to_sign_contract)                         | Invite a worker to sign the contract. Worker will be notified via email.                                                                                                                                             |
-| [uninvite_to_sign_contract](#uninvite_to_sign_contract)                     | Remove invite in order to re-invite a worker to sign the contract.                                                                                                                                                   |
-| [calculate_final_payment](#calculate_final_payment)                         | Calculate the final payment due to the contractor when ending the contract.                                                                                                                                          |
-| [post_contract_estimate](#post_contract_estimate)                           | First payment is calculated from the number of working/calendar days between their start date and the start of the payment cycle.                                                                                    |
-| [get_contract_templates](#get_contract_templates)                           | Retrieve a list of contract templates in your organization.                                                                                                                                                          |
-| [get_worker_documents_by_id](#get_worker_documents_by_id)                   | Retrieve a list of documents of a worker.                                                                                                                                                                            |
-| [get_download_worker_documents_by_id](#get_download_worker_documents_by_id) | Get the download link of worker document.                                                                                                                                                                            |
-
-#### **get_contract_list**
-
-Retrieve a list of contracts.
-
-- HTTP Method: `GET`
-- Endpoint: `/contracts`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| after_cursor | str | ❌ | Retrieve a list of contracts. |
-| limit | float | ❌ | Retrieve a list of contracts. |
-| order_direction | SortDirEnum | ❌ | Retrieve a list of contracts. |
-| types | List[ContractTypeEnum] | ❌ | Retrieve a list of contracts. |
-| statuses | List[ContractStatusEnum] | ❌ | Retrieve a list of contracts. |
-| team_id | str | ❌ | Retrieve a list of contracts. |
-| external_id | str | ❌ | Retrieve a list of contracts. |
-| countries | List[str] | ❌ | Retrieve a list of contracts. |
-| currencies | GetContractListCurrencies | ❌ | Retrieve a list of contracts. |
-| search | str | ❌ | Retrieve a list of contracts. |
-| sort_by | ContractsSortByEnum | ❌ | Retrieve a list of contracts. |
-
-**Return Type**
-
-`ContractListContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import SortDirEnum, GetContractListCurrencies, ContractsSortByEnum
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-types=[
-    "ongoing_time_based"
-]
-statuses=[
-    "new"
-]
-countries=[
-    "US"
-]
-currencies=GetContractListCurrencies(**[
-    "GBP"
-])
-
-result = sdk.contracts.get_contract_list(
-    after_cursor="after_cursor",
-    limit=10,
-    order_direction="asc",
-    types=types,
-    statuses=statuses,
-    team_id="team_id",
-    external_id="external_id",
-    countries=countries,
-    currencies=currencies,
-    search="search",
-    sort_by="contract_title"
-)
-
-print(result)
-```
-
-#### **get_contract_by_id**
-
-Retrieve a single contract.
-
-- HTTP Method: `GET`
-- Endpoint: `/contracts/{contract_id}`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| contract_id | str | ✅ | Retrieve a single contract. |
-
-**Return Type**
-
-`ContractContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.get_contract_by_id(contract_id="contract_id")
-
-print(result)
-```
-
-#### **attach_external_id**
-
-Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later.
-
-- HTTP Method: `PATCH`
-- Endpoint: `/contracts/{contract_id}`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | InputToPatchContractExternalId | ✅ | The request body. |
-| contract_id | str | ✅ | Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later. |
-
-**Return Type**
-
-`GenericResultCreated`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import InputToPatchContractExternalId
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-request_body = InputToPatchContractExternalId(**{
-    "data": {
-        "external_id": "external_id"
-    }
-})
-
-result = sdk.contracts.attach_external_id(
-    request_body=request_body,
-    contract_id="contract_id"
-)
-
-print(result)
-```
-
-#### **add_contract_document**
-
-Attach a file to contract document.
-
-- HTTP Method: `POST`
-- Endpoint: `/contracts/{contract_id}/documents`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | dict | ❌ | The request body. |
-| contract_id | str | ✅ | Attach a file to contract document. |
-
-**Return Type**
-
-`ContractDocumentContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import FileObject
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-request_body = {
-    "file": "file"
-}
-
-result = sdk.contracts.add_contract_document(
-    request_body=request_body,
-    contract_id="contract_id"
-)
-
-print(result)
-```
-
-#### **edit_contract_document**
-
-Overwrite the file currently attached to contract document.
-
-- HTTP Method: `PUT`
-- Endpoint: `/contracts/{contract_id}/documents`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | dict | ❌ | The request body. |
-| contract_id | str | ✅ | Overwrite the file currently attached to contract document. |
-
-**Return Type**
-
-`ContractDocumentContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import FileObject
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-request_body = {
-    "file": "file"
-}
-
-result = sdk.contracts.edit_contract_document(
-    request_body=request_body,
-    contract_id="contract_id"
-)
-
-print(result)
-```
-
-#### **get_alternate_emails_by_contract_id**
-
-Returns an array of alternate email objects
-
-- HTTP Method: `GET`
-- Endpoint: `/contracts/{contract_id}/alternate_emails`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| contract_id | str | ✅ | Returns an array of alternate email objects |
-
-**Return Type**
-
-`List[AlternateEmailItem]`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.get_alternate_emails_by_contract_id(contract_id="contract_id")
-
-print(result)
-```
-
-#### **sign_contract**
-
-Sign a contract as a client.
-
-- HTTP Method: `POST`
-- Endpoint: `/contracts/{contract_id}/signatures`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | ContractSignatureToCreateContainer | ✅ | The request body. |
-| contract_id | str | ✅ | Sign a contract as a client. |
-
-**Return Type**
-
-`GenericResultCreated`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import ContractSignatureToCreateContainer
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-request_body = ContractSignatureToCreateContainer(**{
-    "data": {
-        "client_signature": "ea exercitat",
-        "contract_template_id": 8.35
-    }
-})
-
-result = sdk.contracts.sign_contract(
-    request_body=request_body,
-    contract_id="contract_id"
-)
-
-print(result)
-```
-
-#### **invite_to_sign_contract**
-
-Invite a worker to sign the contract. Worker will be notified via email.
-
-- HTTP Method: `POST`
-- Endpoint: `/contracts/{contract_id}/invitations`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | ContractInvitationToCreateContainer | ✅ | The request body. |
-| contract_id | str | ✅ | Invite a worker to sign the contract. Worker will be notified via email. |
-
-**Return Type**
-
-`GenericResultCreated`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import ContractInvitationToCreateContainer
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-request_body = ContractInvitationToCreateContainer(**{
-    "data": {
-        "email": "eiusm",
-        "message": "officia ut"
-    }
-})
-
-result = sdk.contracts.invite_to_sign_contract(
-    request_body=request_body,
-    contract_id="contract_id"
-)
-
-print(result)
-```
-
-#### **uninvite_to_sign_contract**
-
-Remove invite in order to re-invite a worker to sign the contract.
-
-- HTTP Method: `DELETE`
-- Endpoint: `/contracts/{contract_id}/invitations`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| contract_id | str | ✅ | Remove invite in order to re-invite a worker to sign the contract. |
-
-**Return Type**
-
-`GenericResultDeleted`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.uninvite_to_sign_contract(contract_id="contract_id")
-
-print(result)
-```
-
-#### **calculate_final_payment**
-
-Calculate the final payment due to the contractor when ending the contract.
-
-- HTTP Method: `GET`
-- Endpoint: `/contracts/{contract_id}/final-payments`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| contract_id | str | ✅ | Calculate the final payment due to the contractor when ending the contract. |
-| end_date | str | ❌ | Calculate the final payment due to the contractor when ending the contract. |
-| calculation_type | CalculateFinalPaymentCalculationType | ❌ | Calculate the final payment due to the contractor when ending the contract. |
-| workweek_start | str | ❌ | Calculate the final payment due to the contractor when ending the contract. |
-| workweek_end | str | ❌ | Calculate the final payment due to the contractor when ending the contract. |
-
-**Return Type**
-
-`FinalPaymentCalculatedContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import CalculateFinalPaymentCalculationType
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.calculate_final_payment(
-    contract_id="contract_id",
-    end_date="1999-12-31",
-    calculation_type="CUSTOM_AMOUNT",
-    workweek_start="workweek_start",
-    workweek_end="workweek_end"
-)
-
-print(result)
-```
-
-#### **post_contract_estimate**
-
-First payment is calculated from the number of working/calendar days between their start date and the start of the payment cycle.
-
-- HTTP Method: `POST`
-- Endpoint: `/contracts/estimate`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| request_body | EstimateFirstPaymentContainer | ✅ | The request body. |
-
-**Return Type**
-
-`ResponseEstimateFirstPaymentContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import EstimateFirstPaymentContainer
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-request_body = EstimateFirstPaymentContainer(**{
-    "data": {
-        "type_": "ongoing_time_based",
-        "country_code": "US",
-        "start_date": "1999-12-31",
-        "compensation_details": {
-            "amount": 2500,
-            "currency_code": "GBP",
-            "scale": "weekly",
-            "cycle_end": 30.28,
-            "cycle_end_type": "DAY_OF_WEEK",
-            "payment_due_type": "REGULAR",
-            "payment_due_days": 11.81,
-            "calculation_type": "CUSTOM_AMOUNT",
-            "work_week_start": "Sunday",
-            "work_week_end": "Sunday"
-        }
-    }
-})
-
-result = sdk.contracts.post_contract_estimate(request_body=request_body)
-
-print(result)
-```
-
-#### **get_contract_templates**
-
-Retrieve a list of contract templates in your organization.
-
-- HTTP Method: `GET`
-- Endpoint: `/contract-templates`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-
-**Return Type**
-
-`ContractTemplateListContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.get_contract_templates()
-
-print(result)
-```
-
-#### **get_worker_documents_by_id**
-
-Retrieve a list of documents of a worker.
-
-- HTTP Method: `GET`
-- Endpoint: `/workers/{worker_id}/documents`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| worker_id | str | ✅ | Retrieve a list of documents of a worker. |
-
-**Return Type**
-
-`WorkerDocumentsByIdContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.get_worker_documents_by_id(worker_id="worker_id")
-
-print(result)
-```
-
-#### **get_download_worker_documents_by_id**
-
-Get the download link of worker document.
-
-- HTTP Method: `GET`
-- Endpoint: `/workers/{worker_id}/documents/{document_id}/download`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| worker_id | str | ✅ | Get the download link of worker document. |
-| document_id | float | ✅ | Get the download link of worker document. |
-
-**Return Type**
-
-`DownloadWorkerDocumentsByIdContainer`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.get_download_worker_documents_by_id(
-    worker_id="worker_id",
-    document_id=8.43
-)
-
-print(result)
-```
-
 ### TasksService
 
 A list of all methods in the `TasksService` service. Click on the method name to view detailed information about that method.
 
 | Methods                                               | Description                                                     |
 | :---------------------------------------------------- | :-------------------------------------------------------------- |
 | [get_tasks_by_contract](#get_tasks_by_contract)       | Retrieve a list of tasks for a given contract.                  |
@@ -4261,25 +5249,25 @@
 from deel_sdk.models import InputToCreatePgoTask
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = InputToCreatePgoTask(**{
-    "data": {
+request_body = InputToCreatePgoTask(
+    data={
         "amount": "123.45",
         "date_submitted": "1999-12-31",
         "description": "Make the button pop.",
         "attachment": {
             "filename": "filename",
             "key": "key"
         }
     }
-})
+)
 
 result = sdk.tasks.create_contract_pgo_tak(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -4309,23 +5297,23 @@
 from deel_sdk.models import RequestBodyToCreatePgoTaskReviewsReviewsContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = RequestBodyToCreatePgoTaskReviewsReviewsContainer(**{
-    "data": {
+request_body = RequestBodyToCreatePgoTaskReviewsReviewsContainer(
+    data={
         "status": "approved",
         "reason": "Great work.",
         "ids": [
             "00000000-0000-0000-0000-000000000000"
         ]
     }
-})
+)
 
 result = sdk.tasks.create_task_many_review(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -4356,20 +5344,20 @@
 from deel_sdk.models import RequestBodyToCreatePgoTaskReviewsByIdReviewsContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = RequestBodyToCreatePgoTaskReviewsByIdReviewsContainer(**{
-    "data": {
+request_body = RequestBodyToCreatePgoTaskReviewsByIdReviewsContainer(
+    data={
         "status": "approved",
         "reason": "Excited!"
     }
-})
+)
 
 result = sdk.tasks.create_task_review_by_id(
     request_body=request_body,
     contract_id="contract_id",
     task_id="task_id"
 )
 
@@ -4471,15 +5459,15 @@
     contract_id="contract_id",
     contract_types=contract_types,
     statuses=statuses,
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=99,
-    offset=564786626.18
+    offset=38650248.43
 )
 
 print(result)
 ```
 
 #### **get_timesheets**
 
@@ -4524,15 +5512,15 @@
     contract_id="contract_id",
     contract_types=contract_types,
     statuses=statuses,
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=99,
-    offset=911169937.96
+    offset=530446812.74
 )
 
 print(result)
 ```
 
 #### **create_timesheet**
 
@@ -4557,22 +5545,22 @@
 from deel_sdk.models import TimesheetToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TimesheetToCreateContainer(**{
-    "data": {
+request_body = TimesheetToCreateContainer(
+    data={
         "contract_id": "contract_id",
         "description": "description",
         "date_submitted": "1999-12-31",
         "quantity": 2
     }
-})
+)
 
 result = sdk.timesheets.create_timesheet(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_timesheet_by_id**
@@ -4630,20 +5618,20 @@
 from deel_sdk.models import TimesheetToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TimesheetToUpdateContainer(**{
-    "data": {
+request_body = TimesheetToUpdateContainer(
+    data={
         "description": "description",
-        "quantity": 3.77
+        "quantity": 8.4
     }
-})
+)
 
 result = sdk.timesheets.update_timesheet_by_id(
     request_body=request_body,
     timesheet_id="timesheet_id"
 )
 
 print(result)
@@ -4708,20 +5696,20 @@
 from deel_sdk.models import TimesheetReviewToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TimesheetReviewToCreateContainer(**{
-    "data": {
+request_body = TimesheetReviewToCreateContainer(
+    data={
         "status": "approved",
         "reason": "reason"
     }
-})
+)
 
 result = sdk.timesheets.create_timesheet_review(
     request_body=request_body,
     timesheet_id="timesheet_id"
 )
 
 print(result)
@@ -4750,23 +5738,23 @@
 from deel_sdk.models import TimesheetReviewsToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TimesheetReviewsToCreateContainer(**{
-    "data": {
+request_body = TimesheetReviewsToCreateContainer(
+    data={
         "status": "approved",
         "reason": "reason",
         "ids": [
-            1.77
+            8.09
         ]
     }
-})
+)
 
 result = sdk.timesheets.create_timesheet_reviews(request_body=request_body)
 
 print(result)
 ```
 
 ### MilestonesService
@@ -4837,21 +5825,21 @@
 from deel_sdk.models import MilestoneToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = MilestoneToCreateContainer(**{
-    "data": {
+request_body = MilestoneToCreateContainer(
+    data={
         "amount": "900.00",
         "title": "Sprint 2",
         "description": "Sprint #2"
     }
-})
+)
 
 result = sdk.milestones.create_milestone(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -4952,20 +5940,20 @@
 from deel_sdk.models import MilestoneReviewToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = MilestoneReviewToCreateContainer(**{
-    "data": {
+request_body = MilestoneReviewToCreateContainer(
+    data={
         "status": "approved",
         "reason": "reason"
     }
-})
+)
 
 result = sdk.milestones.create_milestone_review(
     request_body=request_body,
     contract_id="contract_id",
     milestone_id="milestone_id"
 )
 
@@ -4996,23 +5984,23 @@
 from deel_sdk.models import MilestoneReviewsToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = MilestoneReviewsToCreateContainer(**{
-    "data": {
+request_body = MilestoneReviewsToCreateContainer(
+    data={
         "status": "approved",
         "reason": "reason",
         "ids": [
-            6.78
+            "00000000-0000-0000-0000-000000000000"
         ]
     }
-})
+)
 
 result = sdk.milestones.create_milestone_reviews(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -5083,21 +6071,21 @@
 from deel_sdk.models import OffCyclePaymentToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = OffCyclePaymentToCreateContainer(**{
-    "data": {
+request_body = OffCyclePaymentToCreateContainer(
+    data={
         "date_submitted": "1999-12-31",
         "amount": 2500,
         "description": "description"
     }
-})
+)
 
 result = sdk.off_cycle_payments.create_off_cycle_payment(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -5207,26 +6195,26 @@
 from deel_sdk.models import CreateTimeoffContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CreateTimeoffContainer(**{
-    "data": {
+request_body = CreateTimeoffContainer(
+    data={
         "type_": "VACATION",
         "start_date": "2022-09-03T00:00:00.000Z",
         "end_date": "2022-09-05T00:00:00.000Z",
         "with_multiple_dates": True,
         "reason": "Holiday",
-        "is_start_date_half_day": True,
+        "is_start_date_half_day": False,
         "is_end_date_half_day": False,
         "other_timeoff_name": "Birthday"
     }
-})
+)
 
 result = sdk.time_off.create_eor_time_offs(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
@@ -5257,26 +6245,26 @@
 from deel_sdk.models import CreateTimeoffContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CreateTimeoffContainer(**{
-    "data": {
+request_body = CreateTimeoffContainer(
+    data={
         "type_": "VACATION",
         "start_date": "2022-09-03T00:00:00.000Z",
         "end_date": "2022-09-05T00:00:00.000Z",
         "with_multiple_dates": True,
         "reason": "Holiday",
-        "is_start_date_half_day": True,
+        "is_start_date_half_day": False,
         "is_end_date_half_day": False,
         "other_timeoff_name": "Birthday"
     }
-})
+)
 
 result = sdk.time_off.edit_eor_time_offs(
     request_body=request_body,
     contract_id="contract_id",
     timeoff_id="timeoff_id"
 )
 
@@ -5403,20 +6391,20 @@
 from deel_sdk.models import TimeoffToReviewContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TimeoffToReviewContainer(**{
-    "data": {
+request_body = TimeoffToReviewContainer(
+    data={
         "is_approved": True,
         "denial_reason": "Not allowed for this day."
     }
-})
+)
 
 result = sdk.time_off.review_timeoff(
     request_body=request_body,
     timeoff_id="timeoff_id"
 )
 
 print(result)
@@ -5487,15 +6475,15 @@
     types=types,
     statuses=statuses,
     invoice_id="invoice_id",
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=10,
-    offset=226515477.25
+    offset=893166763.24
 )
 
 print(result)
 ```
 
 #### **get_invoice_adjustments**
 
@@ -5547,15 +6535,15 @@
     types=types,
     statuses=statuses,
     invoice_id="invoice_id",
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=10,
-    offset=240522187.51
+    offset=114760289.77
 )
 
 print(result)
 ```
 
 #### **create_invoice_adjustment**
 
@@ -5581,24 +6569,24 @@
 from deel_sdk.models import InvoiceAdjustmentToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = InvoiceAdjustmentToCreateContainer(**{
-    "data": {
+request_body = InvoiceAdjustmentToCreateContainer(
+    data={
         "contract_id": "contract_id",
         "date_submitted": "1999-12-31",
         "type_": "bonus",
         "amount": 2500,
         "description": "Bonus for being awesome.",
-        "payment_cycle_id": 6.69
+        "payment_cycle_id": 7.22
     }
-})
+)
 
 result = sdk.invoices.create_invoice_adjustment(
     request_body=request_body,
     recurring=False
 )
 
 print(result)
@@ -5628,20 +6616,20 @@
 from deel_sdk.models import InvoiceAdjustmentToUpdateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = InvoiceAdjustmentToUpdateContainer(**{
-    "data": {
-        "description": "sunt laborum Duis exercitation id",
-        "amount": 9.39
+request_body = InvoiceAdjustmentToUpdateContainer(
+    data={
+        "description": "nostrud ad ullamco dolor",
+        "amount": 9.38
     }
-})
+)
 
 result = sdk.invoices.update_invoice_adjustment_by_id(
     request_body=request_body,
     invoice_adjustment_id="invoice_adjustment_id"
 )
 
 print(result)
@@ -5706,20 +6694,20 @@
 from deel_sdk.models import InvoiceAdjustmentReviewToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = InvoiceAdjustmentReviewToCreateContainer(**{
-    "data": {
+request_body = InvoiceAdjustmentReviewToCreateContainer(
+    data={
         "status": "approved",
         "reason": "reason"
     }
-})
+)
 
 result = sdk.invoices.create_invoice_adjustment_review(
     request_body=request_body,
     invoice_adjustment_id="invoice_adjustment_id"
 )
 
 print(result)
@@ -5748,23 +6736,23 @@
 from deel_sdk.models import InvoiceAdjustmentReviewsToCreateContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = InvoiceAdjustmentReviewsToCreateContainer(**{
-    "data": {
+request_body = InvoiceAdjustmentReviewsToCreateContainer(
+    data={
         "status": "approved",
         "reason": "reason",
         "ids": [
-            1.77
+            8.09
         ]
     }
-})
+)
 
 result = sdk.invoices.create_invoice_adjustment_reviews(request_body=request_body)
 
 print(result)
 ```
 
 #### **get_invoice_adjustments_attachment**
@@ -6233,25 +7221,25 @@
 from deel_sdk.models import CreateWebhookRequest
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CreateWebhookRequest(**{
-    "name": "My first webhook.",
-    "description": "I like it very much.",
-    "status": "enabled",
-    "url": "https://mywebhook.com",
-    "signing_key": "signing_key",
-    "api_version": "v2",
-    "events": [
+request_body = CreateWebhookRequest(
+    name="My first webhook.",
+    description="I like it very much.",
+    status="enabled",
+    url="https://mywebhook.com",
+    signing_key="signing_key",
+    api_version="v2",
+    events=[
         "events"
     ]
-})
+)
 
 result = sdk.webhooks.create_webhook(request_body=request_body)
 
 print(result)
 ```
 
 #### **webhook_controller_get_by_id**
@@ -6309,25 +7297,25 @@
 from deel_sdk.models import PatchWebhookRequest
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = PatchWebhookRequest(**{
-    "name": "Demo webhook",
-    "description": "My first webhook",
-    "status": "enabled",
-    "url": "https://mywebhook.com/listening",
-    "signing_key": "signing_key",
-    "api_version": "v2",
-    "events": [
+request_body = PatchWebhookRequest(
+    name="Demo webhook",
+    description="My first webhook",
+    status="enabled",
+    url="https://mywebhook.com/listening",
+    signing_key="signing_key",
+    api_version="v2",
+    events=[
         "events"
     ]
-})
+)
 
 result = sdk.webhooks.webhook_controller_edit_by_id(
     request_body=request_body,
     id_="id"
 )
 
 print(result)
@@ -6421,21 +7409,21 @@
 from deel_sdk.models import CreatePublicTokenContainer
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CreatePublicTokenContainer(**{
-    "data": {
+request_body = CreatePublicTokenContainer(
+    data={
         "scope": [
             "contracts:read"
         ]
     }
-})
+)
 
 result = sdk.token.create_public_token(request_body=request_body)
 
 print(result)
 ```
 
 ### CartaService
```

### Comparing `deel_sdk-1.0.2/src/deel_sdk.egg-info/SOURCES.txt` & `deel_sdk-1.0.4/src/deel_sdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 src/deel_sdk/models/candidate_status_enum.py
 src/deel_sdk/models/candidate_to_create.py
 src/deel_sdk/models/candidate_to_create_container.py
 src/deel_sdk/models/candidate_to_patch.py
 src/deel_sdk/models/candidate_to_patch_container.py
 src/deel_sdk/models/client_of_basic_contract.py
 src/deel_sdk/models/client_of_contract.py
-src/deel_sdk/models/client_of_contract_legal_entity_5.py
+src/deel_sdk/models/client_of_contract_legal_entity_1.py
 src/deel_sdk/models/compensation_details_of_contract.py
 src/deel_sdk/models/compensation_details_of_contract_to_create_shared.py
 src/deel_sdk/models/contract.py
 src/deel_sdk/models/contract_container.py
 src/deel_sdk/models/contract_container_ongoing_time_based.py
 src/deel_sdk/models/contract_container_pay_as_you_go_time_based.py
 src/deel_sdk/models/contract_container_payg_milestones.py
@@ -107,16 +107,23 @@
 src/deel_sdk/models/create_admin_user_response_container.py
 src/deel_sdk/models/create_people_timeoff.py
 src/deel_sdk/models/create_public_token.py
 src/deel_sdk/models/create_public_token_container.py
 src/deel_sdk/models/create_timeoff.py
 src/deel_sdk/models/create_timeoff_container.py
 src/deel_sdk/models/create_webhook_request.py
+src/deel_sdk/models/created_exercise_equity_container.py
+src/deel_sdk/models/created_role_container.py
 src/deel_sdk/models/currency.py
 src/deel_sdk/models/currency_list_container.py
+src/deel_sdk/models/custom_field_item_container.py
+src/deel_sdk/models/custom_field_to_update_container.py
+src/deel_sdk/models/custom_field_values_container.py
+src/deel_sdk/models/custom_fields_list_container.py
+src/deel_sdk/models/custom_fields_object.py
 src/deel_sdk/models/deel_invoice.py
 src/deel_sdk/models/deel_invoice_list_container.py
 src/deel_sdk/models/departments.py
 src/deel_sdk/models/departments_container.py
 src/deel_sdk/models/download_worker_documents_by_id_container.py
 src/deel_sdk/models/email.py
 src/deel_sdk/models/employee.py
@@ -165,30 +172,37 @@
 src/deel_sdk/models/eor_timeoffs_container.py
 src/deel_sdk/models/eor_timeoffs_employee_item.py
 src/deel_sdk/models/eor_timeoffs_item_container.py
 src/deel_sdk/models/equity_stakeholder.py
 src/deel_sdk/models/equity_stakeholders_container.py
 src/deel_sdk/models/estimate_first_payment.py
 src/deel_sdk/models/estimate_first_payment_container.py
+src/deel_sdk/models/exercise_equity_to_create_container.py
+src/deel_sdk/models/exercise_equity_to_update_container.py
 src/deel_sdk/models/file_attachment_info.py
 src/deel_sdk/models/file_object.py
 src/deel_sdk/models/file_ref_type_enum.py
 src/deel_sdk/models/final_payment_calculated.py
 src/deel_sdk/models/final_payment_calculated_container.py
 src/deel_sdk/models/first_payment_date.py
 src/deel_sdk/models/generic_result_created.py
 src/deel_sdk/models/generic_result_created_with_id.py
 src/deel_sdk/models/generic_result_deleted.py
 src/deel_sdk/models/generic_result_updated.py
+src/deel_sdk/models/get_all_org_structures_container.py
 src/deel_sdk/models/get_contract_list_currencies.py
 src/deel_sdk/models/get_employee_compliance_document_template_download_link_container.py
 src/deel_sdk/models/get_employee_compliance_documents_container.py
+src/deel_sdk/models/get_hris_position_container.py
 src/deel_sdk/models/get_invoice_list_entities.py
+src/deel_sdk/models/get_org_structure_container.py
 src/deel_sdk/models/get_payment_list_currencies.py
 src/deel_sdk/models/get_payment_list_entities.py
+src/deel_sdk/models/get_roles_container.py
+src/deel_sdk/models/get_roles_item.py
 src/deel_sdk/models/global_payroll_g2_n_report.py
 src/deel_sdk/models/global_payroll_g2_n_report_container.py
 src/deel_sdk/models/gp_client.py
 src/deel_sdk/models/gp_contract_created.py
 src/deel_sdk/models/gp_contract_created_container.py
 src/deel_sdk/models/gp_contract_salary_scale_enum.py
 src/deel_sdk/models/gp_contract_salary_status_enum.py
@@ -221,14 +235,15 @@
 src/deel_sdk/models/hris_contract_part_time.py
 src/deel_sdk/models/hris_direct_employee.py
 src/deel_sdk/models/hris_direct_employee_container.py
 src/deel_sdk/models/hris_direct_employee_details.py
 src/deel_sdk/models/hris_direct_employee_response.py
 src/deel_sdk/models/hris_job_information_title_id.py
 src/deel_sdk/models/hris_job_information_title_name.py
+src/deel_sdk/models/hris_position_to_change_container.py
 src/deel_sdk/models/hris_team_information.py
 src/deel_sdk/models/identifier_value.py
 src/deel_sdk/models/input_to_create_file_ref.py
 src/deel_sdk/models/input_to_create_pgo_task.py
 src/deel_sdk/models/input_to_patch_contract_external_id.py
 src/deel_sdk/models/internal_people.py
 src/deel_sdk/models/internal_people_container.py
@@ -273,14 +288,16 @@
 src/deel_sdk/models/milestone_to_create_form_with_file.py
 src/deel_sdk/models/monthly_payment.py
 src/deel_sdk/models/off_cycle_payment.py
 src/deel_sdk/models/off_cycle_payment_container.py
 src/deel_sdk/models/off_cycle_payment_list_container.py
 src/deel_sdk/models/off_cycle_payment_to_create.py
 src/deel_sdk/models/off_cycle_payment_to_create_container.py
+src/deel_sdk/models/org_structure_to_create_container.py
+src/deel_sdk/models/org_structure_to_update_container.py
 src/deel_sdk/models/organization_list_container.py
 src/deel_sdk/models/output_to_create_file_ref.py
 src/deel_sdk/models/output_to_create_file_ref_container.py
 src/deel_sdk/models/page_info.py
 src/deel_sdk/models/page_info_without_cursor.py
 src/deel_sdk/models/page_info_without_cursor_new.py
 src/deel_sdk/models/patch_webhook_request.py
@@ -321,14 +338,16 @@
 src/deel_sdk/models/request_body_to_create_pgo_task_reviews_by_id_reviews_container.py
 src/deel_sdk/models/request_body_to_create_pgo_task_reviews_reviews_container.py
 src/deel_sdk/models/request_custom_verification_letter_container.py
 src/deel_sdk/models/request_custom_verification_letter_with_file.py
 src/deel_sdk/models/requester_time_off.py
 src/deel_sdk/models/response_estimate_first_payment.py
 src/deel_sdk/models/response_estimate_first_payment_container.py
+src/deel_sdk/models/role_to_create_container.py
+src/deel_sdk/models/role_to_update_container.py
 src/deel_sdk/models/salary_frequency_scale_enum.py
 src/deel_sdk/models/seniority.py
 src/deel_sdk/models/seniority_list_container.py
 src/deel_sdk/models/seniority_required.py
 src/deel_sdk/models/signatures_of_basic_contract.py
 src/deel_sdk/models/signatures_of_contract.py
 src/deel_sdk/models/sort_dir_enum.py
@@ -364,14 +383,16 @@
 src/deel_sdk/models/timesheet_to_create_container_with_file.py
 src/deel_sdk/models/timesheet_to_update.py
 src/deel_sdk/models/timesheet_to_update_container.py
 src/deel_sdk/models/update_worker_department.py
 src/deel_sdk/models/update_worker_department_container.py
 src/deel_sdk/models/update_worker_working_location.py
 src/deel_sdk/models/update_worker_working_location_container.py
+src/deel_sdk/models/updated_exercise_equity_container.py
+src/deel_sdk/models/updated_role_container.py
 src/deel_sdk/models/upload_employee_compliance_document_container.py
 src/deel_sdk/models/upload_employee_compliance_document_file_container.py
 src/deel_sdk/models/validation_type.py
 src/deel_sdk/models/validation_type_enum.py
 src/deel_sdk/models/webhook_event_type_list_response.py
 src/deel_sdk/models/webhook_event_type_response.py
 src/deel_sdk/models/webhook_item.py
@@ -421,24 +442,28 @@
 src/deel_sdk/services/__init__.py
 src/deel_sdk/services/accounting.py
 src/deel_sdk/services/adjustments.py
 src/deel_sdk/services/candidates.py
 src/deel_sdk/services/carta.py
 src/deel_sdk/services/contractors.py
 src/deel_sdk/services/contracts.py
+src/deel_sdk/services/custom_fields.py
 src/deel_sdk/services/eor.py
 src/deel_sdk/services/global_payroll.py
+src/deel_sdk/services/hris_organizations.py
 src/deel_sdk/services/invoices.py
 src/deel_sdk/services/lookups.py
 src/deel_sdk/services/managers.py
 src/deel_sdk/services/milestones.py
 src/deel_sdk/services/off_cycle_payments.py
+src/deel_sdk/services/organization_structure.py
 src/deel_sdk/services/organizations.py
 src/deel_sdk/services/partner_managed.py
 src/deel_sdk/services/people.py
+src/deel_sdk/services/positions.py
 src/deel_sdk/services/tasks.py
 src/deel_sdk/services/time_off.py
 src/deel_sdk/services/timesheets.py
 src/deel_sdk/services/token.py
 src/deel_sdk/services/webhooks.py
 src/deel_sdk/services/utils/base_service.py
 src/deel_sdk/services/utils/default_headers.py
```

