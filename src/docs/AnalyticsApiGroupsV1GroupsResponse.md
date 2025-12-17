# AnalyticsApiGroupsV1GroupsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**groups** | [**List[AnalyticsApiGroupsV1GroupResponse]**](AnalyticsApiGroupsV1GroupResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.analytics_api_groups_v1_groups_response import AnalyticsApiGroupsV1GroupsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiGroupsV1GroupsResponse from a JSON string
analytics_api_groups_v1_groups_response_instance = AnalyticsApiGroupsV1GroupsResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiGroupsV1GroupsResponse.to_json())

# convert the object into a dict
analytics_api_groups_v1_groups_response_dict = analytics_api_groups_v1_groups_response_instance.to_dict()
# create an instance of AnalyticsApiGroupsV1GroupsResponse from a dict
analytics_api_groups_v1_groups_response_from_dict = AnalyticsApiGroupsV1GroupsResponse.from_dict(analytics_api_groups_v1_groups_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


