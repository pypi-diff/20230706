# Comparing `tmp/aws-cdk.cli-lib-alpha-2.86.0a0.tar.gz` & `tmp/aws-cdk.cli-lib-alpha-2.87.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src3755887465/src/packages/@aws-cdk/cli-lib-alpha/dist/python/aws-cdk.cli-lib-alpha-2.86.0a0.tar", last modified: Thu Jun 29 08:23:34 2023, max compression
+gzip compressed data, was "/codebuild/output/src94387485/src/packages/@aws-cdk/cli-lib-alpha/dist/python/aws-cdk.cli-lib-alpha-2.87.0a0.tar", last modified: Thu Jul  6 16:50:31 2023, max compression
```

## Comparing `aws-cdk.cli-lib-alpha-2.86.0a0.tar` & `aws-cdk.cli-lib-alpha-2.87.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:34.000000 aws-cdk.cli-lib-alpha-2.86.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-29 08:23:25.000000 aws-cdk.cli-lib-alpha-2.86.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-29 08:23:28.000000 aws-cdk.cli-lib-alpha-2.86.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      726 2023-06-29 08:23:27.000000 aws-cdk.cli-lib-alpha-2.86.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4179 2023-06-29 08:23:34.000000 aws-cdk.cli-lib-alpha-2.86.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3192 2023-06-29 08:23:28.000000 aws-cdk.cli-lib-alpha-2.86.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-29 08:23:28.000000 aws-cdk.cli-lib-alpha-2.86.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 08:23:34.000000 aws-cdk.cli-lib-alpha-2.86.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1766 2023-06-29 08:23:28.000000 aws-cdk.cli-lib-alpha-2.86.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:34.000000 aws-cdk.cli-lib-alpha-2.86.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:34.000000 aws-cdk.cli-lib-alpha-2.86.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:34.000000 aws-cdk.cli-lib-alpha-2.86.0a0/src/aws_cdk/cli_lib_alpha/
--rw-r--r--   0 root         (0) root         (0)   194202 2023-06-29 08:23:28.000000 aws-cdk.cli-lib-alpha-2.86.0a0/src/aws_cdk/cli_lib_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:34.000000 aws-cdk.cli-lib-alpha-2.86.0a0/src/aws_cdk/cli_lib_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      387 2023-06-29 08:23:28.000000 aws-cdk.cli-lib-alpha-2.86.0a0/src/aws_cdk/cli_lib_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)  4328913 2023-06-29 08:23:25.000000 aws-cdk.cli-lib-alpha-2.86.0a0/src/aws_cdk/cli_lib_alpha/_jsii/cli-lib-alpha@2.86.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 08:23:28.000000 aws-cdk.cli-lib-alpha-2.86.0a0/src/aws_cdk/cli_lib_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:34.000000 aws-cdk.cli-lib-alpha-2.86.0a0/src/aws_cdk.cli_lib_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4179 2023-06-29 08:23:34.000000 aws-cdk.cli-lib-alpha-2.86.0a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      491 2023-06-29 08:23:34.000000 aws-cdk.cli-lib-alpha-2.86.0a0/src/aws_cdk.cli_lib_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 08:23:34.000000 aws-cdk.cli-lib-alpha-2.86.0a0/src/aws_cdk.cli_lib_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-29 08:23:34.000000 aws-cdk.cli-lib-alpha-2.86.0a0/src/aws_cdk.cli_lib_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-29 08:23:34.000000 aws-cdk.cli-lib-alpha-2.86.0a0/src/aws_cdk.cli_lib_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:50:31.000000 aws-cdk.cli-lib-alpha-2.87.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-07-06 16:50:23.000000 aws-cdk.cli-lib-alpha-2.87.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-06 16:50:25.000000 aws-cdk.cli-lib-alpha-2.87.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      726 2023-07-06 16:50:25.000000 aws-cdk.cli-lib-alpha-2.87.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4306 2023-07-06 16:50:31.000000 aws-cdk.cli-lib-alpha-2.87.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3319 2023-07-06 16:50:25.000000 aws-cdk.cli-lib-alpha-2.87.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-07-06 16:50:25.000000 aws-cdk.cli-lib-alpha-2.87.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 16:50:31.000000 aws-cdk.cli-lib-alpha-2.87.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-07-06 16:50:25.000000 aws-cdk.cli-lib-alpha-2.87.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:50:31.000000 aws-cdk.cli-lib-alpha-2.87.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:50:31.000000 aws-cdk.cli-lib-alpha-2.87.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:50:31.000000 aws-cdk.cli-lib-alpha-2.87.0a0/src/aws_cdk/cli_lib_alpha/
+-rw-r--r--   0 root         (0) root         (0)   256641 2023-07-06 16:50:25.000000 aws-cdk.cli-lib-alpha-2.87.0a0/src/aws_cdk/cli_lib_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:50:31.000000 aws-cdk.cli-lib-alpha-2.87.0a0/src/aws_cdk/cli_lib_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      387 2023-07-06 16:50:25.000000 aws-cdk.cli-lib-alpha-2.87.0a0/src/aws_cdk/cli_lib_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  4370710 2023-07-06 16:50:23.000000 aws-cdk.cli-lib-alpha-2.87.0a0/src/aws_cdk/cli_lib_alpha/_jsii/cli-lib-alpha@2.87.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 16:50:25.000000 aws-cdk.cli-lib-alpha-2.87.0a0/src/aws_cdk/cli_lib_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:50:31.000000 aws-cdk.cli-lib-alpha-2.87.0a0/src/aws_cdk.cli_lib_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4306 2023-07-06 16:50:30.000000 aws-cdk.cli-lib-alpha-2.87.0a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      491 2023-07-06 16:50:30.000000 aws-cdk.cli-lib-alpha-2.87.0a0/src/aws_cdk.cli_lib_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 16:50:30.000000 aws-cdk.cli-lib-alpha-2.87.0a0/src/aws_cdk.cli_lib_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-06 16:50:30.000000 aws-cdk.cli-lib-alpha-2.87.0a0/src/aws_cdk.cli_lib_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 16:50:30.000000 aws-cdk.cli-lib-alpha-2.87.0a0/src/aws_cdk.cli_lib_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.cli-lib-alpha-2.86.0a0/LICENSE` & `aws-cdk.cli-lib-alpha-2.87.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.86.0a0/NOTICE` & `aws-cdk.cli-lib-alpha-2.87.0a0/NOTICE`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.86.0a0/PKG-INFO` & `aws-cdk.cli-lib-alpha-2.87.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cli-lib-alpha
-Version: 2.86.0a0
+Version: 2.87.0a0
 Summary: AWS CDK Programmatic CLI library
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -56,14 +56,15 @@
 ## Overview
 
 Provides a library to interact with the AWS CDK CLI programmatically from jsii supported languages.
 Currently the package includes implementations for:
 
 * `cdk deploy`
 * `cdk synth`
+* `cdk bootstrap`
 * `cdk destroy`
 * `cdk list`
 
 ## Setup
 
 ### AWS CDK app directory
 
@@ -116,14 +117,21 @@
 ```python
 # await this asynchronous method call using a language feature
 cli.synth(
     stacks=["MyTestStack"]
 )
 ```
 
+### bootstrap
+
+```python
+# await this asynchronous method call using a language feature
+cli.bootstrap()
+```
+
 ### deploy
 
 ```python
 # await this asynchronous method call using a language feature
 cli.deploy(
     stacks=["MyTestStack"]
 )
```

### Comparing `aws-cdk.cli-lib-alpha-2.86.0a0/README.md` & `aws-cdk.cli-lib-alpha-2.87.0a0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 ## Overview
 
 Provides a library to interact with the AWS CDK CLI programmatically from jsii supported languages.
 Currently the package includes implementations for:
 
 * `cdk deploy`
 * `cdk synth`
+* `cdk bootstrap`
 * `cdk destroy`
 * `cdk list`
 
 ## Setup
 
 ### AWS CDK app directory
 
@@ -89,14 +90,21 @@
 ```python
 # await this asynchronous method call using a language feature
 cli.synth(
     stacks=["MyTestStack"]
 )
 ```
 
