# IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**job_type_id** | **str** |  | [optional] 
**job_type_name** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**input** | **str** |  | [optional] 
**active** | **bool** |  | [optional] 
**schedule** | [**IdentityApiInstructionalInsightsV1ScheduleMessage**](IdentityApiInstructionalInsightsV1ScheduleMessage.md) |  | [optional] 
**retry_policy** | [**IdentityApiInstructionalInsightsV1RetryPolicyMessage**](IdentityApiInstructionalInsightsV1RetryPolicyMessage.md) |  | [optional] 
**callback_notifications** | [**List[IdentityApiInstructionalInsightsV1CallbackNotificationMessage]**](IdentityApiInstructionalInsightsV1CallbackNotificationMessage.md) |  | [optional] [readonly] 
**last_execution** | [**IdentityApiInstructionalInsightsV1JobExecutionMessage**](IdentityApiInstructionalInsightsV1JobExecutionMessage.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_instructional_insights_v1_instructional_insights_security_sync_job_response import IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobResponse from a JSON string
identity_api_instructional_insights_v1_instructional_insights_security_sync_job_response_instance = IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobResponse.to_json())

# convert the object into a dict
identity_api_instructional_insights_v1_instructional_insights_security_sync_job_response_dict = identity_api_instructional_insights_v1_instructional_insights_security_sync_job_response_instance.to_dict()
# create an instance of IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobResponse from a dict
identity_api_instructional_insights_v1_instructional_insights_security_sync_job_response_from_dict = IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobResponse.from_dict(identity_api_instructional_insights_v1_instructional_insights_security_sync_job_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


