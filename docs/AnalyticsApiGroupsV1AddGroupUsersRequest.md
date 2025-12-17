# AnalyticsApiGroupsV1AddGroupUsersRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**group_id** | **str** |  | [optional] 
**users** | [**List[AnalyticsApiGroupsV1AnalyticsGroupUser]**](AnalyticsApiGroupsV1AnalyticsGroupUser.md) |  | [optional] [readonly] 
**add_global_tenant_users** | **bool** |  | [optional] 
**tenant_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.analytics_api_groups_v1_add_group_users_request import AnalyticsApiGroupsV1AddGroupUsersRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiGroupsV1AddGroupUsersRequest from a JSON string
analytics_api_groups_v1_add_group_users_request_instance = AnalyticsApiGroupsV1AddGroupUsersRequest.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiGroupsV1AddGroupUsersRequest.to_json())

# convert the object into a dict
analytics_api_groups_v1_add_group_users_request_dict = analytics_api_groups_v1_add_group_users_request_instance.to_dict()
# create an instance of AnalyticsApiGroupsV1AddGroupUsersRequest from a dict
analytics_api_groups_v1_add_group_users_request_from_dict = AnalyticsApiGroupsV1AddGroupUsersRequest.from_dict(analytics_api_groups_v1_add_group_users_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


