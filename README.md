# ![LOGO](logo.png) CostManagementClient **flow**ground Connector

## Description

A generated **flow**ground connector for the CostManagementClient API (version 2019-03-01-preview).

Generated from: https://api.apis.guru/v2/specs/azure.com/cost-management-costmanagement/2019-03-01-preview/swagger.json<br/>
Generated at: 2019-05-07T17:37:54+03:00

## API Description



## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Forecast the usage data for department.

*Tags:* `Forecast`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `billingAccountId` - _required_ - BillingAccount ID
* `departmentId` - _required_ - Department ID

### Query the usage data for department.

*Tags:* `Query`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `billingAccountId` - _required_ - BillingAccount ID
* `departmentId` - _required_ - Department ID

### Lists the dimensions by Department Id.

*Tags:* `Dimensions`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `billingAccountId` - _required_ - BillingAccount ID
* `departmentId` - _required_ - Department ID
* `$filter` - _optional_ - May be used to filter dimensions by properties/category, properties/usageStart, properties/usageEnd. Supported operators are 'eq','lt', 'gt', 'le', 'ge'.
* `$expand` - _optional_ - May be used to expand the properties/data within a dimension category. By default, data is not included when listing dimensions.
* `$skiptoken` - _optional_ - Skiptoken is only used if a previous operation returned a partial result. If a previous response contains a nextLink element, the value of the nextLink element will include a skiptoken parameter that specifies a starting point to use for subsequent calls.
* `$top` - _optional_ - May be used to limit the number of results to the most recent N dimension data.

### Forecast the usage data for an enrollment account.

*Tags:* `Forecast`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `billingAccountId` - _required_ - BillingAccount ID
* `enrollmentAccountId` - _required_ - Enrollment Account ID

### Query the usage data for an enrollment account.

*Tags:* `Query`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `billingAccountId` - _required_ - BillingAccount ID
* `enrollmentAccountId` - _required_ - Enrollment Account ID

### Lists the dimensions by Enrollment Account Id.

*Tags:* `Dimensions`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `billingAccountId` - _required_ - BillingAccount ID
* `enrollmentAccountId` - _required_ - Enrollment Account ID
* `$filter` - _optional_ - May be used to filter dimensions by properties/category, properties/usageStart, properties/usageEnd. Supported operators are 'eq','lt', 'gt', 'le', 'ge'.
* `$expand` - _optional_ - May be used to expand the properties/data within a dimension category. By default, data is not included when listing dimensions.
* `$skiptoken` - _optional_ - Skiptoken is only used if a previous operation returned a partial result. If a previous response contains a nextLink element, the value of the nextLink element will include a skiptoken parameter that specifies a starting point to use for subsequent calls.
* `$top` - _optional_ - May be used to limit the number of results to the most recent N dimension data.

### Forecast the usage data for billing account.

*Tags:* `Forecast`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `billingAccountId` - _required_ - BillingAccount ID

### Query the usage data for billing account.

*Tags:* `Query`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `billingAccountId` - _required_ - BillingAccount ID

### Lists the dimensions by billingAccount Id.

*Tags:* `Dimensions`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `billingAccountId` - _required_ - BillingAccount ID
* `$filter` - _optional_ - May be used to filter dimensions by properties/category, properties/usageStart, properties/usageEnd. Supported operators are 'eq','lt', 'gt', 'le', 'ge'.
* `$expand` - _optional_ - May be used to expand the properties/data within a dimension category. By default, data is not included when listing dimensions.
* `$skiptoken` - _optional_ - Skiptoken is only used if a previous operation returned a partial result. If a previous response contains a nextLink element, the value of the nextLink element will include a skiptoken parameter that specifies a starting point to use for subsequent calls.
* `$top` - _optional_ - May be used to limit the number of results to the most recent N dimension data.

### Get list all Showback Rules.

*Tags:* `ShowbackRules`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `billingAccountId` - _required_ - BillingAccount ID

### Gets the showback rule by rule name.

*Tags:* `ShowbackRules`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `billingAccountId` - _required_ - BillingAccount ID
* `ruleName` - _required_ - Showback rule name

### Create/Update showback rule for billing account.

*Tags:* `ShowbackRules`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `billingAccountId` - _required_ - BillingAccount ID
* `ruleName` - _required_ - Showback rule name

### List all cloud connector definitions

*Tags:* `CloudConnectors`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview

### Delete a cloud connector definition

*Tags:* `CloudConnectors`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `connectorName` - _required_ - Connector Name.

### Get a cloud connector definition

*Tags:* `CloudConnectors`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `connectorName` - _required_ - Connector Name.
* `$expand` - _optional_ - May be used to expand the collectionInfo property. By default, collectionInfo is not included.

### Update a cloud connector definition

*Tags:* `CloudConnectors`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `connectorName` - _required_ - Connector Name.

### Create or update a cloud connector definition

*Tags:* `CloudConnectors`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `connectorName` - _required_ - Connector Name.

### List all ExternalBillingAccount definitions

*Tags:* `ExternalBillingAccounts`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview

### Get a ExternalBillingAccount definition

