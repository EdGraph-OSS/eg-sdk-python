# ValidationsApiJobsV1Metric


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**entity** | **str** |  | [optional] 
**processed** | **int** |  | [optional] 
**success** | **int** |  | [optional] 
**errors** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_jobs_v1_metric import ValidationsApiJobsV1Metric

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiJobsV1Metric from a JSON string
validations_api_jobs_v1_metric_instance = ValidationsApiJobsV1Metric.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiJobsV1Metric.to_json())

# convert the object into a dict
validations_api_jobs_v1_metric_dict = validations_api_jobs_v1_metric_instance.to_dict()
# create an instance of ValidationsApiJobsV1Metric from a dict
validations_api_jobs_v1_metric_from_dict = ValidationsApiJobsV1Metric.from_dict(validations_api_jobs_v1_metric_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


