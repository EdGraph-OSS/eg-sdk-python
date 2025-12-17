# EdGraphServicesStateReportingV1ReportingPeriodCertificationStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**reporting_period** | [**EdGraphServicesStateReportingV1ReportingPeriodListResponse**](EdGraphServicesStateReportingV1ReportingPeriodListResponse.md) |  | [optional] 
**certification_percentage** | **float** |  | [optional] 
**categories** | [**List[EdGraphServicesStateReportingV1ReportingPeriodCertificationStatusCategory]**](EdGraphServicesStateReportingV1ReportingPeriodCertificationStatusCategory.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_certification_status import EdGraphServicesStateReportingV1ReportingPeriodCertificationStatus

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodCertificationStatus from a JSON string
ed_graph_services_state_reporting_v1_reporting_period_certification_status_instance = EdGraphServicesStateReportingV1ReportingPeriodCertificationStatus.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1ReportingPeriodCertificationStatus.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_reporting_period_certification_status_dict = ed_graph_services_state_reporting_v1_reporting_period_certification_status_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodCertificationStatus from a dict
ed_graph_services_state_reporting_v1_reporting_period_certification_status_from_dict = EdGraphServicesStateReportingV1ReportingPeriodCertificationStatus.from_dict(ed_graph_services_state_reporting_v1_reporting_period_certification_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


