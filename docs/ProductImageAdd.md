# ProductImageAdd
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **String** | Defines image&#39;s types that are specified by comma-separated list | 
**ImageName** | **String** | Defines image&#39;s name | 
**ProductId** | **String** | Defines product id where the image should be added | [optional] 
**ProductVariantId** | **String** | Defines product&#39;s variants specified by variant id | [optional] 
**VariantIds** | **String** | Defines product&#39;s variants ids | [optional] 
**OptionValueIds** | **String** | Defines product&#39;s option values ids | [optional] 
**StoreId** | **String** | Store Id | [optional] 
**LangId** | **String** | Add product image on specified language id | [optional] 
**Url** | **String** | Defines URL of the image that has to be added | [optional] 
**Content** | **String** | Content(body) encoded in base64 of image file | [optional] 
**Label** | **String** | Defines alternative text that has to be attached to the picture | [optional] 
**Mime** | **String** | Mime type of image http://en.wikipedia.org/wiki/Internet_media_type. | [optional] 
**Position** | **Int32** | Defines image’s position in the list | [optional] [default to 0]
**UseLatestApiVersion** | **Boolean** | Use the latest platform API version | [optional] [default to $false]

## Examples

- Prepare the resource
```powershell
$ProductImageAdd = Initialize-PSOpenAPIToolsProductImageAdd  -Type base,small `
 -ImageName bag-gray.png `
 -ProductId 10 `
 -ProductVariantId 45 `
 -VariantIds 1,2,3,4,5 `
 -OptionValueIds 1,2,3,4,5 `
 -StoreId 1 `
 -LangId 3 `
 -Url http://docs.api2cart.com/img/logo.png `
 -Content /9j/4AAQSkZ...gD/2Q&#x3D;&#x3D; `
 -Label This cool image `
 -Mime image/jpeg `
 -Position 5 `
 -UseLatestApiVersion true
```

- Convert the resource to JSON
```powershell
$ProductImageAdd | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

