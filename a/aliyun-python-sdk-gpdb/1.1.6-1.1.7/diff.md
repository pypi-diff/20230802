# Comparing `tmp/aliyun-python-sdk-gpdb-1.1.6.tar.gz` & `tmp/aliyun-python-sdk-gpdb-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-gpdb-1.1.6.tar", last modified: Wed May 24 02:53:04 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-gpdb-1.1.7.tar", last modified: Wed Aug  2 01:59:30 2023, max compression
```

## Comparing `aliyun-python-sdk-gpdb-1.1.6.tar` & `aliyun-python-sdk-gpdb-1.1.7.tar`

### file list

```diff
@@ -1,113 +1,116 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:53:04.000000 aliyun-python-sdk-gpdb-1.1.6/
--rw-r--r--   0 root         (0) root         (0)      575 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1542 2023-05-24 02:53:04.000000 aliyun-python-sdk-gpdb-1.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:53:04.000000 aliyun-python-sdk-gpdb-1.1.6/aliyun_python_sdk_gpdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1542 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyun_python_sdk_gpdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6444 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyun_python_sdk_gpdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyun_python_sdk_gpdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyun_python_sdk_gpdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyun_python_sdk_gpdb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:53:04.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:53:04.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:53:04.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/
--rw-r--r--   0 root         (0) root         (0)     1859 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/AddBuDBInstanceRelationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2757 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/AllocateInstancePublicConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1282 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CheckServiceLinkedRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2717 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     3011 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateDBInstancePlanRequest.py
--rw-r--r--   0 root         (0) root         (0)     8602 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     6730 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateECSDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateSampleDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateServiceLinkedRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1817 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DeleteDBInstancePlanRequest.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DeleteDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1857 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DeleteDatabaseRequest.py
--rw-r--r--   0 root         (0) root         (0)     1670 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeAccountsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1815 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeAvailableResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1481 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBClusterNodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2344 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBClusterPerformanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1885 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1869 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDataBloatRequest.py
--rw-r--r--   0 root         (0) root         (0)     1867 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDataSkewRequest.py
--rw-r--r--   0 root         (0) root         (0)     2456 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDiagnosisSummaryRequest.py
--rw-r--r--   0 root         (0) root         (0)     3072 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceErrorLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     1720 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceIPArrayListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1871 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceIndexUsageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1491 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceNetInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceOnECSAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2227 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstancePerformanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2623 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstancePlansRequest.py
--rw-r--r--   0 root         (0) root         (0)     2579 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceSQLPatternsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1483 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceSSLRequest.py
--rw-r--r--   0 root         (0) root         (0)     4374 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2963 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDataBackupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2251 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDataShareInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDataSharePerformanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1495 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisDimensionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2418 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisMonitorPerformanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3104 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1841 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisSQLInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDownloadRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1630 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeHealthStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2209 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeLogBackupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeModifyParameterLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     1477 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2874 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeRdsVSwitchsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2705 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeRdsVpcsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1435 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1483 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeResourceUsageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1493 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLCollectorPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogByQueryIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     3813 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogCountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2032 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogFilesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2913 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2838 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogsOnSliceRequest.py
--rw-r--r--   0 root         (0) root         (0)     4179 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     4400 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogsV2Request.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSampleDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2541 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSlowLogRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3990 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSlowSQLLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2235 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSpecificationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1656 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSupportFeaturesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2526 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1666 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeUserEncryptionKeyListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1813 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeWaitingSQLInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     3106 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeWaitingSQLRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2772 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DownloadDiagnosisRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3187 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1925 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyAccountDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2730 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1716 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConnectionModeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2192 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConnectionStringRequest.py
--rw-r--r--   0 root         (0) root         (0)     1973 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2076 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceMaintainTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2313 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceNetworkTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2799 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1899 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceSSLRequest.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1728 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifySQLCollectorPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2646 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifySecurityIpsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1636 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/PauseInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1676 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/RebalanceDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1969 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ReleaseInstancePublicConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1899 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ResetAccountPasswordRequest.py
--rw-r--r--   0 root         (0) root         (0)     1672 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/RestartDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1638 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ResumeInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2014 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/SetDBInstancePlanStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1881 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/SetDataShareInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1905 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/SwitchDBInstanceNetTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2994 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/UnloadSampleDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2972 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2772 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/UpdateDBInstancePlanRequest.py
--rw-r--r--   0 root         (0) root         (0)     3987 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/UpgradeDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2454 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/UpgradeDBVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-24 02:53:04.000000 aliyun-python-sdk-gpdb-1.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2457 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyun_python_sdk_gpdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyun_python_sdk_gpdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6562 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyun_python_sdk_gpdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyun_python_sdk_gpdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyun_python_sdk_gpdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyun_python_sdk_gpdb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/
+-rw-r--r--   0 root         (0) root         (0)     2757 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/AllocateInstancePublicConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/CheckServiceLinkedRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2717 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/CreateAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/CreateCollectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3011 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/CreateDBInstancePlanRequest.py
+-rw-r--r--   0 root         (0) root         (0)     8602 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/CreateDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/CreateNamespaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/CreateSampleDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/CreateServiceLinkedRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2858 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/CreateVectorIndexRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2725 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DeleteCollectionDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DeleteCollectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DeleteDBInstancePlanRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DeleteDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2303 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DeleteNamespaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DeleteVectorIndexRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeAccountsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeAvailableResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1481 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeBackupPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeCollectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBClusterNodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBClusterPerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDataBloatRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDataSkewRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDiagnosisSummaryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3072 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceErrorLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1720 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceIPArrayListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceIndexUsageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceNetInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstancePerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstancePlansRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceSSLRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4374 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDataBackupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDataReDistributeInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDataShareInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDataSharePerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisDimensionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2418 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisMonitorPerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3104 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisSQLInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDownloadRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDownloadSQLLogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1630 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeHealthStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2209 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeLogBackupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeModifyParameterLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeNamespaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1477 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeRdsVSwitchsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeRdsVpcsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3813 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeSQLLogCountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4400 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeSQLLogsV2Request.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeSampleDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeSupportFeaturesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeUserEncryptionKeyListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeWaitingSQLInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3106 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeWaitingSQLRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DownloadDiagnosisRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DownloadSQLLogsRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2906 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/GrantCollectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/InitVectorDatabaseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ListCollectionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ListNamespacesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3187 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifyAccountDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2730 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifyBackupPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2385 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConnectionStringRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1973 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceMaintainTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceSSLRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifyParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifySQLCollectorPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2646 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifySecurityIpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifyVectorConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/PauseInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2937 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/QueryCollectionDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/RebalanceDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ReleaseInstancePublicConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ResetAccountPasswordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/RestartDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ResumeInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/SetDBInstancePlanStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/SetDataShareInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1905 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/SwitchDBInstanceNetTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2994 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/UnloadSampleDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2972 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/UpdateDBInstancePlanRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3987 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/UpgradeDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2454 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/UpgradeDBVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2436 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/UpsertCollectionDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-08-02 01:59:30.000000 aliyun-python-sdk-gpdb-1.1.7/setup.py
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/LICENSE` & `aliyun-python-sdk-gpdb-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/PKG-INFO` & `aliyun-python-sdk-gpdb-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-gpdb
-Version: 1.1.6
+Version: 1.1.7
 Summary: The gpdb module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-gpdb
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/README.rst` & `aliyun-python-sdk-gpdb-1.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyun_python_sdk_gpdb.egg-info/PKG-INFO` & `aliyun-python-sdk-gpdb-1.1.7/aliyun_python_sdk_gpdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-gpdb
-Version: 1.1.6
+Version: 1.1.7
 Summary: The gpdb module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-gpdb
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyun_python_sdk_gpdb.egg-info/SOURCES.txt` & `aliyun-python-sdk-gpdb-1.1.7/aliyun_python_sdk_gpdb.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,101 +7,104 @@
 aliyun_python_sdk_gpdb.egg-info/SOURCES.txt
 aliyun_python_sdk_gpdb.egg-info/dependency_links.txt
 aliyun_python_sdk_gpdb.egg-info/requires.txt
 aliyun_python_sdk_gpdb.egg-info/top_level.txt
 aliyunsdkgpdb/__init__.py
 aliyunsdkgpdb/endpoint.py
 aliyunsdkgpdb/request/__init__.py
-aliyunsdkgpdb/request/v20160503/AddBuDBInstanceRelationRequest.py
 aliyunsdkgpdb/request/v20160503/AllocateInstancePublicConnectionRequest.py
 aliyunsdkgpdb/request/v20160503/CheckServiceLinkedRoleRequest.py
 aliyunsdkgpdb/request/v20160503/CreateAccountRequest.py
+aliyunsdkgpdb/request/v20160503/CreateCollectionRequest.py
 aliyunsdkgpdb/request/v20160503/CreateDBInstancePlanRequest.py
 aliyunsdkgpdb/request/v20160503/CreateDBInstanceRequest.py
-aliyunsdkgpdb/request/v20160503/CreateECSDBInstanceRequest.py
+aliyunsdkgpdb/request/v20160503/CreateNamespaceRequest.py
 aliyunsdkgpdb/request/v20160503/CreateSampleDataRequest.py
 aliyunsdkgpdb/request/v20160503/CreateServiceLinkedRoleRequest.py
+aliyunsdkgpdb/request/v20160503/CreateVectorIndexRequest.py
+aliyunsdkgpdb/request/v20160503/DeleteCollectionDataRequest.py
+aliyunsdkgpdb/request/v20160503/DeleteCollectionRequest.py
 aliyunsdkgpdb/request/v20160503/DeleteDBInstancePlanRequest.py
 aliyunsdkgpdb/request/v20160503/DeleteDBInstanceRequest.py
