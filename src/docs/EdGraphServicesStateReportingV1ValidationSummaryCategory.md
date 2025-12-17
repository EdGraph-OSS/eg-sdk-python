# EdGraphServicesStateReportingV1ValidationSummaryCategory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**category** | [**EdGraphServicesStateReportingV1Category**](EdGraphServicesStateReportingV1Category.md) |  | [optional] 
**sub_categories** | [**List[EdGraphServicesStateReportingV1ValidationSummarySubCategory]**](EdGraphServicesStateReportingV1ValidationSummarySubCategory.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_validation_summary_category import EdGraphServicesStateReportingV1ValidationSummaryCategory

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1ValidationSummaryCategory from a JSON string
ed_graph_services_state_reporting_v1_validation_summary_category_instance = EdGraphServicesStateReportingV1ValidationSummaryCategory.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1ValidationSummaryCategory.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_validation_summary_category_dict = ed_graph_services_state_reporting_v1_validation_summary_category_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1ValidationSummaryCategory from a dict
ed_graph_services_state_reporting_v1_validation_summary_category_from_dict = EdGraphServicesStateReportingV1ValidationSummaryCategory.from_dict(ed_graph_services_state_reporting_v1_validation_summary_category_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


