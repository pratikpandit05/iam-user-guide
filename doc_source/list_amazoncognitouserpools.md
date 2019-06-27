# Actions, Resources, and Condition Keys for Amazon Cognito User Pools<a name="list_amazoncognitouserpools"></a>

Amazon Cognito User Pools \(service prefix: `cognito-idp`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](https://docs.aws.amazon.com/cognito/latest/developerguide/)\.
+ View a [list of the API operations available for this service](https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/)\.
+ Learn how to protect this service and its resources by [using IAM](https://docs.aws.amazon.com/cognito/latest/developerguide/resource-permissions.html#amazon-cognito-amazon-resource-names) permission policies\.

**Topics**
+ [Actions Defined by Amazon Cognito User Pools](#amazoncognitouserpools-actions-as-permissions)
+ [Resources Defined by Amazon Cognito User Pools](#amazoncognitouserpools-resources-for-iam-policies)
+ [Condition Keys for Amazon Cognito User Pools](#amazoncognitouserpools-policy-keys)

## Actions Defined by Amazon Cognito User Pools<a name="amazoncognitouserpools-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. By using policies, you define the permissions for anyone performing an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\. For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  
[\[See the AWS documentation website for more details\]](http://docs.aws.amazon.com/IAM/latest/UserGuide/list_amazoncognitouserpools.html)

## Resources Defined by Amazon Cognito User Pools<a name="amazoncognitouserpools-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#amazoncognitouserpools-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The Resource Types Table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource Types | ARN | Condition Keys | 
| --- | --- | --- | 
|   [ userpool ](https://docs.aws.amazon.com/cognito/latest/developerguide/resource-permissions.html#amazon-cognito-amazon-resource-names)  |  arn:$\{Partition\}:cognito\-idp:$\{Region\}:$\{Account\}:userpool/$\{UserPoolId\}  |   [ aws:ResourceTag/$\{TagKey\} ](#amazoncognitouserpools-aws_ResourceTag___TagKey_)   | 

## Condition Keys for Amazon Cognito User Pools<a name="amazoncognitouserpools-policy-keys"></a>

Amazon Cognito User Pools defines the following condition keys that can be used in the `Condition` element of an IAM policy\. You can use these keys to further refine the conditions under which the policy statement applies\. For details about the columns in the following table, see [The Condition Keys Table](reference_policies_actions-resources-contextkeys.md#context_keys_table)\.

To view the global condition keys that are available to all services, see [Available Global Condition Keys](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.


****  

| Condition Keys | Description | Type | 
| --- | --- | --- | 
|   [ aws:RequestTag/$\{TagKey\} ](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_condition-keys.html#condition-keys-requesttag)  | Filters actions based on the presence of tag key\-value pairs in the request\. | String | 
|   [ aws:ResourceTag/$\{TagKey\} ](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_condition-keys.html#condition-keys-resourcetag)  | Filters actions based on tag key\-value pairs attached to the resource\. | String | 
|   [ aws:TagKeys ](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_condition-keys.html#condition-keys-tagkeys)  | Filters access by a key that is present in the request\. | String | 