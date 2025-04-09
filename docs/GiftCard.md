# GiftCard
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Code** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Type** | **String** |  | [optional] 
**CurrencyCode** | **String** |  | [optional] 
**Amount** | **Decimal** |  | [optional] 
**InitialAmount** | **Decimal** |  | [optional] 
**Status** | **String** |  | [optional] 
**CreatedAt** | **String** |  | [optional] 
**AvailTo** | **String** |  | [optional] 
**FreeProductIds** | **String** |  | [optional] 
**Message** | **String** |  | [optional] 
**IssuerEmail** | **String** |  | [optional] 
**RecipientEmail** | **String** |  | [optional] 
**IssuerName** | **String** |  | [optional] 
**RecipientName** | **String** |  | [optional] 
**UsageHistory** | [**CouponHistory[]**](CouponHistory.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$GiftCard = Initialize-PSOpenAPIToolsGiftCard  -Id null `
 -Code null `
 -Name null `
 -Type null `
 -CurrencyCode null `
 -Amount null `
 -InitialAmount null `
 -Status null `
 -CreatedAt null `
 -AvailTo null `
 -FreeProductIds null `
 -Message null `
 -IssuerEmail null `
 -RecipientEmail null `
 -IssuerName null `
 -RecipientName null `
 -UsageHistory null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$GiftCard | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

