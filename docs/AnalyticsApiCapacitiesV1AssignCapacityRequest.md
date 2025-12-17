# AnalyticsApiCapacitiesV1AssignCapacityRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**group_id** | **str** |  | [optional] 
**capacity_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.analytics_api_capacities_v1_assign_capacity_request import AnalyticsApiCapacitiesV1AssignCapacityRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiCapacitiesV1AssignCapacityRequest from a JSON string
analytics_api_capacities_v1_assign_capacity_request_instance = AnalyticsApiCapacitiesV1AssignCapacityRequest.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiCapacitiesV1AssignCapacityRequest.to_json())

# convert the object into a dict
analytics_api_capacities_v1_assign_capacity_request_dict = analytics_api_capacities_v1_assign_capacity_request_instance.to_dict()
# create an instance of AnalyticsApiCapacitiesV1AssignCapacityRequest from a dict
analytics_api_capacities_v1_assign_capacity_request_from_dict = AnalyticsApiCapacitiesV1AssignCapacityRequest.from_dict(analytics_api_capacities_v1_assign_capacity_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


