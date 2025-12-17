# AnalyticsApiCapacitiesV1SuspendCapacityRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**dedicated_capacity_name** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.analytics_api_capacities_v1_suspend_capacity_request import AnalyticsApiCapacitiesV1SuspendCapacityRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiCapacitiesV1SuspendCapacityRequest from a JSON string
analytics_api_capacities_v1_suspend_capacity_request_instance = AnalyticsApiCapacitiesV1SuspendCapacityRequest.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiCapacitiesV1SuspendCapacityRequest.to_json())

# convert the object into a dict
analytics_api_capacities_v1_suspend_capacity_request_dict = analytics_api_capacities_v1_suspend_capacity_request_instance.to_dict()
# create an instance of AnalyticsApiCapacitiesV1SuspendCapacityRequest from a dict
analytics_api_capacities_v1_suspend_capacity_request_from_dict = AnalyticsApiCapacitiesV1SuspendCapacityRequest.from_dict(analytics_api_capacities_v1_suspend_capacity_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