-aliyunsdkgpdb/request/v20160503/DeleteDatabaseRequest.py
+aliyunsdkgpdb/request/v20160503/DeleteNamespaceRequest.py
+aliyunsdkgpdb/request/v20160503/DeleteVectorIndexRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeAccountsRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeAvailableResourcesRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeBackupPolicyRequest.py
+aliyunsdkgpdb/request/v20160503/DescribeCollectionRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDBClusterNodeRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDBClusterPerformanceRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDBInstanceAttributeRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDataBloatRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDataSkewRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDiagnosisSummaryRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDBInstanceErrorLogRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDBInstanceIPArrayListRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDBInstanceIndexUsageRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDBInstanceNetInfoRequest.py
-aliyunsdkgpdb/request/v20160503/DescribeDBInstanceOnECSAttributeRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDBInstancePerformanceRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDBInstancePlansRequest.py
-aliyunsdkgpdb/request/v20160503/DescribeDBInstanceSQLPatternsRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDBInstanceSSLRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDBInstancesRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDataBackupsRequest.py
+aliyunsdkgpdb/request/v20160503/DescribeDataReDistributeInfoRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDataShareInstancesRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDataSharePerformanceRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDiagnosisDimensionsRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDiagnosisMonitorPerformanceRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDiagnosisRecordsRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDiagnosisSQLInfoRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeDownloadRecordsRequest.py
+aliyunsdkgpdb/request/v20160503/DescribeDownloadSQLLogsRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeHealthStatusRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeLogBackupsRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeModifyParameterLogRequest.py
+aliyunsdkgpdb/request/v20160503/DescribeNamespaceRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeParametersRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeRdsVSwitchsRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeRdsVpcsRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeRegionsRequest.py
-aliyunsdkgpdb/request/v20160503/DescribeResourceUsageRequest.py
-aliyunsdkgpdb/request/v20160503/DescribeSQLCollectorPolicyRequest.py
-aliyunsdkgpdb/request/v20160503/DescribeSQLLogByQueryIdRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeSQLLogCountRequest.py
-aliyunsdkgpdb/request/v20160503/DescribeSQLLogFilesRequest.py
-aliyunsdkgpdb/request/v20160503/DescribeSQLLogRecordsRequest.py
-aliyunsdkgpdb/request/v20160503/DescribeSQLLogsOnSliceRequest.py
-aliyunsdkgpdb/request/v20160503/DescribeSQLLogsRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeSQLLogsV2Request.py
 aliyunsdkgpdb/request/v20160503/DescribeSampleDataRequest.py
-aliyunsdkgpdb/request/v20160503/DescribeSlowLogRecordsRequest.py
-aliyunsdkgpdb/request/v20160503/DescribeSlowSQLLogsRequest.py
-aliyunsdkgpdb/request/v20160503/DescribeSpecificationRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeSupportFeaturesRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeTagsRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeUserEncryptionKeyListRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeWaitingSQLInfoRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeWaitingSQLRecordsRequest.py
 aliyunsdkgpdb/request/v20160503/DownloadDiagnosisRecordsRequest.py
+aliyunsdkgpdb/request/v20160503/DownloadSQLLogsRecordsRequest.py
+aliyunsdkgpdb/request/v20160503/GrantCollectionRequest.py
+aliyunsdkgpdb/request/v20160503/InitVectorDatabaseRequest.py
+aliyunsdkgpdb/request/v20160503/ListCollectionsRequest.py
+aliyunsdkgpdb/request/v20160503/ListNamespacesRequest.py
 aliyunsdkgpdb/request/v20160503/ListTagResourcesRequest.py
 aliyunsdkgpdb/request/v20160503/ModifyAccountDescriptionRequest.py
 aliyunsdkgpdb/request/v20160503/ModifyBackupPolicyRequest.py
-aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConnectionModeRequest.py
+aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConfigRequest.py
 aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConnectionStringRequest.py
 aliyunsdkgpdb/request/v20160503/ModifyDBInstanceDescriptionRequest.py
 aliyunsdkgpdb/request/v20160503/ModifyDBInstanceMaintainTimeRequest.py
-aliyunsdkgpdb/request/v20160503/ModifyDBInstanceNetworkTypeRequest.py
 aliyunsdkgpdb/request/v20160503/ModifyDBInstanceResourceGroupRequest.py
 aliyunsdkgpdb/request/v20160503/ModifyDBInstanceSSLRequest.py
 aliyunsdkgpdb/request/v20160503/ModifyParametersRequest.py
 aliyunsdkgpdb/request/v20160503/ModifySQLCollectorPolicyRequest.py
 aliyunsdkgpdb/request/v20160503/ModifySecurityIpsRequest.py
+aliyunsdkgpdb/request/v20160503/ModifyVectorConfigurationRequest.py
 aliyunsdkgpdb/request/v20160503/PauseInstanceRequest.py
+aliyunsdkgpdb/request/v20160503/QueryCollectionDataRequest.py
 aliyunsdkgpdb/request/v20160503/RebalanceDBInstanceRequest.py
 aliyunsdkgpdb/request/v20160503/ReleaseInstancePublicConnectionRequest.py
 aliyunsdkgpdb/request/v20160503/ResetAccountPasswordRequest.py
 aliyunsdkgpdb/request/v20160503/RestartDBInstanceRequest.py
 aliyunsdkgpdb/request/v20160503/ResumeInstanceRequest.py
 aliyunsdkgpdb/request/v20160503/SetDBInstancePlanStatusRequest.py
 aliyunsdkgpdb/request/v20160503/SetDataShareInstanceRequest.py
 aliyunsdkgpdb/request/v20160503/SwitchDBInstanceNetTypeRequest.py
 aliyunsdkgpdb/request/v20160503/TagResourcesRequest.py
 aliyunsdkgpdb/request/v20160503/UnloadSampleDataRequest.py
 aliyunsdkgpdb/request/v20160503/UntagResourcesRequest.py
 aliyunsdkgpdb/request/v20160503/UpdateDBInstancePlanRequest.py
 aliyunsdkgpdb/request/v20160503/UpgradeDBInstanceRequest.py
 aliyunsdkgpdb/request/v20160503/UpgradeDBVersionRequest.py
+aliyunsdkgpdb/request/v20160503/UpsertCollectionDataRequest.py
 aliyunsdkgpdb/request/v20160503/__init__.py
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/endpoint.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/AddBuDBInstanceRelationRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/PauseInstanceRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class AddBuDBInstanceRelationRequest(RpcRequest):
+class PauseInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'AddBuDBInstanceRelation')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'PauseInstance')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,12 +37,7 @@
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_BusinessUnit(self): # String
-		return self.get_query_params().get('BusinessUnit')
-
-	def set_BusinessUnit(self, BusinessUnit):  # String
-		self.add_query_param('BusinessUnit', BusinessUnit)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/AllocateInstancePublicConnectionRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/AllocateInstancePublicConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CheckServiceLinkedRoleRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/CheckServiceLinkedRoleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateAccountRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/CreateAccountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateDBInstancePlanRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/CreateDBInstancePlanRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateDBInstanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/CreateDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateECSDBInstanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeSQLLogsV2Request.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,152 +16,98 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class CreateECSDBInstanceRequest(RpcRequest):
+class DescribeSQLLogsV2Request(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'CreateECSDBInstance')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeSQLLogsV2')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_EngineVersion(self): # String
-		return self.get_query_params().get('EngineVersion')
+	def get_StartTime(self): # String
+		return self.get_query_params().get('StartTime')
 
-	def set_EngineVersion(self, EngineVersion):  # String
-		self.add_query_param('EngineVersion', EngineVersion)
-	def get_DBInstanceCategory(self): # String
-		return self.get_query_params().get('DBInstanceCategory')
+	def set_StartTime(self, StartTime):  # String
+		self.add_query_param('StartTime', StartTime)
+	def get_QueryKeywords(self): # String
+		return self.get_query_params().get('QueryKeywords')
+
+	def set_QueryKeywords(self, QueryKeywords):  # String
+		self.add_query_param('QueryKeywords', QueryKeywords)
+	def get_PageNumber(self): # String
+		return self.get_query_params().get('PageNumber')
 
-	def set_DBInstanceCategory(self, DBInstanceCategory):  # String
-		self.add_query_param('DBInstanceCategory', DBInstanceCategory)
+	def set_PageNumber(self, PageNumber):  # String
+		self.add_query_param('PageNumber', PageNumber)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
-	def get_EncryptionType(self): # String
-		return self.get_query_params().get('EncryptionType')
+	def get_Database(self): # String
+		return self.get_query_params().get('Database')
 
