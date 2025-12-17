# ValidationsApiValidationResultsV1ValidationResultDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**collection_id** | **str** |  | [optional] 
**container_id** | **str** |  | [optional] 
**rule_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**job_execution_id** | **str** |  | [optional] 
**response** | **str** |  | [optional] 
**result** | **int** |  | [optional] 
**evaluation** | **bool** |  | [optional] 
**status_id** | **int** |  | [optional] 
**execution_date** | **str** |  | [optional] 
**execution_time_ms** | **int** |  | [optional] 
**executed_sql** | **str** |  | [optional] 
**diagnostic_sql** | **str** |  | [optional] 
**rule_details_destination_id** | **int** |  | [optional] 
**details_schema** | **str** |  | [optional] 
**details_table_name** | **str** |  | [optional] 
**last_execution_id** | **str** |  | [optional] 
**last_execution_total_results** | **int** |  | [optional] 
**last_execution_total_invalid_results** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_validation_results_v1_validation_result_dto import ValidationsApiValidationResultsV1ValidationResultDto

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiValidationResultsV1ValidationResultDto from a JSON string
validations_api_validation_results_v1_validation_result_dto_instance = ValidationsApiValidationResultsV1ValidationResultDto.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiValidationResultsV1ValidationResultDto.to_json())

# convert the object into a dict
validations_api_validation_results_v1_validation_result_dto_dict = validations_api_validation_results_v1_validation_result_dto_instance.to_dict()
# create an instance of ValidationsApiValidationResultsV1ValidationResultDto from a dict
validations_api_validation_results_v1_validation_result_dto_from_dict = ValidationsApiValidationResultsV1ValidationResultDto.from_dict(validations_api_validation_results_v1_validation_result_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


