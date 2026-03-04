# FormApiFormsV1CreateFullFormRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**source** | [**FormApiFormsV1FormSource**](FormApiFormsV1FormSource.md) |  | [optional] 
**version** | **str** |  | [optional] 
**anonymous** | **bool** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**status** | [**FormApiFormsV1FormStatus**](FormApiFormsV1FormStatus.md) |  | [optional] 
**sections** | [**List[FormApiFormsV1CreateFullSectionRequest]**](FormApiFormsV1CreateFullSectionRequest.md) |  | [optional] [readonly] 
**image** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_forms_v1_create_full_form_request import FormApiFormsV1CreateFullFormRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiFormsV1CreateFullFormRequest from a JSON string
form_api_forms_v1_create_full_form_request_instance = FormApiFormsV1CreateFullFormRequest.from_json(json)
# print the JSON string representation of the object
print(FormApiFormsV1CreateFullFormRequest.to_json())

# convert the object into a dict
form_api_forms_v1_create_full_form_request_dict = form_api_forms_v1_create_full_form_request_instance.to_dict()
# create an instance of FormApiFormsV1CreateFullFormRequest from a dict
form_api_forms_v1_create_full_form_request_from_dict = FormApiFormsV1CreateFullFormRequest.from_dict(form_api_forms_v1_create_full_form_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


