# IdentityApiInstructionalInsightsV1ScheduleMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** |  | [optional] 
**begin_date** | **str** |  | [optional] 
**end_date** | **str** |  | [optional] 
**cron_expression** | **str** |  | [optional] 
**time_zone** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_instructional_insights_v1_schedule_message import IdentityApiInstructionalInsightsV1ScheduleMessage

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiInstructionalInsightsV1ScheduleMessage from a JSON string
identity_api_instructional_insights_v1_schedule_message_instance = IdentityApiInstructionalInsightsV1ScheduleMessage.from_json(json)
# print the JSON string representation of the object
print(IdentityApiInstructionalInsightsV1ScheduleMessage.to_json())

# convert the object into a dict
identity_api_instructional_insights_v1_schedule_message_dict = identity_api_instructional_insights_v1_schedule_message_instance.to_dict()
# create an instance of IdentityApiInstructionalInsightsV1ScheduleMessage from a dict
identity_api_instructional_insights_v1_schedule_message_from_dict = IdentityApiInstructionalInsightsV1ScheduleMessage.from_dict(identity_api_instructional_insights_v1_schedule_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


