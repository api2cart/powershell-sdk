# ProductOptionAdd
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **String** | Defines option&#39;s name | 
**Type** | **String** | Defines option&#39;s type that has to be added | 
**ProductId** | **String** | Defines product id where the option should be added | [optional] 
**DefaultOptionValue** | **String** | Defines default option value that has to be added | [optional] 
**OptionValues** | **String** | Defines option values that has to be added | [optional] 
**Description** | **String** | Defines option&#39;s description | [optional] 
**Avail** | **Boolean** | Defines whether the option is available | [optional] [default to $true]
**SortOrder** | **Int32** | Sort number in the list | [optional] [default to 0]
**Required** | **Boolean** | Defines if the option is required | [optional] [default to $false]
**Values** | [**ProductOptionAddValuesInner[]**](ProductOptionAddValuesInner.md) | An array of option values.&lt;/b&gt; | [optional] 
**ClearCache** | **Boolean** | Is cache clear required | [optional] [default to $true]

## Examples

- Prepare the resource
```powershell
$ProductOptionAdd = Initialize-PSOpenAPIToolsProductOptionAdd  -Name Color `
 -Type option_type_select `
 -ProductId 10 `
 -DefaultOptionValue green `
 -OptionValues green,black,yellow `
 -Description Product option `
 -Avail false `
 -SortOrder 2 `
 -Required true `
 -Values null `
 -ClearCache false
```

- Convert the resource to JSON
```powershell
$ProductOptionAdd | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

