# Subscriber
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**CustomerId** | **String** |  | [optional] 
**Email** | **String** |  | [optional] 
**Subscribed** | **Boolean** |  | [optional] 
**FirstName** | **String** |  | [optional] 
**LastName** | **String** |  | [optional] 
**StoresIds** | **String[]** |  | [optional] 
**CreatedTime** | **String** |  | [optional] 
**ModifiedTime** | **String** |  | [optional] 
**LangId** | **String** |  | [optional] 
**Gender** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$Subscriber = Initialize-PSOpenAPIToolsSubscriber  -Id null `
 -CustomerId null `
 -Email null `
 -Subscribed null `
 -FirstName null `
 -LastName null `
 -StoresIds null `
 -CreatedTime null `
 -ModifiedTime null `
 -LangId null `
 -Gender null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$Subscriber | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

