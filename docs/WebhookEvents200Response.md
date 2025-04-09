# WebhookEvents200Response
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReturnCode** | **Int32** |  | [optional] 
**ReturnMessage** | **String** |  | [optional] 
**Result** | [**WebhookEvents200ResponseResult**](WebhookEvents200ResponseResult.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$WebhookEvents200Response = Initialize-PSOpenAPIToolsWebhookEvents200Response  -ReturnCode null `
 -ReturnMessage null `
 -Result null
```

- Convert the resource to JSON
```powershell
$WebhookEvents200Response | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

