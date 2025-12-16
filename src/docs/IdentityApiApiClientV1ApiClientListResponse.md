# IdentityApiApiClientV1ApiClientListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**client_name** | **str** |  | [optional] 
**client_uri** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**expiration_date** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_api_client_v1_api_client_list_response import IdentityApiApiClientV1ApiClientListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiApiClientV1ApiClientListResponse from a JSON string
identity_api_api_client_v1_api_client_list_response_instance = IdentityApiApiClientV1ApiClientListResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiApiClientV1ApiClientListResponse.to_json())

# convert the object into a dict
identity_api_api_client_v1_api_client_list_response_dict = identity_api_api_client_v1_api_client_list_response_instance.to_dict()
# create an instance of IdentityApiApiClientV1ApiClientListResponse from a dict
identity_api_api_client_v1_api_client_list_response_from_dict = IdentityApiApiClientV1ApiClientListResponse.from_dict(identity_api_api_client_v1_api_client_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


