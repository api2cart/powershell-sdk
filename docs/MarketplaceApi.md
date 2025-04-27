# PSOpenAPITools.PSOpenAPITools\Api.MarketplaceApi

All URIs are relative to *https://api.api2cart.com/v1.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Invoke-MarketplaceProductFind**](MarketplaceApi.md#Invoke-MarketplaceProductFind) | **GET** /marketplace.product.find.json | marketplace.product.find


<a id="Invoke-MarketplaceProductFind"></a>
# **Invoke-MarketplaceProductFind**
> ModelResponseMarketplaceProductFind Invoke-MarketplaceProductFind<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Keyword] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CategoriesIds] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Asin] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Ean] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Gtin] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Upc] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Mpn] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Isbn] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

marketplace.product.find

Search product in global catalog.

### Example
```powershell
# general setting of the PowerShell module, e.g. base URL, authentication, etc
$Configuration = Get-Configuration
# Configure API key authorization: StoreKeyAuth
$Configuration.ApiKey.x-store-key = "YOUR_API_KEY"
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
#$Configuration.ApiKeyPrefix.x-store-key = "Bearer"

# Configure API key authorization: ApiKeyAuth
$Configuration.ApiKey.x-api-key = "YOUR_API_KEY"
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
#$Configuration.ApiKeyPrefix.x-api-key = "Bearer"

$Count = 20 # Int32 | This parameter sets the entity amount that has to be retrieved. Max allowed count=250 (optional) (default to 10)
$PageCursor = "MyPageCursor" # String | Used to retrieve entities via cursor-based pagination (it can't be used with any other filtering parameter) (optional)
$Keyword = "T-shirt" # String | Defines search keyword (optional)
$CategoriesIds = "23,56" # String | Defines product add that is specified by comma-separated categories id (optional)
$StoreId = "1" # String | Store Id (optional)
$Asin = "97703178470" # String | Amazon Standard Identification Number. (optional)
$Ean = "5901234123457" # String | European Article Number. An EAN is a unique 8 or 13-digit identifier that many industries (such as book publishers) use to identify products. (optional)
$Gtin = "12345678912345" # String | Global Trade Item Number. An GTIN is an identifier for trade items. (optional)
$Upc = "9770317847001" # String | Universal Product Code. A UPC (UPC-A) is a commonly used identifer for many different products. (optional)
$Mpn = "9770317847001" # String | Manufacturer Part Number. A MPN is an identifier of a particular part design or material used. (optional)
$Isbn = "9783161484100" # String | International Standard Book Number. An ISBN is a unique identifier for books. (optional)
$ResponseFields = "{result}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Params = "id,model,price,images" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "force_all")
$Exclude = "false" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# marketplace.product.find
try {
    $Result = Invoke-MarketplaceProductFind -Count $Count -PageCursor $PageCursor -Keyword $Keyword -CategoriesIds $CategoriesIds -StoreId $StoreId -Asin $Asin -Ean $Ean -Gtin $Gtin -Upc $Upc -Mpn $Mpn -Isbn $Isbn -ResponseFields $ResponseFields -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-MarketplaceProductFind: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **Keyword** | **String**| Defines search keyword | [optional] 
 **CategoriesIds** | **String**| Defines product add that is specified by comma-separated categories id | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **Asin** | **String**| Amazon Standard Identification Number. | [optional] 
 **Ean** | **String**| European Article Number. An EAN is a unique 8 or 13-digit identifier that many industries (such as book publishers) use to identify products. | [optional] 
 **Gtin** | **String**| Global Trade Item Number. An GTIN is an identifier for trade items. | [optional] 
 **Upc** | **String**| Universal Product Code. A UPC (UPC-A) is a commonly used identifer for many different products. | [optional] 
 **Mpn** | **String**| Manufacturer Part Number. A MPN is an identifier of a particular part design or material used. | [optional] 
 **Isbn** | **String**| International Standard Book Number. An ISBN is a unique identifier for books. | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;force_all&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**ModelResponseMarketplaceProductFind**](ModelResponseMarketplaceProductFind.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

