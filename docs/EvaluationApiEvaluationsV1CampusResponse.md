# EvaluationApiEvaluationsV1CampusResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**campus** | **str** |  | [optional] 
**identifier_type** | [**EvaluationApiEvaluationsV1OrganizationIdentifierType**](EvaluationApiEvaluationsV1OrganizationIdentifierType.md) |  | [optional] 
**discriminator** | [**EvaluationApiEvaluationsV1OrganizationDiscriminator**](EvaluationApiEvaluationsV1OrganizationDiscriminator.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.evaluation_api_evaluations_v1_campus_response import EvaluationApiEvaluationsV1CampusResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EvaluationApiEvaluationsV1CampusResponse from a JSON string
evaluation_api_evaluations_v1_campus_response_instance = EvaluationApiEvaluationsV1CampusResponse.from_json(json)
# print the JSON string representation of the object
print(EvaluationApiEvaluationsV1CampusResponse.to_json())

# convert the object into a dict
evaluation_api_evaluations_v1_campus_response_dict = evaluation_api_evaluations_v1_campus_response_instance.to_dict()
# create an instance of EvaluationApiEvaluationsV1CampusResponse from a dict
evaluation_api_evaluations_v1_campus_response_from_dict = EvaluationApiEvaluationsV1CampusResponse.from_dict(evaluation_api_evaluations_v1_campus_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


