# CartConfigUpdate
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DbTablesPrefix** | **String** | This parameter is deprecated for this method. Please, use this parameter in method account.config.update | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) | This parameter sets the list of params to the shopping cart. | [optional] 
**StoreId** | **String** | Store Id | [optional] 
**UserAgent** | **String** | This parameter allows you to set your custom user agent, which will be used in requests to the store. Please use it cautiously, as the store&#39;s firewall may block specific values. | [optional] 

## Examples

- Prepare the resource
```powershell
$CartConfigUpdate = Initialize-PSOpenAPIToolsCartConfigUpdate  -DbTablesPrefix oc_ `
 -CustomFields null `
 -StoreId 1 `
 -UserAgent Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:47.0) Gecko/20100101 Firefox/47.0
```

- Convert the resource to JSON
```powershell
$CartConfigUpdate | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

