# Comparing `tmp/stytch-7.1.0.tar.gz` & `tmp/stytch-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stytch-7.1.0.tar", last modified: Mon Jul 24 19:43:48 2023, max compression
+gzip compressed data, was "stytch-7.2.0.tar", last modified: Wed Aug  2 17:15:26 2023, max compression
```

## Comparing `stytch-7.1.0.tar` & `stytch-7.2.0.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.327844 stytch-7.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-24 19:43:31.000000 stytch-7.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-07-24 19:43:48.327844 stytch-7.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-24 19:43:31.000000 stytch-7.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-24 19:43:48.327844 stytch-7.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-24 19:43:31.000000 stytch-7.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.311844 stytch-7.1.0/stytch/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.311844 stytch-7.1.0/stytch/b2b/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.315844 stytch-7.1.0/stytch/b2b/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/discovery_intermediate_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21709 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/discovery_organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/magic_links_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/magic_links_email_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/oauth_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    32087 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)    25074 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/organizations_members.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/otp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    19953 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/sso.py
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/sso_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/sso_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.319844 stytch-7.1.0/stytch/b2b/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/discovery_intermediate_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/discovery_organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/magic_links_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/magic_links_email_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/mfa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/oauth_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/organizations_members.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/sso.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/sso_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/sso_saml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.319844 stytch-7.1.0/stytch/consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.323844 stytch-7.1.0/stytch/consumer/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    32410 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/otp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16525 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)    28091 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    15782 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15027 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/totps.py
--rw-r--r--   0 runner    (1001) docker     (123)    28332 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/users.py
--rw-r--r--   0 runner    (1001) docker     (123)    17303 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/webauthn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.327844 stytch-7.1.0/stytch/consumer/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/otp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    10322 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/totps.py
--rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/webauthn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.327844 stytch-7.1.0/stytch/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/core/api_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/core/client_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.327844 stytch-7.1.0/stytch/core/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/core/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/core/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/core/response_base.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.311844 stytch-7.1.0/stytch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-07-24 19:43:48.000000 stytch-7.1.0/stytch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-24 19:43:48.000000 stytch-7.1.0/stytch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:43:48.000000 stytch-7.1.0/stytch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-24 19:43:48.000000 stytch-7.1.0/stytch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 19:43:48.000000 stytch-7.1.0/stytch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.327844 stytch-7.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-07-24 19:43:31.000000 stytch-7.1.0/test/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-07-24 19:43:31.000000 stytch-7.1.0/test/test_integration_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.468517 stytch-7.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-02 17:15:10.000000 stytch-7.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-08-02 17:15:26.468517 stytch-7.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-08-02 17:15:10.000000 stytch-7.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-02 17:15:26.468517 stytch-7.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-08-02 17:15:10.000000 stytch-7.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.456517 stytch-7.2.0/stytch/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.456517 stytch-7.2.0/stytch/b2b/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.460517 stytch-7.2.0/stytch/b2b/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11794 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26657 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/oauth_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33911 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27586 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/organizations_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25401 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21718 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29703 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/sso.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/sso_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/sso_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.460517 stytch-7.2.0/stytch/b2b/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/oauth_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/organizations_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/sso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/sso_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/sso_saml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.460517 stytch-7.2.0/stytch/consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.464517 stytch-7.2.0/stytch/consumer/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32424 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14101 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28095 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15027 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/totps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28332 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17303 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.464517 stytch-7.2.0/stytch/consumer/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/totps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/webauthn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.464517 stytch-7.2.0/stytch/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/core/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/core/client_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.464517 stytch-7.2.0/stytch/core/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/core/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/core/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/core/response_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.456517 stytch-7.2.0/stytch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-08-02 17:15:26.000000 stytch-7.2.0/stytch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-08-02 17:15:26.000000 stytch-7.2.0/stytch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:15:26.000000 stytch-7.2.0/stytch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 17:15:26.000000 stytch-7.2.0/stytch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 17:15:26.000000 stytch-7.2.0/stytch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.468517 stytch-7.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-08-02 17:15:10.000000 stytch-7.2.0/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-08-02 17:15:10.000000 stytch-7.2.0/test/test_integration_async.py
```

### Comparing `stytch-7.1.0/LICENSE.txt` & `stytch-7.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/PKG-INFO` & `stytch-7.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 7.1.0
+Version: 7.2.0
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
@@ -36,27 +36,26 @@
 pip install stytch
 ```
 
 ## Usage
 
 You can find your API credentials in the [Stytch Dashboard](https://stytch.com/dashboard/api-keys).
 
-This client library supports all of Stytch's live products:
-
-- [x] [Email Magic Links](https://stytch.com/docs/api/send-by-email)
-- [x] [Embeddable Magic Links](https://stytch.com/docs/api/create-magic-link-overview)
-- [x] [OAuth logins](https://stytch.com/docs/api/oauth-overview)
-- [x] [SMS passcodes](https://stytch.com/docs/api/send-otp-by-sms)
-- [x] [WhatsApp passcodes](https://stytch.com/docs/api/whatsapp-send)
-- [x] [Email passcodes](https://stytch.com/docs/api/send-otp-by-email)
-- [x] [Session Management](https://stytch.com/docs/api/sessions-overview)
-- [x] [WebAuthn](https://stytch.com/docs/api/webauthn-overview)
-- [x] [Time-based one-time passcodes (TOTPs)](https://stytch.com/docs/api/totps-overview)
-- [x] [Crypto wallets](https://stytch.com/docs/api/crypto-wallet-overview)
-- [x] [Passwords](https://stytch.com/docs/api/password-overview)
+This client library supports all Stytch's live products:
+  - [x] [Email Magic Links](https://stytch.com/docs/api/send-by-email)
+  - [x] [Embeddable Magic Links](https://stytch.com/docs/guides/magic-links/embeddable-magic-links/api)
+  - [x] [OAuth logins](https://stytch.com/docs/guides/oauth/idp-overview)
+  - [x] [SMS passcodes](https://stytch.com/docs/api/send-otp-by-sms)
+  - [x] [WhatsApp passcodes](https://stytch.com/docs/api/whatsapp-send)
+  - [x] [Email passcodes](https://stytch.com/docs/api/send-otp-by-email)
+  - [x] [Session Management](https://stytch.com/docs/guides/sessions/using-sessions)
+  - [x] [WebAuthn](https://stytch.com/docs/guides/webauthn/api)
+  - [x] [Time-based one-time passcodes (TOTPs)](https://stytch.com/docs/guides/totp/api)
+  - [x] [Crypto wallets](https://stytch.com/docs/guides/web3/api)
+  - [x] [Passwords](https://stytch.com/docs/guides/passwords/api)
 
 ### Example usage
 
 Create an API client:
 
 ```python
 import stytch
