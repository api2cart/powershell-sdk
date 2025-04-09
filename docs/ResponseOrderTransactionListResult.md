# ResponseOrderTransactionListResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TransactionsCount** | **Int32** |  | [optional] 
**Transactions** | [**OrderTransaction[]**](OrderTransaction.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ResponseOrderTransactionListResult = Initialize-PSOpenAPIToolsResponseOrderTransactionListResult  -TransactionsCount null `
 -Transactions null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ResponseOrderTransactionListResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

