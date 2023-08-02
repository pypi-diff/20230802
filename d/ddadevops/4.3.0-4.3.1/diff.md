# Comparing `tmp/ddadevops-4.3.0.tar.gz` & `tmp/ddadevops-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddadevops-4.3.0.tar", last modified: Fri Jul 21 15:44:33 2023, max compression
+gzip compressed data, was "ddadevops-4.3.1.tar", last modified: Wed Aug  2 14:51:58 2023, max compression
```

## Comparing `ddadevops-4.3.0.tar` & `ddadevops-4.3.1.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:44:33.803721 ddadevops-4.3.0/
--rw-rw-r--   0 root         (0) root         (0)      137 2023-07-21 15:44:33.000000 ddadevops-4.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6803 2023-07-21 15:44:33.803721 ddadevops-4.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 15:44:33.000000 ddadevops-4.3.0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:44:33.798721 ddadevops-4.3.0/ddadevops/
--rw-rw-rw-   0 root         (0) root         (0)    11357 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      640 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:44:33.799721 ddadevops-4.3.0/ddadevops/application/
--rw-rw-rw-   0 root         (0) root         (0)      150 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/application/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2855 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/application/image_build_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2515 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/application/release_mixin_services.py
--rw-rw-rw-   0 root         (0) root         (0)     9245 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/application/terraform_service.py
--rw-rw-rw-   0 root         (0) root         (0)     3953 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/aws_mfa_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1540 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/c4k_build.py
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/credential.py
--rw-rw-rw-   0 root         (0) root         (0)     1018 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/devops_build.py
--rw-rw-rw-   0 root         (0) root         (0)     1358 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/devops_image_build.py
--rw-rw-rw-   0 root         (0) root         (0)     2284 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/devops_terraform_build.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:44:33.801721 ddadevops-4.3.0/ddadevops/domain/
--rw-rw-rw-   0 root         (0) root         (0)      647 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/domain/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5182 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/domain/build_file.py
--rw-rw-rw-   0 root         (0) root         (0)     2982 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/domain/c4k.py
--rw-rw-rw-   0 root         (0) root         (0)     3284 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/domain/common.py
--rw-rw-rw-   0 root         (0) root         (0)     1916 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/domain/credentials.py
--rw-rw-rw-   0 root         (0) root         (0)     1870 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/domain/devops_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     2425 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/domain/image.py
--rw-rw-rw-   0 root         (0) root         (0)     4531 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/domain/init_service.py
--rw-rw-rw-   0 root         (0) root         (0)     3687 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/domain/provider_aws.py
--rw-rw-rw-   0 root         (0) root         (0)     3891 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/domain/provider_digitalocean.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/domain/provider_hetzner.py
--rw-rw-rw-   0 root         (0) root         (0)     3422 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/domain/provs_k3s.py
--rw-rw-rw-   0 root         (0) root         (0)     2381 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/domain/release.py
--rw-rw-rw-   0 root         (0) root         (0)     4101 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/domain/terraform.py
--rw-rw-rw-   0 root         (0) root         (0)     4564 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/domain/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:44:33.801721 ddadevops-4.3.0/ddadevops/infrastructure/
--rw-rw-rw-   0 root         (0) root         (0)      226 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/infrastructure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7068 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/infrastructure/infrastructure.py
--rw-rw-rw-   0 root         (0) root         (0)     1097 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/infrastructure/repository.py
--rw-rw-rw-   0 root         (0) root         (0)     1332 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/provs_k3s_build.py
--rw-rw-rw-   0 root         (0) root         (0)     1177 2023-07-21 15:44:22.000000 ddadevops-4.3.0/ddadevops/release_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:44:33.797721 ddadevops-4.3.0/ddadevops/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:44:33.797721 ddadevops-4.3.0/ddadevops/src/main/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:44:33.797721 ddadevops-4.3.0/ddadevops/src/main/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:44:33.797721 ddadevops-4.3.0/ddadevops/src/main/resources/docker/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:44:33.797721 ddadevops-4.3.0/ddadevops/src/main/resources/docker/image/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:44:33.801721 ddadevops-4.3.0/ddadevops/src/main/resources/docker/image/resources/
--rwxrwxrwx   0 root         (0) root         (0)      628 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops/src/main/resources/docker/image/resources/install_functions.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:44:33.802721 ddadevops-4.3.0/ddadevops/src/main/resources/terraform/
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops/src/main/resources/terraform/aws_backend.tf
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops/src/main/resources/terraform/aws_backend_wkms_vars.tf
--rw-rw-rw-   0 root         (0) root         (0)       65 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops/src/main/resources/terraform/aws_backend_wokms_vars.tf
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops/src/main/resources/terraform/aws_provider.tf
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops/src/main/resources/terraform/aws_provider_vars.tf
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops/src/main/resources/terraform/do_backend.tf
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops/src/main/resources/terraform/do_backend_vars.tf
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops/src/main/resources/terraform/do_provider.tf
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops/src/main/resources/terraform/do_provider_vars.tf
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops/src/main/resources/terraform/hetzner_provider.tf
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops/src/main/resources/terraform/hetzner_provider_vars.tf
--rw-rw-rw-   0 root         (0) root         (0)      392 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops/src/main/resources/terraform/provider_registry.tf
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops/src/main/resources/terraform/terraform_build_vars.tf
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops/src/main/resources/terraform/versions.tf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:44:33.799721 ddadevops-4.3.0/ddadevops.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6803 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2144 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:44:33.000000 ddadevops-4.3.0/ddadevops.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 15:44:33.803721 ddadevops-4.3.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     8335 2023-07-21 15:44:33.000000 ddadevops-4.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:51:58.001868 ddadevops-4.3.1/
+-rw-rw-r--   0 root         (0) root         (0)      137 2023-08-02 14:51:57.000000 ddadevops-4.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6866 2023-08-02 14:51:58.001868 ddadevops-4.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 14:51:57.000000 ddadevops-4.3.1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:51:57.996868 ddadevops-4.3.1/ddadevops/
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      640 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:51:57.997868 ddadevops-4.3.1/ddadevops/application/
+-rw-rw-rw-   0 root         (0) root         (0)      150 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/application/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/application/image_build_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2515 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/application/release_mixin_services.py
+-rw-rw-rw-   0 root         (0) root         (0)     9245 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/application/terraform_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/artifact_deployment_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3953 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/aws_mfa_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1540 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/c4k_build.py
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/credential.py
+-rw-rw-rw-   0 root         (0) root         (0)     1018 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/devops_build.py
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/devops_image_build.py
+-rw-rw-rw-   0 root         (0) root         (0)     2284 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/devops_terraform_build.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:51:57.998868 ddadevops-4.3.1/ddadevops/domain/
+-rw-rw-rw-   0 root         (0) root         (0)      647 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/domain/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5182 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/domain/build_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     2982 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/domain/c4k.py
+-rw-rw-rw-   0 root         (0) root         (0)     3284 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/domain/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     1916 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/domain/credentials.py
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/domain/devops_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2425 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/domain/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     4531 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/domain/init_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     3789 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/domain/provider_aws.py
+-rw-rw-rw-   0 root         (0) root         (0)     3891 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/domain/provider_digitalocean.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/domain/provider_hetzner.py
+-rw-rw-rw-   0 root         (0) root         (0)     3422 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/domain/provs_k3s.py
+-rw-rw-rw-   0 root         (0) root         (0)     2381 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/domain/release.py
+-rw-rw-rw-   0 root         (0) root         (0)     4101 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/domain/terraform.py
+-rw-rw-rw-   0 root         (0) root         (0)     4564 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/domain/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:51:57.999868 ddadevops-4.3.1/ddadevops/infrastructure/
+-rw-rw-rw-   0 root         (0) root         (0)      226 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/infrastructure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7068 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/infrastructure/infrastructure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/infrastructure/repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/provs_k3s_build.py
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2023-08-02 14:51:47.000000 ddadevops-4.3.1/ddadevops/release_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:51:57.994868 ddadevops-4.3.1/ddadevops/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:51:57.994868 ddadevops-4.3.1/ddadevops/src/main/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:51:57.994868 ddadevops-4.3.1/ddadevops/src/main/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:51:57.994868 ddadevops-4.3.1/ddadevops/src/main/resources/docker/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:51:57.994868 ddadevops-4.3.1/ddadevops/src/main/resources/docker/image/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:51:57.999868 ddadevops-4.3.1/ddadevops/src/main/resources/docker/image/resources/
+-rwxrwxrwx   0 root         (0) root         (0)      628 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops/src/main/resources/docker/image/resources/install_functions.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:51:58.000868 ddadevops-4.3.1/ddadevops/src/main/resources/terraform/
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops/src/main/resources/terraform/aws_backend.tf
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops/src/main/resources/terraform/aws_backend_wkms_vars.tf
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops/src/main/resources/terraform/aws_backend_wokms_vars.tf
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops/src/main/resources/terraform/aws_provider.tf
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops/src/main/resources/terraform/aws_provider_vars.tf
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops/src/main/resources/terraform/do_backend.tf
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops/src/main/resources/terraform/do_backend_vars.tf
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops/src/main/resources/terraform/do_provider.tf
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops/src/main/resources/terraform/do_provider_vars.tf
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops/src/main/resources/terraform/hetzner_provider.tf
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops/src/main/resources/terraform/hetzner_provider_vars.tf
+-rw-rw-rw-   0 root         (0) root         (0)      392 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops/src/main/resources/terraform/provider_registry.tf
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops/src/main/resources/terraform/terraform_build_vars.tf
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops/src/main/resources/terraform/versions.tf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:51:57.996868 ddadevops-4.3.1/ddadevops.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6866 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2183 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 14:51:57.000000 ddadevops-4.3.1/ddadevops.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 14:51:58.001868 ddadevops-4.3.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     8399 2023-08-02 14:51:57.000000 ddadevops-4.3.1/setup.py
```

### Comparing `ddadevops-4.3.0/PKG-INFO` & `ddadevops-4.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddadevops
-Version: 4.3.0
+Version: 4.3.1
 Summary: tools to support builds combining gopass, terraform, dda-pallet, aws & hetzner-cloud
 Home-page: https://repo.prod.meissa.de/meissa/dda-devops-build
 Author: meissa GmbH
 Author-email: buero@meissa-gmbh.de
 Maintainer: 
 Maintainer-email: 
 License: Apache Software License
