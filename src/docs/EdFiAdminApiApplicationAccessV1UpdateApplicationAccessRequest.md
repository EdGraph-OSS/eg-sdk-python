# EdFiAdminApiApplicationAccessV1UpdateApplicationAccessRequest


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
from edgraph_platform_client.models.ed_fi_admin_api_application_access_v1_update_application_access_request import EdFiAdminApiApplicationAccessV1UpdateApplicationAccessRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdFiAdminApiApplicationAccessV1UpdateApplicationAccessRequest from a JSON string
ed_fi_admin_api_application_access_v1_update_application_access_request_instance = EdFiAdminApiApplicationAccessV1UpdateApplicationAccessRequest.from_json(json)
# print the JSON string representation of the object
print(EdFiAdminApiApplicationAccessV1UpdateApplicationAccessRequest.to_json())

# convert the object into a dict
ed_fi_admin_api_application_access_v1_update_application_access_request_dict = ed_fi_admin_api_application_access_v1_update_application_access_request_instance.to_dict()
# create an instance of EdFiAdminApiApplicationAccessV1UpdateApplicationAccessRequest from a dict
ed_fi_admin_api_application_access_v1_update_application_access_request_from_dict = EdFiAdminApiApplicationAccessV1UpdateApplicationAccessRequest.from_dict(ed_fi_admin_api_application_access_v1_update_application_access_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


