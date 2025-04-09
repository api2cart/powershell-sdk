# ResponseCartGiftcardListResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**GiftCard** | [**GiftCard[]**](GiftCard.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ResponseCartGiftcardListResult = Initialize-PSOpenAPIToolsResponseCartGiftcardListResult  -GiftCard null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ResponseCartGiftcardListResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

