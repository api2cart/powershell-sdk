# ResponseCustomerListResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CustomersCount** | **Int32** |  | [optional] 
**Customer** | [**Customer[]**](Customer.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ResponseCustomerListResult = Initialize-PSOpenAPIToolsResponseCustomerListResult  -CustomersCount null `
 -Customer null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ResponseCustomerListResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

