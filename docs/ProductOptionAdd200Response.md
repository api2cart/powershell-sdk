# ProductOptionAdd200Response
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReturnCode** | **Int32** |  | [optional] 
**ReturnMessage** | **String** |  | [optional] 
**Result** | [**ProductOptionAdd200ResponseResult**](ProductOptionAdd200ResponseResult.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductOptionAdd200Response = Initialize-PSOpenAPIToolsProductOptionAdd200Response  -ReturnCode null `
 -ReturnMessage null `
 -Result null
```

- Convert the resource to JSON
```powershell
$ProductOptionAdd200Response | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

