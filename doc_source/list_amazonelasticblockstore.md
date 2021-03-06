# Actions, Resources, and Condition Keys for Amazon Elastic Block Store<a name="list_amazonelasticblockstore"></a>

Amazon Elastic Block Store \(service prefix: `ebs`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](https://docs.aws.amazon.com/ebs/latest/APIReference/Welcome.html)\.
+ View a list of the [API operations available for this service](https://docs.aws.amazon.com/ebs/latest/APIReference/API_Operations.html)\.
+ Learn how to secure this service and its resources by [using IAM](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-accessing-snapshot.html#ebsapi-permissions) permission policies\.

**Topics**
+ [Actions Defined by Amazon Elastic Block Store](#amazonelasticblockstore-actions-as-permissions)
+ [Resource Types Defined by Amazon Elastic Block Store](#amazonelasticblockstore-resources-for-iam-policies)
+ [Condition Keys for Amazon Elastic Block Store](#amazonelasticblockstore-policy-keys)

## Actions Defined by Amazon Elastic Block Store<a name="amazonelasticblockstore-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. Use policies to grant permissions to perform an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\.

The **Resource Types** column indicates whether each action supports resource\-level permissions\. If there is no value for this column, you must specify all resources \("\*"\) in the `Resource` element of your policy statement\. If the column includes a resource type, then you can specify an ARN of that type in a statement with that action\. Required resources are indicated in the table with an asterisk \(\*\)\. If you specify a resource\-level permission ARN in a statement using this action, then it must be of this type\. Some actions support multiple resource types\. If the resource type is optional \(not indicated as required\), then you can choose to use one but not the other\.

For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  

| Actions | Description | Access Level | Resource Types \(\*required\) | Condition Keys | Dependent Actions | 
| --- | --- | --- | --- | --- | --- | 
|   [ GetSnapshotBlock ](https://docs.aws.amazon.com/ebs/latest/APIReference/API_GetSnapshotBlock.html)  | Grants permission to return the data of a block in an Amazon Elastic Block Store \(EBS\) snapshot | Read |   [ snapshot\* ](#amazonelasticblockstore-snapshot)   |  |  | 
|   [ ListChangedBlocks ](https://docs.aws.amazon.com/ebs/latest/APIReference/API_ListChangedBlocks.html)  | Grants permission to list the block indexes and block tokens for blocks that are different between two Amazon Elastic Block Store \(EBS\) snapshots of the same volume/snapshot lineage | Read |   [ snapshot\* ](#amazonelasticblockstore-snapshot)   |  |  | 
|   [ ListSnapshotBlocks ](https://docs.aws.amazon.com/ebs/latest/APIReference/API_ListSnapshotBlocks.html)  | Grants permission to list the block indexes and block tokens for blocks in an Amazon Elastic Block Store \(EBS\) snapshot\. | Read |   [ snapshot\* ](#amazonelasticblockstore-snapshot)   |  |  | 

## Resource Types Defined by Amazon Elastic Block Store<a name="amazonelasticblockstore-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#amazonelasticblockstore-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The Resource Types Table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource Types | ARN | Condition Keys | 
| --- | --- | --- | 
|   [ snapshot ](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/iam-policy-structure.html#EC2_ARN_Format)  |  arn:$\{Partition\}:ec2:$\{Region\}::snapshot/$\{SnapshotId\}  |   [ aws:ResourceTag/$\{TagKey\} ](#amazonelasticblockstore-aws_ResourceTag___TagKey_)   | 

## Condition Keys for Amazon Elastic Block Store<a name="amazonelasticblockstore-policy-keys"></a>

Amazon Elastic Block Store defines the following condition keys that can be used in the `Condition` element of an IAM policy\. You can use these keys to further refine the conditions under which the policy statement applies\. For details about the columns in the following table, see [The Condition Keys Table](reference_policies_actions-resources-contextkeys.md#context_keys_table)\.

To view the global condition keys that are available to all services, see [Available Global Condition Keys](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.


****  

| Condition Keys | Description | Type | 
| --- | --- | --- | 
|   [ aws:ResourceTag/$\{TagKey\} ](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_condition-keys.html#condition-keys-resourcetag)  | Filters access based on tag key\-value pairs assigned to the AWS resource | String | 