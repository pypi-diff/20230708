# Comparing `tmp/pulumi_artifactory-4.2.0a1688644862.tar.gz` & `tmp/pulumi_artifactory-4.2.0a1688687344.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_artifactory-4.2.0a1688644862.tar", last modified: Thu Jul  6 12:06:00 2023, max compression
+gzip compressed data, was "pulumi_artifactory-4.2.0a1688687344.tar", last modified: Thu Jul  6 23:54:40 2023, max compression
```

## Comparing `pulumi_artifactory-4.2.0a1688644862.tar` & `pulumi_artifactory-4.2.0a1688687344.tar`

### file list

```diff
@@ -1,308 +1,315 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:06:00.966655 pulumi_artifactory-4.2.0a1688644862/
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-06 12:06:00.966655 pulumi_artifactory-4.2.0a1688644862/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:06:00.962654 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/
--rw-r--r--   0 runner    (1001) docker     (123)    45591 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   345890 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    35054 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    55059 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/anonymous_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    20682 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/artifact_property_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/artifact_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    21303 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/artifactory_release_bundle_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    37201 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19787 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/build_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    15681 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:06:00.966655 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    62204 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/distribution_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/distribution_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    52691 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    59110 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    20243 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/docker_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    64052 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    67404 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58929 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58869 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58891 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    68742 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    69522 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    62856 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    69144 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58809 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58793 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_gitltfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58509 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    82094 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    81914 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    82034 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58569 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    65115 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58749 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    74462 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    81914 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    59285 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    59401 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58809 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/general_security.py
--rw-r--r--   0 runner    (1001) docker     (123)    18670 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16869 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    19407 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16866 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17129 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17064 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16869 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16869 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    20395 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17609 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    19309 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    19818 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17039 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16674 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21978 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21747 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21901 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    18608 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21651 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21747 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16869 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17454 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17580 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_fileinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15539 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13215 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15951 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13167 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12927 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    18115 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17935 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    18055 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17839 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17935 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_terraformbackend_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13167 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_permission_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    34729 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37310 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38810 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34507 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    39127 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38984 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    35982 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34618 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34507 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34729 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42231 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34507 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    36249 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34729 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    35593 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    46136 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    40415 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    45761 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    46868 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34396 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    41369 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34507 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34285 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34396 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34347 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37762 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34396 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    45761 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34618 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    36691 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_terraform_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    39001 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_vcs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16037 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    18607 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    14372 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15027 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15924 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13434 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11434 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_terraform_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    45831 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    30892 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    20049 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)    35213 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/ldap_group_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    51241 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/ldap_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    57650 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49016 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48978 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49759 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48928 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_gitltfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48750 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    71368 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    72133 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    71388 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    55830 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48902 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    23513 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_repository_multi_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)    54950 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_repository_single_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)    69786 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    72133 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49174 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_terraform_backend_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49148 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49220 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48940 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    26725 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/managed_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    47096 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/oauth_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)   303865 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19731 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/permission_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    14587 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/property_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    28448 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    45985 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/pull_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)    20481 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/push_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20304 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/release_bundle_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)   130335 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   138869 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   140151 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   130223 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   139476 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   139130 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   133206 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   130271 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   130205 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   130317 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   147825 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   130201 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   133045 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   130359 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   133037 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   154471 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   144104 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   154309 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   154524 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   130371 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   145461 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   130253 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   130149 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   130191 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   130315 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   137491 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    41782 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_repository_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)   130165 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   154195 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   130237 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   137491 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_terraform_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   140709 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_vcs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/replication_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24784 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/repository_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    43485 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/saml_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    45098 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/scoped_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/single_replication_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    27537 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/unmanaged_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    28961 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    44687 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48898 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42194 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38889 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42286 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42196 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42154 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    54429 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42611 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38715 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38837 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38787 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    50146 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    46520 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    50032 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    52303 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42573 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38627 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38673 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38791 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38699 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    44622 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    50054 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38749 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38517 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_terraform_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:06:00.966655 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 12:06:00.966655 pulumi_artifactory-4.2.0a1688644862/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-06 12:06:00.000000 pulumi_artifactory-4.2.0a1688644862/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:54:40.189628 pulumi_artifactory-4.2.0a1688687344/
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-06 23:54:40.185628 pulumi_artifactory-4.2.0a1688687344/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:54:40.185628 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/
+-rw-r--r--   0 runner    (1001) docker     (123)    47499 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   401292 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35054 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55059 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/anonymous_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21268 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/artifact_custom_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21386 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/artifact_property_custom_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20682 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/artifact_property_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/artifact_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22027 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/artifactory_release_bundle_custom_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21303 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/artifactory_release_bundle_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37201 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20491 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/build_custom_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19787 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/build_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15681 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:54:40.185628 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62204 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22064 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/distribution_custom_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/distribution_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/distribution_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20947 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/docker_custom_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52691 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59110 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20243 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/docker_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64052 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67404 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58929 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58869 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58891 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68742 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69522 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62856 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69144 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58809 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58793 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_gitltfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58509 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82094 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81914 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82034 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58569 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65115 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58749 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74462 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81914 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59285 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59401 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58809 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/general_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18670 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16869 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19407 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16866 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17129 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17064 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16869 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16869 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20395 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17609 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19309 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19818 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17039 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16674 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21978 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21747 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21901 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18608 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21651 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21747 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16869 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17454 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17580 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_fileinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15539 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13215 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15951 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13167 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12927 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18115 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17935 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18055 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17839 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17935 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_terraformbackend_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13167 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_permission_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34729 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37310 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38810 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34507 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39127 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38984 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35982 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34618 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34507 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34729 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42231 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34507 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36249 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34729 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35593 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46136 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40415 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45761 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46868 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34396 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41369 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34507 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34285 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34396 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34347 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37762 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34396 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45761 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34618 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36691 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_terraform_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39001 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_vcs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16037 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18607 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14372 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15027 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15924 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13434 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11434 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_terraform_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45831 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30892 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20049 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35213 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/ldap_group_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51241 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/ldap_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57650 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49016 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48978 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49759 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48928 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_gitltfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48750 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71368 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72133 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71388 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55830 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48902 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23513 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_repository_multi_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54950 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_repository_single_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69786 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72133 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49174 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_terraform_backend_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49148 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49220 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48940 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26725 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/managed_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47096 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/oauth_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)   356166 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19731 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/permission_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14587 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/property_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28448 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45985 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/pull_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20481 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/push_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21008 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/release_bundle_custom_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20304 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/release_bundle_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130335 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138869 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   140151 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130223 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139476 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139130 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133206 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130271 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130205 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130317 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   147825 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130201 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133045 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130359 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133037 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154471 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144104 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154309 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154524 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130371 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   145461 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130253 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130149 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130191 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130315 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137491 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41782 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_repository_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130165 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154195 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130237 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137491 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_terraform_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   140709 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_vcs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/replication_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24784 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/repository_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43485 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/saml_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44958 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/scoped_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/single_replication_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27537 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/unmanaged_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28961 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44687 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48898 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42194 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38889 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42286 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42196 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42154 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54429 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42611 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38715 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38837 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38787 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50146 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46520 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50032 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52303 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42573 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38627 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38673 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38791 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38699 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44622 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50054 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38749 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38517 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_terraform_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:54:40.185628 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-06 23:54:40.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14483 2023-07-06 23:54:40.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 23:54:40.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 23:54:40.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-06 23:54:40.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 23:54:40.000000 pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 23:54:40.189628 pulumi_artifactory-4.2.0a1688687344/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-06 23:54:39.000000 pulumi_artifactory-4.2.0a1688687344/setup.py
```

### Comparing `pulumi_artifactory-4.2.0a1688644862/PKG-INFO` & `pulumi_artifactory-4.2.0a1688687344/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_artifactory
-Version: 4.2.0a1688644862
+Version: 4.2.0a1688687344
 Summary: A Pulumi package for creating and managing artifactory cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-artifactory
 Keywords: pulumi artifactory
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_artifactory-4.2.0a1688644862/README.md` & `pulumi_artifactory-4.2.0a1688687344/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/__init__.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,29 @@
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .access_token import *
 from .alpine_repository import *
 from .anonymous_user import *
 from .api_key import *
+from .artifact_custom_webhook import *
+from .artifact_property_custom_webhook import *
 from .artifact_property_webhook import *
 from .artifact_webhook import *
+from .artifactory_release_bundle_custom_webhook import *
 from .artifactory_release_bundle_webhook import *
 from .backup import *
+from .build_custom_webhook import *
 from .build_webhook import *
 from .certificate import *
 from .debian_repository import *
+from .distribution_custom_webhook import *
 from .distribution_public_key import *
 from .distribution_webhook import *
+from .docker_custom_webhook import *
 from .docker_v1_repository import *
 from .docker_v2_repository import *
 from .docker_webhook import *
 from .federated_alpine_repository import *
 from .federated_bower_repository import *
 from .federated_cargo_repository import *
 from .federated_chef_repository import *
@@ -222,14 +228,15 @@
 from .oauth_settings import *
 from .permission_target import *
 from .property_set import *
 from .provider import *
 from .proxy import *
 from .pull_replication import *
 from .push_replication import *
+from .release_bundle_custom_webhook import *
 from .release_bundle_webhook import *
 from .remote_alpine_repository import *
 from .remote_bower_repository import *
 from .remote_cargo_repository import *
 from .remote_chef_repository import *
 from .remote_cocoapods_repository import *
 from .remote_composer_repository import *
