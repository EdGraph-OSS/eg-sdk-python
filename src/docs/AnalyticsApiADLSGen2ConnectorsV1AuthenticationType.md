# AnalyticsApiADLSGen2ConnectorsV1AuthenticationType


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**service_principal_authentication** | [**AnalyticsApiADLSGen2ConnectorsV1ServicePrincipalAuthentication**](AnalyticsApiADLSGen2ConnectorsV1ServicePrincipalAuthentication.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.analytics_api_adls_gen2_connectors_v1_authentication_type import AnalyticsApiADLSGen2ConnectorsV1AuthenticationType

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiADLSGen2ConnectorsV1AuthenticationType from a JSON string
analytics_api_adls_gen2_connectors_v1_authentication_type_instance = AnalyticsApiADLSGen2ConnectorsV1AuthenticationType.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiADLSGen2ConnectorsV1AuthenticationType.to_json())

# convert the object into a dict
analytics_api_adls_gen2_connectors_v1_authentication_type_dict = analytics_api_adls_gen2_connectors_v1_authentication_type_instance.to_dict()
# create an instance of AnalyticsApiADLSGen2ConnectorsV1AuthenticationType from a dict
analytics_api_adls_gen2_connectors_v1_authentication_type_from_dict = AnalyticsApiADLSGen2ConnectorsV1AuthenticationType.from_dict(analytics_api_adls_gen2_connectors_v1_authentication_type_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


