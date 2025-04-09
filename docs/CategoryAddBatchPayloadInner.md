# CategoryAddBatchPayloadInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **String** |  | 
**Avail** | **Boolean** |  | [optional] 
**Description** | **String** |  | [optional] 
**MetaTitle** | **String** |  | [optional] 
**MetaDescription** | **String** |  | [optional] 
**MetaKeywords** | **String[]** |  | [optional] 
**ParentId** | **String** |  | [optional] 
**SortOrder** | **Int32** |  | [optional] 
**SeoUrl** | **String** |  | [optional] 
**StoreId** | **String** |  | [optional] 
**Images** | [**CategoryAddBatchPayloadInnerImagesInner[]**](CategoryAddBatchPayloadInnerImagesInner.md) |  | [optional] 
**StoresIds** | **String[]** |  | [optional] 

## Examples

- Prepare the resource
```powershell
$CategoryAddBatchPayloadInner = Initialize-PSOpenAPIToolsCategoryAddBatchPayloadInner  -Name null `
 -Avail null `
 -Description null `
 -MetaTitle null `
 -MetaDescription null `
 -MetaKeywords null `
 -ParentId null `
 -SortOrder null `
 -SeoUrl null `
 -StoreId null `
 -Images null `
 -StoresIds null
```

- Convert the resource to JSON
```powershell
$CategoryAddBatchPayloadInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

