# ValidationsApiRulesV1PaginatedRules


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[ValidationsApiRulesV1RuleDto]**](ValidationsApiRulesV1RuleDto.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_rules_v1_paginated_rules import ValidationsApiRulesV1PaginatedRules

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiRulesV1PaginatedRules from a JSON string
validations_api_rules_v1_paginated_rules_instance = ValidationsApiRulesV1PaginatedRules.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiRulesV1PaginatedRules.to_json())

# convert the object into a dict
validations_api_rules_v1_paginated_rules_dict = validations_api_rules_v1_paginated_rules_instance.to_dict()
# create an instance of ValidationsApiRulesV1PaginatedRules from a dict
validations_api_rules_v1_paginated_rules_from_dict = ValidationsApiRulesV1PaginatedRules.from_dict(validations_api_rules_v1_paginated_rules_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


