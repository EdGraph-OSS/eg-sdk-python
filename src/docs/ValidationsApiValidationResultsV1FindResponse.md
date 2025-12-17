# ValidationsApiValidationResultsV1FindResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[ValidationsApiValidationResultsV1ValidationResultDto]**](ValidationsApiValidationResultsV1ValidationResultDto.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_validation_results_v1_find_response import ValidationsApiValidationResultsV1FindResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiValidationResultsV1FindResponse from a JSON string
validations_api_validation_results_v1_find_response_instance = ValidationsApiValidationResultsV1FindResponse.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiValidationResultsV1FindResponse.to_json())

# convert the object into a dict
validations_api_validation_results_v1_find_response_dict = validations_api_validation_results_v1_find_response_instance.to_dict()
# create an instance of ValidationsApiValidationResultsV1FindResponse from a dict
validations_api_validation_results_v1_find_response_from_dict = ValidationsApiValidationResultsV1FindResponse.from_dict(validations_api_validation_results_v1_find_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


