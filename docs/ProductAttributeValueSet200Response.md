# ProductAttributeValueSet200Response
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReturnCode** | **Int32** |  | [optional] 
**ReturnMessage** | **String** |  | [optional] 
**Result** | [**ProductAttributeValueSet200ResponseResult**](ProductAttributeValueSet200ResponseResult.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductAttributeValueSet200Response = Initialize-PSOpenAPIToolsProductAttributeValueSet200Response  -ReturnCode null `
 -ReturnMessage null `
 -Result null
```

- Convert the resource to JSON
```powershell
$ProductAttributeValueSet200Response | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

