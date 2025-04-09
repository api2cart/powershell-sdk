# CartPluginList200ResponseResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AllPlugins** | **Int32** |  | [optional] 
**Plugins** | [**PluginList[]**](PluginList.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$CartPluginList200ResponseResult = Initialize-PSOpenAPIToolsCartPluginList200ResponseResult  -AllPlugins null `
 -Plugins null
```

- Convert the resource to JSON
```powershell
$CartPluginList200ResponseResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

