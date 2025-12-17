# FormApiFormsV1FormAccessResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**target_audience** | [**FormApiFormsV1AudienceType**](FormApiFormsV1AudienceType.md) |  | [optional] 
**single_response_per_individual** | **bool** |  | [optional] 
**staff_classifications** | **List[str]** |  | [optional] [readonly] 
**users** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.form_api_forms_v1_form_access_response import FormApiFormsV1FormAccessResponse

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiFormsV1FormAccessResponse from a JSON string
form_api_forms_v1_form_access_response_instance = FormApiFormsV1FormAccessResponse.from_json(json)
# print the JSON string representation of the object
print(FormApiFormsV1FormAccessResponse.to_json())

# convert the object into a dict
form_api_forms_v1_form_access_response_dict = form_api_forms_v1_form_access_response_instance.to_dict()
# create an instance of FormApiFormsV1FormAccessResponse from a dict
form_api_forms_v1_form_access_response_from_dict = FormApiFormsV1FormAccessResponse.from_dict(form_api_forms_v1_form_access_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


