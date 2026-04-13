# IdentityApiInstructionalInsightsV1CreateInstructionalInsightsSecuritySyncJobRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**input** | [**IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobInputMessage**](IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobInputMessage.md) |  | [optional] 
**schedule** | [**IdentityApiInstructionalInsightsV1ScheduleMessage**](IdentityApiInstructionalInsightsV1ScheduleMessage.md) |  | [optional] 
**retry_policy** | [**IdentityApiInstructionalInsightsV1RetryPolicyMessage**](IdentityApiInstructionalInsightsV1RetryPolicyMessage.md) |  | [optional] 
**callback_notifications** | [**List[IdentityApiInstructionalInsightsV1CallbackNotificationMessage]**](IdentityApiInstructionalInsightsV1CallbackNotificationMessage.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.identity_api_instructional_insights_v1_create_instructional_insights_security_sync_job_request import IdentityApiInstructionalInsightsV1CreateInstructionalInsightsSecuritySyncJobRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiInstructionalInsightsV1CreateInstructionalInsightsSecuritySyncJobRequest from a JSON string
identity_api_instructional_insights_v1_create_instructional_insights_security_sync_job_request_instance = IdentityApiInstructionalInsightsV1CreateInstructionalInsightsSecuritySyncJobRequest.from_json(json)
# print the JSON string representation of the object
print(IdentityApiInstructionalInsightsV1CreateInstructionalInsightsSecuritySyncJobRequest.to_json())

# convert the object into a dict
identity_api_instructional_insights_v1_create_instructional_insights_security_sync_job_request_dict = identity_api_instructional_insights_v1_create_instructional_insights_security_sync_job_request_instance.to_dict()
# create an instance of IdentityApiInstructionalInsightsV1CreateInstructionalInsightsSecuritySyncJobRequest from a dict
identity_api_instructional_insights_v1_create_instructional_insights_security_sync_job_request_from_dict = IdentityApiInstructionalInsightsV1CreateInstructionalInsightsSecuritySyncJobRequest.from_dict(identity_api_instructional_insights_v1_create_instructional_insights_security_sync_job_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


