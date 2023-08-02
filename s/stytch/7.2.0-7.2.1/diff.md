# Comparing `tmp/stytch-7.2.0.tar.gz` & `tmp/stytch-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stytch-7.2.0.tar", last modified: Wed Aug  2 17:15:26 2023, max compression
+gzip compressed data, was "stytch-7.2.1.tar", last modified: Wed Aug  2 21:08:39 2023, max compression
```

## Comparing `stytch-7.2.0.tar` & `stytch-7.2.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.468517 stytch-7.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-02 17:15:10.000000 stytch-7.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-08-02 17:15:26.468517 stytch-7.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-08-02 17:15:10.000000 stytch-7.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-02 17:15:26.468517 stytch-7.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-08-02 17:15:10.000000 stytch-7.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.456517 stytch-7.2.0/stytch/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.456517 stytch-7.2.0/stytch/b2b/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.460517 stytch-7.2.0/stytch/b2b/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    11794 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/discovery_intermediate_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)    26657 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/discovery_organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/magic_links_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/magic_links_email_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/oauth_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    33911 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)    27586 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/organizations_members.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/otp.py
--rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)    25401 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)    21718 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    29703 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/sso.py
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/sso_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/api/sso_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.460517 stytch-7.2.0/stytch/b2b/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/discovery_intermediate_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/discovery_organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/magic_links_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/magic_links_email_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/mfa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/oauth_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/organizations_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/sso.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/sso_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/b2b/models/sso_saml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.460517 stytch-7.2.0/stytch/consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.464517 stytch-7.2.0/stytch/consumer/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    32424 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/otp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    14101 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)    28095 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15027 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/totps.py
--rw-r--r--   0 runner    (1001) docker     (123)    28332 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/users.py
--rw-r--r--   0 runner    (1001) docker     (123)    17303 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/api/webauthn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.464517 stytch-7.2.0/stytch/consumer/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/otp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/totps.py
--rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/consumer/models/webauthn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.464517 stytch-7.2.0/stytch/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/core/api_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/core/client_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.464517 stytch-7.2.0/stytch/core/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/core/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/core/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/core/response_base.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 17:15:10.000000 stytch-7.2.0/stytch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.456517 stytch-7.2.0/stytch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-08-02 17:15:26.000000 stytch-7.2.0/stytch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-08-02 17:15:26.000000 stytch-7.2.0/stytch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:15:26.000000 stytch-7.2.0/stytch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 17:15:26.000000 stytch-7.2.0/stytch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 17:15:26.000000 stytch-7.2.0/stytch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:15:26.468517 stytch-7.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-08-02 17:15:10.000000 stytch-7.2.0/test/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-08-02 17:15:10.000000 stytch-7.2.0/test/test_integration_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:08:39.311711 stytch-7.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-02 21:08:20.000000 stytch-7.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-08-02 21:08:39.311711 stytch-7.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-08-02 21:08:20.000000 stytch-7.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-02 21:08:39.311711 stytch-7.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-08-02 21:08:20.000000 stytch-7.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:08:39.299710 stytch-7.2.1/stytch/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:08:39.299710 stytch-7.2.1/stytch/b2b/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:08:39.303710 stytch-7.2.1/stytch/b2b/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11794 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26657 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/oauth_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33911 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27586 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/organizations_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25401 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21718 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29703 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/sso.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/sso_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/api/sso_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:08:39.307711 stytch-7.2.1/stytch/b2b/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/oauth_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/organizations_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/sso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/sso_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/b2b/models/sso_saml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:08:39.307711 stytch-7.2.1/stytch/consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:08:39.307711 stytch-7.2.1/stytch/consumer/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/api/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32424 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/api/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/api/otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/api/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14101 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/api/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/api/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28095 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15027 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/api/totps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28332 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/api/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17303 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/api/webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:08:39.311711 stytch-7.2.1/stytch/consumer/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/models/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/models/otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/models/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/models/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/models/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/models/totps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/consumer/models/webauthn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:08:39.311711 stytch-7.2.1/stytch/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/core/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/core/client_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:08:39.311711 stytch-7.2.1/stytch/core/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/core/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/core/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/core/response_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 21:08:20.000000 stytch-7.2.1/stytch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:08:39.299710 stytch-7.2.1/stytch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-08-02 21:08:39.000000 stytch-7.2.1/stytch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-08-02 21:08:39.000000 stytch-7.2.1/stytch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:08:39.000000 stytch-7.2.1/stytch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 21:08:39.000000 stytch-7.2.1/stytch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 21:08:39.000000 stytch-7.2.1/stytch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:08:39.311711 stytch-7.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-08-02 21:08:20.000000 stytch-7.2.1/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-08-02 21:08:20.000000 stytch-7.2.1/test/test_integration_async.py
```

### Comparing `stytch-7.2.0/LICENSE.txt` & `stytch-7.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/PKG-INFO` & `stytch-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 7.2.0
+Version: 7.2.1
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-7.2.0/README.md` & `stytch-7.2.1/README.md`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/setup.py` & `stytch-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/discovery.py` & `stytch-7.2.1/stytch/b2b/api/discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/discovery_intermediate_sessions.py` & `stytch-7.2.1/stytch/b2b/api/discovery_intermediate_sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/discovery_organizations.py` & `stytch-7.2.1/stytch/b2b/api/discovery_organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/magic_links.py` & `stytch-7.2.1/stytch/b2b/api/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/magic_links_discovery.py` & `stytch-7.2.1/stytch/b2b/api/magic_links_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/magic_links_email.py` & `stytch-7.2.1/stytch/b2b/api/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/magic_links_email_discovery.py` & `stytch-7.2.1/stytch/b2b/api/magic_links_email_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/oauth.py` & `stytch-7.2.1/stytch/b2b/api/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/oauth_discovery.py` & `stytch-7.2.1/stytch/b2b/api/oauth_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/organizations.py` & `stytch-7.2.1/stytch/b2b/api/organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/organizations_members.py` & `stytch-7.2.1/stytch/b2b/api/organizations_members.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/otp.py` & `stytch-7.2.1/stytch/b2b/api/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/otp_sms.py` & `stytch-7.2.1/stytch/b2b/api/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/passwords.py` & `stytch-7.2.1/stytch/b2b/api/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/passwords_email.py` & `stytch-7.2.1/stytch/b2b/api/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/passwords_existing_password.py` & `stytch-7.2.1/stytch/b2b/api/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/passwords_session.py` & `stytch-7.2.1/stytch/b2b/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/sessions.py` & `stytch-7.2.1/stytch/b2b/api/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/sso.py` & `stytch-7.2.1/stytch/b2b/api/sso.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/sso_oidc.py` & `stytch-7.2.1/stytch/b2b/api/sso_oidc.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/api/sso_saml.py` & `stytch-7.2.1/stytch/b2b/api/sso_saml.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/client.py` & `stytch-7.2.1/stytch/b2b/client.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/models/discovery.py` & `stytch-7.2.1/stytch/b2b/models/discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/models/discovery_intermediate_sessions.py` & `stytch-7.2.1/stytch/b2b/models/discovery_intermediate_sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/models/discovery_organizations.py` & `stytch-7.2.1/stytch/b2b/models/discovery_organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/models/magic_links.py` & `stytch-7.2.1/stytch/b2b/models/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/models/magic_links_discovery.py` & `stytch-7.2.1/stytch/b2b/models/magic_links_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/models/magic_links_email.py` & `stytch-7.2.1/stytch/b2b/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/models/mfa.py` & `stytch-7.2.1/stytch/b2b/models/mfa.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/models/oauth.py` & `stytch-7.2.1/stytch/b2b/models/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/models/oauth_discovery.py` & `stytch-7.2.1/stytch/b2b/models/oauth_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/models/organizations.py` & `stytch-7.2.1/stytch/b2b/models/organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/models/organizations_members.py` & `stytch-7.2.1/stytch/b2b/models/organizations_members.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/models/otp_sms.py` & `stytch-7.2.1/stytch/b2b/models/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/models/passwords.py` & `stytch-7.2.1/stytch/b2b/models/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/models/passwords_email.py` & `stytch-7.2.1/stytch/b2b/models/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/models/passwords_existing_password.py` & `stytch-7.2.1/stytch/b2b/models/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/models/passwords_session.py` & `stytch-7.2.1/stytch/b2b/models/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/models/sessions.py` & `stytch-7.2.1/stytch/b2b/models/sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,26 +29,26 @@
     Fields:
       - member_session_id: Globally unique UUID that identifies a specific Session.
       - member_id: Globally unique UUID that identifies a specific Member.
       - started_at: The timestamp when the Session was created. Values conform to the RFC 3339 standard and are expressed in UTC, e.g. `2021-12-29T12:33:09Z`.
       - last_accessed_at: The timestamp when the Session was last accessed. Values conform to the RFC 3339 standard and are expressed in UTC, e.g. `2021-12-29T12:33:09Z`.
       - expires_at: The timestamp when the Session expires. Values conform to the RFC 3339 standard and are expressed in UTC, e.g. `2021-12-29T12:33:09Z`.
       - authentication_factors: An array of different authentication factors that have initiated a Session.
-      - custom_claims: The custom claims map for a Session. Claims can be added to a session during a Sessions authenticate call.
       - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+      - custom_claims: The custom claims map for a Session. Claims can be added to a session during a Sessions authenticate call.
     """  # noqa
 
     member_session_id: str
     member_id: str
     started_at: datetime.datetime
     last_accessed_at: datetime.datetime
     expires_at: datetime.datetime
     authentication_factors: List[AuthenticationFactor]
-    custom_claims: Dict[str, Any]
     organization_id: str
+    custom_claims: Optional[Dict[str, Any]] = None
 
 
 class AuthenticateResponse(ResponseBase):
     """Response type for `Sessions.authenticate`.
     Fields:
       - member_session: The [Session object](https://stytch.com/docs/b2b/api/session-object).
       - session_token: A secret token for a given Stytch Session.
```

