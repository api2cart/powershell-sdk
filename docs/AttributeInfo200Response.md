# AttributeInfo200Response
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReturnCode** | **Int32** |  | [optional] 
**ReturnMessage** | **String** |  | [optional] 
**Result** | [**StoreAttribute**](StoreAttribute.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$AttributeInfo200Response = Initialize-PSOpenAPIToolsAttributeInfo200Response  -ReturnCode null `
 -ReturnMessage null `
 -Result null
```

- Convert the resource to JSON
```powershell
$AttributeInfo200Response | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

