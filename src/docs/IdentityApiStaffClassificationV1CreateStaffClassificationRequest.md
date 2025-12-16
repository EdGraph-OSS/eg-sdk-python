# IdentityApiStaffClassificationV1CreateStaffClassificationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**namespace** | **str** |  | [optional] 
**code_value** | **str** |  | [optional] 
**short_description** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**licenses** | [**List[IdentityApiStaffClassificationV1StaffClassificationLicenseRequest]**](IdentityApiStaffClassificationV1StaffClassificationLicenseRequest.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.identity_api_staff_classification_v1_create_staff_classification_request import IdentityApiStaffClassificationV1CreateStaffClassificationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiStaffClassificationV1CreateStaffClassificationRequest from a JSON string
identity_api_staff_classification_v1_create_staff_classification_request_instance = IdentityApiStaffClassificationV1CreateStaffClassificationRequest.from_json(json)
# print the JSON string representation of the object
print(IdentityApiStaffClassificationV1CreateStaffClassificationRequest.to_json())

# convert the object into a dict
identity_api_staff_classification_v1_create_staff_classification_request_dict = identity_api_staff_classification_v1_create_staff_classification_request_instance.to_dict()
# create an instance of IdentityApiStaffClassificationV1CreateStaffClassificationRequest from a dict
identity_api_staff_classification_v1_create_staff_classification_request_from_dict = IdentityApiStaffClassificationV1CreateStaffClassificationRequest.from_dict(identity_api_staff_classification_v1_create_staff_classification_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