### Comparing `stytch-7.2.0/stytch/b2b/models/sso.py` & `stytch-7.2.1/stytch/b2b/models/sso.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/models/sso_oidc.py` & `stytch-7.2.1/stytch/b2b/models/sso_oidc.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/b2b/models/sso_saml.py` & `stytch-7.2.1/stytch/b2b/models/sso_saml.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/api/crypto_wallets.py` & `stytch-7.2.1/stytch/consumer/api/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/api/magic_links.py` & `stytch-7.2.1/stytch/consumer/api/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/api/magic_links_email.py` & `stytch-7.2.1/stytch/consumer/api/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/api/oauth.py` & `stytch-7.2.1/stytch/consumer/api/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/api/otp.py` & `stytch-7.2.1/stytch/consumer/api/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/api/otp_email.py` & `stytch-7.2.1/stytch/consumer/api/otp_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/api/otp_sms.py` & `stytch-7.2.1/stytch/consumer/api/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/api/otp_whatsapp.py` & `stytch-7.2.1/stytch/consumer/api/otp_whatsapp.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/api/passwords.py` & `stytch-7.2.1/stytch/consumer/api/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/api/passwords_email.py` & `stytch-7.2.1/stytch/consumer/api/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/api/passwords_existing_password.py` & `stytch-7.2.1/stytch/consumer/api/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/api/passwords_session.py` & `stytch-7.2.1/stytch/consumer/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/api/sessions.py` & `stytch-7.2.1/stytch/consumer/api/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/api/totps.py` & `stytch-7.2.1/stytch/consumer/api/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/api/users.py` & `stytch-7.2.1/stytch/consumer/api/users.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/api/webauthn.py` & `stytch-7.2.1/stytch/consumer/api/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/client.py` & `stytch-7.2.1/stytch/consumer/client.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/models/crypto_wallets.py` & `stytch-7.2.1/stytch/consumer/models/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/models/magic_links.py` & `stytch-7.2.1/stytch/consumer/models/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/models/magic_links_email.py` & `stytch-7.2.1/stytch/consumer/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/models/oauth.py` & `stytch-7.2.1/stytch/consumer/models/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/models/otp.py` & `stytch-7.2.1/stytch/consumer/models/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/models/otp_email.py` & `stytch-7.2.1/stytch/consumer/models/otp_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/models/otp_sms.py` & `stytch-7.2.1/stytch/consumer/models/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/models/otp_whatsapp.py` & `stytch-7.2.1/stytch/consumer/models/otp_whatsapp.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/models/passwords.py` & `stytch-7.2.1/stytch/consumer/models/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/models/passwords_email.py` & `stytch-7.2.1/stytch/consumer/models/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/models/passwords_existing_password.py` & `stytch-7.2.1/stytch/consumer/models/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/models/passwords_session.py` & `stytch-7.2.1/stytch/consumer/models/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/models/sessions.py` & `stytch-7.2.1/stytch/consumer/models/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/models/totps.py` & `stytch-7.2.1/stytch/consumer/models/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/models/users.py` & `stytch-7.2.1/stytch/consumer/models/users.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/consumer/models/webauthn.py` & `stytch-7.2.1/stytch/consumer/models/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/core/api_base.py` & `stytch-7.2.1/stytch/core/api_base.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/core/client_base.py` & `stytch-7.2.1/stytch/core/client_base.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/core/http/client.py` & `stytch-7.2.1/stytch/core/http/client.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch/core/response_base.py` & `stytch-7.2.1/stytch/core/response_base.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/stytch.egg-info/PKG-INFO` & `stytch-7.2.1/stytch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 7.2.0
+Version: 7.2.1
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-7.2.0/stytch.egg-info/SOURCES.txt` & `stytch-7.2.1/stytch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/test/test_integration.py` & `stytch-7.2.1/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `stytch-7.2.0/test/test_integration_async.py` & `stytch-7.2.1/test/test_integration_async.py`

 * *Files identical despite different names*

