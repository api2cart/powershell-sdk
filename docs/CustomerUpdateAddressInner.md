# CustomerUpdateAddressInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AddressBookId** | **String** | The ID of the address. | [optional] 
**AddressBookFirstName** | **String** | Specifies customer&#39;s first name in the address book | [optional] 
**AddressBookLastName** | **String** | Specifies customer&#39;s last name in the address book | [optional] 
**AddressBookCompany** | **String** | Specifies customer&#39;s company name in the address book | [optional] 
**AddressBookFax** | **String** | Specifies customer&#39;s fax in the address book | [optional] 
**AddressBookPhone** | **String** | Specifies customer&#39;s phone number in the address book | [optional] 
**AddressBookPhoneMobile** | **String** | Specifies customer&#39;s mobile phone number in the address book | [optional] 
**AddressBookAddress1** | **String** | Specifies customer&#39;s first address in the address book | [optional] 
**AddressBookAddress2** | **String** | Specifies customer&#39;s second address in the address book | [optional] 
**AddressBookCity** | **String** | Specifies customer&#39;s city in the address book | [optional] 
**AddressBookCountry** | **String** | ISO code or name of country | [optional] 
**AddressBookState** | **String** | ISO code or name of state. | [optional] 
**AddressBookPostcode** | **String** | Specifies customer&#39;s postcode | [optional] 
**AddressBookTaxId** | **String** | Add Tax Id | [optional] 
**AddressBookIdentificationNumber** | **String** | The national ID card number of this person, or a unique tax identification number. | [optional] 
**AddressBookGender** | **String** | Specifies customer&#39;s gender | [optional] 
**AddressBookAlias** | **String** | Specifies customer&#39;s alias in the address book | [optional] 
**AddressBookType** | **String** | Specifies customer&#39;s address type | [optional] 
**AddressBookDefault** | **Boolean** | Defines whether the address is used by default | [optional] 

## Examples

- Prepare the resource
```powershell
$CustomerUpdateAddressInner = Initialize-PSOpenAPIToolsCustomerUpdateAddressInner  -AddressBookId 7805807034473 `
 -AddressBookFirstName John `
 -AddressBookLastName Smith `
 -AddressBookCompany Samsung `
 -AddressBookFax 5758787 `
 -AddressBookPhone 5758787 `
 -AddressBookPhoneMobile 5758787 `
 -AddressBookAddress1 Green str. 35 `
 -AddressBookAddress2 Green str. 35 `
 -AddressBookCity Chicago `
 -AddressBookCountry US `
 -AddressBookState IL `
 -AddressBookPostcode 12345 `
 -AddressBookTaxId &#x60;12345678&#x60; `
 -AddressBookIdentificationNumber &#x60;123-456-7890&#x60; `
 -AddressBookGender male `
 -AddressBookAlias Address alias `
 -AddressBookType billing `
 -AddressBookDefault true
```

- Convert the resource to JSON
```powershell
$CustomerUpdateAddressInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

