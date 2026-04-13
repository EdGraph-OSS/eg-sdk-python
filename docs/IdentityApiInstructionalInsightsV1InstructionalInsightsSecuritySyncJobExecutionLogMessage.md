# IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutionLogMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**execution_id** | **str** |  | [optional] 
**logged_date_time** | **str** |  | [optional] 
**level** | **str** |  | [optional] 
**message** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_instructional_insights_v1_instructional_insights_security_sync_job_execution_log_message import IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutionLogMessage

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutionLogMessage from a JSON string
identity_api_instructional_insights_v1_instructional_insights_security_sync_job_execution_log_message_instance = IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutionLogMessage.from_json(json)
# print the JSON string representation of the object
print(IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutionLogMessage.to_json())

# convert the object into a dict
identity_api_instructional_insights_v1_instructional_insights_security_sync_job_execution_log_message_dict = identity_api_instructional_insights_v1_instructional_insights_security_sync_job_execution_log_message_instance.to_dict()
# create an instance of IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutionLogMessage from a dict
identity_api_instructional_insights_v1_instructional_insights_security_sync_job_execution_log_message_from_dict = IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobExecutionLogMessage.from_dict(identity_api_instructional_insights_v1_instructional_insights_security_sync_job_execution_log_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


