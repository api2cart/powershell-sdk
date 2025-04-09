# CartBridge200Response
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReturnCode** | **Int32** |  | [optional] 
**ReturnMessage** | **String** |  | [optional] 
**Result** | [**CartBridge200ResponseResult**](CartBridge200ResponseResult.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$CartBridge200Response = Initialize-PSOpenAPIToolsCartBridge200Response  -ReturnCode null `
 -ReturnMessage null `
 -Result null
```

- Convert the resource to JSON
```powershell
$CartBridge200Response | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

