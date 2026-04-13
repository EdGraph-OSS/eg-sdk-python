# IdentityApiInstructionalInsightsV1JobExecutionMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**execution_id** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**queue_date_time** | **str** |  | [optional] 
**start_date_time** | **str** |  | [optional] 
**end_date_time** | **str** |  | [optional] 
**input** | **str** |  | [optional] 
**output** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_instructional_insights_v1_job_execution_message import IdentityApiInstructionalInsightsV1JobExecutionMessage

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiInstructionalInsightsV1JobExecutionMessage from a JSON string
identity_api_instructional_insights_v1_job_execution_message_instance = IdentityApiInstructionalInsightsV1JobExecutionMessage.from_json(json)
# print the JSON string representation of the object
print(IdentityApiInstructionalInsightsV1JobExecutionMessage.to_json())

# convert the object into a dict
identity_api_instructional_insights_v1_job_execution_message_dict = identity_api_instructional_insights_v1_job_execution_message_instance.to_dict()
# create an instance of IdentityApiInstructionalInsightsV1JobExecutionMessage from a dict
identity_api_instructional_insights_v1_job_execution_message_from_dict = IdentityApiInstructionalInsightsV1JobExecutionMessage.from_dict(identity_api_instructional_insights_v1_job_execution_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