-	def set_EncryptionType(self, EncryptionType):  # String
-		self.add_query_param('EncryptionType', EncryptionType)
-	def get_DBInstanceDescription(self): # String
-		return self.get_query_params().get('DBInstanceDescription')
-
-	def set_DBInstanceDescription(self, DBInstanceDescription):  # String
-		self.add_query_param('DBInstanceDescription', DBInstanceDescription)
-	def get_Tags(self): # RepeatList
-		return self.get_query_params().get('Tag')
-
-	def set_Tags(self, Tag):  # RepeatList
-		for depth1 in range(len(Tag)):
-			if Tag[depth1].get('Value') is not None:
-				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
-			if Tag[depth1].get('Key') is not None:
-				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
-	def get_Period(self): # String
-		return self.get_query_params().get('Period')
-
-	def set_Period(self, Period):  # String
-		self.add_query_param('Period', Period)
-	def get_BackupId(self): # String
-		return self.get_query_params().get('BackupId')
-
-	def set_BackupId(self, BackupId):  # String
-		self.add_query_param('BackupId', BackupId)
-	def get_EncryptionKey(self): # String
-		return self.get_query_params().get('EncryptionKey')
-
-	def set_EncryptionKey(self, EncryptionKey):  # String
-		self.add_query_param('EncryptionKey', EncryptionKey)
-	def get_OwnerId(self): # Long
-		return self.get_query_params().get('OwnerId')
-
-	def set_OwnerId(self, OwnerId):  # Long
-		self.add_query_param('OwnerId', OwnerId)
-	def get_SecurityIPList(self): # String
-		return self.get_query_params().get('SecurityIPList')
-
-	def set_SecurityIPList(self, SecurityIPList):  # String
-		self.add_query_param('SecurityIPList', SecurityIPList)
-	def get_VSwitchId(self): # String
-		return self.get_query_params().get('VSwitchId')
-
-	def set_VSwitchId(self, VSwitchId):  # String
-		self.add_query_param('VSwitchId', VSwitchId)
-	def get_PrivateIpAddress(self): # String
-		return self.get_query_params().get('PrivateIpAddress')
-
-	def set_PrivateIpAddress(self, PrivateIpAddress):  # String
-		self.add_query_param('PrivateIpAddress', PrivateIpAddress)
-	def get_ZoneId(self): # String
-		return self.get_query_params().get('ZoneId')
-
-	def set_ZoneId(self, ZoneId):  # String
-		self.add_query_param('ZoneId', ZoneId)
-	def get_InstanceNetworkType(self): # String
-		return self.get_query_params().get('InstanceNetworkType')
-
-	def set_InstanceNetworkType(self, InstanceNetworkType):  # String
-		self.add_query_param('InstanceNetworkType', InstanceNetworkType)
-	def get_ClientToken(self): # String
-		return self.get_query_params().get('ClientToken')
-
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_query_param('ClientToken', ClientToken)
-	def get_InstanceSpec(self): # String
-		return self.get_query_params().get('InstanceSpec')
-
-	def set_InstanceSpec(self, InstanceSpec):  # String
-		self.add_query_param('InstanceSpec', InstanceSpec)
-	def get_StorageSize(self): # Integer
-		return self.get_query_params().get('StorageSize')
-
-	def set_StorageSize(self, StorageSize):  # Integer
-		self.add_query_param('StorageSize', StorageSize)
-	def get_SegStorageType(self): # String
-		return self.get_query_params().get('SegStorageType')
-
-	def set_SegStorageType(self, SegStorageType):  # String
-		self.add_query_param('SegStorageType', SegStorageType)
-	def get_MasterNodeNum(self): # Integer
-		return self.get_query_params().get('MasterNodeNum')
-
-	def set_MasterNodeNum(self, MasterNodeNum):  # Integer
-		self.add_query_param('MasterNodeNum', MasterNodeNum)
-	def get_SegNodeNum(self): # Integer
-		return self.get_query_params().get('SegNodeNum')
-
-	def set_SegNodeNum(self, SegNodeNum):  # Integer
-		self.add_query_param('SegNodeNum', SegNodeNum)
-	def get_Engine(self): # String
-		return self.get_query_params().get('Engine')
-
-	def set_Engine(self, Engine):  # String
-		self.add_query_param('Engine', Engine)
-	def get_UsedTime(self): # String
-		return self.get_query_params().get('UsedTime')
-
-	def set_UsedTime(self, UsedTime):  # String
-		self.add_query_param('UsedTime', UsedTime)
-	def get_VPCId(self): # String
-		return self.get_query_params().get('VPCId')
-
-	def set_VPCId(self, VPCId):  # String
-		self.add_query_param('VPCId', VPCId)
-	def get_PayType(self): # String
-		return self.get_query_params().get('PayType')
-
-	def set_PayType(self, PayType):  # String
-		self.add_query_param('PayType', PayType)
-	def get_SrcDbInstanceName(self): # String
-		return self.get_query_params().get('SrcDbInstanceName')
+	def set_Database(self, Database):  # String
+		self.add_query_param('Database', Database)
+	def get_SourceIP(self): # String
+		return self.get_query_params().get('SourceIP')
+
+	def set_SourceIP(self, SourceIP):  # String
+		self.add_query_param('SourceIP', SourceIP)
+	def get_MinExecuteCost(self): # String
+		return self.get_query_params().get('MinExecuteCost')
+
+	def set_MinExecuteCost(self, MinExecuteCost):  # String
+		self.add_query_param('MinExecuteCost', MinExecuteCost)
+	def get_PageSize(self): # String
+		return self.get_query_params().get('PageSize')
+
+	def set_PageSize(self, PageSize):  # String
+		self.add_query_param('PageSize', PageSize)
+	def get_DBInstanceId(self): # String
+		return self.get_query_params().get('DBInstanceId')
+
+	def set_DBInstanceId(self, DBInstanceId):  # String
+		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_MaxExecuteCost(self): # String
+		return self.get_query_params().get('MaxExecuteCost')
+
+	def set_MaxExecuteCost(self, MaxExecuteCost):  # String
+		self.add_query_param('MaxExecuteCost', MaxExecuteCost)
+	def get_ExecuteCost(self): # String
+		return self.get_query_params().get('ExecuteCost')
+
+	def set_ExecuteCost(self, ExecuteCost):  # String
+		self.add_query_param('ExecuteCost', ExecuteCost)
+	def get_ExecuteState(self): # String
+		return self.get_query_params().get('ExecuteState')
+
+	def set_ExecuteState(self, ExecuteState):  # String
+		self.add_query_param('ExecuteState', ExecuteState)
+	def get_EndTime(self): # String
+		return self.get_query_params().get('EndTime')
+
+	def set_EndTime(self, EndTime):  # String
+		self.add_query_param('EndTime', EndTime)
+	def get_OperationType(self): # String
+		return self.get_query_params().get('OperationType')
+
+	def set_OperationType(self, OperationType):  # String
+		self.add_query_param('OperationType', OperationType)
+	def get_OperationClass(self): # String
+		return self.get_query_params().get('OperationClass')
+
+	def set_OperationClass(self, OperationClass):  # String
+		self.add_query_param('OperationClass', OperationClass)
+	def get_User(self): # String
+		return self.get_query_params().get('User')
 
-	def set_SrcDbInstanceName(self, SrcDbInstanceName):  # String
-		self.add_query_param('SrcDbInstanceName', SrcDbInstanceName)
+	def set_User(self, User):  # String
+		self.add_query_param('User', User)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateSampleDataRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/CreateSampleDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateServiceLinkedRoleRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/CreateServiceLinkedRoleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DeleteDBInstancePlanRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DeleteDBInstancePlanRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DeleteDBInstanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DeleteDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DeleteDatabaseRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceIPArrayListRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DeleteDatabaseRequest(RpcRequest):
+class DescribeDBInstanceIPArrayListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DeleteDatabase')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeDBInstanceIPArrayList')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,12 +37,7 @@
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_DBName(self): # String
-		return self.get_query_params().get('DBName')
-
-	def set_DBName(self, DBName):  # String
-		self.add_query_param('DBName', DBName)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeAccountsRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeAccountsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeAvailableResourcesRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeAvailableResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeBackupPolicyRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeBackupPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBClusterNodeRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBClusterNodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBClusterPerformanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBClusterPerformanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceAttributeRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDataBloatRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDataBloatRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDataSkewRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDataSkewRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDiagnosisSummaryRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDiagnosisSummaryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceErrorLogRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceErrorLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceIPArrayListRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeSampleDataRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeDBInstanceIPArrayListRequest(RpcRequest):
+class DescribeSampleDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeDBInstanceIPArrayList')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeSampleData')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ResourceGroupId(self): # String
-		return self.get_query_params().get('ResourceGroupId')
-
-	def set_ResourceGroupId(self, ResourceGroupId):  # String
-		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_OwnerId(self): # Long
+		return self.get_query_params().get('OwnerId')
+
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceIndexUsageRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceIndexUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceNetInfoRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDownloadRecordsRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeDBInstanceNetInfoRequest(RpcRequest):
+class DescribeDownloadRecordsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeDBInstanceNetInfo')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeDownloadRecords')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceOnECSAttributeRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceSSLRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,28 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeDBInstanceOnECSAttributeRequest(RpcRequest):
+class DescribeDBInstanceSSLRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeDBInstanceOnECSAttribute')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeDBInstanceSSL')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_OwnerId(self): # Long
-		return self.get_query_params().get('OwnerId')
-
-	def set_OwnerId(self, OwnerId):  # Long
-		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstancePerformanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstancePerformanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstancePlansRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstancePlansRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceSQLPatternsRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDataBackupsRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,53 +16,63 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeDBInstanceSQLPatternsRequest(RpcRequest):
+class DescribeDataBackupsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeDBInstanceSQLPatterns')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeDataBackups')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_StartTime(self): # String
 		return self.get_query_params().get('StartTime')
 
 	def set_StartTime(self, StartTime):  # String
 		self.add_query_param('StartTime', StartTime)
-	def get_QueryKeywords(self): # String
-		return self.get_query_params().get('QueryKeywords')
+	def get_PageNumber(self): # Integer
+		return self.get_query_params().get('PageNumber')
 
-	def set_QueryKeywords(self, QueryKeywords):  # String
-		self.add_query_param('QueryKeywords', QueryKeywords)
-	def get_Database(self): # String
-		return self.get_query_params().get('Database')
-
-	def set_Database(self, Database):  # String
-		self.add_query_param('Database', Database)
-	def get_SourceIP(self): # String
-		return self.get_query_params().get('SourceIP')
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_DataType(self): # String
+		return self.get_query_params().get('DataType')
+
+	def set_DataType(self, DataType):  # String
+		self.add_query_param('DataType', DataType)
+	def get_PageSize(self): # Integer
+		return self.get_query_params().get('PageSize')
 
-	def set_SourceIP(self, SourceIP):  # String
-		self.add_query_param('SourceIP', SourceIP)
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_BackupId(self): # String
+		return self.get_query_params().get('BackupId')
+
+	def set_BackupId(self, BackupId):  # String
+		self.add_query_param('BackupId', BackupId)
 	def get_EndTime(self): # String
 		return self.get_query_params().get('EndTime')
 
 	def set_EndTime(self, EndTime):  # String
 		self.add_query_param('EndTime', EndTime)
-	def get_User(self): # String
-		return self.get_query_params().get('User')
+	def get_BackupStatus(self): # String
+		return self.get_query_params().get('BackupStatus')
+
+	def set_BackupStatus(self, BackupStatus):  # String
+		self.add_query_param('BackupStatus', BackupStatus)
+	def get_BackupMode(self): # String
+		return self.get_query_params().get('BackupMode')
 
-	def set_User(self, User):  # String
-		self.add_query_param('User', User)
+	def set_BackupMode(self, BackupMode):  # String
+		self.add_query_param('BackupMode', BackupMode)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceSSLRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisDimensionsRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeDBInstanceSSLRequest(RpcRequest):
+class DescribeDiagnosisDimensionsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeDBInstanceSSL')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeDiagnosisDimensions')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstancesRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDataBackupsRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DeleteCollectionRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,63 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeDataBackupsRequest(RpcRequest):
+class DeleteCollectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeDataBackups')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DeleteCollection')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_StartTime(self): # String
-		return self.get_query_params().get('StartTime')
-
-	def set_StartTime(self, StartTime):  # String
-		self.add_query_param('StartTime', StartTime)
-	def get_PageNumber(self): # Integer
-		return self.get_query_params().get('PageNumber')
-
-	def set_PageNumber(self, PageNumber):  # Integer
-		self.add_query_param('PageNumber', PageNumber)
-	def get_DataType(self): # String
-		return self.get_query_params().get('DataType')
-
-	def set_DataType(self, DataType):  # String
-		self.add_query_param('DataType', DataType)
-	def get_PageSize(self): # Integer
-		return self.get_query_params().get('PageSize')
-
-	def set_PageSize(self, PageSize):  # Integer
-		self.add_query_param('PageSize', PageSize)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_BackupId(self): # String
-		return self.get_query_params().get('BackupId')
+	def get_Collection(self): # String
+		return self.get_query_params().get('Collection')
 