@@ -138,15 +137,15 @@
 
 ## Support
 
 If you've found a bug, [open an issue](https://github.com/stytchauth/stytch-python/issues/new)!
 
 If you have questions or want help troubleshooting, join us in [Slack](https://join.slack.com/t/stytch/shared_invite/zt-nil4wo92-jApJ9Cl32cJbEd9esKkvyg) or email support@stytch.com.
 
-If you've found a security vulnerability, please follow our [responsible disclosure instructions](https://stytch.com/docs/security).
+If you've found a security vulnerability, please follow our [responsible disclosure instructions](https://stytch.com/docs/resources/security-and-trust/security#:~:text=Responsible%20disclosure%20program).
 
 ## Development
 
 See DEVELOPMENT.md
 
 ## Code of Conduct
```

### Comparing `stytch-7.1.0/README.md` & `stytch-7.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -14,27 +14,26 @@
 pip install stytch
 ```
 
 ## Usage
 
 You can find your API credentials in the [Stytch Dashboard](https://stytch.com/dashboard/api-keys).
 
-This client library supports all of Stytch's live products:
-
-- [x] [Email Magic Links](https://stytch.com/docs/api/send-by-email)
-- [x] [Embeddable Magic Links](https://stytch.com/docs/api/create-magic-link-overview)
-- [x] [OAuth logins](https://stytch.com/docs/api/oauth-overview)
-- [x] [SMS passcodes](https://stytch.com/docs/api/send-otp-by-sms)
-- [x] [WhatsApp passcodes](https://stytch.com/docs/api/whatsapp-send)
-- [x] [Email passcodes](https://stytch.com/docs/api/send-otp-by-email)
-- [x] [Session Management](https://stytch.com/docs/api/sessions-overview)
-- [x] [WebAuthn](https://stytch.com/docs/api/webauthn-overview)
-- [x] [Time-based one-time passcodes (TOTPs)](https://stytch.com/docs/api/totps-overview)
-- [x] [Crypto wallets](https://stytch.com/docs/api/crypto-wallet-overview)
-- [x] [Passwords](https://stytch.com/docs/api/password-overview)
+This client library supports all Stytch's live products:
+  - [x] [Email Magic Links](https://stytch.com/docs/api/send-by-email)
+  - [x] [Embeddable Magic Links](https://stytch.com/docs/guides/magic-links/embeddable-magic-links/api)
+  - [x] [OAuth logins](https://stytch.com/docs/guides/oauth/idp-overview)
+  - [x] [SMS passcodes](https://stytch.com/docs/api/send-otp-by-sms)
+  - [x] [WhatsApp passcodes](https://stytch.com/docs/api/whatsapp-send)
+  - [x] [Email passcodes](https://stytch.com/docs/api/send-otp-by-email)
+  - [x] [Session Management](https://stytch.com/docs/guides/sessions/using-sessions)
+  - [x] [WebAuthn](https://stytch.com/docs/guides/webauthn/api)
+  - [x] [Time-based one-time passcodes (TOTPs)](https://stytch.com/docs/guides/totp/api)
+  - [x] [Crypto wallets](https://stytch.com/docs/guides/web3/api)
+  - [x] [Passwords](https://stytch.com/docs/guides/passwords/api)
 
 ### Example usage
 
 Create an API client:
 
 ```python
 import stytch
@@ -116,15 +115,15 @@
 
 ## Support
 
 If you've found a bug, [open an issue](https://github.com/stytchauth/stytch-python/issues/new)!
 
 If you have questions or want help troubleshooting, join us in [Slack](https://join.slack.com/t/stytch/shared_invite/zt-nil4wo92-jApJ9Cl32cJbEd9esKkvyg) or email support@stytch.com.
 
-If you've found a security vulnerability, please follow our [responsible disclosure instructions](https://stytch.com/docs/security).
+If you've found a security vulnerability, please follow our [responsible disclosure instructions](https://stytch.com/docs/resources/security-and-trust/security#:~:text=Responsible%20disclosure%20program).
 
 ## Development
 
 See DEVELOPMENT.md
 
 ## Code of Conduct
```

### Comparing `stytch-7.1.0/setup.py` & `stytch-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/b2b/api/discovery.py` & `stytch-7.2.0/stytch/b2b/api/discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/b2b/api/discovery_intermediate_sessions.py` & `stytch-7.2.0/stytch/consumer/api/otp.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,123 +4,138 @@
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
 from typing import Any, Dict, Optional
 
-from stytch.b2b.models.discovery_intermediate_sessions import (
-    ExchangeRequestLocale,
-    ExchangeResponse,
-)
+from stytch.consumer.api.otp_email import Email
+from stytch.consumer.api.otp_sms import Sms
+from stytch.consumer.api.otp_whatsapp import Whatsapp
+from stytch.consumer.models.attribute import Attributes
+from stytch.consumer.models.magic_links import Options
+from stytch.consumer.models.otp import AuthenticateResponse
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
-class IntermediateSessions:
+class OTPs:
     def __init__(
         self,
         api_base: ApiBase,
         sync_client: SyncClient,
         async_client: AsyncClient,
     ) -> None:
         self.api_base = api_base
         self.sync_client = sync_client
         self.async_client = async_client
+        self.sms = Sms(api_base, sync_client, async_client)
+        self.whatsapp = Whatsapp(api_base, sync_client, async_client)
+        self.email = Email(api_base, sync_client, async_client)
 
-    def exchange(
+    def authenticate(
         self,
-        intermediate_session_token: str,
-        organization_id: str,
+        method_id: str,
+        code: str,
+        attributes: Optional[Attributes] = None,
+        options: Optional[Options] = None,
+        session_token: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
+        session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
-        locale: Optional[ExchangeRequestLocale] = None,
-    ) -> ExchangeResponse:
-        """Exchange an Intermediate Session for a fully realized [Member Session](https://stytch.com/docs/b2b/api/session-object) in a desired [Organization](https://stytch.com/docs/b2b/api/organization-object).
-        This operation consumes the Intermediate Session.
-
-        This endpoint can be used to accept invites and create new members via domain matching.
+    ) -> AuthenticateResponse:
+        """Authenticate a User given a `method_id` (the associated `email_id` or `phone_id`) and a `code`. This endpoint verifies that the code is valid, hasn't expired or been previously used, and any optional security settings such as IP match or user agent match are satisfied. A given `method_id` may only have a single active OTP code at any given time, if a User requests another OTP code before the first one has expired, the first one will be invalidated.
 
         Fields:
-          - intermediate_session_token: The Intermediate Session Token. This token does not belong to a specific instance of a member, but may be exchanged for an existing Member Session or used to create a new organization.
-          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - method_id: The `email_id` or `phone_id` involved in the given authentication.
+          - code: The code to authenticate.
+          - attributes: Provided attributes help with fraud detection.
+          - options: Specify optional security settings.
+          - session_token: The `session_token` associated with a User's existing Session.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
           five minutes regardless of the underlying session duration, and will need to be refreshed over time.
 
           This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
 
           If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
 
-          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
-          to use the Stytch session product, you can ignore the session fields in the response.
-          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
-          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
-          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
-          Total custom claims size cannot exceed four kilobytes.
-          - locale: (no documentation yet)
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will not be created.
+          - session_jwt: The `session_jwt` associated with a User's existing Session.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value.
+
+          Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes.
         """  # noqa
         data: Dict[str, Any] = {
-            "intermediate_session_token": intermediate_session_token,
-            "organization_id": organization_id,
+            "method_id": method_id,
+            "code": code,
         }
+        if attributes is not None:
+            data["attributes"] = attributes.dict()
+        if options is not None:
+            data["options"] = options.dict()
+        if session_token is not None:
+            data["session_token"] = session_token
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
+        if session_jwt is not None:
+            data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
-        if locale is not None:
-            data["locale"] = locale.value
 
-        url = self.api_base.url_for(
-            "/v1/b2b/discovery/intermediate_sessions/exchange", data
-        )
+        url = self.api_base.url_for("/v1/otps/authenticate", data)
         res = self.sync_client.post(url, data)
-        return ExchangeResponse.from_json(res.response.status_code, res.json)
+        return AuthenticateResponse.from_json(res.response.status_code, res.json)
 
-    async def exchange_async(
+    async def authenticate_async(
         self,
-        intermediate_session_token: str,
-        organization_id: str,
+        method_id: str,
+        code: str,
+        attributes: Optional[Attributes] = None,
+        options: Optional[Options] = None,
+        session_token: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
+        session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
-        locale: Optional[ExchangeRequestLocale] = None,
-    ) -> ExchangeResponse:
-        """Exchange an Intermediate Session for a fully realized [Member Session](https://stytch.com/docs/b2b/api/session-object) in a desired [Organization](https://stytch.com/docs/b2b/api/organization-object).
-        This operation consumes the Intermediate Session.
-
-        This endpoint can be used to accept invites and create new members via domain matching.
+    ) -> AuthenticateResponse:
+        """Authenticate a User given a `method_id` (the associated `email_id` or `phone_id`) and a `code`. This endpoint verifies that the code is valid, hasn't expired or been previously used, and any optional security settings such as IP match or user agent match are satisfied. A given `method_id` may only have a single active OTP code at any given time, if a User requests another OTP code before the first one has expired, the first one will be invalidated.
 
         Fields:
-          - intermediate_session_token: The Intermediate Session Token. This token does not belong to a specific instance of a member, but may be exchanged for an existing Member Session or used to create a new organization.
-          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - method_id: The `email_id` or `phone_id` involved in the given authentication.
+          - code: The code to authenticate.
+          - attributes: Provided attributes help with fraud detection.
+          - options: Specify optional security settings.
+          - session_token: The `session_token` associated with a User's existing Session.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
           five minutes regardless of the underlying session duration, and will need to be refreshed over time.
 
           This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
 
           If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
 
-          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
-          to use the Stytch session product, you can ignore the session fields in the response.
-          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
-          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
-          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
-          Total custom claims size cannot exceed four kilobytes.
-          - locale: (no documentation yet)
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will not be created.
+          - session_jwt: The `session_jwt` associated with a User's existing Session.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value.
+
+          Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes.
         """  # noqa
         data: Dict[str, Any] = {
-            "intermediate_session_token": intermediate_session_token,
-            "organization_id": organization_id,
+            "method_id": method_id,
+            "code": code,
         }
+        if attributes is not None:
+            data["attributes"] = attributes.dict()
+        if options is not None:
+            data["options"] = options.dict()
+        if session_token is not None:
+            data["session_token"] = session_token
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
+        if session_jwt is not None:
+            data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
-        if locale is not None:
-            data["locale"] = locale.value
 
-        url = self.api_base.url_for(
-            "/v1/b2b/discovery/intermediate_sessions/exchange", data
-        )
+        url = self.api_base.url_for("/v1/otps/authenticate", data)
         res = await self.async_client.post(url, data)
-        return ExchangeResponse.from_json(res.response.status, res.json)
+        return AuthenticateResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-7.1.0/stytch/b2b/api/discovery_organizations.py` & `stytch-7.2.0/stytch/b2b/api/discovery_organizations.py`

 * *Files 20% similar despite different names*

```diff
@@ -44,16 +44,25 @@
         """If an end user does not want to join any already-existing organization, or has no possible organizations to join, this endpoint can be used to create a new
         [Organization](https://stytch.com/docs/b2b/api/organization-object) and [Member](https://stytch.com/docs/b2b/api/member-object).
 
         This operation consumes the Intermediate Session.
 
         This endpoint can also be used to start an initial session for the newly created member and organization.
 
+        (Coming Soon) If the new Organization is created with a `mfa_policy` of `REQUIRED_FOR_ALL`, the newly created Member will need to complete an MFA step to log in to the Organization.
+        The `intermediate_session_token` will not be consumed and instead will be returned in the response.
+        The `intermediate_session_token` can be passed into the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete the MFA step and acquire a full member session.
+        The `intermediate_session_token` can also be used with the [Exchange Intermediate Session endpoint](https://stytch.com/docs/b2b/api/exchange-intermediate-session) or the [Create Organization via Discovery endpoint](https://stytch.com/docs/b2b/api/create-organization-via-discovery) to join a different Organization or create a new one.
+        The `session_duration_minutes` and `session_custom_claims` parameters will be ignored.
+
         Fields:
-          - intermediate_session_token: The Intermediate Session Token. This token does not belong to a specific instance of a member, but may be exchanged for an existing Member Session or used to create a new organization.
+          - intermediate_session_token: The Intermediate Session Token. This token does not necessarily belong to a specific instance of a Member, but represents a bag of factors that may be converted to a member session.
+            The token can be used with the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete an MFA flow;
+            the [Exchange Intermediate Session endpoint](https://stytch.com/docs/b2b/api/exchange-intermediate-session) to join a specific Organization that allows the factors represented by the intermediate session token;
+            or the [Create Organization via Discovery endpoint](https://stytch.com/docs/b2b/api/create-organization-via-discovery) to create a new Organization and Member.
           - organization_name: The name of the Organization. If the name is not specified, a default name will be created based on the email used to initiate the discovery flow. If the email domain is a common email provider such as gmail.com, or if the email is a .edu email, the organization name will be generated based on the name portion of the email. Otherwise, the organization name will be generated based on the email domain.
           - organization_slug: The unique URL slug of the Organization. A minimum of two characters is required. The slug only accepts alphanumeric characters and the following reserved characters: `-` `.` `_` `~`. If the slug is not specified, a default slug will be created based on the email used to initiate the discovery flow. If the email domain is a common email provider such as gmail.com, or if the email is a .edu email, the organization slug will be generated based on the name portion of the email. Otherwise, the organization slug will be generated based on the email domain.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
           five minutes regardless of the underlying session duration, and will need to be refreshed over time.
 
           This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
@@ -100,15 +109,20 @@
 
           `RESTRICTED` – only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
 
           - allowed_auth_methods:
           An array of allowed authentication methods. This list is enforced when `auth_methods` is set to `RESTRICTED`.
           The list's accepted values are: `sso`, `magic_link`, `password`, `google_oauth`, and `microsoft_oauth`.
 
-          - mfa_policy: (no documentation yet)
+          - mfa_policy: (Coming Soon) The setting that controls the MFA policy for all Members in the Organization. The accepted values are:
+
+          `REQUIRED_FOR_ALL` – All Members within the Organization will be required to complete MFA every time they wish to log in.
+
+          `OPTIONAL` – The default value. The Organization does not require MFA by default for all Members. Members will be required to complete MFA only if their `mfa_enrolled` status is set to true.
+
         """  # noqa
         data: Dict[str, Any] = {
             "intermediate_session_token": intermediate_session_token,
             "organization_name": organization_name,
             "organization_slug": organization_slug,
         }
         if session_duration_minutes is not None:
@@ -158,16 +172,25 @@
         """If an end user does not want to join any already-existing organization, or has no possible organizations to join, this endpoint can be used to create a new
         [Organization](https://stytch.com/docs/b2b/api/organization-object) and [Member](https://stytch.com/docs/b2b/api/member-object).
 
         This operation consumes the Intermediate Session.
 
         This endpoint can also be used to start an initial session for the newly created member and organization.
 
+        (Coming Soon) If the new Organization is created with a `mfa_policy` of `REQUIRED_FOR_ALL`, the newly created Member will need to complete an MFA step to log in to the Organization.
+        The `intermediate_session_token` will not be consumed and instead will be returned in the response.
+        The `intermediate_session_token` can be passed into the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete the MFA step and acquire a full member session.
+        The `intermediate_session_token` can also be used with the [Exchange Intermediate Session endpoint](https://stytch.com/docs/b2b/api/exchange-intermediate-session) or the [Create Organization via Discovery endpoint](https://stytch.com/docs/b2b/api/create-organization-via-discovery) to join a different Organization or create a new one.
+        The `session_duration_minutes` and `session_custom_claims` parameters will be ignored.
+
         Fields:
-          - intermediate_session_token: The Intermediate Session Token. This token does not belong to a specific instance of a member, but may be exchanged for an existing Member Session or used to create a new organization.
+          - intermediate_session_token: The Intermediate Session Token. This token does not necessarily belong to a specific instance of a Member, but represents a bag of factors that may be converted to a member session.
+            The token can be used with the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete an MFA flow;
+            the [Exchange Intermediate Session endpoint](https://stytch.com/docs/b2b/api/exchange-intermediate-session) to join a specific Organization that allows the factors represented by the intermediate session token;
+            or the [Create Organization via Discovery endpoint](https://stytch.com/docs/b2b/api/create-organization-via-discovery) to create a new Organization and Member.
           - organization_name: The name of the Organization. If the name is not specified, a default name will be created based on the email used to initiate the discovery flow. If the email domain is a common email provider such as gmail.com, or if the email is a .edu email, the organization name will be generated based on the name portion of the email. Otherwise, the organization name will be generated based on the email domain.
           - organization_slug: The unique URL slug of the Organization. A minimum of two characters is required. The slug only accepts alphanumeric characters and the following reserved characters: `-` `.` `_` `~`. If the slug is not specified, a default slug will be created based on the email used to initiate the discovery flow. If the email domain is a common email provider such as gmail.com, or if the email is a .edu email, the organization slug will be generated based on the name portion of the email. Otherwise, the organization slug will be generated based on the email domain.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
           five minutes regardless of the underlying session duration, and will need to be refreshed over time.
 
           This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
@@ -214,15 +237,20 @@
 
           `RESTRICTED` – only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
 
           - allowed_auth_methods:
           An array of allowed authentication methods. This list is enforced when `auth_methods` is set to `RESTRICTED`.
           The list's accepted values are: `sso`, `magic_link`, `password`, `google_oauth`, and `microsoft_oauth`.
 
-          - mfa_policy: (no documentation yet)
+          - mfa_policy: (Coming Soon) The setting that controls the MFA policy for all Members in the Organization. The accepted values are:
+
+          `REQUIRED_FOR_ALL` – All Members within the Organization will be required to complete MFA every time they wish to log in.
+
+          `OPTIONAL` – The default value. The Organization does not require MFA by default for all Members. Members will be required to complete MFA only if their `mfa_enrolled` status is set to true.
+
         """  # noqa
         data: Dict[str, Any] = {
             "intermediate_session_token": intermediate_session_token,
             "organization_name": organization_name,
             "organization_slug": organization_slug,
         }
         if session_duration_minutes is not None:
@@ -269,15 +297,18 @@
 
         This endpoint requires either an `intermediate_session_token`, `session_jwt` or `session_token` be included in the request.
         It will return an error if multiple are present.
 
         This operation does not consume the Intermediate Session or Session Token passed in.
 
         Fields:
-          - intermediate_session_token: The Intermediate Session Token. This token does not belong to a specific instance of a member, but may be exchanged for an existing Member Session or used to create a new organization.
+          - intermediate_session_token: The Intermediate Session Token. This token does not necessarily belong to a specific instance of a Member, but represents a bag of factors that may be converted to a member session.
+            The token can be used with the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete an MFA flow;
+            the [Exchange Intermediate Session endpoint](https://stytch.com/docs/b2b/api/exchange-intermediate-session) to join a specific Organization that allows the factors represented by the intermediate session token;
+            or the [Create Organization via Discovery endpoint](https://stytch.com/docs/b2b/api/create-organization-via-discovery) to create a new Organization and Member.
           - session_token: A secret token for a given Stytch Session.
           - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
         """  # noqa
         data: Dict[str, Any] = {}
         if intermediate_session_token is not None:
             data["intermediate_session_token"] = intermediate_session_token
         if session_token is not None:
@@ -306,15 +337,18 @@
 
         This endpoint requires either an `intermediate_session_token`, `session_jwt` or `session_token` be included in the request.
         It will return an error if multiple are present.
 
         This operation does not consume the Intermediate Session or Session Token passed in.
 
         Fields:
-          - intermediate_session_token: The Intermediate Session Token. This token does not belong to a specific instance of a member, but may be exchanged for an existing Member Session or used to create a new organization.
+          - intermediate_session_token: The Intermediate Session Token. This token does not necessarily belong to a specific instance of a Member, but represents a bag of factors that may be converted to a member session.
+            The token can be used with the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete an MFA flow;
+            the [Exchange Intermediate Session endpoint](https://stytch.com/docs/b2b/api/exchange-intermediate-session) to join a specific Organization that allows the factors represented by the intermediate session token;
+            or the [Create Organization via Discovery endpoint](https://stytch.com/docs/b2b/api/create-organization-via-discovery) to create a new Organization and Member.
           - session_token: A secret token for a given Stytch Session.
           - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
         """  # noqa
         data: Dict[str, Any] = {}
         if intermediate_session_token is not None:
             data["intermediate_session_token"] = intermediate_session_token
         if session_token is not None:
```

### Comparing `stytch-7.1.0/stytch/b2b/api/magic_links.py` & `stytch-7.2.0/stytch/consumer/api/magic_links.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
 from typing import Any, Dict, Optional
 
-from stytch.b2b.api.magic_links_discovery import Discovery
-from stytch.b2b.api.magic_links_email import Email
-from stytch.b2b.models.magic_links import (
-    AuthenticateRequestLocale,
+from stytch.consumer.api.magic_links_email import Email
+from stytch.consumer.models.attribute import Attributes
+from stytch.consumer.models.magic_links import (
     AuthenticateResponse,
+    CreateResponse,
+    Options,
 )
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
 class MagicLinks:
     def __init__(
@@ -25,122 +26,173 @@
         sync_client: SyncClient,
         async_client: AsyncClient,
     ) -> None:
         self.api_base = api_base
         self.sync_client = sync_client
         self.async_client = async_client
         self.email = Email(api_base, sync_client, async_client)
-        self.discovery = Discovery(api_base, sync_client, async_client)
 
     def authenticate(
         self,
-        magic_links_token: str,
-        pkce_code_verifier: Optional[str] = None,
+        token: str,
+        attributes: Optional[Attributes] = None,
+        options: Optional[Options] = None,
         session_token: Optional[str] = None,
-        session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
+        session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
-        locale: Optional[AuthenticateRequestLocale] = None,
+        code_verifier: Optional[str] = None,
     ) -> AuthenticateResponse:
-        """Authenticate a Member with a Magic Link. This endpoint requires a Magic Link token that is not expired or previously used. If the Member’s status is `pending` or `invited`, they will be updated to `active`. Provide the `session_duration_minutes` parameter to set the lifetime of the session. If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration.
+        """Authenticate a User given a Magic Link. This endpoint verifies that the Magic Link token is valid, hasn't expired or been previously used, and any optional security settings such as IP match or user agent match are satisfied.
 
         Fields:
-          - magic_links_token: The Email Magic Link token to authenticate.
-          - pkce_code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
-          - session_token: Reuse an existing session instead of creating a new one. If you provide a `session_token`, Stytch will update the session.
-              If the `session_token` and `magic_links_token` belong to different Members, the `session_token` will be ignored. This endpoint will error if
-              both `session_token` and `session_jwt` are provided.
-          - session_jwt: Reuse an existing session instead of creating a new one. If you provide a `session_jwt`, Stytch will update the session. If the `session_jwt`
-              and `magic_links_token` belong to different Members, the `session_jwt` will be ignored. This endpoint will error if both `session_token` and `session_jwt`
-              are provided.
+          - token: The token to authenticate.
+          - attributes: Provided attributes help with fraud detection.
+          - options: Specify optional security settings.
+          - session_token: The `session_token` associated with a User's existing Session.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
           five minutes regardless of the underlying session duration, and will need to be refreshed over time.
 
           This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
 
           If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
 
-          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
-          to use the Stytch session product, you can ignore the session fields in the response.
-          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
-          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
-          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
-          Total custom claims size cannot exceed four kilobytes.
-          - locale: (no documentation yet)
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will not be created.
+          - session_jwt: The `session_jwt` associated with a User's existing Session.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value.
+
+          Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes.
+          - code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
         """  # noqa
         data: Dict[str, Any] = {
-            "magic_links_token": magic_links_token,
+            "token": token,
         }
-        if pkce_code_verifier is not None:
-            data["pkce_code_verifier"] = pkce_code_verifier
+        if attributes is not None:
+            data["attributes"] = attributes.dict()
+        if options is not None:
+            data["options"] = options.dict()
         if session_token is not None:
             data["session_token"] = session_token
-        if session_jwt is not None:
-            data["session_jwt"] = session_jwt
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
+        if session_jwt is not None:
+            data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
-        if locale is not None:
-            data["locale"] = locale.value
+        if code_verifier is not None:
+            data["code_verifier"] = code_verifier
 
-        url = self.api_base.url_for("/v1/b2b/magic_links/authenticate", data)
+        url = self.api_base.url_for("/v1/magic_links/authenticate", data)
         res = self.sync_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status_code, res.json)
 
     async def authenticate_async(
         self,
-        magic_links_token: str,
-        pkce_code_verifier: Optional[str] = None,
+        token: str,
+        attributes: Optional[Attributes] = None,
+        options: Optional[Options] = None,
         session_token: Optional[str] = None,
-        session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
+        session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
-        locale: Optional[AuthenticateRequestLocale] = None,
+        code_verifier: Optional[str] = None,
     ) -> AuthenticateResponse:
-        """Authenticate a Member with a Magic Link. This endpoint requires a Magic Link token that is not expired or previously used. If the Member’s status is `pending` or `invited`, they will be updated to `active`. Provide the `session_duration_minutes` parameter to set the lifetime of the session. If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration.
+        """Authenticate a User given a Magic Link. This endpoint verifies that the Magic Link token is valid, hasn't expired or been previously used, and any optional security settings such as IP match or user agent match are satisfied.
 
         Fields:
-          - magic_links_token: The Email Magic Link token to authenticate.
-          - pkce_code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
-          - session_token: Reuse an existing session instead of creating a new one. If you provide a `session_token`, Stytch will update the session.
-              If the `session_token` and `magic_links_token` belong to different Members, the `session_token` will be ignored. This endpoint will error if
-              both `session_token` and `session_jwt` are provided.
-          - session_jwt: Reuse an existing session instead of creating a new one. If you provide a `session_jwt`, Stytch will update the session. If the `session_jwt`
-              and `magic_links_token` belong to different Members, the `session_jwt` will be ignored. This endpoint will error if both `session_token` and `session_jwt`
-              are provided.
+          - token: The token to authenticate.
+          - attributes: Provided attributes help with fraud detection.
+          - options: Specify optional security settings.
+          - session_token: The `session_token` associated with a User's existing Session.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
           five minutes regardless of the underlying session duration, and will need to be refreshed over time.
 
           This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
 
           If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
 
-          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
-          to use the Stytch session product, you can ignore the session fields in the response.
-          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
-          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
-          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
-          Total custom claims size cannot exceed four kilobytes.
-          - locale: (no documentation yet)
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will not be created.
+          - session_jwt: The `session_jwt` associated with a User's existing Session.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value.
+
+          Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes.
+          - code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
         """  # noqa
         data: Dict[str, Any] = {
-            "magic_links_token": magic_links_token,
+            "token": token,
         }
-        if pkce_code_verifier is not None:
-            data["pkce_code_verifier"] = pkce_code_verifier
+        if attributes is not None:
+            data["attributes"] = attributes.dict()
+        if options is not None:
+            data["options"] = options.dict()
         if session_token is not None:
             data["session_token"] = session_token
-        if session_jwt is not None:
-            data["session_jwt"] = session_jwt
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
+        if session_jwt is not None:
+            data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
-        if locale is not None:
-            data["locale"] = locale.value
+        if code_verifier is not None:
+            data["code_verifier"] = code_verifier
 
-        url = self.api_base.url_for("/v1/b2b/magic_links/authenticate", data)
+        url = self.api_base.url_for("/v1/magic_links/authenticate", data)
         res = await self.async_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status, res.json)
+
+    def create(
+        self,
+        user_id: str,
+        expiration_minutes: Optional[int] = None,
+        attributes: Optional[Attributes] = None,
+    ) -> CreateResponse:
+        """Create an embeddable Magic Link token for a User. Access to this endpoint is restricted. To enable it, please send us a note at support@stytch.com.
+
+        ### Next steps
+        Send the returned `token` value to the end user in a link which directs to your application. When the end user follows your link, collect the token, and call [Authenticate Magic Link](https://stytch.com/docs/api/authenticate-magic-link) to complete authentication.
+
+        Fields:
+          - user_id: The unique ID of a specific User.
+          - expiration_minutes: Set the expiration for the Magic Link `token` in minutes. By default, it expires in 1 hour. The minimum expiration is 5 minutes and the maximum is 7 days (10080 mins).
+          - attributes: Provided attributes help with fraud detection.
+        """  # noqa
+        data: Dict[str, Any] = {
+            "user_id": user_id,
+        }
+        if expiration_minutes is not None:
+            data["expiration_minutes"] = expiration_minutes
+        if attributes is not None:
+            data["attributes"] = attributes.dict()
+
+        url = self.api_base.url_for("/v1/magic_links", data)
+        res = self.sync_client.post(url, data)
+        return CreateResponse.from_json(res.response.status_code, res.json)
+
+    async def create_async(
+        self,
+        user_id: str,
+        expiration_minutes: Optional[int] = None,
+        attributes: Optional[Attributes] = None,
+    ) -> CreateResponse:
+        """Create an embeddable Magic Link token for a User. Access to this endpoint is restricted. To enable it, please send us a note at support@stytch.com.
+
+        ### Next steps
+        Send the returned `token` value to the end user in a link which directs to your application. When the end user follows your link, collect the token, and call [Authenticate Magic Link](https://stytch.com/docs/api/authenticate-magic-link) to complete authentication.
+
+        Fields:
+          - user_id: The unique ID of a specific User.
+          - expiration_minutes: Set the expiration for the Magic Link `token` in minutes. By default, it expires in 1 hour. The minimum expiration is 5 minutes and the maximum is 7 days (10080 mins).
+          - attributes: Provided attributes help with fraud detection.
+        """  # noqa
+        data: Dict[str, Any] = {
+            "user_id": user_id,
+        }
+        if expiration_minutes is not None:
+            data["expiration_minutes"] = expiration_minutes
+        if attributes is not None:
+            data["attributes"] = attributes.dict()
+
+        url = self.api_base.url_for("/v1/magic_links", data)
+        res = await self.async_client.post(url, data)
+        return CreateResponse.from_json(res.response.status, res.json)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `stytch-7.1.0/stytch/b2b/api/magic_links_discovery.py` & `stytch-7.2.0/stytch/b2b/api/magic_links_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/b2b/api/magic_links_email.py` & `stytch-7.2.0/stytch/b2b/api/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/b2b/api/magic_links_email_discovery.py` & `stytch-7.2.0/stytch/b2b/api/magic_links_email_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/b2b/api/oauth.py` & `stytch-7.2.0/stytch/consumer/api/passwords_existing_password.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,130 +4,120 @@
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
 from typing import Any, Dict, Optional
 
-from stytch.b2b.api.oauth_discovery import Discovery
-from stytch.b2b.models.oauth import AuthenticateRequestLocale, AuthenticateResponse
+from stytch.consumer.models.passwords_existing_password import ResetResponse
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
-class OAuth:
+class ExistingPassword:
     def __init__(
         self,
         api_base: ApiBase,
         sync_client: SyncClient,
         async_client: AsyncClient,
     ) -> None:
         self.api_base = api_base
         self.sync_client = sync_client
         self.async_client = async_client
-        self.discovery = Discovery(api_base, sync_client, async_client)
 
-    def authenticate(
+    def reset(
         self,
-        oauth_token: str,
+        email: str,
+        existing_password: str,
+        new_password: str,
         session_token: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
-        pkce_code_verifier: Optional[str] = None,
-        locale: Optional[AuthenticateRequestLocale] = None,
-    ) -> AuthenticateResponse:
-        """Authenticate a Member given a `token`. This endpoint verifies that the member completed the OAuth flow by verifying that the token is valid and hasn't expired.  Provide the `session_duration_minutes` parameter to set the lifetime of the session. If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration.
+    ) -> ResetResponse:
+        """Reset the User’s password using their existing password.
 
         Fields:
-          - oauth_token: The token to authenticate.
-          - session_token: A secret token for a given Stytch Session.
+          - email: The email address of the end user.
+          - existing_password: The user's existing password.
+          - new_password: The new password for the user.
+          - session_token: The `session_token` associated with a User's existing Session.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
           five minutes regardless of the underlying session duration, and will need to be refreshed over time.
 
           This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
 
           If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
 
-          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
-          to use the Stytch session product, you can ignore the session fields in the response.
-          - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
-          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
-          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
-          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
-          Total custom claims size cannot exceed four kilobytes.
-          - pkce_code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
-          - locale: (no documentation yet)
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will not be created.
+          - session_jwt: The `session_jwt` associated with a User's existing Session.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value.
+
+          Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes.
         """  # noqa
         data: Dict[str, Any] = {
-            "oauth_token": oauth_token,
+            "email": email,
+            "existing_password": existing_password,
+            "new_password": new_password,
         }
         if session_token is not None:
             data["session_token"] = session_token
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
-        if pkce_code_verifier is not None:
-            data["pkce_code_verifier"] = pkce_code_verifier
-        if locale is not None:
-            data["locale"] = locale.value
 
-        url = self.api_base.url_for("/v1/b2b/oauth/authenticate", data)
+        url = self.api_base.url_for("/v1/passwords/existing_password/reset", data)
         res = self.sync_client.post(url, data)
-        return AuthenticateResponse.from_json(res.response.status_code, res.json)
+        return ResetResponse.from_json(res.response.status_code, res.json)
 
-    async def authenticate_async(
+    async def reset_async(
         self,
-        oauth_token: str,
+        email: str,
+        existing_password: str,
+        new_password: str,
         session_token: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
-        pkce_code_verifier: Optional[str] = None,
-        locale: Optional[AuthenticateRequestLocale] = None,
-    ) -> AuthenticateResponse:
-        """Authenticate a Member given a `token`. This endpoint verifies that the member completed the OAuth flow by verifying that the token is valid and hasn't expired.  Provide the `session_duration_minutes` parameter to set the lifetime of the session. If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration.
+    ) -> ResetResponse:
+        """Reset the User’s password using their existing password.
 
         Fields:
-          - oauth_token: The token to authenticate.
-          - session_token: A secret token for a given Stytch Session.
+          - email: The email address of the end user.
+          - existing_password: The user's existing password.
+          - new_password: The new password for the user.
+          - session_token: The `session_token` associated with a User's existing Session.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
           five minutes regardless of the underlying session duration, and will need to be refreshed over time.
 
           This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
 
           If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
 
-          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
-          to use the Stytch session product, you can ignore the session fields in the response.
-          - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
-          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
-          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
-          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
-          Total custom claims size cannot exceed four kilobytes.
-          - pkce_code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
-          - locale: (no documentation yet)
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will not be created.
+          - session_jwt: The `session_jwt` associated with a User's existing Session.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value.
+
+          Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes.
         """  # noqa
         data: Dict[str, Any] = {
-            "oauth_token": oauth_token,
+            "email": email,
+            "existing_password": existing_password,
+            "new_password": new_password,
         }
         if session_token is not None:
             data["session_token"] = session_token
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
-        if pkce_code_verifier is not None:
-            data["pkce_code_verifier"] = pkce_code_verifier
-        if locale is not None:
-            data["locale"] = locale.value
 
-        url = self.api_base.url_for("/v1/b2b/oauth/authenticate", data)
+        url = self.api_base.url_for("/v1/passwords/existing_password/reset", data)
         res = await self.async_client.post(url, data)
-        return AuthenticateResponse.from_json(res.response.status, res.json)
+        return ResetResponse.from_json(res.response.status, res.json)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stytch-7.1.0/stytch/b2b/api/oauth_discovery.py` & `stytch-7.2.0/stytch/b2b/api/oauth_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/b2b/api/organizations.py` & `stytch-7.2.0/stytch/b2b/api/organizations.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         email_invites: Optional[str] = None,
         auth_methods: Optional[str] = None,
         allowed_auth_methods: Optional[List[str]] = None,
         mfa_policy: Optional[str] = None,
     ) -> CreateResponse:
         """Creates an Organization. An `organization_name` and a unique `organization_slug` are required.
 
-        By default, `email_invites` and `sso_jit_provisioning` will be set to `ALL_ALLOWED` if no Organization authentication settings are explicitly defined in the request.
+        By default, `email_invites` and `sso_jit_provisioning` will be set to `ALL_ALLOWED`, and `mfa_policy` will be set to `OPTIONAL` if no Organization authentication settings are explicitly defined in the request.
 
         *See the [Organization authentication settings](https://stytch.com/docs/b2b/api/org-auth-settings) resource to learn more about fields like `email_jit_provisioning`, `email_invites`, `sso_jit_provisioning`, etc., and their behaviors.
 
         Fields:
           - organization_name: The name of the Organization.
           - organization_slug: The unique URL slug of the Organization. A minimum of two characters is required. The slug only accepts alphanumeric characters and the following reserved characters: `-` `.` `_` `~`.
           - organization_logo_url: The image URL of the Organization logo.
@@ -90,15 +90,20 @@
 
           `RESTRICTED` – only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
 
           - allowed_auth_methods:
           An array of allowed authentication methods. This list is enforced when `auth_methods` is set to `RESTRICTED`.
           The list's accepted values are: `sso`, `magic_link`, `password`, `google_oauth`, and `microsoft_oauth`.
 
-          - mfa_policy: (no documentation yet)
+          - mfa_policy: (Coming Soon) The setting that controls the MFA policy for all Members in the Organization. The accepted values are:
+
+          `REQUIRED_FOR_ALL` – All Members within the Organization will be required to complete MFA every time they wish to log in.
+
+          `OPTIONAL` – The default value. The Organization does not require MFA by default for all Members. Members will be required to complete MFA only if their `mfa_enrolled` status is set to true.
+
         """  # noqa
         data: Dict[str, Any] = {
             "organization_name": organization_name,
         }
         if organization_slug is not None:
             data["organization_slug"] = organization_slug
         if organization_logo_url is not None:
@@ -136,15 +141,15 @@
         email_invites: Optional[str] = None,
         auth_methods: Optional[str] = None,
         allowed_auth_methods: Optional[List[str]] = None,
         mfa_policy: Optional[str] = None,
     ) -> CreateResponse:
         """Creates an Organization. An `organization_name` and a unique `organization_slug` are required.
 
-        By default, `email_invites` and `sso_jit_provisioning` will be set to `ALL_ALLOWED` if no Organization authentication settings are explicitly defined in the request.
+        By default, `email_invites` and `sso_jit_provisioning` will be set to `ALL_ALLOWED`, and `mfa_policy` will be set to `OPTIONAL` if no Organization authentication settings are explicitly defined in the request.
 
         *See the [Organization authentication settings](https://stytch.com/docs/b2b/api/org-auth-settings) resource to learn more about fields like `email_jit_provisioning`, `email_invites`, `sso_jit_provisioning`, etc., and their behaviors.
 
         Fields:
           - organization_name: The name of the Organization.
           - organization_slug: The unique URL slug of the Organization. A minimum of two characters is required. The slug only accepts alphanumeric characters and the following reserved characters: `-` `.` `_` `~`.
           - organization_logo_url: The image URL of the Organization logo.
@@ -181,15 +186,20 @@
 
           `RESTRICTED` – only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
 
           - allowed_auth_methods:
           An array of allowed authentication methods. This list is enforced when `auth_methods` is set to `RESTRICTED`.
           The list's accepted values are: `sso`, `magic_link`, `password`, `google_oauth`, and `microsoft_oauth`.
 
-          - mfa_policy: (no documentation yet)
+          - mfa_policy: (Coming Soon) The setting that controls the MFA policy for all Members in the Organization. The accepted values are:
+
+          `REQUIRED_FOR_ALL` – All Members within the Organization will be required to complete MFA every time they wish to log in.
+
+          `OPTIONAL` – The default value. The Organization does not require MFA by default for all Members. Members will be required to complete MFA only if their `mfa_enrolled` status is set to true.
+
         """  # noqa
         data: Dict[str, Any] = {
             "organization_name": organization_name,
         }
         if organization_slug is not None:
             data["organization_slug"] = organization_slug
         if organization_logo_url is not None:
@@ -311,15 +321,20 @@
 
           `RESTRICTED` – only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
 
           - allowed_auth_methods:
           An array of allowed authentication methods. This list is enforced when `auth_methods` is set to `RESTRICTED`.
           The list's accepted values are: `sso`, `magic_link`, `password`, `google_oauth`, and `microsoft_oauth`.
 
-          - mfa_policy: (no documentation yet)
+          - mfa_policy: (Coming Soon) The setting that controls the MFA policy for all Members in the Organization. The accepted values are:
+
+          `REQUIRED_FOR_ALL` – All Members within the Organization will be required to complete MFA every time they wish to log in.
+
+          `OPTIONAL` – The default value. The Organization does not require MFA by default for all Members. Members will be required to complete MFA only if their `mfa_enrolled` status is set to true.
+
         """  # noqa
         data: Dict[str, Any] = {
             "organization_id": organization_id,
         }
         if organization_name is not None:
             data["organization_name"] = organization_name
         if organization_slug is not None:
@@ -415,15 +430,20 @@
 
           `RESTRICTED` – only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
 
           - allowed_auth_methods:
           An array of allowed authentication methods. This list is enforced when `auth_methods` is set to `RESTRICTED`.
           The list's accepted values are: `sso`, `magic_link`, `password`, `google_oauth`, and `microsoft_oauth`.
 
-          - mfa_policy: (no documentation yet)
+          - mfa_policy: (Coming Soon) The setting that controls the MFA policy for all Members in the Organization. The accepted values are:
+
+          `REQUIRED_FOR_ALL` – All Members within the Organization will be required to complete MFA every time they wish to log in.
+
+          `OPTIONAL` – The default value. The Organization does not require MFA by default for all Members. Members will be required to complete MFA only if their `mfa_enrolled` status is set to true.
+
         """  # noqa
         data: Dict[str, Any] = {
             "organization_id": organization_id,
         }
         if organization_name is not None:
             data["organization_name"] = organization_name
         if organization_slug is not None:
```

### Comparing `stytch-7.1.0/stytch/b2b/api/organizations_members.py` & `stytch-7.2.0/stytch/b2b/api/organizations_members.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,16 +51,16 @@
           - member_id: Globally unique UUID that identifies a specific Member. The `member_id` is critical to perform operations on a Member, so be sure to preserve this value.
           - name: The name of the Member.
           - trusted_metadata: An arbitrary JSON object for storing application-specific data or identity-provider-specific data.
           - untrusted_metadata: An arbitrary JSON object of application-specific data. These fields can be edited directly by the
           frontend SDK, and should not be used to store critical information. See the [Metadata resource](https://stytch.com/docs/b2b/api/metadata)
           for complete field behavior details.
           - is_breakglass: Identifies the Member as a break glass user - someone who has permissions to authenticate into an Organization by bypassing the Organization's settings. A break glass account is typically used for emergency purposes to gain access outside of normal authentication procedures. Refer to the [Organization object](organization-object) and its `auth_methods` and `allowed_auth_methods` fields for more details.
-          - phone_number: (no documentation yet)
-          - mfa_enrolled: (no documentation yet)
+          - phone_number: (Coming Soon) Sets the Member's phone number. Throws an error if the Member already has a phone number. To change the Member's phone number, use the [Delete member phone number endpoint](https://stytch.com/docs/b2b/api/delete-member-phone-number) to delete the Member's existing phone number first.
+          - mfa_enrolled: (Coming Soon) Sets whether the Member is enrolled in MFA. If true, the Member must complete an MFA step whenever they wish to log in to their Organization. If false, the Member only needs to complete an MFA step if the Organization's MFA policy is set to `REQUIRED_FOR_ALL`.
         """  # noqa
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "member_id": member_id,
         }
         if name is not None:
             data["name"] = name
@@ -99,16 +99,16 @@
           - member_id: Globally unique UUID that identifies a specific Member. The `member_id` is critical to perform operations on a Member, so be sure to preserve this value.
           - name: The name of the Member.
           - trusted_metadata: An arbitrary JSON object for storing application-specific data or identity-provider-specific data.
           - untrusted_metadata: An arbitrary JSON object of application-specific data. These fields can be edited directly by the
           frontend SDK, and should not be used to store critical information. See the [Metadata resource](https://stytch.com/docs/b2b/api/metadata)
           for complete field behavior details.
           - is_breakglass: Identifies the Member as a break glass user - someone who has permissions to authenticate into an Organization by bypassing the Organization's settings. A break glass account is typically used for emergency purposes to gain access outside of normal authentication procedures. Refer to the [Organization object](organization-object) and its `auth_methods` and `allowed_auth_methods` fields for more details.
-          - phone_number: (no documentation yet)
-          - mfa_enrolled: (no documentation yet)
+          - phone_number: (Coming Soon) Sets the Member's phone number. Throws an error if the Member already has a phone number. To change the Member's phone number, use the [Delete member phone number endpoint](https://stytch.com/docs/b2b/api/delete-member-phone-number) to delete the Member's existing phone number first.
+          - mfa_enrolled: (Coming Soon) Sets whether the Member is enrolled in MFA. If true, the Member must complete an MFA step whenever they wish to log in to their Organization. If false, the Member only needs to complete an MFA step if the Organization's MFA policy is set to `REQUIRED_FOR_ALL`.
         """  # noqa
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "member_id": member_id,
         }
         if name is not None:
             data["name"] = name
@@ -174,14 +174,20 @@
         return DeleteResponse.from_json(res.response.status, res.json)
 
     def delete_phone_number(
         self,
         organization_id: str,
         member_id: str,
     ) -> DeletePhoneNumberResponse:
+        """Delete a Member's phone number.
+
+        Fields:
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - member_id: Globally unique UUID that identifies a specific Member. The `member_id` is critical to perform operations on a Member, so be sure to preserve this value.
+        """  # noqa
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "member_id": member_id,
         }
 
         url = self.api_base.url_for(
             "/v1/b2b/organizations/{organization_id}/members/phone_numbers/{member_id}",
@@ -191,14 +197,20 @@
         return DeletePhoneNumberResponse.from_json(res.response.status_code, res.json)
 
     async def delete_phone_number_async(
         self,
         organization_id: str,
         member_id: str,
     ) -> DeletePhoneNumberResponse:
+        """Delete a Member's phone number.
+
+        Fields:
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - member_id: Globally unique UUID that identifies a specific Member. The `member_id` is critical to perform operations on a Member, so be sure to preserve this value.
+        """  # noqa
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "member_id": member_id,
         }
 
         url = self.api_base.url_for(
             "/v1/b2b/organizations/{organization_id}/members/phone_numbers/{member_id}",
@@ -218,15 +230,15 @@
 
         *All fuzzy search filters require a minimum of three characters.
 
         Fields:
           - organization_ids: An array of organization_ids. At least one value is required.
           - cursor: The `cursor` field allows you to paginate through your results. Each result array is limited to 1000 results. If your query returns more than 1000 results, you will need to paginate the responses using the `cursor`. If you receive a response that includes a non-null `next_cursor` in the `results_metadata` object, repeat the search call with the `next_cursor` value set to the `cursor` field to retrieve the next page of results. Continue to make search calls until the `next_cursor` in the response is null.
           - limit: The number of search results to return per page. The default limit is 100. A maximum of 1000 results can be returned by a single search request. If the total size of your result set is greater than one page size, you must paginate the response. See the `cursor` field.
-          - query: The optional query object contains the operator, i.e. `AND` or `OR`, and the operands that will filter your results. Only an operator is required. If you include no operands, no filtering will be applied. If you include no query object, it will return all Organizations with no filtering applied.
+          - query: The optional query object contains the operator, i.e. `AND` or `OR`, and the operands that will filter your results. Only an operator is required. If you include no operands, no filtering will be applied. If you include no query object, it will return all Members with no filtering applied.
         """  # noqa
         data: Dict[str, Any] = {
             "organization_ids": organization_ids,
         }
         if cursor is not None:
             data["cursor"] = cursor
         if limit is not None:
@@ -249,15 +261,15 @@
 
         *All fuzzy search filters require a minimum of three characters.
 
         Fields:
           - organization_ids: An array of organization_ids. At least one value is required.
           - cursor: The `cursor` field allows you to paginate through your results. Each result array is limited to 1000 results. If your query returns more than 1000 results, you will need to paginate the responses using the `cursor`. If you receive a response that includes a non-null `next_cursor` in the `results_metadata` object, repeat the search call with the `next_cursor` value set to the `cursor` field to retrieve the next page of results. Continue to make search calls until the `next_cursor` in the response is null.
           - limit: The number of search results to return per page. The default limit is 100. A maximum of 1000 results can be returned by a single search request. If the total size of your result set is greater than one page size, you must paginate the response. See the `cursor` field.
-          - query: The optional query object contains the operator, i.e. `AND` or `OR`, and the operands that will filter your results. Only an operator is required. If you include no operands, no filtering will be applied. If you include no query object, it will return all Organizations with no filtering applied.
+          - query: The optional query object contains the operator, i.e. `AND` or `OR`, and the operands that will filter your results. Only an operator is required. If you include no operands, no filtering will be applied. If you include no query object, it will return all Members with no filtering applied.
         """  # noqa
         data: Dict[str, Any] = {
             "organization_ids": organization_ids,
         }
         if cursor is not None:
             data["cursor"] = cursor
         if limit is not None:
@@ -335,16 +347,16 @@
           - name: The name of the Member.
           - trusted_metadata: An arbitrary JSON object for storing application-specific data or identity-provider-specific data.
           - untrusted_metadata: An arbitrary JSON object of application-specific data. These fields can be edited directly by the
           frontend SDK, and should not be used to store critical information. See the [Metadata resource](https://stytch.com/docs/b2b/api/metadata)
           for complete field behavior details.
           - create_member_as_pending: Flag for whether or not to save a Member as `pending` or `active` in Stytch. It defaults to false. If true, new Members will be created with status `pending` in Stytch's backend. Their status will remain `pending` and they will continue to receive signup email templates for every Email Magic Link until that Member authenticates and becomes `active`. If false, new Members will be created with status `active`.
           - is_breakglass: Identifies the Member as a break glass user - someone who has permissions to authenticate into an Organization by bypassing the Organization's settings. A break glass account is typically used for emergency purposes to gain access outside of normal authentication procedures. Refer to the [Organization object](organization-object) and its `auth_methods` and `allowed_auth_methods` fields for more details.
-          - phone_number: (no documentation yet)
-          - mfa_enrolled: (no documentation yet)
+          - phone_number: (Coming Soon) Sets the Member's phone number.
+          - mfa_enrolled: (Coming Soon) Sets whether the Member is enrolled in MFA. If true, the Member must complete an MFA step whenever they wish to log in to their Organization. If false, the Member only needs to complete an MFA step if the Organization's MFA policy is set to `REQUIRED_FOR_ALL`.
         """  # noqa
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "email_address": email_address,
         }
         if name is not None:
             data["name"] = name
@@ -387,16 +399,16 @@
           - name: The name of the Member.
           - trusted_metadata: An arbitrary JSON object for storing application-specific data or identity-provider-specific data.
           - untrusted_metadata: An arbitrary JSON object of application-specific data. These fields can be edited directly by the
           frontend SDK, and should not be used to store critical information. See the [Metadata resource](https://stytch.com/docs/b2b/api/metadata)
           for complete field behavior details.
           - create_member_as_pending: Flag for whether or not to save a Member as `pending` or `active` in Stytch. It defaults to false. If true, new Members will be created with status `pending` in Stytch's backend. Their status will remain `pending` and they will continue to receive signup email templates for every Email Magic Link until that Member authenticates and becomes `active`. If false, new Members will be created with status `active`.
           - is_breakglass: Identifies the Member as a break glass user - someone who has permissions to authenticate into an Organization by bypassing the Organization's settings. A break glass account is typically used for emergency purposes to gain access outside of normal authentication procedures. Refer to the [Organization object](organization-object) and its `auth_methods` and `allowed_auth_methods` fields for more details.
-          - phone_number: (no documentation yet)
-          - mfa_enrolled: (no documentation yet)
+          - phone_number: (Coming Soon) Sets the Member's phone number.
+          - mfa_enrolled: (Coming Soon) Sets whether the Member is enrolled in MFA. If true, the Member must complete an MFA step whenever they wish to log in to their Organization. If false, the Member only needs to complete an MFA step if the Organization's MFA policy is set to `REQUIRED_FOR_ALL`.
         """  # noqa
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "email_address": email_address,
         }
         if name is not None:
             data["name"] = name
```

### Comparing `stytch-7.1.0/stytch/b2b/api/otp.py` & `stytch-7.2.0/stytch/b2b/api/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/b2b/api/passwords.py` & `stytch-7.2.0/stytch/b2b/api/passwords.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,22 +46,22 @@
     def strength_check(
         self,
         password: str,
         email_address: Optional[str] = None,
     ) -> StrengthCheckResponse:
         """This API allows you to check whether the user’s provided password is valid, and to provide feedback to the user on how to increase the strength of their password.
 
-        This endpoint adapts to your Project's password strength configuration. If you're using [zxcvbn](https://stytch.com/docs/passwords#strength-requirements), the default, your passwords are considered valid if the strength score is >= 3. If you're using [LUDS](https://stytch.com/docs/passwords#strength-requirements), your passwords are considered valid if they meet the requirements that you've set with Stytch. You may update your password strength configuration in the [stytch dashboard](https://stytch.com/dashboard/password-strength-config).
+        This endpoint adapts to your Project's password strength configuration. If you're using [zxcvbn](https://stytch.com/docs/guides/passwords/strength-policy), the default, your passwords are considered valid if the strength score is >= 3. If you're using [LUDS](https://stytch.com/docs/guides/passwords/strength-policy), your passwords are considered valid if they meet the requirements that you've set with Stytch. You may update your password strength configuration in the [stytch dashboard](https://stytch.com/dashboard/password-strength-config).
 
         ## Password feedback
         The zxcvbn_feedback and luds_feedback objects contains relevant fields for you to relay feedback to users that failed to create a strong enough password.
 
-        If you're using [zxcvbn](https://stytch.com/docs/passwords#strength-requirements), the feedback object will contain warning and suggestions for any password that does not meet the [zxcvbn](https://stytch.com/docs/passwords#strength-requirements) strength requirements. You can return these strings directly to the user to help them craft a strong password.
+        If you're using [zxcvbn](https://stytch.com/docs/guides/passwords/strength-policy), the feedback object will contain warning and suggestions for any password that does not meet the [zxcvbn](https://stytch.com/docs/guides/passwords/strength-policy) strength requirements. You can return these strings directly to the user to help them craft a strong password.
 
-        If you're using [LUDS](https://stytch.com/docs/passwords#strength-requirements), the feedback object will contain a collection of fields that the user failed or passed. You'll want to prompt the user to create a password that meets all requirements that they failed.
+        If you're using [LUDS](https://stytch.com/docs/guides/passwords/strength-policy), the feedback object will contain a collection of fields that the user failed or passed. You'll want to prompt the user to create a password that meets all requirements that they failed.
 
         Fields:
           - password: The password to authenticate.
           - email_address: The email address of the Member.
         """  # noqa
         data: Dict[str, Any] = {
             "password": password,
@@ -76,22 +76,22 @@
     async def strength_check_async(
         self,
         password: str,
         email_address: Optional[str] = None,
     ) -> StrengthCheckResponse:
         """This API allows you to check whether the user’s provided password is valid, and to provide feedback to the user on how to increase the strength of their password.
 
-        This endpoint adapts to your Project's password strength configuration. If you're using [zxcvbn](https://stytch.com/docs/passwords#strength-requirements), the default, your passwords are considered valid if the strength score is >= 3. If you're using [LUDS](https://stytch.com/docs/passwords#strength-requirements), your passwords are considered valid if they meet the requirements that you've set with Stytch. You may update your password strength configuration in the [stytch dashboard](https://stytch.com/dashboard/password-strength-config).
+        This endpoint adapts to your Project's password strength configuration. If you're using [zxcvbn](https://stytch.com/docs/guides/passwords/strength-policy), the default, your passwords are considered valid if the strength score is >= 3. If you're using [LUDS](https://stytch.com/docs/guides/passwords/strength-policy), your passwords are considered valid if they meet the requirements that you've set with Stytch. You may update your password strength configuration in the [stytch dashboard](https://stytch.com/dashboard/password-strength-config).
 
         ## Password feedback
         The zxcvbn_feedback and luds_feedback objects contains relevant fields for you to relay feedback to users that failed to create a strong enough password.
 
-        If you're using [zxcvbn](https://stytch.com/docs/passwords#strength-requirements), the feedback object will contain warning and suggestions for any password that does not meet the [zxcvbn](https://stytch.com/docs/passwords#strength-requirements) strength requirements. You can return these strings directly to the user to help them craft a strong password.
+        If you're using [zxcvbn](https://stytch.com/docs/guides/passwords/strength-policy), the feedback object will contain warning and suggestions for any password that does not meet the [zxcvbn](https://stytch.com/docs/guides/passwords/strength-policy) strength requirements. You can return these strings directly to the user to help them craft a strong password.
 
-        If you're using [LUDS](https://stytch.com/docs/passwords#strength-requirements), the feedback object will contain a collection of fields that the user failed or passed. You'll want to prompt the user to create a password that meets all requirements that they failed.
+        If you're using [LUDS](https://stytch.com/docs/guides/passwords/strength-policy), the feedback object will contain a collection of fields that the user failed or passed. You'll want to prompt the user to create a password that meets all requirements that they failed.
 
         Fields:
           - password: The password to authenticate.
           - email_address: The email address of the Member.
         """  # noqa
         data: Dict[str, Any] = {
             "password": password,
@@ -237,14 +237,20 @@
         """Authenticate a member with their email address and password. This endpoint verifies that the member has a password currently set, and that the entered password is correct. There are two instances where the endpoint will return a reset_password error even if they enter their previous password:
         * The member’s credentials appeared in the HaveIBeenPwned dataset.
             * We force a password reset to ensure that the member is the legitimate owner of the email address, and not a malicious actor abusing the compromised credentials.
         * A member that has previously authenticated with email/password uses a passwordless authentication method tied to the same email address (e.g. Magic Links) for the first time. Any subsequent email/password authentication attempt will result in this error.
             * We force a password reset in this instance in order to safely deduplicate the account by email address, without introducing the risk of a pre-hijack account takeover attack.
             * Imagine a bad actor creates many accounts using passwords and the known email addresses of their victims. If a victim comes to the site and logs in for the first time with an email-based passwordless authentication method then both the victim and the bad actor have credentials to access to the same account. To prevent this, any further email/password login attempts first require a password reset which can only be accomplished by someone with access to the underlying email address.
 
+        (Coming Soon) If the Member is required to complete MFA to log in to the Organization, the returned value of `member_authenticated` will be `false`, and an `intermediate_session_token` will be returned.
+        The `intermediate_session_token` can be passed into the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete the MFA step and acquire a full member session.
+        The `session_duration_minutes` and `session_custom_claims` parameters will be ignored.
+
+        If a valid `session_token` or `session_jwt` is passed in, the Member will not be required to complete an MFA step.
+
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - email_address: The email address of the Member.
           - password: The password to authenticate.
           - session_token: A secret token for a given Stytch Session.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
@@ -257,15 +263,22 @@
           If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
           to use the Stytch session product, you can ignore the session fields in the response.
           - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
-          - locale: (no documentation yet)
+          - locale: (Coming Soon) If the Member needs to complete an MFA step, and the Member has a phone number, this endpoint will pre-emptively send a one-time passcode (OTP) to the Member's phone number. The locale argument will be used to determine which language to use when sending the passcode.
+
+        Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
+
+        Currently supported languages are English (`"en"`), Spanish (`"es"`), and Brazilian Portuguese (`"pt-br"`); if no value is provided, the copy defaults to English.
+
+        Request support for additional languages [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link")!
+
         """  # noqa
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "email_address": email_address,
             "password": password,
         }
         if session_token is not None:
@@ -297,14 +310,20 @@
         """Authenticate a member with their email address and password. This endpoint verifies that the member has a password currently set, and that the entered password is correct. There are two instances where the endpoint will return a reset_password error even if they enter their previous password:
         * The member’s credentials appeared in the HaveIBeenPwned dataset.
             * We force a password reset to ensure that the member is the legitimate owner of the email address, and not a malicious actor abusing the compromised credentials.
         * A member that has previously authenticated with email/password uses a passwordless authentication method tied to the same email address (e.g. Magic Links) for the first time. Any subsequent email/password authentication attempt will result in this error.
             * We force a password reset in this instance in order to safely deduplicate the account by email address, without introducing the risk of a pre-hijack account takeover attack.
             * Imagine a bad actor creates many accounts using passwords and the known email addresses of their victims. If a victim comes to the site and logs in for the first time with an email-based passwordless authentication method then both the victim and the bad actor have credentials to access to the same account. To prevent this, any further email/password login attempts first require a password reset which can only be accomplished by someone with access to the underlying email address.
 
+        (Coming Soon) If the Member is required to complete MFA to log in to the Organization, the returned value of `member_authenticated` will be `false`, and an `intermediate_session_token` will be returned.
+        The `intermediate_session_token` can be passed into the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete the MFA step and acquire a full member session.
+        The `session_duration_minutes` and `session_custom_claims` parameters will be ignored.
+
+        If a valid `session_token` or `session_jwt` is passed in, the Member will not be required to complete an MFA step.
+
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - email_address: The email address of the Member.
           - password: The password to authenticate.
           - session_token: A secret token for a given Stytch Session.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
@@ -317,15 +336,22 @@
           If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
           to use the Stytch session product, you can ignore the session fields in the response.
           - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
-          - locale: (no documentation yet)
+          - locale: (Coming Soon) If the Member needs to complete an MFA step, and the Member has a phone number, this endpoint will pre-emptively send a one-time passcode (OTP) to the Member's phone number. The locale argument will be used to determine which language to use when sending the passcode.
+
+        Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
+
+        Currently supported languages are English (`"en"`), Spanish (`"es"`), and Brazilian Portuguese (`"pt-br"`); if no value is provided, the copy defaults to English.
+
+        Request support for additional languages [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link")!
+
         """  # noqa
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "email_address": email_address,
             "password": password,
         }
         if session_token is not None:
```

### Comparing `stytch-7.1.0/stytch/b2b/api/passwords_email.py` & `stytch-7.2.0/stytch/b2b/api/passwords_email.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,16 +39,16 @@
         login_redirect_url: Optional[str] = None,
         locale: Optional[ResetStartRequestLocale] = None,
         reset_password_template_id: Optional[str] = None,
     ) -> ResetStartResponse:
         """Initiates a password reset for the email address provided. This will trigger an email to be sent to the address, containing a magic link that will allow them to set a new password and authenticate.
 
         This endpoint adapts to your Project's password strength configuration.
-        If you're using [zxcvbn](https://stytch.com/docs/passwords#strength-requirements), the default, your passwords are considered valid
-        if the strength score is >= 3. If you're using [LUDS](https://stytch.com/docs/passwords#strength-requirements), your passwords are
+        If you're using [zxcvbn](https://stytch.com/docs/guides/passwords/strength-policy), the default, your passwords are considered valid
+        if the strength score is >= 3. If you're using [LUDS](https://stytch.com/docs/guides/passwords/strength-policy), your passwords are
         considered valid if they meet the requirements that you've set with Stytch.
         You may update your password strength configuration in the [stytch dashboard](https://stytch.com/dashboard/password-strength-config).
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - email_address: The email address of the Member to start the email reset process for.
           - reset_password_redirect_url: The URL that the Member clicks from the reset password link. This URL should be an endpoint in the backend server that verifies the request by querying
@@ -101,16 +101,16 @@
         login_redirect_url: Optional[str] = None,
         locale: Optional[ResetStartRequestLocale] = None,
         reset_password_template_id: Optional[str] = None,
     ) -> ResetStartResponse:
         """Initiates a password reset for the email address provided. This will trigger an email to be sent to the address, containing a magic link that will allow them to set a new password and authenticate.
 
         This endpoint adapts to your Project's password strength configuration.
-        If you're using [zxcvbn](https://stytch.com/docs/passwords#strength-requirements), the default, your passwords are considered valid
-        if the strength score is >= 3. If you're using [LUDS](https://stytch.com/docs/passwords#strength-requirements), your passwords are
+        If you're using [zxcvbn](https://stytch.com/docs/guides/passwords/strength-policy), the default, your passwords are considered valid
+        if the strength score is >= 3. If you're using [LUDS](https://stytch.com/docs/guides/passwords/strength-policy), your passwords are
         considered valid if they meet the requirements that you've set with Stytch.
         You may update your password strength configuration in the [stytch dashboard](https://stytch.com/dashboard/password-strength-config).
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - email_address: The email address of the Member to start the email reset process for.
           - reset_password_redirect_url: The URL that the Member clicks from the reset password link. This URL should be an endpoint in the backend server that verifies the request by querying
@@ -164,14 +164,20 @@
         session_custom_claims: Optional[Dict[str, Any]] = None,
         locale: Optional[ResetRequestLocale] = None,
     ) -> ResetResponse:
         """Reset the member's password and authenticate them. This endpoint checks that the password reset token is valid, hasn’t expired, or already been used.
 
         The provided password needs to meet our password strength requirements, which can be checked in advance with the password strength endpoint. If the token and password are accepted, the password is securely stored for future authentication and the user is authenticated.
 
+        (Coming Soon) If the Member is required to complete MFA to log in to the Organization, the returned value of `member_authenticated` will be `false`, and an `intermediate_session_token` will be returned.
+        The `intermediate_session_token` can be passed into the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete the MFA step and acquire a full member session.
+        The `session_duration_minutes` and `session_custom_claims` parameters will be ignored.
+
+        If a valid `session_token` or `session_jwt` is passed in, the Member will not be required to complete an MFA step.
+
         Fields:
           - password_reset_token: The password reset token to authenticate.
           - password: The password to reset.
           - session_token: Reuse an existing session instead of creating a new one. If you provide a `session_token`, Stytch will update the session.
               If the `session_token` and `magic_links_token` belong to different Members, the `session_token` will be ignored. This endpoint will error if
               both `session_token` and `session_jwt` are provided.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
@@ -188,15 +194,22 @@
               and `magic_links_token` belong to different Members, the `session_jwt` will be ignored. This endpoint will error if both `session_token` and `session_jwt`
               are provided.
           - code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
-          - locale: (no documentation yet)
+          - locale: (Coming Soon) If the Member needs to complete an MFA step, and the Member has a phone number, this endpoint will pre-emptively send a one-time passcode (OTP) to the Member's phone number. The locale argument will be used to determine which language to use when sending the passcode.
+
+        Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
+
+        Currently supported languages are English (`"en"`), Spanish (`"es"`), and Brazilian Portuguese (`"pt-br"`); if no value is provided, the copy defaults to English.
+
+        Request support for additional languages [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link")!
+
         """  # noqa
         data: Dict[str, Any] = {
             "password_reset_token": password_reset_token,
             "password": password,
         }
         if session_token is not None:
             data["session_token"] = session_token
@@ -226,14 +239,20 @@
         session_custom_claims: Optional[Dict[str, Any]] = None,
         locale: Optional[ResetRequestLocale] = None,
     ) -> ResetResponse:
         """Reset the member's password and authenticate them. This endpoint checks that the password reset token is valid, hasn’t expired, or already been used.
 
         The provided password needs to meet our password strength requirements, which can be checked in advance with the password strength endpoint. If the token and password are accepted, the password is securely stored for future authentication and the user is authenticated.
 
+        (Coming Soon) If the Member is required to complete MFA to log in to the Organization, the returned value of `member_authenticated` will be `false`, and an `intermediate_session_token` will be returned.
+        The `intermediate_session_token` can be passed into the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete the MFA step and acquire a full member session.
+        The `session_duration_minutes` and `session_custom_claims` parameters will be ignored.
+
+        If a valid `session_token` or `session_jwt` is passed in, the Member will not be required to complete an MFA step.
+
         Fields:
           - password_reset_token: The password reset token to authenticate.
           - password: The password to reset.
           - session_token: Reuse an existing session instead of creating a new one. If you provide a `session_token`, Stytch will update the session.
               If the `session_token` and `magic_links_token` belong to different Members, the `session_token` will be ignored. This endpoint will error if
               both `session_token` and `session_jwt` are provided.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
@@ -250,15 +269,22 @@
               and `magic_links_token` belong to different Members, the `session_jwt` will be ignored. This endpoint will error if both `session_token` and `session_jwt`
               are provided.
           - code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
-          - locale: (no documentation yet)
+          - locale: (Coming Soon) If the Member needs to complete an MFA step, and the Member has a phone number, this endpoint will pre-emptively send a one-time passcode (OTP) to the Member's phone number. The locale argument will be used to determine which language to use when sending the passcode.
+
+        Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
+
+        Currently supported languages are English (`"en"`), Spanish (`"es"`), and Brazilian Portuguese (`"pt-br"`); if no value is provided, the copy defaults to English.
+
+        Request support for additional languages [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link")!
+
         """  # noqa
         data: Dict[str, Any] = {
             "password_reset_token": password_reset_token,
             "password": password,
         }
         if session_token is not None:
             data["session_token"] = session_token
```

### Comparing `stytch-7.1.0/stytch/b2b/api/passwords_existing_password.py` & `stytch-7.2.0/stytch/b2b/api/passwords_existing_password.py`

 * *Files 17% similar despite different names*

```diff
@@ -38,19 +38,25 @@
         session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
         locale: Optional[ResetRequestLocale] = None,
     ) -> ResetResponse:
         """Reset the member’s password using their existing password.
 
         This endpoint adapts to your Project's password strength configuration.
-        If you're using [zxcvbn](https://stytch.com/docs/passwords#strength-requirements), the default, your passwords are considered valid
-        if the strength score is >= 3. If you're using [LUDS](https://stytch.com/docs/passwords#strength-requirements), your passwords are
+        If you're using [zxcvbn](https://stytch.com/docs/guides/passwords/strength-policy), the default, your passwords are considered valid
+        if the strength score is >= 3. If you're using [LUDS](https://stytch.com/docs/guides/passwords/strength-policy), your passwords are
         considered valid if they meet the requirements that you've set with Stytch.
         You may update your password strength configuration in the [stytch dashboard](https://stytch.com/dashboard/password-strength-config).
 
+        (Coming Soon) If the Member is required to complete MFA to log in to the Organization, the returned value of `member_authenticated` will be `false`, and an `intermediate_session_token` will be returned.
+        The `intermediate_session_token` can be passed into the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete the MFA step and acquire a full member session.
+        The `session_duration_minutes` and `session_custom_claims` parameters will be ignored.
+
+        If a valid `session_token` or `session_jwt` is passed in, the Member will not be required to complete an MFA step.
+
         Fields:
           - email_address: The email address of the Member.
           - existing_password: The member's current password that they supplied.
           - new_password: The member's elected new password.
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - session_token: A secret token for a given Stytch Session.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
@@ -64,15 +70,22 @@
           If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
           to use the Stytch session product, you can ignore the session fields in the response.
           - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
-          - locale: (no documentation yet)
+          - locale: (Coming Soon) If the Member needs to complete an MFA step, and the Member has a phone number, this endpoint will pre-emptively send a one-time passcode (OTP) to the Member's phone number. The locale argument will be used to determine which language to use when sending the passcode.
+
+        Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
+
+        Currently supported languages are English (`"en"`), Spanish (`"es"`), and Brazilian Portuguese (`"pt-br"`); if no value is provided, the copy defaults to English.
+
+        Request support for additional languages [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link")!
+
         """  # noqa
         data: Dict[str, Any] = {
             "email_address": email_address,
             "existing_password": existing_password,
             "new_password": new_password,
             "organization_id": organization_id,
         }
@@ -102,19 +115,25 @@
         session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
         locale: Optional[ResetRequestLocale] = None,
     ) -> ResetResponse:
         """Reset the member’s password using their existing password.
 
         This endpoint adapts to your Project's password strength configuration.
-        If you're using [zxcvbn](https://stytch.com/docs/passwords#strength-requirements), the default, your passwords are considered valid
-        if the strength score is >= 3. If you're using [LUDS](https://stytch.com/docs/passwords#strength-requirements), your passwords are
+        If you're using [zxcvbn](https://stytch.com/docs/guides/passwords/strength-policy), the default, your passwords are considered valid
+        if the strength score is >= 3. If you're using [LUDS](https://stytch.com/docs/guides/passwords/strength-policy), your passwords are
         considered valid if they meet the requirements that you've set with Stytch.
         You may update your password strength configuration in the [stytch dashboard](https://stytch.com/dashboard/password-strength-config).
 
+        (Coming Soon) If the Member is required to complete MFA to log in to the Organization, the returned value of `member_authenticated` will be `false`, and an `intermediate_session_token` will be returned.
+        The `intermediate_session_token` can be passed into the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete the MFA step and acquire a full member session.
+        The `session_duration_minutes` and `session_custom_claims` parameters will be ignored.
+
+        If a valid `session_token` or `session_jwt` is passed in, the Member will not be required to complete an MFA step.
+
         Fields:
           - email_address: The email address of the Member.
           - existing_password: The member's current password that they supplied.
           - new_password: The member's elected new password.
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - session_token: A secret token for a given Stytch Session.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
@@ -128,15 +147,22 @@
           If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
           to use the Stytch session product, you can ignore the session fields in the response.
           - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
-          - locale: (no documentation yet)
+          - locale: (Coming Soon) If the Member needs to complete an MFA step, and the Member has a phone number, this endpoint will pre-emptively send a one-time passcode (OTP) to the Member's phone number. The locale argument will be used to determine which language to use when sending the passcode.
+
+        Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
+
+        Currently supported languages are English (`"en"`), Spanish (`"es"`), and Brazilian Portuguese (`"pt-br"`); if no value is provided, the copy defaults to English.
+
+        Request support for additional languages [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link")!
+
         """  # noqa
         data: Dict[str, Any] = {
             "email_address": email_address,
             "existing_password": existing_password,
             "new_password": new_password,
             "organization_id": organization_id,
         }
```

### Comparing `stytch-7.1.0/stytch/b2b/api/passwords_session.py` & `stytch-7.2.0/stytch/b2b/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/b2b/api/sessions.py` & `stytch-7.2.0/stytch/consumer/api/totps.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,349 +4,287 @@
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
 from typing import Any, Dict, Optional
 
-from stytch.b2b.models.sessions import (
+from stytch.consumer.models.totps import (
     AuthenticateResponse,
-    ExchangeRequestLocale,
-    ExchangeResponse,
-    GetJWKSResponse,
-    GetResponse,
-    RevokeResponse,
+    CreateResponse,
+    RecoverResponse,
+    RecoveryCodesResponse,
 )
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
-class Sessions:
+class TOTPs:
     def __init__(
         self,
         api_base: ApiBase,
         sync_client: SyncClient,
         async_client: AsyncClient,
     ) -> None:
         self.api_base = api_base
         self.sync_client = sync_client
         self.async_client = async_client
 
-    def get(
+    def create(
         self,
-        organization_id: str,
-        member_id: str,
-    ) -> GetResponse:
-        """Retrieves all active Sessions for a Member.
+        user_id: str,
+        expiration_minutes: Optional[int] = None,
+    ) -> CreateResponse:
+        """Create a new TOTP instance for a user. The user can use the authenticator application of their choice to scan the QR code or enter the secret.
 
         Fields:
-          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
-          - member_id: Globally unique UUID that identifies a specific Member. The `member_id` is critical to perform operations on a Member, so be sure to preserve this value.
+          - user_id: The `user_id` of an active user the TOTP registration should be tied to.
+          - expiration_minutes: The expiration for the TOTP instance. If the newly created TOTP is not authenticated within this time frame the TOTP will be unusable. Defaults to 60 (1 hour) with a minimum of 5 and a maximum of 1440.
         """  # noqa
         data: Dict[str, Any] = {
-            "organization_id": organization_id,
-            "member_id": member_id,
+            "user_id": user_id,
         }
+        if expiration_minutes is not None:
+            data["expiration_minutes"] = expiration_minutes
 
-        url = self.api_base.url_for("/v1/b2b/sessions", data)
-        res = self.sync_client.get(url, data)
-        return GetResponse.from_json(res.response.status_code, res.json)
+        url = self.api_base.url_for("/v1/totps", data)
+        res = self.sync_client.post(url, data)
+        return CreateResponse.from_json(res.response.status_code, res.json)
 
-    async def get_async(
+    async def create_async(
         self,
-        organization_id: str,
-        member_id: str,
-    ) -> GetResponse:
-        """Retrieves all active Sessions for a Member.
+        user_id: str,
+        expiration_minutes: Optional[int] = None,
+    ) -> CreateResponse:
+        """Create a new TOTP instance for a user. The user can use the authenticator application of their choice to scan the QR code or enter the secret.
 
         Fields:
-          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
-          - member_id: Globally unique UUID that identifies a specific Member. The `member_id` is critical to perform operations on a Member, so be sure to preserve this value.
+          - user_id: The `user_id` of an active user the TOTP registration should be tied to.
+          - expiration_minutes: The expiration for the TOTP instance. If the newly created TOTP is not authenticated within this time frame the TOTP will be unusable. Defaults to 60 (1 hour) with a minimum of 5 and a maximum of 1440.
         """  # noqa
         data: Dict[str, Any] = {
-            "organization_id": organization_id,
-            "member_id": member_id,
+            "user_id": user_id,
         }
+        if expiration_minutes is not None:
+            data["expiration_minutes"] = expiration_minutes
 
-        url = self.api_base.url_for("/v1/b2b/sessions", data)
-        res = await self.async_client.get(url, data)
-        return GetResponse.from_json(res.response.status, res.json)
+        url = self.api_base.url_for("/v1/totps", data)
+        res = await self.async_client.post(url, data)
+        return CreateResponse.from_json(res.response.status, res.json)
 
     def authenticate(
         self,
+        user_id: str,
+        totp_code: str,
         session_token: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
     ) -> AuthenticateResponse:
-        """Authenticates a Session and updates its lifetime by the specified `session_duration_minutes`. If the `session_duration_minutes` is not specified, a Session will not be extended. This endpoint requires either a `session_jwt` or `session_token` be included in the request. It will return an error if both are present.
-
-        You may provide a JWT that needs to be refreshed and is expired according to its `exp` claim. A new JWT will be returned if both the signature and the underlying Session are still valid.
+        """Authenticate a TOTP code entered by a user.
 
         Fields:
-          - session_token: A secret token for a given Stytch Session.
+          - user_id: The `user_id` of an active user the TOTP registration should be tied to.
+          - totp_code: The TOTP code to authenticate. The TOTP code should consist of 6 digits.
+          - session_token: The `session_token` associated with a User's existing Session.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
           five minutes regardless of the underlying session duration, and will need to be refreshed over time.
 
           This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
 
           If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
 
-          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
-          to use the Stytch session product, you can ignore the session fields in the response.
-          - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
-          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
-          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
-          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
-          Total custom claims size cannot exceed four kilobytes.
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will not be created.
+          - session_jwt: The `session_jwt` associated with a User's existing Session.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value.
+
+          Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes.
         """  # noqa
-        data: Dict[str, Any] = {}
+        data: Dict[str, Any] = {
+            "user_id": user_id,
+            "totp_code": totp_code,
+        }
         if session_token is not None:
             data["session_token"] = session_token
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
 
-        url = self.api_base.url_for("/v1/b2b/sessions/authenticate", data)
+        url = self.api_base.url_for("/v1/totps/authenticate", data)
         res = self.sync_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status_code, res.json)
 
     async def authenticate_async(
         self,
+        user_id: str,
+        totp_code: str,
         session_token: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
     ) -> AuthenticateResponse:
-        """Authenticates a Session and updates its lifetime by the specified `session_duration_minutes`. If the `session_duration_minutes` is not specified, a Session will not be extended. This endpoint requires either a `session_jwt` or `session_token` be included in the request. It will return an error if both are present.
-
-        You may provide a JWT that needs to be refreshed and is expired according to its `exp` claim. A new JWT will be returned if both the signature and the underlying Session are still valid.
+        """Authenticate a TOTP code entered by a user.
 
         Fields:
-          - session_token: A secret token for a given Stytch Session.
+          - user_id: The `user_id` of an active user the TOTP registration should be tied to.
+          - totp_code: The TOTP code to authenticate. The TOTP code should consist of 6 digits.
+          - session_token: The `session_token` associated with a User's existing Session.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
           five minutes regardless of the underlying session duration, and will need to be refreshed over time.
 
           This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
 
           If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
 
-          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
-          to use the Stytch session product, you can ignore the session fields in the response.
-          - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
-          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
-          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
-          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
-          Total custom claims size cannot exceed four kilobytes.
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will not be created.
+          - session_jwt: The `session_jwt` associated with a User's existing Session.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value.
+
+          Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes.
         """  # noqa
-        data: Dict[str, Any] = {}
+        data: Dict[str, Any] = {
+            "user_id": user_id,
+            "totp_code": totp_code,
+        }
         if session_token is not None:
             data["session_token"] = session_token
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
 
-        url = self.api_base.url_for("/v1/b2b/sessions/authenticate", data)
+        url = self.api_base.url_for("/v1/totps/authenticate", data)
         res = await self.async_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status, res.json)
 
-    def revoke(
+    def recovery_codes(
         self,
-        member_session_id: Optional[str] = None,
-        session_token: Optional[str] = None,
-        session_jwt: Optional[str] = None,
-        member_id: Optional[str] = None,
-    ) -> RevokeResponse:
-        """Revoke a Session and immediately invalidate all its tokens. To revoke a specific Session, pass either the `member_session_id`, `session_token`, or `session_jwt`. To revoke all Sessions for a Member, pass the `member_id`.
+        user_id: str,
+    ) -> RecoveryCodesResponse:
+        """Retrieve the recovery codes for a TOTP instance tied to a User.
 
         Fields:
-          - member_session_id: Globally unique UUID that identifies a specific Session in the Stytch API. The `member_session_id` is critical to perform operations on an Session, so be sure to preserve this value.
-          - session_token: A secret token for a given Stytch Session.
-          - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
-          - member_id: Globally unique UUID that identifies a specific Member. The `member_id` is critical to perform operations on a Member, so be sure to preserve this value.
+          - user_id: The `user_id` of an active user the TOTP registration should be tied to.
         """  # noqa
-        data: Dict[str, Any] = {}
-        if member_session_id is not None:
-            data["member_session_id"] = member_session_id
-        if session_token is not None:
-            data["session_token"] = session_token
-        if session_jwt is not None:
-            data["session_jwt"] = session_jwt
-        if member_id is not None:
-            data["member_id"] = member_id
+        data: Dict[str, Any] = {
+            "user_id": user_id,
+        }
 
-        url = self.api_base.url_for("/v1/b2b/sessions/revoke", data)
+        url = self.api_base.url_for("/v1/totps/recovery_codes", data)
         res = self.sync_client.post(url, data)
-        return RevokeResponse.from_json(res.response.status_code, res.json)
+        return RecoveryCodesResponse.from_json(res.response.status_code, res.json)
 
-    async def revoke_async(
+    async def recovery_codes_async(
         self,
-        member_session_id: Optional[str] = None,
-        session_token: Optional[str] = None,
-        session_jwt: Optional[str] = None,
-        member_id: Optional[str] = None,
-    ) -> RevokeResponse:
-        """Revoke a Session and immediately invalidate all its tokens. To revoke a specific Session, pass either the `member_session_id`, `session_token`, or `session_jwt`. To revoke all Sessions for a Member, pass the `member_id`.
+        user_id: str,
+    ) -> RecoveryCodesResponse:
+        """Retrieve the recovery codes for a TOTP instance tied to a User.
 
         Fields:
-          - member_session_id: Globally unique UUID that identifies a specific Session in the Stytch API. The `member_session_id` is critical to perform operations on an Session, so be sure to preserve this value.
-          - session_token: A secret token for a given Stytch Session.
-          - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
-          - member_id: Globally unique UUID that identifies a specific Member. The `member_id` is critical to perform operations on a Member, so be sure to preserve this value.
+          - user_id: The `user_id` of an active user the TOTP registration should be tied to.
         """  # noqa
-        data: Dict[str, Any] = {}
-        if member_session_id is not None:
-            data["member_session_id"] = member_session_id
-        if session_token is not None:
-            data["session_token"] = session_token
-        if session_jwt is not None:
-            data["session_jwt"] = session_jwt
-        if member_id is not None:
-            data["member_id"] = member_id
+        data: Dict[str, Any] = {
+            "user_id": user_id,
+        }
 
-        url = self.api_base.url_for("/v1/b2b/sessions/revoke", data)
+        url = self.api_base.url_for("/v1/totps/recovery_codes", data)
         res = await self.async_client.post(url, data)
-        return RevokeResponse.from_json(res.response.status, res.json)
+        return RecoveryCodesResponse.from_json(res.response.status, res.json)
 
-    def exchange(
+    def recover(
         self,
-        organization_id: str,
+        user_id: str,
+        recovery_code: str,
         session_token: Optional[str] = None,
-        session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
+        session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
-        locale: Optional[ExchangeRequestLocale] = None,
-    ) -> ExchangeResponse:
-        """Use this endpoint to exchange a Member's existing session for another session in a different Organization. This can be used to accept an invite, but not to create a new member via domain matching.
-
-        To create a new member via domain matching, use the [Exchange Intermediate Session](https://stytch.com/docs/b2b/api/exchange-intermediate-session) flow instead.
+    ) -> RecoverResponse:
+        """Authenticate a recovery code for a TOTP instance.
 
         Fields:
-          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
-          - session_token: The `session_token` belonging to the member that you wish to associate the email with.
-          - session_jwt: The `session_jwt` belonging to the member that you wish to associate the email with.
+          - user_id: The `user_id` of an active user the TOTP registration should be tied to.
+          - recovery_code: The recovery code to authenticate.
+          - session_token: The `session_token` associated with a User's existing Session.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
           five minutes regardless of the underlying session duration, and will need to be refreshed over time.
 
           This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
 
           If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
 
-          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
-          to use the Stytch session product, you can ignore the session fields in the response.
-          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
-          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
-          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
-          Total custom claims size cannot exceed four kilobytes.
-          - locale: (no documentation yet)
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will not be created.
+          - session_jwt: The `session_jwt` associated with a User's existing Session.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value.
+
+          Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes.
         """  # noqa
         data: Dict[str, Any] = {
-            "organization_id": organization_id,
+            "user_id": user_id,
+            "recovery_code": recovery_code,
         }
         if session_token is not None:
             data["session_token"] = session_token
-        if session_jwt is not None:
-            data["session_jwt"] = session_jwt
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
+        if session_jwt is not None:
+            data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
-        if locale is not None:
-            data["locale"] = locale.value
 
-        url = self.api_base.url_for("/v1/b2b/sessions/exchange", data)
+        url = self.api_base.url_for("/v1/totps/recover", data)
         res = self.sync_client.post(url, data)
-        return ExchangeResponse.from_json(res.response.status_code, res.json)
+        return RecoverResponse.from_json(res.response.status_code, res.json)
 
-    async def exchange_async(
+    async def recover_async(
         self,
-        organization_id: str,
+        user_id: str,
+        recovery_code: str,
         session_token: Optional[str] = None,
-        session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
+        session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
-        locale: Optional[ExchangeRequestLocale] = None,
-    ) -> ExchangeResponse:
-        """Use this endpoint to exchange a Member's existing session for another session in a different Organization. This can be used to accept an invite, but not to create a new member via domain matching.
-
-        To create a new member via domain matching, use the [Exchange Intermediate Session](https://stytch.com/docs/b2b/api/exchange-intermediate-session) flow instead.
+    ) -> RecoverResponse:
+        """Authenticate a recovery code for a TOTP instance.
 
         Fields:
-          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
-          - session_token: The `session_token` belonging to the member that you wish to associate the email with.
-          - session_jwt: The `session_jwt` belonging to the member that you wish to associate the email with.
+          - user_id: The `user_id` of an active user the TOTP registration should be tied to.
+          - recovery_code: The recovery code to authenticate.
+          - session_token: The `session_token` associated with a User's existing Session.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
           five minutes regardless of the underlying session duration, and will need to be refreshed over time.
 
           This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
 
           If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
 
-          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
-          to use the Stytch session product, you can ignore the session fields in the response.
-          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
-          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
-          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
-          Total custom claims size cannot exceed four kilobytes.
-          - locale: (no documentation yet)
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will not be created.
+          - session_jwt: The `session_jwt` associated with a User's existing Session.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value.
+
+          Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes.
         """  # noqa
         data: Dict[str, Any] = {
-            "organization_id": organization_id,
+            "user_id": user_id,
+            "recovery_code": recovery_code,
         }
         if session_token is not None:
             data["session_token"] = session_token
-        if session_jwt is not None:
-            data["session_jwt"] = session_jwt
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
+        if session_jwt is not None:
+            data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
-        if locale is not None:
-            data["locale"] = locale.value
 
-        url = self.api_base.url_for("/v1/b2b/sessions/exchange", data)
+        url = self.api_base.url_for("/v1/totps/recover", data)
         res = await self.async_client.post(url, data)
-        return ExchangeResponse.from_json(res.response.status, res.json)
-
-    def get_jwks(
-        self,
-        project_id: str,
-    ) -> GetJWKSResponse:
-        """Get the JSON Web Key Set (JWKS) for a project.
-
-        Fields:
-          - project_id: The `project_id` to get the JWKS for.
-        """  # noqa
-        data: Dict[str, Any] = {
-            "project_id": project_id,
-        }
-
-        url = self.api_base.url_for("/v1/b2b/sessions/jwks/{project_id}", data)
-        res = self.sync_client.get(url, data)
-        return GetJWKSResponse.from_json(res.response.status_code, res.json)
-
-    async def get_jwks_async(
-        self,
-        project_id: str,
-    ) -> GetJWKSResponse:
-        """Get the JSON Web Key Set (JWKS) for a project.
-
-        Fields:
-          - project_id: The `project_id` to get the JWKS for.
-        """  # noqa
-        data: Dict[str, Any] = {
-            "project_id": project_id,
-        }
-
-        url = self.api_base.url_for("/v1/b2b/sessions/jwks/{project_id}", data)
-        res = await self.async_client.get(url, data)
-        return GetJWKSResponse.from_json(res.response.status, res.json)
+        return RecoverResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-7.1.0/stytch/b2b/api/sso.py` & `stytch-7.2.0/stytch/b2b/api/sso.py`

 * *Files 16% similar despite different names*

```diff
@@ -123,14 +123,20 @@
     ) -> AuthenticateResponse:
         """Authenticate a user given a token.
         This endpoint verifies that the user completed the SSO Authentication flow by verifying that the token is valid and hasn't expired.
         Provide the `session_duration_minutes` parameter to set the lifetime of the session.
         If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration.
         To link this authentication event to an existing Stytch session, include either the `session_token` or `session_jwt` param.
 
+        (Coming Soon) If the Member is required to complete MFA to log in to the Organization, the returned value of `member_authenticated` will be `false`, and an `intermediate_session_token` will be returned.
+        The `intermediate_session_token` can be passed into the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete the MFA step and acquire a full member session.
+        The `session_duration_minutes` and `session_custom_claims` parameters will be ignored.
+
+        If a valid `session_token` or `session_jwt` is passed in, the Member will not be required to complete an MFA step.
+
         Fields:
           - sso_token: The token to authenticate.
           - pkce_code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
           - session_token: The `session_token` belonging to the member that you wish to associate the email with.
           - session_jwt: The `session_jwt` belonging to the member that you wish to associate the email with.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
@@ -142,15 +148,22 @@
 
           If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
           to use the Stytch session product, you can ignore the session fields in the response.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
-          - locale: (no documentation yet)
+          - locale: (Coming Soon) If the Member needs to complete an MFA step, and the Member has a phone number, this endpoint will pre-emptively send a one-time passcode (OTP) to the Member's phone number. The locale argument will be used to determine which language to use when sending the passcode.
+
+        Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
+
+        Currently supported languages are English (`"en"`), Spanish (`"es"`), and Brazilian Portuguese (`"pt-br"`); if no value is provided, the copy defaults to English.
+
+        Request support for additional languages [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link")!
+
         """  # noqa
         data: Dict[str, Any] = {
             "sso_token": sso_token,
         }
         if pkce_code_verifier is not None:
             data["pkce_code_verifier"] = pkce_code_verifier
         if session_token is not None:
@@ -180,14 +193,20 @@
     ) -> AuthenticateResponse:
         """Authenticate a user given a token.
         This endpoint verifies that the user completed the SSO Authentication flow by verifying that the token is valid and hasn't expired.
         Provide the `session_duration_minutes` parameter to set the lifetime of the session.
         If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration.
         To link this authentication event to an existing Stytch session, include either the `session_token` or `session_jwt` param.
 
+        (Coming Soon) If the Member is required to complete MFA to log in to the Organization, the returned value of `member_authenticated` will be `false`, and an `intermediate_session_token` will be returned.
+        The `intermediate_session_token` can be passed into the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete the MFA step and acquire a full member session.
+        The `session_duration_minutes` and `session_custom_claims` parameters will be ignored.
+
+        If a valid `session_token` or `session_jwt` is passed in, the Member will not be required to complete an MFA step.
+
         Fields:
           - sso_token: The token to authenticate.
           - pkce_code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
           - session_token: The `session_token` belonging to the member that you wish to associate the email with.
           - session_jwt: The `session_jwt` belonging to the member that you wish to associate the email with.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
@@ -199,15 +218,22 @@
 
           If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
           to use the Stytch session product, you can ignore the session fields in the response.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
-          - locale: (no documentation yet)
+          - locale: (Coming Soon) If the Member needs to complete an MFA step, and the Member has a phone number, this endpoint will pre-emptively send a one-time passcode (OTP) to the Member's phone number. The locale argument will be used to determine which language to use when sending the passcode.
+
+        Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
+
+        Currently supported languages are English (`"en"`), Spanish (`"es"`), and Brazilian Portuguese (`"pt-br"`); if no value is provided, the copy defaults to English.
+
+        Request support for additional languages [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link")!
+
         """  # noqa
         data: Dict[str, Any] = {
             "sso_token": sso_token,
         }
         if pkce_code_verifier is not None:
             data["pkce_code_verifier"] = pkce_code_verifier
         if session_token is not None:
```

### Comparing `stytch-7.1.0/stytch/b2b/api/sso_oidc.py` & `stytch-7.2.0/stytch/b2b/api/sso_oidc.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/b2b/api/sso_saml.py` & `stytch-7.2.0/stytch/b2b/api/sso_saml.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/b2b/client.py` & `stytch-7.2.0/stytch/b2b/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,8 +41,10 @@
         self.oauth = OAuth(self.api_base, self.sync_client, self.async_client)
         self.otps = OTPs(self.api_base, self.sync_client, self.async_client)
         self.organizations = Organizations(
             self.api_base, self.sync_client, self.async_client
         )
         self.passwords = Passwords(self.api_base, self.sync_client, self.async_client)
         self.sso = SSO(self.api_base, self.sync_client, self.async_client)
-        self.sessions = Sessions(self.api_base, self.sync_client, self.async_client)
+        self.sessions = Sessions(
+            self.api_base, self.sync_client, self.async_client, self.jwks_client
+        )
```

### Comparing `stytch-7.1.0/stytch/b2b/models/discovery_intermediate_sessions.py` & `stytch-7.2.0/stytch/b2b/models/otp_sms.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,30 +10,43 @@
 from typing import Optional
 
 from stytch.b2b.models.organizations import Member, Organization
 from stytch.b2b.models.sessions import MemberSession
 from stytch.core.response_base import ResponseBase
 
 
-class ExchangeRequestLocale(enum.Enum):
+class SendRequestLocale(enum.Enum):
     EN = "en"
     ES = "es"
     PTBR = "pt-br"
 
 
-class ExchangeResponse(ResponseBase):
-    """Response type for `IntermediateSessions.exchange`.
+class AuthenticateResponse(ResponseBase):
+    """Response type for `Sms.authenticate`.
     Fields:
       - member_id: Globally unique UUID that identifies a specific Member.
-      - session_token: A secret token for a given Stytch Session.
-      - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
       - member: The [Member object](https://stytch.com/docs/b2b/api/member-object).
       - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
+      - session_token: A secret token for a given Stytch Session.
+      - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
       - member_session: The [Session object](https://stytch.com/docs/b2b/api/session-object).
     """  # noqa
 
     member_id: str
+    member: Member
+    organization: Organization
     session_token: str
     session_jwt: str
+    member_session: Optional[MemberSession] = None
+
+
+class SendResponse(ResponseBase):
+    """Response type for `Sms.send`.
+    Fields:
+      - member_id: Globally unique UUID that identifies a specific Member.
+      - member: The [Member object](https://stytch.com/docs/b2b/api/member-object).
+      - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
+    """  # noqa
+
+    member_id: str
     member: Member
     organization: Organization
-    member_session: Optional[MemberSession] = None
```

### Comparing `stytch-7.1.0/stytch/b2b/models/discovery_organizations.py` & `stytch-7.2.0/stytch/b2b/models/magic_links_discovery.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,44 +2,27 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
-from typing import List, Optional
+from typing import List
 
 from stytch.b2b.models.discovery import DiscoveredOrganization
-from stytch.b2b.models.organizations import Member, Organization
-from stytch.b2b.models.sessions import MemberSession
 from stytch.core.response_base import ResponseBase
 
 
-class CreateResponse(ResponseBase):
-    """Response type for `Organizations.create`.
-    Fields:
-      - member_id: Globally unique UUID that identifies a specific Member.
-      - session_token: A secret token for a given Stytch Session.
-      - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
-      - member: The [Member object](https://stytch.com/docs/b2b/api/member-object).
-      - member_session: The [Session object](https://stytch.com/docs/b2b/api/session-object).
-      - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
-    """  # noqa
-
-    member_id: str
-    session_token: str
-    session_jwt: str
-    member: Member
-    member_session: Optional[MemberSession] = None
-    organization: Optional[Organization] = None
-
-
-class ListResponse(ResponseBase):
-    """Response type for `Organizations.list`.
+class AuthenticateResponse(ResponseBase):
+    """Response type for `Discovery.authenticate`.
     Fields:
+      - intermediate_session_token: The Intermediate Session Token. This token does not necessarily belong to a specific instance of a Member, but represents a bag of factors that may be converted to a member session.
+        The token can be used with the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete an MFA flow;
+        the [Exchange Intermediate Session endpoint](https://stytch.com/docs/b2b/api/exchange-intermediate-session) to join a specific Organization that allows the factors represented by the intermediate session token;
+        or the [Create Organization via Discovery endpoint](https://stytch.com/docs/b2b/api/create-organization-via-discovery) to create a new Organization and Member.
       - email_address: The email address.
       - discovered_organizations: An array of `discovered_organization` objects tied to the `intermediate_session_token`, `session_token`, or `session_jwt`. See the [Discovered Organization Object](https://stytch.com/docs/b2b/api/discovered-organization-object) for complete details.
 
       Note that Organizations will only appear here under any of the following conditions:
       1. The end user is already a Member of the Organization.
       2. The end user is invited to the Organization.
       3. The end user can join the Organization because:
@@ -47,9 +30,10 @@
           a) The Organization allows JIT provisioning.
 
           b) The Organizations' allowed domains list contains the Member's email domain.
 
           c) The Organization has at least one other Member with a verified email address with the same domain as the end user (to prevent phishing attacks).
     """  # noqa
 
+    intermediate_session_token: str
     email_address: str
     discovered_organizations: List[DiscoveredOrganization]
```

### Comparing `stytch-7.1.0/stytch/b2b/models/magic_links.py` & `stytch-7.2.0/stytch/b2b/models/magic_links.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
 import enum
+from typing import Optional
 
+from stytch.b2b.models.mfa import MfaRequired
 from stytch.b2b.models.organizations import Member, Organization
 from stytch.b2b.models.sessions import MemberSession
 from stytch.core.response_base import ResponseBase
 
 
 class AuthenticateRequestLocale(enum.Enum):
     EN = "en"
@@ -28,18 +30,27 @@
         Stytch's Session product. If you are using Stytch's Session product, we revoke the Member’s other Sessions for you.
       - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
       - member: The [Member object](https://stytch.com/docs/b2b/api/member-object).
       - session_token: A secret token for a given Stytch Session.
       - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
       - member_session: The [Session object](https://stytch.com/docs/b2b/api/session-object).
       - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
+      - intermediate_session_token: The returned Intermediate Session Token contains an Email Magic Link factor associated with the Member's email address.
+          The token can be used with the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete the MFA flow and log in to the Organization.
+          It can also be used with the [Exchange Intermediate Session endpoint](https://stytch.com/docs/b2b/api/exchange-intermediate-session) to join a different existing Organization that allows login with Email Magic Links,
+          or the [Create Organization via Discovery endpoint](https://stytch.com/docs/b2b/api/create-organization-via-discovery) to create a new Organization.
+      - member_authenticated: Indicates whether the Member is fully authenticated. If false, the Member needs to complete an MFA step to log in to the Organization.
+      - mfa_required: (Coming Soon) Information about the MFA requirements of the Organization and the Member's options for fulfilling MFA.
     """  # noqa
 
     member_id: str
     method_id: str
     reset_sessions: bool
     organization_id: str
     member: Member
     session_token: str
     session_jwt: str
     member_session: MemberSession
     organization: Organization
+    intermediate_session_token: str
+    member_authenticated: bool
+    mfa_required: Optional[MfaRequired] = None
```

### Comparing `stytch-7.1.0/stytch/b2b/models/magic_links_email.py` & `stytch-7.2.0/stytch/b2b/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/b2b/models/oauth.py` & `stytch-7.2.0/stytch/consumer/models/oauth.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,69 +3,72 @@
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
 import datetime
-import enum
 from typing import List, Optional
 
 import pydantic
 
-from stytch.b2b.models.organizations import Member, Organization
-from stytch.b2b.models.sessions import MemberSession
+from stytch.consumer.models.sessions import Session
+from stytch.consumer.models.users import User
 from stytch.core.response_base import ResponseBase
 
 
-class AuthenticateRequestLocale(enum.Enum):
-    EN = "en"
-    ES = "es"
-    PTBR = "pt-br"
-
-
 class ProviderValues(pydantic.BaseModel):
     """
     Fields:
       - access_token: The `access_token` that you may use to access the User's data in the provider's API.
-      - scopes: The OAuth scopes included for a given provider. See each provider's section above to see which scopes are included by default and how to add custom scopes.
       - refresh_token: The `refresh_token` that you may use to refresh a User's session within the provider's API.
-      - expires_at: (no documentation yet)
       - id_token: The `id_token` returned by the OAuth provider. ID Tokens are JWTs that contain structured information about a user. The exact content of each ID Token varies from provider to provider. ID Tokens are returned from OAuth providers that conform to the [OpenID Connect](https://openid.net/foundation/) specification, which is based on OAuth.
+      - scopes: The OAuth scopes included for a given provider. See each provider's section above to see which scopes are included by default and how to add custom scopes.
+      - expires_at: The timestamp when the Session expires. Values conform to the RFC 3339 standard and are expressed in UTC, e.g. `2021-12-29T12:33:09Z`.
     """  # noqa
 
     access_token: str
+    refresh_token: str
+    id_token: str
     scopes: List[str]
-    refresh_token: Optional[str] = None
     expires_at: Optional[datetime.datetime] = None
-    id_token: Optional[str] = None
+
+
+class AttachResponse(ResponseBase):
+    """Response type for `OAuth.attach`.
+    Fields:
+      - oauth_attach_token: A single-use token for connecting the Stytch User selection from an OAuth Attach request to the corresponding OAuth Start request.
+    """  # noqa
+
+    oauth_attach_token: str
 
 
 class AuthenticateResponse(ResponseBase):
     """Response type for `OAuth.authenticate`.
     Fields:
-      - member_id: Globally unique UUID that identifies a specific Member.
-      - provider_subject: (no documentation yet)
-      - provider_type: (no documentation yet)
+      - user_id: The unique ID of the affected User.
+      - provider_subject: The unique identifier for the User within a given OAuth provider. Also commonly called the "sub" or "Subject field" in OAuth protocols.
+      - provider_type: Denotes the OAuth identity provider that the user has authenticated with, e.g. Google, Facebook, GitHub etc.
       - session_token: A secret token for a given Stytch Session.
       - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
-      - member: The [Member object](https://stytch.com/docs/b2b/api/member-object).
-      - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
-      - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
-      - reset_sessions: (no documentation yet)
-      - member_session: The [Session object](https://stytch.com/docs/b2b/api/session-object).
       - provider_values: The `provider_values` object lists relevant identifiers, values, and scopes for a given OAuth provider. For example this object will include a provider's `access_token` that you can use to access the provider's API for a given user.
 
-      Note that these values will vary based on the OAuth provider in question, e.g. `id_token` is only returned by Microsoft.
+      Note that these values will vary based on the OAuth provider in question, e.g. `id_token` is only returned by OIDC complaint identity providers.
+      - user: The `user` object affected by this API call. See the [Get user endpoint](https://stytch.com/docs/api/get-user) for complete response field details.
+      - reset_sessions: Indicates if all other of the User's Sessions need to be reset. You should check this field if you aren't using Stytch's Session product. If you are using Stytch's Session product, we revoke the User's other sessions for you.
+      - oauth_user_registration_id: The unique ID for an OAuth registration.
+      - user_session: A `Session` object. For backwards compatibility reasons, the session from an OAuth authenticate call is labeled as `user_session`, but is otherwise just a standard stytch `Session` object.
+
+      See [GET sessions](https://stytch.com/docs/api/session-get) for complete response fields.
+
     """  # noqa
 
-    member_id: str
+    user_id: str
     provider_subject: str
     provider_type: str
     session_token: str
     session_jwt: str
-    member: Member
-    organization_id: str
-    organization: Organization
+    provider_values: ProviderValues
+    user: User
     reset_sessions: bool
-    member_session: Optional[MemberSession] = None
-    provider_values: Optional[ProviderValues] = None
+    oauth_user_registration_id: str
+    user_session: Optional[Session] = None
```

### Comparing `stytch-7.1.0/stytch/b2b/models/organizations.py` & `stytch-7.2.0/stytch/b2b/models/organizations.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,16 +149,16 @@
       - email_address: The email address of the Member.
       - status: The status of the Member. The possible values are: `pending`, `invited`, `active`, or `deleted`.
       - name: The name of the Member.
       - sso_registrations: An array of registered [SAML Connection](saml-connection-object) objects the Member has authenticated with.
       - is_breakglass: Identifies the Member as a break glass user - someone who has permissions to authenticate into an Organization by bypassing the Organization's settings. A break glass account is typically used for emergency purposes to gain access outside of normal authentication procedures. Refer to the [Organization object](organization-object) and its `auth_methods` and `allowed_auth_methods` fields for more details.
       - member_password_id: Globally unique UUID that identifies a Member's password.
       - oauth_registrations: A list of OAuth registrations for this member.
-      - mfa_enrolled: (no documentation yet)
-      - mfa_phone_number: (no documentation yet)
+      - mfa_enrolled: (Coming Soon) Sets whether the Member is enrolled in MFA. If true, the Member must complete an MFA step whenever they wish to log in to their Organization. If false, the Member only needs to complete an MFA step if the Organization's MFA policy is set to `REQUIRED_FOR_ALL`.
+      - mfa_phone_number: (Coming Soon) The Member's phone number. A Member may only have one phone number.
       - trusted_metadata: An arbitrary JSON object for storing application-specific data or identity-provider-specific data.
       - untrusted_metadata: An arbitrary JSON object of application-specific data. These fields can be edited directly by the
       frontend SDK, and should not be used to store critical information. See the [Metadata resource](https://stytch.com/docs/b2b/api/metadata)
       for complete field behavior details.
     """  # noqa
 
     organization_id: str
```

### Comparing `stytch-7.1.0/stytch/b2b/models/organizations_members.py` & `stytch-7.2.0/stytch/b2b/models/organizations_members.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,14 +35,21 @@
 
     member_id: str
     member: Member
     organization: Organization
 
 
 class DeletePhoneNumberResponse(ResponseBase):
+    """Response type for `Members.delete_phone_number`.
+    Fields:
+      - member_id: Globally unique UUID that identifies a specific Member.
+      - member: The [Member object](https://stytch.com/docs/b2b/api/member-object).
+      - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
+    """  # noqa
+
     member_id: str
     member: Member
     organization: Organization
 
 
 class DeleteResponse(ResponseBase):
     """Response type for `Members.delete`.
```

### Comparing `stytch-7.1.0/stytch/b2b/models/otp_sms.py` & `stytch-7.2.0/stytch/b2b/models/passwords_session.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,34 +2,27 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
-import enum
 from typing import Optional
 
 from stytch.b2b.models.organizations import Member, Organization
 from stytch.b2b.models.sessions import MemberSession
 from stytch.core.response_base import ResponseBase
 
 
-class SendRequestLocale(enum.Enum):
-    EN = "en"
-    ES = "es"
-    PTBR = "pt-br"
+class ResetResponse(ResponseBase):
+    """Response type for `Sessions.reset`.
+    Fields:
+      - member_id: Globally unique UUID that identifies a specific Member.
+      - member: The [Member object](https://stytch.com/docs/b2b/api/member-object).
+      - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
+      - member_session: The [Session object](https://stytch.com/docs/b2b/api/session-object).
+    """  # noqa
 
-
-class AuthenticateResponse(ResponseBase):
     member_id: str
     member: Member
     organization: Organization
-    session_token: str
-    session_jwt: str
     member_session: Optional[MemberSession] = None
-
-
-class SendResponse(ResponseBase):
-    member_id: str
-    member: Member
-    organization: Organization
```

### Comparing `stytch-7.1.0/stytch/b2b/models/passwords.py` & `stytch-7.2.0/stytch/b2b/models/passwords.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from __future__ import annotations
 
 import enum
 from typing import List, Optional
 
 import pydantic
 
+from stytch.b2b.models.mfa import MfaRequired
 from stytch.b2b.models.organizations import Member, Organization
 from stytch.b2b.models.sessions import MemberSession
 from stytch.core.response_base import ResponseBase
 
 
 class AuthenticateRequestLocale(enum.Enum):
     EN = "en"
@@ -70,24 +71,32 @@
     Fields:
       - member_id: Globally unique UUID that identifies a specific Member.
       - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
       - member: The [Member object](https://stytch.com/docs/b2b/api/member-object).
       - session_token: A secret token for a given Stytch Session.
       - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
       - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
+      - intermediate_session_token: The returned Intermediate Session Token contains a password factor associated with the Member.
+          The token can be used with the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete the MFA flow and log in to the Organization.
+          Password factors are not transferable between Organizations, so the intermediate session token is not valid for use with discovery endpoints.
+      - member_authenticated: Indicates whether the Member is fully authenticated. If false, the Member needs to complete an MFA step to log in to the Organization.
       - member_session: The [Session object](https://stytch.com/docs/b2b/api/session-object).
+      - mfa_required: (Coming Soon) Information about the MFA requirements of the Organization and the Member's options for fulfilling MFA.
     """  # noqa
 
     member_id: str
     organization_id: str
     member: Member
     session_token: str
     session_jwt: str
     organization: Organization
+    intermediate_session_token: str
+    member_authenticated: bool
     member_session: Optional[MemberSession] = None
+    mfa_required: Optional[MfaRequired] = None
 
 
 class MigrateResponse(ResponseBase):
     """Response type for `Passwords.migrate`.
     Fields:
       - member_id: Globally unique UUID that identifies a specific Member.
       - member_created: A flag indicating `true` if a new Member object was created and `false` if the Member object already existed.
```

### Comparing `stytch-7.1.0/stytch/b2b/models/sessions.py` & `stytch-7.2.0/stytch/b2b/models/sessions.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
 import datetime
 import enum
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Optional
 
 import pydantic
 
+from stytch.b2b.models.mfa import MfaRequired
 from stytch.b2b.models.organizations import Member, Organization
 from stytch.consumer.models.sessions import JWK, AuthenticationFactor
 from stytch.core.response_base import ResponseBase
 
 
 class ExchangeRequestLocale(enum.Enum):
     EN = "en"
@@ -68,22 +69,31 @@
     Fields:
       - member_id: Globally unique UUID that identifies a specific Member.
       - member_session: The [Session object](https://stytch.com/docs/b2b/api/session-object).
       - session_token: A secret token for a given Stytch Session.
       - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
       - member: The [Member object](https://stytch.com/docs/b2b/api/member-object).
       - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
+      - member_authenticated: Indicates whether the Member is fully authenticated. If false, the Member needs to complete an MFA step to log in to the Organization.
+      - intermediate_session_token: The returned Intermediate Session Token contains any Email Magic Link or OAuth factors from the original member session that are valid for the target Organization.
+          The token can be used with the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete the MFA flow and log in to the target Organization.
+          It can also be used with the [Exchange Intermediate Session endpoint](https://stytch.com/docs/b2b/api/exchange-intermediate-session) to join a different existing Organization,
+          or the [Create Organization via Discovery endpoint](https://stytch.com/docs/b2b/api/create-organization-via-discovery) to create a new Organization.
+      - mfa_required: (Coming Soon) Information about the MFA requirements of the Organization and the Member's options for fulfilling MFA.
     """  # noqa
 
     member_id: str
     member_session: MemberSession
     session_token: str
     session_jwt: str
     member: Member
     organization: Organization
+    member_authenticated: bool
+    intermediate_session_token: str
+    mfa_required: Optional[MfaRequired] = None
 
 
 class GetJWKSResponse(ResponseBase):
     """Response type for `Sessions.get_jwks`.
     Fields:
       - keys: The JWK
     """  # noqa
```

### Comparing `stytch-7.1.0/stytch/b2b/models/sso.py` & `stytch-7.2.0/stytch/b2b/models/sso.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import datetime
 import enum
 from typing import Any, Dict, List, Optional
 
 import pydantic
 
+from stytch.b2b.models.mfa import MfaRequired
 from stytch.b2b.models.organizations import Member, Organization
 from stytch.b2b.models.sessions import MemberSession
 from stytch.core.response_base import ResponseBase
 
 
 class AuthenticateRequestLocale(enum.Enum):
     EN = "en"
@@ -67,25 +68,33 @@
       - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
       - member: The [Member object](https://stytch.com/docs/b2b/api/member-object).
       - session_token: A secret token for a given Stytch Session.
       - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
       - reset_session: Indicates if all Sessions linked to the Member need to be reset. You should check this field if you aren't using
         Stytch's Session product. If you are using Stytch's Session product, we revoke the Member’s other Sessions for you.
       - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
+      - intermediate_session_token: The returned Intermediate Session Token contains an SSO factor associated with the Member.
+          The token can be used with the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete the MFA flow and log in to the Organization.
+          SSO factors are not transferable between Organizations, so the intermediate session token is not valid for use with discovery endpoints.
+      - member_authenticated: Indicates whether the Member is fully authenticated. If false, the Member needs to complete an MFA step to log in to the Organization.
       - member_session: The [Session object](https://stytch.com/docs/b2b/api/session-object).
+      - mfa_required: (Coming Soon) Information about the MFA requirements of the Organization and the Member's options for fulfilling MFA.
     """  # noqa
 
     member_id: str
     organization_id: str
     member: Member
     session_token: str
     session_jwt: str
     reset_session: bool
     organization: Organization
+    intermediate_session_token: str
+    member_authenticated: bool
     member_session: Optional[MemberSession] = None
+    mfa_required: Optional[MfaRequired] = None
 
 
 class DeleteConnectionResponse(ResponseBase):
     """Response type for `SSO.delete_connection`.
     Fields:
       - connection_id: The `connection_id` that was deleted as part of the delete request.
     """  # noqa
```

### Comparing `stytch-7.1.0/stytch/b2b/models/sso_oidc.py` & `stytch-7.2.0/stytch/b2b/models/sso_oidc.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/b2b/models/sso_saml.py` & `stytch-7.2.0/stytch/b2b/models/sso_saml.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/consumer/api/crypto_wallets.py` & `stytch-7.2.0/stytch/consumer/api/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/consumer/api/magic_links.py` & `stytch-7.2.0/stytch/consumer/api/oauth.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,195 +4,182 @@
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
 from typing import Any, Dict, Optional
 
-from stytch.consumer.api.magic_links_email import Email
-from stytch.consumer.models.attribute import Attributes
-from stytch.consumer.models.magic_links import (
-    AuthenticateResponse,
-    CreateResponse,
-    Options,
-)
+from stytch.consumer.models.oauth import AttachResponse, AuthenticateResponse
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
-class MagicLinks:
+class OAuth:
     def __init__(
         self,
         api_base: ApiBase,
         sync_client: SyncClient,
         async_client: AsyncClient,
     ) -> None:
         self.api_base = api_base
         self.sync_client = sync_client
         self.async_client = async_client
-        self.email = Email(api_base, sync_client, async_client)
+
+    def attach(
+        self,
+        provider: str,
+        user_id: Optional[str] = None,
+        session_token: Optional[str] = None,
+        session_jwt: Optional[str] = None,
+    ) -> AttachResponse:
+        """Generate an OAuth Attach Token to pre-associate an OAuth flow with an existing Stytch User. Pass the returned `oauth_attach_token` to the same provider's OAuth Start endpoint to treat this OAuth flow as a login for that user instead of a signup for a new user.
+
+        Exactly one of `user_id`, `session_token`, or `session_jwt` must be provided to identify the target Stytch User.
+
+        This is an optional step in the OAuth flow. Stytch can often determine whether to create a new user or log in an existing one based on verified identity provider information. This endpoint is useful for cases where we can't, such as missing or unverified provider information.
+
+        Fields:
+          - provider: The OAuth provider's name.
+          - user_id: The unique ID of a specific User.
+          - session_token: The `session_token` associated with a User's existing Session.
+          - session_jwt: The `session_jwt` associated with a User's existing Session.
+        """  # noqa
+        data: Dict[str, Any] = {
+            "provider": provider,
+        }
+        if user_id is not None:
+            data["user_id"] = user_id
+        if session_token is not None:
+            data["session_token"] = session_token
+        if session_jwt is not None:
+            data["session_jwt"] = session_jwt
+
+        url = self.api_base.url_for("/v1/oauth/attach", data)
+        res = self.sync_client.post(url, data)
+        return AttachResponse.from_json(res.response.status_code, res.json)
+
+    async def attach_async(
+        self,
+        provider: str,
+        user_id: Optional[str] = None,
+        session_token: Optional[str] = None,
+        session_jwt: Optional[str] = None,
+    ) -> AttachResponse:
+        """Generate an OAuth Attach Token to pre-associate an OAuth flow with an existing Stytch User. Pass the returned `oauth_attach_token` to the same provider's OAuth Start endpoint to treat this OAuth flow as a login for that user instead of a signup for a new user.
+
+        Exactly one of `user_id`, `session_token`, or `session_jwt` must be provided to identify the target Stytch User.
+
+        This is an optional step in the OAuth flow. Stytch can often determine whether to create a new user or log in an existing one based on verified identity provider information. This endpoint is useful for cases where we can't, such as missing or unverified provider information.
+
+        Fields:
+          - provider: The OAuth provider's name.
+          - user_id: The unique ID of a specific User.
+          - session_token: The `session_token` associated with a User's existing Session.
+          - session_jwt: The `session_jwt` associated with a User's existing Session.
+        """  # noqa
+        data: Dict[str, Any] = {
+            "provider": provider,
+        }
+        if user_id is not None:
+            data["user_id"] = user_id
+        if session_token is not None:
+            data["session_token"] = session_token
+        if session_jwt is not None:
+            data["session_jwt"] = session_jwt
+
+        url = self.api_base.url_for("/v1/oauth/attach", data)
+        res = await self.async_client.post(url, data)
+        return AttachResponse.from_json(res.response.status, res.json)
 
     def authenticate(
         self,
         token: str,
-        attributes: Optional[Attributes] = None,
-        options: Optional[Options] = None,
         session_token: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
         code_verifier: Optional[str] = None,
     ) -> AuthenticateResponse:
-        """Authenticate a User given a Magic Link. This endpoint verifies that the Magic Link token is valid, hasn't expired or been previously used, and any optional security settings such as IP match or user agent match are satisfied.
+        """Authenticate a User given a `token`. This endpoint verifies that the user completed the OAuth flow by verifying that the token is valid and hasn't expired. To initiate a Stytch session for the user while authenticating their OAuth token, include `session_duration_minutes`; a session with the identity provider, e.g. Google or Facebook, will always be initiated upon successful authentication.
 
         Fields:
           - token: The token to authenticate.
-          - attributes: Provided attributes help with fraud detection.
-          - options: Specify optional security settings.
-          - session_token: The `session_token` associated with a User's existing Session.
+          - session_token: Reuse an existing session instead of creating a new one. If you provide us with a `session_token`, then we'll update the session represented by this session token with this OAuth factor. If this `session_token` belongs to a different user than the OAuth token, the session_jwt will be ignored. This endpoint will error if both `session_token` and `session_jwt` are provided.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
           five minutes regardless of the underlying session duration, and will need to be refreshed over time.
 
           This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
 
           If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
 
           If the `session_duration_minutes` parameter is not specified, a Stytch session will not be created.
-          - session_jwt: The `session_jwt` associated with a User's existing Session.
+          - session_jwt: Reuse an existing session instead of creating a new one. If you provide us with a `session_jwt`, then we'll update the session represented by this JWT with this OAuth factor. If this `session_jwt` belongs to a different user than the OAuth token, the session_jwt will be ignored. This endpoint will error if both `session_token` and `session_jwt` are provided.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value.
 
           Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes.
           - code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
         """  # noqa
         data: Dict[str, Any] = {
             "token": token,
         }
-        if attributes is not None:
-            data["attributes"] = attributes.dict()
-        if options is not None:
-            data["options"] = options.dict()
         if session_token is not None:
             data["session_token"] = session_token
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
         if code_verifier is not None:
             data["code_verifier"] = code_verifier
 
-        url = self.api_base.url_for("/v1/magic_links/authenticate", data)
+        url = self.api_base.url_for("/v1/oauth/authenticate", data)
         res = self.sync_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status_code, res.json)
 
     async def authenticate_async(
         self,
         token: str,
-        attributes: Optional[Attributes] = None,
-        options: Optional[Options] = None,
         session_token: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
         code_verifier: Optional[str] = None,
     ) -> AuthenticateResponse:
-        """Authenticate a User given a Magic Link. This endpoint verifies that the Magic Link token is valid, hasn't expired or been previously used, and any optional security settings such as IP match or user agent match are satisfied.
+        """Authenticate a User given a `token`. This endpoint verifies that the user completed the OAuth flow by verifying that the token is valid and hasn't expired. To initiate a Stytch session for the user while authenticating their OAuth token, include `session_duration_minutes`; a session with the identity provider, e.g. Google or Facebook, will always be initiated upon successful authentication.
 
         Fields:
           - token: The token to authenticate.
-          - attributes: Provided attributes help with fraud detection.
-          - options: Specify optional security settings.
-          - session_token: The `session_token` associated with a User's existing Session.
+          - session_token: Reuse an existing session instead of creating a new one. If you provide us with a `session_token`, then we'll update the session represented by this session token with this OAuth factor. If this `session_token` belongs to a different user than the OAuth token, the session_jwt will be ignored. This endpoint will error if both `session_token` and `session_jwt` are provided.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
           five minutes regardless of the underlying session duration, and will need to be refreshed over time.
 
           This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
 
           If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
 
           If the `session_duration_minutes` parameter is not specified, a Stytch session will not be created.
-          - session_jwt: The `session_jwt` associated with a User's existing Session.
+          - session_jwt: Reuse an existing session instead of creating a new one. If you provide us with a `session_jwt`, then we'll update the session represented by this JWT with this OAuth factor. If this `session_jwt` belongs to a different user than the OAuth token, the session_jwt will be ignored. This endpoint will error if both `session_token` and `session_jwt` are provided.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value.
 
           Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes.
           - code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
         """  # noqa
         data: Dict[str, Any] = {
             "token": token,
         }
-        if attributes is not None:
-            data["attributes"] = attributes.dict()
-        if options is not None:
-            data["options"] = options.dict()
         if session_token is not None:
             data["session_token"] = session_token
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
         if code_verifier is not None:
             data["code_verifier"] = code_verifier
 
-        url = self.api_base.url_for("/v1/magic_links/authenticate", data)
+        url = self.api_base.url_for("/v1/oauth/authenticate", data)
         res = await self.async_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status, res.json)
-
-    def create(
-        self,
-        user_id: str,
-        expiration_minutes: Optional[int] = None,
-        attributes: Optional[Attributes] = None,
-    ) -> CreateResponse:
-        """Create an embeddable Magic Link token for a User. Access to this endpoint is restricted. To enable it, please send us a note at support@stytch.com.
-
-        ### Next steps
-        Send the returned `token` value to the end user in a link which directs to your application. When the end user follows your link, collect the token, and call [Authenticate Magic Link](https://stytch.com/docs/api/authenticate-magic-link) to complete authentication.
-
-        Fields:
-          - user_id: The unique ID of a specific User.
-          - expiration_minutes: Set the expiration for the Magic Link `token` in minutes. By default, it expires in 1 hour. The minimum expiration is 5 minutes and the maximum is 7 days (10080 mins).
-          - attributes: Provided attributes help with fraud detection.
-        """  # noqa
-        data: Dict[str, Any] = {
-            "user_id": user_id,
-        }
-        if expiration_minutes is not None:
-            data["expiration_minutes"] = expiration_minutes
-        if attributes is not None:
-            data["attributes"] = attributes.dict()
-
-        url = self.api_base.url_for("/v1/magic_links", data)
-        res = self.sync_client.post(url, data)
-        return CreateResponse.from_json(res.response.status_code, res.json)
-
-    async def create_async(
-        self,
-        user_id: str,
-        expiration_minutes: Optional[int] = None,
-        attributes: Optional[Attributes] = None,
-    ) -> CreateResponse:
-        """Create an embeddable Magic Link token for a User. Access to this endpoint is restricted. To enable it, please send us a note at support@stytch.com.
-
-        ### Next steps
-        Send the returned `token` value to the end user in a link which directs to your application. When the end user follows your link, collect the token, and call [Authenticate Magic Link](https://stytch.com/docs/api/authenticate-magic-link) to complete authentication.
-
-        Fields:
-          - user_id: The unique ID of a specific User.
-          - expiration_minutes: Set the expiration for the Magic Link `token` in minutes. By default, it expires in 1 hour. The minimum expiration is 5 minutes and the maximum is 7 days (10080 mins).
-          - attributes: Provided attributes help with fraud detection.
-        """  # noqa
-        data: Dict[str, Any] = {
-            "user_id": user_id,
-        }
-        if expiration_minutes is not None:
-            data["expiration_minutes"] = expiration_minutes
-        if attributes is not None:
-            data["attributes"] = attributes.dict()
-
-        url = self.api_base.url_for("/v1/magic_links", data)
-        res = await self.async_client.post(url, data)
-        return CreateResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-7.1.0/stytch/consumer/api/magic_links_email.py` & `stytch-7.2.0/stytch/consumer/api/magic_links_email.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
         ### Add an email to an existing user
         This endpoint also allows you to add a new email to an existing Stytch User. Including a `user_id`, `session_token`, or `session_jwt` in the request will add the email to the pre-existing Stytch User upon successful authentication.
 
         Adding a new email to an existing Stytch User requires the user to be present and validate the email via magic link. This requirement is in place to prevent account takeover attacks.
 
         ### Next steps
-        The user is emailed a magic link which redirects them to the provided [redirect URL](https://stytch.com/docs/magic-links#email-magic-links_redirect-routing). Collect the `token` from the URL query parameters, and call [Authenticate magic link](https://stytch.com/docs/api/authenticate-magic-link) to complete authentication.
+        The user is emailed a magic link which redirects them to the provided [redirect URL](https://stytch.com/docs/guides/magic-links/email-magic-links/redirect-routing). Collect the `token` from the URL query parameters, and call [Authenticate magic link](https://stytch.com/docs/api/authenticate-magic-link) to complete authentication.
 
         Fields:
           - email: The email address of the User to send the Magic Link to.
           - login_template_id: Use a custom template for login emails. By default, it will use your default email template. The template must be a template using our built-in customizations or a custom HTML email for Magic links - Login.
           - attributes: Provided attributes help with fraud detection.
           - login_magic_link_url: The URL the end user clicks from the login Email Magic Link. This should be a URL that your app receives and parses and subsequently send an API request to authenticate the Magic Link and log in the User. If this value is not passed, the default login redirect URL that you set in your Dashboard is used. If you have not set a default login redirect URL, an error is returned.
           - signup_magic_link_url: The URL the end user clicks from the sign-up Email Magic Link. This should be a URL that your app receives and parses and subsequently send an API request to authenticate the Magic Link and sign-up the User. If this value is not passed, the default sign-up redirect URL that you set in your Dashboard is used. If you have not set a default sign-up redirect URL, an error is returned.
@@ -132,15 +132,15 @@
 
         ### Add an email to an existing user
         This endpoint also allows you to add a new email to an existing Stytch User. Including a `user_id`, `session_token`, or `session_jwt` in the request will add the email to the pre-existing Stytch User upon successful authentication.
 
         Adding a new email to an existing Stytch User requires the user to be present and validate the email via magic link. This requirement is in place to prevent account takeover attacks.
 
         ### Next steps
-        The user is emailed a magic link which redirects them to the provided [redirect URL](https://stytch.com/docs/magic-links#email-magic-links_redirect-routing). Collect the `token` from the URL query parameters, and call [Authenticate magic link](https://stytch.com/docs/api/authenticate-magic-link) to complete authentication.
+        The user is emailed a magic link which redirects them to the provided [redirect URL](https://stytch.com/docs/guides/magic-links/email-magic-links/redirect-routing). Collect the `token` from the URL query parameters, and call [Authenticate magic link](https://stytch.com/docs/api/authenticate-magic-link) to complete authentication.
 
         Fields:
           - email: The email address of the User to send the Magic Link to.
           - login_template_id: Use a custom template for login emails. By default, it will use your default email template. The template must be a template using our built-in customizations or a custom HTML email for Magic links - Login.
           - attributes: Provided attributes help with fraud detection.
           - login_magic_link_url: The URL the end user clicks from the login Email Magic Link. This should be a URL that your app receives and parses and subsequently send an API request to authenticate the Magic Link and log in the User. If this value is not passed, the default login redirect URL that you set in your Dashboard is used. If you have not set a default login redirect URL, an error is returned.
           - signup_magic_link_url: The URL the end user clicks from the sign-up Email Magic Link. This should be a URL that your app receives and parses and subsequently send an API request to authenticate the Magic Link and sign-up the User. If this value is not passed, the default sign-up redirect URL that you set in your Dashboard is used. If you have not set a default sign-up redirect URL, an error is returned.
```

### Comparing `stytch-7.1.0/stytch/consumer/api/oauth.py` & `stytch-7.2.0/stytch/b2b/api/magic_links.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,182 +4,173 @@
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
 from typing import Any, Dict, Optional
 
-from stytch.consumer.models.oauth import AttachResponse, AuthenticateResponse
+from stytch.b2b.api.magic_links_discovery import Discovery
+from stytch.b2b.api.magic_links_email import Email
+from stytch.b2b.models.magic_links import (
+    AuthenticateRequestLocale,
+    AuthenticateResponse,
+)
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
-class OAuth:
+class MagicLinks:
     def __init__(
         self,
         api_base: ApiBase,
         sync_client: SyncClient,
         async_client: AsyncClient,
     ) -> None:
         self.api_base = api_base
         self.sync_client = sync_client
         self.async_client = async_client
-
-    def attach(
-        self,
-        provider: str,
-        user_id: Optional[str] = None,
-        session_token: Optional[str] = None,
-        session_jwt: Optional[str] = None,
-    ) -> AttachResponse:
-        """Generate an OAuth Attach Token to pre-associate an OAuth flow with an existing Stytch User. Pass the returned `oauth_attach_token` to the same provider's OAuth Start endpoint to treat this OAuth flow as a login for that user instead of a signup for a new user.
-
-        Exactly one of `user_id`, `session_token`, or `session_jwt` must be provided to identify the target Stytch User.
-
-        This is an optional step in the OAuth flow. Stytch can often determine whether to create a new user or log in an existing one based on verified identity provider information. This endpoint is useful for cases where we can't, such as missing or unverified provider information.
-
-        Fields:
-          - provider: The OAuth provider's name.
-          - user_id: The unique ID of a specific User.
-          - session_token: The `session_token` associated with a User's existing Session.
-          - session_jwt: The `session_jwt` associated with a User's existing Session.
-        """  # noqa
-        data: Dict[str, Any] = {
-            "provider": provider,
-        }
-        if user_id is not None:
-            data["user_id"] = user_id
-        if session_token is not None:
-            data["session_token"] = session_token
-        if session_jwt is not None:
-            data["session_jwt"] = session_jwt
-
-        url = self.api_base.url_for("/v1/oauth/attach", data)
-        res = self.sync_client.post(url, data)
-        return AttachResponse.from_json(res.response.status_code, res.json)
-
-    async def attach_async(
-        self,
-        provider: str,
-        user_id: Optional[str] = None,
-        session_token: Optional[str] = None,
-        session_jwt: Optional[str] = None,
-    ) -> AttachResponse:
-        """Generate an OAuth Attach Token to pre-associate an OAuth flow with an existing Stytch User. Pass the returned `oauth_attach_token` to the same provider's OAuth Start endpoint to treat this OAuth flow as a login for that user instead of a signup for a new user.
-
-        Exactly one of `user_id`, `session_token`, or `session_jwt` must be provided to identify the target Stytch User.
-
-        This is an optional step in the OAuth flow. Stytch can often determine whether to create a new user or log in an existing one based on verified identity provider information. This endpoint is useful for cases where we can't, such as missing or unverified provider information.
-
-        Fields:
-          - provider: The OAuth provider's name.
-          - user_id: The unique ID of a specific User.
-          - session_token: The `session_token` associated with a User's existing Session.
-          - session_jwt: The `session_jwt` associated with a User's existing Session.
-        """  # noqa
-        data: Dict[str, Any] = {
-            "provider": provider,
-        }
-        if user_id is not None:
-            data["user_id"] = user_id
-        if session_token is not None:
-            data["session_token"] = session_token
-        if session_jwt is not None:
-            data["session_jwt"] = session_jwt
-
-        url = self.api_base.url_for("/v1/oauth/attach", data)
-        res = await self.async_client.post(url, data)
-        return AttachResponse.from_json(res.response.status, res.json)
+        self.email = Email(api_base, sync_client, async_client)
+        self.discovery = Discovery(api_base, sync_client, async_client)
 
     def authenticate(
         self,
-        token: str,
+        magic_links_token: str,
+        pkce_code_verifier: Optional[str] = None,
         session_token: Optional[str] = None,
-        session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
+        session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
-        code_verifier: Optional[str] = None,
+        locale: Optional[AuthenticateRequestLocale] = None,
     ) -> AuthenticateResponse:
-        """Authenticate a User given a `token`. This endpoint verifies that the user completed the OAuth flow by verifying that the token is valid and hasn't expired. To initiate a Stytch session for the user while authenticating their OAuth token, include `session_duration_minutes`; a session with the identity provider, e.g. Google or Facebook, will always be initiated upon successful authentication.
+        """Authenticate a Member with a Magic Link. This endpoint requires a Magic Link token that is not expired or previously used. If the Member’s status is `pending` or `invited`, they will be updated to `active`.
+        Provide the `session_duration_minutes` parameter to set the lifetime of the session. If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration.
+
+        (Coming Soon) If the Member is required to complete MFA to log in to the Organization, the returned value of `member_authenticated` will be `false`, and an `intermediate_session_token` will be returned.
+        The `intermediate_session_token` can be passed into the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete the MFA step and acquire a full member session.
+        The `intermediate_session_token` can also be used with the [Exchange Intermediate Session endpoint](https://stytch.com/docs/b2b/api/exchange-intermediate-session) or the [Create Organization via Discovery endpoint](https://stytch.com/docs/b2b/api/create-organization-via-discovery) to join a different Organization or create a new one.
+        The `session_duration_minutes` and `session_custom_claims` parameters will be ignored.
+
+        If a valid `session_token` or `session_jwt` is passed in, the Member will not be required to complete an MFA step.
 
         Fields:
-          - token: The token to authenticate.
-          - session_token: Reuse an existing session instead of creating a new one. If you provide us with a `session_token`, then we'll update the session represented by this session token with this OAuth factor. If this `session_token` belongs to a different user than the OAuth token, the session_jwt will be ignored. This endpoint will error if both `session_token` and `session_jwt` are provided.
+          - magic_links_token: The Email Magic Link token to authenticate.
+          - pkce_code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
+          - session_token: Reuse an existing session instead of creating a new one. If you provide a `session_token`, Stytch will update the session.
+              If the `session_token` and `magic_links_token` belong to different Members, the `session_token` will be ignored. This endpoint will error if
+              both `session_token` and `session_jwt` are provided.
+          - session_jwt: Reuse an existing session instead of creating a new one. If you provide a `session_jwt`, Stytch will update the session. If the `session_jwt`
+              and `magic_links_token` belong to different Members, the `session_jwt` will be ignored. This endpoint will error if both `session_token` and `session_jwt`
+              are provided.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
           five minutes regardless of the underlying session duration, and will need to be refreshed over time.
 
           This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
 
           If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
 
-          If the `session_duration_minutes` parameter is not specified, a Stytch session will not be created.
-          - session_jwt: Reuse an existing session instead of creating a new one. If you provide us with a `session_jwt`, then we'll update the session represented by this JWT with this OAuth factor. If this `session_jwt` belongs to a different user than the OAuth token, the session_jwt will be ignored. This endpoint will error if both `session_token` and `session_jwt` are provided.
-          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value.
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
+          to use the Stytch session product, you can ignore the session fields in the response.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
+          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
+          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
+          Total custom claims size cannot exceed four kilobytes.
+          - locale: (Coming Soon) If the Member needs to complete an MFA step, and the Member has a phone number, this endpoint will pre-emptively send a one-time passcode (OTP) to the Member's phone number. The locale argument will be used to determine which language to use when sending the passcode.
+
+        Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
+
+        Currently supported languages are English (`"en"`), Spanish (`"es"`), and Brazilian Portuguese (`"pt-br"`); if no value is provided, the copy defaults to English.
+
+        Request support for additional languages [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link")!
 
-          Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes.
-          - code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
         """  # noqa
         data: Dict[str, Any] = {
-            "token": token,
+            "magic_links_token": magic_links_token,
         }
+        if pkce_code_verifier is not None:
+            data["pkce_code_verifier"] = pkce_code_verifier
         if session_token is not None:
             data["session_token"] = session_token
-        if session_duration_minutes is not None:
-            data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
+        if session_duration_minutes is not None:
+            data["session_duration_minutes"] = session_duration_minutes
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
-        if code_verifier is not None:
-            data["code_verifier"] = code_verifier
+        if locale is not None:
+            data["locale"] = locale.value
 
-        url = self.api_base.url_for("/v1/oauth/authenticate", data)
+        url = self.api_base.url_for("/v1/b2b/magic_links/authenticate", data)
         res = self.sync_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status_code, res.json)
 
     async def authenticate_async(
         self,
-        token: str,
+        magic_links_token: str,
+        pkce_code_verifier: Optional[str] = None,
         session_token: Optional[str] = None,
-        session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
+        session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
-        code_verifier: Optional[str] = None,
+        locale: Optional[AuthenticateRequestLocale] = None,
     ) -> AuthenticateResponse:
-        """Authenticate a User given a `token`. This endpoint verifies that the user completed the OAuth flow by verifying that the token is valid and hasn't expired. To initiate a Stytch session for the user while authenticating their OAuth token, include `session_duration_minutes`; a session with the identity provider, e.g. Google or Facebook, will always be initiated upon successful authentication.
+        """Authenticate a Member with a Magic Link. This endpoint requires a Magic Link token that is not expired or previously used. If the Member’s status is `pending` or `invited`, they will be updated to `active`.
+        Provide the `session_duration_minutes` parameter to set the lifetime of the session. If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration.
+
+        (Coming Soon) If the Member is required to complete MFA to log in to the Organization, the returned value of `member_authenticated` will be `false`, and an `intermediate_session_token` will be returned.
+        The `intermediate_session_token` can be passed into the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete the MFA step and acquire a full member session.
+        The `intermediate_session_token` can also be used with the [Exchange Intermediate Session endpoint](https://stytch.com/docs/b2b/api/exchange-intermediate-session) or the [Create Organization via Discovery endpoint](https://stytch.com/docs/b2b/api/create-organization-via-discovery) to join a different Organization or create a new one.
+        The `session_duration_minutes` and `session_custom_claims` parameters will be ignored.
+
+        If a valid `session_token` or `session_jwt` is passed in, the Member will not be required to complete an MFA step.
 
         Fields:
-          - token: The token to authenticate.
-          - session_token: Reuse an existing session instead of creating a new one. If you provide us with a `session_token`, then we'll update the session represented by this session token with this OAuth factor. If this `session_token` belongs to a different user than the OAuth token, the session_jwt will be ignored. This endpoint will error if both `session_token` and `session_jwt` are provided.
+          - magic_links_token: The Email Magic Link token to authenticate.
+          - pkce_code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
+          - session_token: Reuse an existing session instead of creating a new one. If you provide a `session_token`, Stytch will update the session.
+              If the `session_token` and `magic_links_token` belong to different Members, the `session_token` will be ignored. This endpoint will error if
+              both `session_token` and `session_jwt` are provided.
+          - session_jwt: Reuse an existing session instead of creating a new one. If you provide a `session_jwt`, Stytch will update the session. If the `session_jwt`
+              and `magic_links_token` belong to different Members, the `session_jwt` will be ignored. This endpoint will error if both `session_token` and `session_jwt`
+              are provided.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
           returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
           five minutes regardless of the underlying session duration, and will need to be refreshed over time.
 
           This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
 
           If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
 
-          If the `session_duration_minutes` parameter is not specified, a Stytch session will not be created.
-          - session_jwt: Reuse an existing session instead of creating a new one. If you provide us with a `session_jwt`, then we'll update the session represented by this JWT with this OAuth factor. If this `session_jwt` belongs to a different user than the OAuth token, the session_jwt will be ignored. This endpoint will error if both `session_token` and `session_jwt` are provided.
-          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value.
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
+          to use the Stytch session product, you can ignore the session fields in the response.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
+          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
+          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
+          Total custom claims size cannot exceed four kilobytes.
+          - locale: (Coming Soon) If the Member needs to complete an MFA step, and the Member has a phone number, this endpoint will pre-emptively send a one-time passcode (OTP) to the Member's phone number. The locale argument will be used to determine which language to use when sending the passcode.
+
+        Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
+
+        Currently supported languages are English (`"en"`), Spanish (`"es"`), and Brazilian Portuguese (`"pt-br"`); if no value is provided, the copy defaults to English.
+
+        Request support for additional languages [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link")!
 
-          Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes.
-          - code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
         """  # noqa
         data: Dict[str, Any] = {
-            "token": token,
+            "magic_links_token": magic_links_token,
         }
+        if pkce_code_verifier is not None:
+            data["pkce_code_verifier"] = pkce_code_verifier
         if session_token is not None:
             data["session_token"] = session_token
-        if session_duration_minutes is not None:
-            data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
+        if session_duration_minutes is not None:
+            data["session_duration_minutes"] = session_duration_minutes
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
-        if code_verifier is not None:
-            data["code_verifier"] = code_verifier
+        if locale is not None:
+            data["locale"] = locale.value
 
-        url = self.api_base.url_for("/v1/oauth/authenticate", data)
+        url = self.api_base.url_for("/v1/b2b/magic_links/authenticate", data)
         res = await self.async_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status, res.json)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stytch-7.1.0/stytch/consumer/api/otp_email.py` & `stytch-7.2.0/stytch/consumer/api/otp_email.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         Adding a new email to an existing Stytch User requires the User to be present and validate the email via OTP. This requirement is in place to prevent account takeover attacks.
 
         ### Next steps
         Collect the OTP which was delivered to the user. Call [Authenticate OTP](https://stytch.com/docs/api/authenticate-otp) using the OTP `code` along with the `phone_id` found in the response as the `method_id`.
 
         Fields:
           - email: The email address of the user to send the one-time passcode to. You may use sandbox@stytch.com to test this endpoint, see [Testing](https://stytch.com/docs/home#resources_testing) for more detail.
-          - expiration_minutes: Set the expiration for the Magic Link `token` in minutes. By default, it expires in 1 hour. The minimum expiration is 5 minutes and the maximum is 7 days (10080 mins).
+          - expiration_minutes: Set the expiration for the one-time passcode, in minutes. The minimum expiration is 1 minute and the maximum is 10 minutes. The default expiration is 2 minutes.
           - attributes: Provided attributes help with fraud detection.
           - locale: Used to determine which language to use when sending the user this delivery method. Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
 
         Currently supported languages are English (`"en"`), Spanish (`"es"`), and Brazilian Portuguese (`"pt-br"`); if no value is provided, the copy defaults to English.
 
         Request support for additional languages [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link")!
 
@@ -112,15 +112,15 @@
         Adding a new email to an existing Stytch User requires the User to be present and validate the email via OTP. This requirement is in place to prevent account takeover attacks.
 
         ### Next steps
         Collect the OTP which was delivered to the user. Call [Authenticate OTP](https://stytch.com/docs/api/authenticate-otp) using the OTP `code` along with the `phone_id` found in the response as the `method_id`.
 
         Fields:
           - email: The email address of the user to send the one-time passcode to. You may use sandbox@stytch.com to test this endpoint, see [Testing](https://stytch.com/docs/home#resources_testing) for more detail.
-          - expiration_minutes: Set the expiration for the Magic Link `token` in minutes. By default, it expires in 1 hour. The minimum expiration is 5 minutes and the maximum is 7 days (10080 mins).
+          - expiration_minutes: Set the expiration for the one-time passcode, in minutes. The minimum expiration is 1 minute and the maximum is 10 minutes. The default expiration is 2 minutes.
           - attributes: Provided attributes help with fraud detection.
           - locale: Used to determine which language to use when sending the user this delivery method. Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
 
         Currently supported languages are English (`"en"`), Spanish (`"es"`), and Brazilian Portuguese (`"pt-br"`); if no value is provided, the copy defaults to English.
 
         Request support for additional languages [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link")!
 
@@ -168,15 +168,15 @@
 
         ### Next steps
 
         Collect the OTP which was delivered to the User. Call [Authenticate OTP](https://stytch.com/docs/api/authenticate-otp) using the OTP `code` along with the `phone_id` found in the response as the `method_id`.
 
         Fields:
           - email: The email address of the user to send the one-time passcode to. You may use sandbox@stytch.com to test this endpoint, see [Testing](https://stytch.com/docs/home#resources_testing) for more detail.
-          - expiration_minutes: Set the expiration for the Magic Link `token` in minutes. By default, it expires in 1 hour. The minimum expiration is 5 minutes and the maximum is 7 days (10080 mins).
+          - expiration_minutes: Set the expiration for the one-time passcode, in minutes. The minimum expiration is 1 minute and the maximum is 10 minutes. The default expiration is 2 minutes.
           - attributes: Provided attributes help with fraud detection.
           - create_user_as_pending: Flag for whether or not to save a user as pending vs active in Stytch. Defaults to false.
                 If true, users will be saved with status pending in Stytch's backend until authenticated.
                 If false, users will be created as active. An example usage of
                 a true flag would be to require users to verify their phone by entering the OTP code before creating
                 an account for them.
           - locale: Used to determine which language to use when sending the user this delivery method. Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
@@ -222,15 +222,15 @@
 
         ### Next steps
 
         Collect the OTP which was delivered to the User. Call [Authenticate OTP](https://stytch.com/docs/api/authenticate-otp) using the OTP `code` along with the `phone_id` found in the response as the `method_id`.
 
         Fields:
           - email: The email address of the user to send the one-time passcode to. You may use sandbox@stytch.com to test this endpoint, see [Testing](https://stytch.com/docs/home#resources_testing) for more detail.
-          - expiration_minutes: Set the expiration for the Magic Link `token` in minutes. By default, it expires in 1 hour. The minimum expiration is 5 minutes and the maximum is 7 days (10080 mins).
+          - expiration_minutes: Set the expiration for the one-time passcode, in minutes. The minimum expiration is 1 minute and the maximum is 10 minutes. The default expiration is 2 minutes.
           - attributes: Provided attributes help with fraud detection.
           - create_user_as_pending: Flag for whether or not to save a user as pending vs active in Stytch. Defaults to false.
                 If true, users will be saved with status pending in Stytch's backend until authenticated.
                 If false, users will be created as active. An example usage of
                 a true flag would be to require users to verify their phone by entering the OTP code before creating
                 an account for them.
           - locale: Used to determine which language to use when sending the user this delivery method. Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
```

### Comparing `stytch-7.1.0/stytch/consumer/api/otp_sms.py` & `stytch-7.2.0/stytch/consumer/api/otp_sms.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
         ### Next steps
 
         Collect the OTP which was delivered to the user. Call [Authenticate OTP](https://stytch.com/docs/api/authenticate-otp) using the OTP `code` along with the `phone_id` found in the response as the `method_id`.
 
         Fields:
           - phone_number: The phone number to use for one-time passcodes. The phone number should be in E.164 format. The phone number should be in E.164 format (i.e. +1XXXXXXXXXX). You may use +10000000000 to test this endpoint, see [Testing](https://stytch.com/docs/home#resources_testing) for more detail.
-          - expiration_minutes: Set the expiration for the Magic Link `token` in minutes. By default, it expires in 1 hour. The minimum expiration is 5 minutes and the maximum is 7 days (10080 mins).
+          - expiration_minutes: Set the expiration for the one-time passcode, in minutes. The minimum expiration is 1 minute and the maximum is 10 minutes. The default expiration is 2 minutes.
           - attributes: Provided attributes help with fraud detection.
           - locale: Used to determine which language to use when sending the user this delivery method. Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
 
         Currently supported languages are English (`"en"`), Spanish (`"es"`), and Brazilian Portuguese (`"pt-br"`); if no value is provided, the copy defaults to English.
 
         Request support for additional languages [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link")!
 
@@ -110,15 +110,15 @@
 
         ### Next steps
 
         Collect the OTP which was delivered to the user. Call [Authenticate OTP](https://stytch.com/docs/api/authenticate-otp) using the OTP `code` along with the `phone_id` found in the response as the `method_id`.
 
         Fields:
           - phone_number: The phone number to use for one-time passcodes. The phone number should be in E.164 format. The phone number should be in E.164 format (i.e. +1XXXXXXXXXX). You may use +10000000000 to test this endpoint, see [Testing](https://stytch.com/docs/home#resources_testing) for more detail.
-          - expiration_minutes: Set the expiration for the Magic Link `token` in minutes. By default, it expires in 1 hour. The minimum expiration is 5 minutes and the maximum is 7 days (10080 mins).
+          - expiration_minutes: Set the expiration for the one-time passcode, in minutes. The minimum expiration is 1 minute and the maximum is 10 minutes. The default expiration is 2 minutes.
           - attributes: Provided attributes help with fraud detection.
           - locale: Used to determine which language to use when sending the user this delivery method. Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
 
         Currently supported languages are English (`"en"`), Spanish (`"es"`), and Brazilian Portuguese (`"pt-br"`); if no value is provided, the copy defaults to English.
 
         Request support for additional languages [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link")!
 
@@ -158,15 +158,15 @@
 
         ### Next steps
 
         Collect the OTP which was delivered to the User. Call [Authenticate OTP](https://stytch.com/docs/api/authenticate-otp) using the OTP `code` along with the `phone_id` found in the response as the `method_id`.
 
         Fields:
           - phone_number: The phone number to use for one-time passcodes. The phone number should be in E.164 format. The phone number should be in E.164 format (i.e. +1XXXXXXXXXX). You may use +10000000000 to test this endpoint, see [Testing](https://stytch.com/docs/home#resources_testing) for more detail.
-          - expiration_minutes: Set the expiration for the Magic Link `token` in minutes. By default, it expires in 1 hour. The minimum expiration is 5 minutes and the maximum is 7 days (10080 mins).
+          - expiration_minutes: Set the expiration for the one-time passcode, in minutes. The minimum expiration is 1 minute and the maximum is 10 minutes. The default expiration is 2 minutes.
           - attributes: Provided attributes help with fraud detection.
           - create_user_as_pending: Flag for whether or not to save a user as pending vs active in Stytch. Defaults to false.
                 If true, users will be saved with status pending in Stytch's backend until authenticated.
                 If false, users will be created as active. An example usage of
                 a true flag would be to require users to verify their phone by entering the OTP code before creating
                 an account for them.
           - locale: Used to determine which language to use when sending the user this delivery method. Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
@@ -204,15 +204,15 @@
 
         ### Next steps
 
         Collect the OTP which was delivered to the User. Call [Authenticate OTP](https://stytch.com/docs/api/authenticate-otp) using the OTP `code` along with the `phone_id` found in the response as the `method_id`.
 
         Fields:
           - phone_number: The phone number to use for one-time passcodes. The phone number should be in E.164 format. The phone number should be in E.164 format (i.e. +1XXXXXXXXXX). You may use +10000000000 to test this endpoint, see [Testing](https://stytch.com/docs/home#resources_testing) for more detail.
-          - expiration_minutes: Set the expiration for the Magic Link `token` in minutes. By default, it expires in 1 hour. The minimum expiration is 5 minutes and the maximum is 7 days (10080 mins).
+          - expiration_minutes: Set the expiration for the one-time passcode, in minutes. The minimum expiration is 1 minute and the maximum is 10 minutes. The default expiration is 2 minutes.
           - attributes: Provided attributes help with fraud detection.
           - create_user_as_pending: Flag for whether or not to save a user as pending vs active in Stytch. Defaults to false.
                 If true, users will be saved with status pending in Stytch's backend until authenticated.
                 If false, users will be created as active. An example usage of
                 a true flag would be to require users to verify their phone by entering the OTP code before creating
                 an account for them.
           - locale: Used to determine which language to use when sending the user this delivery method. Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
```

### Comparing `stytch-7.1.0/stytch/consumer/api/otp_whatsapp.py` & `stytch-7.2.0/stytch/consumer/api/otp_whatsapp.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
         ### Next steps
 
         Collect the OTP which was delivered to the user. Call [Authenticate OTP](https://stytch.com/docs/api/authenticate-otp) using the OTP `code` along with the `phone_id` found in the response as the `method_id`.
 
         Fields:
           - phone_number: The phone number to use for one-time passcodes. The phone number should be in E.164 format. The phone number should be in E.164 format (i.e. +1XXXXXXXXXX). You may use +10000000000 to test this endpoint, see [Testing](https://stytch.com/docs/home#resources_testing) for more detail.
-          - expiration_minutes: Set the expiration for the Magic Link `token` in minutes. By default, it expires in 1 hour. The minimum expiration is 5 minutes and the maximum is 7 days (10080 mins).
+          - expiration_minutes: Set the expiration for the one-time passcode, in minutes. The minimum expiration is 1 minute and the maximum is 10 minutes. The default expiration is 2 minutes.
           - attributes: Provided attributes help with fraud detection.
           - locale: Used to determine which language to use when sending the user this delivery method. Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
 
         Currently supported languages are English (`"en"`), Spanish (`"es"`), and Brazilian Portuguese (`"pt-br"`); if no value is provided, the copy defaults to English.
 
         Request support for additional languages [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link")!
 
@@ -110,15 +110,15 @@
 
         ### Next steps
 
         Collect the OTP which was delivered to the user. Call [Authenticate OTP](https://stytch.com/docs/api/authenticate-otp) using the OTP `code` along with the `phone_id` found in the response as the `method_id`.
 
         Fields:
           - phone_number: The phone number to use for one-time passcodes. The phone number should be in E.164 format. The phone number should be in E.164 format (i.e. +1XXXXXXXXXX). You may use +10000000000 to test this endpoint, see [Testing](https://stytch.com/docs/home#resources_testing) for more detail.
-          - expiration_minutes: Set the expiration for the Magic Link `token` in minutes. By default, it expires in 1 hour. The minimum expiration is 5 minutes and the maximum is 7 days (10080 mins).
+          - expiration_minutes: Set the expiration for the one-time passcode, in minutes. The minimum expiration is 1 minute and the maximum is 10 minutes. The default expiration is 2 minutes.
           - attributes: Provided attributes help with fraud detection.
           - locale: Used to determine which language to use when sending the user this delivery method. Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
 
         Currently supported languages are English (`"en"`), Spanish (`"es"`), and Brazilian Portuguese (`"pt-br"`); if no value is provided, the copy defaults to English.
 
         Request support for additional languages [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link")!
 
@@ -158,15 +158,15 @@
 
         ### Next steps
 
         Collect the OTP which was delivered to the User. Call [Authenticate OTP](https://stytch.com/docs/api/authenticate-otp) using the OTP `code` along with the `phone_id` found in the response as the `method_id`.
 
         Fields:
           - phone_number: The phone number to use for one-time passcodes. The phone number should be in E.164 format. The phone number should be in E.164 format (i.e. +1XXXXXXXXXX). You may use +10000000000 to test this endpoint, see [Testing](https://stytch.com/docs/home#resources_testing) for more detail.
-          - expiration_minutes: Set the expiration for the Magic Link `token` in minutes. By default, it expires in 1 hour. The minimum expiration is 5 minutes and the maximum is 7 days (10080 mins).
+          - expiration_minutes: Set the expiration for the one-time passcode, in minutes. The minimum expiration is 1 minute and the maximum is 10 minutes. The default expiration is 2 minutes.
           - attributes: Provided attributes help with fraud detection.
           - create_user_as_pending: Flag for whether or not to save a user as pending vs active in Stytch. Defaults to false.
                 If true, users will be saved with status pending in Stytch's backend until authenticated.
                 If false, users will be created as active. An example usage of
                 a true flag would be to require users to verify their phone by entering the OTP code before creating
                 an account for them.
           - locale: Used to determine which language to use when sending the user this delivery method. Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
@@ -204,15 +204,15 @@
 
         ### Next steps
 
         Collect the OTP which was delivered to the User. Call [Authenticate OTP](https://stytch.com/docs/api/authenticate-otp) using the OTP `code` along with the `phone_id` found in the response as the `method_id`.
 
         Fields:
           - phone_number: The phone number to use for one-time passcodes. The phone number should be in E.164 format. The phone number should be in E.164 format (i.e. +1XXXXXXXXXX). You may use +10000000000 to test this endpoint, see [Testing](https://stytch.com/docs/home#resources_testing) for more detail.
-          - expiration_minutes: Set the expiration for the Magic Link `token` in minutes. By default, it expires in 1 hour. The minimum expiration is 5 minutes and the maximum is 7 days (10080 mins).
+          - expiration_minutes: Set the expiration for the one-time passcode, in minutes. The minimum expiration is 1 minute and the maximum is 10 minutes. The default expiration is 2 minutes.
           - attributes: Provided attributes help with fraud detection.
           - create_user_as_pending: Flag for whether or not to save a user as pending vs active in Stytch. Defaults to false.
                 If true, users will be saved with status pending in Stytch's backend until authenticated.
                 If false, users will be created as active. An example usage of
                 a true flag would be to require users to verify their phone by entering the OTP code before creating
                 an account for them.
           - locale: Used to determine which language to use when sending the user this delivery method. Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
```

### Comparing `stytch-7.1.0/stytch/consumer/api/passwords.py` & `stytch-7.2.0/stytch/consumer/api/passwords.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,15 @@
     def strength_check(
         self,
         password: str,
         email: Optional[str] = None,
     ) -> StrengthCheckResponse:
         """This API allows you to check whether or not the user’s provided password is valid, and to provide feedback to the user on how to increase the strength of their password.
 
-        This endpoint adapts to your Project's password strength configuration. If you're using [zxcvbn](https://stytch.com/docs/passwords#strength-requirements), the default, your passwords are considered valid if the strength score is >= 3. If you're using [LUDS](https://stytch.com/docs/passwords#strength-requirements), your passwords are considered valid if they meet the requirements that you've set with Stytch. You may update your password strength configuration in the [stytch dashboard](https://stytch.com/dashboard/password-strength-config).
+        This endpoint adapts to your Project's password strength configuration. If you're using [zxcvbn](https://stytch.com/docs/guides/passwords/strength-policy), the default, your passwords are considered valid if the strength score is >= 3. If you're using [LUDS](https://stytch.com/docs/guides/passwords/strength-policy), your passwords are considered valid if they meet the requirements that you've set with Stytch. You may update your password strength configuration in the [stytch dashboard](https://stytch.com/dashboard/password-strength-config).
 
 
         ### Password feedback
 
         The `feedback` object contains relevant fields for you to relay feedback to users that failed to create a strong enough password.
 
         If you're using zxcvbn, the `feedback` object will contain `warning` and `suggestions` for any password that does not meet the zxcvbn strength requirements. You can return these strings directly to the user to help them craft a strong password.
@@ -289,15 +289,15 @@
     async def strength_check_async(
         self,
         password: str,
         email: Optional[str] = None,
     ) -> StrengthCheckResponse:
         """This API allows you to check whether or not the user’s provided password is valid, and to provide feedback to the user on how to increase the strength of their password.
 
-        This endpoint adapts to your Project's password strength configuration. If you're using [zxcvbn](https://stytch.com/docs/passwords#strength-requirements), the default, your passwords are considered valid if the strength score is >= 3. If you're using [LUDS](https://stytch.com/docs/passwords#strength-requirements), your passwords are considered valid if they meet the requirements that you've set with Stytch. You may update your password strength configuration in the [stytch dashboard](https://stytch.com/dashboard/password-strength-config).
+        This endpoint adapts to your Project's password strength configuration. If you're using [zxcvbn](https://stytch.com/docs/guides/passwords/strength-policy), the default, your passwords are considered valid if the strength score is >= 3. If you're using [LUDS](https://stytch.com/docs/guides/passwords/strength-policy), your passwords are considered valid if they meet the requirements that you've set with Stytch. You may update your password strength configuration in the [stytch dashboard](https://stytch.com/dashboard/password-strength-config).
 
 
         ### Password feedback
 
         The `feedback` object contains relevant fields for you to relay feedback to users that failed to create a strong enough password.
 
         If you're using zxcvbn, the `feedback` object will contain `warning` and `suggestions` for any password that does not meet the zxcvbn strength requirements. You can return these strings directly to the user to help them craft a strong password.
```

### Comparing `stytch-7.1.0/stytch/consumer/api/passwords_email.py` & `stytch-7.2.0/stytch/consumer/api/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/consumer/api/passwords_session.py` & `stytch-7.2.0/stytch/consumer/api/passwords_session.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     def reset(
         self,
         password: str,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
     ) -> ResetResponse:
-        """Reset the user’s password using their existing session. The endpoint will error if the session does not have a password, email magic link, or email OTP authentication factor that has been issued within the last 5 minutes.
+        """Reset the user’s password using their existing session. The endpoint will error if the session does not have a password, email magic link, or email OTP authentication factor that has been issued within the last 5 minutes. This endpoint requires either a `session_jwt` or `session_token` be included in the request.
 
         Fields:
           - password: The password of the user
           - session_token: The `session_token` associated with a User's existing Session.
           - session_jwt: The `session_jwt` associated with a User's existing Session.
         """  # noqa
         data: Dict[str, Any] = {
@@ -51,15 +51,15 @@
 
     async def reset_async(
         self,
         password: str,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
     ) -> ResetResponse:
-        """Reset the user’s password using their existing session. The endpoint will error if the session does not have a password, email magic link, or email OTP authentication factor that has been issued within the last 5 minutes.
+        """Reset the user’s password using their existing session. The endpoint will error if the session does not have a password, email magic link, or email OTP authentication factor that has been issued within the last 5 minutes. This endpoint requires either a `session_jwt` or `session_token` be included in the request.
 
         Fields:
           - password: The password of the user
           - session_token: The `session_token` associated with a User's existing Session.
           - session_jwt: The `session_jwt` associated with a User's existing Session.
         """  # noqa
         data: Dict[str, Any] = {
```

### Comparing `stytch-7.1.0/stytch/consumer/api/sessions.py` & `stytch-7.2.0/stytch/consumer/api/sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 
 class Sessions:
     def __init__(
         self,
         api_base: ApiBase,
         sync_client: SyncClient,
         async_client: AsyncClient,
+        jwks_client: jwt.PyJWKClient,
     ) -> None:
         self.api_base = api_base
         self.sync_client = sync_client
         self.async_client = async_client
+        self.jwks_client = jwks_client
 
     def get(
         self,
         user_id: str,
     ) -> GetResponse:
         """List all active Sessions for a given `user_id`. All timestamps are formatted according to the RFC 3339 standard and are expressed in UTC, e.g. `2021-12-29T12:33:09Z`.
 
@@ -270,22 +272,16 @@
                 )
             ).session
         )
 
     # ENDMANUAL(authenticate_jwt)
 
     # MANUAL(authenticate_jwt_local)(SERVICE_METHOD)
-    # ADDIMPORT: import jwt
     # ADDIMPORT: import time
     # ADDIMPORT: from stytch.consumer.models.sessions import Session
-    def get_jwks_client(self) -> jwt.PyJWKClient:
-        data = {"project_id": self.sync_client.project_id}
-        jwks_url = self.api_base.url_for("v1/sessions/jwks/{project_id}", data)
-        return jwt.PyJWKClient(jwks_url)
-
     def authenticate_jwt_local(
         self,
         session_jwt: str,
         max_token_age_seconds: Optional[int] = None,
         leeway: int = 0,
     ) -> Optional[Session]:
         """Parse a JWT and verify the signature locally
@@ -301,18 +297,17 @@
         comparing timestamps. It defaults to zero.
         """
         project_id = self.sync_client.project_id
         jwt_audience = project_id
         jwt_issuer = "stytch.com/{}".format(project_id)
         _session_claim = "https://stytch.com/session"
 
-        jwks_client = self.get_jwks_client()
         now = time.time()
 
-        signing_key = jwks_client.get_signing_key_from_jwt(session_jwt)
+        signing_key = self.jwks_client.get_signing_key_from_jwt(session_jwt)
 
         # NOTE: The max_token_age_seconds value is applied after decoding.
         payload = jwt.decode(
             session_jwt,
             signing_key.key,
             algorithms=["RS256"],
             options={
@@ -337,19 +332,32 @@
 
         # Unpack the session claim to match the detached session format.
         claim = payload[_session_claim]
 
         # For JWTs that include it, prefer the inner expires_at claim.
         expires_at = claim.get("expires_at", payload["exp"])
 
+        # Parse custom claims by taking everything other than the reserved claims
+        reserved_claims = [
+            "aud",
+            "exp",
+            "iat",
+            "iss",
+            "jti",
+            "nbf",
+            "sub",
+            _session_claim,
+        ]
+        custom_claims = {k: v for k, v in payload.items() if k not in reserved_claims}
+
         return Session(
             attributes=claim["attributes"],
             authentication_factors=claim["authentication_factors"],
             expires_at=expires_at,
             last_accessed_at=claim["last_accessed_at"],
             session_id=claim["id"],
             started_at=claim["started_at"],
             user_id=payload["sub"],
-            custom_claims=None,
+            custom_claims=custom_claims,
         )
 
     # ENDMANUAL(authenticate_jwt_local)
```

### Comparing `stytch-7.1.0/stytch/consumer/api/users.py` & `stytch-7.2.0/stytch/consumer/api/users.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/consumer/api/webauthn.py` & `stytch-7.2.0/stytch/consumer/api/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/consumer/client.py` & `stytch-7.2.0/stytch/consumer/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,11 +40,13 @@
         )
         self.magic_links = MagicLinks(
             self.api_base, self.sync_client, self.async_client
         )
         self.oauth = OAuth(self.api_base, self.sync_client, self.async_client)
         self.otps = OTPs(self.api_base, self.sync_client, self.async_client)
         self.passwords = Passwords(self.api_base, self.sync_client, self.async_client)
-        self.sessions = Sessions(self.api_base, self.sync_client, self.async_client)
+        self.sessions = Sessions(
+            self.api_base, self.sync_client, self.async_client, self.jwks_client
+        )
         self.totps = TOTPs(self.api_base, self.sync_client, self.async_client)
         self.users = Users(self.api_base, self.sync_client, self.async_client)
         self.webauthn = WebAuthn(self.api_base, self.sync_client, self.async_client)
```

### Comparing `stytch-7.1.0/stytch/consumer/models/crypto_wallets.py` & `stytch-7.2.0/stytch/consumer/models/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/consumer/models/magic_links.py` & `stytch-7.2.0/stytch/consumer/models/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/consumer/models/magic_links_email.py` & `stytch-7.2.0/stytch/consumer/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/consumer/models/otp.py` & `stytch-7.2.0/stytch/consumer/models/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/consumer/models/otp_email.py` & `stytch-7.2.0/stytch/consumer/models/otp_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/consumer/models/otp_sms.py` & `stytch-7.2.0/stytch/consumer/models/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/consumer/models/otp_whatsapp.py` & `stytch-7.2.0/stytch/consumer/models/otp_whatsapp.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/consumer/models/passwords.py` & `stytch-7.2.0/stytch/consumer/models/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/consumer/models/passwords_email.py` & `stytch-7.2.0/stytch/consumer/models/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/consumer/models/passwords_existing_password.py` & `stytch-7.2.0/stytch/consumer/models/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/consumer/models/passwords_session.py` & `stytch-7.2.0/stytch/consumer/models/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/consumer/models/sessions.py` & `stytch-7.2.0/stytch/consumer/models/sessions.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,27 +333,27 @@
     attributes: Optional[Attributes] = None
     custom_claims: Optional[Dict[str, Any]] = None
 
 
 class AuthenticateResponse(ResponseBase):
     """Response type for `Sessions.authenticate`.
     Fields:
-      - session_token: A secret token for a given Stytch Session.
-      - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
-      - user: The `user` object affected by this API call. See the [Get user endpoint](https://stytch.com/docs/api/get-user) for complete response field details.
       - session: If you initiate a Session, by including `session_duration_minutes` in your authenticate call, you'll receive a full Session object in the response.
 
       See [GET sessions](https://stytch.com/docs/api/session-get) for complete response fields.
 
+      - session_token: A secret token for a given Stytch Session.
+      - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
+      - user: The `user` object affected by this API call. See the [Get user endpoint](https://stytch.com/docs/api/get-user) for complete response field details.
     """  # noqa
 
+    session: Session
     session_token: str
     session_jwt: str
     user: User
-    session: Optional[Session] = None
 
 
 class GetJWKSResponse(ResponseBase):
     """Response type for `Sessions.get_jwks`.
     Fields:
       - keys: The JWK
     """  # noqa
```

### Comparing `stytch-7.1.0/stytch/consumer/models/totps.py` & `stytch-7.2.0/stytch/consumer/models/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/consumer/models/users.py` & `stytch-7.2.0/stytch/consumer/models/users.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/consumer/models/webauthn.py` & `stytch-7.2.0/stytch/consumer/models/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/core/api_base.py` & `stytch-7.2.0/stytch/core/api_base.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/core/client_base.py` & `stytch-7.2.0/stytch/core/client_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import warnings
 from typing import Optional
 
+import jwt
+
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
 class ClientBase:
     def __init__(
         self,
@@ -13,14 +15,20 @@
         environment: Optional[str] = None,
         suppress_warnings: bool = False,
     ):
         base_url = self._env_url(project_id, environment, suppress_warnings)
         self.api_base = ApiBase(base_url)
         self.sync_client = SyncClient(project_id, secret)
         self.async_client = AsyncClient(project_id, secret)
+        self.jwks_client = self.get_jwks_client(project_id)
+
+    def get_jwks_client(self, project_id: str) -> jwt.PyJWKClient:
+        data = {"project_id": project_id}
+        url = self.api_base.url_for("/v1/b2b/sessions/jwks/{project_id}", data)
+        return jwt.PyJWKClient(url)
 
     @classmethod
     def _env_url(
         cls, project_id: str, env: Optional[str], suppress_warnings: bool = False
     ) -> str:
         """Resolve the base URL for the Stytch API environment."""
         if env is None:
```

### Comparing `stytch-7.1.0/stytch/core/http/client.py` & `stytch-7.2.0/stytch/core/http/client.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch/core/response_base.py` & `stytch-7.2.0/stytch/core/response_base.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/stytch.egg-info/PKG-INFO` & `stytch-7.2.0/stytch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 7.1.0
+Version: 7.2.0
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
@@ -36,27 +36,26 @@
 pip install stytch
 ```
 
 ## Usage
 
 You can find your API credentials in the [Stytch Dashboard](https://stytch.com/dashboard/api-keys).
 
-This client library supports all of Stytch's live products:
-
-- [x] [Email Magic Links](https://stytch.com/docs/api/send-by-email)
-- [x] [Embeddable Magic Links](https://stytch.com/docs/api/create-magic-link-overview)
-- [x] [OAuth logins](https://stytch.com/docs/api/oauth-overview)
-- [x] [SMS passcodes](https://stytch.com/docs/api/send-otp-by-sms)
-- [x] [WhatsApp passcodes](https://stytch.com/docs/api/whatsapp-send)
-- [x] [Email passcodes](https://stytch.com/docs/api/send-otp-by-email)
-- [x] [Session Management](https://stytch.com/docs/api/sessions-overview)
-- [x] [WebAuthn](https://stytch.com/docs/api/webauthn-overview)
-- [x] [Time-based one-time passcodes (TOTPs)](https://stytch.com/docs/api/totps-overview)
-- [x] [Crypto wallets](https://stytch.com/docs/api/crypto-wallet-overview)
-- [x] [Passwords](https://stytch.com/docs/api/password-overview)
+This client library supports all Stytch's live products:
+  - [x] [Email Magic Links](https://stytch.com/docs/api/send-by-email)
+  - [x] [Embeddable Magic Links](https://stytch.com/docs/guides/magic-links/embeddable-magic-links/api)
+  - [x] [OAuth logins](https://stytch.com/docs/guides/oauth/idp-overview)
+  - [x] [SMS passcodes](https://stytch.com/docs/api/send-otp-by-sms)
+  - [x] [WhatsApp passcodes](https://stytch.com/docs/api/whatsapp-send)
+  - [x] [Email passcodes](https://stytch.com/docs/api/send-otp-by-email)
+  - [x] [Session Management](https://stytch.com/docs/guides/sessions/using-sessions)
+  - [x] [WebAuthn](https://stytch.com/docs/guides/webauthn/api)
+  - [x] [Time-based one-time passcodes (TOTPs)](https://stytch.com/docs/guides/totp/api)
+  - [x] [Crypto wallets](https://stytch.com/docs/guides/web3/api)
+  - [x] [Passwords](https://stytch.com/docs/guides/passwords/api)
 
 ### Example usage
 
 Create an API client:
 
 ```python
 import stytch
@@ -138,15 +137,15 @@
 
 ## Support
 
 If you've found a bug, [open an issue](https://github.com/stytchauth/stytch-python/issues/new)!
 
 If you have questions or want help troubleshooting, join us in [Slack](https://join.slack.com/t/stytch/shared_invite/zt-nil4wo92-jApJ9Cl32cJbEd9esKkvyg) or email support@stytch.com.
 
-If you've found a security vulnerability, please follow our [responsible disclosure instructions](https://stytch.com/docs/security).
+If you've found a security vulnerability, please follow our [responsible disclosure instructions](https://stytch.com/docs/resources/security-and-trust/security#:~:text=Responsible%20disclosure%20program).
 
 ## Development
 
 See DEVELOPMENT.md
 
 ## Code of Conduct
```

### Comparing `stytch-7.1.0/stytch.egg-info/SOURCES.txt` & `stytch-7.2.0/stytch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/test/test_integration.py` & `stytch-7.2.0/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `stytch-7.1.0/test/test_integration_async.py` & `stytch-7.2.0/test/test_integration_async.py`

 * *Files identical despite different names*

