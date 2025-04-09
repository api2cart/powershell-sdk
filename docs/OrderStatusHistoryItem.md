# OrderStatusHistoryItem
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**ModifiedTime** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**Notify** | **Boolean** |  | [optional] 
**Comment** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderStatusHistoryItem = Initialize-PSOpenAPIToolsOrderStatusHistoryItem  -Id null `
 -Name null `
 -ModifiedTime null `
 -Notify null `
 -Comment null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$OrderStatusHistoryItem | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

