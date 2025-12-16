# TenantApiTenantV1UpdateSubscriptionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**subscription_id** | **str** |  | [optional] 
**start_date_time** | **str** |  | [optional] 
**end_date_time** | **str** |  | [optional] 
**grace_period** | **int** |  | [optional] 
**number_of_licenses** | **int** |  | [optional] 
**assigned_licenses** | **int** |  | [optional] 
**license_type** | [**TenantApiTenantV1LicenseType**](TenantApiTenantV1LicenseType.md) |  | [optional] 
**auto_assign** | **bool** | SubscriptionStatus SubscriptionStatus &#x3D; 10; | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_update_subscription_request import TenantApiTenantV1UpdateSubscriptionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1UpdateSubscriptionRequest from a JSON string
tenant_api_tenant_v1_update_subscription_request_instance = TenantApiTenantV1UpdateSubscriptionRequest.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1UpdateSubscriptionRequest.to_json())

# convert the object into a dict
tenant_api_tenant_v1_update_subscription_request_dict = tenant_api_tenant_v1_update_subscription_request_instance.to_dict()
# create an instance of TenantApiTenantV1UpdateSubscriptionRequest from a dict
tenant_api_tenant_v1_update_subscription_request_from_dict = TenantApiTenantV1UpdateSubscriptionRequest.from_dict(tenant_api_tenant_v1_update_subscription_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


