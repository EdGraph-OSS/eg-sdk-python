# TenantApiIntegrationsV1CreateIntegrationVendorRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**integration_type_ids** | **List[str]** |  | [optional] [readonly] 
**code** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_integrations_v1_create_integration_vendor_request import TenantApiIntegrationsV1CreateIntegrationVendorRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiIntegrationsV1CreateIntegrationVendorRequest from a JSON string
tenant_api_integrations_v1_create_integration_vendor_request_instance = TenantApiIntegrationsV1CreateIntegrationVendorRequest.from_json(json)
# print the JSON string representation of the object
print(TenantApiIntegrationsV1CreateIntegrationVendorRequest.to_json())

# convert the object into a dict
tenant_api_integrations_v1_create_integration_vendor_request_dict = tenant_api_integrations_v1_create_integration_vendor_request_instance.to_dict()
# create an instance of TenantApiIntegrationsV1CreateIntegrationVendorRequest from a dict
tenant_api_integrations_v1_create_integration_vendor_request_from_dict = TenantApiIntegrationsV1CreateIntegrationVendorRequest.from_dict(tenant_api_integrations_v1_create_integration_vendor_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