-	def set_BackupId(self, BackupId):  # String
-		self.add_query_param('BackupId', BackupId)
-	def get_EndTime(self): # String
-		return self.get_query_params().get('EndTime')
-
-	def set_EndTime(self, EndTime):  # String
-		self.add_query_param('EndTime', EndTime)
-	def get_BackupStatus(self): # String
-		return self.get_query_params().get('BackupStatus')
-
-	def set_BackupStatus(self, BackupStatus):  # String
-		self.add_query_param('BackupStatus', BackupStatus)
-	def get_BackupMode(self): # String
-		return self.get_query_params().get('BackupMode')
+	def set_Collection(self, Collection):  # String
+		self.add_query_param('Collection', Collection)
+	def get_OwnerId(self): # Long
+		return self.get_query_params().get('OwnerId')
+
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_NamespacePassword(self): # String
+		return self.get_query_params().get('NamespacePassword')
+
+	def set_NamespacePassword(self, NamespacePassword):  # String
+		self.add_query_param('NamespacePassword', NamespacePassword)
+	def get_Namespace(self): # String
+		return self.get_query_params().get('Namespace')
 
-	def set_BackupMode(self, BackupMode):  # String
-		self.add_query_param('BackupMode', BackupMode)
+	def set_Namespace(self, Namespace):  # String
+		self.add_query_param('Namespace', Namespace)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDataShareInstancesRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDataShareInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDataSharePerformanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDataSharePerformanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisDimensionsRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeSupportFeaturesRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,23 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeDiagnosisDimensionsRequest(RpcRequest):
+class DescribeSupportFeaturesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeDiagnosisDimensions')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeSupportFeatures')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_OwnerId(self): # Long
+		return self.get_query_params().get('OwnerId')
+
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisMonitorPerformanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisMonitorPerformanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisRecordsRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisSQLInfoRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisSQLInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDownloadRecordsRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeHealthStatusRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,23 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeDownloadRecordsRequest(RpcRequest):
+class DescribeHealthStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeDownloadRecords')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeHealthStatus')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_Key(self): # String
+		return self.get_query_params().get('Key')
+
+	def set_Key(self, Key):  # String
+		self.add_query_param('Key', Key)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeHealthStatusRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeModifyParameterLogRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,28 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeHealthStatusRequest(RpcRequest):
+class DescribeModifyParameterLogRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeHealthStatus')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeModifyParameterLog')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_StartTime(self): # String
+		return self.get_query_params().get('StartTime')
+
+	def set_StartTime(self, StartTime):  # String
+		self.add_query_param('StartTime', StartTime)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_Key(self): # String
-		return self.get_query_params().get('Key')
+	def get_EndTime(self): # String
+		return self.get_query_params().get('EndTime')
 
-	def set_Key(self, Key):  # String
-		self.add_query_param('Key', Key)
+	def set_EndTime(self, EndTime):  # String
+		self.add_query_param('EndTime', EndTime)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeLogBackupsRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeLogBackupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeModifyParameterLogRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifyAccountDescriptionRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,33 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeModifyParameterLogRequest(RpcRequest):
+class ModifyAccountDescriptionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeModifyParameterLog')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'ModifyAccountDescription')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_StartTime(self): # String
-		return self.get_query_params().get('StartTime')
+	def get_AccountDescription(self): # String
+		return self.get_query_params().get('AccountDescription')
 
-	def set_StartTime(self, StartTime):  # String
-		self.add_query_param('StartTime', StartTime)
+	def set_AccountDescription(self, AccountDescription):  # String
+		self.add_query_param('AccountDescription', AccountDescription)
+	def get_AccountName(self): # String
+		return self.get_query_params().get('AccountName')
+
+	def set_AccountName(self, AccountName):  # String
+		self.add_query_param('AccountName', AccountName)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_EndTime(self): # String
-		return self.get_query_params().get('EndTime')
-
-	def set_EndTime(self, EndTime):  # String
-		self.add_query_param('EndTime', EndTime)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeParametersRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeParametersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeRdsVSwitchsRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeRdsVSwitchsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeRdsVpcsRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeRdsVpcsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeRegionsRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeResourceUsageRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDownloadSQLLogsRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeResourceUsageRequest(RpcRequest):
+class DescribeDownloadSQLLogsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeResourceUsage')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeDownloadSQLLogs')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLCollectorPolicyRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ResumeInstanceRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,23 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeSQLCollectorPolicyRequest(RpcRequest):
+class ResumeInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeSQLCollectorPolicy')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'ResumeInstance')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_OwnerId(self): # Long
+		return self.get_query_params().get('OwnerId')
+
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogByQueryIdRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifyParametersRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,28 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeSQLLogByQueryIdRequest(RpcRequest):
+class ModifyParametersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeSQLLogByQueryId')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'ModifyParameters')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ForceRestartInstance(self): # Boolean
+		return self.get_query_params().get('ForceRestartInstance')
+
+	def set_ForceRestartInstance(self, ForceRestartInstance):  # Boolean
+		self.add_query_param('ForceRestartInstance', ForceRestartInstance)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_QueryId(self): # String
-		return self.get_query_params().get('QueryId')
+	def get_Parameters(self): # String
+		return self.get_query_params().get('Parameters')
 
-	def set_QueryId(self, QueryId):  # String
-		self.add_query_param('QueryId', QueryId)
+	def set_Parameters(self, Parameters):  # String
+		self.add_query_param('Parameters', Parameters)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogCountRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeSQLLogCountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogFilesRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeWaitingSQLInfoRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,38 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeSQLLogFilesRequest(RpcRequest):
+class DescribeWaitingSQLInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeSQLLogFiles')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeWaitingSQLInfo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_PageNumber(self): # Integer
-		return self.get_query_params().get('PageNumber')
+	def get_PID(self): # String
+		return self.get_query_params().get('PID')
 
-	def set_PageNumber(self, PageNumber):  # Integer
-		self.add_query_param('PageNumber', PageNumber)
-	def get_PageSize(self): # Integer
-		return self.get_query_params().get('PageSize')
+	def set_PID(self, PID):  # String
+		self.add_query_param('PID', PID)
+	def get_Database(self): # String
+		return self.get_query_params().get('Database')
 
-	def set_PageSize(self, PageSize):  # Integer
-		self.add_query_param('PageSize', PageSize)
+	def set_Database(self, Database):  # String
+		self.add_query_param('Database', Database)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_FileName(self): # String
-		return self.get_query_params().get('FileName')
-
-	def set_FileName(self, FileName):  # String
-		self.add_query_param('FileName', FileName)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogRecordsRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeWaitingSQLRecordsRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,35 +16,35 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeSQLLogRecordsRequest(RpcRequest):
+class DescribeWaitingSQLRecordsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeSQLLogRecords')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeWaitingSQLRecords')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_QueryCondition(self): # String
+		return self.get_query_params().get('QueryCondition')
+
+	def set_QueryCondition(self, QueryCondition):  # String
+		self.add_query_param('QueryCondition', QueryCondition)
 	def get_StartTime(self): # String
 		return self.get_query_params().get('StartTime')
 
 	def set_StartTime(self, StartTime):  # String
 		self.add_query_param('StartTime', StartTime)
-	def get_QueryKeywords(self): # String
-		return self.get_query_params().get('QueryKeywords')
-
-	def set_QueryKeywords(self, QueryKeywords):  # String
-		self.add_query_param('QueryKeywords', QueryKeywords)
 	def get_PageNumber(self): # Integer
 		return self.get_query_params().get('PageNumber')
 
 	def set_PageNumber(self, PageNumber):  # Integer
 		self.add_query_param('PageNumber', PageNumber)
 	def get_Database(self): # String
 		return self.get_query_params().get('Database')
@@ -57,22 +57,27 @@
 	def set_PageSize(self, PageSize):  # Integer
 		self.add_query_param('PageSize', PageSize)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_Keyword(self): # String
+		return self.get_query_params().get('Keyword')
+
+	def set_Keyword(self, Keyword):  # String
+		self.add_query_param('Keyword', Keyword)
+	def get_Order(self): # String
+		return self.get_query_params().get('Order')
+
+	def set_Order(self, Order):  # String
+		self.add_query_param('Order', Order)
 	def get_EndTime(self): # String
 		return self.get_query_params().get('EndTime')
 
 	def set_EndTime(self, EndTime):  # String
 		self.add_query_param('EndTime', EndTime)
-	def get_Form(self): # String
-		return self.get_query_params().get('Form')
-
-	def set_Form(self, Form):  # String
-		self.add_query_param('Form', Form)
 	def get_User(self): # String
 		return self.get_query_params().get('User')
 
 	def set_User(self, User):  # String
 		self.add_query_param('User', User)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogsOnSliceRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/CreateVectorIndexRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,58 +16,58 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeSQLLogsOnSliceRequest(RpcRequest):
+class CreateVectorIndexRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeSQLLogsOnSlice')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'CreateVectorIndex')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_SliceId(self): # String
-		return self.get_query_params().get('SliceId')
+	def get_ManagerAccount(self): # String
+		return self.get_query_params().get('ManagerAccount')
 
