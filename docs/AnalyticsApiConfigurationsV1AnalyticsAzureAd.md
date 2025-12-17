# AnalyticsApiConfigurationsV1AnalyticsAzureAd


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**client_id** | **str** |  | [optional] 
**azure_tenant_id** | **str** |  | [optional] 
**client_secret** | **str** |  | [optional] 
**scopes** | **List[str]** |  | [optional] [readonly] 
**tenant_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.analytics_api_configurations_v1_analytics_azure_ad import AnalyticsApiConfigurationsV1AnalyticsAzureAd

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiConfigurationsV1AnalyticsAzureAd from a JSON string
analytics_api_configurations_v1_analytics_azure_ad_instance = AnalyticsApiConfigurationsV1AnalyticsAzureAd.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiConfigurationsV1AnalyticsAzureAd.to_json())

# convert the object into a dict
analytics_api_configurations_v1_analytics_azure_ad_dict = analytics_api_configurations_v1_analytics_azure_ad_instance.to_dict()
# create an instance of AnalyticsApiConfigurationsV1AnalyticsAzureAd from a dict
analytics_api_configurations_v1_analytics_azure_ad_from_dict = AnalyticsApiConfigurationsV1AnalyticsAzureAd.from_dict(analytics_api_configurations_v1_analytics_azure_ad_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


