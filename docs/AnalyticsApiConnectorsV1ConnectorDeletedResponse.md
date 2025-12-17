# AnalyticsApiConnectorsV1ConnectorDeletedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**connector_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.analytics_api_connectors_v1_connector_deleted_response import AnalyticsApiConnectorsV1ConnectorDeletedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiConnectorsV1ConnectorDeletedResponse from a JSON string
analytics_api_connectors_v1_connector_deleted_response_instance = AnalyticsApiConnectorsV1ConnectorDeletedResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiConnectorsV1ConnectorDeletedResponse.to_json())

# convert the object into a dict
analytics_api_connectors_v1_connector_deleted_response_dict = analytics_api_connectors_v1_connector_deleted_response_instance.to_dict()
# create an instance of AnalyticsApiConnectorsV1ConnectorDeletedResponse from a dict
analytics_api_connectors_v1_connector_deleted_response_from_dict = AnalyticsApiConnectorsV1ConnectorDeletedResponse.from_dict(analytics_api_connectors_v1_connector_deleted_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


