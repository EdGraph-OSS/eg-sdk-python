# IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutionMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**execution_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**queued_date_time** | **str** |  | [optional] 
**start_date_time** | **str** |  | [optional] 
**cancel_date_time** | **str** |  | [optional] 
**end_date_time** | **str** |  | [optional] 
**input** | **str** |  | [optional] 
**output** | **str** |  | [optional] 
**metrics** | [**List[IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutionMetricMessage]**](IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutionMetricMessage.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.identity_api_instructional_insights_v1_instructional_insights_security_sync_job_execution_message import IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutionMessage

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutionMessage from a JSON string
identity_api_instructional_insights_v1_instructional_insights_security_sync_job_execution_message_instance = IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutionMessage.from_json(json)
# print the JSON string representation of the object
print(IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutionMessage.to_json())

# convert the object into a dict
identity_api_instructional_insights_v1_instructional_insights_security_sync_job_execution_message_dict = identity_api_instructional_insights_v1_instructional_insights_security_sync_job_execution_message_instance.to_dict()
# create an instance of IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutionMessage from a dict
identity_api_instructional_insights_v1_instructional_insights_security_sync_job_execution_message_from_dict = IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutionMessage.from_dict(identity_api_instructional_insights_v1_instructional_insights_security_sync_job_execution_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