@@ -220,14 +220,15 @@
 ## Development & mirrors
 
 Development happens at: https://repo.prod.meissa.de/meissa/dda-devops-build
 
 Mirrors are:
 
 * https://gitlab.com/domaindrivenarchitecture/dda-devops-build (issues and PR, CI)
+* https://github.com/DomainDrivenArchitecture/dda-devops-build
 
 For more details about our repository model see: https://repo.prod.meissa.de/meissa/federate-your-repos
 
 ## License
 
 Copyright © 2021 meissa GmbH
 Licensed under the [Apache License, Version 2.0](LICENSE) (the "License")
```

### Comparing `ddadevops-4.3.0/ddadevops/LICENSE` & `ddadevops-4.3.1/ddadevops/LICENSE`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/__init__.py` & `ddadevops-4.3.1/ddadevops/__init__.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/application/image_build_service.py` & `ddadevops-4.3.1/ddadevops/application/image_build_service.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/application/release_mixin_services.py` & `ddadevops-4.3.1/ddadevops/application/release_mixin_services.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/application/terraform_service.py` & `ddadevops-4.3.1/ddadevops/application/terraform_service.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/aws_mfa_mixin.py` & `ddadevops-4.3.1/ddadevops/aws_mfa_mixin.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/c4k_build.py` & `ddadevops-4.3.1/ddadevops/c4k_build.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/devops_build.py` & `ddadevops-4.3.1/ddadevops/devops_build.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/devops_image_build.py` & `ddadevops-4.3.1/ddadevops/devops_image_build.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/devops_terraform_build.py` & `ddadevops-4.3.1/ddadevops/devops_terraform_build.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/domain/__init__.py` & `ddadevops-4.3.1/ddadevops/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/domain/build_file.py` & `ddadevops-4.3.1/ddadevops/domain/build_file.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/domain/c4k.py` & `ddadevops-4.3.1/ddadevops/domain/c4k.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/domain/common.py` & `ddadevops-4.3.1/ddadevops/domain/common.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/domain/credentials.py` & `ddadevops-4.3.1/ddadevops/domain/credentials.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/domain/devops_factory.py` & `ddadevops-4.3.1/ddadevops/domain/devops_factory.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/domain/image.py` & `ddadevops-4.3.1/ddadevops/domain/image.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/domain/init_service.py` & `ddadevops-4.3.1/ddadevops/domain/init_service.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/domain/provider_aws.py` & `ddadevops-4.3.1/ddadevops/domain/provider_aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
             result += self.__validate_is_not_empty__("aws_region")
         return result
 
     def backend_config(self) -> Dict[str, Any]:
         result = {}
         if self.aws_as_backend:
             result = {
+                "access_key": self.aws_access_key,
+                "secret_key": self.aws_secret_key,
                 "bucket": self.aws_bucket,
                 "key": self.__bucket_key__(),
                 "region": self.aws_region,
             }
             if self.aws_bucket_kms_key_id:
                 result["kms_key_id"] = self.aws_bucket_kms_key_id
         return result
```

