# Comparing `tmp/cdklabs.cdk-aws-sagemaker-role-manager-0.0.8.tar.gz` & `tmp/cdklabs.cdk-aws-sagemaker-role-manager-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.cdk-aws-sagemaker-role-manager-0.0.8.tar", last modified: Wed Jun 14 19:26:38 2023, max compression
+gzip compressed data, was "cdklabs.cdk-aws-sagemaker-role-manager-0.0.9.tar", last modified: Wed Jun 14 22:03:08 2023, max compression
```

## Comparing `cdklabs.cdk-aws-sagemaker-role-manager-0.0.8.tar` & `cdklabs.cdk-aws-sagemaker-role-manager-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:26:38.373669 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-14 19:26:23.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 19:26:23.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-14 19:26:23.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-06-14 19:26:38.373669 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-06-14 19:26:23.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-14 19:26:23.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 19:26:38.373669 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-14 19:26:23.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:26:38.373669 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:26:38.373669 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:26:38.373669 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs/cdk_aws_sagemaker_role_manager/
--rw-r--r--   0 runner    (1001) docker     (123)   157030 2023-06-14 19:26:23.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs/cdk_aws_sagemaker_role_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:26:38.373669 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs/cdk_aws_sagemaker_role_manager/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-14 19:26:23.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs/cdk_aws_sagemaker_role_manager/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57129 2023-06-14 19:26:23.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs/cdk_aws_sagemaker_role_manager/_jsii/cdk-aws-sagemaker-role-manager@0.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:26:23.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs/cdk_aws_sagemaker_role_manager/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:26:38.373669 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-06-14 19:26:38.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-14 19:26:38.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:26:38.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-14 19:26:38.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 19:26:38.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:03:08.527695 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-14 22:02:55.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 22:02:55.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-14 22:02:55.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     9523 2023-06-14 22:03:08.527695 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-06-14 22:02:55.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-14 22:02:55.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 22:03:08.527695 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-14 22:02:55.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:03:08.523695 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:03:08.523695 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/src/cdklabs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:03:08.527695 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/src/cdklabs/cdk_aws_sagemaker_role_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)   155914 2023-06-14 22:02:55.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/src/cdklabs/cdk_aws_sagemaker_role_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:03:08.527695 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/src/cdklabs/cdk_aws_sagemaker_role_manager/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-14 22:02:55.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/src/cdklabs/cdk_aws_sagemaker_role_manager/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56625 2023-06-14 22:02:55.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/src/cdklabs/cdk_aws_sagemaker_role_manager/_jsii/cdk-aws-sagemaker-role-manager@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 22:02:55.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/src/cdklabs/cdk_aws_sagemaker_role_manager/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:03:08.527695 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9523 2023-06-14 22:03:08.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-14 22:03:08.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 22:03:08.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-14 22:03:08.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 22:03:08.000000 cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/top_level.txt
```

### Comparing `cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/LICENSE` & `cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/PKG-INFO` & `cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-aws-sagemaker-role-manager
-Version: 0.0.8
+Version: 0.0.9
 Summary: Create roles and policies for ML Activities and ML Personas
 Home-page: https://github.com/cdklabs/cdk-aws-sagemaker-role-manager
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-aws-sagemaker-role-manager
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -26,169 +26,142 @@
 ## cdk-aws-sagemaker-role-manager
 
 ## Usage
 
 ### Create Role from ML Activity with VPC and KMS conditions
 
 ```python
-import { App, Stack } from 'aws-cdk-lib';
-import { Activity } from 'cdk-aws-sagemaker-role-manager';
+import { Stack } from 'aws-cdk-lib';
+import { Activity } from '@cdklabs/cdk-aws-sagemaker-role-manager';
 
-const app = new App();
-new Stack(app, 'CdkRoleManagerDemo');
+const stack = new Stack(app, 'CdkRoleManagerDemo');
 
-// Simple ML Activity Role Creation
-const activity = Activity.manageJobs(this, 'id1', {
-    rolesToPass: [new iam.Role('Enter Role Parameters')],
+const activity = Activity.manageJobs(stack, 'id1', {
+    rolesToPass: [iam.Role.fromRoleName('Enter Name')],
     subnets: [ec2.Subnet.fromSubnetId('Enter Id')],
     securityGroups: [ec2.SecurityGroup.fromSecurityGroupId('Enter Id')],
     dataKeys: [kms.Key.fromKeyArn('Enter Key Arn')],
     volumeKeys: [kms.Key.fromKeyArn('Enter Key Arn')],
 });
-const role = activity.createRole(this, 'role id', 'Enter Name', 'Enter Description');
+
+activity.createRole(stack, 'role id', 'Enter Name');
 ```
 
 ### Create Role from ML Activity without VPC and KMS conditions
 
 ```python
-import { App, Stack } from 'aws-cdk-lib';
-import { Activity } from 'cdk-aws-sagemaker-role-manager';
+import { Stack } from 'aws-cdk-lib';
+import { Activity } from '@cdklabs/cdk-aws-sagemaker-role-manager';
 
-const app = new App();
-new Stack(app, 'CdkRoleManagerDemo');
+const stack = new Stack(app, 'CdkRoleManagerDemo');
 
-// Simple ML Activity Role Creation
 const activity = Activity.manageJobs(this, 'id1', {
-    rolesToPass: [new iam.Role('Enter Role Parameters')],
+    rolesToPass: [iam.Role.fromRoleName('Enter Name')],
 });
 
-const role = activity.createRole(this, 'role id', 'Enter Name', 'Enter Description');
+activity.createRole(this, 'role id', 'Enter Name', 'Enter Description');
 ```
 
 ### Create Role from Data Scientist ML Persona
 
 ```python
-import { App, Stack } from 'aws-cdk-lib';
-import { Activity } from 'cdk-aws-sagemaker-role-manager';
+import { Stack } from 'aws-cdk-lib';
+import { Activity, Persona } from '@cdklabs/cdk-aws-sagemaker-role-manager';
 
-const app = new App();
-new Stack(app, 'CdkRoleManagerDemo');
+const stack = new Stack(app, 'CdkRoleManagerDemo');
 
-// Please see below how to create the Data Scientist ML Persona using its ML Activities.
-// You can update the following list with changes matching your usecase.
 let persona = new Persona(this, 'persona id', {
     activities: [
         Activity.useStudioApps(),
-        Activity.manageJobs(this, 'id1', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
-        Activity.manageModels(this, 'id2', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
+        Activity.manageJobs(this, 'id1', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
+        Activity.manageModels(this, 'id2', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
         Activity.manageExperiments(this, 'id3', {}),
         Activity.searchExperiments(this, 'id4', {}),
         Activity.accessBuckets(this, 'id5', {buckets: [s3.S3Bucket.fromBucketName('Enter Name')]})
     ],
     subnets: [ec2.Subnet.fromSubnetId('Enter Id')],
     securityGroups: [ec2.SecurityGroup.fromSecurityGroupId('Enter Id')],
     dataKeys: [kms.Key.fromKeyArn('Enter Key Arn')],
     volumeKeys: [kms.Key.fromKeyArn('Enter Key Arn')],
 });
 
-// We can create a role with Data Scientist persona permissions
-const role = persona.createRole(this, 'role id', 'Enter Name', 'Enter Description');
+persona.createRole(this, 'role id', 'Enter Name', 'Enter Description');
 ```
 
 ### Create Role from Data Scientist ML Persona without vpc and kms global conditions
 
 ```python
-import { App, Stack } from 'aws-cdk-lib';
-import { Activity } from 'cdk-aws-sagemaker-role-manager';
+import { Stack } from 'aws-cdk-lib';
+import { Activity, Persona } from '@cdklabs/cdk-aws-sagemaker-role-manager';
 
-const app = new App();
-new Stack(app, 'CdkRoleManagerDemo');
+const stack = new Stack(app, 'CdkRoleManagerDemo');
 
 // Please see below how to create the Data Scientist ML Persona using its ML Activities.
 // You can update the following list with changes matching your usecase.
 let persona = new Persona(this, 'persona id', {
     activities: [
         Activity.useStudioApps(),
-        Activity.manageJobs(this, 'id1', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
-        Activity.manageModels(this, 'id2', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
+        Activity.manageJobs(this, 'id1', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
+        Activity.manageModels(this, 'id2', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
         Activity.manageExperiments(this, 'id3', {}),
         Activity.searchExperiments(this, 'id4', {}),
         Activity.accessBuckets(this, 'id5', {buckets: [s3.S3Bucket.fromBucketName('Enter Name')]})
     ],
 });
 
 // We can create a role with Data Scientist persona permissions
 const role = persona.createRole(this, 'role id', 'Enter Name', 'Enter Description');
 ```
 
 ### Create Role MLOps ML Persona
 
 ```python
-import { App, Stack } from 'aws-cdk-lib';
-import { Activity } from 'cdk-aws-sagemaker-role-manager';
+import { Stack } from 'aws-cdk-lib';
+import { Activity, Persona } from '@cdklabs/cdk-aws-sagemaker-role-manager';
 
-const app = new App();
-new Stack(app, 'CdkRoleManagerDemo');
+const stack = new Stack(app, 'CdkRoleManagerDemo');
 
-// Please see below MLOps ML Activities.
-// You can update the following list with changes matching your usecase.
 let persona = new Persona(this, 'persona id', {
     activities: [
         Activity.useStudioApps(this, 'id1', {}),
-        Activity.manageModels(this, 'id2', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
-        Activity.manageEndpoints(this, 'id3',{rolesToPass: [new iam.Role('Enter Role Parameters')]}),
-        Activity.managePipelines(this, 'id4', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
+        Activity.manageModels(this, 'id2', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
+        Activity.manageEndpoints(this, 'id3',{rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
+        Activity.managePipelines(this, 'id4', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
         Activity.searchExperiments(this, 'id5', {})
     ],
     subnets: [ec2.Subnet.fromSubnetId('Enter Id')],
     securityGroups: [ec2.SecurityGroup.fromSecurityGroupId('Enter Id')],
     dataKeys: [kms.Key.fromKeyArn('Enter Key Arn')],
     volumeKeys: [kms.Key.fromKeyArn('Enter Key Arn')],
 });
 
-// We can create a role with Data Scientist persona permissions
 const role = persona.createRole(this, 'role id', 'Enter Name', 'Enter Description');
 ```
 
 ### Create Role from MLOps ML Persona without vpc and kms global conditions
 
 ```python
-import { App, Stack } from 'aws-cdk-lib';
-import { Activity } from 'cdk-aws-sagemaker-role-manager';
+import { Stack } from 'aws-cdk-lib';
+import { Activity, Persona } from '@cdklabs/cdk-aws-sagemaker-role-manager';
 
-const app = new App();
-new Stack(app, 'CdkRoleManagerDemo');
+const stack = new Stack(app, 'CdkRoleManagerDemo');
 
-// Please see below MLOps ML Activities.
-// You can update the following list with changes matching your usecase.
 let persona = new Persona(this, 'persona id', {
     activities: [
         Activity.useStudioApps(this, 'id1', {}),
-        Activity.manageModels(this, 'id2', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
-        Activity.manageEndpoints(this, 'id3',{rolesToPass: [new iam.Role('Enter Role Parameters')]}),
-        Activity.managePipelines(this, 'id4', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
+        Activity.manageModels(this, 'id2', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
+        Activity.manageEndpoints(this, 'id3',{rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
+        Activity.managePipelines(this, 'id4', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
         Activity.searchExperiments(this, 'id5', {})
     ],
 });
 
-// We can create a role with Data Scientist persona permissions
 const role = persona.createRole(this, 'role id', 'Enter Name', 'Enter Description');
 ```
 
