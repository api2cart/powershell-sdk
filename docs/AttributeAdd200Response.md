# AttributeAdd200Response
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReturnCode** | **Int32** |  | [optional] 
**ReturnMessage** | **String** |  | [optional] 
**Result** | [**AttributeAdd200ResponseResult**](AttributeAdd200ResponseResult.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$AttributeAdd200Response = Initialize-PSOpenAPIToolsAttributeAdd200Response  -ReturnCode null `
 -ReturnMessage null `
 -Result null
```

- Convert the resource to JSON
```powershell
$AttributeAdd200Response | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

