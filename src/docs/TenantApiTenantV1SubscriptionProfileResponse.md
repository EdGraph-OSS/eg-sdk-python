# TenantApiTenantV1SubscriptionProfileResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**subscription_id** | **str** |  | [optional] 
**application_id** | **str** |  | [optional] 
**start_date_time** | **str** |  | [optional] 
**end_date_time** | **str** |  | [optional] 
**actual_end_date_time** | **str** |  | [optional] 
**grace_period** | **int** |  | [optional] 
**number_of_licenses** | **int** |  | [optional] 
**assigned_licenses** | **int** |  | [optional] 
**max_assigned_licenses** | **int** |  | [optional] 
**last_max_assigned_licenses_date_time** | **str** |  | [optional] 
**license_type** | [**TenantApiTenantV1LicenseType**](TenantApiTenantV1LicenseType.md) |  | [optional] 
**subscription_status** | [**TenantApiTenantV1SubscriptionStatus**](TenantApiTenantV1SubscriptionStatus.md) |  | [optional] 
**auto_assign** | **bool** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**deleted_at** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_subscription_profile_response import TenantApiTenantV1SubscriptionProfileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1SubscriptionProfileResponse from a JSON string
tenant_api_tenant_v1_subscription_profile_response_instance = TenantApiTenantV1SubscriptionProfileResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1SubscriptionProfileResponse.to_json())

# convert the object into a dict
tenant_api_tenant_v1_subscription_profile_response_dict = tenant_api_tenant_v1_subscription_profile_response_instance.to_dict()
# create an instance of TenantApiTenantV1SubscriptionProfileResponse from a dict
tenant_api_tenant_v1_subscription_profile_response_from_dict = TenantApiTenantV1SubscriptionProfileResponse.from_dict(tenant_api_tenant_v1_subscription_profile_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


