# AnalyticsApiConfigurationsV1AnalyticsConfigurationPaginatedItemsViewModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[AnalyticsApiConfigurationsV1AnalyticsConfiguration]**](AnalyticsApiConfigurationsV1AnalyticsConfiguration.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.analytics_api_configurations_v1_analytics_configuration_paginated_items_view_model import AnalyticsApiConfigurationsV1AnalyticsConfigurationPaginatedItemsViewModel

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiConfigurationsV1AnalyticsConfigurationPaginatedItemsViewModel from a JSON string
analytics_api_configurations_v1_analytics_configuration_paginated_items_view_model_instance = AnalyticsApiConfigurationsV1AnalyticsConfigurationPaginatedItemsViewModel.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiConfigurationsV1AnalyticsConfigurationPaginatedItemsViewModel.to_json())

# convert the object into a dict
analytics_api_configurations_v1_analytics_configuration_paginated_items_view_model_dict = analytics_api_configurations_v1_analytics_configuration_paginated_items_view_model_instance.to_dict()
# create an instance of AnalyticsApiConfigurationsV1AnalyticsConfigurationPaginatedItemsViewModel from a dict
analytics_api_configurations_v1_analytics_configuration_paginated_items_view_model_from_dict = AnalyticsApiConfigurationsV1AnalyticsConfigurationPaginatedItemsViewModel.from_dict(analytics_api_configurations_v1_analytics_configuration_paginated_items_view_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


