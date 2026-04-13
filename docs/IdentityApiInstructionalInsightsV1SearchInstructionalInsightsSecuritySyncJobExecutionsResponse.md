# IdentityApiInstructionalInsightsV1SearchInstructionalInsightsSecuritySyncJobExecutionsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutionMessage]**](IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutionMessage.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.identity_api_instructional_insights_v1_search_instructional_insights_security_sync_job_executions_response import IdentityApiInstructionalInsightsV1SearchInstructionalInsightsSecuritySyncJobExecutionsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiInstructionalInsightsV1SearchInstructionalInsightsSecuritySyncJobExecutionsResponse from a JSON string
identity_api_instructional_insights_v1_search_instructional_insights_security_sync_job_executions_response_instance = IdentityApiInstructionalInsightsV1SearchInstructionalInsightsSecuritySyncJobExecutionsResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiInstructionalInsightsV1SearchInstructionalInsightsSecuritySyncJobExecutionsResponse.to_json())

# convert the object into a dict
identity_api_instructional_insights_v1_search_instructional_insights_security_sync_job_executions_response_dict = identity_api_instructional_insights_v1_search_instructional_insights_security_sync_job_executions_response_instance.to_dict()
# create an instance of IdentityApiInstructionalInsightsV1SearchInstructionalInsightsSecuritySyncJobExecutionsResponse from a dict
identity_api_instructional_insights_v1_search_instructional_insights_security_sync_job_executions_response_from_dict = IdentityApiInstructionalInsightsV1SearchInstructionalInsightsSecuritySyncJobExecutionsResponse.from_dict(identity_api_instructional_insights_v1_search_instructional_insights_security_sync_job_executions_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


