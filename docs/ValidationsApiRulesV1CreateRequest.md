# ValidationsApiRulesV1CreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** | Details | [optional] 
**container_id** | **str** |  | [optional] 
**id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**diagnostic_sql** | **str** | SQL | [optional] 
**count_sql** | **str** |  | [optional] 
**error_severity_level** | **int** |  | [optional] 
**error_message** | **str** |  | [optional] 
**max_number_results** | **int** |  | [optional] 
**rule_identification** | **str** | Metadata | [optional] 
**resolution** | **str** |  | [optional] 
**tags** | **List[str]** |  | [optional] [readonly] 
**version** | **str** |  | [optional] 
**collection_id** | **str** |  | [optional] 
**urls** | [**List[ValidationsApiRulesV1Url]**](ValidationsApiRulesV1Url.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_rules_v1_create_request import ValidationsApiRulesV1CreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiRulesV1CreateRequest from a JSON string
validations_api_rules_v1_create_request_instance = ValidationsApiRulesV1CreateRequest.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiRulesV1CreateRequest.to_json())

# convert the object into a dict
validations_api_rules_v1_create_request_dict = validations_api_rules_v1_create_request_instance.to_dict()
# create an instance of ValidationsApiRulesV1CreateRequest from a dict
validations_api_rules_v1_create_request_from_dict = ValidationsApiRulesV1CreateRequest.from_dict(validations_api_rules_v1_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


