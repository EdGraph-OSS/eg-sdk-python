# IdentityApiStaffClassificationV1StaffClassificationLicenseRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**application_id** | **str** |  | [optional] 
**license_status** | **str** |  | [optional] 
**roles** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.identity_api_staff_classification_v1_staff_classification_license_request import IdentityApiStaffClassificationV1StaffClassificationLicenseRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiStaffClassificationV1StaffClassificationLicenseRequest from a JSON string
identity_api_staff_classification_v1_staff_classification_license_request_instance = IdentityApiStaffClassificationV1StaffClassificationLicenseRequest.from_json(json)
# print the JSON string representation of the object
print(IdentityApiStaffClassificationV1StaffClassificationLicenseRequest.to_json())

# convert the object into a dict
identity_api_staff_classification_v1_staff_classification_license_request_dict = identity_api_staff_classification_v1_staff_classification_license_request_instance.to_dict()
# create an instance of IdentityApiStaffClassificationV1StaffClassificationLicenseRequest from a dict
identity_api_staff_classification_v1_staff_classification_license_request_from_dict = IdentityApiStaffClassificationV1StaffClassificationLicenseRequest.from_dict(identity_api_staff_classification_v1_staff_classification_license_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


