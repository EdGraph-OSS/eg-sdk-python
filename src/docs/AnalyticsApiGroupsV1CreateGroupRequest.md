# AnalyticsApiGroupsV1CreateGroupRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**group_name** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.analytics_api_groups_v1_create_group_request import AnalyticsApiGroupsV1CreateGroupRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiGroupsV1CreateGroupRequest from a JSON string
analytics_api_groups_v1_create_group_request_instance = AnalyticsApiGroupsV1CreateGroupRequest.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiGroupsV1CreateGroupRequest.to_json())

# convert the object into a dict
analytics_api_groups_v1_create_group_request_dict = analytics_api_groups_v1_create_group_request_instance.to_dict()
# create an instance of AnalyticsApiGroupsV1CreateGroupRequest from a dict
analytics_api_groups_v1_create_group_request_from_dict = AnalyticsApiGroupsV1CreateGroupRequest.from_dict(analytics_api_groups_v1_create_group_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


