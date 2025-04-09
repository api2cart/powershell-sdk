# AccountCartAdd200Response
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReturnCode** | **Int32** |  | [optional] 
**ReturnMessage** | **String** |  | [optional] 
**Result** | [**AccountCartAdd200ResponseResult**](AccountCartAdd200ResponseResult.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$AccountCartAdd200Response = Initialize-PSOpenAPIToolsAccountCartAdd200Response  -ReturnCode null `
 -ReturnMessage null `
 -Result null
```

- Convert the resource to JSON
```powershell
$AccountCartAdd200Response | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

