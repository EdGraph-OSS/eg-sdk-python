# IdentityApiInstructionalInsightsV1RetryPolicyMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**backoff_multiplier** | **float** |  | [optional] 
**initial_delay** | **str** |  | [optional] 
**max_attempts** | **int** |  | [optional] 
**max_backoff** | **str** |  | [optional] 
**timeout** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_instructional_insights_v1_retry_policy_message import IdentityApiInstructionalInsightsV1RetryPolicyMessage

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiInstructionalInsightsV1RetryPolicyMessage from a JSON string
identity_api_instructional_insights_v1_retry_policy_message_instance = IdentityApiInstructionalInsightsV1RetryPolicyMessage.from_json(json)
# print the JSON string representation of the object
print(IdentityApiInstructionalInsightsV1RetryPolicyMessage.to_json())

# convert the object into a dict
identity_api_instructional_insights_v1_retry_policy_message_dict = identity_api_instructional_insights_v1_retry_policy_message_instance.to_dict()
# create an instance of IdentityApiInstructionalInsightsV1RetryPolicyMessage from a dict
identity_api_instructional_insights_v1_retry_policy_message_from_dict = IdentityApiInstructionalInsightsV1RetryPolicyMessage.from_dict(identity_api_instructional_insights_v1_retry_policy_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


