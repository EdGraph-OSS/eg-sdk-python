# IMSAdminApiV1ClientsClaim


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 
**value** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ims_admin_api_v1_clients_claim import IMSAdminApiV1ClientsClaim

# TODO update the JSON string below
json = "{}"
# create an instance of IMSAdminApiV1ClientsClaim from a JSON string
ims_admin_api_v1_clients_claim_instance = IMSAdminApiV1ClientsClaim.from_json(json)
# print the JSON string representation of the object
print(IMSAdminApiV1ClientsClaim.to_json())

# convert the object into a dict
ims_admin_api_v1_clients_claim_dict = ims_admin_api_v1_clients_claim_instance.to_dict()
# create an instance of IMSAdminApiV1ClientsClaim from a dict
ims_admin_api_v1_clients_claim_from_dict = IMSAdminApiV1ClientsClaim.from_dict(ims_admin_api_v1_clients_claim_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


