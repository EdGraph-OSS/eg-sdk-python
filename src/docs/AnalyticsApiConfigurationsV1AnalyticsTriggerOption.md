# AnalyticsApiConfigurationsV1AnalyticsTriggerOption


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**start_time** | **str** |  | [optional] 
**end_time** | **str** |  | [optional] 
**recurrence** | **str** |  | [optional] 
**time_zone** | **str** |  | [optional] 
**interval** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.analytics_api_configurations_v1_analytics_trigger_option import AnalyticsApiConfigurationsV1AnalyticsTriggerOption

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiConfigurationsV1AnalyticsTriggerOption from a JSON string
analytics_api_configurations_v1_analytics_trigger_option_instance = AnalyticsApiConfigurationsV1AnalyticsTriggerOption.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiConfigurationsV1AnalyticsTriggerOption.to_json())

# convert the object into a dict
analytics_api_configurations_v1_analytics_trigger_option_dict = analytics_api_configurations_v1_analytics_trigger_option_instance.to_dict()
# create an instance of AnalyticsApiConfigurationsV1AnalyticsTriggerOption from a dict
analytics_api_configurations_v1_analytics_trigger_option_from_dict = AnalyticsApiConfigurationsV1AnalyticsTriggerOption.from_dict(analytics_api_configurations_v1_analytics_trigger_option_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


