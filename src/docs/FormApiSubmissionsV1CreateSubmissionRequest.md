# FormApiSubmissionsV1CreateSubmissionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**form_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**current_step** | **int** |  | [optional] 
**data** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_submissions_v1_create_submission_request import FormApiSubmissionsV1CreateSubmissionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiSubmissionsV1CreateSubmissionRequest from a JSON string
form_api_submissions_v1_create_submission_request_instance = FormApiSubmissionsV1CreateSubmissionRequest.from_json(json)
# print the JSON string representation of the object
print(FormApiSubmissionsV1CreateSubmissionRequest.to_json())

# convert the object into a dict
form_api_submissions_v1_create_submission_request_dict = form_api_submissions_v1_create_submission_request_instance.to_dict()
# create an instance of FormApiSubmissionsV1CreateSubmissionRequest from a dict
form_api_submissions_v1_create_submission_request_from_dict = FormApiSubmissionsV1CreateSubmissionRequest.from_dict(form_api_submissions_v1_create_submission_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


