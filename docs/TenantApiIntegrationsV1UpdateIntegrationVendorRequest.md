# TenantApiIntegrationsV1UpdateIntegrationVendorRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**integration_type_ids** | **List[str]** |  | [optional] [readonly] 
**code** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_integrations_v1_update_integration_vendor_request import TenantApiIntegrationsV1UpdateIntegrationVendorRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiIntegrationsV1UpdateIntegrationVendorRequest from a JSON string
tenant_api_integrations_v1_update_integration_vendor_request_instance = TenantApiIntegrationsV1UpdateIntegrationVendorRequest.from_json(json)
# print the JSON string representation of the object
print(TenantApiIntegrationsV1UpdateIntegrationVendorRequest.to_json())

# convert the object into a dict
tenant_api_integrations_v1_update_integration_vendor_request_dict = tenant_api_integrations_v1_update_integration_vendor_request_instance.to_dict()
# create an instance of TenantApiIntegrationsV1UpdateIntegrationVendorRequest from a dict
tenant_api_integrations_v1_update_integration_vendor_request_from_dict = TenantApiIntegrationsV1UpdateIntegrationVendorRequest.from_dict(tenant_api_integrations_v1_update_integration_vendor_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


