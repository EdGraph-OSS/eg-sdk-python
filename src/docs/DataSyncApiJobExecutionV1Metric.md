# DataSyncApiJobExecutionV1Metric


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**entity** | **str** |  | [optional] 
**processed** | **int** |  | [optional] 
**success** | **int** |  | [optional] 
**errors** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_job_execution_v1_metric import DataSyncApiJobExecutionV1Metric

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiJobExecutionV1Metric from a JSON string
data_sync_api_job_execution_v1_metric_instance = DataSyncApiJobExecutionV1Metric.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiJobExecutionV1Metric.to_json())

# convert the object into a dict
data_sync_api_job_execution_v1_metric_dict = data_sync_api_job_execution_v1_metric_instance.to_dict()
# create an instance of DataSyncApiJobExecutionV1Metric from a dict
data_sync_api_job_execution_v1_metric_from_dict = DataSyncApiJobExecutionV1Metric.from_dict(data_sync_api_job_execution_v1_metric_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


