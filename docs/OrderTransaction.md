# OrderTransaction
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**TransactionId** | **String** |  | [optional] 
**OrderId** | **String** |  | [optional] 
**ParentId** | **String** |  | [optional] 
**Description** | **String** |  | [optional] 
**Status** | **String** |  | [optional] 
**Gateway** | **String** |  | [optional] 
**ReferenceNumber** | **String** |  | [optional] 
**Currency** | **String** |  | [optional] 
**Amount** | **Decimal** |  | [optional] 
**CreatedTime** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**SettlementCurrency** | **String** |  | [optional] 
**SettlementAmount** | **Decimal** |  | [optional] 
**SettlementCreatedTime** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**CardBrand** | **String** |  | [optional] 
**CardBin** | **String** |  | [optional] 
**CardLastFour** | **String** |  | [optional] 
**AvsStreetRespCode** | **String** |  | [optional] 
**AvsPostalRespCode** | **String** |  | [optional] 
**AvsMessage** | **String** |  | [optional] 
**CvvCode** | **String** |  | [optional] 
**CvvMessage** | **String** |  | [optional] 
**IsTestMode** | **Boolean** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderTransaction = Initialize-PSOpenAPIToolsOrderTransaction  -Id null `
 -TransactionId null `
 -OrderId null `
 -ParentId null `
 -Description null `
 -Status null `
 -Gateway null `
 -ReferenceNumber null `
 -Currency null `
 -Amount null `
 -CreatedTime null `
 -SettlementCurrency null `
 -SettlementAmount null `
 -SettlementCreatedTime null `
 -CardBrand null `
 -CardBin null `
 -CardLastFour null `
 -AvsStreetRespCode null `
 -AvsPostalRespCode null `
 -AvsMessage null `
 -CvvCode null `
 -CvvMessage null `
 -IsTestMode null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$OrderTransaction | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