### Comparing `ddadevops-4.3.0/ddadevops/domain/provider_digitalocean.py` & `ddadevops-4.3.1/ddadevops/domain/provider_digitalocean.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/domain/provider_hetzner.py` & `ddadevops-4.3.1/ddadevops/domain/provider_hetzner.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/domain/provs_k3s.py` & `ddadevops-4.3.1/ddadevops/domain/provs_k3s.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/domain/release.py` & `ddadevops-4.3.1/ddadevops/domain/release.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/domain/terraform.py` & `ddadevops-4.3.1/ddadevops/domain/terraform.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/domain/version.py` & `ddadevops-4.3.1/ddadevops/domain/version.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/infrastructure/infrastructure.py` & `ddadevops-4.3.1/ddadevops/infrastructure/infrastructure.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/infrastructure/repository.py` & `ddadevops-4.3.1/ddadevops/infrastructure/repository.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/provs_k3s_build.py` & `ddadevops-4.3.1/ddadevops/provs_k3s_build.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/release_mixin.py` & `ddadevops-4.3.1/ddadevops/release_mixin.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops/src/main/resources/docker/image/resources/install_functions.sh` & `ddadevops-4.3.1/ddadevops/src/main/resources/docker/image/resources/install_functions.sh`

 * *Files identical despite different names*

