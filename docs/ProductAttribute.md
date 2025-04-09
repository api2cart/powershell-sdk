# ProductAttribute
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AttributeId** | **String** |  | [optional] 
**Code** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**LangId** | **String** |  | [optional] 
**StoreId** | **String** |  | [optional] 
**Value** | **String** |  | [optional] 
**Required** | **Boolean** |  | [optional] 
**Visible** | **Boolean** |  | [optional] 
**Type** | **String** |  | [optional] 
**Position** | **Int32** |  | [optional] 
**AttributeGroupId** | **String** |  | [optional] 
**ProductId** | **String** |  | [optional] 
**VariantId** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductAttribute = Initialize-PSOpenAPIToolsProductAttribute  -AttributeId null `
 -Code null `
 -Name null `
 -LangId null `
 -StoreId null `
 -Value null `
 -Required null `
 -Visible null `
 -Type null `
 -Position null `
 -AttributeGroupId null `
 -ProductId null `
 -VariantId null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ProductAttribute | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