-	def set_SliceId(self, SliceId):  # String
-		self.add_query_param('SliceId', SliceId)
-	def get_PageNumber(self): # Integer
-		return self.get_query_params().get('PageNumber')
-
-	def set_PageNumber(self, PageNumber):  # Integer
-		self.add_query_param('PageNumber', PageNumber)
-	def get_MinExecuteCost(self): # String
-		return self.get_query_params().get('MinExecuteCost')
-
-	def set_MinExecuteCost(self, MinExecuteCost):  # String
-		self.add_query_param('MinExecuteCost', MinExecuteCost)
-	def get_PageSize(self): # Integer
-		return self.get_query_params().get('PageSize')
-
-	def set_PageSize(self, PageSize):  # Integer
-		self.add_query_param('PageSize', PageSize)
+	def set_ManagerAccount(self, ManagerAccount):  # String
+		self.add_query_param('ManagerAccount', ManagerAccount)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_MaxExecuteCost(self): # String
-		return self.get_query_params().get('MaxExecuteCost')
+	def get_Dimension(self): # Integer
+		return self.get_query_params().get('Dimension')
 
-	def set_MaxExecuteCost(self, MaxExecuteCost):  # String
-		self.add_query_param('MaxExecuteCost', MaxExecuteCost)
-	def get_ExecuteState(self): # String
-		return self.get_query_params().get('ExecuteState')
-
-	def set_ExecuteState(self, ExecuteState):  # String
-		self.add_query_param('ExecuteState', ExecuteState)
-	def get_QueryId(self): # String
-		return self.get_query_params().get('QueryId')
+	def set_Dimension(self, Dimension):  # Integer
+		self.add_query_param('Dimension', Dimension)
+	def get_ManagerAccountPassword(self): # String
+		return self.get_query_params().get('ManagerAccountPassword')
+
+	def set_ManagerAccountPassword(self, ManagerAccountPassword):  # String
+		self.add_query_param('ManagerAccountPassword', ManagerAccountPassword)
+	def get_Collection(self): # String
+		return self.get_query_params().get('Collection')
+
+	def set_Collection(self, Collection):  # String
+		self.add_query_param('Collection', Collection)
+	def get_OwnerId(self): # Long
+		return self.get_query_params().get('OwnerId')
+
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_Namespace(self): # String
+		return self.get_query_params().get('Namespace')
+
+	def set_Namespace(self, Namespace):  # String
+		self.add_query_param('Namespace', Namespace)
+	def get_Metrics(self): # String
+		return self.get_query_params().get('Metrics')
 
-	def set_QueryId(self, QueryId):  # String
-		self.add_query_param('QueryId', QueryId)
+	def set_Metrics(self, Metrics):  # String
+		self.add_query_param('Metrics', Metrics)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogsRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DownloadSQLLogsRecordsRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeSQLLogsRequest(RpcRequest):
+class DownloadSQLLogsRecordsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeSQLLogs')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DownloadSQLLogsRecords')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -67,14 +67,19 @@
 	def set_PageSize(self, PageSize):  # Integer
 		self.add_query_param('PageSize', PageSize)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_Lang(self): # String
+		return self.get_query_params().get('Lang')
+
+	def set_Lang(self, Lang):  # String
+		self.add_query_param('Lang', Lang)
 	def get_MaxExecuteCost(self): # String
 		return self.get_query_params().get('MaxExecuteCost')
 
 	def set_MaxExecuteCost(self, MaxExecuteCost):  # String
 		self.add_query_param('MaxExecuteCost', MaxExecuteCost)
 	def get_ExecuteCost(self): # String
 		return self.get_query_params().get('ExecuteCost')
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogsV2Request.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/UpgradeDBInstanceRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,98 +16,83 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeSQLLogsV2Request(RpcRequest):
+class UpgradeDBInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeSQLLogsV2')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'UpgradeDBInstance')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_StartTime(self): # String
-		return self.get_query_params().get('StartTime')
+	def get_InstanceSpec(self): # String
+		return self.get_query_params().get('InstanceSpec')
 
-	def set_StartTime(self, StartTime):  # String
-		self.add_query_param('StartTime', StartTime)
-	def get_QueryKeywords(self): # String
-		return self.get_query_params().get('QueryKeywords')
-
-	def set_QueryKeywords(self, QueryKeywords):  # String
-		self.add_query_param('QueryKeywords', QueryKeywords)
-	def get_PageNumber(self): # String
-		return self.get_query_params().get('PageNumber')
+	def set_InstanceSpec(self, InstanceSpec):  # String
+		self.add_query_param('InstanceSpec', InstanceSpec)
+	def get_StorageSize(self): # String
+		return self.get_query_params().get('StorageSize')
+
+	def set_StorageSize(self, StorageSize):  # String
+		self.add_query_param('StorageSize', StorageSize)
+	def get_SegStorageType(self): # String
+		return self.get_query_params().get('SegStorageType')
+
+	def set_SegStorageType(self, SegStorageType):  # String
+		self.add_query_param('SegStorageType', SegStorageType)
+	def get_MasterNodeNum(self): # String
+		return self.get_query_params().get('MasterNodeNum')
+
+	def set_MasterNodeNum(self, MasterNodeNum):  # String
+		self.add_query_param('MasterNodeNum', MasterNodeNum)
+	def get_UpgradeType(self): # Long
+		return self.get_query_params().get('UpgradeType')
 
-	def set_PageNumber(self, PageNumber):  # String
-		self.add_query_param('PageNumber', PageNumber)
+	def set_UpgradeType(self, UpgradeType):  # Long
+		self.add_query_param('UpgradeType', UpgradeType)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
-	def get_Database(self): # String
-		return self.get_query_params().get('Database')
+	def get_SegNodeNum(self): # String
+		return self.get_query_params().get('SegNodeNum')
 
-	def set_Database(self, Database):  # String
-		self.add_query_param('Database', Database)
-	def get_SourceIP(self): # String
-		return self.get_query_params().get('SourceIP')
-
-	def set_SourceIP(self, SourceIP):  # String
-		self.add_query_param('SourceIP', SourceIP)
-	def get_MinExecuteCost(self): # String
-		return self.get_query_params().get('MinExecuteCost')
-
-	def set_MinExecuteCost(self, MinExecuteCost):  # String
-		self.add_query_param('MinExecuteCost', MinExecuteCost)
-	def get_PageSize(self): # String
-		return self.get_query_params().get('PageSize')
-
-	def set_PageSize(self, PageSize):  # String
-		self.add_query_param('PageSize', PageSize)
+	def set_SegNodeNum(self, SegNodeNum):  # String
+		self.add_query_param('SegNodeNum', SegNodeNum)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_MaxExecuteCost(self): # String
-		return self.get_query_params().get('MaxExecuteCost')
+	def get_DBInstanceGroupCount(self): # String
+		return self.get_query_params().get('DBInstanceGroupCount')
 
-	def set_MaxExecuteCost(self, MaxExecuteCost):  # String
-		self.add_query_param('MaxExecuteCost', MaxExecuteCost)
-	def get_ExecuteCost(self): # String
-		return self.get_query_params().get('ExecuteCost')
-
-	def set_ExecuteCost(self, ExecuteCost):  # String
-		self.add_query_param('ExecuteCost', ExecuteCost)
-	def get_ExecuteState(self): # String
-		return self.get_query_params().get('ExecuteState')
-
-	def set_ExecuteState(self, ExecuteState):  # String
-		self.add_query_param('ExecuteState', ExecuteState)
-	def get_EndTime(self): # String
-		return self.get_query_params().get('EndTime')
-
-	def set_EndTime(self, EndTime):  # String
-		self.add_query_param('EndTime', EndTime)
-	def get_OperationType(self): # String
-		return self.get_query_params().get('OperationType')
-
-	def set_OperationType(self, OperationType):  # String
-		self.add_query_param('OperationType', OperationType)
-	def get_OperationClass(self): # String
-		return self.get_query_params().get('OperationClass')
-
-	def set_OperationClass(self, OperationClass):  # String
-		self.add_query_param('OperationClass', OperationClass)
-	def get_User(self): # String
-		return self.get_query_params().get('User')
+	def set_DBInstanceGroupCount(self, DBInstanceGroupCount):  # String
+		self.add_query_param('DBInstanceGroupCount', DBInstanceGroupCount)
+	def get_OwnerId(self): # Long
+		return self.get_query_params().get('OwnerId')
+
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_SegDiskPerformanceLevel(self): # String
+		return self.get_query_params().get('SegDiskPerformanceLevel')
+
+	def set_SegDiskPerformanceLevel(self, SegDiskPerformanceLevel):  # String
+		self.add_query_param('SegDiskPerformanceLevel', SegDiskPerformanceLevel)
+	def get_DBInstanceClass(self): # String
+		return self.get_query_params().get('DBInstanceClass')
+
+	def set_DBInstanceClass(self, DBInstanceClass):  # String
+		self.add_query_param('DBInstanceClass', DBInstanceClass)
+	def get_PayType(self): # String
+		return self.get_query_params().get('PayType')
 
-	def set_User(self, User):  # String
-		self.add_query_param('User', User)
+	def set_PayType(self, PayType):  # String
+		self.add_query_param('PayType', PayType)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSampleDataRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/UnloadSampleDataRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeSampleDataRequest(RpcRequest):
+class UnloadSampleDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeSampleData')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'UnloadSampleData')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSlowLogRecordsRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceMaintainTimeRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,53 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeSlowLogRecordsRequest(RpcRequest):
+class ModifyDBInstanceMaintainTimeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeSlowLogRecords')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'ModifyDBInstanceMaintainTime')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_StartTime(self): # String
 		return self.get_query_params().get('StartTime')
 
 	def set_StartTime(self, StartTime):  # String
 		self.add_query_param('StartTime', StartTime)
-	def get_PageNumber(self): # Integer
-		return self.get_query_params().get('PageNumber')
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
 
-	def set_PageNumber(self, PageNumber):  # Integer
-		self.add_query_param('PageNumber', PageNumber)
-	def get_PageSize(self): # Integer
-		return self.get_query_params().get('PageSize')
-
-	def set_PageSize(self, PageSize):  # Integer
-		self.add_query_param('PageSize', PageSize)
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_SQLId(self): # Long
-		return self.get_query_params().get('SQLId')
-
-	def set_SQLId(self, SQLId):  # Long
-		self.add_query_param('SQLId', SQLId)
 	def get_EndTime(self): # String
 		return self.get_query_params().get('EndTime')
 
 	def set_EndTime(self, EndTime):  # String
 		self.add_query_param('EndTime', EndTime)
