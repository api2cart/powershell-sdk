# CustomerAddressAdd
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CustomerId** | **String** | Defines customer id | 
**StoreId** | **String** | Store Id | [optional] 
**FirstName** | **String** | Defines customer&#39;s address first name | [optional] 
**LastName** | **String** | Defines customer&#39;s address last name | [optional] 
**Company** | **String** | Defines customer&#39;s address company | [optional] 
**Address1** | **String** | Specifies customer&#39;s address address1 | 
**Address2** | **String** | Specifies customer&#39;s address address2 | [optional] 
**City** | **String** | Specifies customer&#39;s address city | 
**Country** | **String** | Specifies customer&#39;s address ISO code or name of country | 
**State** | **String** | Specifies customer&#39;s address ISO code or name of state | [optional] 
**Postcode** | **String** | Specifies customer&#39;s address postcode | 
**IdentificationNumber** | **String** | Specifies the national ID card number of this person, or a unique tax identification number for customer&#39;s address | [optional] 
**Types** | **String[]** | Specifies customer&#39;s address types | [optional] 
**Default** | **Boolean** | Specifies whether the customer&#39;s address is used by default | [optional] 
**Phone** | **String** | Defines customer&#39;s address phone number | [optional] 
**PhoneMobile** | **String** | Defines customer&#39;s address mobile phone number | [optional] 
**Fax** | **String** | Defines customer&#39;s address fax | [optional] 
**Website** | **String** | Defines Link to customer&#39;s address website | [optional] 
**Gender** | **String** | Defines customer&#39;s address gender | [optional] 
**TaxId** | **String** | Add Tax Id | [optional] 
**Alias** | **String** | Specifies customer&#39;s alias in the address book | [optional] 

## Examples

- Prepare the resource
```powershell
$CustomerAddressAdd = Initialize-PSOpenAPIToolsCustomerAddressAdd  -CustomerId 5 `
 -StoreId 1 `
 -FirstName John `
 -LastName Smith `
 -Company Apple `
 -Address1 Green str. 35 `
 -Address2 Green str. 35 `
 -City Chicago `
 -Country US `
 -State IL `
 -Postcode 12345 `
 -IdentificationNumber &#x60;123-456-7890&#x60; `
 -Types types[0]&#x3D;billing&amp;types[1]&#x3D;shipping `
 -Default true `
 -Phone 56686868654 `
 -PhoneMobile 56686868654 `
 -Fax 54545787 `
 -Website http://api2cart.com `
 -Gender male `
 -TaxId &#x60;12345678&#x60; `
 -Alias Address alias
```

- Convert the resource to JSON
```powershell
$CustomerAddressAdd | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

