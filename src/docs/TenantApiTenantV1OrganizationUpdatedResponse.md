# TenantApiTenantV1OrganizationUpdatedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**identifier_value** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_organization_updated_response import TenantApiTenantV1OrganizationUpdatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1OrganizationUpdatedResponse from a JSON string
tenant_api_tenant_v1_organization_updated_response_instance = TenantApiTenantV1OrganizationUpdatedResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1OrganizationUpdatedResponse.to_json())

# convert the object into a dict
tenant_api_tenant_v1_organization_updated_response_dict = tenant_api_tenant_v1_organization_updated_response_instance.to_dict()
# create an instance of TenantApiTenantV1OrganizationUpdatedResponse from a dict
tenant_api_tenant_v1_organization_updated_response_from_dict = TenantApiTenantV1OrganizationUpdatedResponse.from_dict(tenant_api_tenant_v1_organization_updated_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


