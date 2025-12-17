# FormApiSubmissionsV1SubmissionCreatedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**form_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_submissions_v1_submission_created_response import FormApiSubmissionsV1SubmissionCreatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiSubmissionsV1SubmissionCreatedResponse from a JSON string
form_api_submissions_v1_submission_created_response_instance = FormApiSubmissionsV1SubmissionCreatedResponse.from_json(json)
# print the JSON string representation of the object
print(FormApiSubmissionsV1SubmissionCreatedResponse.to_json())

# convert the object into a dict
form_api_submissions_v1_submission_created_response_dict = form_api_submissions_v1_submission_created_response_instance.to_dict()
# create an instance of FormApiSubmissionsV1SubmissionCreatedResponse from a dict
form_api_submissions_v1_submission_created_response_from_dict = FormApiSubmissionsV1SubmissionCreatedResponse.from_dict(form_api_submissions_v1_submission_created_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


