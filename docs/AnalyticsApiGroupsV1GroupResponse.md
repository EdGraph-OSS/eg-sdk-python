# AnalyticsApiGroupsV1GroupResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**group_id** | **str** |  | [optional] 
**group_name** | **str** |  | [optional] 
**capacity_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.analytics_api_groups_v1_group_response import AnalyticsApiGroupsV1GroupResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiGroupsV1GroupResponse from a JSON string
analytics_api_groups_v1_group_response_instance = AnalyticsApiGroupsV1GroupResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiGroupsV1GroupResponse.to_json())

# convert the object into a dict
analytics_api_groups_v1_group_response_dict = analytics_api_groups_v1_group_response_instance.to_dict()
# create an instance of AnalyticsApiGroupsV1GroupResponse from a dict
analytics_api_groups_v1_group_response_from_dict = AnalyticsApiGroupsV1GroupResponse.from_dict(analytics_api_groups_v1_group_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


