# FormApiSubmissionsV1SubmissionUpdatedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**form_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_submissions_v1_submission_updated_response import FormApiSubmissionsV1SubmissionUpdatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiSubmissionsV1SubmissionUpdatedResponse from a JSON string
form_api_submissions_v1_submission_updated_response_instance = FormApiSubmissionsV1SubmissionUpdatedResponse.from_json(json)
# print the JSON string representation of the object
print(FormApiSubmissionsV1SubmissionUpdatedResponse.to_json())

# convert the object into a dict
form_api_submissions_v1_submission_updated_response_dict = form_api_submissions_v1_submission_updated_response_instance.to_dict()
# create an instance of FormApiSubmissionsV1SubmissionUpdatedResponse from a dict
form_api_submissions_v1_submission_updated_response_from_dict = FormApiSubmissionsV1SubmissionUpdatedResponse.from_dict(form_api_submissions_v1_submission_updated_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


