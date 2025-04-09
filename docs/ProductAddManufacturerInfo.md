# ProductAddManufacturerInfo
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **String** | Defines manufacturer&#x60;s name | [optional] 
**Address** | **String** | Defines manufacturer&#x60;s address | [optional] 
**Phone** | **String** | Defines manufacturer&#x60;s phone | [optional] 
**Email** | **String** | Defines manufacturer&#x60;s email | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductAddManufacturerInfo = Initialize-PSOpenAPIToolsProductAddManufacturerInfo  -Name null `
 -Address null `
 -Phone null `
 -Email null
```

- Convert the resource to JSON
```powershell
$ProductAddManufacturerInfo | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

