# IMSAdminApiV1ClientsClientListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**application_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**client_name** | **str** |  | [optional] 
**client_uri** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**selected_scope** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ims_admin_api_v1_clients_client_list_response import IMSAdminApiV1ClientsClientListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IMSAdminApiV1ClientsClientListResponse from a JSON string
ims_admin_api_v1_clients_client_list_response_instance = IMSAdminApiV1ClientsClientListResponse.from_json(json)
# print the JSON string representation of the object
print(IMSAdminApiV1ClientsClientListResponse.to_json())

# convert the object into a dict
ims_admin_api_v1_clients_client_list_response_dict = ims_admin_api_v1_clients_client_list_response_instance.to_dict()
# create an instance of IMSAdminApiV1ClientsClientListResponse from a dict
ims_admin_api_v1_clients_client_list_response_from_dict = IMSAdminApiV1ClientsClientListResponse.from_dict(ims_admin_api_v1_clients_client_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


