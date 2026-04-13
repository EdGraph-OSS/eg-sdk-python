# IdentityApiInstructionalInsightsV1UpdateInstructionalInsightsSecuritySyncJobRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**job_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**input** | [**IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobInputMessage**](IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobInputMessage.md) |  | [optional] 
**schedule** | [**IdentityApiInstructionalInsightsV1ScheduleMessage**](IdentityApiInstructionalInsightsV1ScheduleMessage.md) |  | [optional] 
**retry_policy** | [**IdentityApiInstructionalInsightsV1RetryPolicyMessage**](IdentityApiInstructionalInsightsV1RetryPolicyMessage.md) |  | [optional] 
**callback_notifications** | [**List[IdentityApiInstructionalInsightsV1CallbackNotificationMessage]**](IdentityApiInstructionalInsightsV1CallbackNotificationMessage.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.identity_api_instructional_insights_v1_update_instructional_insights_security_sync_job_request import IdentityApiInstructionalInsightsV1UpdateInstructionalInsightsSecuritySyncJobRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiInstructionalInsightsV1UpdateInstructionalInsightsSecuritySyncJobRequest from a JSON string
identity_api_instructional_insights_v1_update_instructional_insights_security_sync_job_request_instance = IdentityApiInstructionalInsightsV1UpdateInstructionalInsightsSecuritySyncJobRequest.from_json(json)
# print the JSON string representation of the object
print(IdentityApiInstructionalInsightsV1UpdateInstructionalInsightsSecuritySyncJobRequest.to_json())

# convert the object into a dict
identity_api_instructional_insights_v1_update_instructional_insights_security_sync_job_request_dict = identity_api_instructional_insights_v1_update_instructional_insights_security_sync_job_request_instance.to_dict()
# create an instance of IdentityApiInstructionalInsightsV1UpdateInstructionalInsightsSecuritySyncJobRequest from a dict
identity_api_instructional_insights_v1_update_instructional_insights_security_sync_job_request_from_dict = IdentityApiInstructionalInsightsV1UpdateInstructionalInsightsSecuritySyncJobRequest.from_dict(identity_api_instructional_insights_v1_update_instructional_insights_security_sync_job_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


