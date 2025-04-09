# Customer
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Email** | **String** |  | [optional] 
**FirstName** | **String** |  | [optional] 
**LastName** | **String** |  | [optional] 
**Phone** | **String** |  | [optional] 
**CreatedTime** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**ModifiedTime** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**Group** | [**CustomerGroup[]**](CustomerGroup.md) |  | [optional] 
**Login** | **String** |  | [optional] 
**LastLogin** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**BirthDay** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**Status** | **String** |  | [optional] 
**NewsLetterSubscription** | **Boolean** |  | [optional] 
**Consents** | [**CustomerConsent[]**](CustomerConsent.md) |  | [optional] 
**Gender** | **String** |  | [optional] 
**StoresIds** | **String[]** |  | [optional] 
**Website** | **String** |  | [optional] 
**Fax** | **String** |  | [optional] 
**Company** | **String** |  | [optional] 
**IpAddress** | **String** |  | [optional] 
**AddressBook** | [**CustomerAddress[]**](CustomerAddress.md) |  | [optional] 
**LangId** | **String** |  | [optional] 
**OrdersCount** | **Int32** |  | [optional] 
**LastOrderId** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$Customer = Initialize-PSOpenAPIToolsCustomer  -Id null `
 -Email null `
 -FirstName null `
 -LastName null `
 -Phone null `
 -CreatedTime null `
 -ModifiedTime null `
 -Group null `
 -Login null `
 -LastLogin null `
 -BirthDay null `
 -Status null `
 -NewsLetterSubscription null `
 -Consents null `
 -Gender null `
 -StoresIds null `
 -Website null `
 -Fax null `
 -Company null `
 -IpAddress null `
 -AddressBook null `
 -LangId null `
 -OrdersCount null `
 -LastOrderId null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$Customer | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

