# FormApiSubmissionsV1UpdateSubmissionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**form_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**current_step** | **int** |  | [optional] 
**data** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_submissions_v1_update_submission_request import FormApiSubmissionsV1UpdateSubmissionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiSubmissionsV1UpdateSubmissionRequest from a JSON string
form_api_submissions_v1_update_submission_request_instance = FormApiSubmissionsV1UpdateSubmissionRequest.from_json(json)
# print the JSON string representation of the object
print(FormApiSubmissionsV1UpdateSubmissionRequest.to_json())

# convert the object into a dict
form_api_submissions_v1_update_submission_request_dict = form_api_submissions_v1_update_submission_request_instance.to_dict()
# create an instance of FormApiSubmissionsV1UpdateSubmissionRequest from a dict
form_api_submissions_v1_update_submission_request_from_dict = FormApiSubmissionsV1UpdateSubmissionRequest.from_dict(form_api_submissions_v1_update_submission_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


