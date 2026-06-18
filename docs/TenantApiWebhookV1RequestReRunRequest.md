# TenantApiWebhookV1RequestReRunRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**webhook_id** | **str** |  | [optional] 
**dispatch_id** | **str** |  | [optional] 
**webhook_re_run_strategy** | [**TenantApiWebhookV1WebhookReRunStrategy**](TenantApiWebhookV1WebhookReRunStrategy.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_webhook_v1_request_re_run_request import TenantApiWebhookV1RequestReRunRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiWebhookV1RequestReRunRequest from a JSON string
tenant_api_webhook_v1_request_re_run_request_instance = TenantApiWebhookV1RequestReRunRequest.from_json(json)
# print the JSON string representation of the object
print(TenantApiWebhookV1RequestReRunRequest.to_json())

# convert the object into a dict
tenant_api_webhook_v1_request_re_run_request_dict = tenant_api_webhook_v1_request_re_run_request_instance.to_dict()
# create an instance of TenantApiWebhookV1RequestReRunRequest from a dict
tenant_api_webhook_v1_request_re_run_request_from_dict = TenantApiWebhookV1RequestReRunRequest.from_dict(tenant_api_webhook_v1_request_re_run_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


