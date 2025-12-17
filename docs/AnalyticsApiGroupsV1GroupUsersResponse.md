# AnalyticsApiGroupsV1GroupUsersResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**group_users** | [**List[AnalyticsApiGroupsV1AnalyticsGroupUser]**](AnalyticsApiGroupsV1AnalyticsGroupUser.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.analytics_api_groups_v1_group_users_response import AnalyticsApiGroupsV1GroupUsersResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiGroupsV1GroupUsersResponse from a JSON string
analytics_api_groups_v1_group_users_response_instance = AnalyticsApiGroupsV1GroupUsersResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiGroupsV1GroupUsersResponse.to_json())

# convert the object into a dict
analytics_api_groups_v1_group_users_response_dict = analytics_api_groups_v1_group_users_response_instance.to_dict()
# create an instance of AnalyticsApiGroupsV1GroupUsersResponse from a dict
analytics_api_groups_v1_group_users_response_from_dict = AnalyticsApiGroupsV1GroupUsersResponse.from_dict(analytics_api_groups_v1_group_users_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


