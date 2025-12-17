# FormApiSubmissionsV1SubmissionsExportedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**form_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**type** | [**FormApiSubmissionsV1ExportType**](FormApiSubmissionsV1ExportType.md) |  | [optional] 
**status** | [**FormApiSubmissionsV1ExportStatus**](FormApiSubmissionsV1ExportStatus.md) |  | [optional] 
**details** | **str** |  | [optional] 
**contents** | **List[int]** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_submissions_v1_submissions_exported_response import FormApiSubmissionsV1SubmissionsExportedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiSubmissionsV1SubmissionsExportedResponse from a JSON string
form_api_submissions_v1_submissions_exported_response_instance = FormApiSubmissionsV1SubmissionsExportedResponse.from_json(json)
# print the JSON string representation of the object
print(FormApiSubmissionsV1SubmissionsExportedResponse.to_json())

# convert the object into a dict
form_api_submissions_v1_submissions_exported_response_dict = form_api_submissions_v1_submissions_exported_response_instance.to_dict()
# create an instance of FormApiSubmissionsV1SubmissionsExportedResponse from a dict
form_api_submissions_v1_submissions_exported_response_from_dict = FormApiSubmissionsV1SubmissionsExportedResponse.from_dict(form_api_submissions_v1_submissions_exported_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


