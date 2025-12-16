# MicrosoftAspNetCoreMvcValidationProblemDetails


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**errors** | **Dict[str, List[str]]** |  | [optional] 
**type** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**status** | **int** |  | [optional] 
**detail** | **str** |  | [optional] 
**instance** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.microsoft_asp_net_core_mvc_validation_problem_details import MicrosoftAspNetCoreMvcValidationProblemDetails

# TODO update the JSON string below
json = "{}"
# create an instance of MicrosoftAspNetCoreMvcValidationProblemDetails from a JSON string
microsoft_asp_net_core_mvc_validation_problem_details_instance = MicrosoftAspNetCoreMvcValidationProblemDetails.from_json(json)
# print the JSON string representation of the object
print(MicrosoftAspNetCoreMvcValidationProblemDetails.to_json())

# convert the object into a dict
microsoft_asp_net_core_mvc_validation_problem_details_dict = microsoft_asp_net_core_mvc_validation_problem_details_instance.to_dict()
# create an instance of MicrosoftAspNetCoreMvcValidationProblemDetails from a dict
microsoft_asp_net_core_mvc_validation_problem_details_from_dict = MicrosoftAspNetCoreMvcValidationProblemDetails.from_dict(microsoft_asp_net_core_mvc_validation_problem_details_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


