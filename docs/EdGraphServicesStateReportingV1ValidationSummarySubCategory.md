# EdGraphServicesStateReportingV1ValidationSummarySubCategory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sub_category** | [**EdGraphServicesStateReportingV1SubCategory**](EdGraphServicesStateReportingV1SubCategory.md) |  | [optional] 
**rules** | [**List[EdGraphServicesStateReportingV1Rule]**](EdGraphServicesStateReportingV1Rule.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_validation_summary_sub_category import EdGraphServicesStateReportingV1ValidationSummarySubCategory

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1ValidationSummarySubCategory from a JSON string
ed_graph_services_state_reporting_v1_validation_summary_sub_category_instance = EdGraphServicesStateReportingV1ValidationSummarySubCategory.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1ValidationSummarySubCategory.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_validation_summary_sub_category_dict = ed_graph_services_state_reporting_v1_validation_summary_sub_category_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1ValidationSummarySubCategory from a dict
ed_graph_services_state_reporting_v1_validation_summary_sub_category_from_dict = EdGraphServicesStateReportingV1ValidationSummarySubCategory.from_dict(ed_graph_services_state_reporting_v1_validation_summary_sub_category_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


