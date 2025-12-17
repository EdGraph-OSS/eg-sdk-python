# FormApiFormsV1SetFormAccessRequest


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
from edgraph_platform_client.models.form_api_forms_v1_set_form_access_request import FormApiFormsV1SetFormAccessRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiFormsV1SetFormAccessRequest from a JSON string
form_api_forms_v1_set_form_access_request_instance = FormApiFormsV1SetFormAccessRequest.from_json(json)
# print the JSON string representation of the object
print(FormApiFormsV1SetFormAccessRequest.to_json())

# convert the object into a dict
form_api_forms_v1_set_form_access_request_dict = form_api_forms_v1_set_form_access_request_instance.to_dict()
# create an instance of FormApiFormsV1SetFormAccessRequest from a dict
form_api_forms_v1_set_form_access_request_from_dict = FormApiFormsV1SetFormAccessRequest.from_dict(form_api_forms_v1_set_form_access_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


