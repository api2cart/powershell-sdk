# ReturnCount200Response
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReturnCode** | **Int32** |  | [optional] 
**ReturnMessage** | **String** |  | [optional] 
**Result** | [**ReturnCount200ResponseResult**](ReturnCount200ResponseResult.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ReturnCount200Response = Initialize-PSOpenAPIToolsReturnCount200Response  -ReturnCode null `
 -ReturnMessage null `
 -Result null
```

- Convert the resource to JSON
```powershell
$ReturnCount200Response | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

