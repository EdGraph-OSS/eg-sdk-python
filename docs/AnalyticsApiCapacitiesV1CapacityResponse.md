# AnalyticsApiCapacitiesV1CapacityResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**capacities** | [**List[AnalyticsApiCapacitiesV1AnalyticsCapacity]**](AnalyticsApiCapacitiesV1AnalyticsCapacity.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.analytics_api_capacities_v1_capacity_response import AnalyticsApiCapacitiesV1CapacityResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiCapacitiesV1CapacityResponse from a JSON string
analytics_api_capacities_v1_capacity_response_instance = AnalyticsApiCapacitiesV1CapacityResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiCapacitiesV1CapacityResponse.to_json())

# convert the object into a dict
analytics_api_capacities_v1_capacity_response_dict = analytics_api_capacities_v1_capacity_response_instance.to_dict()
# create an instance of AnalyticsApiCapacitiesV1CapacityResponse from a dict
analytics_api_capacities_v1_capacity_response_from_dict = AnalyticsApiCapacitiesV1CapacityResponse.from_dict(analytics_api_capacities_v1_capacity_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


