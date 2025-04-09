# ProductAddCertificationsInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** | Certification ID | 
**Images** | [**ProductAddCertificationsInnerImagesInner[]**](ProductAddCertificationsInnerImagesInner.md) | Certification images | [optional] 
**Files** | [**ProductAddCertificationsInnerFilesInner[]**](ProductAddCertificationsInnerFilesInner.md) | Certification files | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductAddCertificationsInner = Initialize-PSOpenAPIToolsProductAddCertificationsInner  -Id null `
 -Images null `
 -Files null
```

- Convert the resource to JSON
```powershell
$ProductAddCertificationsInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

