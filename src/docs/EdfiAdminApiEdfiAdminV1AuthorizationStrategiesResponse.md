# EdfiAdminApiEdfiAdminV1AuthorizationStrategiesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_authorization_strategies_response import EdfiAdminApiEdfiAdminV1AuthorizationStrategiesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1AuthorizationStrategiesResponse from a JSON string
edfi_admin_api_edfi_admin_v1_authorization_strategies_response_instance = EdfiAdminApiEdfiAdminV1AuthorizationStrategiesResponse.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1AuthorizationStrategiesResponse.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_authorization_strategies_response_dict = edfi_admin_api_edfi_admin_v1_authorization_strategies_response_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1AuthorizationStrategiesResponse from a dict
edfi_admin_api_edfi_admin_v1_authorization_strategies_response_from_dict = EdfiAdminApiEdfiAdminV1AuthorizationStrategiesResponse.from_dict(edfi_admin_api_edfi_admin_v1_authorization_strategies_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