-### Use created role to initialize notebook instance and/or user profile
-
-```python
-// Variable role has already been created through cdk
-// ...
-
-// Create a notebook instance and/or user profile with role
-let notebookInstance = new CfnNotebookInstance(this, 'nb', { RoleArn: role.RoleArn, ...});
-let userProfile = new CfnNUserProfile(this, 'up', { RoleName: role.RoleName, ... });
-```
-
 ## Available ML Activities
 
 | ML Activity Name | ML Activity Interface           | ML Activity Description                                                                                   | ML Activity Required Parameters |
 |------------------|---------------------------------|-----------------------------------------------------------------------------------------------------------|---------------------------------|
 | Access Required AWS Services          | Activity.accessAwsServices()    | Permissions to access S3, ECR, Cloudwatch and EC2. Required for execution roles for jobs and endpoints.   | ecrRepositories, s3Buckets      |
 | Run Studio Applications         | Activity.runStudioApps()        | Permissions to operate within a Studio environment. Required for domain and user-profile execution roles. | rolesToPass                     |
 | Manage ML Jobs          | Activity.manageJobs()           | Permissions to manage SageMaker jobs across their lifecycles.                                             | rolesToPass                     |
```

### Comparing `cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/README.md` & `cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,169 +1,167 @@
+Metadata-Version: 2.1
+Name: cdklabs.cdk-aws-sagemaker-role-manager
+Version: 0.0.9
+Summary: Create roles and policies for ML Activities and ML Personas
+Home-page: https://github.com/cdklabs/cdk-aws-sagemaker-role-manager
+Author: Amazon Web Services<aws-cdk-dev@amazon.com>
+License: Apache-2.0
+Project-URL: Source, https://github.com/cdklabs/cdk-aws-sagemaker-role-manager
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: JavaScript
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved
+Requires-Python: ~=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: NOTICE
+
 ## cdk-aws-sagemaker-role-manager
 
 ## Usage
 
 ### Create Role from ML Activity with VPC and KMS conditions
 
 ```python
-import { App, Stack } from 'aws-cdk-lib';
-import { Activity } from 'cdk-aws-sagemaker-role-manager';
+import { Stack } from 'aws-cdk-lib';
+import { Activity } from '@cdklabs/cdk-aws-sagemaker-role-manager';
 
-const app = new App();
-new Stack(app, 'CdkRoleManagerDemo');
+const stack = new Stack(app, 'CdkRoleManagerDemo');
 
-// Simple ML Activity Role Creation
-const activity = Activity.manageJobs(this, 'id1', {
-    rolesToPass: [new iam.Role('Enter Role Parameters')],
+const activity = Activity.manageJobs(stack, 'id1', {
+    rolesToPass: [iam.Role.fromRoleName('Enter Name')],
     subnets: [ec2.Subnet.fromSubnetId('Enter Id')],
     securityGroups: [ec2.SecurityGroup.fromSecurityGroupId('Enter Id')],
     dataKeys: [kms.Key.fromKeyArn('Enter Key Arn')],
     volumeKeys: [kms.Key.fromKeyArn('Enter Key Arn')],
 });
-const role = activity.createRole(this, 'role id', 'Enter Name', 'Enter Description');
+
+activity.createRole(stack, 'role id', 'Enter Name');
 ```
 
 ### Create Role from ML Activity without VPC and KMS conditions
 
 ```python
-import { App, Stack } from 'aws-cdk-lib';
-import { Activity } from 'cdk-aws-sagemaker-role-manager';
+import { Stack } from 'aws-cdk-lib';
+import { Activity } from '@cdklabs/cdk-aws-sagemaker-role-manager';
 
-const app = new App();
-new Stack(app, 'CdkRoleManagerDemo');
+const stack = new Stack(app, 'CdkRoleManagerDemo');
 
-// Simple ML Activity Role Creation
 const activity = Activity.manageJobs(this, 'id1', {
-    rolesToPass: [new iam.Role('Enter Role Parameters')],
+    rolesToPass: [iam.Role.fromRoleName('Enter Name')],
 });
 
-const role = activity.createRole(this, 'role id', 'Enter Name', 'Enter Description');
+activity.createRole(this, 'role id', 'Enter Name', 'Enter Description');
 ```
 
 ### Create Role from Data Scientist ML Persona
 
 ```python
-import { App, Stack } from 'aws-cdk-lib';
-import { Activity } from 'cdk-aws-sagemaker-role-manager';
+import { Stack } from 'aws-cdk-lib';
+import { Activity, Persona } from '@cdklabs/cdk-aws-sagemaker-role-manager';
 
-const app = new App();
-new Stack(app, 'CdkRoleManagerDemo');
+const stack = new Stack(app, 'CdkRoleManagerDemo');
 
-// Please see below how to create the Data Scientist ML Persona using its ML Activities.
-// You can update the following list with changes matching your usecase.
 let persona = new Persona(this, 'persona id', {
     activities: [
         Activity.useStudioApps(),
-        Activity.manageJobs(this, 'id1', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
-        Activity.manageModels(this, 'id2', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
+        Activity.manageJobs(this, 'id1', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
+        Activity.manageModels(this, 'id2', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
         Activity.manageExperiments(this, 'id3', {}),
         Activity.searchExperiments(this, 'id4', {}),
         Activity.accessBuckets(this, 'id5', {buckets: [s3.S3Bucket.fromBucketName('Enter Name')]})
     ],
     subnets: [ec2.Subnet.fromSubnetId('Enter Id')],
     securityGroups: [ec2.SecurityGroup.fromSecurityGroupId('Enter Id')],
     dataKeys: [kms.Key.fromKeyArn('Enter Key Arn')],
     volumeKeys: [kms.Key.fromKeyArn('Enter Key Arn')],
 });
 
-// We can create a role with Data Scientist persona permissions
-const role = persona.createRole(this, 'role id', 'Enter Name', 'Enter Description');
+persona.createRole(this, 'role id', 'Enter Name', 'Enter Description');
 ```
 
 ### Create Role from Data Scientist ML Persona without vpc and kms global conditions
 
 ```python
-import { App, Stack } from 'aws-cdk-lib';
-import { Activity } from 'cdk-aws-sagemaker-role-manager';
+import { Stack } from 'aws-cdk-lib';
+import { Activity, Persona } from '@cdklabs/cdk-aws-sagemaker-role-manager';
 
-const app = new App();
-new Stack(app, 'CdkRoleManagerDemo');
+const stack = new Stack(app, 'CdkRoleManagerDemo');
 
 // Please see below how to create the Data Scientist ML Persona using its ML Activities.
 // You can update the following list with changes matching your usecase.
 let persona = new Persona(this, 'persona id', {
     activities: [
         Activity.useStudioApps(),
-        Activity.manageJobs(this, 'id1', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
-        Activity.manageModels(this, 'id2', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
+        Activity.manageJobs(this, 'id1', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
+        Activity.manageModels(this, 'id2', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
         Activity.manageExperiments(this, 'id3', {}),
         Activity.searchExperiments(this, 'id4', {}),
         Activity.accessBuckets(this, 'id5', {buckets: [s3.S3Bucket.fromBucketName('Enter Name')]})
     ],
 });
 
 // We can create a role with Data Scientist persona permissions
 const role = persona.createRole(this, 'role id', 'Enter Name', 'Enter Description');
 ```
 
 ### Create Role MLOps ML Persona
 
 ```python
-import { App, Stack } from 'aws-cdk-lib';
-import { Activity } from 'cdk-aws-sagemaker-role-manager';
+import { Stack } from 'aws-cdk-lib';
+import { Activity, Persona } from '@cdklabs/cdk-aws-sagemaker-role-manager';
 
-const app = new App();
-new Stack(app, 'CdkRoleManagerDemo');
+const stack = new Stack(app, 'CdkRoleManagerDemo');
 
-// Please see below MLOps ML Activities.
-// You can update the following list with changes matching your usecase.
 let persona = new Persona(this, 'persona id', {
     activities: [
         Activity.useStudioApps(this, 'id1', {}),
-        Activity.manageModels(this, 'id2', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
-        Activity.manageEndpoints(this, 'id3',{rolesToPass: [new iam.Role('Enter Role Parameters')]}),
-        Activity.managePipelines(this, 'id4', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
+        Activity.manageModels(this, 'id2', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
+        Activity.manageEndpoints(this, 'id3',{rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
+        Activity.managePipelines(this, 'id4', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
         Activity.searchExperiments(this, 'id5', {})
     ],
     subnets: [ec2.Subnet.fromSubnetId('Enter Id')],
     securityGroups: [ec2.SecurityGroup.fromSecurityGroupId('Enter Id')],
     dataKeys: [kms.Key.fromKeyArn('Enter Key Arn')],
     volumeKeys: [kms.Key.fromKeyArn('Enter Key Arn')],
 });
 
-// We can create a role with Data Scientist persona permissions
 const role = persona.createRole(this, 'role id', 'Enter Name', 'Enter Description');
 ```
 
 ### Create Role from MLOps ML Persona without vpc and kms global conditions
 
 ```python
-import { App, Stack } from 'aws-cdk-lib';
-import { Activity } from 'cdk-aws-sagemaker-role-manager';
+import { Stack } from 'aws-cdk-lib';
+import { Activity, Persona } from '@cdklabs/cdk-aws-sagemaker-role-manager';
 
-const app = new App();
-new Stack(app, 'CdkRoleManagerDemo');
+const stack = new Stack(app, 'CdkRoleManagerDemo');
 
-// Please see below MLOps ML Activities.
-// You can update the following list with changes matching your usecase.
 let persona = new Persona(this, 'persona id', {
     activities: [
         Activity.useStudioApps(this, 'id1', {}),
-        Activity.manageModels(this, 'id2', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
-        Activity.manageEndpoints(this, 'id3',{rolesToPass: [new iam.Role('Enter Role Parameters')]}),
-        Activity.managePipelines(this, 'id4', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
+        Activity.manageModels(this, 'id2', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
+        Activity.manageEndpoints(this, 'id3',{rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
+        Activity.managePipelines(this, 'id4', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
         Activity.searchExperiments(this, 'id5', {})
     ],
 });
 
-// We can create a role with Data Scientist persona permissions
 const role = persona.createRole(this, 'role id', 'Enter Name', 'Enter Description');
 ```
 