-	def get_DBName(self): # String
-		return self.get_query_params().get('DBName')
-
-	def set_DBName(self, DBName):  # String
-		self.add_query_param('DBName', DBName)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSlowSQLLogsRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/UpdateDBInstancePlanRequest.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,88 +16,58 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeSlowSQLLogsRequest(RpcRequest):
+class UpdateDBInstancePlanRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeSlowSQLLogs')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'UpdateDBInstancePlan')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_StartTime(self): # String
-		return self.get_query_params().get('StartTime')
+	def get_PlanStartDate(self): # String
+		return self.get_query_params().get('PlanStartDate')
 
-	def set_StartTime(self, StartTime):  # String
-		self.add_query_param('StartTime', StartTime)
-	def get_QueryKeywords(self): # String
-		return self.get_query_params().get('QueryKeywords')
-
-	def set_QueryKeywords(self, QueryKeywords):  # String
-		self.add_query_param('QueryKeywords', QueryKeywords)
-	def get_PageNumber(self): # Integer
-		return self.get_query_params().get('PageNumber')
-
-	def set_PageNumber(self, PageNumber):  # Integer
-		self.add_query_param('PageNumber', PageNumber)
-	def get_Database(self): # String
-		return self.get_query_params().get('Database')
-
-	def set_Database(self, Database):  # String
-		self.add_query_param('Database', Database)
-	def get_SourceIP(self): # String
-		return self.get_query_params().get('SourceIP')
-
-	def set_SourceIP(self, SourceIP):  # String
-		self.add_query_param('SourceIP', SourceIP)
-	def get_MinExecuteCost(self): # String
-		return self.get_query_params().get('MinExecuteCost')
-
-	def set_MinExecuteCost(self, MinExecuteCost):  # String
-		self.add_query_param('MinExecuteCost', MinExecuteCost)
-	def get_PageSize(self): # Integer
-		return self.get_query_params().get('PageSize')
+	def set_PlanStartDate(self, PlanStartDate):  # String
+		self.add_query_param('PlanStartDate', PlanStartDate)
+	def get_PlanConfig(self): # String
+		return self.get_query_params().get('PlanConfig')
+
+	def set_PlanConfig(self, PlanConfig):  # String
+		self.add_query_param('PlanConfig', PlanConfig)
+	def get_PlanName(self): # String
+		return self.get_query_params().get('PlanName')
 
-	def set_PageSize(self, PageSize):  # Integer
-		self.add_query_param('PageSize', PageSize)
+	def set_PlanName(self, PlanName):  # String
+		self.add_query_param('PlanName', PlanName)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_MaxExecuteCost(self): # String
-		return self.get_query_params().get('MaxExecuteCost')
+	def get_PlanDesc(self): # String
+		return self.get_query_params().get('PlanDesc')
 
-	def set_MaxExecuteCost(self, MaxExecuteCost):  # String
-		self.add_query_param('MaxExecuteCost', MaxExecuteCost)
-	def get_ExecuteState(self): # String
-		return self.get_query_params().get('ExecuteState')
-
-	def set_ExecuteState(self, ExecuteState):  # String
-		self.add_query_param('ExecuteState', ExecuteState)
-	def get_EndTime(self): # String
-		return self.get_query_params().get('EndTime')
-
-	def set_EndTime(self, EndTime):  # String
-		self.add_query_param('EndTime', EndTime)
-	def get_OperationType(self): # String
-		return self.get_query_params().get('OperationType')
-
-	def set_OperationType(self, OperationType):  # String
-		self.add_query_param('OperationType', OperationType)
-	def get_OperationClass(self): # String
-		return self.get_query_params().get('OperationClass')
-
-	def set_OperationClass(self, OperationClass):  # String
-		self.add_query_param('OperationClass', OperationClass)
-	def get_User(self): # String
-		return self.get_query_params().get('User')
+	def set_PlanDesc(self, PlanDesc):  # String
+		self.add_query_param('PlanDesc', PlanDesc)
+	def get_OwnerId(self): # Long
+		return self.get_query_params().get('OwnerId')
+
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_PlanEndDate(self): # String
+		return self.get_query_params().get('PlanEndDate')
+
+	def set_PlanEndDate(self, PlanEndDate):  # String
+		self.add_query_param('PlanEndDate', PlanEndDate)
+	def get_PlanId(self): # String
+		return self.get_query_params().get('PlanId')
 
-	def set_User(self, User):  # String
-		self.add_query_param('User', User)
+	def set_PlanId(self, PlanId):  # String
+		self.add_query_param('PlanId', PlanId)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSpecificationRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ListNamespacesRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,43 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeSpecificationRequest(RpcRequest):
+class ListNamespacesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeSpecification')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'ListNamespaces')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_StorageType(self): # String
-		return self.get_query_params().get('StorageType')
+	def get_ManagerAccount(self): # String
+		return self.get_query_params().get('ManagerAccount')
 
-	def set_StorageType(self, StorageType):  # String
-		self.add_query_param('StorageType', StorageType)
-	def get_CpuCores(self): # Integer
-		return self.get_query_params().get('CpuCores')
-
-	def set_CpuCores(self, CpuCores):  # Integer
-		self.add_query_param('CpuCores', CpuCores)
+	def set_ManagerAccount(self, ManagerAccount):  # String
+		self.add_query_param('ManagerAccount', ManagerAccount)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_TotalNodeNum(self): # Integer
-		return self.get_query_params().get('TotalNodeNum')
+	def get_ManagerAccountPassword(self): # String
+		return self.get_query_params().get('ManagerAccountPassword')
 
-	def set_TotalNodeNum(self, TotalNodeNum):  # Integer
-		self.add_query_param('TotalNodeNum', TotalNodeNum)
+	def set_ManagerAccountPassword(self, ManagerAccountPassword):  # String
+		self.add_query_param('ManagerAccountPassword', ManagerAccountPassword)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSupportFeaturesRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDataReDistributeInfoRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeSupportFeaturesRequest(RpcRequest):
+class DescribeDataReDistributeInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeSupportFeatures')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeDataReDistributeInfo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeTagsRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeUserEncryptionKeyListRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeUserEncryptionKeyListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeWaitingSQLInfoRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeNamespaceRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,33 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeWaitingSQLInfoRequest(RpcRequest):
+class DescribeNamespaceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeWaitingSQLInfo')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeNamespace')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_PID(self): # String
-		return self.get_query_params().get('PID')
+	def get_ManagerAccount(self): # String
+		return self.get_query_params().get('ManagerAccount')
 
-	def set_PID(self, PID):  # String
-		self.add_query_param('PID', PID)
-	def get_Database(self): # String
-		return self.get_query_params().get('Database')
-
-	def set_Database(self, Database):  # String
-		self.add_query_param('Database', Database)
+	def set_ManagerAccount(self, ManagerAccount):  # String
+		self.add_query_param('ManagerAccount', ManagerAccount)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_ManagerAccountPassword(self): # String
+		return self.get_query_params().get('ManagerAccountPassword')
+
+	def set_ManagerAccountPassword(self, ManagerAccountPassword):  # String
+		self.add_query_param('ManagerAccountPassword', ManagerAccountPassword)
+	def get_OwnerId(self): # Long
+		return self.get_query_params().get('OwnerId')
+
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_Namespace(self): # String
+		return self.get_query_params().get('Namespace')
+
+	def set_Namespace(self, Namespace):  # String
+		self.add_query_param('Namespace', Namespace)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeWaitingSQLRecordsRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DownloadDiagnosisRecordsRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DescribeWaitingSQLRecordsRequest(RpcRequest):
+class DownloadDiagnosisRecordsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeWaitingSQLRecords')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DownloadDiagnosisRecords')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,44 +37,34 @@
 	def set_QueryCondition(self, QueryCondition):  # String
 		self.add_query_param('QueryCondition', QueryCondition)
 	def get_StartTime(self): # String
 		return self.get_query_params().get('StartTime')
 
 	def set_StartTime(self, StartTime):  # String
 		self.add_query_param('StartTime', StartTime)
-	def get_PageNumber(self): # Integer
-		return self.get_query_params().get('PageNumber')
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
 
-	def set_PageNumber(self, PageNumber):  # Integer
-		self.add_query_param('PageNumber', PageNumber)
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_Database(self): # String
 		return self.get_query_params().get('Database')
 
 	def set_Database(self, Database):  # String
 		self.add_query_param('Database', Database)
-	def get_PageSize(self): # Integer
-		return self.get_query_params().get('PageSize')
-
-	def set_PageSize(self, PageSize):  # Integer
-		self.add_query_param('PageSize', PageSize)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_Keyword(self): # String
-		return self.get_query_params().get('Keyword')
-
-	def set_Keyword(self, Keyword):  # String
-		self.add_query_param('Keyword', Keyword)
-	def get_Order(self): # String
-		return self.get_query_params().get('Order')
+	def get_Lang(self): # String
+		return self.get_query_params().get('Lang')
 
-	def set_Order(self, Order):  # String
-		self.add_query_param('Order', Order)
+	def set_Lang(self, Lang):  # String
+		self.add_query_param('Lang', Lang)
 	def get_EndTime(self): # String
 		return self.get_query_params().get('EndTime')
 
 	def set_EndTime(self, EndTime):  # String
 		self.add_query_param('EndTime', EndTime)
 	def get_User(self): # String
 		return self.get_query_params().get('User')
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DownloadDiagnosisRecordsRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/CreateCollectionRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,58 +16,68 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class DownloadDiagnosisRecordsRequest(RpcRequest):
+class CreateCollectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DownloadDiagnosisRecords')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'CreateCollection')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_QueryCondition(self): # String
-		return self.get_query_params().get('QueryCondition')
+	def get_Metadata(self): # String
+		return self.get_query_params().get('Metadata')
 
-	def set_QueryCondition(self, QueryCondition):  # String
-		self.add_query_param('QueryCondition', QueryCondition)
-	def get_StartTime(self): # String
-		return self.get_query_params().get('StartTime')
-
-	def set_StartTime(self, StartTime):  # String
-		self.add_query_param('StartTime', StartTime)
-	def get_ResourceGroupId(self): # String
-		return self.get_query_params().get('ResourceGroupId')
-
-	def set_ResourceGroupId(self, ResourceGroupId):  # String
-		self.add_query_param('ResourceGroupId', ResourceGroupId)
-	def get_Database(self): # String
-		return self.get_query_params().get('Database')
+	def set_Metadata(self, Metadata):  # String
+		self.add_query_param('Metadata', Metadata)
+	def get_FullTextRetrievalFields(self): # String
+		return self.get_query_params().get('FullTextRetrievalFields')
+
+	def set_FullTextRetrievalFields(self, FullTextRetrievalFields):  # String
+		self.add_query_param('FullTextRetrievalFields', FullTextRetrievalFields)
+	def get_ManagerAccount(self): # String
+		return self.get_query_params().get('ManagerAccount')
 
