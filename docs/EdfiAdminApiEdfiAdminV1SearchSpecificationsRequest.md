# EdfiAdminApiEdfiAdminV1SearchSpecificationsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_size** | **int** |  | [optional] 
**page_index** | **int** |  | [optional] 
**order_by** | **str** |  | [optional] 
**filter** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_search_specifications_request import EdfiAdminApiEdfiAdminV1SearchSpecificationsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1SearchSpecificationsRequest from a JSON string
edfi_admin_api_edfi_admin_v1_search_specifications_request_instance = EdfiAdminApiEdfiAdminV1SearchSpecificationsRequest.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1SearchSpecificationsRequest.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_search_specifications_request_dict = edfi_admin_api_edfi_admin_v1_search_specifications_request_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1SearchSpecificationsRequest from a dict
edfi_admin_api_edfi_admin_v1_search_specifications_request_from_dict = EdfiAdminApiEdfiAdminV1SearchSpecificationsRequest.from_dict(edfi_admin_api_edfi_admin_v1_search_specifications_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


