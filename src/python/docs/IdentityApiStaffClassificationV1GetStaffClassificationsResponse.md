# IdentityApiStaffClassificationV1GetStaffClassificationsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[IdentityApiStaffClassificationV1StaffClassificationResponse]**](IdentityApiStaffClassificationV1StaffClassificationResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.identity_api_staff_classification_v1_get_staff_classifications_response import IdentityApiStaffClassificationV1GetStaffClassificationsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiStaffClassificationV1GetStaffClassificationsResponse from a JSON string
identity_api_staff_classification_v1_get_staff_classifications_response_instance = IdentityApiStaffClassificationV1GetStaffClassificationsResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiStaffClassificationV1GetStaffClassificationsResponse.to_json())

# convert the object into a dict
identity_api_staff_classification_v1_get_staff_classifications_response_dict = identity_api_staff_classification_v1_get_staff_classifications_response_instance.to_dict()
# create an instance of IdentityApiStaffClassificationV1GetStaffClassificationsResponse from a dict
identity_api_staff_classification_v1_get_staff_classifications_response_from_dict = IdentityApiStaffClassificationV1GetStaffClassificationsResponse.from_dict(identity_api_staff_classification_v1_get_staff_classifications_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


