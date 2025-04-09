# AccountFailedWebhooks200ResponseResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AllFailedWebhook** | **String** |  | [optional] 
**Webhook** | [**AccountFailedWebhooks200ResponseResultWebhookInner[]**](AccountFailedWebhooks200ResponseResultWebhookInner.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$AccountFailedWebhooks200ResponseResult = Initialize-PSOpenAPIToolsAccountFailedWebhooks200ResponseResult  -AllFailedWebhook null `
 -Webhook null
```

- Convert the resource to JSON
```powershell
$AccountFailedWebhooks200ResponseResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

