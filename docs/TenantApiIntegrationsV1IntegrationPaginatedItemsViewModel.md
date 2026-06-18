# TenantApiIntegrationsV1IntegrationPaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[TenantApiIntegrationsV1Integration]**](TenantApiIntegrationsV1Integration.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_integrations_v1_integration_paginated_items_view_model import TenantApiIntegrationsV1IntegrationPaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiIntegrationsV1IntegrationPaginatedItemsViewModel from a JSON string
tenant_api_integrations_v1_integration_paginated_items_view_model_instance = TenantApiIntegrationsV1IntegrationPaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(TenantApiIntegrationsV1IntegrationPaginatedItemsViewModel.to_json())

# convert the object into a dict
tenant_api_integrations_v1_integration_paginated_items_view_model_dict = tenant_api_integrations_v1_integration_paginated_items_view_model_instance.to_dict()
# create an instance of TenantApiIntegrationsV1IntegrationPaginatedItemsViewModel from a dict
tenant_api_integrations_v1_integration_paginated_items_view_model_from_dict = TenantApiIntegrationsV1IntegrationPaginatedItemsViewModel.from_dict(tenant_api_integrations_v1_integration_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


