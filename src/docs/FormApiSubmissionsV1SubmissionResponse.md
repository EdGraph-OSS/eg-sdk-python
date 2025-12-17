# FormApiSubmissionsV1SubmissionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**form_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**current_step** | **int** |  | [optional] 
**data** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**deleted_by** | **str** |  | [optional] 
**deleted_date_time** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.form_api_submissions_v1_submission_response import FormApiSubmissionsV1SubmissionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of FormApiSubmissionsV1SubmissionResponse from a JSON string
form_api_submissions_v1_submission_response_instance = FormApiSubmissionsV1SubmissionResponse.from_json(json)
# print the JSON string representation of the object
print(FormApiSubmissionsV1SubmissionResponse.to_json())

# convert the object into a dict
form_api_submissions_v1_submission_response_dict = form_api_submissions_v1_submission_response_instance.to_dict()
# create an instance of FormApiSubmissionsV1SubmissionResponse from a dict
form_api_submissions_v1_submission_response_from_dict = FormApiSubmissionsV1SubmissionResponse.from_dict(form_api_submissions_v1_submission_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