*Tags:* `ExternalBillingAccounts`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `externalBillingAccountName` - _required_ - External Billing Account Name. (eg 'aws-{PayerAccountId}')

### List all ExternalSubscriptions by ExternalBillingAccount definitions

*Tags:* `ExternalSubscriptions`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `externalBillingAccountName` - _required_ - External Billing Account Name. (eg 'aws-{PayerAccountId}')

### List all ExternalSubscription definitions

*Tags:* `ExternalSubscriptions`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview

### Get an ExternalSubscription definition

*Tags:* `ExternalSubscriptions`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `externalSubscriptionName` - _required_ - External Subscription Name. (eg 'aws-{UsageAccountId}')

### Lists all of the available consumption REST API operations.

*Tags:* `Operations`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview

### Lists the usage data for management group.

*Tags:* `Forecast`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `managementGroupId` - _required_ - ManagementGroup ID

### Lists the usage data for management group.

*Tags:* `Query`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `managementGroupId` - _required_ - ManagementGroup ID

### Lists the dimensions by managementGroup Id.

*Tags:* `Dimensions`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `managementGroupId` - _required_ - ManagementGroup ID
* `$filter` - _optional_ - May be used to filter dimensions by properties/category, properties/usageStart, properties/usageEnd. Supported operators are 'eq','lt', 'gt', 'le', 'ge'.
* `$expand` - _optional_ - May be used to expand the properties/data within a dimension category. By default, data is not included when listing dimensions.
* `$skiptoken` - _optional_ - Skiptoken is only used if a previous operation returned a partial result. If a previous response contains a nextLink element, the value of the nextLink element will include a skiptoken parameter that specifies a starting point to use for subsequent calls.
* `$top` - _optional_ - May be used to limit the number of results to the most recent N dimension data.

### List all ExternalSubscription definitions for Management Group

*Tags:* `ExternalSubscriptions`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `managementGroupId` - _required_ - ManagementGroup ID

### Associates ExternalSubscription with the management group

*Tags:* `ExternalSubscriptions`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `managementGroupId` - _required_ - ManagementGroup ID
* `externalSubscriptionName` - _required_ - External Subscription Name. (eg 'aws-{UsageAccountId}')

### List all entities (Management Groups, Subscriptions, ExternalSubscriptions, etc.) focusing on a particular group for the authenticated user.

*Tags:* `Entities`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `managementGroupId` - _required_ - ManagementGroup ID
* `$view` - _optional_ - The view parameter allows clients to filter the type of data that is returned by the getEntities call.
    Possible values: FullHierarchy, GroupsOnly, SubscriptionsOnly, ExternalSubscriptionsOnly, Audit.

### Forecast the usage data for subscriptionId.

*Tags:* `Forecast`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `subscriptionId` - _required_ - Azure Subscription ID.

### Query the usage data for subscriptionId.

*Tags:* `Query`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `subscriptionId` - _required_ - Azure Subscription ID.

### Lists the dimensions by subscription Id.

*Tags:* `Dimensions`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `subscriptionId` - _required_ - Azure Subscription ID.
* `$filter` - _optional_ - May be used to filter dimensions by properties/category, properties/usageStart, properties/usageEnd. Supported operators are 'eq','lt', 'gt', 'le', 'ge'.
* `$expand` - _optional_ - May be used to expand the properties/data within a dimension category. By default, data is not included when listing dimensions.
* `$skiptoken` - _optional_ - Skiptoken is only used if a previous operation returned a partial result. If a previous response contains a nextLink element, the value of the nextLink element will include a skiptoken parameter that specifies a starting point to use for subsequent calls.
* `$top` - _optional_ - May be used to limit the number of results to the most recent N dimension data.

### Lists the dimensions by resource group Id.

*Tags:* `Dimensions`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `subscriptionId` - _required_ - Azure Subscription ID.
* `resourceGroupName` - _required_ - Azure Resource Group Name.
* `$filter` - _optional_ - May be used to filter dimensions by properties/category, properties/usageStart, properties/usageEnd. Supported operators are 'eq','lt', 'gt', 'le', 'ge'.
* `$expand` - _optional_ - May be used to expand the properties/data within a dimension category. By default, data is not included when listing dimensions.
* `$skiptoken` - _optional_ - Skiptoken is only used if a previous operation returned a partial result. If a previous response contains a nextLink element, the value of the nextLink element will include a skiptoken parameter that specifies a starting point to use for subsequent calls.
* `$top` - _optional_ - May be used to limit the number of results to the most recent N dimension data.

### Forecast the usage data for subscriptionId and resource group.

*Tags:* `Forecast`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `subscriptionId` - _required_ - Azure Subscription ID.
* `resourceGroupName` - _required_ - Azure Resource Group Name.

### Query the usage data for subscriptionId and resource group.

*Tags:* `Query`

#### Input Parameters
* `api-version` - _required_ - Version of the API to be used with the client request. The current version is 2019-03-01-preview
* `subscriptionId` - _required_ - Azure Subscription ID.
* `resourceGroupName` - _required_ - Azure Resource Group Name.

## License

**flow**ground :- Telekom iPaaS / azure-com-cost-management-costmanagement-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
