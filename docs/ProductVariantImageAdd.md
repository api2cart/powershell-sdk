# ProductVariantImageAdd
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ProductId** | **String** | Defines product id where the variant image has to be added | [optional] 
**ProductVariantId** | **String** | Defines product&#39;s variants specified by variant id | 
**ImageName** | **String** | Defines image&#39;s name | 
**Type** | **String** | Defines image&#39;s types that are specified by comma-separated list | [default to "base"]
**Url** | **String** | Defines URL of the image that has to be added | [optional] 
**Content** | **String** | Content(body) encoded in base64 of image file | [optional] 
**Label** | **String** | Defines alternative text that has to be attached to the picture | [optional] 
**Mime** | **String** | Mime type of image http://en.wikipedia.org/wiki/Internet_media_type. | [optional] 
**Position** | **Int32** | Defines image’s position in the list | [optional] [default to 0]
**StoreId** | **String** | Store Id | [optional] 
**OptionId** | **String** | Defines option id of the product variant for which the image will be added | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductVariantImageAdd = Initialize-PSOpenAPIToolsProductVariantImageAdd  -ProductId 10 `
 -ProductVariantId 45 `
 -ImageName abibas.png `
 -Type base `
 -Url http://docs.api2cart.com/img/logo.png `
 -Content /9j/4AAQSkZ...gD/2Q&#x3D;&#x3D; `
 -Label This cool image `
 -Mime image/jpeg `
 -Position 5 `
 -StoreId 1 `
 -OptionId 5
```

- Convert the resource to JSON
```powershell
$ProductVariantImageAdd | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

