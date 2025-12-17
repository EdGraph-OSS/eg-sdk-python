# FormApiFormsV1FormDeletedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_forms_v1_form_deleted_response import FormApiFormsV1FormDeletedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiFormsV1FormDeletedResponse from a JSON string
form_api_forms_v1_form_deleted_response_instance = FormApiFormsV1FormDeletedResponse.from_json(json)
# print the JSON string representation of the object
print(FormApiFormsV1FormDeletedResponse.to_json())

# convert the object into a dict
form_api_forms_v1_form_deleted_response_dict = form_api_forms_v1_form_deleted_response_instance.to_dict()
# create an instance of FormApiFormsV1FormDeletedResponse from a dict
form_api_forms_v1_form_deleted_response_from_dict = FormApiFormsV1FormDeletedResponse.from_dict(form_api_forms_v1_form_deleted_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