+### bootstrap
+
+```python
+# await this asynchronous method call using a language feature
+cli.bootstrap()
+```
+
 ### deploy
 
 ```python
 # await this asynchronous method call using a language feature
 cli.deploy(
     stacks=["MyTestStack"]
 )
```

### Comparing `aws-cdk.cli-lib-alpha-2.86.0a0/setup.py` & `aws-cdk.cli-lib-alpha-2.87.0a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.cli-lib-alpha",
-    "version": "2.86.0.a0",
+    "version": "2.87.0.a0",
     "description": "AWS CDK Programmatic CLI library",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_cdk.cli_lib_alpha",
         "aws_cdk.cli_lib_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.cli_lib_alpha._jsii": [
-            "cli-lib-alpha@2.86.0-alpha.0.jsii.tgz"
+            "cli-lib-alpha@2.87.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.cli_lib_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws-cdk.cli-lib-alpha-2.86.0a0/src/aws_cdk/cli_lib_alpha/__init__.py` & `aws-cdk.cli-lib-alpha-2.87.0a0/src/aws_cdk/cli_lib_alpha/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 ## Overview
 
 Provides a library to interact with the AWS CDK CLI programmatically from jsii supported languages.
 Currently the package includes implementations for:
 
 * `cdk deploy`
 * `cdk synth`
+* `cdk bootstrap`
 * `cdk destroy`
 * `cdk list`
 
 ## Setup
 
 ### AWS CDK app directory
 
@@ -90,14 +91,21 @@
 ```python
 # await this asynchronous method call using a language feature
 cli.synth(
     stacks=["MyTestStack"]
 )
 ```
 
+### bootstrap
+
+```python
+# await this asynchronous method call using a language feature
+cli.bootstrap()
+```
+
 ### deploy
 
 ```python
 # await this asynchronous method call using a language feature
 cli.deploy(
     stacks=["MyTestStack"]
 )
@@ -205,14 +213,100 @@
 @jsii.interface(jsii_type="@aws-cdk/cli-lib-alpha.IAwsCdkCli")
 class IAwsCdkCli(typing_extensions.Protocol):
     '''(experimental) AWS CDK CLI operations.
 
     :stability: experimental
     '''
 
+    @jsii.member(jsii_name="bootstrap")
+    def bootstrap(
+        self,
+        *,
+        bootstrap_bucket_name: typing.Optional[builtins.str] = None,
+        bootstrap_customer_key: typing.Optional[builtins.str] = None,
+        bootstrap_kms_key_id: typing.Optional[builtins.str] = None,
+        cfn_execution_policy: typing.Optional[builtins.str] = None,
+        custom_permissions_boundary: typing.Optional[builtins.str] = None,
+        example_permissions_boundary: typing.Optional[builtins.bool] = None,
+        execute: typing.Optional[builtins.bool] = None,
+        force: typing.Optional[builtins.bool] = None,
+        public_access_block_configuration: typing.Optional[builtins.str] = None,
+        qualifier: typing.Optional[builtins.str] = None,
+        show_template: typing.Optional[builtins.bool] = None,
+        template: typing.Optional[builtins.str] = None,
+        termination_protection: typing.Optional[builtins.bool] = None,
+        toolkit_stack_name: typing.Optional[builtins.str] = None,
+        trust: typing.Optional[builtins.str] = None,
+        trust_for_lookup: typing.Optional[builtins.str] = None,
+        use_previous_parameters: typing.Optional[builtins.bool] = None,
+        asset_metadata: typing.Optional[builtins.bool] = None,
+        ca_bundle_path: typing.Optional[builtins.str] = None,
+        color: typing.Optional[builtins.bool] = None,
+        context: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        debug: typing.Optional[builtins.bool] = None,
+        ec2_creds: typing.Optional[builtins.bool] = None,
+        ignore_errors: typing.Optional[builtins.bool] = None,
+        json: typing.Optional[builtins.bool] = None,
+        lookups: typing.Optional[builtins.bool] = None,
+        notices: typing.Optional[builtins.bool] = None,
+        path_metadata: typing.Optional[builtins.bool] = None,
+        profile: typing.Optional[builtins.str] = None,
+        proxy: typing.Optional[builtins.str] = None,
+        role_arn: typing.Optional[builtins.str] = None,
+        stacks: typing.Optional[typing.Sequence[builtins.str]] = None,
+        staging: typing.Optional[builtins.bool] = None,
+        strict: typing.Optional[builtins.bool] = None,
+        trace: typing.Optional[builtins.bool] = None,
+        verbose: typing.Optional[builtins.bool] = None,
+        version_reporting: typing.Optional[builtins.bool] = None,
+    ) -> None:
+        '''(experimental) cdk bootstrap.
+
+        :param bootstrap_bucket_name: (experimental) The name of the CDK toolkit bucket; bucket will be created and must not exist Default: - auto-generated CloudFormation name
+        :param bootstrap_customer_key: (experimental) Create a Customer Master Key (CMK) for the bootstrap bucket (you will be charged but can customize permissions, modern bootstrapping only). Default: undefined
+        :param bootstrap_kms_key_id: (experimental) AWS KMS master key ID used for the SSE-KMS encryption. Default: undefined
+        :param cfn_execution_policy: (experimental) The Managed Policy ARNs that should be attached to the role performing deployments into this environment (may be repeated, modern bootstrapping only). Default: - none
+        :param custom_permissions_boundary: (experimental) Use the permissions boundary specified by name. Default: undefined
+        :param example_permissions_boundary: (experimental) Use the example permissions boundary. Default: undefined
+        :param execute: (experimental) Whether to execute ChangeSet (--no-execute will NOT execute the ChangeSet). Default: true
+        :param force: (experimental) Always bootstrap even if it would downgrade template version. Default: false
+        :param public_access_block_configuration: (experimental) Block public access configuration on CDK toolkit bucket (enabled by default). Default: undefined
+        :param qualifier: (experimental) String which must be unique for each bootstrap stack. You must configure it on your CDK app if you change this from the default. Default: undefined
+        :param show_template: (experimental) Instead of actual bootstrapping, print the current CLI's bootstrapping template to stdout for customization. Default: false
+        :param template: (experimental) Use the template from the given file instead of the built-in one (use --show-template to obtain an example).
+        :param termination_protection: (experimental) Toggle CloudFormation termination protection on the bootstrap stacks. Default: false
+        :param toolkit_stack_name: (experimental) The name of the CDK toolkit stack to create.
+        :param trust: (experimental) The AWS account IDs that should be trusted to perform deployments into this environment (may be repeated, modern bootstrapping only). Default: undefined
+        :param trust_for_lookup: (experimental) The AWS account IDs that should be trusted to look up values in this environment (may be repeated, modern bootstrapping only). Default: undefined
+        :param use_previous_parameters: (experimental) Use previous values for existing parameters (you must specify all parameters on every deployment if this is disabled). Default: true
+        :param asset_metadata: (experimental) Include "aws:asset:*" CloudFormation metadata for resources that use assets. Default: true
+        :param ca_bundle_path: (experimental) Path to CA certificate to use when validating HTTPS requests. Default: - read from AWS_CA_BUNDLE environment variable
+        :param color: (experimental) Show colors and other style from console output. Default: - ``true`` unless the environment variable ``NO_COLOR`` is set
+        :param context: (experimental) Additional context. Default: - no additional context
+        :param debug: (experimental) enable emission of additional debugging information, such as creation stack traces of tokens. Default: false
+        :param ec2_creds: (experimental) Force trying to fetch EC2 instance credentials. Default: - guess EC2 instance status
+        :param ignore_errors: (experimental) Ignores synthesis errors, which will likely produce an invalid output. Default: false
+        :param json: (experimental) Use JSON output instead of YAML when templates are printed to STDOUT. Default: false
+        :param lookups: (experimental) Perform context lookups. Synthesis fails if this is disabled and context lookups need to be performed Default: true
+        :param notices: (experimental) Show relevant notices. Default: true
+        :param path_metadata: (experimental) Include "aws:cdk:path" CloudFormation metadata for each resource. Default: true
+        :param profile: (experimental) Use the indicated AWS profile as the default environment. Default: - no profile is used
+        :param proxy: (experimental) Use the indicated proxy. Will read from HTTPS_PROXY environment if specified Default: - no proxy
+        :param role_arn: (experimental) Role to pass to CloudFormation for deployment. Default: - use the bootstrap cfn-exec role
+        :param stacks: (experimental) List of stacks to deploy. Default: - all stacks
+        :param staging: (experimental) Copy assets to the output directory. Needed for local debugging the source files with SAM CLI Default: false
+        :param strict: (experimental) Do not construct stacks with warnings. Default: false
+        :param trace: (experimental) Print trace for stack warnings. Default: false
+        :param verbose: (experimental) show debug logs. Default: false
+        :param version_reporting: (experimental) Include "AWS::CDK::Metadata" resource in synthesized templates. Default: true
+
+        :stability: experimental
+        '''
+        ...
+
     @jsii.member(jsii_name="deploy")
     def deploy(
         self,
         *,
         asset_parallelism: typing.Optional[builtins.bool] = None,
         asset_prebuild: typing.Optional[builtins.bool] = None,
         change_set_name: typing.Optional[builtins.str] = None,
@@ -468,14 +562,140 @@
     '''(experimental) AWS CDK CLI operations.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/cli-lib-alpha.IAwsCdkCli"
 
+    @jsii.member(jsii_name="bootstrap")
+    def bootstrap(
+        self,
+        *,
+        bootstrap_bucket_name: typing.Optional[builtins.str] = None,
+        bootstrap_customer_key: typing.Optional[builtins.str] = None,
+        bootstrap_kms_key_id: typing.Optional[builtins.str] = None,
+        cfn_execution_policy: typing.Optional[builtins.str] = None,
+        custom_permissions_boundary: typing.Optional[builtins.str] = None,
+        example_permissions_boundary: typing.Optional[builtins.bool] = None,
+        execute: typing.Optional[builtins.bool] = None,
+        force: typing.Optional[builtins.bool] = None,
+        public_access_block_configuration: typing.Optional[builtins.str] = None,
+        qualifier: typing.Optional[builtins.str] = None,
+        show_template: typing.Optional[builtins.bool] = None,
+        template: typing.Optional[builtins.str] = None,
+        termination_protection: typing.Optional[builtins.bool] = None,
+        toolkit_stack_name: typing.Optional[builtins.str] = None,
+        trust: typing.Optional[builtins.str] = None,
+        trust_for_lookup: typing.Optional[builtins.str] = None,
+        use_previous_parameters: typing.Optional[builtins.bool] = None,
+        asset_metadata: typing.Optional[builtins.bool] = None,
+        ca_bundle_path: typing.Optional[builtins.str] = None,
+        color: typing.Optional[builtins.bool] = None,
+        context: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        debug: typing.Optional[builtins.bool] = None,
+        ec2_creds: typing.Optional[builtins.bool] = None,
+        ignore_errors: typing.Optional[builtins.bool] = None,
+        json: typing.Optional[builtins.bool] = None,
+        lookups: typing.Optional[builtins.bool] = None,
+        notices: typing.Optional[builtins.bool] = None,
+        path_metadata: typing.Optional[builtins.bool] = None,
+        profile: typing.Optional[builtins.str] = None,
+        proxy: typing.Optional[builtins.str] = None,
+        role_arn: typing.Optional[builtins.str] = None,
+        stacks: typing.Optional[typing.Sequence[builtins.str]] = None,
+        staging: typing.Optional[builtins.bool] = None,
+        strict: typing.Optional[builtins.bool] = None,
+        trace: typing.Optional[builtins.bool] = None,
+        verbose: typing.Optional[builtins.bool] = None,
+        version_reporting: typing.Optional[builtins.bool] = None,
+    ) -> None:
+        '''(experimental) cdk bootstrap.
+
+        :param bootstrap_bucket_name: (experimental) The name of the CDK toolkit bucket; bucket will be created and must not exist Default: - auto-generated CloudFormation name
+        :param bootstrap_customer_key: (experimental) Create a Customer Master Key (CMK) for the bootstrap bucket (you will be charged but can customize permissions, modern bootstrapping only). Default: undefined
+        :param bootstrap_kms_key_id: (experimental) AWS KMS master key ID used for the SSE-KMS encryption. Default: undefined
+        :param cfn_execution_policy: (experimental) The Managed Policy ARNs that should be attached to the role performing deployments into this environment (may be repeated, modern bootstrapping only). Default: - none
+        :param custom_permissions_boundary: (experimental) Use the permissions boundary specified by name. Default: undefined
+        :param example_permissions_boundary: (experimental) Use the example permissions boundary. Default: undefined
+        :param execute: (experimental) Whether to execute ChangeSet (--no-execute will NOT execute the ChangeSet). Default: true
+        :param force: (experimental) Always bootstrap even if it would downgrade template version. Default: false
+        :param public_access_block_configuration: (experimental) Block public access configuration on CDK toolkit bucket (enabled by default). Default: undefined
+        :param qualifier: (experimental) String which must be unique for each bootstrap stack. You must configure it on your CDK app if you change this from the default. Default: undefined
+        :param show_template: (experimental) Instead of actual bootstrapping, print the current CLI's bootstrapping template to stdout for customization. Default: false
+        :param template: (experimental) Use the template from the given file instead of the built-in one (use --show-template to obtain an example).
+        :param termination_protection: (experimental) Toggle CloudFormation termination protection on the bootstrap stacks. Default: false
+        :param toolkit_stack_name: (experimental) The name of the CDK toolkit stack to create.
+        :param trust: (experimental) The AWS account IDs that should be trusted to perform deployments into this environment (may be repeated, modern bootstrapping only). Default: undefined
+        :param trust_for_lookup: (experimental) The AWS account IDs that should be trusted to look up values in this environment (may be repeated, modern bootstrapping only). Default: undefined
+        :param use_previous_parameters: (experimental) Use previous values for existing parameters (you must specify all parameters on every deployment if this is disabled). Default: true
+        :param asset_metadata: (experimental) Include "aws:asset:*" CloudFormation metadata for resources that use assets. Default: true
+        :param ca_bundle_path: (experimental) Path to CA certificate to use when validating HTTPS requests. Default: - read from AWS_CA_BUNDLE environment variable
+        :param color: (experimental) Show colors and other style from console output. Default: - ``true`` unless the environment variable ``NO_COLOR`` is set
+        :param context: (experimental) Additional context. Default: - no additional context
+        :param debug: (experimental) enable emission of additional debugging information, such as creation stack traces of tokens. Default: false
+        :param ec2_creds: (experimental) Force trying to fetch EC2 instance credentials. Default: - guess EC2 instance status
+        :param ignore_errors: (experimental) Ignores synthesis errors, which will likely produce an invalid output. Default: false
+        :param json: (experimental) Use JSON output instead of YAML when templates are printed to STDOUT. Default: false
+        :param lookups: (experimental) Perform context lookups. Synthesis fails if this is disabled and context lookups need to be performed Default: true
+        :param notices: (experimental) Show relevant notices. Default: true
+        :param path_metadata: (experimental) Include "aws:cdk:path" CloudFormation metadata for each resource. Default: true
+        :param profile: (experimental) Use the indicated AWS profile as the default environment. Default: - no profile is used
+        :param proxy: (experimental) Use the indicated proxy. Will read from HTTPS_PROXY environment if specified Default: - no proxy
+        :param role_arn: (experimental) Role to pass to CloudFormation for deployment. Default: - use the bootstrap cfn-exec role
+        :param stacks: (experimental) List of stacks to deploy. Default: - all stacks
+        :param staging: (experimental) Copy assets to the output directory. Needed for local debugging the source files with SAM CLI Default: false
+        :param strict: (experimental) Do not construct stacks with warnings. Default: false
+        :param trace: (experimental) Print trace for stack warnings. Default: false
+        :param verbose: (experimental) show debug logs. Default: false
+        :param version_reporting: (experimental) Include "AWS::CDK::Metadata" resource in synthesized templates. Default: true
+
+        :stability: experimental
+        '''
+        options = BootstrapOptions(
+            bootstrap_bucket_name=bootstrap_bucket_name,
+            bootstrap_customer_key=bootstrap_customer_key,
+            bootstrap_kms_key_id=bootstrap_kms_key_id,
+            cfn_execution_policy=cfn_execution_policy,
+            custom_permissions_boundary=custom_permissions_boundary,
+            example_permissions_boundary=example_permissions_boundary,
+            execute=execute,
+            force=force,
+            public_access_block_configuration=public_access_block_configuration,
+            qualifier=qualifier,
+            show_template=show_template,
+            template=template,
+            termination_protection=termination_protection,
+            toolkit_stack_name=toolkit_stack_name,
+            trust=trust,
+            trust_for_lookup=trust_for_lookup,
+            use_previous_parameters=use_previous_parameters,
+            asset_metadata=asset_metadata,
+            ca_bundle_path=ca_bundle_path,
+            color=color,
+            context=context,
+            debug=debug,
+            ec2_creds=ec2_creds,
+            ignore_errors=ignore_errors,
+            json=json,
+            lookups=lookups,
+            notices=notices,
+            path_metadata=path_metadata,
+            profile=profile,
+            proxy=proxy,
+            role_arn=role_arn,
+            stacks=stacks,
+            staging=staging,
+            strict=strict,
+            trace=trace,
+            verbose=verbose,
+            version_reporting=version_reporting,
+        )
+
+        return typing.cast(None, jsii.invoke(self, "bootstrap", [options]))
+
     @jsii.member(jsii_name="deploy")
     def deploy(
         self,
         *,
         asset_parallelism: typing.Optional[builtins.bool] = None,
         asset_prebuild: typing.Optional[builtins.bool] = None,
         change_set_name: typing.Optional[builtins.str] = None,
@@ -1902,14 +2122,140 @@
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c9bfa499e48a3fc09d071d19e318c0bc809314da2a23cf1b26886e4c5890f959)
             check_type(argname="argument producer", value=producer, expected_type=type_hints["producer"])
         return typing.cast("AwsCdkCli", jsii.sinvoke(cls, "fromCloudAssemblyDirectoryProducer", [producer]))
 
+    @jsii.member(jsii_name="bootstrap")
+    def bootstrap(
+        self,
+        *,
+        bootstrap_bucket_name: typing.Optional[builtins.str] = None,
+        bootstrap_customer_key: typing.Optional[builtins.str] = None,
+        bootstrap_kms_key_id: typing.Optional[builtins.str] = None,
+        cfn_execution_policy: typing.Optional[builtins.str] = None,
+        custom_permissions_boundary: typing.Optional[builtins.str] = None,
+        example_permissions_boundary: typing.Optional[builtins.bool] = None,
+        execute: typing.Optional[builtins.bool] = None,
+        force: typing.Optional[builtins.bool] = None,
+        public_access_block_configuration: typing.Optional[builtins.str] = None,
+        qualifier: typing.Optional[builtins.str] = None,
+        show_template: typing.Optional[builtins.bool] = None,
+        template: typing.Optional[builtins.str] = None,
+        termination_protection: typing.Optional[builtins.bool] = None,
+        toolkit_stack_name: typing.Optional[builtins.str] = None,
+        trust: typing.Optional[builtins.str] = None,
+        trust_for_lookup: typing.Optional[builtins.str] = None,
+        use_previous_parameters: typing.Optional[builtins.bool] = None,
+        asset_metadata: typing.Optional[builtins.bool] = None,
+        ca_bundle_path: typing.Optional[builtins.str] = None,
+        color: typing.Optional[builtins.bool] = None,
+        context: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        debug: typing.Optional[builtins.bool] = None,
+        ec2_creds: typing.Optional[builtins.bool] = None,
+        ignore_errors: typing.Optional[builtins.bool] = None,
+        json: typing.Optional[builtins.bool] = None,
+        lookups: typing.Optional[builtins.bool] = None,
+        notices: typing.Optional[builtins.bool] = None,
+        path_metadata: typing.Optional[builtins.bool] = None,
+        profile: typing.Optional[builtins.str] = None,
+        proxy: typing.Optional[builtins.str] = None,
+        role_arn: typing.Optional[builtins.str] = None,
+        stacks: typing.Optional[typing.Sequence[builtins.str]] = None,
+        staging: typing.Optional[builtins.bool] = None,
+        strict: typing.Optional[builtins.bool] = None,
+        trace: typing.Optional[builtins.bool] = None,
+        verbose: typing.Optional[builtins.bool] = None,
+        version_reporting: typing.Optional[builtins.bool] = None,
+    ) -> None:
+        '''(experimental) cdk bootstrap.
+
+        :param bootstrap_bucket_name: (experimental) The name of the CDK toolkit bucket; bucket will be created and must not exist Default: - auto-generated CloudFormation name
+        :param bootstrap_customer_key: (experimental) Create a Customer Master Key (CMK) for the bootstrap bucket (you will be charged but can customize permissions, modern bootstrapping only). Default: undefined
+        :param bootstrap_kms_key_id: (experimental) AWS KMS master key ID used for the SSE-KMS encryption. Default: undefined
+        :param cfn_execution_policy: (experimental) The Managed Policy ARNs that should be attached to the role performing deployments into this environment (may be repeated, modern bootstrapping only). Default: - none
+        :param custom_permissions_boundary: (experimental) Use the permissions boundary specified by name. Default: undefined
+        :param example_permissions_boundary: (experimental) Use the example permissions boundary. Default: undefined
+        :param execute: (experimental) Whether to execute ChangeSet (--no-execute will NOT execute the ChangeSet). Default: true
+        :param force: (experimental) Always bootstrap even if it would downgrade template version. Default: false
+        :param public_access_block_configuration: (experimental) Block public access configuration on CDK toolkit bucket (enabled by default). Default: undefined
+        :param qualifier: (experimental) String which must be unique for each bootstrap stack. You must configure it on your CDK app if you change this from the default. Default: undefined
+        :param show_template: (experimental) Instead of actual bootstrapping, print the current CLI's bootstrapping template to stdout for customization. Default: false
+        :param template: (experimental) Use the template from the given file instead of the built-in one (use --show-template to obtain an example).
+        :param termination_protection: (experimental) Toggle CloudFormation termination protection on the bootstrap stacks. Default: false
+        :param toolkit_stack_name: (experimental) The name of the CDK toolkit stack to create.
+        :param trust: (experimental) The AWS account IDs that should be trusted to perform deployments into this environment (may be repeated, modern bootstrapping only). Default: undefined
+        :param trust_for_lookup: (experimental) The AWS account IDs that should be trusted to look up values in this environment (may be repeated, modern bootstrapping only). Default: undefined
+        :param use_previous_parameters: (experimental) Use previous values for existing parameters (you must specify all parameters on every deployment if this is disabled). Default: true
+        :param asset_metadata: (experimental) Include "aws:asset:*" CloudFormation metadata for resources that use assets. Default: true
+        :param ca_bundle_path: (experimental) Path to CA certificate to use when validating HTTPS requests. Default: - read from AWS_CA_BUNDLE environment variable
+        :param color: (experimental) Show colors and other style from console output. Default: - ``true`` unless the environment variable ``NO_COLOR`` is set
+        :param context: (experimental) Additional context. Default: - no additional context
+        :param debug: (experimental) enable emission of additional debugging information, such as creation stack traces of tokens. Default: false
+        :param ec2_creds: (experimental) Force trying to fetch EC2 instance credentials. Default: - guess EC2 instance status
+        :param ignore_errors: (experimental) Ignores synthesis errors, which will likely produce an invalid output. Default: false
+        :param json: (experimental) Use JSON output instead of YAML when templates are printed to STDOUT. Default: false
+        :param lookups: (experimental) Perform context lookups. Synthesis fails if this is disabled and context lookups need to be performed Default: true
+        :param notices: (experimental) Show relevant notices. Default: true
+        :param path_metadata: (experimental) Include "aws:cdk:path" CloudFormation metadata for each resource. Default: true
+        :param profile: (experimental) Use the indicated AWS profile as the default environment. Default: - no profile is used
+        :param proxy: (experimental) Use the indicated proxy. Will read from HTTPS_PROXY environment if specified Default: - no proxy
+        :param role_arn: (experimental) Role to pass to CloudFormation for deployment. Default: - use the bootstrap cfn-exec role
+        :param stacks: (experimental) List of stacks to deploy. Default: - all stacks
+        :param staging: (experimental) Copy assets to the output directory. Needed for local debugging the source files with SAM CLI Default: false
+        :param strict: (experimental) Do not construct stacks with warnings. Default: false
+        :param trace: (experimental) Print trace for stack warnings. Default: false
+        :param verbose: (experimental) show debug logs. Default: false
+        :param version_reporting: (experimental) Include "AWS::CDK::Metadata" resource in synthesized templates. Default: true
+
+        :stability: experimental
+        '''
+        options = BootstrapOptions(
+            bootstrap_bucket_name=bootstrap_bucket_name,
+            bootstrap_customer_key=bootstrap_customer_key,
+            bootstrap_kms_key_id=bootstrap_kms_key_id,
+            cfn_execution_policy=cfn_execution_policy,
+            custom_permissions_boundary=custom_permissions_boundary,
+            example_permissions_boundary=example_permissions_boundary,
+            execute=execute,
+            force=force,
+            public_access_block_configuration=public_access_block_configuration,
+            qualifier=qualifier,
+            show_template=show_template,
+            template=template,
+            termination_protection=termination_protection,
+            toolkit_stack_name=toolkit_stack_name,
+            trust=trust,
+            trust_for_lookup=trust_for_lookup,
+            use_previous_parameters=use_previous_parameters,
+            asset_metadata=asset_metadata,
+            ca_bundle_path=ca_bundle_path,
+            color=color,
+            context=context,
+            debug=debug,
+            ec2_creds=ec2_creds,
+            ignore_errors=ignore_errors,
+            json=json,
+            lookups=lookups,
+            notices=notices,
+            path_metadata=path_metadata,
+            profile=profile,
+            proxy=proxy,
+            role_arn=role_arn,
+            stacks=stacks,
+            staging=staging,
+            strict=strict,
+            trace=trace,
+            verbose=verbose,
+            version_reporting=version_reporting,
+        )
+
+        return typing.cast(None, jsii.ainvoke(self, "bootstrap", [options]))
+
     @jsii.member(jsii_name="deploy")
     def deploy(
         self,
         *,
         asset_parallelism: typing.Optional[builtins.bool] = None,
         asset_prebuild: typing.Optional[builtins.bool] = None,
         change_set_name: typing.Optional[builtins.str] = None,
@@ -2273,14 +2619,735 @@
             version_reporting=version_reporting,
         )
 
         return typing.cast(None, jsii.ainvoke(self, "synth", [options]))
 
 
 @jsii.data_type(
+    jsii_type="@aws-cdk/cli-lib-alpha.BootstrapOptions",
+    jsii_struct_bases=[SharedOptions],
+    name_mapping={
+        "asset_metadata": "assetMetadata",
+        "ca_bundle_path": "caBundlePath",
+        "color": "color",
+        "context": "context",
+        "debug": "debug",
+        "ec2_creds": "ec2Creds",
+        "ignore_errors": "ignoreErrors",
+        "json": "json",
+        "lookups": "lookups",
+        "notices": "notices",
+        "path_metadata": "pathMetadata",
+        "profile": "profile",
+        "proxy": "proxy",
+        "role_arn": "roleArn",
+        "stacks": "stacks",
+        "staging": "staging",
+        "strict": "strict",
+        "trace": "trace",
+        "verbose": "verbose",
+        "version_reporting": "versionReporting",
+        "bootstrap_bucket_name": "bootstrapBucketName",
+        "bootstrap_customer_key": "bootstrapCustomerKey",
+        "bootstrap_kms_key_id": "bootstrapKmsKeyId",
+        "cfn_execution_policy": "cfnExecutionPolicy",
+        "custom_permissions_boundary": "customPermissionsBoundary",
+        "example_permissions_boundary": "examplePermissionsBoundary",
+        "execute": "execute",
+        "force": "force",
+        "public_access_block_configuration": "publicAccessBlockConfiguration",
+        "qualifier": "qualifier",
+        "show_template": "showTemplate",
+        "template": "template",
+        "termination_protection": "terminationProtection",
+        "toolkit_stack_name": "toolkitStackName",
+        "trust": "trust",
+        "trust_for_lookup": "trustForLookup",
+        "use_previous_parameters": "usePreviousParameters",
+    },
+)
+class BootstrapOptions(SharedOptions):
+    def __init__(
+        self,
+        *,
+        asset_metadata: typing.Optional[builtins.bool] = None,
+        ca_bundle_path: typing.Optional[builtins.str] = None,
+        color: typing.Optional[builtins.bool] = None,
+        context: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        debug: typing.Optional[builtins.bool] = None,
+        ec2_creds: typing.Optional[builtins.bool] = None,
+        ignore_errors: typing.Optional[builtins.bool] = None,
+        json: typing.Optional[builtins.bool] = None,
+        lookups: typing.Optional[builtins.bool] = None,
+        notices: typing.Optional[builtins.bool] = None,
+        path_metadata: typing.Optional[builtins.bool] = None,
+        profile: typing.Optional[builtins.str] = None,
+        proxy: typing.Optional[builtins.str] = None,
+        role_arn: typing.Optional[builtins.str] = None,
+        stacks: typing.Optional[typing.Sequence[builtins.str]] = None,
+        staging: typing.Optional[builtins.bool] = None,
+        strict: typing.Optional[builtins.bool] = None,
+        trace: typing.Optional[builtins.bool] = None,
+        verbose: typing.Optional[builtins.bool] = None,
+        version_reporting: typing.Optional[builtins.bool] = None,
+        bootstrap_bucket_name: typing.Optional[builtins.str] = None,
+        bootstrap_customer_key: typing.Optional[builtins.str] = None,
+        bootstrap_kms_key_id: typing.Optional[builtins.str] = None,
+        cfn_execution_policy: typing.Optional[builtins.str] = None,
+        custom_permissions_boundary: typing.Optional[builtins.str] = None,
+        example_permissions_boundary: typing.Optional[builtins.bool] = None,
+        execute: typing.Optional[builtins.bool] = None,
+        force: typing.Optional[builtins.bool] = None,
+        public_access_block_configuration: typing.Optional[builtins.str] = None,
+        qualifier: typing.Optional[builtins.str] = None,
+        show_template: typing.Optional[builtins.bool] = None,
+        template: typing.Optional[builtins.str] = None,
+        termination_protection: typing.Optional[builtins.bool] = None,
+        toolkit_stack_name: typing.Optional[builtins.str] = None,
+        trust: typing.Optional[builtins.str] = None,
+        trust_for_lookup: typing.Optional[builtins.str] = None,
+        use_previous_parameters: typing.Optional[builtins.bool] = None,
+    ) -> None:
+        '''(experimental) Options to use with cdk bootstrap.
+
+        :param asset_metadata: (experimental) Include "aws:asset:*" CloudFormation metadata for resources that use assets. Default: true
+        :param ca_bundle_path: (experimental) Path to CA certificate to use when validating HTTPS requests. Default: - read from AWS_CA_BUNDLE environment variable
+        :param color: (experimental) Show colors and other style from console output. Default: - ``true`` unless the environment variable ``NO_COLOR`` is set
+        :param context: (experimental) Additional context. Default: - no additional context
+        :param debug: (experimental) enable emission of additional debugging information, such as creation stack traces of tokens. Default: false
+        :param ec2_creds: (experimental) Force trying to fetch EC2 instance credentials. Default: - guess EC2 instance status
+        :param ignore_errors: (experimental) Ignores synthesis errors, which will likely produce an invalid output. Default: false
+        :param json: (experimental) Use JSON output instead of YAML when templates are printed to STDOUT. Default: false
+        :param lookups: (experimental) Perform context lookups. Synthesis fails if this is disabled and context lookups need to be performed Default: true
+        :param notices: (experimental) Show relevant notices. Default: true
+        :param path_metadata: (experimental) Include "aws:cdk:path" CloudFormation metadata for each resource. Default: true
+        :param profile: (experimental) Use the indicated AWS profile as the default environment. Default: - no profile is used
+        :param proxy: (experimental) Use the indicated proxy. Will read from HTTPS_PROXY environment if specified Default: - no proxy
+        :param role_arn: (experimental) Role to pass to CloudFormation for deployment. Default: - use the bootstrap cfn-exec role
+        :param stacks: (experimental) List of stacks to deploy. Default: - all stacks
+        :param staging: (experimental) Copy assets to the output directory. Needed for local debugging the source files with SAM CLI Default: false
+        :param strict: (experimental) Do not construct stacks with warnings. Default: false
+        :param trace: (experimental) Print trace for stack warnings. Default: false
+        :param verbose: (experimental) show debug logs. Default: false
+        :param version_reporting: (experimental) Include "AWS::CDK::Metadata" resource in synthesized templates. Default: true
+        :param bootstrap_bucket_name: (experimental) The name of the CDK toolkit bucket; bucket will be created and must not exist Default: - auto-generated CloudFormation name
+        :param bootstrap_customer_key: (experimental) Create a Customer Master Key (CMK) for the bootstrap bucket (you will be charged but can customize permissions, modern bootstrapping only). Default: undefined
+        :param bootstrap_kms_key_id: (experimental) AWS KMS master key ID used for the SSE-KMS encryption. Default: undefined
+        :param cfn_execution_policy: (experimental) The Managed Policy ARNs that should be attached to the role performing deployments into this environment (may be repeated, modern bootstrapping only). Default: - none
+        :param custom_permissions_boundary: (experimental) Use the permissions boundary specified by name. Default: undefined
+        :param example_permissions_boundary: (experimental) Use the example permissions boundary. Default: undefined
+        :param execute: (experimental) Whether to execute ChangeSet (--no-execute will NOT execute the ChangeSet). Default: true
+        :param force: (experimental) Always bootstrap even if it would downgrade template version. Default: false
+        :param public_access_block_configuration: (experimental) Block public access configuration on CDK toolkit bucket (enabled by default). Default: undefined
+        :param qualifier: (experimental) String which must be unique for each bootstrap stack. You must configure it on your CDK app if you change this from the default. Default: undefined
+        :param show_template: (experimental) Instead of actual bootstrapping, print the current CLI's bootstrapping template to stdout for customization. Default: false
+        :param template: (experimental) Use the template from the given file instead of the built-in one (use --show-template to obtain an example).
+        :param termination_protection: (experimental) Toggle CloudFormation termination protection on the bootstrap stacks. Default: false
+        :param toolkit_stack_name: (experimental) The name of the CDK toolkit stack to create.
+        :param trust: (experimental) The AWS account IDs that should be trusted to perform deployments into this environment (may be repeated, modern bootstrapping only). Default: undefined
+        :param trust_for_lookup: (experimental) The AWS account IDs that should be trusted to look up values in this environment (may be repeated, modern bootstrapping only). Default: undefined
+        :param use_previous_parameters: (experimental) Use previous values for existing parameters (you must specify all parameters on every deployment if this is disabled). Default: true
+
+        :stability: experimental
+        :exampleMetadata: fixture=_generated
+
+        Example::
+
+            # The code below shows an example of how to instantiate this type.
+            # The values are placeholders you should change.
+            import aws_cdk.cli_lib_alpha as cli_lib_alpha
+            
+            bootstrap_options = cli_lib_alpha.BootstrapOptions(
+                asset_metadata=False,
+                bootstrap_bucket_name="bootstrapBucketName",
+                bootstrap_customer_key="bootstrapCustomerKey",
+                bootstrap_kms_key_id="bootstrapKmsKeyId",
+                ca_bundle_path="caBundlePath",
+                cfn_execution_policy="cfnExecutionPolicy",
+                color=False,
+                context={
+                    "context_key": "context"
+                },
+                custom_permissions_boundary="customPermissionsBoundary",
+                debug=False,
+                ec2_creds=False,
+                example_permissions_boundary=False,
+                execute=False,
+                force=False,
+                ignore_errors=False,
+                json=False,
+                lookups=False,
+                notices=False,
+                path_metadata=False,
+                profile="profile",
+                proxy="proxy",
+                public_access_block_configuration="publicAccessBlockConfiguration",
+                qualifier="qualifier",
+                role_arn="roleArn",
+                show_template=False,
+                stacks=["stacks"],
+                staging=False,
+                strict=False,
+                template="template",
+                termination_protection=False,
+                toolkit_stack_name="toolkitStackName",
+                trace=False,
+                trust="trust",
+                trust_for_lookup="trustForLookup",
+                use_previous_parameters=False,
+                verbose=False,
+                version_reporting=False
+            )
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__301cfa1f6f197da85fa27bad052a38a0837341d7d0e1901658cbcaf1c29d6582)
+            check_type(argname="argument asset_metadata", value=asset_metadata, expected_type=type_hints["asset_metadata"])
+            check_type(argname="argument ca_bundle_path", value=ca_bundle_path, expected_type=type_hints["ca_bundle_path"])
+            check_type(argname="argument color", value=color, expected_type=type_hints["color"])
+            check_type(argname="argument context", value=context, expected_type=type_hints["context"])
+            check_type(argname="argument debug", value=debug, expected_type=type_hints["debug"])
+            check_type(argname="argument ec2_creds", value=ec2_creds, expected_type=type_hints["ec2_creds"])
+            check_type(argname="argument ignore_errors", value=ignore_errors, expected_type=type_hints["ignore_errors"])
+            check_type(argname="argument json", value=json, expected_type=type_hints["json"])
+            check_type(argname="argument lookups", value=lookups, expected_type=type_hints["lookups"])
+            check_type(argname="argument notices", value=notices, expected_type=type_hints["notices"])
+            check_type(argname="argument path_metadata", value=path_metadata, expected_type=type_hints["path_metadata"])
+            check_type(argname="argument profile", value=profile, expected_type=type_hints["profile"])
+            check_type(argname="argument proxy", value=proxy, expected_type=type_hints["proxy"])
+            check_type(argname="argument role_arn", value=role_arn, expected_type=type_hints["role_arn"])
+            check_type(argname="argument stacks", value=stacks, expected_type=type_hints["stacks"])
+            check_type(argname="argument staging", value=staging, expected_type=type_hints["staging"])
+            check_type(argname="argument strict", value=strict, expected_type=type_hints["strict"])
+            check_type(argname="argument trace", value=trace, expected_type=type_hints["trace"])
+            check_type(argname="argument verbose", value=verbose, expected_type=type_hints["verbose"])
+            check_type(argname="argument version_reporting", value=version_reporting, expected_type=type_hints["version_reporting"])
+            check_type(argname="argument bootstrap_bucket_name", value=bootstrap_bucket_name, expected_type=type_hints["bootstrap_bucket_name"])
+            check_type(argname="argument bootstrap_customer_key", value=bootstrap_customer_key, expected_type=type_hints["bootstrap_customer_key"])
+            check_type(argname="argument bootstrap_kms_key_id", value=bootstrap_kms_key_id, expected_type=type_hints["bootstrap_kms_key_id"])
+            check_type(argname="argument cfn_execution_policy", value=cfn_execution_policy, expected_type=type_hints["cfn_execution_policy"])
+            check_type(argname="argument custom_permissions_boundary", value=custom_permissions_boundary, expected_type=type_hints["custom_permissions_boundary"])
+            check_type(argname="argument example_permissions_boundary", value=example_permissions_boundary, expected_type=type_hints["example_permissions_boundary"])
+            check_type(argname="argument execute", value=execute, expected_type=type_hints["execute"])
+            check_type(argname="argument force", value=force, expected_type=type_hints["force"])
+            check_type(argname="argument public_access_block_configuration", value=public_access_block_configuration, expected_type=type_hints["public_access_block_configuration"])
+            check_type(argname="argument qualifier", value=qualifier, expected_type=type_hints["qualifier"])
+            check_type(argname="argument show_template", value=show_template, expected_type=type_hints["show_template"])
+            check_type(argname="argument template", value=template, expected_type=type_hints["template"])
+            check_type(argname="argument termination_protection", value=termination_protection, expected_type=type_hints["termination_protection"])
+            check_type(argname="argument toolkit_stack_name", value=toolkit_stack_name, expected_type=type_hints["toolkit_stack_name"])
+            check_type(argname="argument trust", value=trust, expected_type=type_hints["trust"])
+            check_type(argname="argument trust_for_lookup", value=trust_for_lookup, expected_type=type_hints["trust_for_lookup"])
+            check_type(argname="argument use_previous_parameters", value=use_previous_parameters, expected_type=type_hints["use_previous_parameters"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if asset_metadata is not None:
+            self._values["asset_metadata"] = asset_metadata
+        if ca_bundle_path is not None:
+            self._values["ca_bundle_path"] = ca_bundle_path
+        if color is not None:
+            self._values["color"] = color
+        if context is not None:
+            self._values["context"] = context
+        if debug is not None:
+            self._values["debug"] = debug
+        if ec2_creds is not None:
+            self._values["ec2_creds"] = ec2_creds
+        if ignore_errors is not None:
+            self._values["ignore_errors"] = ignore_errors
+        if json is not None:
+            self._values["json"] = json
+        if lookups is not None:
+            self._values["lookups"] = lookups
+        if notices is not None:
+            self._values["notices"] = notices
+        if path_metadata is not None:
+            self._values["path_metadata"] = path_metadata
+        if profile is not None:
+            self._values["profile"] = profile
+        if proxy is not None:
+            self._values["proxy"] = proxy
+        if role_arn is not None:
+            self._values["role_arn"] = role_arn
+        if stacks is not None:
+            self._values["stacks"] = stacks
+        if staging is not None:
+            self._values["staging"] = staging
+        if strict is not None:
+            self._values["strict"] = strict
+        if trace is not None:
+            self._values["trace"] = trace
+        if verbose is not None:
+            self._values["verbose"] = verbose
+        if version_reporting is not None:
+            self._values["version_reporting"] = version_reporting
+        if bootstrap_bucket_name is not None:
+            self._values["bootstrap_bucket_name"] = bootstrap_bucket_name
+        if bootstrap_customer_key is not None:
+            self._values["bootstrap_customer_key"] = bootstrap_customer_key
+        if bootstrap_kms_key_id is not None:
+            self._values["bootstrap_kms_key_id"] = bootstrap_kms_key_id
+        if cfn_execution_policy is not None:
+            self._values["cfn_execution_policy"] = cfn_execution_policy
+        if custom_permissions_boundary is not None:
+            self._values["custom_permissions_boundary"] = custom_permissions_boundary
+        if example_permissions_boundary is not None:
+            self._values["example_permissions_boundary"] = example_permissions_boundary
+        if execute is not None:
+            self._values["execute"] = execute
+        if force is not None:
+            self._values["force"] = force
+        if public_access_block_configuration is not None:
+            self._values["public_access_block_configuration"] = public_access_block_configuration
+        if qualifier is not None:
+            self._values["qualifier"] = qualifier
+        if show_template is not None:
+            self._values["show_template"] = show_template
+        if template is not None:
+            self._values["template"] = template
+        if termination_protection is not None:
+            self._values["termination_protection"] = termination_protection
+        if toolkit_stack_name is not None:
+            self._values["toolkit_stack_name"] = toolkit_stack_name
+        if trust is not None:
+            self._values["trust"] = trust
+        if trust_for_lookup is not None:
+            self._values["trust_for_lookup"] = trust_for_lookup
+        if use_previous_parameters is not None:
+            self._values["use_previous_parameters"] = use_previous_parameters
+
+    @builtins.property
+    def asset_metadata(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Include "aws:asset:*" CloudFormation metadata for resources that use assets.
+
+        :default: true
+
+        :stability: experimental
+        '''
+        result = self._values.get("asset_metadata")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def ca_bundle_path(self) -> typing.Optional[builtins.str]:
+        '''(experimental) Path to CA certificate to use when validating HTTPS requests.
+
+        :default: - read from AWS_CA_BUNDLE environment variable
+
+        :stability: experimental
+        '''
+        result = self._values.get("ca_bundle_path")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def color(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Show colors and other style from console output.
+
+        :default: - ``true`` unless the environment variable ``NO_COLOR`` is set
+
+        :stability: experimental
+        '''
+        result = self._values.get("color")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def context(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
+        '''(experimental) Additional context.
+
+        :default: - no additional context
+
+        :stability: experimental
+        '''
+        result = self._values.get("context")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
+
+    @builtins.property
+    def debug(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) enable emission of additional debugging information, such as creation stack traces of tokens.
+
+        :default: false
+
+        :stability: experimental
+        '''
+        result = self._values.get("debug")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def ec2_creds(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Force trying to fetch EC2 instance credentials.
+
+        :default: - guess EC2 instance status
+
+        :stability: experimental
+        '''
+        result = self._values.get("ec2_creds")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def ignore_errors(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Ignores synthesis errors, which will likely produce an invalid output.
+
+        :default: false
+
+        :stability: experimental
+        '''
+        result = self._values.get("ignore_errors")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def json(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Use JSON output instead of YAML when templates are printed to STDOUT.
+
+        :default: false
+
+        :stability: experimental
+        '''
+        result = self._values.get("json")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def lookups(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Perform context lookups.
+
+        Synthesis fails if this is disabled and context lookups need
+        to be performed
+
+        :default: true
+
+        :stability: experimental
+        '''
+        result = self._values.get("lookups")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def notices(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Show relevant notices.
+
+        :default: true
+
+        :stability: experimental
+        '''
+        result = self._values.get("notices")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def path_metadata(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Include "aws:cdk:path" CloudFormation metadata for each resource.
+
+        :default: true
+
+        :stability: experimental
+        '''
+        result = self._values.get("path_metadata")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def profile(self) -> typing.Optional[builtins.str]:
+        '''(experimental) Use the indicated AWS profile as the default environment.
+
+        :default: - no profile is used
+
+        :stability: experimental
+        '''
+        result = self._values.get("profile")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def proxy(self) -> typing.Optional[builtins.str]:
+        '''(experimental) Use the indicated proxy.
+
+        Will read from
+        HTTPS_PROXY environment if specified
+
+        :default: - no proxy
+
+        :stability: experimental
+        '''
+        result = self._values.get("proxy")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def role_arn(self) -> typing.Optional[builtins.str]:
+        '''(experimental) Role to pass to CloudFormation for deployment.
+
+        :default: - use the bootstrap cfn-exec role
+
+        :stability: experimental
+        '''
+        result = self._values.get("role_arn")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def stacks(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''(experimental) List of stacks to deploy.
+
+        :default: - all stacks
+
+        :stability: experimental
+        '''
+        result = self._values.get("stacks")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+
+    @builtins.property
+    def staging(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Copy assets to the output directory.
+
+        Needed for local debugging the source files with SAM CLI
+
+        :default: false
+
+        :stability: experimental
+        '''
+        result = self._values.get("staging")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def strict(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Do not construct stacks with warnings.
+
+        :default: false
+
+        :stability: experimental
+        '''
+        result = self._values.get("strict")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def trace(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Print trace for stack warnings.
+
+        :default: false
+
+        :stability: experimental
+        '''
+        result = self._values.get("trace")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def verbose(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) show debug logs.
+
+        :default: false
+
+        :stability: experimental
+        '''
+        result = self._values.get("verbose")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def version_reporting(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Include "AWS::CDK::Metadata" resource in synthesized templates.
+
+        :default: true
+
+        :stability: experimental
+        '''
+        result = self._values.get("version_reporting")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def bootstrap_bucket_name(self) -> typing.Optional[builtins.str]:
+        '''(experimental) The name of the CDK toolkit bucket;
+
+        bucket will be created and
+        must not exist
+
+        :default: - auto-generated CloudFormation name
+
+        :stability: experimental
+        '''
+        result = self._values.get("bootstrap_bucket_name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def bootstrap_customer_key(self) -> typing.Optional[builtins.str]:
+        '''(experimental) Create a Customer Master Key (CMK) for the bootstrap bucket (you will be charged but can customize permissions, modern bootstrapping only).
+
+        :default: undefined
+
+        :stability: experimental
+        '''
+        result = self._values.get("bootstrap_customer_key")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def bootstrap_kms_key_id(self) -> typing.Optional[builtins.str]:
+        '''(experimental) AWS KMS master key ID used for the SSE-KMS encryption.
+
+        :default: undefined
+
+        :stability: experimental
+        '''
+        result = self._values.get("bootstrap_kms_key_id")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def cfn_execution_policy(self) -> typing.Optional[builtins.str]:
+        '''(experimental) The Managed Policy ARNs that should be attached to the role performing deployments into this environment (may be repeated, modern bootstrapping only).
+
+        :default: - none
+
+        :stability: experimental
+        '''
+        result = self._values.get("cfn_execution_policy")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def custom_permissions_boundary(self) -> typing.Optional[builtins.str]:
+        '''(experimental) Use the permissions boundary specified by name.
+
+        :default: undefined
+
+        :stability: experimental
+        '''
+        result = self._values.get("custom_permissions_boundary")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def example_permissions_boundary(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Use the example permissions boundary.
+
+        :default: undefined
+
+        :stability: experimental
+        '''
+        result = self._values.get("example_permissions_boundary")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def execute(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Whether to execute ChangeSet (--no-execute will NOT execute the ChangeSet).
+
+        :default: true
+
+        :stability: experimental
+        '''
+        result = self._values.get("execute")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def force(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Always bootstrap even if it would downgrade template version.
+
+        :default: false
+
+        :stability: experimental
+        '''
+        result = self._values.get("force")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def public_access_block_configuration(self) -> typing.Optional[builtins.str]:
+        '''(experimental) Block public access configuration on CDK toolkit bucket (enabled by default).
+
+        :default: undefined
+
+        :stability: experimental
+        '''
+        result = self._values.get("public_access_block_configuration")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def qualifier(self) -> typing.Optional[builtins.str]:
+        '''(experimental) String which must be unique for each bootstrap stack.
+
+        You
+        must configure it on your CDK app if you change this
+        from the default.
+
+        :default: undefined
+
+        :stability: experimental
+        '''
+        result = self._values.get("qualifier")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def show_template(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Instead of actual bootstrapping, print the current CLI's bootstrapping template to stdout for customization.
+
+        :default: false
+
+        :stability: experimental
+        '''
+        result = self._values.get("show_template")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def template(self) -> typing.Optional[builtins.str]:
+        '''(experimental) Use the template from the given file instead of the built-in one (use --show-template to obtain an example).
+
+        :stability: experimental
+        '''
+        result = self._values.get("template")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def termination_protection(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Toggle CloudFormation termination protection on the bootstrap stacks.
+
+        :default: false
+
+        :stability: experimental
+        '''
+        result = self._values.get("termination_protection")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def toolkit_stack_name(self) -> typing.Optional[builtins.str]:
+        '''(experimental) The name of the CDK toolkit stack to create.
+
+        :stability: experimental
+        '''
+        result = self._values.get("toolkit_stack_name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def trust(self) -> typing.Optional[builtins.str]:
+        '''(experimental) The AWS account IDs that should be trusted to perform deployments into this environment (may be repeated, modern bootstrapping only).
+
+        :default: undefined
+
+        :stability: experimental
+        '''
+        result = self._values.get("trust")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def trust_for_lookup(self) -> typing.Optional[builtins.str]:
+        '''(experimental) The AWS account IDs that should be trusted to look up values in this environment (may be repeated, modern bootstrapping only).
+
+        :default: undefined
+
+        :stability: experimental
+        '''
+        result = self._values.get("trust_for_lookup")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def use_previous_parameters(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Use previous values for existing parameters (you must specify all parameters on every deployment if this is disabled).
+
+        :default: true
+
+        :stability: experimental
+        '''
+        result = self._values.get("use_previous_parameters")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "BootstrapOptions(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
     jsii_type="@aws-cdk/cli-lib-alpha.DeployOptions",
     jsii_struct_bases=[SharedOptions],
     name_mapping={
         "asset_metadata": "assetMetadata",
         "ca_bundle_path": "caBundlePath",
         "color": "color",
         "context": "context",
@@ -3810,14 +4877,15 @@
         return "ListOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
     "AwsCdkCli",
+    "BootstrapOptions",
     "CdkAppDirectoryProps",
     "DeployOptions",
     "DestroyOptions",
     "IAwsCdkCli",
     "ICloudAssemblyDirectoryProducer",
     "ListOptions",
     "RequireApproval",
@@ -3914,14 +4982,57 @@
 
 def _typecheckingstub__c9bfa499e48a3fc09d071d19e318c0bc809314da2a23cf1b26886e4c5890f959(
     producer: ICloudAssemblyDirectoryProducer,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__301cfa1f6f197da85fa27bad052a38a0837341d7d0e1901658cbcaf1c29d6582(
+    *,
+    asset_metadata: typing.Optional[builtins.bool] = None,
+    ca_bundle_path: typing.Optional[builtins.str] = None,
+    color: typing.Optional[builtins.bool] = None,
+    context: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    debug: typing.Optional[builtins.bool] = None,
+    ec2_creds: typing.Optional[builtins.bool] = None,
+    ignore_errors: typing.Optional[builtins.bool] = None,
+    json: typing.Optional[builtins.bool] = None,
+    lookups: typing.Optional[builtins.bool] = None,
+    notices: typing.Optional[builtins.bool] = None,
+    path_metadata: typing.Optional[builtins.bool] = None,
+    profile: typing.Optional[builtins.str] = None,
+    proxy: typing.Optional[builtins.str] = None,
+    role_arn: typing.Optional[builtins.str] = None,
+    stacks: typing.Optional[typing.Sequence[builtins.str]] = None,
+    staging: typing.Optional[builtins.bool] = None,
+    strict: typing.Optional[builtins.bool] = None,
+    trace: typing.Optional[builtins.bool] = None,
+    verbose: typing.Optional[builtins.bool] = None,
+    version_reporting: typing.Optional[builtins.bool] = None,
+    bootstrap_bucket_name: typing.Optional[builtins.str] = None,
+    bootstrap_customer_key: typing.Optional[builtins.str] = None,
+    bootstrap_kms_key_id: typing.Optional[builtins.str] = None,
+    cfn_execution_policy: typing.Optional[builtins.str] = None,
+    custom_permissions_boundary: typing.Optional[builtins.str] = None,
+    example_permissions_boundary: typing.Optional[builtins.bool] = None,
+    execute: typing.Optional[builtins.bool] = None,
+    force: typing.Optional[builtins.bool] = None,
+    public_access_block_configuration: typing.Optional[builtins.str] = None,
+    qualifier: typing.Optional[builtins.str] = None,
+    show_template: typing.Optional[builtins.bool] = None,
+    template: typing.Optional[builtins.str] = None,
+    termination_protection: typing.Optional[builtins.bool] = None,
+    toolkit_stack_name: typing.Optional[builtins.str] = None,
+    trust: typing.Optional[builtins.str] = None,
+    trust_for_lookup: typing.Optional[builtins.str] = None,
+    use_previous_parameters: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__b018eeefbacd83149d0e1a84a6c871f9439b9b3ae192abb0cdb3973220e72861(
     *,
     asset_metadata: typing.Optional[builtins.bool] = None,
     ca_bundle_path: typing.Optional[builtins.str] = None,
     color: typing.Optional[builtins.bool] = None,
     context: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     debug: typing.Optional[builtins.bool] = None,
```

### Comparing `aws-cdk.cli-lib-alpha-2.86.0a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO` & `aws-cdk.cli-lib-alpha-2.87.0a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cli-lib-alpha
-Version: 2.86.0a0
+Version: 2.87.0a0
 Summary: AWS CDK Programmatic CLI library
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -56,14 +56,15 @@
 ## Overview
 
 Provides a library to interact with the AWS CDK CLI programmatically from jsii supported languages.
 Currently the package includes implementations for:
 
 * `cdk deploy`
 * `cdk synth`
+* `cdk bootstrap`
 * `cdk destroy`
 * `cdk list`
 
 ## Setup
 
 ### AWS CDK app directory
 
@@ -116,14 +117,21 @@
 ```python
 # await this asynchronous method call using a language feature
 cli.synth(
     stacks=["MyTestStack"]
 )
 ```
 
+### bootstrap
+
+```python
+# await this asynchronous method call using a language feature
+cli.bootstrap()
+```
+
 ### deploy
 
 ```python
 # await this asynchronous method call using a language feature
 cli.deploy(
     stacks=["MyTestStack"]
 )
```

