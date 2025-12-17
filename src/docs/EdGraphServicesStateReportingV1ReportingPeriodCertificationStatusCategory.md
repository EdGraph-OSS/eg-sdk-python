# EdGraphServicesStateReportingV1ReportingPeriodCertificationStatusCategory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**category** | [**EdGraphServicesStateReportingV1Category**](EdGraphServicesStateReportingV1Category.md) |  | [optional] 
**record_count** | **int** |  | [optional] 
**fatal_count** | **int** |  | [optional] 
**warning_count** | **int** |  | [optional] 
**excluded_count** | **int** |  | [optional] 
**status** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_certification_status_category import EdGraphServicesStateReportingV1ReportingPeriodCertificationStatusCategory

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodCertificationStatusCategory from a JSON string
ed_graph_services_state_reporting_v1_reporting_period_certification_status_category_instance = EdGraphServicesStateReportingV1ReportingPeriodCertificationStatusCategory.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1ReportingPeriodCertificationStatusCategory.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_reporting_period_certification_status_category_dict = ed_graph_services_state_reporting_v1_reporting_period_certification_status_category_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodCertificationStatusCategory from a dict
ed_graph_services_state_reporting_v1_reporting_period_certification_status_category_from_dict = EdGraphServicesStateReportingV1ReportingPeriodCertificationStatusCategory.from_dict(ed_graph_services_state_reporting_v1_reporting_period_certification_status_category_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


