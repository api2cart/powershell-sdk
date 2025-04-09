# Info
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Owner** | **String** |  | [optional] 
**Country** | **String** |  | [optional] 
**State** | **String** |  | [optional] 
**StateCode** | **String** |  | [optional] 
**City** | **String** |  | [optional] 
**StreetAddress** | **String** |  | [optional] 
**StreetAddressLine2** | **String** |  | [optional] 
**ZipCode** | **String** |  | [optional] 
**Email** | **String** |  | [optional] 
**Phone** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$Info = Initialize-PSOpenAPIToolsInfo  -Owner null `
 -Country null `
 -State null `
 -StateCode null `
 -City null `
 -StreetAddress null `
 -StreetAddressLine2 null `
 -ZipCode null `
 -Email null `
 -Phone null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$Info | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

