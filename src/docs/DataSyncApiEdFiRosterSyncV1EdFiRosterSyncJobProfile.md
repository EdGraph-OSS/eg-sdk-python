# DataSyncApiEdFiRosterSyncV1EdFiRosterSyncJobProfile


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**mode** | [**DataSyncApiEdFiRosterSyncV1EdFiRosterSyncJobMode**](DataSyncApiEdFiRosterSyncV1EdFiRosterSyncJobMode.md) |  | [optional] 
**provider** | [**DataSyncApiEdFiRosterSyncV1EdFiRosterSyncJobProvider**](DataSyncApiEdFiRosterSyncV1EdFiRosterSyncJobProvider.md) |  | [optional] 
**connection_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**client_secret** | **str** |  | [optional] 
**base_url** | **str** |  | [optional] 
**authentication_url** | **str** |  | [optional] 
**resources_url** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**ed_fi_instance_id** | **str** |  | [optional] 
**use_ssa_instead_of_seoaa** | [**DataSyncApiEdFiRosterSyncV1UseSSAInsteadOfSEOAAOptions**](DataSyncApiEdFiRosterSyncV1UseSSAInsteadOfSEOAAOptions.md) |  | [optional] 
**import_section_and_course_data** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.data_sync_api_ed_fi_roster_sync_v1_ed_fi_roster_sync_job_profile import DataSyncApiEdFiRosterSyncV1EdFiRosterSyncJobProfile

# TODO update the JSON string below
json = "{}"
# create an instance of DataSyncApiEdFiRosterSyncV1EdFiRosterSyncJobProfile from a JSON string
data_sync_api_ed_fi_roster_sync_v1_ed_fi_roster_sync_job_profile_instance = DataSyncApiEdFiRosterSyncV1EdFiRosterSyncJobProfile.from_json(json)
# print the JSON string representation of the object
print(DataSyncApiEdFiRosterSyncV1EdFiRosterSyncJobProfile.to_json())

# convert the object into a dict
data_sync_api_ed_fi_roster_sync_v1_ed_fi_roster_sync_job_profile_dict = data_sync_api_ed_fi_roster_sync_v1_ed_fi_roster_sync_job_profile_instance.to_dict()
# create an instance of DataSyncApiEdFiRosterSyncV1EdFiRosterSyncJobProfile from a dict
data_sync_api_ed_fi_roster_sync_v1_ed_fi_roster_sync_job_profile_from_dict = DataSyncApiEdFiRosterSyncV1EdFiRosterSyncJobProfile.from_dict(data_sync_api_ed_fi_roster_sync_v1_ed_fi_roster_sync_job_profile_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


