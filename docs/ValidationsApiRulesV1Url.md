# ValidationsApiRulesV1Url


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | [optional] 
**label** | **str** |  | [optional] 
**value** | **str** |  | [optional] 
**open_in_new_tab** | **bool** |  | [optional] 
**system_defined** | **bool** |  | [optional] 
**readonly** | **bool** |  | [optional] 
**url_type** | [**ValidationsApiRulesV1UrlType**](ValidationsApiRulesV1UrlType.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_rules_v1_url import ValidationsApiRulesV1Url

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiRulesV1Url from a JSON string
validations_api_rules_v1_url_instance = ValidationsApiRulesV1Url.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiRulesV1Url.to_json())

# convert the object into a dict
validations_api_rules_v1_url_dict = validations_api_rules_v1_url_instance.to_dict()
# create an instance of ValidationsApiRulesV1Url from a dict
validations_api_rules_v1_url_from_dict = ValidationsApiRulesV1Url.from_dict(validations_api_rules_v1_url_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