@@ -334,14 +341,30 @@
   "fqn": "pulumi_artifactory",
   "classes": {
    "artifactory:index/apiKey:ApiKey": "ApiKey"
   }
  },
  {
   "pkg": "artifactory",
+  "mod": "index/artifactCustomWebhook",
+  "fqn": "pulumi_artifactory",
+  "classes": {
+   "artifactory:index/artifactCustomWebhook:ArtifactCustomWebhook": "ArtifactCustomWebhook"
+  }
+ },
+ {
+  "pkg": "artifactory",
+  "mod": "index/artifactPropertyCustomWebhook",
+  "fqn": "pulumi_artifactory",
+  "classes": {
+   "artifactory:index/artifactPropertyCustomWebhook:ArtifactPropertyCustomWebhook": "ArtifactPropertyCustomWebhook"
+  }
+ },
+ {
+  "pkg": "artifactory",
   "mod": "index/artifactPropertyWebhook",
   "fqn": "pulumi_artifactory",
   "classes": {
    "artifactory:index/artifactPropertyWebhook:ArtifactPropertyWebhook": "ArtifactPropertyWebhook"
   }
  },
  {
@@ -350,14 +373,22 @@
   "fqn": "pulumi_artifactory",
   "classes": {
    "artifactory:index/artifactWebhook:ArtifactWebhook": "ArtifactWebhook"
   }
  },
  {
   "pkg": "artifactory",
+  "mod": "index/artifactoryReleaseBundleCustomWebhook",
+  "fqn": "pulumi_artifactory",
+  "classes": {
+   "artifactory:index/artifactoryReleaseBundleCustomWebhook:ArtifactoryReleaseBundleCustomWebhook": "ArtifactoryReleaseBundleCustomWebhook"
+  }
+ },
+ {
+  "pkg": "artifactory",
   "mod": "index/artifactoryReleaseBundleWebhook",
   "fqn": "pulumi_artifactory",
   "classes": {
    "artifactory:index/artifactoryReleaseBundleWebhook:ArtifactoryReleaseBundleWebhook": "ArtifactoryReleaseBundleWebhook"
   }
  },
  {
@@ -366,14 +397,22 @@
   "fqn": "pulumi_artifactory",
   "classes": {
    "artifactory:index/backup:Backup": "Backup"
   }
  },
  {
   "pkg": "artifactory",
+  "mod": "index/buildCustomWebhook",
+  "fqn": "pulumi_artifactory",
+  "classes": {
+   "artifactory:index/buildCustomWebhook:BuildCustomWebhook": "BuildCustomWebhook"
+  }
+ },
+ {
+  "pkg": "artifactory",
   "mod": "index/buildWebhook",
   "fqn": "pulumi_artifactory",
   "classes": {
    "artifactory:index/buildWebhook:BuildWebhook": "BuildWebhook"
   }
  },
  {
@@ -390,14 +429,22 @@
   "fqn": "pulumi_artifactory",
   "classes": {
    "artifactory:index/debianRepository:DebianRepository": "DebianRepository"
   }
  },
  {
   "pkg": "artifactory",
+  "mod": "index/distributionCustomWebhook",
+  "fqn": "pulumi_artifactory",
+  "classes": {
+   "artifactory:index/distributionCustomWebhook:DistributionCustomWebhook": "DistributionCustomWebhook"
+  }
+ },
+ {
+  "pkg": "artifactory",
   "mod": "index/distributionPublicKey",
   "fqn": "pulumi_artifactory",
   "classes": {
    "artifactory:index/distributionPublicKey:DistributionPublicKey": "DistributionPublicKey"
   }
  },
  {
@@ -406,14 +453,22 @@
   "fqn": "pulumi_artifactory",
   "classes": {
    "artifactory:index/distributionWebhook:DistributionWebhook": "DistributionWebhook"
   }
  },
  {
   "pkg": "artifactory",
+  "mod": "index/dockerCustomWebhook",
+  "fqn": "pulumi_artifactory",
+  "classes": {
+   "artifactory:index/dockerCustomWebhook:DockerCustomWebhook": "DockerCustomWebhook"
+  }
+ },
+ {
+  "pkg": "artifactory",
   "mod": "index/dockerV1Repository",
   "fqn": "pulumi_artifactory",
   "classes": {
    "artifactory:index/dockerV1Repository:DockerV1Repository": "DockerV1Repository"
   }
  },
  {
@@ -1046,14 +1101,22 @@
   "fqn": "pulumi_artifactory",
   "classes": {
    "artifactory:index/pushReplication:PushReplication": "PushReplication"
   }
  },
  {
   "pkg": "artifactory",
+  "mod": "index/releaseBundleCustomWebhook",
+  "fqn": "pulumi_artifactory",
+  "classes": {
+   "artifactory:index/releaseBundleCustomWebhook:ReleaseBundleCustomWebhook": "ReleaseBundleCustomWebhook"
+  }
+ },
+ {
+  "pkg": "artifactory",
   "mod": "index/releaseBundleWebhook",
   "fqn": "pulumi_artifactory",
   "classes": {
    "artifactory:index/releaseBundleWebhook:ReleaseBundleWebhook": "ReleaseBundleWebhook"
   }
  },
  {
```

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/_inputs.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/_inputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,24 +7,36 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
     'AccessTokenAdminTokenArgs',
+    'ArtifactCustomWebhookCriteriaArgs',
+    'ArtifactCustomWebhookHandlerArgs',
+    'ArtifactPropertyCustomWebhookCriteriaArgs',
+    'ArtifactPropertyCustomWebhookHandlerArgs',
     'ArtifactPropertyWebhookCriteriaArgs',
     'ArtifactPropertyWebhookHandlerArgs',
     'ArtifactWebhookCriteriaArgs',
     'ArtifactWebhookHandlerArgs',
+    'ArtifactoryReleaseBundleCustomWebhookCriteriaArgs',
+    'ArtifactoryReleaseBundleCustomWebhookHandlerArgs',
     'ArtifactoryReleaseBundleWebhookCriteriaArgs',
     'ArtifactoryReleaseBundleWebhookHandlerArgs',
+    'BuildCustomWebhookCriteriaArgs',
+    'BuildCustomWebhookHandlerArgs',
     'BuildWebhookCriteriaArgs',
     'BuildWebhookHandlerArgs',
+    'DistributionCustomWebhookCriteriaArgs',
+    'DistributionCustomWebhookHandlerArgs',
     'DistributionWebhookCriteriaArgs',
     'DistributionWebhookHandlerArgs',
+    'DockerCustomWebhookCriteriaArgs',
+    'DockerCustomWebhookHandlerArgs',
     'DockerWebhookCriteriaArgs',
     'DockerWebhookHandlerArgs',
     'FederatedAlpineRepositoryMemberArgs',
     'FederatedBowerRepositoryMemberArgs',
     'FederatedCargoRepositoryMemberArgs',
     'FederatedChefRepositoryMemberArgs',
     'FederatedCocoapodsRepositoryMemberArgs',
@@ -68,14 +80,16 @@
     'PermissionTargetRepoArgs',
     'PermissionTargetRepoActionArgs',
     'PermissionTargetRepoActionGroupArgs',
     'PermissionTargetRepoActionUserArgs',
     'PropertySetPropertyArgs',
     'PropertySetPropertyPredefinedValueArgs',
     'PushReplicationReplicationArgs',
+    'ReleaseBundleCustomWebhookCriteriaArgs',
+    'ReleaseBundleCustomWebhookHandlerArgs',
     'ReleaseBundleWebhookCriteriaArgs',
     'ReleaseBundleWebhookHandlerArgs',
     'RemoteAlpineRepositoryContentSynchronisationArgs',
     'RemoteBowerRepositoryContentSynchronisationArgs',
     'RemoteCargoRepositoryContentSynchronisationArgs',
     'RemoteChefRepositoryContentSynchronisationArgs',
     'RemoteCocoapodsRepositoryContentSynchronisationArgs',
@@ -196,14 +210,362 @@
 
     @instance_id.setter
     def instance_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "instance_id", value)
 
 
 @pulumi.input_type
+class ArtifactCustomWebhookCriteriaArgs:
+    def __init__(__self__, *,
+                 any_local: pulumi.Input[bool],
+                 any_remote: pulumi.Input[bool],
+                 repo_keys: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 exclude_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 include_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[bool] any_local: Trigger on any local repo.
+        :param pulumi.Input[bool] any_remote: Trigger on any remote repo.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] repo_keys: Trigger on this list of repo keys.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] exclude_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] include_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        pulumi.set(__self__, "any_local", any_local)
+        pulumi.set(__self__, "any_remote", any_remote)
+        pulumi.set(__self__, "repo_keys", repo_keys)
+        if exclude_patterns is not None:
+            pulumi.set(__self__, "exclude_patterns", exclude_patterns)
+        if include_patterns is not None:
+            pulumi.set(__self__, "include_patterns", include_patterns)
+
+    @property
+    @pulumi.getter(name="anyLocal")
+    def any_local(self) -> pulumi.Input[bool]:
+        """
+        Trigger on any local repo.
+        """
+        return pulumi.get(self, "any_local")
+
+    @any_local.setter
+    def any_local(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "any_local", value)
+
+    @property
+    @pulumi.getter(name="anyRemote")
+    def any_remote(self) -> pulumi.Input[bool]:
+        """
+        Trigger on any remote repo.
+        """
+        return pulumi.get(self, "any_remote")
+
+    @any_remote.setter
+    def any_remote(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "any_remote", value)
+
+    @property
+    @pulumi.getter(name="repoKeys")
+    def repo_keys(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+        """
+        Trigger on this list of repo keys.
+        """
+        return pulumi.get(self, "repo_keys")
+
+    @repo_keys.setter
+    def repo_keys(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "repo_keys", value)
+
+    @property
+    @pulumi.getter(name="excludePatterns")
+    def exclude_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        return pulumi.get(self, "exclude_patterns")
+
+    @exclude_patterns.setter
+    def exclude_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "exclude_patterns", value)
+
+    @property
+    @pulumi.getter(name="includePatterns")
+    def include_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        return pulumi.get(self, "include_patterns")
+
+    @include_patterns.setter
+    def include_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "include_patterns", value)
+
+
+@pulumi.input_type
+class ArtifactCustomWebhookHandlerArgs:
+    def __init__(__self__, *,
+                 url: pulumi.Input[str],
+                 http_headers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 payload: Optional[pulumi.Input[str]] = None,
+                 proxy: Optional[pulumi.Input[str]] = None,
+                 secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[str] url: Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] http_headers: HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        :param pulumi.Input[str] proxy: Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example: 
+               
+               ```python
+               import pulumi
+               ```
+        """
+        pulumi.set(__self__, "url", url)
+        if http_headers is not None:
+            pulumi.set(__self__, "http_headers", http_headers)
+        if payload is not None:
+            pulumi.set(__self__, "payload", payload)
+        if proxy is not None:
+            pulumi.set(__self__, "proxy", proxy)
+        if secrets is not None:
+            pulumi.set(__self__, "secrets", secrets)
+
+    @property
+    @pulumi.getter
+    def url(self) -> pulumi.Input[str]:
+        """
+        Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        """
+        return pulumi.get(self, "url")
+
+    @url.setter
+    def url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "url", value)
+
+    @property
+    @pulumi.getter(name="httpHeaders")
+    def http_headers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        """
+        return pulumi.get(self, "http_headers")
+
+    @http_headers.setter
+    def http_headers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "http_headers", value)
+
+    @property
+    @pulumi.getter
+    def payload(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "payload")
+
+    @payload.setter
+    def payload(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "payload", value)
+
+    @property
+    @pulumi.getter
+    def proxy(self) -> Optional[pulumi.Input[str]]:
+        """
+        Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        """
+        return pulumi.get(self, "proxy")
+
+    @proxy.setter
+    def proxy(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "proxy", value)
+
+    @property
+    @pulumi.getter
+    def secrets(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example: 
+
+        ```python
+        import pulumi
+        ```
+        """
+        return pulumi.get(self, "secrets")
+
+    @secrets.setter
+    def secrets(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "secrets", value)
+
+
+@pulumi.input_type
+class ArtifactPropertyCustomWebhookCriteriaArgs:
+    def __init__(__self__, *,
+                 any_local: pulumi.Input[bool],
+                 any_remote: pulumi.Input[bool],
+                 repo_keys: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 exclude_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 include_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[bool] any_local: Trigger on any local repo.
+        :param pulumi.Input[bool] any_remote: Trigger on any remote repo.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] repo_keys: Trigger on this list of repo keys.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] exclude_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] include_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        pulumi.set(__self__, "any_local", any_local)
+        pulumi.set(__self__, "any_remote", any_remote)
+        pulumi.set(__self__, "repo_keys", repo_keys)
+        if exclude_patterns is not None:
+            pulumi.set(__self__, "exclude_patterns", exclude_patterns)
+        if include_patterns is not None:
+            pulumi.set(__self__, "include_patterns", include_patterns)
+
+    @property
+    @pulumi.getter(name="anyLocal")
+    def any_local(self) -> pulumi.Input[bool]:
+        """
+        Trigger on any local repo.
+        """
+        return pulumi.get(self, "any_local")
+
+    @any_local.setter
+    def any_local(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "any_local", value)
+
+    @property
+    @pulumi.getter(name="anyRemote")
+    def any_remote(self) -> pulumi.Input[bool]:
+        """
+        Trigger on any remote repo.
+        """
+        return pulumi.get(self, "any_remote")
+
+    @any_remote.setter
+    def any_remote(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "any_remote", value)
+
+    @property
+    @pulumi.getter(name="repoKeys")
+    def repo_keys(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+        """
+        Trigger on this list of repo keys.
+        """
+        return pulumi.get(self, "repo_keys")
+
+    @repo_keys.setter
+    def repo_keys(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "repo_keys", value)
+
+    @property
+    @pulumi.getter(name="excludePatterns")
+    def exclude_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        return pulumi.get(self, "exclude_patterns")
+
+    @exclude_patterns.setter
+    def exclude_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "exclude_patterns", value)
+
+    @property
+    @pulumi.getter(name="includePatterns")
+    def include_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        return pulumi.get(self, "include_patterns")
+
+    @include_patterns.setter
+    def include_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "include_patterns", value)
+
+
+@pulumi.input_type
+class ArtifactPropertyCustomWebhookHandlerArgs:
+    def __init__(__self__, *,
+                 url: pulumi.Input[str],
+                 http_headers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 payload: Optional[pulumi.Input[str]] = None,
+                 proxy: Optional[pulumi.Input[str]] = None,
+                 secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[str] url: Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] http_headers: HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        :param pulumi.Input[str] proxy: Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+               
+               ```python
+               import pulumi
+               ```
+        """
+        pulumi.set(__self__, "url", url)
+        if http_headers is not None:
+            pulumi.set(__self__, "http_headers", http_headers)
+        if payload is not None:
+            pulumi.set(__self__, "payload", payload)
+        if proxy is not None:
+            pulumi.set(__self__, "proxy", proxy)
+        if secrets is not None:
+            pulumi.set(__self__, "secrets", secrets)
+
+    @property
+    @pulumi.getter
+    def url(self) -> pulumi.Input[str]:
+        """
+        Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        """
+        return pulumi.get(self, "url")
+
+    @url.setter
+    def url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "url", value)
+
+    @property
+    @pulumi.getter(name="httpHeaders")
+    def http_headers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        """
+        return pulumi.get(self, "http_headers")
+
+    @http_headers.setter
+    def http_headers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "http_headers", value)
+
+    @property
+    @pulumi.getter
+    def payload(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "payload")
+
+    @payload.setter
+    def payload(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "payload", value)
+
+    @property
+    @pulumi.getter
+    def proxy(self) -> Optional[pulumi.Input[str]]:
+        """
+        Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        """
+        return pulumi.get(self, "proxy")
+
+    @proxy.setter
+    def proxy(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "proxy", value)
+
+    @property
+    @pulumi.getter
+    def secrets(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+
+        ```python
+        import pulumi
+        ```
+        """
+        return pulumi.get(self, "secrets")
+
+    @secrets.setter
+    def secrets(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "secrets", value)
+
+
+@pulumi.input_type
 class ArtifactPropertyWebhookCriteriaArgs:
     def __init__(__self__, *,
                  any_local: pulumi.Input[bool],
                  any_remote: pulumi.Input[bool],
                  repo_keys: pulumi.Input[Sequence[pulumi.Input[str]]],
                  exclude_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  include_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
@@ -504,14 +866,173 @@
 
     @secret.setter
     def secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret", value)
 
 
 @pulumi.input_type
+class ArtifactoryReleaseBundleCustomWebhookCriteriaArgs:
+    def __init__(__self__, *,
+                 any_release_bundle: pulumi.Input[bool],
+                 registered_release_bundle_names: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 exclude_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 include_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[bool] any_release_bundle: Trigger on any release bundle
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] registered_release_bundle_names: Trigger on this list of release bundle names
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] exclude_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] include_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`
+        """
+        pulumi.set(__self__, "any_release_bundle", any_release_bundle)
+        pulumi.set(__self__, "registered_release_bundle_names", registered_release_bundle_names)
+        if exclude_patterns is not None:
+            pulumi.set(__self__, "exclude_patterns", exclude_patterns)
+        if include_patterns is not None:
+            pulumi.set(__self__, "include_patterns", include_patterns)
+
+    @property
+    @pulumi.getter(name="anyReleaseBundle")
+    def any_release_bundle(self) -> pulumi.Input[bool]:
+        """
+        Trigger on any release bundle
+        """
+        return pulumi.get(self, "any_release_bundle")
+
+    @any_release_bundle.setter
+    def any_release_bundle(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "any_release_bundle", value)
+
+    @property
+    @pulumi.getter(name="registeredReleaseBundleNames")
+    def registered_release_bundle_names(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+        """
+        Trigger on this list of release bundle names
+        """
+        return pulumi.get(self, "registered_release_bundle_names")
+
+    @registered_release_bundle_names.setter
+    def registered_release_bundle_names(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "registered_release_bundle_names", value)
+
+    @property
+    @pulumi.getter(name="excludePatterns")
+    def exclude_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`
+        """
+        return pulumi.get(self, "exclude_patterns")
+
+    @exclude_patterns.setter
+    def exclude_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "exclude_patterns", value)
+
+    @property
+    @pulumi.getter(name="includePatterns")
+    def include_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`
+        """
+        return pulumi.get(self, "include_patterns")
+
+    @include_patterns.setter
+    def include_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "include_patterns", value)
+
+
+@pulumi.input_type
+class ArtifactoryReleaseBundleCustomWebhookHandlerArgs:
+    def __init__(__self__, *,
+                 url: pulumi.Input[str],
+                 http_headers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 payload: Optional[pulumi.Input[str]] = None,
+                 proxy: Optional[pulumi.Input[str]] = None,
+                 secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[str] url: Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] http_headers: HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        :param pulumi.Input[str] proxy: Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+               
+               ```python
+               import pulumi
+               ```
+        """
+        pulumi.set(__self__, "url", url)
+        if http_headers is not None:
+            pulumi.set(__self__, "http_headers", http_headers)
+        if payload is not None:
+            pulumi.set(__self__, "payload", payload)
+        if proxy is not None:
+            pulumi.set(__self__, "proxy", proxy)
+        if secrets is not None:
+            pulumi.set(__self__, "secrets", secrets)
+
+    @property
+    @pulumi.getter
+    def url(self) -> pulumi.Input[str]:
+        """
+        Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        """
+        return pulumi.get(self, "url")
+
+    @url.setter
+    def url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "url", value)
+
+    @property
+    @pulumi.getter(name="httpHeaders")
+    def http_headers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        """
+        return pulumi.get(self, "http_headers")
+
+    @http_headers.setter
+    def http_headers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "http_headers", value)
+
+    @property
+    @pulumi.getter
+    def payload(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "payload")
+
+    @payload.setter
+    def payload(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "payload", value)
+
+    @property
+    @pulumi.getter
+    def proxy(self) -> Optional[pulumi.Input[str]]:
+        """
+        Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        """
+        return pulumi.get(self, "proxy")
+
+    @proxy.setter
+    def proxy(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "proxy", value)
+
+    @property
+    @pulumi.getter
+    def secrets(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+
+        ```python
+        import pulumi
+        ```
+        """
+        return pulumi.get(self, "secrets")
+
+    @secrets.setter
+    def secrets(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "secrets", value)
+
+
+@pulumi.input_type
 class ArtifactoryReleaseBundleWebhookCriteriaArgs:
     def __init__(__self__, *,
                  any_release_bundle: pulumi.Input[bool],
                  registered_release_bundle_names: pulumi.Input[Sequence[pulumi.Input[str]]],
                  exclude_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  include_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
@@ -643,14 +1164,173 @@
 
     @secret.setter
     def secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret", value)
 
 
 @pulumi.input_type
+class BuildCustomWebhookCriteriaArgs:
+    def __init__(__self__, *,
+                 any_build: pulumi.Input[bool],
+                 selected_builds: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 exclude_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 include_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[bool] any_build: Trigger on any build.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] selected_builds: Trigger on this list of build names.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] exclude_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] include_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        pulumi.set(__self__, "any_build", any_build)
+        pulumi.set(__self__, "selected_builds", selected_builds)
+        if exclude_patterns is not None:
+            pulumi.set(__self__, "exclude_patterns", exclude_patterns)
+        if include_patterns is not None:
+            pulumi.set(__self__, "include_patterns", include_patterns)
+
+    @property
+    @pulumi.getter(name="anyBuild")
+    def any_build(self) -> pulumi.Input[bool]:
+        """
+        Trigger on any build.
+        """
+        return pulumi.get(self, "any_build")
+
+    @any_build.setter
+    def any_build(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "any_build", value)
+
+    @property
+    @pulumi.getter(name="selectedBuilds")
+    def selected_builds(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+        """
+        Trigger on this list of build names.
+        """
+        return pulumi.get(self, "selected_builds")
+
+    @selected_builds.setter
+    def selected_builds(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "selected_builds", value)
+
+    @property
+    @pulumi.getter(name="excludePatterns")
+    def exclude_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        return pulumi.get(self, "exclude_patterns")
+
+    @exclude_patterns.setter
+    def exclude_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "exclude_patterns", value)
+
+    @property
+    @pulumi.getter(name="includePatterns")
+    def include_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        return pulumi.get(self, "include_patterns")
+
+    @include_patterns.setter
+    def include_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "include_patterns", value)
+
+
+@pulumi.input_type
+class BuildCustomWebhookHandlerArgs:
+    def __init__(__self__, *,
+                 url: pulumi.Input[str],
+                 http_headers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 payload: Optional[pulumi.Input[str]] = None,
+                 proxy: Optional[pulumi.Input[str]] = None,
+                 secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[str] url: Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] http_headers: HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        :param pulumi.Input[str] proxy: Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+               
+               ```python
+               import pulumi
+               ```
+        """
+        pulumi.set(__self__, "url", url)
+        if http_headers is not None:
+            pulumi.set(__self__, "http_headers", http_headers)
+        if payload is not None:
+            pulumi.set(__self__, "payload", payload)
+        if proxy is not None:
+            pulumi.set(__self__, "proxy", proxy)
+        if secrets is not None:
+            pulumi.set(__self__, "secrets", secrets)
+
+    @property
+    @pulumi.getter
+    def url(self) -> pulumi.Input[str]:
+        """
+        Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        """
+        return pulumi.get(self, "url")
+
+    @url.setter
+    def url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "url", value)
+
+    @property
+    @pulumi.getter(name="httpHeaders")
+    def http_headers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        """
+        return pulumi.get(self, "http_headers")
+
+    @http_headers.setter
+    def http_headers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "http_headers", value)
+
+    @property
+    @pulumi.getter
+    def payload(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "payload")
+
+    @payload.setter
+    def payload(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "payload", value)
+
+    @property
+    @pulumi.getter
+    def proxy(self) -> Optional[pulumi.Input[str]]:
+        """
+        Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        """
+        return pulumi.get(self, "proxy")
+
+    @proxy.setter
+    def proxy(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "proxy", value)
+
+    @property
+    @pulumi.getter
+    def secrets(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+
+        ```python
+        import pulumi
+        ```
+        """
+        return pulumi.get(self, "secrets")
+
+    @secrets.setter
+    def secrets(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "secrets", value)
+
+
+@pulumi.input_type
 class BuildWebhookCriteriaArgs:
     def __init__(__self__, *,
                  any_build: pulumi.Input[bool],
                  selected_builds: pulumi.Input[Sequence[pulumi.Input[str]]],
                  exclude_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  include_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
@@ -782,14 +1462,173 @@
 
     @secret.setter
     def secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret", value)
 
 
 @pulumi.input_type
+class DistributionCustomWebhookCriteriaArgs:
+    def __init__(__self__, *,
+                 any_release_bundle: pulumi.Input[bool],
+                 registered_release_bundle_names: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 exclude_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 include_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[bool] any_release_bundle: Trigger on any release bundle.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] registered_release_bundle_names: Trigger on this list of release bundle names.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] exclude_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] include_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        pulumi.set(__self__, "any_release_bundle", any_release_bundle)
+        pulumi.set(__self__, "registered_release_bundle_names", registered_release_bundle_names)
+        if exclude_patterns is not None:
+            pulumi.set(__self__, "exclude_patterns", exclude_patterns)
+        if include_patterns is not None:
+            pulumi.set(__self__, "include_patterns", include_patterns)
+
+    @property
+    @pulumi.getter(name="anyReleaseBundle")
+    def any_release_bundle(self) -> pulumi.Input[bool]:
+        """
+        Trigger on any release bundle.
+        """
+        return pulumi.get(self, "any_release_bundle")
+
+    @any_release_bundle.setter
+    def any_release_bundle(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "any_release_bundle", value)
+
+    @property
+    @pulumi.getter(name="registeredReleaseBundleNames")
+    def registered_release_bundle_names(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+        """
+        Trigger on this list of release bundle names.
+        """
+        return pulumi.get(self, "registered_release_bundle_names")
+
+    @registered_release_bundle_names.setter
+    def registered_release_bundle_names(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "registered_release_bundle_names", value)
+
+    @property
+    @pulumi.getter(name="excludePatterns")
+    def exclude_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        return pulumi.get(self, "exclude_patterns")
+
+    @exclude_patterns.setter
+    def exclude_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "exclude_patterns", value)
+
+    @property
+    @pulumi.getter(name="includePatterns")
+    def include_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        return pulumi.get(self, "include_patterns")
+
+    @include_patterns.setter
+    def include_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "include_patterns", value)
+
+
+@pulumi.input_type
+class DistributionCustomWebhookHandlerArgs:
+    def __init__(__self__, *,
+                 url: pulumi.Input[str],
+                 http_headers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 payload: Optional[pulumi.Input[str]] = None,
+                 proxy: Optional[pulumi.Input[str]] = None,
+                 secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[str] url: Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] http_headers: HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        :param pulumi.Input[str] proxy: Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+               
+               ```python
+               import pulumi
+               ```
+        """
+        pulumi.set(__self__, "url", url)
+        if http_headers is not None:
+            pulumi.set(__self__, "http_headers", http_headers)
+        if payload is not None:
+            pulumi.set(__self__, "payload", payload)
+        if proxy is not None:
+            pulumi.set(__self__, "proxy", proxy)
+        if secrets is not None:
+            pulumi.set(__self__, "secrets", secrets)
+
+    @property
+    @pulumi.getter
+    def url(self) -> pulumi.Input[str]:
+        """
+        Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        """
+        return pulumi.get(self, "url")
+
+    @url.setter
+    def url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "url", value)
+
+    @property
+    @pulumi.getter(name="httpHeaders")
+    def http_headers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        """
+        return pulumi.get(self, "http_headers")
+
+    @http_headers.setter
+    def http_headers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "http_headers", value)
+
+    @property
+    @pulumi.getter
+    def payload(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "payload")
+
+    @payload.setter
+    def payload(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "payload", value)
+
+    @property
+    @pulumi.getter
+    def proxy(self) -> Optional[pulumi.Input[str]]:
+        """
+        Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        """
+        return pulumi.get(self, "proxy")
+
+    @proxy.setter
+    def proxy(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "proxy", value)
+
+    @property
+    @pulumi.getter
+    def secrets(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+
+        ```python
+        import pulumi
+        ```
+        """
+        return pulumi.get(self, "secrets")
+
+    @secrets.setter
+    def secrets(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "secrets", value)
+
+
+@pulumi.input_type
 class DistributionWebhookCriteriaArgs:
     def __init__(__self__, *,
                  any_release_bundle: pulumi.Input[bool],
                  registered_release_bundle_names: pulumi.Input[Sequence[pulumi.Input[str]]],
                  exclude_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  include_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
@@ -921,14 +1760,188 @@
 
     @secret.setter
     def secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret", value)
 
 
 @pulumi.input_type
+class DockerCustomWebhookCriteriaArgs:
+    def __init__(__self__, *,
+                 any_local: pulumi.Input[bool],
+                 any_remote: pulumi.Input[bool],
+                 repo_keys: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 exclude_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 include_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[bool] any_local: Trigger on any local repo.
+        :param pulumi.Input[bool] any_remote: Trigger on any remote repo.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] repo_keys: Trigger on this list of repo keys.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] exclude_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] include_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        pulumi.set(__self__, "any_local", any_local)
+        pulumi.set(__self__, "any_remote", any_remote)
+        pulumi.set(__self__, "repo_keys", repo_keys)
+        if exclude_patterns is not None:
+            pulumi.set(__self__, "exclude_patterns", exclude_patterns)
+        if include_patterns is not None:
+            pulumi.set(__self__, "include_patterns", include_patterns)
+
+    @property
+    @pulumi.getter(name="anyLocal")
+    def any_local(self) -> pulumi.Input[bool]:
+        """
+        Trigger on any local repo.
+        """
+        return pulumi.get(self, "any_local")
+
+    @any_local.setter
+    def any_local(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "any_local", value)
+
+    @property
+    @pulumi.getter(name="anyRemote")
+    def any_remote(self) -> pulumi.Input[bool]:
+        """
+        Trigger on any remote repo.
+        """
+        return pulumi.get(self, "any_remote")
+
+    @any_remote.setter
+    def any_remote(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "any_remote", value)
+
+    @property
+    @pulumi.getter(name="repoKeys")
+    def repo_keys(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+        """
+        Trigger on this list of repo keys.
+        """
+        return pulumi.get(self, "repo_keys")
+
+    @repo_keys.setter
+    def repo_keys(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "repo_keys", value)
+
+    @property
+    @pulumi.getter(name="excludePatterns")
+    def exclude_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        return pulumi.get(self, "exclude_patterns")
+
+    @exclude_patterns.setter
+    def exclude_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "exclude_patterns", value)
+
+    @property
+    @pulumi.getter(name="includePatterns")
+    def include_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        return pulumi.get(self, "include_patterns")
+
+    @include_patterns.setter
+    def include_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "include_patterns", value)
+
+
+@pulumi.input_type
+class DockerCustomWebhookHandlerArgs:
+    def __init__(__self__, *,
+                 url: pulumi.Input[str],
+                 http_headers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 payload: Optional[pulumi.Input[str]] = None,
+                 proxy: Optional[pulumi.Input[str]] = None,
+                 secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[str] url: Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] http_headers: HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        :param pulumi.Input[str] proxy: Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+               
+               ```python
+               import pulumi
+               ```
+        """
+        pulumi.set(__self__, "url", url)
+        if http_headers is not None:
+            pulumi.set(__self__, "http_headers", http_headers)
+        if payload is not None:
+            pulumi.set(__self__, "payload", payload)
+        if proxy is not None:
+            pulumi.set(__self__, "proxy", proxy)
+        if secrets is not None:
+            pulumi.set(__self__, "secrets", secrets)
+
+    @property
+    @pulumi.getter
+    def url(self) -> pulumi.Input[str]:
+        """
+        Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        """
+        return pulumi.get(self, "url")
+
+    @url.setter
+    def url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "url", value)
+
+    @property
+    @pulumi.getter(name="httpHeaders")
+    def http_headers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        """
+        return pulumi.get(self, "http_headers")
+
+    @http_headers.setter
+    def http_headers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "http_headers", value)
+
+    @property
+    @pulumi.getter
+    def payload(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "payload")
+
+    @payload.setter
+    def payload(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "payload", value)
+
+    @property
+    @pulumi.getter
+    def proxy(self) -> Optional[pulumi.Input[str]]:
+        """
+        Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        """
+        return pulumi.get(self, "proxy")
+
+    @proxy.setter
+    def proxy(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "proxy", value)
+
+    @property
+    @pulumi.getter
+    def secrets(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+
+        ```python
+        import pulumi
+        ```
+        """
+        return pulumi.get(self, "secrets")
+
+    @secrets.setter
+    def secrets(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "secrets", value)
+
+
+@pulumi.input_type
 class DockerWebhookCriteriaArgs:
     def __init__(__self__, *,
                  any_local: pulumi.Input[bool],
                  any_remote: pulumi.Input[bool],
                  repo_keys: pulumi.Input[Sequence[pulumi.Input[str]]],
                  exclude_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  include_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
@@ -3467,14 +4480,173 @@
 
     @sync_statistics.setter
     def sync_statistics(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "sync_statistics", value)
 
 
 @pulumi.input_type
+class ReleaseBundleCustomWebhookCriteriaArgs:
+    def __init__(__self__, *,
+                 any_release_bundle: pulumi.Input[bool],
+                 registered_release_bundle_names: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 exclude_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 include_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[bool] any_release_bundle: Trigger on any release bundle.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] registered_release_bundle_names: Trigger on this list of release bundle names.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] exclude_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: "org/apache/**".
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] include_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: "org/apache/**".
+        """
+        pulumi.set(__self__, "any_release_bundle", any_release_bundle)
+        pulumi.set(__self__, "registered_release_bundle_names", registered_release_bundle_names)
+        if exclude_patterns is not None:
+            pulumi.set(__self__, "exclude_patterns", exclude_patterns)
+        if include_patterns is not None:
+            pulumi.set(__self__, "include_patterns", include_patterns)
+
+    @property
+    @pulumi.getter(name="anyReleaseBundle")
+    def any_release_bundle(self) -> pulumi.Input[bool]:
+        """
+        Trigger on any release bundle.
+        """
+        return pulumi.get(self, "any_release_bundle")
+
+    @any_release_bundle.setter
+    def any_release_bundle(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "any_release_bundle", value)
+
+    @property
+    @pulumi.getter(name="registeredReleaseBundleNames")
+    def registered_release_bundle_names(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+        """
+        Trigger on this list of release bundle names.
+        """
+        return pulumi.get(self, "registered_release_bundle_names")
+
+    @registered_release_bundle_names.setter
+    def registered_release_bundle_names(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "registered_release_bundle_names", value)
+
+    @property
+    @pulumi.getter(name="excludePatterns")
+    def exclude_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: "org/apache/**".
+        """
+        return pulumi.get(self, "exclude_patterns")
+
+    @exclude_patterns.setter
+    def exclude_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "exclude_patterns", value)
+
+    @property
+    @pulumi.getter(name="includePatterns")
+    def include_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: "org/apache/**".
+        """
+        return pulumi.get(self, "include_patterns")
+
+    @include_patterns.setter
+    def include_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "include_patterns", value)
+
+
+@pulumi.input_type
+class ReleaseBundleCustomWebhookHandlerArgs:
+    def __init__(__self__, *,
+                 url: pulumi.Input[str],
+                 http_headers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 payload: Optional[pulumi.Input[str]] = None,
+                 proxy: Optional[pulumi.Input[str]] = None,
+                 secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[str] url: Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] http_headers: HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        :param pulumi.Input[str] proxy: Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+               
+               ```python
+               import pulumi
+               ```
+        """
+        pulumi.set(__self__, "url", url)
+        if http_headers is not None:
+            pulumi.set(__self__, "http_headers", http_headers)
+        if payload is not None:
+            pulumi.set(__self__, "payload", payload)
+        if proxy is not None:
+            pulumi.set(__self__, "proxy", proxy)
+        if secrets is not None:
+            pulumi.set(__self__, "secrets", secrets)
+
+    @property
+    @pulumi.getter
+    def url(self) -> pulumi.Input[str]:
+        """
+        Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        """
+        return pulumi.get(self, "url")
+
+    @url.setter
+    def url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "url", value)
+
+    @property
+    @pulumi.getter(name="httpHeaders")
+    def http_headers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        """
+        return pulumi.get(self, "http_headers")
+
+    @http_headers.setter
+    def http_headers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "http_headers", value)
+
+    @property
+    @pulumi.getter
+    def payload(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "payload")
+
+    @payload.setter
+    def payload(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "payload", value)
+
+    @property
+    @pulumi.getter
+    def proxy(self) -> Optional[pulumi.Input[str]]:
+        """
+        Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        """
+        return pulumi.get(self, "proxy")
+
+    @proxy.setter
+    def proxy(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "proxy", value)
+
+    @property
+    @pulumi.getter
+    def secrets(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+
+        ```python
+        import pulumi
+        ```
+        """
+        return pulumi.get(self, "secrets")
+
+    @secrets.setter
+    def secrets(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "secrets", value)
+
+
+@pulumi.input_type
 class ReleaseBundleWebhookCriteriaArgs:
     def __init__(__self__, *,
                  any_release_bundle: pulumi.Input[bool],
                  registered_release_bundle_names: pulumi.Input[Sequence[pulumi.Input[str]]],
                  exclude_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  include_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/_utilities.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/access_token.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/alpine_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/anonymous_user.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/anonymous_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/api_key.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/artifact_property_webhook.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/artifact_property_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/artifact_webhook.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/artifact_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/artifactory_release_bundle_webhook.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/artifactory_release_bundle_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/backup.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/build_webhook.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/build_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/certificate.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/config/vars.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/debian_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/distribution_public_key.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/distribution_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/distribution_webhook.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/distribution_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/docker_v1_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/docker_v2_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/docker_webhook.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/docker_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_alpine_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_bower_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_cargo_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_chef_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_cocoapods_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_composer_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_conan_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_conda_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_cran_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_debian_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_docker_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_docker_v1_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_docker_v2_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_gems_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_generic_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_gitltfs_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_gitltfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_go_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_gradle_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_helm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_ivy_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_maven_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_npm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_nuget_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_opkg_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_puppet_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_pypi_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_rpm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_sbt_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_swift_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_terraform_module_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_terraform_provider_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/federated_vagrant_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/federated_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/general_security.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/general_security.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_alpine_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_bower_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_cargo_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_chef_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_cocoapods_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_composer_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_conan_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_conda_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_cran_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_debian_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_docker_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_docker_v1_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_docker_v2_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_gems_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_generic_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_gitlfs_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_go_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_gradle_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_helm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_ivy_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_maven_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_npm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_nuget_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_opkg_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_puppet_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_pypi_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_rpm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_sbt_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_swift_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_terraform_module_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_terraform_provider_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_federated_vagrant_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_federated_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_file.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_fileinfo.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_fileinfo.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_group.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_alpine_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_bower_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_cargo_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_chef_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_cocoapods_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_composer_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_conan_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_conda_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_cran_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_debian_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_docker_v1_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_docker_v2_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_gems_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_generic_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_gitlfs_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_go_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_gradle_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_helm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_ivy_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_maven_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_npm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_nuget_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_opkg_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_pub_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_puppet_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_pypi_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_rpm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_sbt_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_swift_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_terraform_module_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_terraform_provider_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_terraformbackend_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_terraformbackend_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_local_vagrant_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_local_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_permission_target.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_permission_target.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_alpine_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_bower_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_cargo_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_chef_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_cocoapods_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_composer_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_conan_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_conda_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_cran_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_debian_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_docker_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_gems_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_generic_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_gitlfs_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_go_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_gradle_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_helm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_ivy_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_maven_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_npm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_nuget_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_opkg_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_p2_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_pub_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_puppet_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_pypi_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_rpm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_sbt_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_swift_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_terraform_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_remote_vcs_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_remote_vcs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_user.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_alpine_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_bower_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_chef_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_composer_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_conan_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_conda_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_cran_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_debian_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_docker_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_gems_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_generic_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_gitlfs_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_go_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_gradle_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_helm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_ivy_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_npm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_nuget_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_p2_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_pub_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_puppet_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_pypi_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_rpm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_sbt_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_swift_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/get_virtual_terraform_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/get_virtual_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/go_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/group.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/keypair.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/keypair.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/ldap_group_setting.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/ldap_group_setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/ldap_setting.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/ldap_setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_bower_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_cargo_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_chef_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_cocoapods_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_composer_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_conan_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_conda_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_cran_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_gems_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_generic_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_gitltfs_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_gitltfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_go_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_gradle_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_helm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_ivy_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_maven_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_npm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_nuget_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_opkg_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_pub_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_puppet_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_pypi_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_repository_multi_replication.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_repository_multi_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_repository_single_replication.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_repository_single_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_rpm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_sbt_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_swift_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_terraform_backend_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_terraform_backend_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_terraform_module_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_terraform_provider_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/local_vagrant_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/local_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/managed_user.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/managed_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/maven_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/oauth_settings.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/oauth_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/outputs.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/outputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,24 +8,36 @@
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
 __all__ = [
     'AccessTokenAdminToken',
+    'ArtifactCustomWebhookCriteria',
+    'ArtifactCustomWebhookHandler',
+    'ArtifactPropertyCustomWebhookCriteria',
+    'ArtifactPropertyCustomWebhookHandler',
     'ArtifactPropertyWebhookCriteria',
     'ArtifactPropertyWebhookHandler',
     'ArtifactWebhookCriteria',
     'ArtifactWebhookHandler',
+    'ArtifactoryReleaseBundleCustomWebhookCriteria',
+    'ArtifactoryReleaseBundleCustomWebhookHandler',
     'ArtifactoryReleaseBundleWebhookCriteria',
     'ArtifactoryReleaseBundleWebhookHandler',
+    'BuildCustomWebhookCriteria',
+    'BuildCustomWebhookHandler',
     'BuildWebhookCriteria',
     'BuildWebhookHandler',
+    'DistributionCustomWebhookCriteria',
+    'DistributionCustomWebhookHandler',
     'DistributionWebhookCriteria',
     'DistributionWebhookHandler',
+    'DockerCustomWebhookCriteria',
+    'DockerCustomWebhookHandler',
     'DockerWebhookCriteria',
     'DockerWebhookHandler',
     'FederatedAlpineRepositoryMember',
     'FederatedBowerRepositoryMember',
     'FederatedCargoRepositoryMember',
     'FederatedChefRepositoryMember',
     'FederatedCocoapodsRepositoryMember',
@@ -69,14 +81,16 @@
     'PermissionTargetRepo',
     'PermissionTargetRepoAction',
     'PermissionTargetRepoActionGroup',
     'PermissionTargetRepoActionUser',
     'PropertySetProperty',
     'PropertySetPropertyPredefinedValue',
     'PushReplicationReplication',
+    'ReleaseBundleCustomWebhookCriteria',
+    'ReleaseBundleCustomWebhookHandler',
     'ReleaseBundleWebhookCriteria',
     'ReleaseBundleWebhookHandler',
     'RemoteAlpineRepositoryContentSynchronisation',
     'RemoteBowerRepositoryContentSynchronisation',
     'RemoteCargoRepositoryContentSynchronisation',
     'RemoteChefRepositoryContentSynchronisation',
     'RemoteCocoapodsRepositoryContentSynchronisation',
@@ -210,14 +224,366 @@
     @property
     @pulumi.getter(name="instanceId")
     def instance_id(self) -> str:
         return pulumi.get(self, "instance_id")
 
 
 @pulumi.output_type
+class ArtifactCustomWebhookCriteria(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "anyLocal":
+            suggest = "any_local"
+        elif key == "anyRemote":
+            suggest = "any_remote"
+        elif key == "repoKeys":
+            suggest = "repo_keys"
+        elif key == "excludePatterns":
+            suggest = "exclude_patterns"
+        elif key == "includePatterns":
+            suggest = "include_patterns"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ArtifactCustomWebhookCriteria. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ArtifactCustomWebhookCriteria.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ArtifactCustomWebhookCriteria.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 any_local: bool,
+                 any_remote: bool,
+                 repo_keys: Sequence[str],
+                 exclude_patterns: Optional[Sequence[str]] = None,
+                 include_patterns: Optional[Sequence[str]] = None):
+        """
+        :param bool any_local: Trigger on any local repo.
+        :param bool any_remote: Trigger on any remote repo.
+        :param Sequence[str] repo_keys: Trigger on this list of repo keys.
+        :param Sequence[str] exclude_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        :param Sequence[str] include_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        pulumi.set(__self__, "any_local", any_local)
+        pulumi.set(__self__, "any_remote", any_remote)
+        pulumi.set(__self__, "repo_keys", repo_keys)
+        if exclude_patterns is not None:
+            pulumi.set(__self__, "exclude_patterns", exclude_patterns)
+        if include_patterns is not None:
+            pulumi.set(__self__, "include_patterns", include_patterns)
+
+    @property
+    @pulumi.getter(name="anyLocal")
+    def any_local(self) -> bool:
+        """
+        Trigger on any local repo.
+        """
+        return pulumi.get(self, "any_local")
+
+    @property
+    @pulumi.getter(name="anyRemote")
+    def any_remote(self) -> bool:
+        """
+        Trigger on any remote repo.
+        """
+        return pulumi.get(self, "any_remote")
+
+    @property
+    @pulumi.getter(name="repoKeys")
+    def repo_keys(self) -> Sequence[str]:
+        """
+        Trigger on this list of repo keys.
+        """
+        return pulumi.get(self, "repo_keys")
+
+    @property
+    @pulumi.getter(name="excludePatterns")
+    def exclude_patterns(self) -> Optional[Sequence[str]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        return pulumi.get(self, "exclude_patterns")
+
+    @property
+    @pulumi.getter(name="includePatterns")
+    def include_patterns(self) -> Optional[Sequence[str]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        return pulumi.get(self, "include_patterns")
+
+
+@pulumi.output_type
+class ArtifactCustomWebhookHandler(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "httpHeaders":
+            suggest = "http_headers"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ArtifactCustomWebhookHandler. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ArtifactCustomWebhookHandler.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ArtifactCustomWebhookHandler.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 url: str,
+                 http_headers: Optional[Mapping[str, str]] = None,
+                 payload: Optional[str] = None,
+                 proxy: Optional[str] = None,
+                 secrets: Optional[Mapping[str, str]] = None):
+        """
+        :param str url: Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        :param Mapping[str, str] http_headers: HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        :param str proxy: Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        :param Mapping[str, str] secrets: Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example: 
+               
+               ```python
+               import pulumi
+               ```
+        """
+        pulumi.set(__self__, "url", url)
+        if http_headers is not None:
+            pulumi.set(__self__, "http_headers", http_headers)
+        if payload is not None:
+            pulumi.set(__self__, "payload", payload)
+        if proxy is not None:
+            pulumi.set(__self__, "proxy", proxy)
+        if secrets is not None:
+            pulumi.set(__self__, "secrets", secrets)
+
+    @property
+    @pulumi.getter
+    def url(self) -> str:
+        """
+        Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        """
+        return pulumi.get(self, "url")
+
+    @property
+    @pulumi.getter(name="httpHeaders")
+    def http_headers(self) -> Optional[Mapping[str, str]]:
+        """
+        HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        """
+        return pulumi.get(self, "http_headers")
+
+    @property
+    @pulumi.getter
+    def payload(self) -> Optional[str]:
+        return pulumi.get(self, "payload")
+
+    @property
+    @pulumi.getter
+    def proxy(self) -> Optional[str]:
+        """
+        Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        """
+        return pulumi.get(self, "proxy")
+
+    @property
+    @pulumi.getter
+    def secrets(self) -> Optional[Mapping[str, str]]:
+        """
+        Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example: 
+
+        ```python
+        import pulumi
+        ```
+        """
+        return pulumi.get(self, "secrets")
+
+
+@pulumi.output_type
+class ArtifactPropertyCustomWebhookCriteria(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "anyLocal":
+            suggest = "any_local"
+        elif key == "anyRemote":
+            suggest = "any_remote"
+        elif key == "repoKeys":
+            suggest = "repo_keys"
+        elif key == "excludePatterns":
+            suggest = "exclude_patterns"
+        elif key == "includePatterns":
+            suggest = "include_patterns"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ArtifactPropertyCustomWebhookCriteria. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ArtifactPropertyCustomWebhookCriteria.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ArtifactPropertyCustomWebhookCriteria.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 any_local: bool,
+                 any_remote: bool,
+                 repo_keys: Sequence[str],
+                 exclude_patterns: Optional[Sequence[str]] = None,
+                 include_patterns: Optional[Sequence[str]] = None):
+        """
+        :param bool any_local: Trigger on any local repo.
+        :param bool any_remote: Trigger on any remote repo.
+        :param Sequence[str] repo_keys: Trigger on this list of repo keys.
+        :param Sequence[str] exclude_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        :param Sequence[str] include_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        pulumi.set(__self__, "any_local", any_local)
+        pulumi.set(__self__, "any_remote", any_remote)
+        pulumi.set(__self__, "repo_keys", repo_keys)
+        if exclude_patterns is not None:
+            pulumi.set(__self__, "exclude_patterns", exclude_patterns)
+        if include_patterns is not None:
+            pulumi.set(__self__, "include_patterns", include_patterns)
+
+    @property
+    @pulumi.getter(name="anyLocal")
+    def any_local(self) -> bool:
+        """
+        Trigger on any local repo.
+        """
+        return pulumi.get(self, "any_local")
+
+    @property
+    @pulumi.getter(name="anyRemote")
+    def any_remote(self) -> bool:
+        """
+        Trigger on any remote repo.
+        """
+        return pulumi.get(self, "any_remote")
+
+    @property
+    @pulumi.getter(name="repoKeys")
+    def repo_keys(self) -> Sequence[str]:
+        """
+        Trigger on this list of repo keys.
+        """
+        return pulumi.get(self, "repo_keys")
+
+    @property
+    @pulumi.getter(name="excludePatterns")
+    def exclude_patterns(self) -> Optional[Sequence[str]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        return pulumi.get(self, "exclude_patterns")
+
+    @property
+    @pulumi.getter(name="includePatterns")
+    def include_patterns(self) -> Optional[Sequence[str]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        return pulumi.get(self, "include_patterns")
+
+
+@pulumi.output_type
+class ArtifactPropertyCustomWebhookHandler(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "httpHeaders":
+            suggest = "http_headers"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ArtifactPropertyCustomWebhookHandler. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ArtifactPropertyCustomWebhookHandler.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ArtifactPropertyCustomWebhookHandler.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 url: str,
+                 http_headers: Optional[Mapping[str, str]] = None,
+                 payload: Optional[str] = None,
+                 proxy: Optional[str] = None,
+                 secrets: Optional[Mapping[str, str]] = None):
+        """
+        :param str url: Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        :param Mapping[str, str] http_headers: HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        :param str proxy: Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        :param Mapping[str, str] secrets: Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+               
+               ```python
+               import pulumi
+               ```
+        """
+        pulumi.set(__self__, "url", url)
+        if http_headers is not None:
+            pulumi.set(__self__, "http_headers", http_headers)
+        if payload is not None:
+            pulumi.set(__self__, "payload", payload)
+        if proxy is not None:
+            pulumi.set(__self__, "proxy", proxy)
+        if secrets is not None:
+            pulumi.set(__self__, "secrets", secrets)
+
+    @property
+    @pulumi.getter
+    def url(self) -> str:
+        """
+        Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        """
+        return pulumi.get(self, "url")
+
+    @property
+    @pulumi.getter(name="httpHeaders")
+    def http_headers(self) -> Optional[Mapping[str, str]]:
+        """
+        HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        """
+        return pulumi.get(self, "http_headers")
+
+    @property
+    @pulumi.getter
+    def payload(self) -> Optional[str]:
+        return pulumi.get(self, "payload")
+
+    @property
+    @pulumi.getter
+    def proxy(self) -> Optional[str]:
+        """
+        Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        """
+        return pulumi.get(self, "proxy")
+
+    @property
+    @pulumi.getter
+    def secrets(self) -> Optional[Mapping[str, str]]:
+        """
+        Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+
+        ```python
+        import pulumi
+        ```
+        """
+        return pulumi.get(self, "secrets")
+
+
+@pulumi.output_type
 class ArtifactPropertyWebhookCriteria(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "anyLocal":
             suggest = "any_local"
         elif key == "anyRemote":
@@ -530,14 +896,177 @@
         """
         Secret authentication token that will be sent to the configured URL. The value will be sent as `x-jfrog-event-auth` header.
         """
         return pulumi.get(self, "secret")
 
 
 @pulumi.output_type
+class ArtifactoryReleaseBundleCustomWebhookCriteria(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "anyReleaseBundle":
+            suggest = "any_release_bundle"
+        elif key == "registeredReleaseBundleNames":
+            suggest = "registered_release_bundle_names"
+        elif key == "excludePatterns":
+            suggest = "exclude_patterns"
+        elif key == "includePatterns":
+            suggest = "include_patterns"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ArtifactoryReleaseBundleCustomWebhookCriteria. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ArtifactoryReleaseBundleCustomWebhookCriteria.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ArtifactoryReleaseBundleCustomWebhookCriteria.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 any_release_bundle: bool,
+                 registered_release_bundle_names: Sequence[str],
+                 exclude_patterns: Optional[Sequence[str]] = None,
+                 include_patterns: Optional[Sequence[str]] = None):
+        """
+        :param bool any_release_bundle: Trigger on any release bundle
+        :param Sequence[str] registered_release_bundle_names: Trigger on this list of release bundle names
+        :param Sequence[str] exclude_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`
+        :param Sequence[str] include_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`
+        """
+        pulumi.set(__self__, "any_release_bundle", any_release_bundle)
+        pulumi.set(__self__, "registered_release_bundle_names", registered_release_bundle_names)
+        if exclude_patterns is not None:
+            pulumi.set(__self__, "exclude_patterns", exclude_patterns)
+        if include_patterns is not None:
+            pulumi.set(__self__, "include_patterns", include_patterns)
+
+    @property
+    @pulumi.getter(name="anyReleaseBundle")
+    def any_release_bundle(self) -> bool:
+        """
+        Trigger on any release bundle
+        """
+        return pulumi.get(self, "any_release_bundle")
+
+    @property
+    @pulumi.getter(name="registeredReleaseBundleNames")
+    def registered_release_bundle_names(self) -> Sequence[str]:
+        """
+        Trigger on this list of release bundle names
+        """
+        return pulumi.get(self, "registered_release_bundle_names")
+
+    @property
+    @pulumi.getter(name="excludePatterns")
+    def exclude_patterns(self) -> Optional[Sequence[str]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`
+        """
+        return pulumi.get(self, "exclude_patterns")
+
+    @property
+    @pulumi.getter(name="includePatterns")
+    def include_patterns(self) -> Optional[Sequence[str]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`
+        """
+        return pulumi.get(self, "include_patterns")
+
+
+@pulumi.output_type
+class ArtifactoryReleaseBundleCustomWebhookHandler(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "httpHeaders":
+            suggest = "http_headers"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ArtifactoryReleaseBundleCustomWebhookHandler. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ArtifactoryReleaseBundleCustomWebhookHandler.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ArtifactoryReleaseBundleCustomWebhookHandler.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 url: str,
+                 http_headers: Optional[Mapping[str, str]] = None,
+                 payload: Optional[str] = None,
+                 proxy: Optional[str] = None,
+                 secrets: Optional[Mapping[str, str]] = None):
+        """
+        :param str url: Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        :param Mapping[str, str] http_headers: HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        :param str proxy: Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        :param Mapping[str, str] secrets: Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+               
+               ```python
+               import pulumi
+               ```
+        """
+        pulumi.set(__self__, "url", url)
+        if http_headers is not None:
+            pulumi.set(__self__, "http_headers", http_headers)
+        if payload is not None:
+            pulumi.set(__self__, "payload", payload)
+        if proxy is not None:
+            pulumi.set(__self__, "proxy", proxy)
+        if secrets is not None:
+            pulumi.set(__self__, "secrets", secrets)
+
+    @property
+    @pulumi.getter
+    def url(self) -> str:
+        """
+        Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        """
+        return pulumi.get(self, "url")
+
+    @property
+    @pulumi.getter(name="httpHeaders")
+    def http_headers(self) -> Optional[Mapping[str, str]]:
+        """
+        HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        """
+        return pulumi.get(self, "http_headers")
+
+    @property
+    @pulumi.getter
+    def payload(self) -> Optional[str]:
+        return pulumi.get(self, "payload")
+
+    @property
+    @pulumi.getter
+    def proxy(self) -> Optional[str]:
+        """
+        Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        """
+        return pulumi.get(self, "proxy")
+
+    @property
+    @pulumi.getter
+    def secrets(self) -> Optional[Mapping[str, str]]:
+        """
+        Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+
+        ```python
+        import pulumi
+        ```
+        """
+        return pulumi.get(self, "secrets")
+
+
+@pulumi.output_type
 class ArtifactoryReleaseBundleWebhookCriteria(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "anyReleaseBundle":
             suggest = "any_release_bundle"
         elif key == "registeredReleaseBundleNames":
@@ -677,14 +1206,177 @@
         """
         Secret authentication token that will be sent to the configured URL. The value will be sent as `x-jfrog-event-auth` header.
         """
         return pulumi.get(self, "secret")
 
 
 @pulumi.output_type
+class BuildCustomWebhookCriteria(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "anyBuild":
+            suggest = "any_build"
+        elif key == "selectedBuilds":
+            suggest = "selected_builds"
+        elif key == "excludePatterns":
+            suggest = "exclude_patterns"
+        elif key == "includePatterns":
+            suggest = "include_patterns"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in BuildCustomWebhookCriteria. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        BuildCustomWebhookCriteria.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        BuildCustomWebhookCriteria.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 any_build: bool,
+                 selected_builds: Sequence[str],
+                 exclude_patterns: Optional[Sequence[str]] = None,
+                 include_patterns: Optional[Sequence[str]] = None):
+        """
+        :param bool any_build: Trigger on any build.
+        :param Sequence[str] selected_builds: Trigger on this list of build names.
+        :param Sequence[str] exclude_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        :param Sequence[str] include_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        pulumi.set(__self__, "any_build", any_build)
+        pulumi.set(__self__, "selected_builds", selected_builds)
+        if exclude_patterns is not None:
+            pulumi.set(__self__, "exclude_patterns", exclude_patterns)
+        if include_patterns is not None:
+            pulumi.set(__self__, "include_patterns", include_patterns)
+
+    @property
+    @pulumi.getter(name="anyBuild")
+    def any_build(self) -> bool:
+        """
+        Trigger on any build.
+        """
+        return pulumi.get(self, "any_build")
+
+    @property
+    @pulumi.getter(name="selectedBuilds")
+    def selected_builds(self) -> Sequence[str]:
+        """
+        Trigger on this list of build names.
+        """
+        return pulumi.get(self, "selected_builds")
+
+    @property
+    @pulumi.getter(name="excludePatterns")
+    def exclude_patterns(self) -> Optional[Sequence[str]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        return pulumi.get(self, "exclude_patterns")
+
+    @property
+    @pulumi.getter(name="includePatterns")
+    def include_patterns(self) -> Optional[Sequence[str]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        return pulumi.get(self, "include_patterns")
+
+
+@pulumi.output_type
+class BuildCustomWebhookHandler(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "httpHeaders":
+            suggest = "http_headers"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in BuildCustomWebhookHandler. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        BuildCustomWebhookHandler.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        BuildCustomWebhookHandler.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 url: str,
+                 http_headers: Optional[Mapping[str, str]] = None,
+                 payload: Optional[str] = None,
+                 proxy: Optional[str] = None,
+                 secrets: Optional[Mapping[str, str]] = None):
+        """
+        :param str url: Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        :param Mapping[str, str] http_headers: HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        :param str proxy: Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        :param Mapping[str, str] secrets: Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+               
+               ```python
+               import pulumi
+               ```
+        """
+        pulumi.set(__self__, "url", url)
+        if http_headers is not None:
+            pulumi.set(__self__, "http_headers", http_headers)
+        if payload is not None:
+            pulumi.set(__self__, "payload", payload)
+        if proxy is not None:
+            pulumi.set(__self__, "proxy", proxy)
+        if secrets is not None:
+            pulumi.set(__self__, "secrets", secrets)
+
+    @property
+    @pulumi.getter
+    def url(self) -> str:
+        """
+        Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        """
+        return pulumi.get(self, "url")
+
+    @property
+    @pulumi.getter(name="httpHeaders")
+    def http_headers(self) -> Optional[Mapping[str, str]]:
+        """
+        HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        """
+        return pulumi.get(self, "http_headers")
+
+    @property
+    @pulumi.getter
+    def payload(self) -> Optional[str]:
+        return pulumi.get(self, "payload")
+
+    @property
+    @pulumi.getter
+    def proxy(self) -> Optional[str]:
+        """
+        Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        """
+        return pulumi.get(self, "proxy")
+
+    @property
+    @pulumi.getter
+    def secrets(self) -> Optional[Mapping[str, str]]:
+        """
+        Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+
+        ```python
+        import pulumi
+        ```
+        """
+        return pulumi.get(self, "secrets")
+
+
+@pulumi.output_type
 class BuildWebhookCriteria(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "anyBuild":
             suggest = "any_build"
         elif key == "selectedBuilds":
@@ -824,14 +1516,177 @@
         """
         Secret authentication token that will be sent to the configured URL. The value will be sent as `x-jfrog-event-auth` header.
         """
         return pulumi.get(self, "secret")
 
 
 @pulumi.output_type
+class DistributionCustomWebhookCriteria(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "anyReleaseBundle":
+            suggest = "any_release_bundle"
+        elif key == "registeredReleaseBundleNames":
+            suggest = "registered_release_bundle_names"
+        elif key == "excludePatterns":
+            suggest = "exclude_patterns"
+        elif key == "includePatterns":
+            suggest = "include_patterns"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in DistributionCustomWebhookCriteria. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        DistributionCustomWebhookCriteria.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        DistributionCustomWebhookCriteria.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 any_release_bundle: bool,
+                 registered_release_bundle_names: Sequence[str],
+                 exclude_patterns: Optional[Sequence[str]] = None,
+                 include_patterns: Optional[Sequence[str]] = None):
+        """
+        :param bool any_release_bundle: Trigger on any release bundle.
+        :param Sequence[str] registered_release_bundle_names: Trigger on this list of release bundle names.
+        :param Sequence[str] exclude_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        :param Sequence[str] include_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        pulumi.set(__self__, "any_release_bundle", any_release_bundle)
+        pulumi.set(__self__, "registered_release_bundle_names", registered_release_bundle_names)
+        if exclude_patterns is not None:
+            pulumi.set(__self__, "exclude_patterns", exclude_patterns)
+        if include_patterns is not None:
+            pulumi.set(__self__, "include_patterns", include_patterns)
+
+    @property
+    @pulumi.getter(name="anyReleaseBundle")
+    def any_release_bundle(self) -> bool:
+        """
+        Trigger on any release bundle.
+        """
+        return pulumi.get(self, "any_release_bundle")
+
+    @property
+    @pulumi.getter(name="registeredReleaseBundleNames")
+    def registered_release_bundle_names(self) -> Sequence[str]:
+        """
+        Trigger on this list of release bundle names.
+        """
+        return pulumi.get(self, "registered_release_bundle_names")
+
+    @property
+    @pulumi.getter(name="excludePatterns")
+    def exclude_patterns(self) -> Optional[Sequence[str]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        return pulumi.get(self, "exclude_patterns")
+
+    @property
+    @pulumi.getter(name="includePatterns")
+    def include_patterns(self) -> Optional[Sequence[str]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        return pulumi.get(self, "include_patterns")
+
+
+@pulumi.output_type
+class DistributionCustomWebhookHandler(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "httpHeaders":
+            suggest = "http_headers"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in DistributionCustomWebhookHandler. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        DistributionCustomWebhookHandler.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        DistributionCustomWebhookHandler.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 url: str,
+                 http_headers: Optional[Mapping[str, str]] = None,
+                 payload: Optional[str] = None,
+                 proxy: Optional[str] = None,
+                 secrets: Optional[Mapping[str, str]] = None):
+        """
+        :param str url: Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        :param Mapping[str, str] http_headers: HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        :param str proxy: Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        :param Mapping[str, str] secrets: Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+               
+               ```python
+               import pulumi
+               ```
+        """
+        pulumi.set(__self__, "url", url)
+        if http_headers is not None:
+            pulumi.set(__self__, "http_headers", http_headers)
+        if payload is not None:
+            pulumi.set(__self__, "payload", payload)
+        if proxy is not None:
+            pulumi.set(__self__, "proxy", proxy)
+        if secrets is not None:
+            pulumi.set(__self__, "secrets", secrets)
+
+    @property
+    @pulumi.getter
+    def url(self) -> str:
+        """
+        Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        """
+        return pulumi.get(self, "url")
+
+    @property
+    @pulumi.getter(name="httpHeaders")
+    def http_headers(self) -> Optional[Mapping[str, str]]:
+        """
+        HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        """
+        return pulumi.get(self, "http_headers")
+
+    @property
+    @pulumi.getter
+    def payload(self) -> Optional[str]:
+        return pulumi.get(self, "payload")
+
+    @property
+    @pulumi.getter
+    def proxy(self) -> Optional[str]:
+        """
+        Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        """
+        return pulumi.get(self, "proxy")
+
+    @property
+    @pulumi.getter
+    def secrets(self) -> Optional[Mapping[str, str]]:
+        """
+        Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+
+        ```python
+        import pulumi
+        ```
+        """
+        return pulumi.get(self, "secrets")
+
+
+@pulumi.output_type
 class DistributionWebhookCriteria(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "anyReleaseBundle":
             suggest = "any_release_bundle"
         elif key == "registeredReleaseBundleNames":
@@ -971,14 +1826,190 @@
         """
         Secret authentication token that will be sent to the configured URL. The value will be sent as `x-jfrog-event-auth` header.
         """
         return pulumi.get(self, "secret")
 
 
 @pulumi.output_type
+class DockerCustomWebhookCriteria(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "anyLocal":
+            suggest = "any_local"
+        elif key == "anyRemote":
+            suggest = "any_remote"
+        elif key == "repoKeys":
+            suggest = "repo_keys"
+        elif key == "excludePatterns":
+            suggest = "exclude_patterns"
+        elif key == "includePatterns":
+            suggest = "include_patterns"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in DockerCustomWebhookCriteria. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        DockerCustomWebhookCriteria.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        DockerCustomWebhookCriteria.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 any_local: bool,
+                 any_remote: bool,
+                 repo_keys: Sequence[str],
+                 exclude_patterns: Optional[Sequence[str]] = None,
+                 include_patterns: Optional[Sequence[str]] = None):
+        """
+        :param bool any_local: Trigger on any local repo.
+        :param bool any_remote: Trigger on any remote repo.
+        :param Sequence[str] repo_keys: Trigger on this list of repo keys.
+        :param Sequence[str] exclude_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        :param Sequence[str] include_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        pulumi.set(__self__, "any_local", any_local)
+        pulumi.set(__self__, "any_remote", any_remote)
+        pulumi.set(__self__, "repo_keys", repo_keys)
+        if exclude_patterns is not None:
+            pulumi.set(__self__, "exclude_patterns", exclude_patterns)
+        if include_patterns is not None:
+            pulumi.set(__self__, "include_patterns", include_patterns)
+
+    @property
+    @pulumi.getter(name="anyLocal")
+    def any_local(self) -> bool:
+        """
+        Trigger on any local repo.
+        """
+        return pulumi.get(self, "any_local")
+
+    @property
+    @pulumi.getter(name="anyRemote")
+    def any_remote(self) -> bool:
+        """
+        Trigger on any remote repo.
+        """
+        return pulumi.get(self, "any_remote")
+
+    @property
+    @pulumi.getter(name="repoKeys")
+    def repo_keys(self) -> Sequence[str]:
+        """
+        Trigger on this list of repo keys.
+        """
+        return pulumi.get(self, "repo_keys")
+
+    @property
+    @pulumi.getter(name="excludePatterns")
+    def exclude_patterns(self) -> Optional[Sequence[str]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        return pulumi.get(self, "exclude_patterns")
+
+    @property
+    @pulumi.getter(name="includePatterns")
+    def include_patterns(self) -> Optional[Sequence[str]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: `org/apache/**`.
+        """
+        return pulumi.get(self, "include_patterns")
+
+
+@pulumi.output_type
+class DockerCustomWebhookHandler(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "httpHeaders":
+            suggest = "http_headers"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in DockerCustomWebhookHandler. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        DockerCustomWebhookHandler.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        DockerCustomWebhookHandler.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 url: str,
+                 http_headers: Optional[Mapping[str, str]] = None,
+                 payload: Optional[str] = None,
+                 proxy: Optional[str] = None,
+                 secrets: Optional[Mapping[str, str]] = None):
+        """
+        :param str url: Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        :param Mapping[str, str] http_headers: HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        :param str proxy: Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        :param Mapping[str, str] secrets: Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+               
+               ```python
+               import pulumi
+               ```
+        """
+        pulumi.set(__self__, "url", url)
+        if http_headers is not None:
+            pulumi.set(__self__, "http_headers", http_headers)
+        if payload is not None:
+            pulumi.set(__self__, "payload", payload)
+        if proxy is not None:
+            pulumi.set(__self__, "proxy", proxy)
+        if secrets is not None:
+            pulumi.set(__self__, "secrets", secrets)
+
+    @property
+    @pulumi.getter
+    def url(self) -> str:
+        """
+        Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        """
+        return pulumi.get(self, "url")
+
+    @property
+    @pulumi.getter(name="httpHeaders")
+    def http_headers(self) -> Optional[Mapping[str, str]]:
+        """
+        HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        """
+        return pulumi.get(self, "http_headers")
+
+    @property
+    @pulumi.getter
+    def payload(self) -> Optional[str]:
+        return pulumi.get(self, "payload")
+
+    @property
+    @pulumi.getter
+    def proxy(self) -> Optional[str]:
+        """
+        Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        """
+        return pulumi.get(self, "proxy")
+
+    @property
+    @pulumi.getter
+    def secrets(self) -> Optional[Mapping[str, str]]:
+        """
+        Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+
+        ```python
+        import pulumi
+        ```
+        """
+        return pulumi.get(self, "secrets")
+
+
+@pulumi.output_type
 class DockerWebhookCriteria(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "anyLocal":
             suggest = "any_local"
         elif key == "anyRemote":
@@ -3173,14 +4204,177 @@
         """
         When set, artifact download statistics will also be replicated. Set to avoid inadvertent cleanup at the target instance when setting up replication for disaster recovery.
         """
         return pulumi.get(self, "sync_statistics")
 
 
 @pulumi.output_type
+class ReleaseBundleCustomWebhookCriteria(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "anyReleaseBundle":
+            suggest = "any_release_bundle"
+        elif key == "registeredReleaseBundleNames":
+            suggest = "registered_release_bundle_names"
+        elif key == "excludePatterns":
+            suggest = "exclude_patterns"
+        elif key == "includePatterns":
+            suggest = "include_patterns"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ReleaseBundleCustomWebhookCriteria. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ReleaseBundleCustomWebhookCriteria.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ReleaseBundleCustomWebhookCriteria.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 any_release_bundle: bool,
+                 registered_release_bundle_names: Sequence[str],
+                 exclude_patterns: Optional[Sequence[str]] = None,
+                 include_patterns: Optional[Sequence[str]] = None):
+        """
+        :param bool any_release_bundle: Trigger on any release bundle.
+        :param Sequence[str] registered_release_bundle_names: Trigger on this list of release bundle names.
+        :param Sequence[str] exclude_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: "org/apache/**".
+        :param Sequence[str] include_patterns: Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: "org/apache/**".
+        """
+        pulumi.set(__self__, "any_release_bundle", any_release_bundle)
+        pulumi.set(__self__, "registered_release_bundle_names", registered_release_bundle_names)
+        if exclude_patterns is not None:
+            pulumi.set(__self__, "exclude_patterns", exclude_patterns)
+        if include_patterns is not None:
+            pulumi.set(__self__, "include_patterns", include_patterns)
+
+    @property
+    @pulumi.getter(name="anyReleaseBundle")
+    def any_release_bundle(self) -> bool:
+        """
+        Trigger on any release bundle.
+        """
+        return pulumi.get(self, "any_release_bundle")
+
+    @property
+    @pulumi.getter(name="registeredReleaseBundleNames")
+    def registered_release_bundle_names(self) -> Sequence[str]:
+        """
+        Trigger on this list of release bundle names.
+        """
+        return pulumi.get(self, "registered_release_bundle_names")
+
+    @property
+    @pulumi.getter(name="excludePatterns")
+    def exclude_patterns(self) -> Optional[Sequence[str]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: "org/apache/**".
+        """
+        return pulumi.get(self, "exclude_patterns")
+
+    @property
+    @pulumi.getter(name="includePatterns")
+    def include_patterns(self) -> Optional[Sequence[str]]:
+        """
+        Simple comma separated wildcard patterns for repository artifact paths (with no leading slash). Ant-style path expressions are supported (*, *\\*, ?). For example: "org/apache/**".
+        """
+        return pulumi.get(self, "include_patterns")
+
+
+@pulumi.output_type
+class ReleaseBundleCustomWebhookHandler(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "httpHeaders":
+            suggest = "http_headers"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ReleaseBundleCustomWebhookHandler. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ReleaseBundleCustomWebhookHandler.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ReleaseBundleCustomWebhookHandler.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 url: str,
+                 http_headers: Optional[Mapping[str, str]] = None,
+                 payload: Optional[str] = None,
+                 proxy: Optional[str] = None,
+                 secrets: Optional[Mapping[str, str]] = None):
+        """
+        :param str url: Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        :param Mapping[str, str] http_headers: HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        :param str proxy: Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        :param Mapping[str, str] secrets: Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+               
+               ```python
+               import pulumi
+               ```
+        """
+        pulumi.set(__self__, "url", url)
+        if http_headers is not None:
+            pulumi.set(__self__, "http_headers", http_headers)
+        if payload is not None:
+            pulumi.set(__self__, "payload", payload)
+        if proxy is not None:
+            pulumi.set(__self__, "proxy", proxy)
+        if secrets is not None:
+            pulumi.set(__self__, "secrets", secrets)
+
+    @property
+    @pulumi.getter
+    def url(self) -> str:
+        """
+        Specifies the URL that the Webhook invokes. This will be the URL that Artifactory will send an HTTP POST request to.
+        """
+        return pulumi.get(self, "url")
+
+    @property
+    @pulumi.getter(name="httpHeaders")
+    def http_headers(self) -> Optional[Mapping[str, str]]:
+        """
+        HTTP headers you wish to use to invoke the Webhook, comprise key/value pair.
+        """
+        return pulumi.get(self, "http_headers")
+
+    @property
+    @pulumi.getter
+    def payload(self) -> Optional[str]:
+        return pulumi.get(self, "payload")
+
+    @property
+    @pulumi.getter
+    def proxy(self) -> Optional[str]:
+        """
+        Proxy key from Artifactory UI (Administration > Proxies > Configuration).
+        """
+        return pulumi.get(self, "proxy")
+
+    @property
+    @pulumi.getter
+    def secrets(self) -> Optional[Mapping[str, str]]:
+        """
+        Defines a set of sensitive values (such as, tokens and passwords) that can be injected in the headers and/or payload.Secrets’ values are encrypted. In the header/payload, the value can be invoked using the `{{.secrets.token}}` format, where token is the name provided for the secret value. Comprise key/value pair. **Note:** if multiple handlers are used, same secret name and different secret value for the same url won't work. Example:
+
+        ```python
+        import pulumi
+        ```
+        """
+        return pulumi.get(self, "secrets")
+
+
+@pulumi.output_type
 class ReleaseBundleWebhookCriteria(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "anyReleaseBundle":
             suggest = "any_release_bundle"
         elif key == "registeredReleaseBundleNames":
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/permission_target.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/permission_target.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/property_set.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/property_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/provider.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/proxy.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/proxy.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/pull_replication.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/pull_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/push_replication.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/push_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/release_bundle_webhook.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/release_bundle_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_alpine_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_bower_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_cargo_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_chef_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_cocoapods_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_composer_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_conan_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_conda_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_cran_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_debian_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_docker_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_gems_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_generic_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_gitlfs_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_go_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_gradle_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_helm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_ivy_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_maven_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_npm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_nuget_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_opkg_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_p2_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_pub_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_puppet_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_pypi_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_repository_replication.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_repository_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_rpm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_sbt_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_swift_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_terraform_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/remote_vcs_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/remote_vcs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/replication_config.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/replication_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/repository_layout.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/repository_layout.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/saml_settings.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/saml_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/scoped_token.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/scoped_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
                  username: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ScopedToken resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to '*@*' if not set. Service ID must begin with valid JFrog service type. Options: jfrt, jfxr, jfpip, jfds, jfmc, jfac, jfevt, jfmd, jfcon, or *. For instructions to retrieve the Artifactory Service ID see this [documentation](https://jfrog.com/help/r/jfrog-rest-apis/get-service-id)
         :param pulumi.Input[str] description: Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
         :param pulumi.Input[int] expires_in: The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in 'access.config.yaml'. See [API documentation](https://jfrog.com/help/r/jfrog-rest-apis/revoke-token-by-id) for details. Access Token would not be saved by Artifactory if this is less than the persistence threshold value (default to 10800 seconds) set in Access configuration. See [official documentation](https://jfrog.com/help/r/jfrog-platform-administration-documentation/using-the-revocable-and-persistency-thresholds) for details.
         :param pulumi.Input[str] grant_type: The grant type used to authenticate the request. In this case, the only value supported is `client_credentials` which is also the default value if this parameter is not specified.
-        :param pulumi.Input[bool] include_reference_token: Also create a reference token which can be used like an API key. Default is `false`.
+        :param pulumi.Input[bool] include_reference_token: Also create a reference token which can be used like an API key.
         :param pulumi.Input[bool] refreshable: Is this token refreshable? Default is `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
                The supported scopes include:
         :param pulumi.Input[str] username: The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: \\n\\n/users/\\n\\n. Limited to 255 characters.
         """
         if audiences is not None:
             pulumi.set(__self__, "audiences", audiences)
@@ -99,15 +99,15 @@
     def grant_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "grant_type", value)
 
     @property
     @pulumi.getter(name="includeReferenceToken")
     def include_reference_token(self) -> Optional[pulumi.Input[bool]]:
         """
-        Also create a reference token which can be used like an API key. Default is `false`.
+        Also create a reference token which can be used like an API key.
         """
         return pulumi.get(self, "include_reference_token")
 
     @include_reference_token.setter
     def include_reference_token(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "include_reference_token", value)
 
@@ -172,15 +172,15 @@
         Input properties used for looking up and filtering ScopedToken resources.
         :param pulumi.Input[str] access_token: Returns the access token to authenticate to Artifactory.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to '*@*' if not set. Service ID must begin with valid JFrog service type. Options: jfrt, jfxr, jfpip, jfds, jfmc, jfac, jfevt, jfmd, jfcon, or *. For instructions to retrieve the Artifactory Service ID see this [documentation](https://jfrog.com/help/r/jfrog-rest-apis/get-service-id)
         :param pulumi.Input[str] description: Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
         :param pulumi.Input[int] expires_in: The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in 'access.config.yaml'. See [API documentation](https://jfrog.com/help/r/jfrog-rest-apis/revoke-token-by-id) for details. Access Token would not be saved by Artifactory if this is less than the persistence threshold value (default to 10800 seconds) set in Access configuration. See [official documentation](https://jfrog.com/help/r/jfrog-platform-administration-documentation/using-the-revocable-and-persistency-thresholds) for details.
         :param pulumi.Input[int] expiry: Returns the token expiry.
         :param pulumi.Input[str] grant_type: The grant type used to authenticate the request. In this case, the only value supported is `client_credentials` which is also the default value if this parameter is not specified.
-        :param pulumi.Input[bool] include_reference_token: Also create a reference token which can be used like an API key. Default is `false`.
+        :param pulumi.Input[bool] include_reference_token: Also create a reference token which can be used like an API key.
         :param pulumi.Input[int] issued_at: Returns the token issued at date/time.
         :param pulumi.Input[str] issuer: Returns the token issuer.
         :param pulumi.Input[str] reference_token: Reference Token (alias to Access Token).
         :param pulumi.Input[str] refresh_token: Refresh token.
         :param pulumi.Input[bool] refreshable: Is this token refreshable? Default is `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
                The supported scopes include:
@@ -293,15 +293,15 @@
     def grant_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "grant_type", value)
 
     @property
     @pulumi.getter(name="includeReferenceToken")
     def include_reference_token(self) -> Optional[pulumi.Input[bool]]:
         """
-        Also create a reference token which can be used like an API key. Default is `false`.
+        Also create a reference token which can be used like an API key.
         """
         return pulumi.get(self, "include_reference_token")
 
     @include_reference_token.setter
     def include_reference_token(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "include_reference_token", value)
 
@@ -491,15 +491,15 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to '*@*' if not set. Service ID must begin with valid JFrog service type. Options: jfrt, jfxr, jfpip, jfds, jfmc, jfac, jfevt, jfmd, jfcon, or *. For instructions to retrieve the Artifactory Service ID see this [documentation](https://jfrog.com/help/r/jfrog-rest-apis/get-service-id)
         :param pulumi.Input[str] description: Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
         :param pulumi.Input[int] expires_in: The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in 'access.config.yaml'. See [API documentation](https://jfrog.com/help/r/jfrog-rest-apis/revoke-token-by-id) for details. Access Token would not be saved by Artifactory if this is less than the persistence threshold value (default to 10800 seconds) set in Access configuration. See [official documentation](https://jfrog.com/help/r/jfrog-platform-administration-documentation/using-the-revocable-and-persistency-thresholds) for details.
         :param pulumi.Input[str] grant_type: The grant type used to authenticate the request. In this case, the only value supported is `client_credentials` which is also the default value if this parameter is not specified.
-        :param pulumi.Input[bool] include_reference_token: Also create a reference token which can be used like an API key. Default is `false`.
+        :param pulumi.Input[bool] include_reference_token: Also create a reference token which can be used like an API key.
         :param pulumi.Input[bool] refreshable: Is this token refreshable? Default is `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
                The supported scopes include:
         :param pulumi.Input[str] username: The user name for which this token is created. The username is based on the authenticated user - either from the user of the authenticated token or based on the username (if basic auth was used). The username is then used to set the subject of the token: \\n\\n/users/\\n\\n. Limited to 255 characters.
         """
         ...
     @overload
@@ -652,15 +652,15 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_token: Returns the access token to authenticate to Artifactory.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to '*@*' if not set. Service ID must begin with valid JFrog service type. Options: jfrt, jfxr, jfpip, jfds, jfmc, jfac, jfevt, jfmd, jfcon, or *. For instructions to retrieve the Artifactory Service ID see this [documentation](https://jfrog.com/help/r/jfrog-rest-apis/get-service-id)
         :param pulumi.Input[str] description: Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
         :param pulumi.Input[int] expires_in: The amount of time, in seconds, it would take for the token to expire. An admin shall be able to set whether expiry is mandatory, what is the default expiry, and what is the maximum expiry allowed. Must be non-negative. Default value is based on configuration in 'access.config.yaml'. See [API documentation](https://jfrog.com/help/r/jfrog-rest-apis/revoke-token-by-id) for details. Access Token would not be saved by Artifactory if this is less than the persistence threshold value (default to 10800 seconds) set in Access configuration. See [official documentation](https://jfrog.com/help/r/jfrog-platform-administration-documentation/using-the-revocable-and-persistency-thresholds) for details.
         :param pulumi.Input[int] expiry: Returns the token expiry.
         :param pulumi.Input[str] grant_type: The grant type used to authenticate the request. In this case, the only value supported is `client_credentials` which is also the default value if this parameter is not specified.
-        :param pulumi.Input[bool] include_reference_token: Also create a reference token which can be used like an API key. Default is `false`.
+        :param pulumi.Input[bool] include_reference_token: Also create a reference token which can be used like an API key.
         :param pulumi.Input[int] issued_at: Returns the token issued at date/time.
         :param pulumi.Input[str] issuer: Returns the token issuer.
         :param pulumi.Input[str] reference_token: Reference Token (alias to Access Token).
         :param pulumi.Input[str] refresh_token: Refresh token.
         :param pulumi.Input[bool] refreshable: Is this token refreshable? Default is `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope of access that the token provides. Access to the REST API is always provided by default. Administrators can set any scope, while non-admin users can only set the scope to a subset of the groups to which they belong.
                The supported scopes include:
@@ -738,15 +738,15 @@
         """
         return pulumi.get(self, "grant_type")
 
     @property
     @pulumi.getter(name="includeReferenceToken")
     def include_reference_token(self) -> pulumi.Output[bool]:
         """
-        Also create a reference token which can be used like an API key. Default is `false`.
+        Also create a reference token which can be used like an API key.
         """
         return pulumi.get(self, "include_reference_token")
 
     @property
     @pulumi.getter(name="issuedAt")
     def issued_at(self) -> pulumi.Output[int]:
         """
```

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/single_replication_config.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/single_replication_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/unmanaged_user.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/unmanaged_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/user.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_alpine_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_bower_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_chef_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_composer_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_conan_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_conda_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_cran_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_debian_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_docker_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_gems_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_generic_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_gitlfs_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_gradle_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_helm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_ivy_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_npm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_nuget_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_p2_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_pub_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_puppet_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_pypi_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_rpm_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_sbt_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_swift_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory/virtual_terraform_repository.py` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory/virtual_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory.egg-info/PKG-INFO` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-artifactory
-Version: 4.2.0a1688644862
+Version: 4.2.0a1688687344
 Summary: A Pulumi package for creating and managing artifactory cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-artifactory
 Keywords: pulumi artifactory
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_artifactory-4.2.0a1688644862/pulumi_artifactory.egg-info/SOURCES.txt` & `pulumi_artifactory-4.2.0a1688687344/pulumi_artifactory.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,29 @@
 pulumi_artifactory/__init__.py
 pulumi_artifactory/_inputs.py
 pulumi_artifactory/_utilities.py
 pulumi_artifactory/access_token.py
 pulumi_artifactory/alpine_repository.py
 pulumi_artifactory/anonymous_user.py
 pulumi_artifactory/api_key.py
+pulumi_artifactory/artifact_custom_webhook.py
+pulumi_artifactory/artifact_property_custom_webhook.py
 pulumi_artifactory/artifact_property_webhook.py
 pulumi_artifactory/artifact_webhook.py
+pulumi_artifactory/artifactory_release_bundle_custom_webhook.py
 pulumi_artifactory/artifactory_release_bundle_webhook.py
 pulumi_artifactory/backup.py
+pulumi_artifactory/build_custom_webhook.py
 pulumi_artifactory/build_webhook.py
 pulumi_artifactory/certificate.py
 pulumi_artifactory/debian_repository.py
+pulumi_artifactory/distribution_custom_webhook.py
 pulumi_artifactory/distribution_public_key.py
 pulumi_artifactory/distribution_webhook.py
+pulumi_artifactory/docker_custom_webhook.py
 pulumi_artifactory/docker_v1_repository.py
 pulumi_artifactory/docker_v2_repository.py
 pulumi_artifactory/docker_webhook.py
 pulumi_artifactory/federated_alpine_repository.py
 pulumi_artifactory/federated_bower_repository.py
 pulumi_artifactory/federated_cargo_repository.py
 pulumi_artifactory/federated_chef_repository.py
@@ -223,14 +229,15 @@
 pulumi_artifactory/property_set.py
 pulumi_artifactory/provider.py
 pulumi_artifactory/proxy.py
 pulumi_artifactory/pull_replication.py
 pulumi_artifactory/pulumi-plugin.json
 pulumi_artifactory/push_replication.py
 pulumi_artifactory/py.typed
+pulumi_artifactory/release_bundle_custom_webhook.py
 pulumi_artifactory/release_bundle_webhook.py
 pulumi_artifactory/remote_alpine_repository.py
 pulumi_artifactory/remote_bower_repository.py
 pulumi_artifactory/remote_cargo_repository.py
 pulumi_artifactory/remote_chef_repository.py
 pulumi_artifactory/remote_cocoapods_repository.py
 pulumi_artifactory/remote_composer_repository.py
```

### Comparing `pulumi_artifactory-4.2.0a1688644862/setup.py` & `pulumi_artifactory-4.2.0a1688687344/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.2.0a1688644862"
-PLUGIN_VERSION = "4.2.0-alpha.1688644862+77c045f8"
+VERSION = "4.2.0a1688687344"
+PLUGIN_VERSION = "4.2.0-alpha.1688687344+e16aa1de"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'artifactory', PLUGIN_VERSION])
         except OSError as error:
```

