# IdentityApiStaffClassificationV1StaffClassificationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**namespace** | **str** |  | [optional] 
**code_value** | **str** |  | [optional] 
**short_description** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**licenses** | [**List[IdentityApiStaffClassificationV1StaffClassificationLicense]**](IdentityApiStaffClassificationV1StaffClassificationLicense.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.identity_api_staff_classification_v1_staff_classification_response import IdentityApiStaffClassificationV1StaffClassificationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiStaffClassificationV1StaffClassificationResponse from a JSON string
identity_api_staff_classification_v1_staff_classification_response_instance = IdentityApiStaffClassificationV1StaffClassificationResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiStaffClassificationV1StaffClassificationResponse.to_json())

# convert the object into a dict
identity_api_staff_classification_v1_staff_classification_response_dict = identity_api_staff_classification_v1_staff_classification_response_instance.to_dict()
# create an instance of IdentityApiStaffClassificationV1StaffClassificationResponse from a dict
identity_api_staff_classification_v1_staff_classification_response_from_dict = IdentityApiStaffClassificationV1StaffClassificationResponse.from_dict(identity_api_staff_classification_v1_staff_classification_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


