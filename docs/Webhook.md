# Webhook
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **Int32** |  | [optional] 
**Label** | **String** |  | [optional] 
**StoreId** | **String** |  | [optional] 
**LangId** | **String** |  | [optional] 
**Active** | **Boolean** |  | [optional] 
**Callback** | **String** |  | [optional] 
**Fields** | **String** |  | [optional] 
**ResponseFields** | **String** |  | [optional] 
**CreatedAt** | **String** |  | [optional] 
**UpdatedAt** | **String** |  | [optional] 
**Entity** | **String** |  | [optional] 
**Action** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$Webhook = Initialize-PSOpenAPIToolsWebhook  -Id null `
 -Label null `
 -StoreId null `
 -LangId null `
 -Active null `
 -Callback null `
 -Fields null `
 -ResponseFields null `
 -CreatedAt null `
 -UpdatedAt null `
 -Entity null `
 -Action null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$Webhook | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

