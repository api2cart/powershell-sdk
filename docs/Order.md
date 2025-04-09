# Order
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**OrderId** | **String** |  | [optional] 
**BasketId** | **String** |  | [optional] 
**ChannelId** | **String** |  | [optional] 
**Customer** | [**BaseCustomer**](BaseCustomer.md) |  | [optional] 
**CreateAt** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**Currency** | [**Currency**](Currency.md) |  | [optional] 
**ShippingAddress** | [**CustomerAddress**](CustomerAddress.md) |  | [optional] 
**BillingAddress** | [**CustomerAddress**](CustomerAddress.md) |  | [optional] 
**PaymentMethod** | [**OrderPaymentMethod**](OrderPaymentMethod.md) |  | [optional] 
**ShippingMethod** | [**OrderShippingMethod**](OrderShippingMethod.md) |  | [optional] 
**ShippingMethods** | [**OrderShippingMethod[]**](OrderShippingMethod.md) |  | [optional] 
**Status** | [**OrderStatus**](OrderStatus.md) |  | [optional] 
**Totals** | [**OrderTotals**](OrderTotals.md) |  | [optional] 
**Total** | [**OrderTotal**](OrderTotal.md) |  | [optional] 
**Discounts** | [**OrderTotalsNewDiscount[]**](OrderTotalsNewDiscount.md) |  | [optional] 
**OrderProducts** | [**OrderItem[]**](OrderItem.md) |  | [optional] 
**Bundles** | [**OrderItem[]**](OrderItem.md) |  | [optional] 
**ModifiedAt** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**FinishedTime** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**Comment** | **String** |  | [optional] 
**StoreId** | **String** |  | [optional] 
**WarehousesIds** | **String[]** |  | [optional] 
**Refunds** | [**OrderRefund[]**](OrderRefund.md) |  | [optional] 
**GiftMessage** | **String** |  | [optional] 
**OrderDetailsUrl** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$Order = Initialize-PSOpenAPIToolsOrder  -Id null `
 -OrderId null `
 -BasketId null `
 -ChannelId null `
 -Customer null `
 -CreateAt null `
 -Currency null `
 -ShippingAddress null `
 -BillingAddress null `
 -PaymentMethod null `
 -ShippingMethod null `
 -ShippingMethods null `
 -Status null `
 -Totals null `
 -Total null `
 -Discounts null `
 -OrderProducts null `
 -Bundles null `
 -ModifiedAt null `
 -FinishedTime null `
 -Comment null `
 -StoreId null `
 -WarehousesIds null `
 -Refunds null `
 -GiftMessage null `
 -OrderDetailsUrl null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$Order | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

