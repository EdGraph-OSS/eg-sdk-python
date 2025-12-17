# ValidationsApiReportingPeriodsV1CertificationStatusCategory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**category** | [**ValidationsApiContainersV1ContainerDto**](ValidationsApiContainersV1ContainerDto.md) |  | [optional] 
**record_count** | **int** |  | [optional] 
**fatal_count** | **int** |  | [optional] 
**warning_count** | **int** |  | [optional] 
**excluded_count** | **int** |  | [optional] 
**status** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_certification_status_category import ValidationsApiReportingPeriodsV1CertificationStatusCategory

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1CertificationStatusCategory from a JSON string
validations_api_reporting_periods_v1_certification_status_category_instance = ValidationsApiReportingPeriodsV1CertificationStatusCategory.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1CertificationStatusCategory.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_certification_status_category_dict = validations_api_reporting_periods_v1_certification_status_category_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1CertificationStatusCategory from a dict
validations_api_reporting_periods_v1_certification_status_category_from_dict = ValidationsApiReportingPeriodsV1CertificationStatusCategory.from_dict(validations_api_reporting_periods_v1_certification_status_category_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


