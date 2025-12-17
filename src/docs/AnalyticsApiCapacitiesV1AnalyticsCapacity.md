# AnalyticsApiCapacitiesV1AnalyticsCapacity


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**capacity_id** | **str** |  | [optional] 
**display_name** | **str** |  | [optional] 
**sku** | **str** |  | [optional] 
**state** | **str** |  | [optional] 
**region** | **str** |  | [optional] 
**capacity_user_access_right** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.analytics_api_capacities_v1_analytics_capacity import AnalyticsApiCapacitiesV1AnalyticsCapacity

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiCapacitiesV1AnalyticsCapacity from a JSON string
analytics_api_capacities_v1_analytics_capacity_instance = AnalyticsApiCapacitiesV1AnalyticsCapacity.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiCapacitiesV1AnalyticsCapacity.to_json())

# convert the object into a dict
analytics_api_capacities_v1_analytics_capacity_dict = analytics_api_capacities_v1_analytics_capacity_instance.to_dict()
# create an instance of AnalyticsApiCapacitiesV1AnalyticsCapacity from a dict
analytics_api_capacities_v1_analytics_capacity_from_dict = AnalyticsApiCapacitiesV1AnalyticsCapacity.from_dict(analytics_api_capacities_v1_analytics_capacity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


