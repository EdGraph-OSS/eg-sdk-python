# FormApiFormComponentsV1FormComponentResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**display_name** | **str** |  | [optional] 
**type** | [**FormApiFormComponentsV1FormComponentType**](FormApiFormComponentsV1FormComponentType.md) |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**deleted_by** | **str** |  | [optional] 
**deleted_date_time** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_form_components_v1_form_component_response import FormApiFormComponentsV1FormComponentResponse

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiFormComponentsV1FormComponentResponse from a JSON string
form_api_form_components_v1_form_component_response_instance = FormApiFormComponentsV1FormComponentResponse.from_json(json)
# print the JSON string representation of the object
print(FormApiFormComponentsV1FormComponentResponse.to_json())

# convert the object into a dict
form_api_form_components_v1_form_component_response_dict = form_api_form_components_v1_form_component_response_instance.to_dict()
# create an instance of FormApiFormComponentsV1FormComponentResponse from a dict
form_api_form_components_v1_form_component_response_from_dict = FormApiFormComponentsV1FormComponentResponse.from_dict(form_api_form_components_v1_form_component_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


