# EdGraphCommonErrorsCoreProblemDetails


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 
**status** | **int** |  | [optional] 
**title** | **str** |  | [optional] 
**details** | **str** |  | [optional] 
**instance** | **str** |  | [optional] 
**extensions** | **Dict[str, Optional[object]]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ed_graph_common_errors_core_problem_details import EdGraphCommonErrorsCoreProblemDetails

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphCommonErrorsCoreProblemDetails from a JSON string
ed_graph_common_errors_core_problem_details_instance = EdGraphCommonErrorsCoreProblemDetails.from_json(json)
# print the JSON string representation of the object
print(EdGraphCommonErrorsCoreProblemDetails.to_json())

# convert the object into a dict
ed_graph_common_errors_core_problem_details_dict = ed_graph_common_errors_core_problem_details_instance.to_dict()
# create an instance of EdGraphCommonErrorsCoreProblemDetails from a dict
ed_graph_common_errors_core_problem_details_from_dict = EdGraphCommonErrorsCoreProblemDetails.from_dict(ed_graph_common_errors_core_problem_details_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