### Comparing `ddadevops-4.3.0/ddadevops.egg-info/PKG-INFO` & `ddadevops-4.3.1/ddadevops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddadevops
-Version: 4.3.0
+Version: 4.3.1
 Summary: tools to support builds combining gopass, terraform, dda-pallet, aws & hetzner-cloud
 Home-page: https://repo.prod.meissa.de/meissa/dda-devops-build
 Author: meissa GmbH
 Author-email: buero@meissa-gmbh.de
 Maintainer: 
 Maintainer-email: 
 License: Apache Software License
@@ -220,14 +220,15 @@
 ## Development & mirrors
 
 Development happens at: https://repo.prod.meissa.de/meissa/dda-devops-build
 
 Mirrors are:
 
 * https://gitlab.com/domaindrivenarchitecture/dda-devops-build (issues and PR, CI)
+* https://github.com/DomainDrivenArchitecture/dda-devops-build
 
 For more details about our repository model see: https://repo.prod.meissa.de/meissa/federate-your-repos
 
 ## License
 
 Copyright © 2021 meissa GmbH
 Licensed under the [Apache License, Version 2.0](LICENSE) (the "License")
```

### Comparing `ddadevops-4.3.0/ddadevops.egg-info/SOURCES.txt` & `ddadevops-4.3.1/ddadevops.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 MANIFEST.in
 __init__.py
 setup.py
 ddadevops/LICENSE
 ddadevops/__init__.py
