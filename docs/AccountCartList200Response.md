# AccountCartList200Response
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReturnCode** | **Int32** |  | [optional] 
**ReturnMessage** | **String** |  | [optional] 
**Result** | [**AccountCartList200ResponseResult**](AccountCartList200ResponseResult.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$AccountCartList200Response = Initialize-PSOpenAPIToolsAccountCartList200Response  -ReturnCode null `
 -ReturnMessage null `
 -Result null
```

- Convert the resource to JSON
```powershell
$AccountCartList200Response | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

