# TenantApiTenantV1SubscriptionUpdatedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**subscription_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_subscription_updated_response import TenantApiTenantV1SubscriptionUpdatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1SubscriptionUpdatedResponse from a JSON string
tenant_api_tenant_v1_subscription_updated_response_instance = TenantApiTenantV1SubscriptionUpdatedResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1SubscriptionUpdatedResponse.to_json())

# convert the object into a dict
tenant_api_tenant_v1_subscription_updated_response_dict = tenant_api_tenant_v1_subscription_updated_response_instance.to_dict()
# create an instance of TenantApiTenantV1SubscriptionUpdatedResponse from a dict
tenant_api_tenant_v1_subscription_updated_response_from_dict = TenantApiTenantV1SubscriptionUpdatedResponse.from_dict(tenant_api_tenant_v1_subscription_updated_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


