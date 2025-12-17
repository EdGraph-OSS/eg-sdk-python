# ValidationsApiResultsV1RuleSummary


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**rule_id** | **str** |  | [optional] 
**rule_identification** | **str** |  | [optional] 
**severity_level** | **str** |  | [optional] 
**total_count** | **int** |  | [optional] 
**exception_count** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_results_v1_rule_summary import ValidationsApiResultsV1RuleSummary

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiResultsV1RuleSummary from a JSON string
validations_api_results_v1_rule_summary_instance = ValidationsApiResultsV1RuleSummary.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiResultsV1RuleSummary.to_json())

# convert the object into a dict
validations_api_results_v1_rule_summary_dict = validations_api_results_v1_rule_summary_instance.to_dict()
# create an instance of ValidationsApiResultsV1RuleSummary from a dict
validations_api_results_v1_rule_summary_from_dict = ValidationsApiResultsV1RuleSummary.from_dict(validations_api_results_v1_rule_summary_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