+ddadevops/artifact_deployment_mixin.py
 ddadevops/aws_mfa_mixin.py
 ddadevops/c4k_build.py
 ddadevops/credential.py
 ddadevops/devops_build.py
 ddadevops/devops_image_build.py
 ddadevops/devops_terraform_build.py
 ddadevops/provs_k3s_build.py
```

### Comparing `ddadevops-4.3.0/setup.py` & `ddadevops-4.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'ddadevops',
-        version = '4.3.0',
+        version = '4.3.1',
         description = 'tools to support builds combining gopass, terraform, dda-pallet, aws & hetzner-cloud',
-        long_description = '# dda-devops-build\n\n[![Slack](https://img.shields.io/badge/chat-clojurians-green.svg?style=flat)](https://clojurians.slack.com/messages/#dda-pallet/) | [<img src="https://meissa-gmbh.de/img/community/Mastodon_Logotype.svg" width=20 alt="team@social.meissa-gmbh.de"> team@social.meissa-gmbh.de](https://social.meissa-gmbh.de/@team) | [Website & Blog](https://domaindrivenarchitecture.org)\n\n![release prod](https://github.com/DomainDrivenArchitecture/dda-devops-build/workflows/release%20prod/badge.svg)\n\ndda-devops-build integrates all the tools we use to work with clouds & provide some nice functions around.\n\nTools we support are\n\n* terraform: for setting up the plain infrastructure around.\n* docker: for creating images\n* c4k: for generating kubernetes manifests\n* provs: for setting up small single-node k3s clusters\n* gopass: for credential management on devops computers\n* cloud providers: hetzner, digitalocean, aws\n\nIn addition we provide a ReleaseMixin for release related tasks like tag / publish & version-bump\n\n```mermaid\nclassDiagram\n    class DevopsBuild {\n        name()\n        build_path()\n        initialize_build_dir()\n    }\n\n    class DevopsTerraformBuild {\n        initialize_build_dir()\n        post_build()\n        read_output_json()\n        plan()\n        plan_fail_on_diff()\n        apply(auto_approve=False)\n        refresh()\n        destroy(auto_approve=False)\n        tf_import(tf_import_name,tf_import_resource)\n    }\n\n    class DevopsImageBuild {\n        initialize_build_dir()\n        image()\n        drun()\n        dockerhub_login()\n        dockerhub_publish()\n        test()\n    }\n\n    class ReleaseMixin {\n        prepare_release()\n        tag_and_push_release()\n    }\n    \n    class ProvsK3sBuild {\n        def update_runtime_config(dns_record)\n        write_provs_config()\n        provs_apply(dry_run=False)\n    }\n\n    class C4kBuild {\n        def update_runtime_config(dns_record)\n        def write_c4k_config()\n        def write_c4k_auth()\n        c4k_apply(dry_run=False)\n    }\n\n    DevopsBuild <|-- DevopsImageBuild\n    DevopsBuild <|-- DevopsTerraformBuild\n    DevopsBuild <|-- ReleaseMixin\n    DevopsBuild <|-- ProvsK3sBuild\n    DevopsBuild <|-- C4kBuild\n\n    link DevopsBuild "dda-devops-build/src/doc/DevopsBuild.md"\n    link DevopsImageBuild "dda-devops-build/src/doc/DevopsImageBuild.md"\n    link DevopsTerraformBuild "dda-devops-build/src/doc/DevopsTerraformBuild.md"\n    link ReleaseMixin "dda-devops-build/src/doc/ReleaseMixin.md"\n    link ProvsK3sBuild "dda-devops-build/src/doc/ProvsK3sBuild.md"\n    link C4kBuild "dda-devops-build/src/doc/C4kBuild.md"\n\n```\n\nPrinciples we follow are:\n\n* Seperate build artefacts from version controlled code\n* Domain Driven Design - in order to stay sustainable\n\n## Installation\n\nEnsure that yout python3 version is at least Python 3.10\n\n```\nsudo apt install python3-pip\npip3 install -r requirements.txt\nexport PATH=$PATH:~/.local/bin\n```\n\n## Reference\n\n* [DevopsBuild](./doc/DevopsBuild.md)\n* [DevopsImageBuild](./doc/DevopsImageBuild.md)\n* [DevopsTerraformBuild](./doc/DevopsTerraformBuild.md)\n  * [AwsProvider](doc/DevopsTerraformBuildWithAwsProvider.md)\n  * [DigitaloceanProvider](doc/DevopsTerraformBuildWithDigitaloceanProvider.md)\n  * [HetznerProvider](doc/DevopsTerraformBuildWithHetznerProvider.md)\n* [ReleaseMixin](./doc/ReleaseMixin.md)\n* [ProvsK3sBuild](doc/ProvsK3sBuild.md)\n* [C4kBuild](doc/C4kBuild.md)\n\n## Example Build\n\nlets assume the following project structure\n\n```\nmy-project\n   | -> my-module\n   |       | -> build.py\n   |       | -> some-terraform.tf\n   | -> an-other-module\n   | -> target  (here will the build happen)\n   |       | -> ...\n```\n\n```python\nfrom pybuilder.core import task, init\nfrom ddadevops import *\n\nname = \'my-project\'\nMODULE = \'my-module\'\nPROJECT_ROOT_PATH = \'..\'\n\n\n@init\ndef initialize(project):\n    project.build_depends_on("ddadevops>=4.0.0-dev")\n\n    config = {\n        "credentials_mapping": [\n            {\n                "gopass_path": environ.get("DIGITALOCEAN_TOKEN_KEY_PATH", None),\n                "name": "do_api_key",\n            },\n            {\n                "gopass_path": environ.get("HETZNER_API_KEY_PATH", None),\n                "name": "hetzner_api_key",\n            },\n        ],\n        "name": name,\n        "module": MODULE,\n        "stage": environ["STAGE"],\n        "project_root_path": PROJECT_ROOT_PATH,\n        "build_types": ["TERRAFORM"],\n        "mixin_types": [],\n        "tf_provider_types": ["DIGITALOCEAN", "HETZNER"],\n        "tf_use_workspace": False,\n        "tf_terraform_semantic_version": "1.4.2",\n        "do_as_backend": True,\n        "do_bucket": "your-bucket",\n    }\n\n    build = DevopsTerraformBuild(project, config)\n    build.initialize_build_dir()\n\n\n@task\ndef plan(project):\n    build = get_devops_build(project)\n    build.plan()\n\n\n@task\ndef apply(project):\n    build = get_devops_build(project)\n    build.apply(True)\n\n\n@task\ndef destroy(project):\n    build = get_devops_build(project)\n    build.destroy(True)\n\n```\n\n## Snapshot & Release\n\n```\npyb dev publish upload\npip3 install --upgrade ddadevops --pre\n\npyb [patch|minor|major]\npip3 install --upgrade ddadevops\n```\n\n## Development & mirrors\n\nDevelopment happens at: https://repo.prod.meissa.de/meissa/dda-devops-build\n\nMirrors are:\n\n* https://gitlab.com/domaindrivenarchitecture/dda-devops-build (issues and PR, CI)\n\nFor more details about our repository model see: https://repo.prod.meissa.de/meissa/federate-your-repos\n\n## License\n\nCopyright © 2021 meissa GmbH\nLicensed under the [Apache License, Version 2.0](LICENSE) (the "License")\n\n## License\n\nCopyright © 2023 meissa GmbH\nLicensed under the [Apache License, Version 2.0](LICENSE) (the "License")\n',
+        long_description = '# dda-devops-build\n\n[![Slack](https://img.shields.io/badge/chat-clojurians-green.svg?style=flat)](https://clojurians.slack.com/messages/#dda-pallet/) | [<img src="https://meissa-gmbh.de/img/community/Mastodon_Logotype.svg" width=20 alt="team@social.meissa-gmbh.de"> team@social.meissa-gmbh.de](https://social.meissa-gmbh.de/@team) | [Website & Blog](https://domaindrivenarchitecture.org)\n\n![release prod](https://github.com/DomainDrivenArchitecture/dda-devops-build/workflows/release%20prod/badge.svg)\n\ndda-devops-build integrates all the tools we use to work with clouds & provide some nice functions around.\n\nTools we support are\n\n* terraform: for setting up the plain infrastructure around.\n* docker: for creating images\n* c4k: for generating kubernetes manifests\n* provs: for setting up small single-node k3s clusters\n* gopass: for credential management on devops computers\n* cloud providers: hetzner, digitalocean, aws\n\nIn addition we provide a ReleaseMixin for release related tasks like tag / publish & version-bump\n\n```mermaid\nclassDiagram\n    class DevopsBuild {\n        name()\n        build_path()\n        initialize_build_dir()\n    }\n\n    class DevopsTerraformBuild {\n        initialize_build_dir()\n        post_build()\n        read_output_json()\n        plan()\n        plan_fail_on_diff()\n        apply(auto_approve=False)\n        refresh()\n        destroy(auto_approve=False)\n        tf_import(tf_import_name,tf_import_resource)\n    }\n\n    class DevopsImageBuild {\n        initialize_build_dir()\n        image()\n        drun()\n        dockerhub_login()\n        dockerhub_publish()\n        test()\n    }\n\n    class ReleaseMixin {\n        prepare_release()\n        tag_and_push_release()\n    }\n    \n    class ProvsK3sBuild {\n        def update_runtime_config(dns_record)\n        write_provs_config()\n        provs_apply(dry_run=False)\n    }\n\n    class C4kBuild {\n        def update_runtime_config(dns_record)\n        def write_c4k_config()\n        def write_c4k_auth()\n        c4k_apply(dry_run=False)\n    }\n\n    DevopsBuild <|-- DevopsImageBuild\n    DevopsBuild <|-- DevopsTerraformBuild\n    DevopsBuild <|-- ReleaseMixin\n    DevopsBuild <|-- ProvsK3sBuild\n    DevopsBuild <|-- C4kBuild\n\n    link DevopsBuild "dda-devops-build/src/doc/DevopsBuild.md"\n    link DevopsImageBuild "dda-devops-build/src/doc/DevopsImageBuild.md"\n    link DevopsTerraformBuild "dda-devops-build/src/doc/DevopsTerraformBuild.md"\n    link ReleaseMixin "dda-devops-build/src/doc/ReleaseMixin.md"\n    link ProvsK3sBuild "dda-devops-build/src/doc/ProvsK3sBuild.md"\n    link C4kBuild "dda-devops-build/src/doc/C4kBuild.md"\n\n```\n\nPrinciples we follow are:\n\n* Seperate build artefacts from version controlled code\n* Domain Driven Design - in order to stay sustainable\n\n## Installation\n\nEnsure that yout python3 version is at least Python 3.10\n\n```\nsudo apt install python3-pip\npip3 install -r requirements.txt\nexport PATH=$PATH:~/.local/bin\n```\n\n## Reference\n\n* [DevopsBuild](./doc/DevopsBuild.md)\n* [DevopsImageBuild](./doc/DevopsImageBuild.md)\n* [DevopsTerraformBuild](./doc/DevopsTerraformBuild.md)\n  * [AwsProvider](doc/DevopsTerraformBuildWithAwsProvider.md)\n  * [DigitaloceanProvider](doc/DevopsTerraformBuildWithDigitaloceanProvider.md)\n  * [HetznerProvider](doc/DevopsTerraformBuildWithHetznerProvider.md)\n* [ReleaseMixin](./doc/ReleaseMixin.md)\n* [ProvsK3sBuild](doc/ProvsK3sBuild.md)\n* [C4kBuild](doc/C4kBuild.md)\n\n## Example Build\n\nlets assume the following project structure\n\n```\nmy-project\n   | -> my-module\n   |       | -> build.py\n   |       | -> some-terraform.tf\n   | -> an-other-module\n   | -> target  (here will the build happen)\n   |       | -> ...\n```\n\n```python\nfrom pybuilder.core import task, init\nfrom ddadevops import *\n\nname = \'my-project\'\nMODULE = \'my-module\'\nPROJECT_ROOT_PATH = \'..\'\n\n\n@init\ndef initialize(project):\n    project.build_depends_on("ddadevops>=4.0.0-dev")\n\n    config = {\n        "credentials_mapping": [\n            {\n                "gopass_path": environ.get("DIGITALOCEAN_TOKEN_KEY_PATH", None),\n                "name": "do_api_key",\n            },\n            {\n                "gopass_path": environ.get("HETZNER_API_KEY_PATH", None),\n                "name": "hetzner_api_key",\n            },\n        ],\n        "name": name,\n        "module": MODULE,\n        "stage": environ["STAGE"],\n        "project_root_path": PROJECT_ROOT_PATH,\n        "build_types": ["TERRAFORM"],\n        "mixin_types": [],\n        "tf_provider_types": ["DIGITALOCEAN", "HETZNER"],\n        "tf_use_workspace": False,\n        "tf_terraform_semantic_version": "1.4.2",\n        "do_as_backend": True,\n        "do_bucket": "your-bucket",\n    }\n\n    build = DevopsTerraformBuild(project, config)\n    build.initialize_build_dir()\n\n\n@task\ndef plan(project):\n    build = get_devops_build(project)\n    build.plan()\n\n\n@task\ndef apply(project):\n    build = get_devops_build(project)\n    build.apply(True)\n\n\n@task\ndef destroy(project):\n    build = get_devops_build(project)\n    build.destroy(True)\n\n```\n\n## Snapshot & Release\n\n```\npyb dev publish upload\npip3 install --upgrade ddadevops --pre\n\npyb [patch|minor|major]\npip3 install --upgrade ddadevops\n```\n\n## Development & mirrors\n\nDevelopment happens at: https://repo.prod.meissa.de/meissa/dda-devops-build\n\nMirrors are:\n\n* https://gitlab.com/domaindrivenarchitecture/dda-devops-build (issues and PR, CI)\n* https://github.com/DomainDrivenArchitecture/dda-devops-build\n\nFor more details about our repository model see: https://repo.prod.meissa.de/meissa/federate-your-repos\n\n## License\n\nCopyright © 2021 meissa GmbH\nLicensed under the [Apache License, Version 2.0](LICENSE) (the "License")\n\n## License\n\nCopyright © 2023 meissa GmbH\nLicensed under the [Apache License, Version 2.0](LICENSE) (the "License")\n',
         long_description_content_type = 'text/markdown',
         classifiers = [
             'License :: OSI Approved :: Apache Software License',
             'Programming Language :: Python',
             'Programming Language :: Python :: 3',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.10',
```

