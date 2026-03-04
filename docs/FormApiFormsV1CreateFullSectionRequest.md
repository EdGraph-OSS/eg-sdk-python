# FormApiFormsV1CreateFullSectionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**questions** | [**List[FormApiFormsV1CreateFullQuestionRequest]**](FormApiFormsV1CreateFullQuestionRequest.md) |  | [optional] [readonly] 
**order** | **int** |  | [optional] 
**sub_heading** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_forms_v1_create_full_section_request import FormApiFormsV1CreateFullSectionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiFormsV1CreateFullSectionRequest from a JSON string
form_api_forms_v1_create_full_section_request_instance = FormApiFormsV1CreateFullSectionRequest.from_json(json)
# print the JSON string representation of the object
print(FormApiFormsV1CreateFullSectionRequest.to_json())

# convert the object into a dict
form_api_forms_v1_create_full_section_request_dict = form_api_forms_v1_create_full_section_request_instance.to_dict()
# create an instance of FormApiFormsV1CreateFullSectionRequest from a dict
form_api_forms_v1_create_full_section_request_from_dict = FormApiFormsV1CreateFullSectionRequest.from_dict(form_api_forms_v1_create_full_section_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


