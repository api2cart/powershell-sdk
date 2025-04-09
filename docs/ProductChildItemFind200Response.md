# ProductChildItemFind200Response
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReturnCode** | **Int32** |  | [optional] 
**ReturnMessage** | **String** |  | [optional] 
**Result** | [**ProductChildItemFind200ResponseResult**](ProductChildItemFind200ResponseResult.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductChildItemFind200Response = Initialize-PSOpenAPIToolsProductChildItemFind200Response  -ReturnCode null `
 -ReturnMessage null `
 -Result null
```

- Convert the resource to JSON
```powershell
$ProductChildItemFind200Response | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

