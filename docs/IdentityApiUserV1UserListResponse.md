# IdentityApiUserV1UserListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**user_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**tenant_count** | **int** |  | [optional] 
**tenants** | [**List[IdentityApiUserV1Tenant]**](IdentityApiUserV1Tenant.md) |  | [optional] [readonly] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**logins** | [**List[IdentityApiUserV1UserLogin]**](IdentityApiUserV1UserLogin.md) |  | [optional] [readonly] 
**source** | **str** |  | [optional] 
**last_login_date_time** | **str** |  | [optional] 
**mfa_completed** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_user_v1_user_list_response import IdentityApiUserV1UserListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiUserV1UserListResponse from a JSON string
identity_api_user_v1_user_list_response_instance = IdentityApiUserV1UserListResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiUserV1UserListResponse.to_json())

# convert the object into a dict
identity_api_user_v1_user_list_response_dict = identity_api_user_v1_user_list_response_instance.to_dict()
# create an instance of IdentityApiUserV1UserListResponse from a dict
identity_api_user_v1_user_list_response_from_dict = IdentityApiUserV1UserListResponse.from_dict(identity_api_user_v1_user_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


