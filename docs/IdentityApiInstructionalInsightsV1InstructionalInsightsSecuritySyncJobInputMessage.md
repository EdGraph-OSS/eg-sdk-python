# IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobInputMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant** | **str** |  | [optional] 
**page_size** | **int** |  | [optional] 
**order_by** | **str** |  | [optional] 
**filter** | **str** |  | [optional] 
**load_batch_size** | **int** |  | [optional] 
**load_batch_throttle** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_instructional_insights_v1_instructional_insights_security_sync_job_input_message import IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobInputMessage

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobInputMessage from a JSON string
identity_api_instructional_insights_v1_instructional_insights_security_sync_job_input_message_instance = IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobInputMessage.from_json(json)
# print the JSON string representation of the object
print(IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobInputMessage.to_json())

# convert the object into a dict
identity_api_instructional_insights_v1_instructional_insights_security_sync_job_input_message_dict = identity_api_instructional_insights_v1_instructional_insights_security_sync_job_input_message_instance.to_dict()
# create an instance of IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobInputMessage from a dict
identity_api_instructional_insights_v1_instructional_insights_security_sync_job_input_message_from_dict = IdentityApiInstructionalInsightsV1InstructionalInsightsSecuritySyncJobInputMessage.from_dict(identity_api_instructional_insights_v1_instructional_insights_security_sync_job_input_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


