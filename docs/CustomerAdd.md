# CustomerAdd
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Email** | **String** | Defines customer&#39;s email | 
**FirstName** | **String** | Defines customer&#39;s first name | [optional] 
**LastName** | **String** | Defines customer&#39;s last name | [optional] 
**Password** | **String** | Defines customer&#39;s unique password | [optional] 
**Group** | **String** | Defines the group where the customer | [optional] 
**GroupId** | **String** | Customer group_id | [optional] 
**GroupIds** | **String** | Groups that will be assigned to a customer | [optional] 
**Status** | **String** | Defines customer&#39;s status | [optional] [default to "enabled"]
**CreatedTime** | **String** | Entity&#39;s date creation | [optional] 
**ModifiedTime** | **String** | Entity&#39;s date modification | [optional] 
**Login** | **String** | Specifies customer&#39;s login name | [optional] 
**LastLogin** | **String** | Defines customer&#39;s last login time | [optional] 
**BirthDay** | **String** | Defines customer&#39;s birthday | [optional] 
**NewsLetterSubscription** | **Boolean** | Defines whether the newsletter subscription is available for the user | [optional] 
**Consents** | [**CustomerAddConsentsInner[]**](CustomerAddConsentsInner.md) | Defines consents to notifications | [optional] 
**Gender** | **String** | Defines customer&#39;s gender | [optional] 
**Website** | **String** | Link to customer website | [optional] 
**Fax** | **String** | Defines customer&#39;s fax | [optional] 
**Company** | **String** | Defines customer&#39;s company | [optional] 
**Phone** | **String** | Defines customer&#39;s phone number | [optional] 
**Note** | **String** | The customer note. | [optional] 
**Country** | **String** | Specifies ISO code or name of country | [optional] 
**StoreId** | **String** | Store Id | [optional] 
**Address** | [**CustomerAddAddressInner[]**](CustomerAddAddressInner.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$CustomerAdd = Initialize-PSOpenAPIToolsCustomerAdd  -Email mail@example.com `
 -FirstName John `
 -LastName Smith `
 -Password fd5gfd5g75fd `
 -Group Register `
 -GroupId 3 `
 -GroupIds 1,2,3 `
 -Status disabled `
 -CreatedTime 2014-01-30 15:58:41 `
 -ModifiedTime 2014-07-30 15:58:41 `
 -Login makaka `
 -LastLogin 2013-02-26 15:00:00 `
 -BirthDay 2013-02-26 15:00:00 `
 -NewsLetterSubscription true `
 -Consents null `
 -Gender male `
 -Website http://api2cart.com `
 -Fax 54545787 `
 -Company Apple `
 -Phone 56686868654 `
 -Note Customer note `
 -Country US `
 -StoreId 1 `
 -Address null
```

- Convert the resource to JSON
```powershell
$CustomerAdd | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

