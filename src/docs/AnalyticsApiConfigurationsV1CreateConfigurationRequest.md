# AnalyticsApiConfigurationsV1CreateConfigurationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**sql_connection_string** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**use_ed_graph_power_bi** | **bool** |  | [optional] 
**is_global_configuration** | **bool** |  | [optional] 
**is_default_tenant_configuration** | **bool** |  | [optional] 
**azure_ad** | [**AnalyticsApiConfigurationsV1AnalyticsAzureAd**](AnalyticsApiConfigurationsV1AnalyticsAzureAd.md) |  | [optional] 
**power_bi** | [**AnalyticsApiConfigurationsV1AnalyticsPowerBi**](AnalyticsApiConfigurationsV1AnalyticsPowerBi.md) |  | [optional] 
**selected_ed_fi_connection_id** | **str** |  | [optional] 
**trigger_options** | [**List[AnalyticsApiConfigurationsV1AnalyticsTriggerOption]**](AnalyticsApiConfigurationsV1AnalyticsTriggerOption.md) |  | [optional] [readonly] 
**school_years** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.analytics_api_configurations_v1_create_configuration_request import AnalyticsApiConfigurationsV1CreateConfigurationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiConfigurationsV1CreateConfigurationRequest from a JSON string
analytics_api_configurations_v1_create_configuration_request_instance = AnalyticsApiConfigurationsV1CreateConfigurationRequest.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiConfigurationsV1CreateConfigurationRequest.to_json())

# convert the object into a dict
analytics_api_configurations_v1_create_configuration_request_dict = analytics_api_configurations_v1_create_configuration_request_instance.to_dict()
# create an instance of AnalyticsApiConfigurationsV1CreateConfigurationRequest from a dict
analytics_api_configurations_v1_create_configuration_request_from_dict = AnalyticsApiConfigurationsV1CreateConfigurationRequest.from_dict(analytics_api_configurations_v1_create_configuration_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


