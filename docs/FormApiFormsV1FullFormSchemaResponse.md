# FormApiFormsV1FullFormSchemaResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**json_schema** | **str** |  | [optional] 
**ui_schema** | **str** |  | [optional] 
**details** | **str** |  | [optional] 
**status** | [**FormApiFormsV1SchemaStatus**](FormApiFormsV1SchemaStatus.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_forms_v1_full_form_schema_response import FormApiFormsV1FullFormSchemaResponse

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiFormsV1FullFormSchemaResponse from a JSON string
form_api_forms_v1_full_form_schema_response_instance = FormApiFormsV1FullFormSchemaResponse.from_json(json)
# print the JSON string representation of the object
print(FormApiFormsV1FullFormSchemaResponse.to_json())

# convert the object into a dict
form_api_forms_v1_full_form_schema_response_dict = form_api_forms_v1_full_form_schema_response_instance.to_dict()
# create an instance of FormApiFormsV1FullFormSchemaResponse from a dict
form_api_forms_v1_full_form_schema_response_from_dict = FormApiFormsV1FullFormSchemaResponse.from_dict(form_api_forms_v1_full_form_schema_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


