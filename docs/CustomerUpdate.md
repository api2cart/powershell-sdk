# CustomerUpdate
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** | Entity id | [optional] 
**GroupId** | **String** | Customer group_id | [optional] 
**GroupIds** | **String** | Groups that will be assigned to a customer | [optional] 
**Group** | **String** | Defines the group where the customer | [optional] 
**Email** | **String** | Defines customer&#39;s email | [optional] 
**Phone** | **String** | Defines customer&#39;s phone number | [optional] 
**FirstName** | **String** | Defines customer&#39;s first name | [optional] 
**LastName** | **String** | Defines customer&#39;s last name | [optional] 
**BirthDay** | **String** | Defines customer&#39;s birthday | [optional] 
**NewsLetterSubscription** | **Boolean** | Defines whether the newsletter subscription is available for the user | [optional] 
**Consents** | [**CustomerAddConsentsInner[]**](CustomerAddConsentsInner.md) | Defines consents to notifications | [optional] 
**Tags** | **String** | Customer tags | [optional] 
**Gender** | **String** | Defines customer&#39;s gender | [optional] 
**StoreId** | **String** | Store Id | [optional] 
**Note** | **String** | The customer note. | [optional] 
**Status** | **String** | Defines customer&#39;s status | [optional] 
**Address** | [**CustomerUpdateAddressInner[]**](CustomerUpdateAddressInner.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$CustomerUpdate = Initialize-PSOpenAPIToolsCustomerUpdate  -Id 10 `
 -GroupId 3 `
 -GroupIds 1,2,3 `
 -Group Register `
 -Email mail@example.com `
 -Phone 56686868654 `
 -FirstName John `
 -LastName Smith `
 -BirthDay 2013-02-26 15:00:00 `
 -NewsLetterSubscription true `
 -Consents null `
 -Tags tag1,tag2 `
 -Gender male `
 -StoreId 1 `
 -Note Customer note `
 -Status disabled `
 -Address null
```

- Convert the resource to JSON
```powershell
$CustomerUpdate | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

