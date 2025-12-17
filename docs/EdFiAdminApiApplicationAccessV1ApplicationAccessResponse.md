# EdFiAdminApiApplicationAccessV1ApplicationAccessResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**application_id** | **int** |  | [optional] 
**api_client_id** | **int** |  | [optional] 
**users** | [**List[EdFiAdminApiApplicationAccessV1ApplicationUserAccessResponse]**](EdFiAdminApiApplicationAccessV1ApplicationUserAccessResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ed_fi_admin_api_application_access_v1_application_access_response import EdFiAdminApiApplicationAccessV1ApplicationAccessResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdFiAdminApiApplicationAccessV1ApplicationAccessResponse from a JSON string
ed_fi_admin_api_application_access_v1_application_access_response_instance = EdFiAdminApiApplicationAccessV1ApplicationAccessResponse.from_json(json)
# print the JSON string representation of the object
print(EdFiAdminApiApplicationAccessV1ApplicationAccessResponse.to_json())

# convert the object into a dict
ed_fi_admin_api_application_access_v1_application_access_response_dict = ed_fi_admin_api_application_access_v1_application_access_response_instance.to_dict()
# create an instance of EdFiAdminApiApplicationAccessV1ApplicationAccessResponse from a dict
ed_fi_admin_api_application_access_v1_application_access_response_from_dict = EdFiAdminApiApplicationAccessV1ApplicationAccessResponse.from_dict(ed_fi_admin_api_application_access_v1_application_access_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


