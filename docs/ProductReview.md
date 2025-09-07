# ProductReview
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**ProductId** | **String** |  | [optional] 
**CustomerId** | **String** |  | [optional] 
**NickName** | **String** |  | [optional] 
**Email** | **String** |  | [optional] 
**Summary** | **String** |  | [optional] 
**Message** | **String** |  | [optional] 
**Rating** | **Decimal** |  | [optional] 
**Ratings** | [**ProductReviewRating[]**](ProductReviewRating.md) |  | [optional] 
**Status** | **String** |  | [optional] 
**CreatedTime** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**ModifiedTime** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**Medias** | [**Media[]**](Media.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductReview = Initialize-PSOpenAPIToolsProductReview  -Id null `
 -ProductId null `
 -CustomerId null `
 -NickName null `
 -Email null `
 -Summary null `
 -Message null `
 -Rating null `
 -Ratings null `
 -Status null `
 -CreatedTime null `
 -ModifiedTime null `
 -Medias null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ProductReview | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

