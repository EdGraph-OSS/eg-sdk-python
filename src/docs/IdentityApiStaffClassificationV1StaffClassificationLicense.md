# IdentityApiStaffClassificationV1StaffClassificationLicense


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**application_id** | **str** |  | [optional] 
**license_status** | **str** |  | [optional] 
**roles** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.identity_api_staff_classification_v1_staff_classification_license import IdentityApiStaffClassificationV1StaffClassificationLicense

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiStaffClassificationV1StaffClassificationLicense from a JSON string
identity_api_staff_classification_v1_staff_classification_license_instance = IdentityApiStaffClassificationV1StaffClassificationLicense.from_json(json)
# print the JSON string representation of the object
print(IdentityApiStaffClassificationV1StaffClassificationLicense.to_json())

# convert the object into a dict
identity_api_staff_classification_v1_staff_classification_license_dict = identity_api_staff_classification_v1_staff_classification_license_instance.to_dict()
# create an instance of IdentityApiStaffClassificationV1StaffClassificationLicense from a dict
identity_api_staff_classification_v1_staff_classification_license_from_dict = IdentityApiStaffClassificationV1StaffClassificationLicense.from_dict(identity_api_staff_classification_v1_staff_classification_license_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


