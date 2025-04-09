# Brand
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**CreatedTime** | **String** |  | [optional] 
**ModifiedTime** | **String** |  | [optional] 
**FullDescription** | **String** |  | [optional] 
**ShortDescription** | **String** |  | [optional] 
**StoresIds** | **String[]** |  | [optional] 
**Active** | **Boolean** |  | [optional] 
**Url** | **String** |  | [optional] 
**MetaTitle** | **String** |  | [optional] 
**MetaKeywords** | **String** |  | [optional] 
**MetaDescription** | **String** |  | [optional] 
**Images** | [**Image[]**](Image.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$Brand = Initialize-PSOpenAPIToolsBrand  -Id null `
 -Name null `
 -CreatedTime null `
 -ModifiedTime null `
 -FullDescription null `
 -ShortDescription null `
 -StoresIds null `
 -Active null `
 -Url null `
 -MetaTitle null `
 -MetaKeywords null `
 -MetaDescription null `
 -Images null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$Brand | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

