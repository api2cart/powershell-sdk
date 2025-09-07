# OrderCalculate
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CustomerEmail** | **String** | Defines the customer specified by email for whom the order needs to be calculated | 
**CurrencyId** | **String** | Currency Id | [optional] 
**StoreId** | **String** | Store Id | [optional] 
**Coupons** | **String[]** | Coupons that will be applied to order. If the order isn&#39;t eligible for any given discount code or there is no discount with such a code it will be skipped during calculation | [optional] 
**ShippFirstName** | **String** | Specifies shipping first name | 
**ShippLastName** | **String** | Specifies shipping last name | 
**ShippAddress1** | **String** | Specifies first shipping address | 
**ShippAddress2** | **String** | Specifies second address line of a shipping street address | [optional] 
**ShippCity** | **String** | Specifies shipping city | 
**ShippPostcode** | **String** | Specifies shipping postcode | 
**ShippState** | **String** | Specifies shipping state code | [optional] 
**ShippCountry** | **String** | Specifies shipping country code | 
**ShippCompany** | **String** | Specifies shipping company | [optional] 
**ShippPhone** | **String** | Specifies shipping phone | [optional] 
**BillFirstName** | **String** | Specifies billing first name | [optional] 
**BillLastName** | **String** | Specifies billing last name | [optional] 
**BillAddress1** | **String** | Specifies first billing address | [optional] 
**BillAddress2** | **String** | Specifies second billing address | [optional] 
**BillCity** | **String** | Specifies billing city | [optional] 
**BillPostcode** | **String** | Specifies billing postcode | [optional] 
**BillState** | **String** | Specifies billing state code | [optional] 
**BillCountry** | **String** | Specifies billing country code | [optional] 
**BillCompany** | **String** | Specifies billing company | [optional] 
**BillPhone** | **String** | Specifies billing phone | [optional] 
**ResponseFields** | **String** | Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
**OrderItem** | [**OrderCalculateOrderItemInner[]**](OrderCalculateOrderItemInner.md) |  | 

## Examples

- Prepare the resource
```powershell
$OrderCalculate = Initialize-PSOpenAPIToolsOrderCalculate  -CustomerEmail jubari@hannsgroup.com `
 -CurrencyId usd `
 -StoreId 1 `
 -Coupons null `
 -ShippFirstName John `
 -ShippLastName Smith `
 -ShippAddress1 Green str. 35 `
 -ShippAddress2 Green str. 35 `
 -ShippCity Chicago `
 -ShippPostcode 24545 `
 -ShippState IL `
 -ShippCountry US `
 -ShippCompany Apple `
 -ShippPhone 880086544564 `
 -BillFirstName Adam `
 -BillLastName Smith `
 -BillAddress1 Green str. 35 `
 -BillAddress2 Red str, 2 `
 -BillCity Chicago `
 -BillPostcode 12345 `
 -BillState IL `
 -BillCountry US `
 -BillCompany Apple `
 -BillPhone 8 800 5659 6896 `
 -ResponseFields {result} `
 -OrderItem null
```

- Convert the resource to JSON
```powershell
$OrderCalculate | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