-### Use created role to initialize notebook instance and/or user profile
-
-```python
-// Variable role has already been created through cdk
-// ...
-
-// Create a notebook instance and/or user profile with role
-let notebookInstance = new CfnNotebookInstance(this, 'nb', { RoleArn: role.RoleArn, ...});
-let userProfile = new CfnNUserProfile(this, 'up', { RoleName: role.RoleName, ... });
-```
-
 ## Available ML Activities
 
 | ML Activity Name | ML Activity Interface           | ML Activity Description                                                                                   | ML Activity Required Parameters |
 |------------------|---------------------------------|-----------------------------------------------------------------------------------------------------------|---------------------------------|
 | Access Required AWS Services          | Activity.accessAwsServices()    | Permissions to access S3, ECR, Cloudwatch and EC2. Required for execution roles for jobs and endpoints.   | ecrRepositories, s3Buckets      |
 | Run Studio Applications         | Activity.runStudioApps()        | Permissions to operate within a Studio environment. Required for domain and user-profile execution roles. | rolesToPass                     |
 | Manage ML Jobs          | Activity.manageJobs()           | Permissions to manage SageMaker jobs across their lifecycles.                                             | rolesToPass                     |
```

### Comparing `cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/setup.py` & `cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.cdk-aws-sagemaker-role-manager",
-    "version": "0.0.8",
+    "version": "0.0.9",
     "description": "Create roles and policies for ML Activities and ML Personas",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-aws-sagemaker-role-manager",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdklabs.cdk_aws_sagemaker_role_manager",
         "cdklabs.cdk_aws_sagemaker_role_manager._jsii"
     ],
     "package_data": {
         "cdklabs.cdk_aws_sagemaker_role_manager._jsii": [
-            "cdk-aws-sagemaker-role-manager@0.0.8.jsii.tgz"
+            "cdk-aws-sagemaker-role-manager@0.0.9.jsii.tgz"
         ],
         "cdklabs.cdk_aws_sagemaker_role_manager": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs/cdk_aws_sagemaker_role_manager/__init__.py` & `cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/src/cdklabs/cdk_aws_sagemaker_role_manager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,169 +2,142 @@
 ## cdk-aws-sagemaker-role-manager
 
 ## Usage
 
 ### Create Role from ML Activity with VPC and KMS conditions
 
 ```python
-import { App, Stack } from 'aws-cdk-lib';
-import { Activity } from 'cdk-aws-sagemaker-role-manager';
+import { Stack } from 'aws-cdk-lib';
+import { Activity } from '@cdklabs/cdk-aws-sagemaker-role-manager';
 
-const app = new App();
-new Stack(app, 'CdkRoleManagerDemo');
+const stack = new Stack(app, 'CdkRoleManagerDemo');
 
-// Simple ML Activity Role Creation
-const activity = Activity.manageJobs(this, 'id1', {
-    rolesToPass: [new iam.Role('Enter Role Parameters')],
+const activity = Activity.manageJobs(stack, 'id1', {
+    rolesToPass: [iam.Role.fromRoleName('Enter Name')],
     subnets: [ec2.Subnet.fromSubnetId('Enter Id')],
     securityGroups: [ec2.SecurityGroup.fromSecurityGroupId('Enter Id')],
     dataKeys: [kms.Key.fromKeyArn('Enter Key Arn')],
     volumeKeys: [kms.Key.fromKeyArn('Enter Key Arn')],
 });
-const role = activity.createRole(this, 'role id', 'Enter Name', 'Enter Description');
+
+activity.createRole(stack, 'role id', 'Enter Name');
 ```
 
 ### Create Role from ML Activity without VPC and KMS conditions
 
 ```python
-import { App, Stack } from 'aws-cdk-lib';
-import { Activity } from 'cdk-aws-sagemaker-role-manager';
+import { Stack } from 'aws-cdk-lib';
+import { Activity } from '@cdklabs/cdk-aws-sagemaker-role-manager';
 
-const app = new App();
-new Stack(app, 'CdkRoleManagerDemo');
+const stack = new Stack(app, 'CdkRoleManagerDemo');
 
-// Simple ML Activity Role Creation
 const activity = Activity.manageJobs(this, 'id1', {
-    rolesToPass: [new iam.Role('Enter Role Parameters')],
+    rolesToPass: [iam.Role.fromRoleName('Enter Name')],
 });
 
-const role = activity.createRole(this, 'role id', 'Enter Name', 'Enter Description');
+activity.createRole(this, 'role id', 'Enter Name', 'Enter Description');
 ```
 
 ### Create Role from Data Scientist ML Persona
 
 ```python
-import { App, Stack } from 'aws-cdk-lib';
-import { Activity } from 'cdk-aws-sagemaker-role-manager';
+import { Stack } from 'aws-cdk-lib';
+import { Activity, Persona } from '@cdklabs/cdk-aws-sagemaker-role-manager';
 
-const app = new App();
-new Stack(app, 'CdkRoleManagerDemo');
+const stack = new Stack(app, 'CdkRoleManagerDemo');
 
-// Please see below how to create the Data Scientist ML Persona using its ML Activities.
-// You can update the following list with changes matching your usecase.
 let persona = new Persona(this, 'persona id', {
     activities: [
         Activity.useStudioApps(),
-        Activity.manageJobs(this, 'id1', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
-        Activity.manageModels(this, 'id2', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
+        Activity.manageJobs(this, 'id1', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
+        Activity.manageModels(this, 'id2', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
         Activity.manageExperiments(this, 'id3', {}),
         Activity.searchExperiments(this, 'id4', {}),
         Activity.accessBuckets(this, 'id5', {buckets: [s3.S3Bucket.fromBucketName('Enter Name')]})
     ],
     subnets: [ec2.Subnet.fromSubnetId('Enter Id')],
     securityGroups: [ec2.SecurityGroup.fromSecurityGroupId('Enter Id')],
     dataKeys: [kms.Key.fromKeyArn('Enter Key Arn')],
     volumeKeys: [kms.Key.fromKeyArn('Enter Key Arn')],
 });
 
-// We can create a role with Data Scientist persona permissions
-const role = persona.createRole(this, 'role id', 'Enter Name', 'Enter Description');
+persona.createRole(this, 'role id', 'Enter Name', 'Enter Description');
 ```
 
 ### Create Role from Data Scientist ML Persona without vpc and kms global conditions
 
 ```python
-import { App, Stack } from 'aws-cdk-lib';
-import { Activity } from 'cdk-aws-sagemaker-role-manager';
+import { Stack } from 'aws-cdk-lib';
+import { Activity, Persona } from '@cdklabs/cdk-aws-sagemaker-role-manager';
 
-const app = new App();
-new Stack(app, 'CdkRoleManagerDemo');
+const stack = new Stack(app, 'CdkRoleManagerDemo');
 
 // Please see below how to create the Data Scientist ML Persona using its ML Activities.
 // You can update the following list with changes matching your usecase.
 let persona = new Persona(this, 'persona id', {
     activities: [
         Activity.useStudioApps(),
-        Activity.manageJobs(this, 'id1', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
-        Activity.manageModels(this, 'id2', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
+        Activity.manageJobs(this, 'id1', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
+        Activity.manageModels(this, 'id2', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
         Activity.manageExperiments(this, 'id3', {}),
         Activity.searchExperiments(this, 'id4', {}),
         Activity.accessBuckets(this, 'id5', {buckets: [s3.S3Bucket.fromBucketName('Enter Name')]})
     ],
 });
 
 // We can create a role with Data Scientist persona permissions
 const role = persona.createRole(this, 'role id', 'Enter Name', 'Enter Description');
 ```
 
 ### Create Role MLOps ML Persona
 
 ```python
-import { App, Stack } from 'aws-cdk-lib';
-import { Activity } from 'cdk-aws-sagemaker-role-manager';
+import { Stack } from 'aws-cdk-lib';
+import { Activity, Persona } from '@cdklabs/cdk-aws-sagemaker-role-manager';
 
-const app = new App();
-new Stack(app, 'CdkRoleManagerDemo');
+const stack = new Stack(app, 'CdkRoleManagerDemo');
 
-// Please see below MLOps ML Activities.
-// You can update the following list with changes matching your usecase.
 let persona = new Persona(this, 'persona id', {
     activities: [
         Activity.useStudioApps(this, 'id1', {}),
-        Activity.manageModels(this, 'id2', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
-        Activity.manageEndpoints(this, 'id3',{rolesToPass: [new iam.Role('Enter Role Parameters')]}),
-        Activity.managePipelines(this, 'id4', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
+        Activity.manageModels(this, 'id2', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
+        Activity.manageEndpoints(this, 'id3',{rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
+        Activity.managePipelines(this, 'id4', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
         Activity.searchExperiments(this, 'id5', {})
     ],
     subnets: [ec2.Subnet.fromSubnetId('Enter Id')],
     securityGroups: [ec2.SecurityGroup.fromSecurityGroupId('Enter Id')],
     dataKeys: [kms.Key.fromKeyArn('Enter Key Arn')],
     volumeKeys: [kms.Key.fromKeyArn('Enter Key Arn')],
 });
 
-// We can create a role with Data Scientist persona permissions
 const role = persona.createRole(this, 'role id', 'Enter Name', 'Enter Description');
 ```
 
 ### Create Role from MLOps ML Persona without vpc and kms global conditions
 
 ```python
-import { App, Stack } from 'aws-cdk-lib';
-import { Activity } from 'cdk-aws-sagemaker-role-manager';
+import { Stack } from 'aws-cdk-lib';
+import { Activity, Persona } from '@cdklabs/cdk-aws-sagemaker-role-manager';
 
-const app = new App();
-new Stack(app, 'CdkRoleManagerDemo');
+const stack = new Stack(app, 'CdkRoleManagerDemo');
 
-// Please see below MLOps ML Activities.
-// You can update the following list with changes matching your usecase.
 let persona = new Persona(this, 'persona id', {
     activities: [
         Activity.useStudioApps(this, 'id1', {}),
-        Activity.manageModels(this, 'id2', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
-        Activity.manageEndpoints(this, 'id3',{rolesToPass: [new iam.Role('Enter Role Parameters')]}),
-        Activity.managePipelines(this, 'id4', {rolesToPass: [new iam.Role('Enter Role Parameters')]}),
+        Activity.manageModels(this, 'id2', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
+        Activity.manageEndpoints(this, 'id3',{rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
+        Activity.managePipelines(this, 'id4', {rolesToPass: [iam.Role.fromRoleName('Enter Name')]}),
         Activity.searchExperiments(this, 'id5', {})
     ],
 });
 
-// We can create a role with Data Scientist persona permissions
 const role = persona.createRole(this, 'role id', 'Enter Name', 'Enter Description');
 ```
 
-### Use created role to initialize notebook instance and/or user profile
-
-```python
-// Variable role has already been created through cdk
-// ...
-
-// Create a notebook instance and/or user profile with role
-let notebookInstance = new CfnNotebookInstance(this, 'nb', { RoleArn: role.RoleArn, ...});
-let userProfile = new CfnNUserProfile(this, 'up', { RoleName: role.RoleName, ... });
-```
-
 ## Available ML Activities
 
 | ML Activity Name | ML Activity Interface           | ML Activity Description                                                                                   | ML Activity Required Parameters |
 |------------------|---------------------------------|-----------------------------------------------------------------------------------------------------------|---------------------------------|
 | Access Required AWS Services          | Activity.accessAwsServices()    | Permissions to access S3, ECR, Cloudwatch and EC2. Required for execution roles for jobs and endpoints.   | ecrRepositories, s3Buckets      |
 | Run Studio Applications         | Activity.runStudioApps()        | Permissions to operate within a Studio environment. Required for domain and user-profile execution roles. | rolesToPass                     |
 | Manage ML Jobs          | Activity.manageJobs()           | Permissions to manage SageMaker jobs across their lifecycles.                                             | rolesToPass                     |
```

### Comparing `cdklabs.cdk-aws-sagemaker-role-manager-0.0.8/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/SOURCES.txt` & `cdklabs.cdk-aws-sagemaker-role-manager-0.0.9/src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/SOURCES.txt
 src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/dependency_links.txt
 src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/requires.txt
 src/cdklabs.cdk_aws_sagemaker_role_manager.egg-info/top_level.txt
 src/cdklabs/cdk_aws_sagemaker_role_manager/__init__.py
 src/cdklabs/cdk_aws_sagemaker_role_manager/py.typed
 src/cdklabs/cdk_aws_sagemaker_role_manager/_jsii/__init__.py
-src/cdklabs/cdk_aws_sagemaker_role_manager/_jsii/cdk-aws-sagemaker-role-manager@0.0.8.jsii.tgz
+src/cdklabs/cdk_aws_sagemaker_role_manager/_jsii/cdk-aws-sagemaker-role-manager@0.0.9.jsii.tgz
```

