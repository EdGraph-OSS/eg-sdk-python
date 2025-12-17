# AnalyticsApiGroupsV1AnalyticsGroupUser


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**display_name** | **str** |  | [optional] 
**email_address** | **str** |  | [optional] 
**group_user_access_right** | **str** |  | [optional] 
**identifier** | **str** |  | [optional] 
**principal_type** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.analytics_api_groups_v1_analytics_group_user import AnalyticsApiGroupsV1AnalyticsGroupUser

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiGroupsV1AnalyticsGroupUser from a JSON string
analytics_api_groups_v1_analytics_group_user_instance = AnalyticsApiGroupsV1AnalyticsGroupUser.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiGroupsV1AnalyticsGroupUser.to_json())

# convert the object into a dict
analytics_api_groups_v1_analytics_group_user_dict = analytics_api_groups_v1_analytics_group_user_instance.to_dict()
# create an instance of AnalyticsApiGroupsV1AnalyticsGroupUser from a dict
analytics_api_groups_v1_analytics_group_user_from_dict = AnalyticsApiGroupsV1AnalyticsGroupUser.from_dict(analytics_api_groups_v1_analytics_group_user_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