-	def set_Database(self, Database):  # String
-		self.add_query_param('Database', Database)
+	def set_ManagerAccount(self, ManagerAccount):  # String
+		self.add_query_param('ManagerAccount', ManagerAccount)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_Lang(self): # String
-		return self.get_query_params().get('Lang')
+	def get_Dimension(self): # Long
+		return self.get_query_params().get('Dimension')
 
-	def set_Lang(self, Lang):  # String
-		self.add_query_param('Lang', Lang)
-	def get_EndTime(self): # String
-		return self.get_query_params().get('EndTime')
-
-	def set_EndTime(self, EndTime):  # String
-		self.add_query_param('EndTime', EndTime)
-	def get_User(self): # String
-		return self.get_query_params().get('User')
+	def set_Dimension(self, Dimension):  # Long
+		self.add_query_param('Dimension', Dimension)
+	def get_ManagerAccountPassword(self): # String
+		return self.get_query_params().get('ManagerAccountPassword')
+
+	def set_ManagerAccountPassword(self, ManagerAccountPassword):  # String
+		self.add_query_param('ManagerAccountPassword', ManagerAccountPassword)
+	def get_Collection(self): # String
+		return self.get_query_params().get('Collection')
+
+	def set_Collection(self, Collection):  # String
+		self.add_query_param('Collection', Collection)
+	def get_OwnerId(self): # Long
+		return self.get_query_params().get('OwnerId')
+
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_Parser(self): # String
+		return self.get_query_params().get('Parser')
+
+	def set_Parser(self, Parser):  # String
+		self.add_query_param('Parser', Parser)
+	def get_Namespace(self): # String
+		return self.get_query_params().get('Namespace')
 
-	def set_User(self, User):  # String
-		self.add_query_param('User', User)
+	def set_Namespace(self, Namespace):  # String
+		self.add_query_param('Namespace', Namespace)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ListTagResourcesRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ListTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyAccountDescriptionRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceDescriptionRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,33 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class ModifyAccountDescriptionRequest(RpcRequest):
+class ModifyDBInstanceDescriptionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'ModifyAccountDescription')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'ModifyDBInstanceDescription')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_AccountDescription(self): # String
-		return self.get_query_params().get('AccountDescription')
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
 
-	def set_AccountDescription(self, AccountDescription):  # String
-		self.add_query_param('AccountDescription', AccountDescription)
-	def get_AccountName(self): # String
-		return self.get_query_params().get('AccountName')
-
-	def set_AccountName(self, AccountName):  # String
-		self.add_query_param('AccountName', AccountName)
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_DBInstanceDescription(self): # String
+		return self.get_query_params().get('DBInstanceDescription')
+
+	def set_DBInstanceDescription(self, DBInstanceDescription):  # String
+		self.add_query_param('DBInstanceDescription', DBInstanceDescription)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyBackupPolicyRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifyBackupPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConnectionModeRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/SwitchDBInstanceNetTypeRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,28 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class ModifyDBInstanceConnectionModeRequest(RpcRequest):
+class SwitchDBInstanceNetTypeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'ModifyDBInstanceConnectionMode')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'SwitchDBInstanceNetType')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ConnectionMode(self): # String
-		return self.get_query_params().get('ConnectionMode')
+	def get_ConnectionStringPrefix(self): # String
+		return self.get_query_params().get('ConnectionStringPrefix')
 
-	def set_ConnectionMode(self, ConnectionMode):  # String
-		self.add_query_param('ConnectionMode', ConnectionMode)
+	def set_ConnectionStringPrefix(self, ConnectionStringPrefix):  # String
+		self.add_query_param('ConnectionStringPrefix', ConnectionStringPrefix)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_Port(self): # String
+		return self.get_query_params().get('Port')
+
+	def set_Port(self, Port):  # String
+		self.add_query_param('Port', Port)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConnectionStringRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConnectionStringRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceDescriptionRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/RebalanceDBInstanceRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,33 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class ModifyDBInstanceDescriptionRequest(RpcRequest):
+class RebalanceDBInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'ModifyDBInstanceDescription')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'RebalanceDBInstance')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ResourceGroupId(self): # String
-		return self.get_query_params().get('ResourceGroupId')
+	def get_ClientToken(self): # String
+		return self.get_query_params().get('ClientToken')
 
-	def set_ResourceGroupId(self, ResourceGroupId):  # String
-		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def set_ClientToken(self, ClientToken):  # String
+		self.add_query_param('ClientToken', ClientToken)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_DBInstanceDescription(self): # String
-		return self.get_query_params().get('DBInstanceDescription')
-
-	def set_DBInstanceDescription(self, DBInstanceDescription):  # String
-		self.add_query_param('DBInstanceDescription', DBInstanceDescription)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceMaintainTimeRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConfigRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,38 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class ModifyDBInstanceMaintainTimeRequest(RpcRequest):
+class ModifyDBInstanceConfigRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'ModifyDBInstanceMaintainTime')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'ModifyDBInstanceConfig')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_StartTime(self): # String
-		return self.get_query_params().get('StartTime')
-
-	def set_StartTime(self, StartTime):  # String
-		self.add_query_param('StartTime', StartTime)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_EndTime(self): # String
-		return self.get_query_params().get('EndTime')
+	def get_DBInstanceDescription(self): # String
+		return self.get_query_params().get('DBInstanceDescription')
+
+	def set_DBInstanceDescription(self, DBInstanceDescription):  # String
+		self.add_query_param('DBInstanceDescription', DBInstanceDescription)
+	def get_ServerlessResource(self): # Integer
+		return self.get_query_params().get('ServerlessResource')
+
+	def set_ServerlessResource(self, ServerlessResource):  # Integer
+		self.add_query_param('ServerlessResource', ServerlessResource)
+	def get_IdleTime(self): # Integer
+		return self.get_query_params().get('IdleTime')
 
-	def set_EndTime(self, EndTime):  # String
-		self.add_query_param('EndTime', EndTime)
+	def set_IdleTime(self, IdleTime):  # Integer
+		self.add_query_param('IdleTime', IdleTime)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceNetworkTypeRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ResetAccountPasswordRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,43 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class ModifyDBInstanceNetworkTypeRequest(RpcRequest):
+class ResetAccountPasswordRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'ModifyDBInstanceNetworkType')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'ResetAccountPassword')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_AccountName(self): # String
+		return self.get_query_params().get('AccountName')
+
+	def set_AccountName(self, AccountName):  # String
+		self.add_query_param('AccountName', AccountName)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_VSwitchId(self): # String
-		return self.get_query_params().get('VSwitchId')
-
-	def set_VSwitchId(self, VSwitchId):  # String
-		self.add_query_param('VSwitchId', VSwitchId)
-	def get_PrivateIpAddress(self): # String
-		return self.get_query_params().get('PrivateIpAddress')
-
-	def set_PrivateIpAddress(self, PrivateIpAddress):  # String
-		self.add_query_param('PrivateIpAddress', PrivateIpAddress)
-	def get_VPCId(self): # String
-		return self.get_query_params().get('VPCId')
-
-	def set_VPCId(self, VPCId):  # String
-		self.add_query_param('VPCId', VPCId)
-	def get_InstanceNetworkType(self): # String
-		return self.get_query_params().get('InstanceNetworkType')
+	def get_AccountPassword(self): # String
+		return self.get_query_params().get('AccountPassword')
 
-	def set_InstanceNetworkType(self, InstanceNetworkType):  # String
-		self.add_query_param('InstanceNetworkType', InstanceNetworkType)
+	def set_AccountPassword(self, AccountPassword):  # String
+		self.add_query_param('AccountPassword', AccountPassword)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceResourceGroupRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceSSLRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceSSLRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyParametersRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceNetInfoRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,33 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class ModifyParametersRequest(RpcRequest):
+class DescribeDBInstanceNetInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'ModifyParameters')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeDBInstanceNetInfo')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ForceRestartInstance(self): # Boolean
-		return self.get_query_params().get('ForceRestartInstance')
+	def get_ConnectionString(self): # String
+		return self.get_query_params().get('ConnectionString')
 
-	def set_ForceRestartInstance(self, ForceRestartInstance):  # Boolean
-		self.add_query_param('ForceRestartInstance', ForceRestartInstance)
+	def set_ConnectionString(self, ConnectionString):  # String
+		self.add_query_param('ConnectionString', ConnectionString)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_Parameters(self): # String
-		return self.get_query_params().get('Parameters')
-
-	def set_Parameters(self, Parameters):  # String
-		self.add_query_param('Parameters', Parameters)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifySQLCollectorPolicyRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifySQLCollectorPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifySecurityIpsRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifySecurityIpsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/PauseInstanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/RestartDBInstanceRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class PauseInstanceRequest(RpcRequest):
+class RestartDBInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'PauseInstance')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'RestartDBInstance')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ClientToken(self): # String
+		return self.get_query_params().get('ClientToken')
+
+	def set_ClientToken(self, ClientToken):  # String
+		self.add_query_param('ClientToken', ClientToken)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_OwnerId(self): # Long
-		return self.get_query_params().get('OwnerId')
-
-	def set_OwnerId(self, OwnerId):  # Long
-		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/RebalanceDBInstanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ReleaseInstancePublicConnectionRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,28 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class RebalanceDBInstanceRequest(RpcRequest):
+class ReleaseInstancePublicConnectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'RebalanceDBInstance')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'ReleaseInstancePublicConnection')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ClientToken(self): # String
-		return self.get_query_params().get('ClientToken')
+	def get_AddressType(self): # String
+		return self.get_query_params().get('AddressType')
 
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_query_param('ClientToken', ClientToken)
+	def set_AddressType(self, AddressType):  # String
+		self.add_query_param('AddressType', AddressType)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_CurrentConnectionString(self): # String
+		return self.get_query_params().get('CurrentConnectionString')
+
+	def set_CurrentConnectionString(self, CurrentConnectionString):  # String
+		self.add_query_param('CurrentConnectionString', CurrentConnectionString)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ReleaseInstancePublicConnectionRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/SetDBInstancePlanStatusRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,33 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class ReleaseInstancePublicConnectionRequest(RpcRequest):
+class SetDBInstancePlanStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'ReleaseInstancePublicConnection')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'SetDBInstancePlanStatus')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_AddressType(self): # String
-		return self.get_query_params().get('AddressType')
+	def get_PlanStatus(self): # String
+		return self.get_query_params().get('PlanStatus')
 
