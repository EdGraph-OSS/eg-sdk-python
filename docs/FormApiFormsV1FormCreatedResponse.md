# FormApiFormsV1FormCreatedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_forms_v1_form_created_response import FormApiFormsV1FormCreatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiFormsV1FormCreatedResponse from a JSON string
form_api_forms_v1_form_created_response_instance = FormApiFormsV1FormCreatedResponse.from_json(json)
# print the JSON string representation of the object
print(FormApiFormsV1FormCreatedResponse.to_json())

# convert the object into a dict
form_api_forms_v1_form_created_response_dict = form_api_forms_v1_form_created_response_instance.to_dict()
# create an instance of FormApiFormsV1FormCreatedResponse from a dict
form_api_forms_v1_form_created_response_from_dict = FormApiFormsV1FormCreatedResponse.from_dict(form_api_forms_v1_form_created_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


