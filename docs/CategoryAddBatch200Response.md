# CategoryAddBatch200Response
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReturnCode** | **Int32** |  | [optional] 
**ReturnMessage** | **String** |  | [optional] 
**Result** | [**CategoryAddBatch200ResponseResult**](CategoryAddBatch200ResponseResult.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$CategoryAddBatch200Response = Initialize-PSOpenAPIToolsCategoryAddBatch200Response  -ReturnCode null `
 -ReturnMessage null `
 -Result null
```

- Convert the resource to JSON
```powershell
$CategoryAddBatch200Response | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

