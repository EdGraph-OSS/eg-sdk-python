# EdGraphServicesStateReportingV1PaginatedSubmissionLogs


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[EdGraphServicesStateReportingV1SubmissionLog]**](EdGraphServicesStateReportingV1SubmissionLog.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_paginated_submission_logs import EdGraphServicesStateReportingV1PaginatedSubmissionLogs

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1PaginatedSubmissionLogs from a JSON string
ed_graph_services_state_reporting_v1_paginated_submission_logs_instance = EdGraphServicesStateReportingV1PaginatedSubmissionLogs.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1PaginatedSubmissionLogs.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_paginated_submission_logs_dict = ed_graph_services_state_reporting_v1_paginated_submission_logs_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1PaginatedSubmissionLogs from a dict
ed_graph_services_state_reporting_v1_paginated_submission_logs_from_dict = EdGraphServicesStateReportingV1PaginatedSubmissionLogs.from_dict(ed_graph_services_state_reporting_v1_paginated_submission_logs_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


