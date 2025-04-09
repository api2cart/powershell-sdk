# PluginList
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AllPlugins** | **Int32** |  | [optional] 
**Plugins** | [**Plugin[]**](Plugin.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$PluginList = Initialize-PSOpenAPIToolsPluginList  -AllPlugins null `
 -Plugins null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$PluginList | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

