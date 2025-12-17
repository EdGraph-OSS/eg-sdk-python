# ValidationsApiRulesV1RuleDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** | Details | [optional] 
**container_id** | **str** |  | [optional] 
**id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**diagnostic_sql** | **str** | SQL | [optional] 
**count_sql** | **str** |  | [optional] 
**error_severity_level** | **int** |  | [optional] 
**error_message** | **str** |  | [optional] 
**max_number_results** | **int** |  | [optional] 
**rule_identification** | **str** | Metadata | [optional] 
**resolution** | **str** |  | [optional] 
**tags** | **List[str]** |  | [optional] [readonly] 
**version** | **str** |  | [optional] 
**parent_collection** | [**ValidationsApiContainersV1ContainerDto**](ValidationsApiContainersV1ContainerDto.md) |  | [optional] 
**parent_container** | [**ValidationsApiContainersV1ContainerDto**](ValidationsApiContainersV1ContainerDto.md) |  | [optional] 
**last_execution_id** | **str** |  | [optional] 
**last_execution_start_date_time** | **str** |  | [optional] 
**last_execution_end_date_time** | **str** |  | [optional] 
**last_execution_total_results** | **int** |  | [optional] 
**last_execution_total_invalid_results** | **int** |  | [optional] 
**collection_id** | **str** |  | [optional] 
**urls** | [**List[ValidationsApiRulesV1Url]**](ValidationsApiRulesV1Url.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_rules_v1_rule_dto import ValidationsApiRulesV1RuleDto

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiRulesV1RuleDto from a JSON string
validations_api_rules_v1_rule_dto_instance = ValidationsApiRulesV1RuleDto.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiRulesV1RuleDto.to_json())

# convert the object into a dict
validations_api_rules_v1_rule_dto_dict = validations_api_rules_v1_rule_dto_instance.to_dict()
# create an instance of ValidationsApiRulesV1RuleDto from a dict
validations_api_rules_v1_rule_dto_from_dict = ValidationsApiRulesV1RuleDto.from_dict(validations_api_rules_v1_rule_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


