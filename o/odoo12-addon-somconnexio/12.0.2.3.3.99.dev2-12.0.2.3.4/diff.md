# Comparing `tmp/odoo12-addon-somconnexio-12.0.2.3.3.99.dev2.tar.gz` & `tmp/odoo12-addon-somconnexio-12.0.2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odoo12-addon-somconnexio-12.0.2.3.3.99.dev2.tar", last modified: Tue Jul 18 06:20:20 2023, max compression
+gzip compressed data, was "dist/odoo12-addon-somconnexio-12.0.2.3.4.tar", last modified: Wed Aug  2 15:19:59 2023, max compression
```

## Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2.tar` & `odoo12-addon-somconnexio-12.0.2.3.4.tar`

### file list

```diff
@@ -1,600 +1,605 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/
--rw-r--r--   0 root         (0) root         (0)     4980 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     4507 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/README.md
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9782 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/__manifest__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/controllers/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/controllers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5170 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/controllers/controllers.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/controllers/http.py
--rw-rw-rw-   0 root         (0) root         (0)     3458 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/controllers/public_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/correos_services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:19:40.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/correos_services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4432 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/correos_services/shipment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/
--rw-rw-rw-   0 root         (0) root         (0)    46993 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/account.account.template-sc.csv
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/account_chart_template_data.xml
--rw-rw-rw-   0 root         (0) root         (0)     2954 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/account_group.xml
--rw-rw-rw-   0 root         (0) root         (0)     2760 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/account_journal.xml
--rw-rw-rw-   0 root         (0) root         (0)     2599 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/account_payment_mode.xml
--rw-rw-rw-   0 root         (0) root         (0)     4496 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/account_payment_term.xml
--rw-rw-rw-   0 root         (0) root         (0)     1730 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/account_tax.xml
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/account_tax_group.xml
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/analytic_account.xml
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/base_automation.xml
--rw-rw-rw-   0 root         (0) root         (0)     2241 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/company.xml
--rw-rw-rw-   0 root         (0) root         (0)      703 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/contract_compute_current_tariff_cron.xml
--rw-rw-rw-   0 root         (0) root         (0)     3786 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/contract_terminate_reason.xml
--rw-rw-rw-   0 root         (0) root         (0)     2877 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/contract_terminate_user_reason.xml
--rw-rw-rw-   0 root         (0) root         (0)      947 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/crm_stage_data.xml
--rw-rw-rw-   0 root         (0) root         (0)      658 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/crm_track_correos_delivery_cron.xml
--rw-rw-rw-   0 root         (0) root         (0)     1238 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/discovery_channel.xml
--rw-rw-rw-   0 root         (0) root         (0)      752 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/fiber_signal_type_data.xml
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/hr_attendance_place.xml
--rw-rw-rw-   0 root         (0) root         (0)     1040 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/ir_config_pararameter.xml
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/ir_sequence.xml
--rw-rw-rw-   0 root         (0) root         (0)    13962 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/mail_activity_type.xml
--rw-rw-rw-   0 root         (0) root         (0)      150 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/mail_data.xml
--rw-rw-rw-   0 root         (0) root         (0)     3266 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/mail_mass_mailing_list_data.xml
--rw-rw-rw-   0 root         (0) root         (0)     2542 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/mis_report.xml
--rw-rw-rw-   0 root         (0) root         (0)     2532 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/operation_request_terminate_reason.xml
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/partner_action_tag_data.xml
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/partner_priority.xml
--rw-rw-rw-   0 root         (0) root         (0)    13582 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/previous_provider_data.xml
--rw-rw-rw-   0 root         (0) root         (0)     1459 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/product_attribute.xml
--rw-rw-rw-   0 root         (0) root         (0)     7767 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/product_attribute_value.xml
--rw-rw-rw-   0 root         (0) root         (0)     2455 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/product_categories.xml
--rw-rw-rw-   0 root         (0) root         (0)     7830 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/product_category_technology_supplier_data.xml
--rw-rw-rw-   0 root         (0) root         (0)    11481 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/product_pack_line.xml
--rw-rw-rw-   0 root         (0) root         (0)    41333 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/product_product.xml
--rw-rw-rw-   0 root         (0) root         (0)     5653 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/product_template_attribute_line_data.xml
--rw-rw-rw-   0 root         (0) root         (0)    11160 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/product_template_data.xml
--rw-rw-rw-   0 root         (0) root         (0)      413 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/res.partner.bank.xml
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/res.users.xml
--rw-rw-rw-   0 root         (0) root         (0)     3704 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/res_bank_data.xml
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/service_supplier.xml
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/service_technology.xml
--rw-rw-rw-   0 root         (0) root         (0)     1908 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/service_technology_service_supplier.xml
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/share_type.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/demo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/demo/contract/
--rw-rw-rw-   0 root         (0) root         (0)     2573 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/demo/contract/contract.xml
--rw-rw-rw-   0 root         (0) root         (0)     2666 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/demo/contract/contract_pack.xml
--rw-rw-rw-   0 root         (0) root         (0)     4018 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/demo/contract/contract_shared_data.xml
--rw-rw-rw-   0 root         (0) root         (0)     6655 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/demo/partner.xml
--rw-rw-rw-   0 root         (0) root         (0)     2749 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/demo/product.pricelist.csv
--rw-rw-rw-   0 root         (0) root         (0)     2346 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/demo/subscription_requests.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/helpers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:19:40.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/helpers/date.py
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/helpers/language.py
--rw-rw-rw-   0 root         (0) root         (0)     1846 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/i18n/
--rw-rw-rw-   0 root         (0) root         (0)   322385 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/i18n/ca_ES.po
--rw-rw-rw-   0 root         (0) root         (0)   331855 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/i18n/es.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/listeners/
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/listeners/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3078 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/listeners/contract_line_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     1210 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/listeners/contract_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/listeners/crm_lead_listener.py
--rw-rw-rw-   0 root         (0) root         (0)      742 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/listeners/partner_bank_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     1355 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/listeners/partner_listener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.8/pre-clean-mail-tracking-value.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.8.11/
--rw-rw-rw-   0 root         (0) root         (0)      423 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.8.11/post-create-copy-contract-service-info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.8.4/
--rw-rw-rw-   0 root         (0) root         (0)     2709 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.8.4/post-create-copy-contract-service-info.py
--rw-rw-rw-   0 root         (0) root         (0)     1750 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.8.4/pre-create-one-gb-wo-cost.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.9/
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.9/post-link-crm-to-contract.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.9/post-migrate-change-address.py
--rw-rw-rw-   0 root         (0) root         (0)      867 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.9/pre-migrate-change-address.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.9/pre-uniform-contracts-wo-number.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.9.13/
--rw-rw-rw-   0 root         (0) root         (0)     1215 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.9.13/post-change-activities-user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.9.2/
--rw-rw-rw-   0 root         (0) root         (0)      533 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.9.2/post-upper-sponsorship-code.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.9.9/
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.9.9/post-import-es-geonames.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.2.0.0/
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.2.0.0/post-recompute-is-from-pack.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.2.0.0/post-relate-is-from-not-pack-attribute-with-existing-products.py
--rw-rw-rw-   0 root         (0) root         (0)     1260 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-create-is-from-pack-attribute.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-set-xml-id-unlimited-20GB.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.2.1.6/
--rw-rw-rw-   0 root         (0) root         (0)     1191 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.2.1.6/post-set-state_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.2.1.8/
--rw-rw-rw-   0 root         (0) root         (0)      242 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.2.1.8/pre-assign-imd-manual-created-activity-types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.2.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     2293 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.2.2.0/pre-fix-catalog-externalId.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/erppeek/
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/erppeek/README.md
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/erppeek/erppeek.ini
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/erppeek/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)     1043 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/erppeek/update_contract_line_product_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/
--rw-rw-rw-   0 root         (0) root         (0)     1838 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/account_asset.py
--rw-rw-rw-   0 root         (0) root         (0)      931 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/account_banking_mandate.py
--rw-rw-rw-   0 root         (0) root         (0)     6377 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/account_invoice.py
--rw-rw-rw-   0 root         (0) root         (0)     2367 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/account_invoice_line.py
--rw-rw-rw-   0 root         (0) root         (0)      142 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/account_journal.py
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/account_move.py
--rw-rw-rw-   0 root         (0) root         (0)     3769 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/account_move_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1330 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/account_payment_order.py
--rw-rw-rw-   0 root         (0) root         (0)     1897 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/account_payment_return_email_gateway.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/account_tax.py
--rw-rw-rw-   0 root         (0) root         (0)    21169 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/aged_partner_balance.py
--rw-rw-rw-   0 root         (0) root         (0)     7108 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/aged_partner_balance_xlsx.py
--rw-rw-rw-   0 root         (0) root         (0)    40172 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/contract.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/contract_info/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/contract_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/contract_info/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3230 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/contract_info/broadband.py
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/contract_info/mobile.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/contract_terminate_reason.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/contract_terminate_user_reason.py
--rw-rw-rw-   0 root         (0) root         (0)     1232 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/coop_agreement.py
--rw-rw-rw-   0 root         (0) root         (0)    21856 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/crm_lead.py
--rw-rw-rw-   0 root         (0) root         (0)    11230 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/discovery_channel.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/fiber_signal_type.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/hr_attendance.py
--rw-rw-rw-   0 root         (0) root         (0)      200 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/hr_attendance_place.py
--rw-rw-rw-   0 root         (0) root         (0)     3864 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/hr_employee.py
--rw-rw-rw-   0 root         (0) root         (0)     4417 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/ir_model_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1578 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/ir_server_action.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/isp_info/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/isp_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3680 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/isp_info/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3644 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/isp_info/broadband.py
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/isp_info/mobile.py
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/l10n_es_aeat_report.py
--rw-rw-rw-   0 root         (0) root         (0)     3881 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/mail_activity.py
--rw-rw-rw-   0 root         (0) root         (0)      419 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/mail_thread.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/mass_mailing.py
--rw-rw-rw-   0 root         (0) root         (0)     2170 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/mobile_contract_otrs_view.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/opencell_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/operation_request.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/operation_request_terminate_reason.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/partner_action_tag.py
--rw-rw-rw-   0 root         (0) root         (0)     2816 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/partner_otrs_view.py
--rw-rw-rw-   0 root         (0) root         (0)     2038 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/payment_return.py
--rw-rw-rw-   0 root         (0) root         (0)     3407 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/payment_return_line.py
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/previous_provider.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/product_attribute_value.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/product_category_technology_supplier.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/product_pack_line.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/product_pricelist.py
--rw-rw-rw-   0 root         (0) root         (0)     5945 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/product_product.py
--rw-rw-rw-   0 root         (0) root         (0)      640 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/product_template.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/res_company.py
--rw-rw-rw-   0 root         (0) root         (0)    22511 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/res_partner.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/res_partner_bank.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/service_supplier.py
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/service_technology.py
--rw-rw-rw-   0 root         (0) root         (0)     2509 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/stock_move_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1818 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/stock_production_lot.py
--rw-rw-rw-   0 root         (0) root         (0)    12471 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/subscription_request.py
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/utm_source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_models/
--rw-rw-rw-   0 root         (0) root         (0)      366 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_models/access.py
--rw-rw-rw-   0 root         (0) root         (0)     1310 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_models/account_hierarchy_resource.py
--rw-rw-rw-   0 root         (0) root         (0)     5121 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_models/crm_account_hierarchy.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_models/customer.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_models/opencell_resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_models/opencell_types/
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_models/opencell_types/address.py
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_models/opencell_types/custom_field.py
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_models/opencell_types/description.py
--rw-rw-rw-   0 root         (0) root         (0)     1776 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_models/services.py
--rw-rw-rw-   0 root         (0) root         (0)     2144 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_models/subscription.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:19:40.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2730 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2944 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_strategies.py
--rw-rw-rw-   0 root         (0) root         (0)     3430 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_service.py
--rw-rw-rw-   0 root         (0) root         (0)     5227 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_strategies.py
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_services/customer_update_service.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_services/opencell_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_services/subscription_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/otrs_factories/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:19:40.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/otrs_factories/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/otrs_factories/adsl_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1152 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/otrs_factories/base_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     2508 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/otrs_factories/broadband_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/otrs_factories/customer_data_from_res_partner.py
--rw-rw-rw-   0 root         (0) root         (0)     2762 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/otrs_factories/fiber_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1749 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/otrs_factories/mobile_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/otrs_factories/router_4G_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)      999 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/otrs_factories/service_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/otrs_factories/update_ticket_with_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18705 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/account_asset_report_xls.py
--rw-rw-rw-   0 root         (0) root         (0)    20209 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/aged_partner_balance.xml
--rw-rw-rw-   0 root         (0) root         (0)     3285 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/crm_lead_creation_email_template.xml
--rw-rw-rw-   0 root         (0) root         (0)     1363 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/invoice_claim_1_capital_template.xml
--rw-rw-rw-   0 root         (0) root         (0)     1398 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/invoice_claim_1_template.xml
--rw-rw-rw-   0 root         (0) root         (0)     1969 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/mobile_can_be_linked_with_fiber_mail_template.xml
--rw-rw-rw-   0 root         (0) root         (0)     1957 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/mobile_linked_with_fiber_mail_template.xml
--rw-rw-rw-   0 root         (0) root         (0)     3799 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/new_sim_sending_letter_template.xml
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/report_paperformat.xml
--rw-rw-rw-   0 root         (0) root         (0)     8425 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/sim_sending_letter_template.xml
--rw-rw-rw-   0 root         (0) root         (0)     3036 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/sponsor_sell_back_template.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/security/
--rw-rw-rw-   0 root         (0) root         (0)     7111 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/security/ir.model.access.csv
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/security/res_groups.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5557 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/account_invoice_process.py
--rw-rw-rw-   0 root         (0) root         (0)      500 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/account_invoice_service.py
--rw-rw-rw-   0 root         (0) root         (0)     3164 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/account_payment_group_process.py
--rw-rw-rw-   0 root         (0) root         (0)      961 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/bank_from_iban_getter.py
--rw-rw-rw-   0 root         (0) root         (0)     3602 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/change_partner_emails.py
--rw-rw-rw-   0 root         (0) root         (0)     5981 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_change_tariff_process.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_change_tariff_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1657 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_contract_process.py
--rw-rw-rw-   0 root         (0) root         (0)    11694 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_contract_service.py
--rw-rw-rw-   0 root         (0) root         (0)     3710 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_email_change_process.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_email_change_service.py
--rw-rw-rw-   0 root         (0) root         (0)     4844 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_iban_change_process.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_iban_change_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2809 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_one_shot_process.py
--rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_one_shot_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_process/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2008 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_process/adsl.py
--rw-rw-rw-   0 root         (0) root         (0)     1054 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_process/ba.py
--rw-rw-rw-   0 root         (0) root         (0)    13757 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_process/base.py
--rw-rw-rw-   0 root         (0) root         (0)    10896 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_process/fiber.py
--rw-rw-rw-   0 root         (0) root         (0)     3567 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_process/mobile.py
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_process/router4g.py
--rw-rw-rw-   0 root         (0) root         (0)     8974 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/crm_lead_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/discovery_channel_service.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/get_activation_date.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/hashids_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/partner_email_change_process.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/partner_email_change_service.py
--rw-rw-rw-   0 root         (0) root         (0)     8806 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/product_catalog_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1235 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/provider_service.py
--rw-rw-rw-   0 root         (0) root         (0)     5730 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/res_partner_service.py
--rw-rw-rw-   0 root         (0) root         (0)    22108 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/schemas.py
--rw-rw-rw-   0 root         (0) root         (0)     5848 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/subscription_request_service.py
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/vat_normalizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/somoffice/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:19:40.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/somoffice/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/somoffice/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     2167 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/somoffice/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/description/
--rw-rw-rw-   0 root         (0) root         (0)     9682 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/description/activities.png
--rw-rw-rw-   0 root         (0) root         (0)    12957 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/description/broadband_contract.png
--rw-rw-rw-   0 root         (0) root         (0)    13548 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/description/broadband_lead_lines.png
--rw-rw-rw-   0 root         (0) root         (0)     6550 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/description/emails.png
--rw-rw-rw-   0 root         (0) root         (0)    15486 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/description/mobile_contract.png
--rw-rw-rw-   0 root         (0) root         (0)    15574 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/description/mobile_lead_lines.png
--rw-rw-rw-   0 root         (0) root         (0)    15844 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/description/packs.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/img/
--rw-rw-rw-   0 root         (0) root         (0)    17014 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/img/sc-image.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/src/js/
--rw-rw-rw-   0 root         (0) root         (0)     2514 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/src/js/holidays_highlighter.js
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/src/js/many2many_tags_contract_email.js
--rw-rw-rw-   0 root         (0) root         (0)      605 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/src/js/many2one_tags_crm_lead_email.js
--rw-rw-rw-   0 root         (0) root         (0)     2931 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/src/js/my_attendances.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/src/xml/
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/src/xml/activity.xml
--rw-rw-rw-   0 root         (0) root         (0)      684 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/src/xml/attendance.xml
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/src/xml/contract_email.xml
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/src/xml/mail_chatter_buttons.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4825 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1176 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/common_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/correos_services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:19:40.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/correos_services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7677 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/correos_services/test_shipment.py
--rw-rw-rw-   0 root         (0) root         (0)     3047 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/factories.py
--rw-rw-rw-   0 root         (0) root         (0)     6988 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/listeners/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:19:40.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/listeners/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10823 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/listeners/test_contract_line_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     5866 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/listeners/test_contract_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     3485 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/listeners/test_crm_lead_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/listeners/test_partner_bank_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     7360 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/listeners/test_partner_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     2599 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/listeners/test_res_partner_listener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:19:40.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4310 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_account_invoice.py
--rw-rw-rw-   0 root         (0) root         (0)     3598 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_account_move_line.py
--rw-rw-rw-   0 root         (0) root         (0)     3854 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_account_payment_order.py
--rw-rw-rw-   0 root         (0) root         (0)     5342 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_account_payment_return_gateway.py
--rw-rw-rw-   0 root         (0) root         (0)     4540 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_broadband_isp_info.py
--rw-rw-rw-   0 root         (0) root         (0)    34365 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_contract.py
--rw-rw-rw-   0 root         (0) root         (0)     5827 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_coop_agreement.py
--rw-rw-rw-   0 root         (0) root         (0)    85560 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_crm_lead.py
--rw-rw-rw-   0 root         (0) root         (0)     9390 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1646 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_hr_attendance_process.py
--rw-rw-rw-   0 root         (0) root         (0)     1352 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_mail_activity.py
--rw-rw-rw-   0 root         (0) root         (0)     5484 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_mass_mailing.py
--rw-rw-rw-   0 root         (0) root         (0)     6492 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_mobile_isp_info.py
--rw-rw-rw-   0 root         (0) root         (0)     2485 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_opencell_configuration_wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)     9187 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_payment_return.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_previous_provider.py
--rw-rw-rw-   0 root         (0) root         (0)    28217 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_product_category_technology_supplier.py
--rw-rw-rw-   0 root         (0) root         (0)     3131 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_product_product.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_product_template.py
--rw-rw-rw-   0 root         (0) root         (0)     2932 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_production_lot.py
--rw-rw-rw-   0 root         (0) root         (0)    46314 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_res_partner.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_res_partner_bank.py
--rw-rw-rw-   0 root         (0) root         (0)     5237 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_server_action.py
--rw-rw-rw-   0 root         (0) root         (0)    10862 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_service_supplier.py
--rw-rw-rw-   0 root         (0) root         (0)     4876 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_stock_move_line.py
--rw-rw-rw-   0 root         (0) root         (0)    26854 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_subscription_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:19:40.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_models/test_address.py
--rw-rw-rw-   0 root         (0) root         (0)    11179 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_models/test_crm_account_hierarchy.py
--rw-rw-rw-   0 root         (0) root         (0)     4261 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_models/test_customer.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_models/test_description.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_models/test_opencell_service_codes.py
--rw-rw-rw-   0 root         (0) root         (0)     4105 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_models/test_subscription.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:19:40.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15080 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_service.py
--rw-rw-rw-   0 root         (0) root         (0)    10511 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_strategies.py
--rw-rw-rw-   0 root         (0) root         (0)     6230 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_service.py
--rw-rw-rw-   0 root         (0) root         (0)    15234 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_strategies.py
--rw-rw-rw-   0 root         (0) root         (0)     2335 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_services/test_customer_update_service.py
--rw-rw-rw-   0 root         (0) root         (0)     7743 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_services/test_subscription_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/otrs_factories/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:19:40.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/otrs_factories/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5744 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/otrs_factories/test_adsl_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1326 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/otrs_factories/test_customer_data_from_res_partner.py
--rw-rw-rw-   0 root         (0) root         (0)    10739 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/otrs_factories/test_fiber_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     6540 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/otrs_factories/test_mobile_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     4644 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/otrs_factories/test_router_4G_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1657 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/otrs_factories/test_update_ticket_with_error.py
--rw-rw-rw-   0 root         (0) root         (0)      925 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/sc_test_case.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:19:40.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/contract_process/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:19:40.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/contract_process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      984 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/contract_process/base_test_contract_process.py
--rw-rw-rw-   0 root         (0) root         (0)    26941 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/contract_process/test_fiber_contract_process.py
--rw-rw-rw-   0 root         (0) root         (0)    10414 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/contract_process/test_mobile_contract_process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/contract_services/
--rw-rw-rw-   0 root         (0) root         (0)    71869 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/contract_services/test_contract_contract_service.py
--rw-rw-rw-   0 root         (0) root         (0)     6613 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/contract_services/test_contract_count_controller.py
--rw-rw-rw-   0 root         (0) root         (0)    19447 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/contract_services/test_contract_get_fiber_contracts_to_pack_controller.py
--rw-rw-rw-   0 root         (0) root         (0)    27093 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/contract_services/test_contract_search_controller.py
--rw-rw-rw-   0 root         (0) root         (0)    43501 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_account_invoice_service.py
--rw-rw-rw-   0 root         (0) root         (0)     7531 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_change_partner_emails.py
--rw-rw-rw-   0 root         (0) root         (0)    16922 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_contract_change_tariff_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2980 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_contract_contract_process.py
--rw-rw-rw-   0 root         (0) root         (0)    12908 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_contract_email_change_service.py
--rw-rw-rw-   0 root         (0) root         (0)    13013 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_contract_iban_change_service.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_contract_one_shot_service.py
--rw-rw-rw-   0 root         (0) root         (0)    34346 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_crm_lead_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1769 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_discovery_channel_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1456 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_get_activation_date.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_hashids_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1501 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_mass_mailing_unsubscribe.py
--rw-rw-rw-   0 root         (0) root         (0)     6003 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_partner_email_change_service.py
--rw-rw-rw-   0 root         (0) root         (0)    16699 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_product_catalog_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2141 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_provider_service.py
--rw-rw-rw-   0 root         (0) root         (0)    18948 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_res_partner_service.py
--rw-rw-rw-   0 root         (0) root         (0)     8798 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_subscription_request_service.py
--rw-rw-rw-   0 root         (0) root         (0)      578 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_vat_normalizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/somoffice/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:19:40.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/somoffice/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4863 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/somoffice/test_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:19:40.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9061 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_account_payment_line_create.py
--rw-rw-rw-   0 root         (0) root         (0)     9357 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_address_change_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     5722 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_compensation_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     2552 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_force_oc_integration_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    21666 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_holder_change.py
--rw-rw-rw-   0 root         (0) root         (0)     3581 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_force_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     4007 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     5504 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_invoice_payment_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    20923 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_mobile_tariff_change_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    13855 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_one_shot_request_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    12968 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_tariff_change_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     3322 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_terminate_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    30774 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_create_lead_from_partner_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     4421 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_create_subscription_from_partner.py
--rw-rw-rw-   0 root         (0) root         (0)      802 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_crm_lead_generate_SIM_delivery_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_crm_lead_remesa_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     2911 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_crm_leads_validate_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     2760 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_mail_compose_message_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     1648 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_partner_check_somoffice_email.py
--rw-rw-rw-   0 root         (0) root         (0)     7011 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_partner_email_change_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     4028 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_payment_order_generated_to_upload_queued_wizard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/account_asset_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     2886 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/account_invoice_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/account_move.xml
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/account_move_line.xml
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/account_payment_order_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      471 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/account_tax_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/act_account_move_to_account_move_line_open.xml
--rw-rw-rw-   0 root         (0) root         (0)     1347 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/adsl_service_contract_info_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/aeat_report_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     2690 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/broadband_isp_info_view.xml
--rw-rw-rw-   0 root         (0) root         (0)    25408 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/contract_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     1117 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/coop_agreement_view.xml
--rw-rw-rw-   0 root         (0) root         (0)    12099 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/crm_lead.xml
--rw-rw-rw-   0 root         (0) root         (0)    15207 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/crm_lead_line.xml
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/data_range_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     1283 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/hr_attendance.xml
--rw-rw-rw-   0 root         (0) root         (0)      765 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/ir_action_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     9621 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/mail_activity_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/mail_mail_statistics_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      476 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/mass_mailing_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     3474 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/menus.xml
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/mis_budget_item_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      568 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/mm_fiber_service_contract_info.xml
--rw-rw-rw-   0 root         (0) root         (0)     1711 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/mobile_isp_info_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     1009 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/mobile_service_contract_info_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/open_boards_activities.xml
--rw-rw-rw-   0 root         (0) root         (0)      826 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/operation_request.xml
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/orange_fiber_service_contract_info.xml
--rw-rw-rw-   0 root         (0) root         (0)     1042 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/partner_action_tag_views.xml
--rw-rw-rw-   0 root         (0) root         (0)      619 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/payment_return_import_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/payment_return_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     1244 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/previous_provider_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/product_attribute_views.xml
--rw-rw-rw-   0 root         (0) root         (0)      882 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/product_category_technology_supplier_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/product_pricelist_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     2416 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/product_product_view.xml
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/product_template_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     1199 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/res_company_view.xml
--rw-rw-rw-   0 root         (0) root         (0)    13562 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/res_partner_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/router_4G_service_contract_info.xml
--rw-rw-rw-   0 root         (0) root         (0)      781 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/service_technology_service_supplier.xml
--rw-rw-rw-   0 root         (0) root         (0)      637 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/stock_move_line_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/stock_production_lot.xml
--rw-rw-rw-   0 root         (0) root         (0)     6239 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/subscription_request_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/templates_js.xml
--rw-rw-rw-   0 root         (0) root         (0)      640 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/vodafone_fiber_service_contract_info.xml
--rw-rw-rw-   0 root         (0) root         (0)     1148 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/xoln_fiber_service_contract_info.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/
--rw-rw-rw-   0 root         (0) root         (0)     1170 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/account_financial_report/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/account_financial_report/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      499 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/account_financial_report/aged_partner_balance.py
--rw-rw-rw-   0 root         (0) root         (0)      568 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/account_financial_report/aged_partner_balance.xml
--rw-rw-rw-   0 root         (0) root         (0)     1658 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.py
--rw-rw-rw-   0 root         (0) root         (0)      515 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/account_invoice_confirm/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/account_invoice_confirm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1323 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/account_invoice_confirm/account_invoice_confirm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/account_payment_line_create/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/account_payment_line_create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2542 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create.py
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create_view.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_address_change/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_address_change/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8088 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.py
--rw-rw-rw-   0 root         (0) root         (0)     4084 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_compensation/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_compensation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5033 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.py
--rw-rw-rw-   0 root         (0) root         (0)     3492 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_force_oc_integration/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_force_oc_integration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      413 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_force_oc_integration/contract_force_oc_integration.py
--rw-rw-rw-   0 root         (0) root         (0)     1683 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_force_oc_integration/contract_force_oc_integration.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_holder_change/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_holder_change/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12025 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.py
--rw-rw-rw-   0 root         (0) root         (0)     3069 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_iban_change/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_iban_change/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3782 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_iban_change_force/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_iban_change_force/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      643 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.py
--rw-rw-rw-   0 root         (0) root         (0)     1994 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_invoice_payment/
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_invoice_payment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2088 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.py
--rw-rw-rw-   0 root         (0) root         (0)     1235 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14841 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_one_shot_request/
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_one_shot_request/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4650 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.py
--rw-rw-rw-   0 root         (0) root         (0)     2134 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_tariff_change/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_tariff_change/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5592 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.py
--rw-rw-rw-   0 root         (0) root         (0)     2684 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_terminate/
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_terminate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.py
--rw-rw-rw-   0 root         (0) root         (0)      543 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/create_lead_from_partner/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/create_lead_from_partner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11844 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.py
--rw-rw-rw-   0 root         (0) root         (0)    10758 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/create_subscription_from_partner/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/create_subscription_from_partner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2193 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.py
--rw-rw-rw-   0 root         (0) root         (0)     1810 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      600 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1155 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_lead_remesa/
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_lead_remesa/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1515 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.py
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_leads_validate/
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_leads_validate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.py
--rw-rw-rw-   0 root         (0) root         (0)     1082 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/import_payment_group/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/import_payment_group/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      738 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.py
--rw-rw-rw-   0 root         (0) root         (0)     1093 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/invoice_claim_1_send/
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/invoice_claim_1_send/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1163 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.py
--rw-rw-rw-   0 root         (0) root         (0)      970 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/mail_compose_message/
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/mail_compose_message/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2234 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/mail_compose_message/mail_compose_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.py
--rw-rw-rw-   0 root         (0) root         (0)     1210 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.py
--rw-rw-rw-   0 root         (0) root         (0)     1599 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/partner_email_change/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/partner_email_change/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4734 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.py
--rw-rw-rw-   0 root         (0) root         (0)     3484 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/payment_order_confirm/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/payment_order_confirm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/payment_order_confirm/payment_order_confirm.py
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/payment_order_confirm/payment_order_confirm.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      887 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.py
--rw-rw-rw-   0 root         (0) root         (0)      938 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/product_publish/
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/product_publish/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/product_publish/product_publish.py
--rw-rw-rw-   0 root         (0) root         (0)     3253 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/product_publish/product_publish.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/test_mailing/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/test_mailing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1964 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-07-17 15:30:57.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo12_addon_somconnexio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4980 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo12_addon_somconnexio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    32711 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo12_addon_somconnexio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo12_addon_somconnexio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo12_addon_somconnexio.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     2998 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo12_addon_somconnexio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo12_addon_somconnexio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 06:20:20.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     5934 2023-07-17 15:44:48.000000 odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/
+-rw-r--r--   0 root         (0) root         (0)     4984 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     4519 2023-08-02 14:42:54.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9855 2023-08-02 14:11:51.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/controllers/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/controllers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5170 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/controllers/controllers.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/controllers/http.py
+-rw-rw-rw-   0 root         (0) root         (0)     3458 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/controllers/public_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/correos_services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 15:19:18.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/correos_services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4432 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/correos_services/shipment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/
+-rw-rw-rw-   0 root         (0) root         (0)    46993 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/account.account.template-sc.csv
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/account_chart_template_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2954 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/account_group.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/account_journal.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2599 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/account_payment_mode.xml
+-rw-rw-rw-   0 root         (0) root         (0)     4496 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/account_payment_term.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1730 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/account_tax.xml
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/account_tax_group.xml
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/analytic_account.xml
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/base_automation.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2241 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/company.xml
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/contract_compute_current_tariff_cron.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3786 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/contract_terminate_reason.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/contract_terminate_user_reason.xml
+-rw-rw-rw-   0 root         (0) root         (0)      947 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/crm_stage_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)      658 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/crm_track_correos_delivery_cron.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/discovery_channel.xml
+-rw-rw-rw-   0 root         (0) root         (0)      752 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/fiber_signal_type_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)      837 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/hr_attendance_place.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/ir_config_pararameter.xml
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/ir_sequence.xml
+-rw-rw-rw-   0 root         (0) root         (0)    13962 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/mail_activity_type.xml
+-rw-rw-rw-   0 root         (0) root         (0)      150 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/mail_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3266 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/mail_mass_mailing_list_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2542 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/mis_report.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/operation_request_terminate_reason.xml
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/partner_action_tag_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/partner_priority.xml
+-rw-rw-rw-   0 root         (0) root         (0)    14751 2023-08-02 13:24:33.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/previous_provider_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1459 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/product_attribute.xml
+-rw-rw-rw-   0 root         (0) root         (0)     7767 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/product_attribute_value.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2455 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/product_categories.xml
+-rw-rw-rw-   0 root         (0) root         (0)     7830 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/product_category_technology_supplier_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)    11481 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/product_pack_line.xml
+-rw-rw-rw-   0 root         (0) root         (0)    41333 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/product_product.xml
+-rw-rw-rw-   0 root         (0) root         (0)     5653 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/product_template_attribute_line_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)    11160 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/product_template_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)      413 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/res.partner.bank.xml
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/res.users.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3704 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/res_bank_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/service_supplier.xml
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/service_technology.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/service_technology_service_supplier.xml
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/share_type.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/demo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/demo/contract/
+-rw-rw-rw-   0 root         (0) root         (0)     2573 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/demo/contract/contract.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/demo/contract/contract_pack.xml
+-rw-rw-rw-   0 root         (0) root         (0)     4018 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/demo/contract/contract_shared_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)     6655 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/demo/partner.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2749 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/demo/product.pricelist.csv
+-rw-rw-rw-   0 root         (0) root         (0)     2346 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/demo/subscription_requests.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 15:19:18.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/helpers/date.py
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/helpers/language.py
+-rw-rw-rw-   0 root         (0) root         (0)     1846 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)   326041 2023-08-02 13:30:07.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/i18n/ca_ES.po
+-rw-rw-rw-   0 root         (0) root         (0)   332843 2023-08-02 13:30:07.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/i18n/es.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/listeners/
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/listeners/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3078 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/listeners/contract_line_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/listeners/contract_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/listeners/crm_lead_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)      742 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/listeners/partner_bank_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     1355 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/listeners/partner_listener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.8/pre-clean-mail-tracking-value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.8.11/
+-rw-rw-rw-   0 root         (0) root         (0)      423 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.8.11/post-create-copy-contract-service-info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.8.4/
+-rw-rw-rw-   0 root         (0) root         (0)     2709 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.8.4/post-create-copy-contract-service-info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.8.4/pre-create-one-gb-wo-cost.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)      990 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.9/post-link-crm-to-contract.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.9/post-migrate-change-address.py
+-rw-rw-rw-   0 root         (0) root         (0)      867 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.9/pre-migrate-change-address.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.9/pre-uniform-contracts-wo-number.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.9.13/
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.9.13/post-change-activities-user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.9.2/
+-rw-rw-rw-   0 root         (0) root         (0)      533 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.9.2/post-upper-sponsorship-code.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.9.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.9.9/post-import-es-geonames.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.2.0.0/post-recompute-is-from-pack.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.2.0.0/post-relate-is-from-not-pack-attribute-with-existing-products.py
+-rw-rw-rw-   0 root         (0) root         (0)     1260 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-create-is-from-pack-attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-set-xml-id-unlimited-20GB.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.2.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1191 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.2.1.6/post-set-state_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.2.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)      242 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.2.1.8/pre-assign-imd-manual-created-activity-types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.2.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2293 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.2.2.0/pre-fix-catalog-externalId.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/erppeek/
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/erppeek/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/erppeek/erppeek.ini
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/erppeek/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1043 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/erppeek/update_contract_line_product_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/
+-rw-rw-rw-   0 root         (0) root         (0)     1838 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/account_asset.py
+-rw-rw-rw-   0 root         (0) root         (0)      931 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/account_banking_mandate.py
+-rw-rw-rw-   0 root         (0) root         (0)     6377 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/account_invoice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2367 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/account_invoice_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      142 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/account_journal.py
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/account_move.py
+-rw-rw-rw-   0 root         (0) root         (0)     3769 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/account_move_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1330 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/account_payment_order.py
+-rw-rw-rw-   0 root         (0) root         (0)     1897 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/account_payment_return_email_gateway.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/account_tax.py
+-rw-rw-rw-   0 root         (0) root         (0)    21169 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/aged_partner_balance.py
+-rw-rw-rw-   0 root         (0) root         (0)     7108 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/aged_partner_balance_xlsx.py
+-rw-rw-rw-   0 root         (0) root         (0)    40172 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/contract.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/contract_info/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/contract_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/contract_info/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3230 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/contract_info/broadband.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/contract_info/mobile.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/contract_terminate_reason.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/contract_terminate_user_reason.py
+-rw-rw-rw-   0 root         (0) root         (0)     1232 2023-07-31 15:38:12.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/coop_agreement.py
+-rw-rw-rw-   0 root         (0) root         (0)    21856 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/crm_lead.py
+-rw-rw-rw-   0 root         (0) root         (0)    11230 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/discovery_channel.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/fiber_signal_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/hr_attendance.py
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/hr_attendance_place.py
+-rw-rw-rw-   0 root         (0) root         (0)     3864 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/hr_employee.py
+-rw-rw-rw-   0 root         (0) root         (0)     4417 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/ir_model_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/ir_server_action.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/isp_info/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/isp_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3680 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/isp_info/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3644 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/isp_info/broadband.py
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/isp_info/mobile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/l10n_es_aeat_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     3881 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/mail_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)      419 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/mail_thread.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/mass_mailing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/mobile_contract_otrs_view.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/opencell_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/operation_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/operation_request_terminate_reason.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/partner_action_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2816 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/partner_otrs_view.py
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/payment_return.py
+-rw-rw-rw-   0 root         (0) root         (0)     3407 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/payment_return_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/previous_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/product_attribute_value.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/product_category_technology_supplier.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/product_pack_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/product_pricelist.py
+-rw-rw-rw-   0 root         (0) root         (0)     5945 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/product_product.py
+-rw-rw-rw-   0 root         (0) root         (0)      640 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/product_template.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/res_company.py
+-rw-rw-rw-   0 root         (0) root         (0)    22511 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/res_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/res_partner_bank.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/service_supplier.py
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/service_technology.py
+-rw-rw-rw-   0 root         (0) root         (0)     2509 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/stock_move_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1818 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/stock_production_lot.py
+-rw-rw-rw-   0 root         (0) root         (0)    12471 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/subscription_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/utm_source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_models/
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_models/access.py
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_models/account_hierarchy_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     5121 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_models/crm_account_hierarchy.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_models/customer.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_models/opencell_resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_models/opencell_types/
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_models/opencell_types/address.py
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_models/opencell_types/custom_field.py
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_models/opencell_types/description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1776 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_models/services.py
+-rw-rw-rw-   0 root         (0) root         (0)     2144 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_models/subscription.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 15:19:18.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2944 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_strategies.py
+-rw-rw-rw-   0 root         (0) root         (0)     3430 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     5227 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_strategies.py
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_services/customer_update_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_services/opencell_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_services/subscription_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/otrs_factories/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 15:19:18.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/otrs_factories/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/otrs_factories/adsl_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1152 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/otrs_factories/base_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/otrs_factories/broadband_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/otrs_factories/customer_data_from_res_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2762 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/otrs_factories/fiber_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1749 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/otrs_factories/mobile_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/otrs_factories/router_4G_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      999 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/otrs_factories/service_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/otrs_factories/update_ticket_with_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18705 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/account_asset_report_xls.py
+-rw-rw-rw-   0 root         (0) root         (0)    20209 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/aged_partner_balance.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3285 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/crm_lead_creation_email_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1363 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/invoice_claim_1_capital_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1398 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/invoice_claim_1_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1969 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/mobile_can_be_linked_with_fiber_mail_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1957 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/mobile_linked_with_fiber_mail_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3799 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/new_sim_sending_letter_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/report_paperformat.xml
+-rw-rw-rw-   0 root         (0) root         (0)     8425 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/sim_sending_letter_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/sponsor_sell_back_template.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/security/
+-rw-rw-rw-   0 root         (0) root         (0)     7303 2023-08-02 13:30:07.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/security/ir.model.access.csv
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/security/res_groups.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/
+-rw-rw-rw-   0 root         (0) root         (0)      660 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5557 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/account_invoice_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      500 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/account_invoice_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     3164 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/account_payment_group_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      961 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/bank_from_iban_getter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3602 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/change_partner_emails.py
+-rw-rw-rw-   0 root         (0) root         (0)     5981 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_change_tariff_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_change_tariff_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1657 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_contract_process.py
+-rw-rw-rw-   0 root         (0) root         (0)    11694 2023-08-02 11:12:51.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_contract_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     3710 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_email_change_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_email_change_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     4844 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_iban_change_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_iban_change_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2809 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_one_shot_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_one_shot_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_process/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2008 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_process/adsl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_process/ba.py
+-rw-rw-rw-   0 root         (0) root         (0)    13757 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_process/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10896 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_process/fiber.py
+-rw-rw-rw-   0 root         (0) root         (0)     3567 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_process/mobile.py
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_process/router4g.py
+-rw-rw-rw-   0 root         (0) root         (0)     8974 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/crm_lead_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/discovery_channel_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/get_activation_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/hashids_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/partner_email_change_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/partner_email_change_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     8806 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/product_catalog_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1235 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/provider_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     5730 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/res_partner_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    22108 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/schemas.py
+-rw-rw-rw-   0 root         (0) root         (0)     5848 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/subscription_request_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/vat_normalizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/somoffice/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 15:19:18.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/somoffice/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/somoffice/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     2167 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/somoffice/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/description/
+-rw-rw-rw-   0 root         (0) root         (0)     9682 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/description/activities.png
+-rw-rw-rw-   0 root         (0) root         (0)    12957 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/description/broadband_contract.png
+-rw-rw-rw-   0 root         (0) root         (0)    13548 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/description/broadband_lead_lines.png
+-rw-rw-rw-   0 root         (0) root         (0)     6550 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/description/emails.png
+-rw-rw-rw-   0 root         (0) root         (0)    15486 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/description/mobile_contract.png
+-rw-rw-rw-   0 root         (0) root         (0)    15574 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/description/mobile_lead_lines.png
+-rw-rw-rw-   0 root         (0) root         (0)    15844 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/description/packs.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)    17014 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/img/sc-image.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/src/js/
+-rw-rw-rw-   0 root         (0) root         (0)     2514 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/src/js/holidays_highlighter.js
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/src/js/many2many_tags_contract_email.js
+-rw-rw-rw-   0 root         (0) root         (0)      605 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/src/js/many2one_tags_crm_lead_email.js
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/src/js/my_attendances.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/src/xml/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/src/xml/activity.xml
+-rw-rw-rw-   0 root         (0) root         (0)      684 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/src/xml/attendance.xml
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/src/xml/contract_email.xml
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/src/xml/mail_chatter_buttons.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3462 2023-08-02 13:27:47.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/common_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/correos_services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 15:19:18.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/correos_services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7677 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/correos_services/test_shipment.py
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)     6988 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/listeners/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 15:19:18.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/listeners/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10823 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/listeners/test_contract_line_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     5866 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/listeners/test_contract_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     3485 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/listeners/test_crm_lead_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/listeners/test_partner_bank_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     7360 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/listeners/test_partner_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     2599 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/listeners/test_res_partner_listener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 15:19:18.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4310 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_account_invoice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3598 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_account_move_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     3854 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_account_payment_order.py
+-rw-rw-rw-   0 root         (0) root         (0)     5342 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_account_payment_return_gateway.py
+-rw-rw-rw-   0 root         (0) root         (0)     4540 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_broadband_isp_info.py
+-rw-rw-rw-   0 root         (0) root         (0)    34365 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_contract.py
+-rw-rw-rw-   0 root         (0) root         (0)     5827 2023-07-31 15:38:12.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_coop_agreement.py
+-rw-rw-rw-   0 root         (0) root         (0)    85560 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_crm_lead.py
+-rw-rw-rw-   0 root         (0) root         (0)     9390 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1646 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_hr_attendance_process.py
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_mail_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)     5484 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_mass_mailing.py
+-rw-rw-rw-   0 root         (0) root         (0)     6492 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_mobile_isp_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     2485 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_opencell_configuration_wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     9187 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_payment_return.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_previous_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    28217 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_product_category_technology_supplier.py
+-rw-rw-rw-   0 root         (0) root         (0)     3131 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_product_product.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_product_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     2932 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_production_lot.py
+-rw-rw-rw-   0 root         (0) root         (0)    46314 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_res_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)      574 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_res_partner_bank.py
+-rw-rw-rw-   0 root         (0) root         (0)     5237 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_server_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    10862 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_service_supplier.py
+-rw-rw-rw-   0 root         (0) root         (0)     4876 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_stock_move_line.py
+-rw-rw-rw-   0 root         (0) root         (0)    26854 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_subscription_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 15:19:18.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_models/test_address.py
+-rw-rw-rw-   0 root         (0) root         (0)    11179 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_models/test_crm_account_hierarchy.py
+-rw-rw-rw-   0 root         (0) root         (0)     4261 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_models/test_customer.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_models/test_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_models/test_opencell_service_codes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4105 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_models/test_subscription.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 15:19:18.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15080 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    10511 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_strategies.py
+-rw-rw-rw-   0 root         (0) root         (0)     6230 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    15234 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_strategies.py
+-rw-rw-rw-   0 root         (0) root         (0)     2335 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_services/test_customer_update_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     7743 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_services/test_subscription_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/otrs_factories/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 15:19:18.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/otrs_factories/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5744 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/otrs_factories/test_adsl_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/otrs_factories/test_customer_data_from_res_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)    10739 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/otrs_factories/test_fiber_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     6540 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/otrs_factories/test_mobile_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     4644 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/otrs_factories/test_router_4G_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1657 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/otrs_factories/test_update_ticket_with_error.py
+-rw-rw-rw-   0 root         (0) root         (0)      925 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/sc_test_case.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 15:19:18.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/contract_process/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 15:19:18.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/contract_process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      984 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/contract_process/base_test_contract_process.py
+-rw-rw-rw-   0 root         (0) root         (0)    26941 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/contract_process/test_fiber_contract_process.py
+-rw-rw-rw-   0 root         (0) root         (0)    10414 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/contract_process/test_mobile_contract_process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/contract_services/
+-rw-rw-rw-   0 root         (0) root         (0)    71869 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/contract_services/test_contract_contract_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     6613 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/contract_services/test_contract_count_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    19447 2023-08-02 11:12:51.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/contract_services/test_contract_get_fiber_contracts_to_pack_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    27093 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/contract_services/test_contract_search_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    43501 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_account_invoice_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     7531 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_change_partner_emails.py
+-rw-rw-rw-   0 root         (0) root         (0)    16922 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_contract_change_tariff_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2980 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_contract_contract_process.py
+-rw-rw-rw-   0 root         (0) root         (0)    12908 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_contract_email_change_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    13013 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_contract_iban_change_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_contract_one_shot_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    34346 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_crm_lead_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1769 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_discovery_channel_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_get_activation_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_hashids_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1501 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_mass_mailing_unsubscribe.py
+-rw-rw-rw-   0 root         (0) root         (0)     6003 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_partner_email_change_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    16699 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_product_catalog_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2023-08-02 13:24:33.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_provider_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    18948 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_res_partner_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     8798 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_subscription_request_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      578 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_vat_normalizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/somoffice/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 15:19:18.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/somoffice/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/somoffice/test_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 15:19:18.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9061 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_account_payment_line_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     9357 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_address_change_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     5722 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_compensation_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     2552 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_force_oc_integration_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    21666 2023-08-02 11:12:51.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_holder_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     3581 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_force_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     4007 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     5504 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_invoice_payment_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    22728 2023-08-02 13:30:07.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_mobile_tariff_change_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    13855 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_one_shot_request_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    12968 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_tariff_change_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     3322 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_terminate_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-08-02 13:27:47.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_create_lead_add_mobile_line.py
+-rw-rw-rw-   0 root         (0) root         (0)    30774 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_create_lead_from_partner_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     4421 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_create_subscription_from_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_crm_lead_generate_SIM_delivery_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_crm_lead_remesa_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     2911 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_crm_leads_validate_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_mail_compose_message_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     1648 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_partner_check_somoffice_email.py
+-rw-rw-rw-   0 root         (0) root         (0)     7011 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_partner_email_change_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     4028 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_payment_order_generated_to_upload_queued_wizard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/account_asset_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2886 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/account_invoice_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/account_move.xml
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/account_move_line.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/account_payment_order_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      471 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/account_tax_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/act_account_move_to_account_move_line_open.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/adsl_service_contract_info_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/aeat_report_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2690 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/broadband_isp_info_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)    25408 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/contract_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/coop_agreement_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)    12099 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/crm_lead.xml
+-rw-rw-rw-   0 root         (0) root         (0)    15207 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/crm_lead_line.xml
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/data_range_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/hr_attendance.xml
+-rw-rw-rw-   0 root         (0) root         (0)      765 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/ir_action_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     9621 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/mail_activity_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/mail_mail_statistics_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      476 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/mass_mailing_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3474 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/menus.xml
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/mis_budget_item_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      568 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/mm_fiber_service_contract_info.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1711 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/mobile_isp_info_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/mobile_service_contract_info_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/open_boards_activities.xml
+-rw-rw-rw-   0 root         (0) root         (0)      826 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/operation_request.xml
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/orange_fiber_service_contract_info.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1042 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/partner_action_tag_views.xml
+-rw-rw-rw-   0 root         (0) root         (0)      619 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/payment_return_import_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/payment_return_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/previous_provider_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/product_attribute_views.xml
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/product_category_technology_supplier_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/product_pricelist_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2416 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/product_product_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/product_template_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/res_company_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)    13562 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/res_partner_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/router_4G_service_contract_info.xml
+-rw-rw-rw-   0 root         (0) root         (0)      781 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/service_technology_service_supplier.xml
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/stock_move_line_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/stock_production_lot.xml
+-rw-rw-rw-   0 root         (0) root         (0)     6239 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/subscription_request_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/templates_js.xml
+-rw-rw-rw-   0 root         (0) root         (0)      640 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/vodafone_fiber_service_contract_info.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/xoln_fiber_service_contract_info.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-08-02 13:27:47.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/account_financial_report/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/account_financial_report/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/account_financial_report/aged_partner_balance.py
+-rw-rw-rw-   0 root         (0) root         (0)      568 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/account_financial_report/aged_partner_balance.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1658 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.py
+-rw-rw-rw-   0 root         (0) root         (0)      515 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/account_invoice_confirm/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/account_invoice_confirm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/account_invoice_confirm/account_invoice_confirm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/account_payment_line_create/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/account_payment_line_create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2542 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create_view.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_address_change/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_address_change/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8088 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     4084 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_compensation/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_compensation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5033 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3492 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_force_oc_integration/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_force_oc_integration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      413 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_force_oc_integration/contract_force_oc_integration.py
+-rw-rw-rw-   0 root         (0) root         (0)     1683 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_force_oc_integration/contract_force_oc_integration.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_holder_change/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_holder_change/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12025 2023-08-02 11:12:51.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     3069 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_iban_change/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_iban_change/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3782 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_iban_change_force/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_iban_change_force/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      643 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.py
+-rw-rw-rw-   0 root         (0) root         (0)     1994 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_invoice_payment/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_invoice_payment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2088 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1235 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18264 2023-08-02 13:30:07.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     4590 2023-08-02 13:30:07.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_one_shot_request/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_one_shot_request/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4650 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     2134 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_tariff_change/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_tariff_change/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5592 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     2684 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_terminate/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_terminate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.py
+-rw-rw-rw-   0 root         (0) root         (0)      543 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/create_lead_from_partner/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/create_lead_from_partner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11844 2023-08-02 11:12:51.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)    10758 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/create_subscription_from_partner/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/create_subscription_from_partner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2193 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1810 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_add_mobile_line/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-08-02 13:27:47.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_add_mobile_line/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4065 2023-08-02 13:27:47.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_add_mobile_line/crm_lead_add_mobile_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     5190 2023-08-02 13:27:47.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_add_mobile_line/crm_lead_add_mobile_line.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      600 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1155 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_remesa/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_remesa/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_leads_validate/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_leads_validate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/import_payment_group/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/import_payment_group/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      738 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.py
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/invoice_claim_1_send/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/invoice_claim_1_send/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.py
+-rw-rw-rw-   0 root         (0) root         (0)      970 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/mail_compose_message/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/mail_compose_message/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/mail_compose_message/mail_compose_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.py
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.py
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/partner_email_change/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/partner_email_change/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4734 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     3484 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/payment_order_confirm/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/payment_order_confirm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/payment_order_confirm/payment_order_confirm.py
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/payment_order_confirm/payment_order_confirm.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      887 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.py
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/product_publish/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/product_publish/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/product_publish/product_publish.py
+-rw-rw-rw-   0 root         (0) root         (0)     3253 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/product_publish/product_publish.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/test_mailing/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/test_mailing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1964 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-07-31 12:57:28.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo12_addon_somconnexio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4984 2023-08-02 15:19:58.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo12_addon_somconnexio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    33025 2023-08-02 15:19:58.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo12_addon_somconnexio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 15:19:58.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo12_addon_somconnexio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 15:19:58.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo12_addon_somconnexio.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     2998 2023-08-02 15:19:58.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo12_addon_somconnexio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-02 15:19:58.000000 odoo12-addon-somconnexio-12.0.2.3.4/odoo12_addon_somconnexio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 15:19:59.000000 odoo12-addon-somconnexio-12.0.2.3.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     5934 2023-08-02 13:30:07.000000 odoo12-addon-somconnexio-12.0.2.3.4/setup.py
```

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/PKG-INFO` & `odoo12-addon-somconnexio-12.0.2.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo12-addon-somconnexio
-Version: 12.0.2.3.3.99.dev2
+Version: 12.0.2.3.4
 Summary: Odoo Som Connexió customizations
 Home-page: https://coopdevs.org
 Author: Coopdevs Treball SCCL
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
@@ -52,15 +52,15 @@
 
 Enter to your local machine as the user `odoo`, activate the python enviornment first and run the odoo bin:
 ```sh
 $ ssh odoo@odoo-sc.local
 $ pyenv activate odoo
 $ cd /opt/odoo
 $ set -a && source /etc/default/odoo && set +a
-$ ./odoo-bin -c /etc/odoo/odoo.conf -u somconnexio -d odoo
+$ ./odoo-bin -c /etc/odoo/odoo.conf -u somconnexio -d odoo --workers 0
 ```
 
 To use the local somconnexio module (development version) instead of the PyPI published one, you need to upgrade the [version in the manifest](https://gitlab.com/coopdevs/odoo-somconnexio/-/blob/master/somconnexio/__manifest__.py#L3) and then update the module with `-u` in the Odoo CLI.
 
 
 #### Restart ODOO database from scratch
```

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/README.md` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 Enter to your local machine as the user `odoo`, activate the python enviornment first and run the odoo bin:
 ```sh
 $ ssh odoo@odoo-sc.local
 $ pyenv activate odoo
 $ cd /opt/odoo
 $ set -a && source /etc/default/odoo && set +a
-$ ./odoo-bin -c /etc/odoo/odoo.conf -u somconnexio -d odoo
+$ ./odoo-bin -c /etc/odoo/odoo.conf -u somconnexio -d odoo --workers 0
 ```
 
 To use the local somconnexio module (development version) instead of the PyPI published one, you need to upgrade the [version in the manifest](https://gitlab.com/coopdevs/odoo-somconnexio/-/blob/master/somconnexio/__manifest__.py#L3) and then update the module with `-u` in the Odoo CLI.
 
 
 #### Restart ODOO database from scratch
```

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/__manifest__.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/__manifest__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     "name": "Odoo Som Connexió customizations",
-    "version": "12.0.2.3.3",
+    "version": "12.0.2.3.4",
     "depends": [
         "account_asset_management",
         "account_banking_sepa_credit_transfer",
         "account_banking_sepa_direct_debit",
         "account_cancel",
         "account_chart_update",
         "account_due_list",
@@ -216,14 +216,15 @@
         "reports/mobile_can_be_linked_with_fiber_mail_template.xml",
         "reports/mobile_linked_with_fiber_mail_template.xml",
         "views/aeat_report_view.xml",
         "views/account_asset_view.xml",
         "views/data_range_view.xml",
         "wizards/contract_iban_change_force/contract_iban_change_force.xml",
         "wizards/test_mailing/test_mailing.xml",
+        "wizards/crm_lead_add_mobile_line/crm_lead_add_mobile_line.xml",
         "views/mass_mailing_view.xml",
         "views/mail_mail_statistics_view.xml",
         "data/product_pack_line.xml",
     ],
     "demo": [
         "demo/partner.xml",
         "demo/product.pricelist.csv",
```

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/controllers/controllers.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/controllers/controllers.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/controllers/http.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/controllers/http.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/controllers/public_controller.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/controllers/public_controller.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/correos_services/shipment.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/correos_services/shipment.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/account.account.template-sc.csv` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/account.account.template-sc.csv`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/account_chart_template_data.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/account_chart_template_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/account_group.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/account_group.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/account_journal.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/account_journal.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/account_payment_mode.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/account_payment_mode.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/account_payment_term.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/account_payment_term.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/account_tax.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/account_tax.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/analytic_account.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/analytic_account.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/base_automation.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/base_automation.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/company.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/company.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/contract_compute_current_tariff_cron.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/contract_compute_current_tariff_cron.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/contract_terminate_reason.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/contract_terminate_reason.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/contract_terminate_user_reason.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/contract_terminate_user_reason.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/crm_stage_data.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/crm_stage_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/crm_track_correos_delivery_cron.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/crm_track_correos_delivery_cron.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/discovery_channel.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/discovery_channel.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/fiber_signal_type_data.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/fiber_signal_type_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/hr_attendance_place.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/hr_attendance_place.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/ir_config_pararameter.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/ir_config_pararameter.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/ir_sequence.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/ir_sequence.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/mail_activity_type.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/mail_activity_type.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/mail_mass_mailing_list_data.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/mail_mass_mailing_list_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/mis_report.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/mis_report.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/operation_request_terminate_reason.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/operation_request_terminate_reason.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/partner_action_tag_data.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/partner_action_tag_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/partner_priority.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/partner_priority.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/product_attribute.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/product_attribute.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/product_attribute_value.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/product_attribute_value.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/product_categories.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/product_categories.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/product_category_technology_supplier_data.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/product_category_technology_supplier_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/product_pack_line.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/product_pack_line.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/product_product.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/product_product.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/product_template_attribute_line_data.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/product_template_attribute_line_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/product_template_data.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/product_template_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/res_bank_data.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/res_bank_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/service_supplier.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/service_supplier.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/service_technology.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/service_technology.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/service_technology_service_supplier.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/service_technology_service_supplier.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/data/share_type.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/data/share_type.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/demo/contract/contract.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/demo/contract/contract.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/demo/contract/contract_pack.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/demo/contract/contract_pack.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/demo/contract/contract_shared_data.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/demo/contract/contract_shared_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/demo/partner.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/demo/partner.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/demo/product.pricelist.csv` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/demo/product.pricelist.csv`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/demo/subscription_requests.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/demo/subscription_requests.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/hooks.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/hooks.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/i18n/ca_ES.po` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/i18n/ca_ES.po`

 * *Files 1% similar despite different names*

```diff
@@ -1484,19 +1484,14 @@
 msgstr "ID abonament compartit"
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_contract_mobile_tariff_change_wizard__shared_bond_id_to_join
 msgid "Shared bond id to join option"
 msgstr "A quin abonament compartit la volem afegir?"
 
-#. module: somconnexio
-#: model:ir.model.fields,field_description:somconnexio.field_contract_mobile_tariff_change_wizard__sharing_data_options
-msgid "Sharing bond option"
-msgstr "Opcions per compartir dades mòbils"
-
 #. module: easy_my_coop
 #: model:ir.model.fields,field_description:easy_my_coop.field_subscription_request__skip_control_ng
 msgid "Skip control"
 msgstr "Passar els controls"
 
 #. module: easy_my_coop
 #: model:ir.model.fields,field_description:easy_my_coop.field_operation_request__state
@@ -2410,15 +2405,15 @@
 #: code:addons/somconnexio/models/res_partner.py:260
 #: code:addons/somconnexio/models/subscription_request.py:209
 #, python-format
 msgid "A partner with VAT %s already exists in our system"
 msgstr "Ja existeix un contacte amb VAT %s al sistema."
 
 #. module: somconnexio
-#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:309
+#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:342
 #, python-format
 msgid "A new shared bond creation cannot be an exceptional change"
 msgstr "Un canvi de tarifa per crear un abonament de compartides no pot ser excepcional"
 
 #. module: somconnexio
 #: selection:broadband.isp.info,previous_service:0
 msgid "ADSL"
@@ -2526,14 +2521,20 @@
 #: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:149
 #: model:shared.bond.type,name:somconnexio.existing_shared_bond
 #, python-format
 msgid "Add line to existing shared bond"
 msgstr "Afegir línia mòbil a un abonament existent"
 
 #. module: somconnexio
+#: model:ir.actions.act_window,name:somconnexio.action_crm_lead_add_mobile_line_wizard
+#: model_terms:ir.ui.view,arch_db:somconnexio.view_lead_create_mobile_lines_wizard_button
+msgid "Add mobile line to CRM Lead"
+msgstr "Afegir línia mòbil"
+
+#. module: somconnexio
 #: model:ir.actions.act_window,name:somconnexio.move_line_add_to_payment_debit_order_action
 msgid "Add to Payment/Debit Order"
 msgstr "Afegiu a ordre de pagament/cobrament"
 
 #. module: somconnexio
 #: code:addons/somconnexio/listeners/contract_line_listener.py:47
 #, python-format
@@ -2645,14 +2646,20 @@
 
 #. module: somconnexio
 #: model_terms:ir.ui.view,arch_db:somconnexio.report_aged_partner_balance_move_lines
 msgid "Amount due"
 msgstr "Deute vençut"
 
 #. module: somconnexio
+#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:346
+#, python-format
+msgid "Another mobile is required to create a shared data bond"
+msgstr "Necessites com a mínim un altre mòbil per crear un abonament de dades compartit"
+
+#. module: somconnexio
 #: model_terms:ir.ui.view,arch_db:somconnexio.new_sim_sending_letter_lang_template
 msgid "Aquí tens la nova SIM de Som Connexió per a la línia"
 msgstr "Aquí tens la nova SIM de Som Connexió per a la línia"
 
 #. module: somconnexio
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_lead_line_broadband
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_lead_line_mobile
@@ -2857,14 +2864,15 @@
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_contract_address_change_wizard
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_partner_email_change_wizard
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_contract_force_oc_integration
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_contract_holder_change_wizard
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_contract_iban_change_wizard
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_contract_one_shot_request_wizard
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_contract_tariff_change_wizard
+#: model_terms:ir.ui.view,arch_db:somconnexio.view_form_crm_lead_add_mobile_line_wizard
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_crm_leads_validate_wizard
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_invoice_claim_1_send_wizard
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_lead_line_broadband
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_lead_line_mobile
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_partner_create_lead_wizard
 msgid "Cancel"
 msgstr "Cancel·lar"
@@ -3264,14 +3272,15 @@
 #, python-format
 msgid "Couldn't reach SomOffice user. Please contact IT department"
 msgstr "No s'ha trobat l'usuari de la Oficina Virtual. Siusplau, contacta amb l'equip tècnic"
 
 #. module: somconnexio
 #: model_terms:ir.ui.view,arch_db:somconnexio.move_line_add_to_payment_debit_order_form
 #: model_terms:ir.ui.view,arch_db:somconnexio.payment_order_generated_to_uploaded_form
+#: model_terms:ir.ui.view,arch_db:somconnexio.view_form_crm_lead_add_mobile_line_wizard
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_partner_create_lead_wizard
 msgid "Create"
 msgstr "Crear"
 
 #. module: somconnexio
 #: model:ir.actions.act_window,name:somconnexio.action_partner_lead_create_wizard
 msgid "Create Lead"
@@ -3283,15 +3292,15 @@
 msgstr "Obrir petició de servei manualment"
 
 #. module: somconnexio
 #: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:148
 #: model:shared.bond.type,name:somconnexio.new_shared_bond
 #, python-format
 msgid "Create new shared bond"
-msgstr "Crear un nou abonament"
+msgstr "Crear un abonament de dades compartides"
 
 #. module: somconnexio
 #: model_terms:ir.ui.view,arch_db:somconnexio.move_line_add_to_payment_debit_order_form
 msgid "Create Payment Lines"
 msgstr "Crea línies de pagament"
 
 #. module: somconnexio
@@ -3306,14 +3315,15 @@
 #: model:ir.model.fields,field_description:somconnexio.field_partner_email_change_wizard__create_uid
 #: model:ir.model.fields,field_description:somconnexio.field_contract_holder_change_wizard__create_uid
 #: model:ir.model.fields,field_description:somconnexio.field_contract_iban_change_wizard__create_uid
 #: model:ir.model.fields,field_description:somconnexio.field_contract_mobile_tariff_change_wizard__create_uid
 #: model:ir.model.fields,field_description:somconnexio.field_contract_one_shot_request_wizard__create_uid
 #: model:ir.model.fields,field_description:somconnexio.field_contract_tariff_change_wizard__create_uid
 #: model:ir.model.fields,field_description:somconnexio.field_coop_agreement__create_uid
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__create_uid
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_validate_wizard__create_uid
 #: model:ir.model.fields,field_description:somconnexio.field_discovery_channel__create_uid
 #: model:ir.model.fields,field_description:somconnexio.field_invoice_claim_1_send_wizard__create_uid
 #: model:ir.model.fields,field_description:somconnexio.field_mm_fiber_service_contract_info__create_uid
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__create_uid
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_service_contract_info__create_uid
 #: model:ir.model.fields,field_description:somconnexio.field_move_line_add_to_payment_debit_order__create_uid
@@ -3335,14 +3345,15 @@
 #: model:ir.model.fields,field_description:somconnexio.field_contract_address_change_wizard__create_date
 #: model:ir.model.fields,field_description:somconnexio.field_partner_email_change_wizard__create_date
 #: model:ir.model.fields,field_description:somconnexio.field_contract_holder_change_wizard__create_date
 #: model:ir.model.fields,field_description:somconnexio.field_contract_iban_change_wizard__create_date
 #: model:ir.model.fields,field_description:somconnexio.field_contract_one_shot_request_wizard__create_date
 #: model:ir.model.fields,field_description:somconnexio.field_contract_tariff_change_wizard__create_date
 #: model:ir.model.fields,field_description:somconnexio.field_coop_agreement__create_date
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__create_date
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_validate_wizard__create_date
 #: model:ir.model.fields,field_description:somconnexio.field_discovery_channel__create_date
 #: model:ir.model.fields,field_description:somconnexio.field_invoice_claim_1_send_wizard__create_date
 #: model:ir.model.fields,field_description:somconnexio.field_mm_fiber_service_contract_info__create_date
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__create_date
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_service_contract_info__create_date
 #: model:ir.model.fields,field_description:somconnexio.field_move_line_add_to_payment_debit_order__create_date
@@ -3379,14 +3390,15 @@
 
 #. module: somconnexio
 #: model:mis.report.subkpi,description:somconnexio.mis_report_subkpi_credit
 msgid "Credit"
 msgstr "Crèdit"
 
 #. module: somconnexio
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__crm_lead_id
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_validate_wizard__crm_lead_ids
 msgid "Crm Lead"
 msgstr "Petició de contracte"
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_contract_contract__crm_lead_line_id
 msgid "Crm Lead Line"
@@ -3485,26 +3497,28 @@
 msgid "Debit"
 msgstr "Dèbit"
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_base_isp_info__delivery_city
 #: model:ir.model.fields,field_description:somconnexio.field_broadband_isp_info__delivery_city
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead__broadband_delivery_city
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__delivery_city
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead__mobile_1_delivery_city
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_line__broadband_isp_info_delivery_city
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_line__mobile_isp_info_delivery_city
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__delivery_city
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_service_contract_info__delivery_city
 #: model:ir.model.fields,field_description:somconnexio.field_partner_create_lead_wizard__delivery_city
 msgid "Delivery City"
 msgstr "Localitat"
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_base_isp_info__delivery_country_id
 #: model:ir.model.fields,field_description:somconnexio.field_broadband_isp_info__delivery_country_id
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__delivery_country_id
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__delivery_country_id
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_service_contract_info__delivery_country_id
 #: model:ir.model.fields,field_description:somconnexio.field_partner_create_lead_wizard__delivery_country_id
 msgid "Delivery Country"
 msgstr "País"
 
 #. module: somconnexio
@@ -3553,25 +3567,27 @@
 msgstr "Generant enviament"
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_base_isp_info__delivery_state_id
 #: model:ir.model.fields,field_description:somconnexio.field_broadband_isp_info__delivery_state_id
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead__broadband_delivery_state_id
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead__mobile_1_delivery_state_id
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__delivery_state_id
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_line__broadband_isp_info_delivery_state_id
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_line__mobile_isp_info_delivery_state_id
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__delivery_state_id
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_service_contract_info__delivery_state_id
 #: model:ir.model.fields,field_description:somconnexio.field_partner_create_lead_wizard__delivery_state_id
 msgid "Delivery State"
 msgstr "Província"
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_base_isp_info__delivery_street
 #: model:ir.model.fields,field_description:somconnexio.field_broadband_isp_info__delivery_street
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__delivery_street
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead__broadband_delivery_street
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead__mobile_1_delivery_street
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_line__broadband_isp_info_delivery_street
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_line__mobile_isp_info_delivery_street
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__delivery_street
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_service_contract_info__delivery_street
 #: model:ir.model.fields,field_description:somconnexio.field_partner_create_lead_wizard__delivery_street
@@ -3594,22 +3610,24 @@
 #: model:ir.model.fields,field_description:somconnexio.field_base_isp_info__delivery_zip_code
 #: model:ir.model.fields,field_description:somconnexio.field_broadband_isp_info__delivery_zip_code
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead__mobile_1_delivery_zip_code
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_line__mobile_isp_info_delivery_zip_code
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__delivery_zip_code
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_service_contract_info__delivery_zip_code
 #: model:ir.model.fields,field_description:somconnexio.field_partner_create_lead_wizard__delivery_zip_code
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__delivery_zip_code
 msgid "Delivery ZIP"
 msgstr "Codi postal"
 
 #. module: somconnexio
 #: model_terms:ir.ui.view,arch_db:somconnexio.broadband_isp_info_form
 #: model_terms:ir.ui.view,arch_db:somconnexio.crm_case_form_view_pack
 #: model_terms:ir.ui.view,arch_db:somconnexio.mobile_isp_info_form
 #: model_terms:ir.ui.view,arch_db:somconnexio.mobile_service_contract_info_form_view
+#: model_terms:ir.ui.view,arch_db:somconnexio.view_form_crm_lead_add_mobile_line_wizard
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_lead_line_broadband
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_lead_line_mobile
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_partner_create_lead_wizard
 msgid "Delivery address"
 msgstr "Adreça d'enviament"
 
 #. module: somconnexio
@@ -3626,14 +3644,15 @@
 #: model:ir.model.fields,field_description:somconnexio.field_contract_address_change_wizard__display_name
 #: model:ir.model.fields,field_description:somconnexio.field_partner_email_change_wizard__display_name
 #: model:ir.model.fields,field_description:somconnexio.field_contract_holder_change_wizard__display_name
 #: model:ir.model.fields,field_description:somconnexio.field_contract_iban_change_wizard__display_name
 #: model:ir.model.fields,field_description:somconnexio.field_contract_one_shot_request_wizard__display_name
 #: model:ir.model.fields,field_description:somconnexio.field_contract_tariff_change_wizard__display_name
 #: model:ir.model.fields,field_description:somconnexio.field_coop_agreement__display_name
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__display_name
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_validate_wizard__display_name
 #: model:ir.model.fields,field_description:somconnexio.field_discovery_channel__display_name
 #: model:ir.model.fields,field_description:somconnexio.field_invoice_claim_1_send_wizard__display_name
 #: model:ir.model.fields,field_description:somconnexio.field_mm_fiber_service_contract_info__display_name
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__display_name
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_service_contract_info__display_name
 #: model:ir.model.fields,field_description:somconnexio.field_move_line_add_to_payment_debit_order__display_name
@@ -3900,14 +3919,24 @@
 
 #. module: somconnexio
 #: selection:broadband.isp.info,previous_service:0
 msgid "Fiber"
 msgstr "Fibra"
 
 #. module: somconnexio
+#: model:ir.model.fields,field_description:somconnexio.field_contract_holder_change_wizard__fiber_contract_to_link
+msgid "Fiber contract to link"
+msgstr "Contracte de fibra per vincular"
+
+#. module: somconnexio
+#: model:ir.model.fields,field_description:somconnexio.field_contract_mobile_tariff_change_wizard__pack_options
+msgid "Fiber linked options"
+msgstr "Opcions de tarifes mòbils vinculades a una fibra"
+
+#. module: somconnexio
 #: model:mail.activity.type,name:somconnexio.mail_activity_type_fiber_mm_incident
 msgid "Fiber MM Incident"
 msgstr "Incidència Fibra MM"
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_contract_contract__fiber_signal_type_id
 msgid "Fiber Signal Type"
@@ -4078,22 +4107,24 @@
 #, python-format
 msgid "IBAN changed from {} to {} in partner's contract/s '{}'"
 msgstr "Canvi d'IBAN ({} --> {}) en el/s contracte/s '{}' d'aquesta sòcia"
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_contract_contract__icc
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead__mobile_1_icc
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__icc
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_line__mobile_isp_info_icc
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__icc
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_service_contract_info__icc
 #: model:ir.model.fields,field_description:somconnexio.field_partner_create_lead_wizard__icc
 msgid "ICC"
 msgstr "ICC"
 
 #. module: somconnexio
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__donor_icc
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__icc_donor
 #: model:ir.model.fields,field_description:somconnexio.field_partner_create_lead_wizard__donor_icc
 msgid "ICC Donor"
 msgstr "ICC donant"
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_adsl_service_contract_info__id
@@ -4104,14 +4135,15 @@
 #: model:ir.model.fields,field_description:somconnexio.field_contract_address_change_wizard__id
 #: model:ir.model.fields,field_description:somconnexio.field_partner_email_change_wizard__id
 #: model:ir.model.fields,field_description:somconnexio.field_contract_holder_change_wizard__id
 #: model:ir.model.fields,field_description:somconnexio.field_contract_iban_change_wizard__id
 #: model:ir.model.fields,field_description:somconnexio.field_contract_one_shot_request_wizard__id
 #: model:ir.model.fields,field_description:somconnexio.field_contract_tariff_change_wizard__id
 #: model:ir.model.fields,field_description:somconnexio.field_coop_agreement__id
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__id
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_validate_wizard__id
 #: model:ir.model.fields,field_description:somconnexio.field_discovery_channel__id
 #: model:ir.model.fields,field_description:somconnexio.field_invoice_claim_1_send_wizard__id
 #: model:ir.model.fields,field_description:somconnexio.field_mm_fiber_service_contract_info__id
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__id
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_service_contract_info__id
 #: model:ir.model.fields,field_description:somconnexio.field_move_line_add_to_payment_debit_order__id
@@ -4401,14 +4433,15 @@
 #: selection:xoln.fiber.service.contract.info,project:0
 msgid "La Borda"
 msgstr "La Borda"
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_broadband_isp_info__keep_phone_number
 #: model:ir.model.fields,field_description:somconnexio.field_partner_create_lead_wizard__keep_landline
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__keep_landline
 msgid "Keep Phone Number"
 msgstr "Conservar número de telèfon"
 
 #. module: somconnexio
 #: model_terms:ir.ui.view,arch_db:somconnexio.sim_sending_letter_lang_template
 msgid "La SIM té activat el <strong>límit de consum a 36€ IVA Inclòs</strong> per sobre de la tarifa contractada, però ens pots demanar que el baixem o que el pugem. Aquesta limitació serveix per impedir que es faci un consum superior al límit establert per causes imprevistes."
 msgstr "La SIM té activat el <strong>límit de consum a 36€ IVA Inclòs</strong> per sobre de la tarifa contractada, però ens pots demanar que el baixem o que el pugem. Aquesta limitació serveix per impedir que es faci un consum superior al límit establert per causes imprevistes."
@@ -4432,14 +4465,15 @@
 #: model:ir.model.fields,field_description:somconnexio.field_contract_address_change_wizard____last_update
 #: model:ir.model.fields,field_description:somconnexio.field_partner_email_change_wizard____last_update
 #: model:ir.model.fields,field_description:somconnexio.field_contract_holder_change_wizard____last_update
 #: model:ir.model.fields,field_description:somconnexio.field_contract_iban_change_wizard____last_update
 #: model:ir.model.fields,field_description:somconnexio.field_contract_one_shot_request_wizard____last_update
 #: model:ir.model.fields,field_description:somconnexio.field_contract_tariff_change_wizard____last_update
 #: model:ir.model.fields,field_description:somconnexio.field_coop_agreement____last_update
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard____last_update
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_validate_wizard____last_update
 #: model:ir.model.fields,field_description:somconnexio.field_discovery_channel____last_update
 #: model:ir.model.fields,field_description:somconnexio.field_invoice_claim_1_send_wizard____last_update
 #: model:ir.model.fields,field_description:somconnexio.field_mm_fiber_service_contract_info____last_update
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info____last_update
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_service_contract_info____last_update
 #: model:ir.model.fields,field_description:somconnexio.field_move_line_add_to_payment_debit_order____last_update
@@ -5074,14 +5108,20 @@
 
 #. module: somconnexio
 #: model:ir.actions.act_window,name:somconnexio.act_contract_contract_pack_related_contracts
 msgid "Pack contracts"
 msgstr "Contractes vinculats"
 
 #. module: somconnexio
+#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:158
+#, python-format
+msgid "Pack with fiber"
+msgstr "Apinyar a una fibra"
+
+#. module: somconnexio
 #: code:addons/somconnexio/models/aged_partner_balance.py:14
 #: code:addons/somconnexio/models/aged_partner_balance_xlsx.py:10
 #: code:addons/somconnexio/models/aged_partner_balance_xlsx.py:70
 #: code:addons/somconnexio/wizards/account_financial_report/aged_partner_balance.py:8
 #: selection:aged.partner.balance.wizard,group_by_select:0
 #: model:ir.model.fields,field_description:somconnexio.field_contract_address_change_wizard__partner_id
 #: model:ir.model.fields,field_description:somconnexio.field_partner_email_change_wizard__partner_id
@@ -5225,14 +5265,15 @@
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_line__broadband_isp_info_phone_number
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_line__mobile_isp_info_phone_number
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__phone_number
 #: model:ir.model.fields,field_description:somconnexio.field_adsl_service_contract_info__phone_number
 #: model:ir.model.fields,field_description:somconnexio.field_base_service_contract_info__phone_number
 #: model:ir.model.fields,field_description:somconnexio.field_broadband_service_contract_info__phone_number
 #: model:ir.model.fields,field_description:somconnexio.field_mm_fiber_service_contract_info__phone_number
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__phone_number
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_service_contract_info__phone_number
 #: model:ir.model.fields,field_description:somconnexio.field_orange_fiber_service_contract_info__phone_number
 #: model:ir.model.fields,field_description:somconnexio.field_partner_create_lead_wizard__phone_number
 #: model:ir.model.fields,field_description:somconnexio.field_router_4g_service_contract_info__phone_number
 #: model:ir.model.fields,field_description:somconnexio.field_vodafone_fiber_service_contract_info__phone_number
 #: model:ir.model.fields,field_description:somconnexio.field_xoln_fiber_service_contract_info__phone_number
 msgid "Phone Number"
@@ -5313,14 +5354,15 @@
 #. module: somconnexio
 #: selection:mobile.isp.info,previous_contract_type:0
 #: selection:partner.create.lead.wizard,previous_contract_type:0
 msgid "Prepaid"
 msgstr "Prepagament"
 
 #. module: somconnexio
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__previous_contract_type
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__previous_contract_type
 #: model:ir.model.fields,field_description:somconnexio.field_partner_create_lead_wizard__previous_contract_type
 msgid "Previous Contract Type"
 msgstr "Tipus de contracte anterior"
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_adsl_service_contract_info__previous_id
@@ -5330,44 +5372,48 @@
 #: model:ir.model.fields,field_description:somconnexio.field_vodafone_fiber_service_contract_info__previous_id
 msgid "Previous Id"
 msgstr "Id antic"
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_base_isp_info__previous_owner_first_name
 #: model:ir.model.fields,field_description:somconnexio.field_broadband_isp_info__previous_owner_first_name
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__previous_owner_first_name
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__previous_owner_first_name
 #: model:ir.model.fields,field_description:somconnexio.field_partner_create_lead_wizard__previous_owner_first_name
 msgid "Previous Owner First Name"
 msgstr "Nom del propietari anterior"
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_base_isp_info__previous_owner_name
 #: model:ir.model.fields,field_description:somconnexio.field_broadband_isp_info__previous_owner_name
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__previous_owner_name
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__previous_owner_name
 #: model:ir.model.fields,field_description:somconnexio.field_partner_create_lead_wizard__previous_owner_name
 msgid "Previous Owner Name"
 msgstr "Cognom del propietari anterior"
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_base_isp_info__previous_owner_vat_number
 #: model:ir.model.fields,field_description:somconnexio.field_broadband_isp_info__previous_owner_vat_number
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__previous_owner_vat_number
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__previous_owner_vat_number
 #: model:ir.model.fields,field_description:somconnexio.field_partner_create_lead_wizard__previous_owner_vat_number
 msgid "Previous Owner VatNumber"
 msgstr "DNI propietari anterior"
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_contract_address_change_wizard__previous_product_id
 msgid "Previous Product"
 msgstr "Producte previ"
 
 #. module: somconnexio
 #: model:ir.actions.act_window,name:somconnexio.previous_provider_act_view
 #: model:ir.model.fields,field_description:somconnexio.field_base_isp_info__previous_provider
 #: model:ir.model.fields,field_description:somconnexio.field_broadband_isp_info__previous_provider
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__previous_mobile_provider
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__previous_provider
 #: model:ir.model.fields,field_description:somconnexio.field_partner_create_lead_wizard__previous_mobile_provider
 #: model:ir.model.fields,field_description:somconnexio.field_partner_create_lead_wizard__previous_BA_provider
 #: model:ir.ui.menu,name:somconnexio.previous_provider_menu
 msgid "Previous Provider"
 msgstr "Proveïdor previ"
 
@@ -5588,14 +5634,15 @@
 #: code:addons/somconnexio/models/aged_partner_balance_xlsx.py:74
 #, python-format
 msgid "Residual"
 msgstr "Pendent"
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_contract_address_change_wizard__product_id
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__product_id
 #: model:ir.model.fields,field_description:somconnexio.field_partner_create_lead_wizard__product_id
 msgid "Requested product"
 msgstr "Producte sol·licitat"
 
 #. module: somconnexio
 #: model_terms:ir.ui.view,arch_db:somconnexio.crm_case_form_view_pack
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_lead_line_broadband
@@ -6528,14 +6575,15 @@
 msgid "Trying to add changes that would need to divide the customer account hierarchy from customer with code {} . "
 msgstr "Intentant afegir canvis en una subscripció de la sòcia amb codi {} que podrien dividir la seva jerarquia."
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_base_isp_info__type
 #: model:ir.model.fields,field_description:somconnexio.field_broadband_isp_info__type
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead__broadband_type
+#: model:ir.model.fields,field_description:somconnexio.field_crm_lead_add_mobile_line_wizard__type
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead__mobile_1_type
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_line__broadband_isp_info_type
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_line__mobile_isp_info_type
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__type
 #: model:ir.model.fields,field_description:somconnexio.field_partner_create_lead_wizard__type
 #: model:ir.model.fields,field_description:somconnexio.field_subscription_request__type
 msgid "Type"
```

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/i18n/es.po` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/i18n/es.po`

 * *Files 0% similar despite different names*

```diff
@@ -2425,15 +2425,15 @@
 #: code:addons/somconnexio/models/res_partner.py:260
 #: code:addons/somconnexio/models/subscription_request.py:209
 #, python-format
 msgid "A partner with VAT %s already exists in our system"
 msgstr "Ya existe un contacto con VAT %s en el sistema"
 
 #. module: somconnexio
-#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:309
+#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:342
 #, python-format
 msgid "A new shared bond creation cannot be an exceptional change"
 msgstr "Un cambio de tarifa para un nuevo bono compartido no puede ser excepcional"
 
 #. module: somconnexio
 #: selection:broadband.isp.info,previous_service:0
 msgid "ADSL"
@@ -2675,14 +2675,20 @@
 
 #. module: somconnexio
 #: model_terms:ir.ui.view,arch_db:somconnexio.report_aged_partner_balance_move_lines
 msgid "Amount due"
 msgstr "Deuda vencida"
 
 #. module: somconnexio
+#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:346
+#, python-format
+msgid "Another mobile is required to create a shared data bond"
+msgstr "Necessitas como mínimo otro móvil para crear un bono de datos compartido"
+
+#. module: somconnexio
 #: model_terms:ir.ui.view,arch_db:somconnexio.new_sim_sending_letter_lang_template
 msgid "Aquí tens la nova SIM de Som Connexió per a la línia"
 msgstr "Aquí tienes la nueva SIM de Somos Conexión para la línea"
 
 #. module: somconnexio
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_lead_line_broadband
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_lead_line_mobile
@@ -3326,15 +3332,15 @@
 msgstr "Crear líneas de pago"
 
 #. module: somconnexio
 #: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:148
 #: model:shared.bond.type,name:somconnexio.new_shared_bond
 #, python-format
 msgid "Create new shared bond"
-msgstr "Crear un bono nuevo"
+msgstr "Crear un bono de datos compartidos"
 
 #. module: somconnexio
 #: model:ir.model,name:somconnexio.model_move_line_add_to_payment_debit_order
 msgid "Create payment lines from account move line tree view"
 msgstr "Crear línieas de pago de la lista formulario de apuntes contables"
 
 #. module: somconnexio
@@ -3939,14 +3945,24 @@
 
 #. module: somconnexio
 #: selection:broadband.isp.info,previous_service:0
 msgid "Fiber"
 msgstr "Fibra"
 
 #. module: somconnexio
+#: model:ir.model.fields,field_description:somconnexio.field_contract_holder_change_wizard__fiber_contract_to_link
+msgid "Fiber contract to link"
+msgstr "Contrato de fibra para vincular"
+
+#. module: somconnexio
+#: model:ir.model.fields,field_description:somconnexio.field_contract_mobile_tariff_change_wizard__pack_options
+msgid "Fiber linked options"
+msgstr "Opciones de tarifas móviles vinculadas a una fibra"
+
+#. module: somconnexio
 #: model:mail.activity.type,name:somconnexio.mail_activity_type_fiber_mm_incident
 msgid "Fiber MM Incident"
 msgstr "Incidencia Fibra MM"
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_contract_contract__fiber_signal_type_id
 msgid "Fiber Signal Type"
@@ -5255,14 +5271,20 @@
 
 #. module: somconnexio
 #: model:ir.actions.act_window,name:somconnexio.act_contract_contract_pack_related_contracts
 msgid "Pack contracts"
 msgstr "Contratos vinculados"
 
 #. module: somconnexio
+#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:158
+#, python-format
+msgid "Pack with fiber"
+msgstr "Apiñar a una fibra"
+
+#. module: somconnexio
 #: code:addons/somconnexio/models/aged_partner_balance.py:14
 #: code:addons/somconnexio/models/aged_partner_balance_xlsx.py:10
 #: code:addons/somconnexio/models/aged_partner_balance_xlsx.py:70
 #: code:addons/somconnexio/wizards/account_financial_report/aged_partner_balance.py:8
 #: selection:aged.partner.balance.wizard,group_by_select:0
 #: model:ir.model.fields,field_description:somconnexio.field_contract_address_change_wizard__partner_id
 #: model:ir.model.fields,field_description:somconnexio.field_partner_email_change_wizard__partner_id
@@ -6283,19 +6305,14 @@
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_contract_mobile_tariff_change_wizard__shared_bond_id_to_join
 msgid "Shared bond id to join option"
 msgstr "A qué bono compartido la queremos añadir?"
 
 #. module: somconnexio
-#: model:ir.model.fields,field_description:somconnexio.field_contract_mobile_tariff_change_wizard__sharing_data_options
-msgid "Sharing bond option"
-msgstr "Opciones per compartir datos móviles"
-
-#. module: somconnexio
 #: model_terms:ir.ui.view,arch_db:somconnexio.sim_sending_letter_lang_template
 msgid "Si tens qualsevol dubte, posa’t en contacte amb l’equip de treball... ens fa molta il·lusió atendre’t,<br/><br/>\n"
 "                    <strong>Telèfon</strong>:<br/><br/>\n"
 "                    93 131 17 28 (de dilluns a divendres de 10h a 14h)<br/>\n"
 "                    693 761 723 (només per urgències, de 9h a 21h, tots els dies de la setmana)<br/><br/>\n"
 "                    Si tens una urgència fora d’aquest horari, envia un correu electrònic amb la paraula URGENT a l’assumpte, a:<br/>"
 msgstr "Si tienes cualquier duda, ponte en contacto con el equipo de trabajo, nos ilusiona atenderte,<br/><br/>\n"
@@ -7481,7 +7498,13 @@
 #, python-format
 msgid "Partner tags"
 msgstr "Etiquetes del contacte"
 
 #: model_terms:ir.ui.view,arch_db:contract.contract_contract_form_view
 msgid "Recurring Invoices"
 msgstr "Productos"
+
+#. module: somconnexio
+#: model:ir.actions.act_window,name:somconnexio.action_crm_lead_add_mobile_line_wizard
+#: model_terms:ir.ui.view,arch_db:somconnexio.view_lead_create_mobile_lines_wizard_button
+msgid "Add mobile line to CRM Lead"
+msgstr "Añadir línea móvil"
```

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/listeners/contract_line_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/listeners/contract_line_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/listeners/contract_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/listeners/contract_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/listeners/crm_lead_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/listeners/crm_lead_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/listeners/partner_bank_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/listeners/partner_bank_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/listeners/partner_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/listeners/partner_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.8.4/post-create-copy-contract-service-info.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.8.4/post-create-copy-contract-service-info.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.8.4/pre-create-one-gb-wo-cost.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.8.4/pre-create-one-gb-wo-cost.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.9/post-link-crm-to-contract.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.9/post-link-crm-to-contract.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.9/pre-migrate-change-address.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.9/pre-migrate-change-address.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.9/pre-uniform-contracts-wo-number.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.9/pre-uniform-contracts-wo-number.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.9.13/post-change-activities-user.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.9.13/post-change-activities-user.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.9.2/post-upper-sponsorship-code.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.9.2/post-upper-sponsorship-code.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.1.9.9/post-import-es-geonames.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.1.9.9/post-import-es-geonames.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.2.0.0/post-relate-is-from-not-pack-attribute-with-existing-products.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.2.0.0/post-relate-is-from-not-pack-attribute-with-existing-products.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-create-is-from-pack-attribute.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-create-is-from-pack-attribute.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-set-xml-id-unlimited-20GB.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-set-xml-id-unlimited-20GB.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.2.1.6/post-set-state_id.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.2.1.6/post-set-state_id.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/12.0.2.2.0/pre-fix-catalog-externalId.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/12.0.2.2.0/pre-fix-catalog-externalId.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/erppeek/README.md` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/erppeek/README.md`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/migrations/erppeek/update_contract_line_product_id.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/migrations/erppeek/update_contract_line_product_id.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/__init__.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/account_asset.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/account_asset.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/account_banking_mandate.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/account_banking_mandate.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/account_invoice.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/account_invoice.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/account_invoice_line.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/account_invoice_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/account_move_line.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/account_move_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/account_payment_order.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/account_payment_order.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/account_payment_return_email_gateway.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/account_payment_return_email_gateway.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/aged_partner_balance.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/aged_partner_balance.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/aged_partner_balance_xlsx.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/aged_partner_balance_xlsx.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/contract.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/contract.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/contract_info/base.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/contract_info/base.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/contract_info/broadband.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/contract_info/broadband.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/contract_info/mobile.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/contract_info/mobile.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/coop_agreement.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/coop_agreement.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/crm_lead.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/crm_lead.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/hr_employee.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/hr_employee.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/ir_model_data.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/ir_model_data.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/ir_server_action.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/ir_server_action.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/isp_info/base.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/isp_info/base.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/isp_info/broadband.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/isp_info/broadband.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/isp_info/mobile.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/isp_info/mobile.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/l10n_es_aeat_report.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/l10n_es_aeat_report.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/mail_activity.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/mail_activity.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/mass_mailing.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/mass_mailing.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/mobile_contract_otrs_view.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/mobile_contract_otrs_view.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/opencell_configuration.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/opencell_configuration.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/partner_action_tag.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/partner_action_tag.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/partner_otrs_view.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/partner_otrs_view.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/payment_return.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/payment_return.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/payment_return_line.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/payment_return_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/product_product.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/product_product.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/product_template.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/product_template.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/res_company.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/res_company.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/res_partner.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/res_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/stock_move_line.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/stock_move_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/stock_production_lot.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/stock_production_lot.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/models/subscription_request.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/models/subscription_request.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_models/account_hierarchy_resource.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_models/account_hierarchy_resource.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_models/crm_account_hierarchy.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_models/crm_account_hierarchy.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_models/customer.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_models/customer.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_models/services.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_models/services.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_models/subscription.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_models/subscription.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_strategies.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_strategies.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_strategies.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_strategies.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_services/customer_update_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_services/customer_update_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/opencell_services/subscription_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/opencell_services/subscription_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/otrs_factories/adsl_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/otrs_factories/adsl_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/otrs_factories/base_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/otrs_factories/base_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/otrs_factories/broadband_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/otrs_factories/broadband_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/otrs_factories/customer_data_from_res_partner.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/otrs_factories/customer_data_from_res_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/otrs_factories/fiber_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/otrs_factories/fiber_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/otrs_factories/mobile_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/otrs_factories/mobile_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/otrs_factories/service_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/otrs_factories/service_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/otrs_factories/update_ticket_with_error.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/otrs_factories/update_ticket_with_error.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/account_asset_report_xls.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/account_asset_report_xls.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/aged_partner_balance.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/aged_partner_balance.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/crm_lead_creation_email_template.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/crm_lead_creation_email_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/invoice_claim_1_capital_template.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/invoice_claim_1_capital_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/invoice_claim_1_template.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/invoice_claim_1_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/mobile_can_be_linked_with_fiber_mail_template.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/mobile_can_be_linked_with_fiber_mail_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/mobile_linked_with_fiber_mail_template.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/mobile_linked_with_fiber_mail_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/new_sim_sending_letter_template.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/new_sim_sending_letter_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/report_paperformat.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/report_paperformat.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/sim_sending_letter_template.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/sim_sending_letter_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/reports/sponsor_sell_back_template.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/reports/sponsor_sell_back_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/security/ir.model.access.csv` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/security/ir.model.access.csv`

 * *Files 0% similar despite different names*

```diff
@@ -43,7 +43,8 @@
 access_hr_attendance,access_hr_attendance,model_hr_attendance,base.group_user,1,0,0,0
 access_hr_attendance_place,access_hr_attendance_place,model_hr_attendance_place,base.group_user,1,1,1,1
 access_partner_action_tag,access_partner_action_tag,model_partner_action_tag,base.group_user,1,1,1,1
 operation_request_terminate_reason,operation_request_terminate_reason,model_operation_request_terminate_reason,base.group_user,1,1,1,1
 date_range.access_date_range_date_range,date_range.date_range,date_range.model_date_range,base.group_user,1,1,1,1
 mail.access_mail_activity_user,mail.activity.user,model_mail_activity,base.group_user,1,1,1,0
 mail.access_mail_activity_manager,mail.activity.manager,model_mail_activity,base.group_system,1,1,1,1
+contract_mobile_tariff_change_wizard_available_fibers,contract.mobile.tariff.change.wizard.available.fibers,model_contract_mobile_tariff_change_wizard_available_fibers,base.group_user,1,1,1,1
```

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/__init__.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/account_invoice_process.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/account_invoice_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/account_payment_group_process.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/account_payment_group_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/bank_from_iban_getter.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/bank_from_iban_getter.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/change_partner_emails.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/change_partner_emails.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_change_tariff_process.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_change_tariff_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_contract_process.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_contract_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_contract_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_contract_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_email_change_process.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_email_change_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_iban_change_process.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_iban_change_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_one_shot_process.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_one_shot_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_process/adsl.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_process/adsl.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_process/ba.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_process/ba.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_process/base.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_process/base.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_process/fiber.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_process/fiber.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_process/mobile.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_process/mobile.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/contract_process/router4g.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/contract_process/router4g.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/crm_lead_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/crm_lead_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/discovery_channel_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/discovery_channel_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/get_activation_date.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/get_activation_date.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/partner_email_change_process.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/partner_email_change_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/product_catalog_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/product_catalog_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/provider_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/provider_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/res_partner_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/res_partner_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/schemas.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/schemas.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/services/subscription_request_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/services/subscription_request_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/somoffice/user.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/somoffice/user.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/description/activities.png` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/description/activities.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/description/broadband_contract.png` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/description/broadband_contract.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/description/broadband_lead_lines.png` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/description/broadband_lead_lines.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/description/emails.png` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/description/emails.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/description/mobile_contract.png` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/description/mobile_contract.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/description/mobile_lead_lines.png` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/description/mobile_lead_lines.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/description/packs.png` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/description/packs.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/img/sc-image.png` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/img/sc-image.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/src/js/holidays_highlighter.js` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/src/js/holidays_highlighter.js`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/src/js/many2many_tags_contract_email.js` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/src/js/many2many_tags_contract_email.js`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/src/js/many2one_tags_crm_lead_email.js` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/src/js/many2one_tags_crm_lead_email.js`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/src/js/my_attendances.js` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/src/js/my_attendances.js`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/static/src/xml/attendance.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/static/src/xml/attendance.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/common_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/common_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/correos_services/test_shipment.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/correos_services/test_shipment.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/factories.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/factories.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/helpers.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/listeners/test_contract_line_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/listeners/test_contract_line_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/listeners/test_contract_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/listeners/test_contract_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/listeners/test_crm_lead_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/listeners/test_crm_lead_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/listeners/test_partner_bank_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/listeners/test_partner_bank_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/listeners/test_partner_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/listeners/test_partner_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/listeners/test_res_partner_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/listeners/test_res_partner_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_account_invoice.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_account_invoice.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_account_move_line.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_account_move_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_account_payment_order.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_account_payment_order.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_account_payment_return_gateway.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_account_payment_return_gateway.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_broadband_isp_info.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_broadband_isp_info.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_contract.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_contract.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_coop_agreement.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_coop_agreement.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_crm_lead.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_crm_lead.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_hr_attendance_process.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_hr_attendance_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_mail_activity.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_mail_activity.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_mass_mailing.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_mass_mailing.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_mobile_isp_info.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_mobile_isp_info.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_opencell_configuration_wrapper.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_opencell_configuration_wrapper.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_payment_return.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_payment_return.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_previous_provider.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_previous_provider.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_product_category_technology_supplier.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_product_category_technology_supplier.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_product_product.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_product_product.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_product_template.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_product_template.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_production_lot.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_production_lot.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_res_partner.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_res_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_res_partner_bank.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_res_partner_bank.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_server_action.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_server_action.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_service_supplier.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_service_supplier.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_stock_move_line.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_stock_move_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/models/test_subscription_request.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/models/test_subscription_request.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_models/test_address.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_models/test_address.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_models/test_crm_account_hierarchy.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_models/test_crm_account_hierarchy.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_models/test_customer.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_models/test_customer.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_models/test_opencell_service_codes.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_models/test_opencell_service_codes.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_models/test_subscription.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_models/test_subscription.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_strategies.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_strategies.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_strategies.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_strategies.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_services/test_customer_update_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_services/test_customer_update_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/opencell_services/test_subscription_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/opencell_services/test_subscription_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/otrs_factories/test_adsl_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/otrs_factories/test_adsl_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/otrs_factories/test_customer_data_from_res_partner.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/otrs_factories/test_customer_data_from_res_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/otrs_factories/test_fiber_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/otrs_factories/test_fiber_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/otrs_factories/test_mobile_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/otrs_factories/test_mobile_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/otrs_factories/test_router_4G_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/otrs_factories/test_router_4G_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/otrs_factories/test_update_ticket_with_error.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/otrs_factories/test_update_ticket_with_error.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/sc_test_case.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/sc_test_case.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/contract_process/base_test_contract_process.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/contract_process/base_test_contract_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/contract_process/test_fiber_contract_process.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/contract_process/test_fiber_contract_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/contract_process/test_mobile_contract_process.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/contract_process/test_mobile_contract_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/contract_services/test_contract_contract_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/contract_services/test_contract_contract_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/contract_services/test_contract_count_controller.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/contract_services/test_contract_count_controller.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/contract_services/test_contract_get_fiber_contracts_to_pack_controller.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/contract_services/test_contract_get_fiber_contracts_to_pack_controller.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/contract_services/test_contract_search_controller.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/contract_services/test_contract_search_controller.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_account_invoice_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_account_invoice_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_change_partner_emails.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_change_partner_emails.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_contract_change_tariff_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_contract_change_tariff_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_contract_contract_process.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_contract_contract_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_contract_email_change_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_contract_email_change_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_contract_iban_change_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_contract_iban_change_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_contract_one_shot_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_contract_one_shot_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_crm_lead_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_crm_lead_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_discovery_channel_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_discovery_channel_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_get_activation_date.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_get_activation_date.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_mass_mailing_unsubscribe.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_mass_mailing_unsubscribe.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_partner_email_change_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_partner_email_change_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_product_catalog_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_product_catalog_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_provider_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_provider_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,17 @@
         response = self.http_get(url, params)
 
         self.assertEquals(response.status_code, 200)
         self.assertEquals(response.reason, "OK")
 
         content = json.loads(response.content.decode("utf-8"))
 
-        self.assertIn('providers', content)
-        self.assertIn('count', content)
-        self.assertEqual(content['count'], 58)
+        self.assertIn("providers", content)
+        self.assertIn("count", content)
+        self.assertEqual(content["count"], 59)
 
     @odoo.tools.mute_logger("odoo.addons.base_rest.http")
     def test_route_bad_mobile_search_parameter(self):
         url = "/api/provider?mobile=1"
 
         response = self.http_get(url)
 
@@ -55,22 +55,22 @@
         )
 
     def test_route_search_by_mobile(self):
         url = "/api/provider?mobile=true"
 
         content = self.http_get_content(url)
 
-        self.assertEquals(content["count"], 54)
+        self.assertEquals(content["count"], 55)
 
     def test_route_search_by_broadband(self):
         url = "/api/provider?broadband=true"
 
         content = self.http_get_content(url)
 
-        self.assertEquals(content["count"], 12)
+        self.assertEquals(content["count"], 13)
 
     def test_route_search_both_services(self):
         url = "/api/provider?mobile=true&broadband=true"
 
         content = self.http_get_content(url)
 
-        self.assertEquals(content["count"], 11)
+        self.assertEquals(content["count"], 12)
```

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_res_partner_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_res_partner_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_subscription_request_service.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_subscription_request_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/services/test_vat_normalizer.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/services/test_vat_normalizer.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/somoffice/test_user.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/somoffice/test_user.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_account_payment_line_create.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_account_payment_line_create.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_address_change_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_address_change_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_compensation_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_compensation_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_force_oc_integration_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_force_oc_integration_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_holder_change.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_holder_change.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_force_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_force_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_invoice_payment_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_invoice_payment_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_mobile_tariff_change_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_mobile_tariff_change_wizard.py`

 * *Files 7% similar despite different names*

```diff
@@ -137,105 +137,117 @@
             "You must check if any previous tariff change is found in OTRS",
             wizard.button_change
         )
 
     @patch("odoo.addons.somconnexio.wizards.contract_mobile_tariff_change.contract_mobile_tariff_change.ChangeTariffTicket")  # noqa
     @patch("odoo.addons.somconnexio.wizards.contract_mobile_tariff_change.contract_mobile_tariff_change.ChangeTariffExceptionalTicket")  # noqa
     @patch("odoo.addons.somconnexio.services.contract_contract_service.ContractService.get_fiber_contracts_to_pack")  # noqa
-    def test_wizard_mobile_tariff_change_bonified_product_ok(
+    def test_wizard_mobile_exceptional_tariff_change_ok(
             self, mock_get_fiber_contracts_to_pack,
             MockExceptionalChangeTariffTicket, MockChangeTariffTicket):
 
-        fiber_contract = self.env.ref("somconnexio.contract_fibra_600")
-
-        # Bonified mobile product available
-        mock_get_fiber_contracts_to_pack.return_value = [
-            {
-                "id": fiber_contract.id,
-                "code": fiber_contract.code
-            }
-        ]
-
-        pack_product = self.env.ref("somconnexio.TrucadesIllimitades20GBPack")
-        sharing_data_product = self.env.ref("somconnexio.50GBCompartides3mobils")
+        # No bonified mobile product available
+        mock_get_fiber_contracts_to_pack.side_effect = MissingError("")
 
         wizard = self.env['contract.mobile.tariff.change.wizard'].with_context(  # noqa
             active_id=self.contract.id
         ).sudo(
             self.user_admin
         ).create({
-            "new_tariff_product_id": pack_product.id,
+            "exceptional_change": True,
+            "new_tariff_product_id": self.new_product.id,
+            "send_notification": True,
             "otrs_checked": True,
         })
+
         wizard.button_change()
 
-        # Check bonified product available
-        self.assertIn(pack_product, wizard.available_products)
-        # Check sharing data product NOT available
-        self.assertNotIn(sharing_data_product, wizard.available_products)
+        expected_start_date = date.today()
 
-        MockChangeTariffTicket.assert_called_once_with(
+        self.assertEquals(wizard.start_date, expected_start_date)
+        MockExceptionalChangeTariffTicket.assert_called_once_with(
             self.partner_id.vat,
             self.partner_id.ref,
             {
                 "phone_number": self.contract.phone_number,
-                "new_product_code": pack_product.default_code,
+                "new_product_code": self.new_product.default_code,
                 "current_product_code": self.contract.current_tariff_product.default_code,  # noqa
-                "effective_date": date_to_str(first_day_next_month()),
+                "effective_date": date_to_str(expected_start_date),
                 "subscription_email": self.partner_id.email,
                 "language": self.partner_id.lang,
-                "fiber_linked": fiber_contract.code,
-                "send_notification": False,
+                "fiber_linked": False,
+                "send_notification": True,
             },
         )
-        MockChangeTariffTicket.return_value.create.assert_called_once()
-        MockExceptionalChangeTariffTicket.assert_not_called()
+        MockExceptionalChangeTariffTicket.return_value.create.assert_called_once()
+        MockChangeTariffTicket.assert_not_called()
 
     @patch("odoo.addons.somconnexio.wizards.contract_mobile_tariff_change.contract_mobile_tariff_change.ChangeTariffTicket")  # noqa
     @patch("odoo.addons.somconnexio.wizards.contract_mobile_tariff_change.contract_mobile_tariff_change.ChangeTariffExceptionalTicket")  # noqa
     @patch("odoo.addons.somconnexio.services.contract_contract_service.ContractService.get_fiber_contracts_to_pack")  # noqa
-    def test_wizard_mobile_exceptional_tariff_change_ok(
+    def test_wizard_mobile_tariff_change_bonified_product_ok(
             self, mock_get_fiber_contracts_to_pack,
             MockExceptionalChangeTariffTicket, MockChangeTariffTicket):
 
-        # No bonified mobile product available
-        mock_get_fiber_contracts_to_pack.side_effect = MissingError("")
+        fiber_contract = self.env.ref("somconnexio.contract_fibra_600")
+        pack_product = self.env.ref("somconnexio.TrucadesIllimitades20GBPack")
+
+        # Bonified mobile product available
+        mock_get_fiber_contracts_to_pack.return_value = [
+            {
+                "id": fiber_contract.id,
+                "code": fiber_contract.code
+            }
+        ]
 
         wizard = self.env['contract.mobile.tariff.change.wizard'].with_context(  # noqa
             active_id=self.contract.id
         ).sudo(
             self.user_admin
-        ).create({
-            "exceptional_change": True,
-            "new_tariff_product_id": self.new_product.id,
-            "send_notification": True,
-            "otrs_checked": True,
-        })
+        ).create(
+            {
+                "otrs_checked": True,
+                "pack_options": "pinya_mobile_tariff",
+            }
+        )
+        wizard.onchange_pack_options()
 
-        wizard.button_change()
+        self.assertEquals(
+            wizard.available_fiber_contracts,
+            fiber_contract
+        )
 
-        expected_start_date = date.today()
+        wizard.write(
+            {
+                "fiber_contract_to_link": fiber_contract.id,
+            }
+        )
 
-        self.assertEquals(wizard.start_date, expected_start_date)
-        MockExceptionalChangeTariffTicket.assert_called_once_with(
+        wizard.button_change()
+
+        mock_get_fiber_contracts_to_pack.assert_called_with(
+            partner_ref=self.partner_id.ref,
+            mobiles_sharing_data="true"
+        )
+        MockChangeTariffTicket.assert_called_once_with(
             self.partner_id.vat,
             self.partner_id.ref,
             {
                 "phone_number": self.contract.phone_number,
-                "new_product_code": self.new_product.default_code,
+                "new_product_code": pack_product.default_code,
                 "current_product_code": self.contract.current_tariff_product.default_code,  # noqa
-                "effective_date": date_to_str(expected_start_date),
+                "effective_date": date_to_str(first_day_next_month()),
                 "subscription_email": self.partner_id.email,
                 "language": self.partner_id.lang,
-                "fiber_linked": False,
-                "send_notification": True,
+                "fiber_linked": fiber_contract.code,
+                "send_notification": False,
             },
         )
-        MockExceptionalChangeTariffTicket.return_value.create.assert_called_once()
-        MockChangeTariffTicket.assert_not_called()
+        MockChangeTariffTicket.return_value.create.assert_called_once()
+        MockExceptionalChangeTariffTicket.assert_not_called()
 
     @patch("odoo.addons.somconnexio.wizards.contract_mobile_tariff_change.contract_mobile_tariff_change.ChangeTariffTicketSharedBond")  # noqa
     @patch("odoo.addons.somconnexio.services.contract_contract_service.ContractService.get_fiber_contracts_to_pack")  # noqa
     def test_wizard_mobile_new_shared_bond_tariff_change_all_new(
             self, mock_get_fiber_contracts_to_pack,
             MockSharedChangeTariffTicket):
 
@@ -254,50 +266,44 @@
         wizard = self.env['contract.mobile.tariff.change.wizard'].with_context(  # noqa
             active_id=self.contract.id
         ).sudo(
             self.user_admin
         ).create(
             {
                 "otrs_checked": True,
-                "sharing_data_options": "new_shared_bond",
-                # avoid not null constraint
-                "new_tariff_product_id": self.new_product.id,
+                "pack_options": "new_shared_bond",
             }
         )
-        wizard.onchange_sharing_data_options()
+        wizard.onchange_pack_options()
 
         self.assertEquals(
             set(wizard.mobile_contracts_wo_sharing_bond),
             set([mobile_contract, mobile_2_contract])
         )
-        self.assertEquals(
-            wizard.mobile_contracts_to_share_with,
-            self.contract
-        )
-        self.assertEquals(
-            wizard.fiber_contracts_wo_sharing_data_mobiles,
-            fiber_contract
+        self.assertIn(
+            fiber_contract,
+            wizard.available_fiber_contracts,
         )
         mock_get_fiber_contracts_to_pack.assert_called_with(
             partner_ref=self.partner_id.ref,
             mobiles_sharing_data="true"
         )
 
         wizard.write(
             {
-                "mobile_contracts_to_share_with": [(4, mobile_contract.id, 0)],
+                "mobile_contracts_to_share_data": [(4, mobile_contract.id, 0)],
                 "fiber_contract_to_link": fiber_contract.id,
             }
         )
-        wizard.onchange_mobile_contracts_to_share_with()
+        wizard.onchange_mobile_contracts_to_share_data()
         wizard.onchange_fiber_contract_to_link()
 
         # No other mobile added
         self.assertEquals(
-            set(wizard.mobile_contracts_to_share_with),
+            set(wizard.mobile_contracts_to_share_data),
             set([self.contract, mobile_contract])
         )
         self.assertEquals(wizard.new_tariff_product_id, shared_2_product)
 
         wizard.button_change()
 
         MockSharedChangeTariffTicket.assert_called_once_with(
@@ -313,15 +319,15 @@
                 "fiber_linked": fiber_contract.code,
                 "send_notification": False,
                 "contracts": [
                     {
                         "phone_number": contract.phone_number,
                         "current_product_code": contract.current_tariff_product.code,
                         "subscription_email": contract.email_ids[0].email,
-                    } for contract in wizard.mobile_contracts_to_share_with
+                    } for contract in wizard.mobile_contracts_to_share_data
                 ]
             },
         )
 
     @patch("odoo.addons.somconnexio.wizards.contract_mobile_tariff_change.contract_mobile_tariff_change.ChangeTariffTicketSharedBond")  # noqa
     @patch("odoo.addons.somconnexio.services.contract_contract_service.ContractService.get_fiber_contracts_to_pack")  # noqa
     def test_wizard_mobile_new_shared_bond_tariff_change_packed_fiber(
@@ -343,50 +349,44 @@
         wizard = self.env['contract.mobile.tariff.change.wizard'].with_context(  # noqa
             active_id=self.contract.id
         ).sudo(
             self.user_admin
         ).create(
             {
                 "otrs_checked": True,
-                "sharing_data_options": "new_shared_bond",
-                # avoid not null constraint
-                "new_tariff_product_id": self.new_product.id,
+                "pack_options": "new_shared_bond",
             }
         )
-        wizard.onchange_sharing_data_options()
+        wizard.onchange_pack_options()
 
         self.assertEquals(
-            set(wizard.mobile_contracts_wo_sharing_bond),
-            set([mobile_contract, mobile_pack_contract])
-        )
-        self.assertEquals(
-            wizard.fiber_contracts_wo_sharing_data_mobiles,
+            wizard.available_fiber_contracts,
             fiber_pack_contract
         )
         mock_get_fiber_contracts_to_pack.assert_called_with(
             partner_ref=self.partner_id.ref,
             mobiles_sharing_data="true"
         )
 
         wizard.write(
             {
-                "mobile_contracts_to_share_with": [(4, mobile_contract.id, 0)],
+                "mobile_contracts_to_share_data": [(4, mobile_contract.id, 0)],
                 "fiber_contract_to_link": fiber_pack_contract.id,
             }
         )
 
         # Pack mobile added automatically (onchange) because is linked to fiber
         wizard.onchange_fiber_contract_to_link()
         self.assertEquals(
-            set(wizard.mobile_contracts_to_share_with),
+            set(wizard.mobile_contracts_to_share_data),
             set([self.contract, mobile_contract, mobile_pack_contract])
         )
 
         # Pack mobile added automatically (onchange) because is linked to fiber
-        wizard.onchange_mobile_contracts_to_share_with()
+        wizard.onchange_mobile_contracts_to_share_data()
         self.assertEquals(wizard.new_tariff_product_id, shared_3_product)
 
         wizard.button_change()
 
         MockSharedChangeTariffTicket.assert_called_once_with(
             self.partner_id.vat,
             self.partner_id.ref,
@@ -400,15 +400,15 @@
                 "fiber_linked": fiber_pack_contract.code,
                 "send_notification": False,
                 "contracts": [
                     {
                         "phone_number": contract.phone_number,
                         "current_product_code": contract.current_tariff_product.code,
                         "subscription_email": contract.email_ids[0].email,
-                    } for contract in wizard.mobile_contracts_to_share_with
+                    } for contract in wizard.mobile_contracts_to_share_data
                 ]
             },
         )
 
     @patch("odoo.addons.somconnexio.services.contract_contract_service.ContractService.get_fiber_contracts_to_pack")  # noqa
     def test_wizard_mobile_new_shared_bond_tariff_too_many_mobiles(
             self, mock_get_fiber_contracts_to_pack):
@@ -427,58 +427,116 @@
         wizard = self.env['contract.mobile.tariff.change.wizard'].with_context(  # noqa
             active_id=self.contract.id
         ).sudo(
             self.user_admin
         ).create(
             {
                 "otrs_checked": True,
-                "sharing_data_options": "new_shared_bond",
-                # avoid not null constraint
-                "new_tariff_product_id": self.new_product.id,
+                "pack_options": "new_shared_bond",
             }
         )
-        wizard.onchange_sharing_data_options()
+        wizard.onchange_pack_options()
 
         self.assertEquals(
             set(wizard.mobile_contracts_wo_sharing_bond),
             set([mobile_contract, mobile_pack_contract])
         )
         self.assertEquals(
-            wizard.fiber_contracts_wo_sharing_data_mobiles,
+            wizard.available_fiber_contracts,
             fiber_pack_contract
         )
         mock_get_fiber_contracts_to_pack.assert_called_with(
             partner_ref=self.partner_id.ref,
             mobiles_sharing_data="true"
         )
 
         wizard.write(
             {
-                "mobile_contracts_to_share_with": [(4, mobile_contract.id, 0)],
+                "mobile_contracts_to_share_data": [(4, mobile_contract.id, 0)],
                 "fiber_contract_to_link": fiber_pack_contract.id,
             }
         )
         wizard.onchange_fiber_contract_to_link()
-        wizard.onchange_mobile_contracts_to_share_with()
+        wizard.onchange_mobile_contracts_to_share_data()
 
-        self.assertEquals(len(wizard.mobile_contracts_to_share_with), 3)
+        self.assertEquals(len(wizard.mobile_contracts_to_share_data), 3)
 
         other_mobile_contract = self.env["contract.contract"].create(self.vals_contract)
 
         wizard.write(
             {
-                "mobile_contracts_to_share_with": [(4, other_mobile_contract.id, 0)],
+                "mobile_contracts_to_share_data": [(4, other_mobile_contract.id, 0)],
             }
         )
 
         # On change: take a third mobile contract to pack with
         self.assertRaisesRegex(
             ValidationError,
             "Maximum 3 mobile contracts to build a shared data bond",
-            wizard.onchange_mobile_contracts_to_share_with,
+            wizard.onchange_mobile_contracts_to_share_data,
+        )
+
+    @patch("odoo.addons.somconnexio.wizards.contract_mobile_tariff_change.contract_mobile_tariff_change.ChangeTariffTicket")  # noqa
+    @patch("odoo.addons.somconnexio.services.contract_contract_service.ContractService.get_fiber_contracts_to_pack")  # noqa
+    def test_wizard_mobile_add_to_existing_shared_bond(
+            self, mock_get_fiber_contracts_to_pack, MockChangeTariffTicket):
+
+        fiber_sharing_contract = self.env.ref("somconnexio.contract_fibra_600_shared")
+        mobile_sharing_contract = self.env.ref(
+            "somconnexio.contract_mobile_il_20_shared_1")
+        mobile_contract = self.env.ref("somconnexio.contract_mobile_il_20")
+        shared_3_product = self.env.ref("somconnexio.50GBCompartides3mobils")
+
+        mock_get_fiber_contracts_to_pack.side_effect = MissingError("")
+
+        wizard = self.env['contract.mobile.tariff.change.wizard'].with_context(  # noqa
+            active_id=mobile_contract.id
+        ).sudo(
+            self.user_admin
+        ).create(
+            {
+                "otrs_checked": True,
+                "pack_options": "existing_shared_bond",
+            }
+        )
+        wizard.onchange_pack_options()
+
+        self.assertEquals(wizard.new_tariff_product_id, shared_3_product)
+
+        wizard.write(
+            {
+                "shared_bond_id_to_join": mobile_sharing_contract.shared_bond_id,
+            }
+        )
+
+        wizard.onchange_shared_bond_id_to_join()
+
+        self.assertEquals(wizard.fiber_contract_to_link, fiber_sharing_contract)
+
+        wizard.button_change()
+
+        MockChangeTariffTicket.assert_called_once_with(
+            self.partner_id.vat,
+            self.partner_id.ref,
+            {
+                "phone_number": mobile_contract.phone_number,
+                "new_product_code": shared_3_product.default_code,
+                "current_product_code": self.contract.current_tariff_product.default_code,  # noqa
+                "effective_date": date_to_str(first_day_next_month()),
+                "subscription_email": self.partner_id.email,
+                "language": self.partner_id.lang,
+                "fiber_linked": fiber_sharing_contract.code,
+                "send_notification": False,
+                "shared_bond_id": mobile_sharing_contract.shared_bond_id
+            },
+        )
+
+        mock_get_fiber_contracts_to_pack.assert_called_with(
+            partner_ref=self.partner_id.ref,
+            mobiles_sharing_data="true"
         )
 
     @patch("odoo.addons.somconnexio.services.contract_contract_service.ContractService.get_fiber_contracts_to_pack")  # noqa
     def test_wizard_mobile_no_shared_bond_options(
             self, mock_get_fiber_contracts_to_pack):
 
         # No fiber available
@@ -487,19 +545,17 @@
         wizard = self.env['contract.mobile.tariff.change.wizard'].with_context(  # noqa
             active_id=self.contract.id
         ).sudo(
             self.user_admin
         ).create(
             {
                 "otrs_checked": True,
-                # avoid not null constraint
-                "new_tariff_product_id": self.new_product.id,
             }
         )
 
-        self.assertFalse(wizard.fiber_contracts_wo_sharing_data_mobiles)
+        self.assertFalse(wizard.available_fiber_contracts)
 
         self.assertRaises(
             ValueError,
             wizard.write,
-            {"sharing_data_options": "new_shared_bond"}
+            {"pack_options": "new_shared_bond"}
         )
```

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_one_shot_request_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_one_shot_request_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_tariff_change_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_tariff_change_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_contract_terminate_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_contract_terminate_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_create_lead_from_partner_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_create_lead_from_partner_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_create_subscription_from_partner.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_create_subscription_from_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_crm_lead_generate_SIM_delivery_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_crm_lead_generate_SIM_delivery_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_crm_lead_remesa_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_crm_lead_remesa_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_crm_leads_validate_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_crm_leads_validate_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_mail_compose_message_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_mail_compose_message_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_partner_check_somoffice_email.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_partner_check_somoffice_email.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_partner_email_change_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_partner_email_change_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/tests/wizards/test_payment_order_generated_to_upload_queued_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/tests/wizards/test_payment_order_generated_to_upload_queued_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/account_asset_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/account_asset_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/account_invoice_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/account_invoice_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/account_move.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/account_move.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/account_move_line.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/account_move_line.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/account_payment_order_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/account_payment_order_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/adsl_service_contract_info_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/adsl_service_contract_info_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/aeat_report_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/aeat_report_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/broadband_isp_info_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/broadband_isp_info_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/contract_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/contract_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/coop_agreement_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/coop_agreement_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/crm_lead.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/crm_lead.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/crm_lead_line.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/crm_lead_line.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/hr_attendance.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/hr_attendance.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/ir_action_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/ir_action_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/mail_activity_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/mail_activity_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/mail_mail_statistics_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/mail_mail_statistics_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/menus.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/menus.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/mis_budget_item_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/mis_budget_item_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/mm_fiber_service_contract_info.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/mm_fiber_service_contract_info.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/mobile_isp_info_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/mobile_isp_info_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/mobile_service_contract_info_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/mobile_service_contract_info_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/open_boards_activities.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/open_boards_activities.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/operation_request.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/operation_request.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/partner_action_tag_views.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/partner_action_tag_views.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/payment_return_import_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/payment_return_import_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/payment_return_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/payment_return_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/previous_provider_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/previous_provider_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/product_attribute_views.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/product_attribute_views.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/product_category_technology_supplier_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/product_category_technology_supplier_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/product_pricelist_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/product_pricelist_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/product_product_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/product_product_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/res_company_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/res_company_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/res_partner_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/res_partner_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/router_4G_service_contract_info.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/router_4G_service_contract_info.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/service_technology_service_supplier.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/service_technology_service_supplier.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/stock_move_line_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/stock_move_line_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/subscription_request_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/subscription_request_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/templates_js.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/templates_js.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/vodafone_fiber_service_contract_info.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/vodafone_fiber_service_contract_info.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/views/xoln_fiber_service_contract_info.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/views/xoln_fiber_service_contract_info.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/account_financial_report/aged_partner_balance.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/account_financial_report/aged_partner_balance.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/account_invoice_confirm/account_invoice_confirm.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/account_invoice_confirm/account_invoice_confirm.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_force_oc_integration/contract_force_oc_integration.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_force_oc_integration/contract_force_oc_integration.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,70 @@
-from datetime import date
+from datetime import date, datetime, timedelta
+
+from odoo import _, api, fields, models
+from odoo.exceptions import MissingError, ValidationError
 from otrs_somconnexio.otrs_models.ticket_types.change_tariff_ticket import (
-    ChangeTariffTicket, ChangeTariffExceptionalTicket,
+    ChangeTariffExceptionalTicket,
+    ChangeTariffTicket,
 )
 from otrs_somconnexio.otrs_models.ticket_types.change_tariff_ticket_shared_bonds import (  # noqa
-    ChangeTariffTicketSharedBond
+    ChangeTariffTicketSharedBond,
 )
-from odoo import fields, api, models, _
-from odoo.exceptions import MissingError, ValidationError
 
+from ...helpers.date import date_to_str, first_day_next_month
 from ...services.contract_contract_service import ContractService
-from ...helpers.date import first_day_next_month, date_to_str
+
+
+class AvailableFibers(models.TransientModel):
+    # Why is a TransientModel?
+    # Is a hackish solution for a cache problem.
+    # We need a cache to store the information received from OTRS to avoid to call OTRS
+    # API every time the wizard is loaded.
+    # The default Odoo wizard load process execute many times the same methods without a
+    # common context between them.
+    # Using a TransientModel the vacumm remove automaticaly the old records.
+    # osv_memory_count_limit: Force a limit on the maximum number of records kept in the
+    # virtual osv_memory tables. The default is False, which means no count-based limit.
+    # _transient_max_count = lazy_classproperty(
+    #    lambda _: config.get("osv_memory_count_limit")
+    # )
+    # osv_memory_age_limit: Force a limit on the maximum age of records kept in the
+    # virtual osv_memory tables. This is a decimal value expressed in hours,
+    # and the default is 1 hour.
+    # _transient_max_hours = lazy_classproperty(
+    #     lambda _: config.get("osv_memory_age_limit")
+    # )
+    _name = "contract.mobile.tariff.change.wizard.available.fibers"
+
+    partner_ref = fields.Char()
+    fiber_contracts_ids = fields.Char()
 
 
 class ContractMobileTariffChangeWizard(models.TransientModel):
     _name = 'contract.mobile.tariff.change.wizard'
 
     contract_id = fields.Many2one('contract.contract')
     partner_id = fields.Many2one(
         'res.partner',
         related='contract_id.partner_id'
     )
     start_date = fields.Date('Start Date')
     note = fields.Char()
-    fiber_contract_code_to_link = fields.Char(
-        compute='_compute_fiber_contract_code_to_link',
-    )
     current_tariff_contract_line = fields.Many2one(
         'contract.line',
         related='contract_id.current_tariff_contract_line',
     )
     current_tariff_product = fields.Many2one(
         'product.product',
         related='current_tariff_contract_line.product_id',
         string="Current Tariff"
     )
-    has_mobile_pack_offer_text = fields.Selection(
-        [('yes', _('Yes')), ('no', 'No')],
-        string='Is mobile pack offer available?',
-        compute='_compute_has_mobile_pack_offer_text',
-        readonly=True
-    )
     new_tariff_product_id = fields.Many2one(
         'product.product',
         string='New tariff',
-        required=True
     )
     exceptional_change = fields.Boolean(default=False)
     send_notification = fields.Boolean(
         string='Send notification', default=False
     )
     otrs_checked = fields.Boolean(
         string='I have checked OTRS and no other tariff change is pending',
@@ -56,49 +73,49 @@
     available_products = fields.Many2many(
         "product.product",
         compute="_compute_available_products",
     )
     location = fields.Char(
         related='contract_id.phone_number'
     )
-    mobile_contracts_to_share_with = fields.Many2many(
+    mobile_contracts_to_share_data = fields.Many2many(
+        comodel_name="contract.contract",
+        inverse_name="id",
+        string="With which mobile contracts should it share data with?",
+    )
+    available_fiber_contracts = fields.Many2many(
         comodel_name='contract.contract',
         inverse_name="id",
-        string='With which mobile contracts should it share data with?',
+        relation="available_fiber_contracts_change_mobile_tariff_wizard_table"
     )
     fiber_contract_to_link = fields.Many2one(
         'contract.contract',
         string='To which fiber contract should be linked?',
     )
     mobile_contracts_wo_sharing_bond = fields.Many2many(
         'contract.contract',
         compute='_compute_mobile_contracts_wo_sharing_bond',
     )
-    fiber_contracts_wo_sharing_data_mobiles = fields.Many2many(
-        'contract.contract',
-        compute='_compute_fiber_contracts_wo_sharing_data_mobiles',
-    )
-    sharing_data_options = fields.Selection(
-        selection=lambda self: self._get_sharing_data_options(),
-        string='Sharing bond option',
+    pack_options = fields.Selection(
+        selection=lambda self: self._get_pack_options(),
+        string='Fiber linked options',
     )
     shared_bond_id_to_join = fields.Selection(
         selection=lambda self: self._get_shared_bond_id_to_join(),
         string='Shared bond id to join option',
     )
 
     @api.model
     def default_get(self, fields_list):
         defaults = super().default_get(fields_list)
         defaults['contract_id'] = self.env.context['active_id']
         return defaults
 
     def _get_shared_bond_id_to_join(self):
 
-        # TODO -> this method will be unused until existing_shared_bond is an option
         c_id = self.env.context.get('active_id')
         if not c_id:
             return
 
         contract_id = self.env["contract.contract"].browse(c_id)
 
         mobile_contracts_w_sharing_bond = self.env["contract.contract"].search(
@@ -109,92 +126,105 @@
                     "somconnexio.service_technology_mobile").id,
                  ),
                 ("is_terminated", "=", False),
             ]
         ).filtered(lambda c: len(c.sharing_bond_contract_ids) == 2)
 
         shared_bond_dict = {}
-        shared_bond_options = []
+        shared_bond_id_list = []
 
         for contract in mobile_contracts_w_sharing_bond:
             # Group contracts by code
             if contract.shared_bond_id in shared_bond_dict:
                 shared_bond_dict[contract.shared_bond_id].append(contract)
             else:
                 shared_bond_dict[contract.shared_bond_id] = [contract]
 
         # Gather phone numbers for contracts sharing the same shared_bond_id
         for shared_bond_id, contracts in shared_bond_dict.items():
-            shared_bond_options.append(
-                (shared_bond_id, ','.join(
-                    [contract.phone_number for contract in contracts]))
+            shared_bond_id_list.append(
+                (
+                    shared_bond_id,
+                    '{}: {}'.format(shared_bond_id, ', '.join(
+                        [contract.phone_number for contract in contracts]
+                    ))
+                )
             )
 
-        return shared_bond_options
+        return shared_bond_id_list
 
-    def _get_sharing_data_options(self):
-        c_id = self.env.context.get('active_id')
-        if not c_id:
-            return
+    def _get_pack_options(self):
 
+        c_id = self.env.context.get('active_id')
         contract_id = self.env["contract.contract"].browse(c_id)
 
-        sharing_data_options = []
+        pack_options = []
 
-        if contract_id.shared_bond_id:
-            return sharing_data_options
+        if not contract_id or contract_id.shared_bond_id or self.pack_options:
+            return pack_options
+
+        fiber_contracts_wo_sharing_data_mobiles = False
+        mobile_contracts_wo_sharing_bond = False
 
         mobile_contracts = self.env["contract.contract"].search(
             [
                 ("id", "!=", contract_id.id),
                 ("partner_id", "=", contract_id.partner_id.id),
                 ("service_technology_id", "=", self.env.ref(
                     "somconnexio.service_technology_mobile").id,
                  ),
                 ("is_terminated", "=", False),
             ]
         )
-        # mobile_contracts_w_sharing_bond = mobile_contracts.filtered(
-        #     lambda c: len(c.sharing_bond_contract_ids) == 2
-        # )
 
-        fiber_contracts_wo_sharing_data_mobiles = \
-            self._get_fiber_contracts_wo_sharing_data_mobiles(
-                contract_id.partner_id.ref
+        if mobile_contracts:
+            mobile_contracts_w_sharing_bond = mobile_contracts.filtered(
+                lambda c: len(c.sharing_bond_contract_ids) == 2
             )
 
-        # fiber_contracts_w_sharing_data_mobiles = fiber_contracts.filtered(
-        #     lambda c: len(c.children_pack_contract_ids) == 2
-        # )
+            if mobile_contracts_w_sharing_bond:
+                pack_options.append(
+                    ('existing_shared_bond', _('Add line to existing shared bond')),
+                )
+
+            mobile_contracts_wo_sharing_bond = mobile_contracts.filtered(
+                lambda c: not c.shared_bond_id
+            )
+
+        fiber_contracts_to_pack = self._get_fiber_contracts_to_pack(
+            contract_id.partner_id.ref
+        )
 
-        if (fiber_contracts_wo_sharing_data_mobiles and mobile_contracts):
-            sharing_data_options.append(
+        if fiber_contracts_to_pack:
+            fiber_contracts_unlinked = (
+                fiber_contracts_to_pack.filtered(
+                    lambda c: not c.children_pack_contract_ids
+                )
+            )
+            if fiber_contracts_unlinked:
+                pack_options.append(
+                    ('pinya_mobile_tariff', _('Pack with fiber')),
+                )
+
+            fiber_contracts_wo_sharing_data_mobiles = (
+                fiber_contracts_to_pack.filtered(
+                    lambda c: not c.children_pack_contract_ids
+                    or len(c.children_pack_contract_ids) == 1
+                )
+            )
+
+        if (
+            fiber_contracts_wo_sharing_data_mobiles and
+            mobile_contracts_wo_sharing_bond
+        ):
+            pack_options.append(
                 ('new_shared_bond', _('Create new shared bond')),
             )
-        # TODO -> decomment this code to add a mobile to an existing shared bond
-        # if (
-        #      fiber_contracts_w_sharing_data_mobiles and
-        #      mobile_contracts_w_sharing_bond
-        # ):
-        #     sharing_data_options.append(
-        #         ('existing_shared_bond', _('Add line to existing shared bond')),
-        #     )
-
-        return sharing_data_options
-
-    @api.depends("partner_id")
-    def _compute_fiber_contract_code_to_link(self):
-        if self.partner_id:
-            service = ContractService(self.env)
-            try:
-                fiber_contracts = service.get_fiber_contracts_to_pack(
-                    partner_ref=self.partner_id.ref)
-            except MissingError:
-                return
-            self.fiber_contract_code_to_link = fiber_contracts[0]['code']
+
+        return pack_options
 
     @api.depends("contract_id")
     def _compute_mobile_contracts_wo_sharing_bond(self):
         if not self.contract_id:
             return
         self.mobile_contracts_wo_sharing_bond = self.env["contract.contract"].search(
             [
@@ -203,113 +233,166 @@
                 ("service_technology_id", "=", self.env.ref(
                     "somconnexio.service_technology_mobile").id,
                  ),
                 ("is_terminated", "=", False),
             ]
         ).filtered(lambda c: not c.sharing_bond_contract_ids)
 
-    @api.depends("contract_id")
-    def _compute_fiber_contracts_wo_sharing_data_mobiles(self):
-        """
-        Returns all fiber contracts not linked to sharing data mobiles
-        They can be linked to a single bonified mobile contract
-        """
-        if not self.contract_id:
-            return
-
-        self.fiber_contracts_wo_sharing_data_mobiles = \
-            self._get_fiber_contracts_wo_sharing_data_mobiles(
-                self.partner_id.ref
-            )
-
-    @api.depends("fiber_contract_code_to_link")
-    def _compute_has_mobile_pack_offer_text(self):
-        if self.fiber_contract_code_to_link:
-            self.has_mobile_pack_offer_text = "yes"
-        else:
-            self.has_mobile_pack_offer_text = "no"
-
-    @api.depends("has_mobile_pack_offer_text")
+    @api.onchange('contract_id')
     def _compute_available_products(self):
-        if not self.has_mobile_pack_offer_text:
-            return
         mbl_product_templates = self.env["product.template"].search([
             ('categ_id', '=', self.env.ref('somconnexio.mobile_service').id),
         ])
         product_search_domain = [
             ("product_tmpl_id", "in", mbl_product_templates.ids),
             ("active", "=", True),
-            ('has_sharing_data_bond', '=', False),
-            ('attribute_value_ids', '!=', self.env.ref('somconnexio.IsInPack').id)
+            ("attribute_value_ids", "!=", self.env.ref("somconnexio.IsInPack").id)
         ]
-        if self.has_mobile_pack_offer_text == "yes":
-            del product_search_domain[-1]
-
         self.available_products = self.env['product.product'].search(
             product_search_domain
         )
 
     @api.onchange('shared_bond_id_to_join')
     def onchange_shared_bond_id_to_join(self):
-        if self.shared_bond_id_to_join:
-            self.new_tariff_product_id = self.env.ref(
-                'somconnexio.50GBCompartides3mobils').id
+        if not self.shared_bond_id_to_join:
+            return
+
+        chosen_shared_bond_id = self.shared_bond_id_to_join
+        mobile_contracts_to_join = self.env["contract.contract"].search(
+            [
+                ("partner_id", "=", self.partner_id.id),
+                ("service_technology_id", "=", self.env.ref(
+                    "somconnexio.service_technology_mobile").id,
+                 ),
+                ("is_terminated", "=", False),
+                ("shared_bond_id", "=", chosen_shared_bond_id),
+            ]
+        )
+        self.fiber_contract_to_link = (
+            mobile_contracts_to_join[0].parent_pack_contract_id
+        )
 
-    @api.onchange('mobile_contracts_to_share_with')
-    def onchange_mobile_contracts_to_share_with(self):
+    @api.onchange('mobile_contracts_to_share_data')
+    def onchange_mobile_contracts_to_share_data(self):
         # Assign shared product depending on how many contracts to share with
-        # mobile_contracts_to_share_with cannot be empty
-        if len(self.mobile_contracts_to_share_with) == 2:
+        # mobile_contracts_to_share_data cannot be empty
+        if len(self.mobile_contracts_to_share_data) == 2:
             self.new_tariff_product_id = (
-                self.env.ref('somconnexio.50GBCompartides2mobils').id
+                self.env.ref('somconnexio.50GBCompartides2mobils')
             )
-        elif len(self.mobile_contracts_to_share_with) == 3:
+        elif len(self.mobile_contracts_to_share_data) == 3:
             self.new_tariff_product_id = (
-                self.env.ref('somconnexio.50GBCompartides3mobils').id
+                self.env.ref('somconnexio.50GBCompartides3mobils')
             )
-        elif len(self.mobile_contracts_to_share_with) > 3:
+        elif len(self.mobile_contracts_to_share_data) > 3:
             raise ValidationError(_(
                 "Maximum 3 mobile contracts to build a shared data bond"
             ))
 
     @api.onchange('fiber_contract_to_link')
     def onchange_fiber_contract_to_link(self):
         if not self.fiber_contract_to_link:
             return
 
         # If chosen fiber is linked with mobile, that mobile contract should share data
-        if self.fiber_contract_to_link.children_pack_contract_ids:
+        if (
+            self.fiber_contract_to_link.children_pack_contract_ids and
+            self.pack_options == "new_shared_bond"
+        ):
             mobile_pack = self.fiber_contract_to_link.children_pack_contract_ids[0]
-            self.mobile_contracts_to_share_with = [(4, mobile_pack.id)]
+            self.mobile_contracts_to_share_data = [(4, mobile_pack.id)]
 
-    @api.onchange('sharing_data_options')
-    def onchange_sharing_data_options(self):
-        if self.sharing_data_options == "new_shared_bond":
-            self.mobile_contracts_to_share_with = [(4, self.contract_id.id)]
+    @api.onchange('pack_options')
+    def onchange_pack_options(self):
+        if self.pack_options == "pinya_mobile_tariff":
+            self.new_tariff_product_id = (
+                self.env.ref('somconnexio.TrucadesIllimitades20GBPack')
+            )
+            fiber_contracts_to_pack = (
+                self._get_fiber_contracts_to_pack(self.partner_id.ref)
+            )
+            self.available_fiber_contracts = fiber_contracts_to_pack.filtered(
+                lambda c: not c.children_pack_contract_ids
+            )
+            self.available_products = self.env.ref(
+                "somconnexio.TrucadesIllimitades20GBPack"
+            )
+        elif self.pack_options == "new_shared_bond":
+            self.mobile_contracts_to_share_data = [(6, _, [self.contract_id.id])]
+            self.new_tariff_product_id = (
+                self.env.ref('somconnexio.50GBCompartides2mobils')
+            )
+            fiber_contracts_to_pack = (
+                self._get_fiber_contracts_to_pack(self.partner_id.ref)
+            )
+            self.available_fiber_contracts = (
+                fiber_contracts_to_pack.filtered(
+                    lambda c: not c.children_pack_contract_ids
+                    or len(c.children_pack_contract_ids) == 1
+                )
+            )
+            self.available_products = self.env.ref(
+                "somconnexio.50GBCompartides3mobils"
+            ) | self.env.ref("somconnexio.50GBCompartides2mobils")
+        elif self.pack_options == "existing_shared_bond":
+            self.new_tariff_product_id = (
+                self.env.ref('somconnexio.50GBCompartides3mobils')
+            )
+            self.available_products = self.env.ref("somconnexio.50GBCompartides3mobils")
+        else:
+            self.new_tariff_product_id = False
 
-    def _get_fiber_contracts_wo_sharing_data_mobiles(self, partner_ref):
+    def _get_fiber_contracts_to_pack(self, partner_ref):
         """
-        Check fiber contracts available to link with mobile contracts sharing data
+        Check fiber contracts available to link with mobile contracts
         """
-        service = ContractService(self.env)
-        try:
-            fiber_contracts_dct = service.get_fiber_contracts_to_pack(
-                partner_ref=partner_ref,
-                mobiles_sharing_data="true")
-        except MissingError:
-            return
 
-        return self.env["contract.contract"].search(
+        fibers = self.env[
+            "contract.mobile.tariff.change.wizard.available.fibers"
+        ].search(
             [
-                ("id", "in", [c["id"] for c in fiber_contracts_dct])
-                ]
-            ).filtered(
-                lambda c: len(c.sharing_bond_contract_ids) == 1 or
-                not c.sharing_bond_contract_ids
-            )
+                ("partner_ref", "=", partner_ref),
+            ]
+        )
+        old_date = datetime.now() - timedelta(minutes=5)
+        old_register = fibers and fibers.write_date <= old_date
+
+        if not fibers or old_register:
+            service = ContractService(self.env)
+            try:
+                fiber_contracts_dct = service.get_fiber_contracts_to_pack(
+                    partner_ref=partner_ref, mobiles_sharing_data="true"
+                )
+                fiber_contracts_ids = [c["id"] for c in fiber_contracts_dct]
+            except MissingError:
+                return
+            fiber_contracts_id_list = " ".join([str(id) for id in fiber_contracts_ids])
+            if not fibers:
+                self.env[
+                    "contract.mobile.tariff.change.wizard.available.fibers"
+                ].create(
+                    [
+                        {
+                            "partner_ref": partner_ref,
+                            "fiber_contracts_ids": fiber_contracts_id_list,
+                        }
+                    ]
+                )
+            elif old_register:
+                fibers.write(
+                    {
+                        "fiber_contracts_ids": fiber_contracts_id_list,
+                    }
+                )
+        else:
+            fiber_contracts_ids = [
+                int(n) for n in fibers.fiber_contracts_ids.split(" ")
+            ]
+
+        return self.env["contract.contract"].search([("id", "in", fiber_contracts_ids)])
 
     def button_change(self):
         self.ensure_one()
 
         if not self.otrs_checked:
             raise ValidationError(_(
                 "You must check if any previous tariff change is found in OTRS"
@@ -325,44 +408,48 @@
         fields_dict = {
             "phone_number": self.contract_id.phone_number,
             "new_product_code": self.new_tariff_product_id.default_code,
             "current_product_code": self.current_tariff_product.default_code,
             "subscription_email": self.contract_id.email_ids[0].email,
             "effective_date": date_to_str(self.start_date),
             "language": self.partner_id.lang,
-            "fiber_linked": self.fiber_contract_code_to_link,
+            "fiber_linked": (
+                self.fiber_contract_to_link.code
+                if self.fiber_contract_to_link else False
+            ),
             "send_notification": self.send_notification,
         }
 
-        if self.fiber_contract_to_link:
-            fields_dict["fiber_linked"] = self.fiber_contract_to_link.code
+        if self.pack_options == 'existing_shared_bond':
+            fields_dict["shared_bond_id"] = self.shared_bond_id_to_join
 
-        if self.sharing_data_options == 'new_shared_bond':
+        elif self.pack_options == 'new_shared_bond':
             if self.exceptional_change:
                 raise ValidationError(_(
                     "A new shared bond creation cannot be an exceptional change"
                 ))
+            elif len(self.mobile_contracts_to_share_data) < 2:
+                raise ValidationError(_(
+                    "Another mobile is required to create a shared data bond"
+                ))
             Ticket = ChangeTariffTicketSharedBond
             fields_dict["contracts"] = [
                 {
                     "phone_number": contract.phone_number,
                     "current_product_code": contract.current_tariff_product.code,
                     "subscription_email": contract.email_ids[0].email,
-                } for contract in self.mobile_contracts_to_share_with
+                } for contract in self.mobile_contracts_to_share_data
             ]
 
-        elif self.sharing_data_options == 'existing_shared_bond':
-            fields_dict["shared_bond_id"] = self.shared_bond_id_to_join
-
         Ticket(self.partner_id.vat, self.partner_id.ref, fields_dict).create()
 
         message = _("OTRS change tariff ticket created. Tariff to be changed from '{}' to '{}' with start_date: {}")  # noqa
         self.contract_id.message_post(
             message.format(
-                self.current_tariff_contract_line.product_id.showed_name,
+                self.current_tariff_product.showed_name,
                 self.new_tariff_product_id.showed_name,
                 self.start_date,
             )
         )
         self._create_activity()
         return True
```

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.xml`

 * *Files 10% similar despite different names*

#### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.xml`

```diff
@@ -16,30 +16,29 @@
       <field name="name">Contract Mobile Tariff Change Wizard</field>
       <field name="model">contract.mobile.tariff.change.wizard</field>
       <field name="arch" type="xml">
         <form>
           <group>
             <field name="contract_id" invisible="1"/>
             <field name="available_products" invisible="1"/>
-            <field name="fiber_contracts_wo_sharing_data_mobiles" invisible="1"/>
+            <field name="available_fiber_contracts" invisible="1"/>
             <field name="mobile_contracts_wo_sharing_bond" invisible="1"/>
             <field name="exceptional_change"/>
             <field name="send_notification" attrs="{'invisible': [('exceptional_change','=',False)]}"/>
             <separator/>
-            <field name="has_mobile_pack_offer_text" widget="Radio"/>
-            <field name="sharing_data_options"/>
-            <field name="current_tariff_product" options="{'no_open': True,'no_create': 1,'no_create_edit': 1}" attrs="{'invisible': [('sharing_data_options','!=',False)]}"/>
-            <field name="new_tariff_product_id" domain="[('id', 'in', available_products)]" attrs="{'invisible': [('sharing_data_options','!=',False)]}"/>
-            <field name="mobile_contracts_to_share_with" attrs="{                            'invisible': [('sharing_data_options','!=','new_shared_bond')],                            'required': [('sharing_data_options','=','new_shared_bond')]                           }" context="{'tree_view_ref':'somconnexio.contract_mobile_simplified'}" domain="[('id', 'in', mobile_contracts_wo_sharing_bond)]"/>
-            <field name="fiber_contract_to_link" attrs="{                            'invisible': [('sharing_data_options','!=','new_shared_bond')],                            'required': [('sharing_data_options','=','new_shared_bond')]                           }" options="{'no_create_edit':True}" domain="[('id', 'in', fiber_contracts_wo_sharing_data_mobiles)]"/>
-            <field name="shared_bond_id_to_join" attrs="{                            'invisible': [('sharing_data_options','!=','existing_shared_bond')],                            'required': [('sharing_data_options','=','existing_shared_bond')]                           }"/>
+            <field name="pack_options"/>
+            <field name="current_tariff_product" options="{'no_open': True,'no_create': 1,'no_create_edit': 1}" attrs="{'invisible': [('pack_options','!=',False)]}"/>
+            <field name="new_tariff_product_id" domain="[('id', 'in', available_products)]" options="{'no_create_edit':True}" required="1"/>
+            <field name="fiber_contract_to_link" attrs="{                            'invisible': [                               ('pack_options', 'not in', ['new_shared_bond', 'pinya_mobile_tariff'])                             ],                            'required': [                               ('pack_options', 'in', ['new_shared_bond', 'pinya_mobile_tariff'])                             ]                           }" options="{'no_create_edit':True}" domain="[('id', 'in', available_fiber_contracts)]"/>
+            <field name="mobile_contracts_to_share_data" attrs="{                            'invisible': [('pack_options','!=','new_shared_bond')],                            'required': [('pack_options','=','new_shared_bond')]                           }" context="{'tree_view_ref':'somconnexio.contract_mobile_simplified'}" domain="[('id', 'in', mobile_contracts_wo_sharing_bond)]"/>
+            <field name="shared_bond_id_to_join" attrs="{                            'invisible': [('pack_options','!=','existing_shared_bond')],                            'required': [('pack_options','=','existing_shared_bond')]                           }"/>
             <field name="note"/>
-            <separator/>
             <!-- TODO: Remove confirm logic if check is done in OTRs-->
-            <field name="otrs_checked"/>
+            <label style="color:Red;font-weight:bold;" for="otrs_checked"/>
+            <field nolabel="1" name="otrs_checked"/>
           </group>
           <footer>
             <button type="object" name="button_change" string="Change"/>
             <button special="cancel" string="Cancel" class="btn-secondary"/>
           </footer>
         </form>
       </field>
```

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/mail_compose_message/mail_compose_message.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/mail_compose_message/mail_compose_message.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/payment_order_confirm/payment_order_confirm.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/payment_order_confirm/payment_order_confirm.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/product_publish/product_publish.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/product_publish/product_publish.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/product_publish/product_publish.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/product_publish/product_publish.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.py` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.xml` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo12_addon_somconnexio.egg-info/PKG-INFO` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo12_addon_somconnexio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo12-addon-somconnexio
-Version: 12.0.2.3.3.99.dev2
+Version: 12.0.2.3.4
 Summary: Odoo Som Connexió customizations
 Home-page: https://coopdevs.org
 Author: Coopdevs Treball SCCL
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
@@ -52,15 +52,15 @@
 
 Enter to your local machine as the user `odoo`, activate the python enviornment first and run the odoo bin:
 ```sh
 $ ssh odoo@odoo-sc.local
 $ pyenv activate odoo
 $ cd /opt/odoo
 $ set -a && source /etc/default/odoo && set +a
-$ ./odoo-bin -c /etc/odoo/odoo.conf -u somconnexio -d odoo
+$ ./odoo-bin -c /etc/odoo/odoo.conf -u somconnexio -d odoo --workers 0
 ```
 
 To use the local somconnexio module (development version) instead of the PyPI published one, you need to upgrade the [version in the manifest](https://gitlab.com/coopdevs/odoo-somconnexio/-/blob/master/somconnexio/__manifest__.py#L3) and then update the module with `-u` in the Odoo CLI.
 
 
 #### Restart ODOO database from scratch
```

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo12_addon_somconnexio.egg-info/SOURCES.txt` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo12_addon_somconnexio.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -351,14 +351,15 @@
 odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_force_wizard.py
 odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_wizard.py
 odoo/addons/somconnexio/tests/wizards/test_contract_invoice_payment_wizard.py
 odoo/addons/somconnexio/tests/wizards/test_contract_mobile_tariff_change_wizard.py
 odoo/addons/somconnexio/tests/wizards/test_contract_one_shot_request_wizard.py
 odoo/addons/somconnexio/tests/wizards/test_contract_tariff_change_wizard.py
 odoo/addons/somconnexio/tests/wizards/test_contract_terminate_wizard.py
+odoo/addons/somconnexio/tests/wizards/test_create_lead_add_mobile_line.py
 odoo/addons/somconnexio/tests/wizards/test_create_lead_from_partner_wizard.py
 odoo/addons/somconnexio/tests/wizards/test_create_subscription_from_partner.py
 odoo/addons/somconnexio/tests/wizards/test_crm_lead_generate_SIM_delivery_wizard.py
 odoo/addons/somconnexio/tests/wizards/test_crm_lead_remesa_wizard.py
 odoo/addons/somconnexio/tests/wizards/test_crm_leads_validate_wizard.py
 odoo/addons/somconnexio/tests/wizards/test_mail_compose_message_wizard.py
 odoo/addons/somconnexio/tests/wizards/test_partner_check_somoffice_email.py
@@ -457,14 +458,17 @@
 odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.xml
 odoo/addons/somconnexio/wizards/create_lead_from_partner/__init__.py
 odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.py
 odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.xml
 odoo/addons/somconnexio/wizards/create_subscription_from_partner/__init__.py
 odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.py
 odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.xml
+odoo/addons/somconnexio/wizards/crm_lead_add_mobile_line/__init__.py
+odoo/addons/somconnexio/wizards/crm_lead_add_mobile_line/crm_lead_add_mobile_line.py
+odoo/addons/somconnexio/wizards/crm_lead_add_mobile_line/crm_lead_add_mobile_line.xml
 odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/__init__.py
 odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.py
 odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.xml
 odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/__init__.py
 odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.py
 odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.xml
 odoo/addons/somconnexio/wizards/crm_lead_remesa/__init__.py
```

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/odoo12_addon_somconnexio.egg-info/requires.txt` & `odoo12-addon-somconnexio-12.0.2.3.4/odoo12_addon_somconnexio.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -59,10 +59,10 @@
 odoo12-addon-web-favicon==12.0.1.0.0.99.dev14
 odoo12-addon-web-no-bubble==12.0.1.0.0.99.dev8
 odoo12-addon-web-responsive==12.0.2.3.2
 odoo12-addon-web-searchbar-full-width==12.0.1.0.0.99.dev6
 odoo12-addon-web-widget-open-tab==12.0.1.0.1.99.dev2
 odoo12-addon-web_m2x_options
 odoo<12.1dev,>=12.0a
-otrs-somconnexio==0.4.53
+otrs-somconnexio==0.4.55
 pyopencell==0.4.5
 python-stdnum==1.14
```

### Comparing `odoo12-addon-somconnexio-12.0.2.3.3.99.dev2/setup.py` & `odoo12-addon-somconnexio-12.0.2.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,14 @@
         "external_dependencies_override": {
             "python": {
                 "correos_preregistro": "correos-preregistro==0.0.6",
                 "correos_seguimiento": "correos-seguimiento==0.0.3",
                 "factory": "factory-boy",
                 "faker": "faker==9.3.1",
                 "hashids": "hashids==1.3.1",
-                "otrs_somconnexio": "otrs-somconnexio==0.4.53",
+                "otrs_somconnexio": "otrs-somconnexio==0.4.55",
                 "pyopencell": "pyopencell==0.4.5",
                 "stdnum": "python-stdnum==1.14",
             },
         },
     },
 )
```

