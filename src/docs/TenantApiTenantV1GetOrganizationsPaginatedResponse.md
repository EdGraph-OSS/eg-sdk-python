# TenantApiTenantV1GetOrganizationsPaginatedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[TenantApiTenantV1Organization]**](TenantApiTenantV1Organization.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.tenant_api_tenant_v1_get_organizations_paginated_response import TenantApiTenantV1GetOrganizationsPaginatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiTenantV1GetOrganizationsPaginatedResponse from a JSON string
tenant_api_tenant_v1_get_organizations_paginated_response_instance = TenantApiTenantV1GetOrganizationsPaginatedResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiTenantV1GetOrganizationsPaginatedResponse.to_json())

# convert the object into a dict
tenant_api_tenant_v1_get_organizations_paginated_response_dict = tenant_api_tenant_v1_get_organizations_paginated_response_instance.to_dict()
# create an instance of TenantApiTenantV1GetOrganizationsPaginatedResponse from a dict
tenant_api_tenant_v1_get_organizations_paginated_response_from_dict = TenantApiTenantV1GetOrganizationsPaginatedResponse.from_dict(tenant_api_tenant_v1_get_organizations_paginated_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