-	def set_AddressType(self, AddressType):  # String
-		self.add_query_param('AddressType', AddressType)
+	def set_PlanStatus(self, PlanStatus):  # String
+		self.add_query_param('PlanStatus', PlanStatus)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_CurrentConnectionString(self): # String
-		return self.get_query_params().get('CurrentConnectionString')
+	def get_OwnerId(self): # Long
+		return self.get_query_params().get('OwnerId')
 
-	def set_CurrentConnectionString(self, CurrentConnectionString):  # String
-		self.add_query_param('CurrentConnectionString', CurrentConnectionString)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_PlanId(self): # String
+		return self.get_query_params().get('PlanId')
+
+	def set_PlanId(self, PlanId):  # String
+		self.add_query_param('PlanId', PlanId)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ResetAccountPasswordRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ListCollectionsRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,33 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class ResetAccountPasswordRequest(RpcRequest):
+class ListCollectionsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'ResetAccountPassword')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'ListCollections')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_AccountName(self): # String
-		return self.get_query_params().get('AccountName')
-
-	def set_AccountName(self, AccountName):  # String
-		self.add_query_param('AccountName', AccountName)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_AccountPassword(self): # String
-		return self.get_query_params().get('AccountPassword')
+	def get_OwnerId(self): # Long
+		return self.get_query_params().get('OwnerId')
+
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_NamespacePassword(self): # String
+		return self.get_query_params().get('NamespacePassword')
+
+	def set_NamespacePassword(self, NamespacePassword):  # String
+		self.add_query_param('NamespacePassword', NamespacePassword)
+	def get_Namespace(self): # String
+		return self.get_query_params().get('Namespace')
 
-	def set_AccountPassword(self, AccountPassword):  # String
-		self.add_query_param('AccountPassword', AccountPassword)
+	def set_Namespace(self, Namespace):  # String
+		self.add_query_param('Namespace', Namespace)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/RestartDBInstanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/InitVectorDatabaseRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,28 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class RestartDBInstanceRequest(RpcRequest):
+class InitVectorDatabaseRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'RestartDBInstance')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'InitVectorDatabase')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ClientToken(self): # String
-		return self.get_query_params().get('ClientToken')
+	def get_ManagerAccount(self): # String
+		return self.get_query_params().get('ManagerAccount')
 
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_query_param('ClientToken', ClientToken)
+	def set_ManagerAccount(self, ManagerAccount):  # String
+		self.add_query_param('ManagerAccount', ManagerAccount)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_ManagerAccountPassword(self): # String
+		return self.get_query_params().get('ManagerAccountPassword')
+
+	def set_ManagerAccountPassword(self, ManagerAccountPassword):  # String
+		self.add_query_param('ManagerAccountPassword', ManagerAccountPassword)
+	def get_OwnerId(self): # Long
+		return self.get_query_params().get('OwnerId')
+
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ResumeInstanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/ModifyVectorConfigurationRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,28 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class ResumeInstanceRequest(RpcRequest):
+class ModifyVectorConfigurationRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'ResumeInstance')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'ModifyVectorConfiguration')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_VectorConfigurationStatus(self): # String
+		return self.get_query_params().get('VectorConfigurationStatus')
+
+	def set_VectorConfigurationStatus(self, VectorConfigurationStatus):  # String
+		self.add_query_param('VectorConfigurationStatus', VectorConfigurationStatus)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/SetDBInstancePlanStatusRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DeleteVectorIndexRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,38 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class SetDBInstancePlanStatusRequest(RpcRequest):
+class DeleteVectorIndexRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'SetDBInstancePlanStatus')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DeleteVectorIndex')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_PlanStatus(self): # String
-		return self.get_query_params().get('PlanStatus')
+	def get_ManagerAccount(self): # String
+		return self.get_query_params().get('ManagerAccount')
 
-	def set_PlanStatus(self, PlanStatus):  # String
-		self.add_query_param('PlanStatus', PlanStatus)
+	def set_ManagerAccount(self, ManagerAccount):  # String
+		self.add_query_param('ManagerAccount', ManagerAccount)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_ManagerAccountPassword(self): # String
+		return self.get_query_params().get('ManagerAccountPassword')
+
+	def set_ManagerAccountPassword(self, ManagerAccountPassword):  # String
+		self.add_query_param('ManagerAccountPassword', ManagerAccountPassword)
+	def get_Collection(self): # String
+		return self.get_query_params().get('Collection')
+
+	def set_Collection(self, Collection):  # String
+		self.add_query_param('Collection', Collection)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_PlanId(self): # String
-		return self.get_query_params().get('PlanId')
+	def get_Namespace(self): # String
+		return self.get_query_params().get('Namespace')
 
-	def set_PlanId(self, PlanId):  # String
-		self.add_query_param('PlanId', PlanId)
+	def set_Namespace(self, Namespace):  # String
+		self.add_query_param('Namespace', Namespace)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/SetDataShareInstanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/SetDataShareInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/SwitchDBInstanceNetTypeRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DescribeCollectionRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,33 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class SwitchDBInstanceNetTypeRequest(RpcRequest):
+class DescribeCollectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'SwitchDBInstanceNetType')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DescribeCollection')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ConnectionStringPrefix(self): # String
-		return self.get_query_params().get('ConnectionStringPrefix')
-
-	def set_ConnectionStringPrefix(self, ConnectionStringPrefix):  # String
-		self.add_query_param('ConnectionStringPrefix', ConnectionStringPrefix)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_Port(self): # String
-		return self.get_query_params().get('Port')
+	def get_Collection(self): # String
+		return self.get_query_params().get('Collection')
+
+	def set_Collection(self, Collection):  # String
+		self.add_query_param('Collection', Collection)
+	def get_OwnerId(self): # Long
+		return self.get_query_params().get('OwnerId')
+
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_NamespacePassword(self): # String
+		return self.get_query_params().get('NamespacePassword')
+
+	def set_NamespacePassword(self, NamespacePassword):  # String
+		self.add_query_param('NamespacePassword', NamespacePassword)
+	def get_Namespace(self): # String
+		return self.get_query_params().get('Namespace')
 
-	def set_Port(self, Port):  # String
-		self.add_query_param('Port', Port)
+	def set_Namespace(self, Namespace):  # String
+		self.add_query_param('Namespace', Namespace)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/TagResourcesRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/TagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/UnloadSampleDataRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/DeleteNamespaceRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,28 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class UnloadSampleDataRequest(RpcRequest):
+class DeleteNamespaceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'UnloadSampleData')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'DeleteNamespace')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ManagerAccount(self): # String
+		return self.get_query_params().get('ManagerAccount')
+
+	def set_ManagerAccount(self, ManagerAccount):  # String
+		self.add_query_param('ManagerAccount', ManagerAccount)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_ManagerAccountPassword(self): # String
+		return self.get_query_params().get('ManagerAccountPassword')
+
+	def set_ManagerAccountPassword(self, ManagerAccountPassword):  # String
+		self.add_query_param('ManagerAccountPassword', ManagerAccountPassword)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
+	def get_Namespace(self): # String
+		return self.get_query_params().get('Namespace')
+
+	def set_Namespace(self, Namespace):  # String
+		self.add_query_param('Namespace', Namespace)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/UntagResourcesRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/UntagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/UpdateDBInstancePlanRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/UpsertCollectionDataRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,59 +15,50 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
+import json
 
-class UpdateDBInstancePlanRequest(RpcRequest):
+class UpsertCollectionDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'UpdateDBInstancePlan')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'UpsertCollectionData')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_PlanStartDate(self): # String
-		return self.get_query_params().get('PlanStartDate')
-
-	def set_PlanStartDate(self, PlanStartDate):  # String
-		self.add_query_param('PlanStartDate', PlanStartDate)
-	def get_PlanConfig(self): # String
-		return self.get_query_params().get('PlanConfig')
-
-	def set_PlanConfig(self, PlanConfig):  # String
-		self.add_query_param('PlanConfig', PlanConfig)
-	def get_PlanName(self): # String
-		return self.get_query_params().get('PlanName')
-
-	def set_PlanName(self, PlanName):  # String
-		self.add_query_param('PlanName', PlanName)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_PlanDesc(self): # String
-		return self.get_query_params().get('PlanDesc')
+	def get_Collection(self): # String
+		return self.get_query_params().get('Collection')
 
-	def set_PlanDesc(self, PlanDesc):  # String
-		self.add_query_param('PlanDesc', PlanDesc)
+	def set_Collection(self, Collection):  # String
+		self.add_query_param('Collection', Collection)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_PlanEndDate(self): # String
-		return self.get_query_params().get('PlanEndDate')
+	def get_Rows(self): # Array
+		return self.get_query_params().get('Rows')
 
-	def set_PlanEndDate(self, PlanEndDate):  # String
-		self.add_query_param('PlanEndDate', PlanEndDate)
-	def get_PlanId(self): # String
-		return self.get_query_params().get('PlanId')
+	def set_Rows(self, Rows):  # Array
+		self.add_query_param("Rows", json.dumps(Rows))
+	def get_NamespacePassword(self): # String
+		return self.get_query_params().get('NamespacePassword')
+
+	def set_NamespacePassword(self, NamespacePassword):  # String
+		self.add_query_param('NamespacePassword', NamespacePassword)
+	def get_Namespace(self): # String
+		return self.get_query_params().get('Namespace')
 
-	def set_PlanId(self, PlanId):  # String
-		self.add_query_param('PlanId', PlanId)
+	def set_Namespace(self, Namespace):  # String
+		self.add_query_param('Namespace', Namespace)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/UpgradeDBVersionRequest.py` & `aliyun-python-sdk-gpdb-1.1.7/aliyunsdkgpdb/request/v20160503/UpgradeDBVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.6/setup.py` & `aliyun-python-sdk-gpdb-1.1.7/setup.py`

 * *Files identical despite different names*

