# FormApiFormsV1UpdateFullSectionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**questions** | [**List[FormApiFormsV1UpdateFullQuestionRequest]**](FormApiFormsV1UpdateFullQuestionRequest.md) |  | [optional] [readonly] 
**order** | **int** |  | [optional] 
**sub_heading** | **str** |  | [optional] 
**custom_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_forms_v1_update_full_section_request import FormApiFormsV1UpdateFullSectionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiFormsV1UpdateFullSectionRequest from a JSON string
form_api_forms_v1_update_full_section_request_instance = FormApiFormsV1UpdateFullSectionRequest.from_json(json)
# print the JSON string representation of the object
print(FormApiFormsV1UpdateFullSectionRequest.to_json())

# convert the object into a dict
form_api_forms_v1_update_full_section_request_dict = form_api_forms_v1_update_full_section_request_instance.to_dict()
# create an instance of FormApiFormsV1UpdateFullSectionRequest from a dict
form_api_forms_v1_update_full_section_request_from_dict = FormApiFormsV1UpdateFullSectionRequest.from_dict(form_api_forms_v1_update_full_section_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


