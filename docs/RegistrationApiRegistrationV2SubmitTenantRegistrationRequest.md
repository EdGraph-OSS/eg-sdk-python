# RegistrationApiRegistrationV2SubmitTenantRegistrationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_types** | [**List[RegistrationApiRegistrationV2TenantType]**](RegistrationApiRegistrationV2TenantType.md) |  | [optional] [readonly] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**state** | **str** |  | [optional] 
**organization_identifier** | **str** |  | [optional] 
**organization_name** | **str** |  | [optional] 
**password** | **str** |  | [optional] 
**application_ids** | **List[str]** |  | [optional] [readonly] 
**azure_subscription_id** | **str** |  | [optional] 
**azure_subscription_storage_path** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.registration_api_registration_v2_submit_tenant_registration_request import RegistrationApiRegistrationV2SubmitTenantRegistrationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of RegistrationApiRegistrationV2SubmitTenantRegistrationRequest from a JSON string
registration_api_registration_v2_submit_tenant_registration_request_instance = RegistrationApiRegistrationV2SubmitTenantRegistrationRequest.from_json(json)
# print the JSON string representation of the object
print(RegistrationApiRegistrationV2SubmitTenantRegistrationRequest.to_json())

# convert the object into a dict
registration_api_registration_v2_submit_tenant_registration_request_dict = registration_api_registration_v2_submit_tenant_registration_request_instance.to_dict()
# create an instance of RegistrationApiRegistrationV2SubmitTenantRegistrationRequest from a dict
registration_api_registration_v2_submit_tenant_registration_request_from_dict = RegistrationApiRegistrationV2SubmitTenantRegistrationRequest.from_dict(registration_api_registration_v2_submit_tenant_registration_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


