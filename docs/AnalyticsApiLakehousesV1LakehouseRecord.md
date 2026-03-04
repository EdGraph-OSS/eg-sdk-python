# AnalyticsApiLakehousesV1LakehouseRecord


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**school_year** | **int** |  | [optional] 
**data_standard_name** | **str** |  | [optional] 
**data_standard_version** | **str** |  | [optional] 
**entity_name** | **str** |  | [optional] 
**resource_key_hash** | **str** |  | [optional] 
**json_payload** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.analytics_api_lakehouses_v1_lakehouse_record import AnalyticsApiLakehousesV1LakehouseRecord

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiLakehousesV1LakehouseRecord from a JSON string
analytics_api_lakehouses_v1_lakehouse_record_instance = AnalyticsApiLakehousesV1LakehouseRecord.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiLakehousesV1LakehouseRecord.to_json())

# convert the object into a dict
analytics_api_lakehouses_v1_lakehouse_record_dict = analytics_api_lakehouses_v1_lakehouse_record_instance.to_dict()
# create an instance of AnalyticsApiLakehousesV1LakehouseRecord from a dict
analytics_api_lakehouses_v1_lakehouse_record_from_dict = AnalyticsApiLakehousesV1LakehouseRecord.from_dict(analytics_api_lakehouses_v1_lakehouse_record_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


