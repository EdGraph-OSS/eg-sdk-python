# TenantApiTenantV1TenantBrandingResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** |  | [optional] 
**brand_name** | **str** |  | [optional] 
**logo** | [**TenantApiTenantV1TenantBrandingLogo**](TenantApiTenantV1TenantBrandingLogo.md) |  | [optional] 
**background** | [**TenantApiTenantV1TenantBrandingBackground**](TenantApiTenantV1TenantBrandingBackground.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_tenant_branding_response import TenantApiTenantV1TenantBrandingResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1TenantBrandingResponse from a JSON string
tenant_api_tenant_v1_tenant_branding_response_instance = TenantApiTenantV1TenantBrandingResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1TenantBrandingResponse.to_json())

# convert the object into a dict
tenant_api_tenant_v1_tenant_branding_response_dict = tenant_api_tenant_v1_tenant_branding_response_instance.to_dict()
# create an instance of TenantApiTenantV1TenantBrandingResponse from a dict
tenant_api_tenant_v1_tenant_branding_response_from_dict = TenantApiTenantV1TenantBrandingResponse.from_dict(tenant_api_tenant_v1_tenant_branding_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


