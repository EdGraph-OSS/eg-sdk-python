# EdGraphServicesStateReportingV1PaginatedSubmissions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[EdGraphServicesStateReportingV1SubmissionListResponse]**](EdGraphServicesStateReportingV1SubmissionListResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_paginated_submissions import EdGraphServicesStateReportingV1PaginatedSubmissions

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1PaginatedSubmissions from a JSON string
ed_graph_services_state_reporting_v1_paginated_submissions_instance = EdGraphServicesStateReportingV1PaginatedSubmissions.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1PaginatedSubmissions.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_paginated_submissions_dict = ed_graph_services_state_reporting_v1_paginated_submissions_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1PaginatedSubmissions from a dict
ed_graph_services_state_reporting_v1_paginated_submissions_from_dict = EdGraphServicesStateReportingV1PaginatedSubmissions.from_dict(ed_graph_services_state_reporting_v1_paginated_submissions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


