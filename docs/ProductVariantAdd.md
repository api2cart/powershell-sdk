# ProductVariantAdd
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ProductId** | **String** | Defines product&#39;s id where the variant has to be added | [optional] 
**Name** | **String** | Defines variant&#39;s name that has to be added | [optional] 
**Model** | **String** | Specifies variant&#39;s model that has to be added | 
**Sku** | **String** | Defines variant&#39;s sku that has to be added | [optional] 
**Barcode** | **String** | A barcode is a unique code composed of numbers used as a product identifier. | [optional] 
**Gtin** | **String** | Global Trade Item Number. An GTIN is an identifier for trade items. | [optional] 
**Price** | **Decimal** | Defines new product&#39;s variant price | [optional] 
**OldPrice** | **Decimal** | Defines product&#39;s old price | [optional] 
**CostPrice** | **Decimal** | Defines new product&#39;s cost price | [optional] 
**FixedCostShippingPrice** | **Decimal** | Specifies fixed cost shipping price | [optional] 
**Attributes** | [**ProductVariantAddAttributesInner[]**](ProductVariantAddAttributesInner.md) | Defines variant&#39;s attributes list | [optional] 
**Description** | **String** | Specifies variant&#39;s description | [optional] 
**SpecialPrice** | **Decimal** | Specifies variant&#39;s model that has to be added | [optional] 
**SpriceCreate** | **String** | Defines the date of special price creation | [optional] 
**SpriceModified** | **String** | Defines the date of special price modification | [optional] 
**SpriceExpire** | **String** | Defines the term of special price offer duration | [optional] 
**AvailableForView** | **Boolean** | Specifies the set of visible/invisible product&#39;s variants for users | [optional] [default to $true]
**AvailableForSale** | **Boolean** | Specifies the set of visible/invisible product&#39;s variants for sale | [optional] [default to $true]
**Weight** | **Decimal** | Weight | [optional] [default to 0]
**Width** | **Decimal** | Defines product&#39;s width | [optional] 
**Height** | **Decimal** | Defines product&#39;s height | [optional] 
**Length** | **Decimal** | Defines product&#39;s length | [optional] 
**WeightUnit** | **String** | Weight Unit | [optional] 
**ShortDescription** | **String** | Defines short description | [optional] 
**WarehouseId** | **String** | This parameter is used for selecting a warehouse where you need to set/modify a product quantity. | [optional] 
**Quantity** | **Decimal** | Defines product variant&#39;s quantity that has to be added | [optional] [default to 0]
**CreatedAt** | **String** | Defines the date of entity creation | [optional] 
**Manufacturer** | **String** | Specifies the product variant&#39;s manufacturer | [optional] 
**TaxClassId** | **String** | Defines tax classes where entity has to be added | [optional] 
**MetaTitle** | **String** | Defines unique meta title for each entity | [optional] 
**MetaKeywords** | **String** | Defines unique meta keywords for each entity | [optional] 
**MetaDescription** | **String** | Defines unique meta description of a entity | [optional] 
**Url** | **String** | Defines unique product variant&#39;s URL | [optional] 
**StoreId** | **String** | Add variants specified by store id | [optional] 
**LangId** | **String** | Language id | [optional] 
**ClearCache** | **Boolean** | Is cache clear required | [optional] [default to $true]
**Taxable** | **Boolean** | Specifies whether a tax is charged | [optional] [default to $true]
**HarmonizedSystemCode** | **String** | Harmonized System Code. An HSC is a 6-digit identifier that allows participating countries to classify traded goods on a common basis for customs purposes | [optional] 
**CountryOfOrigin** | **String** | The country where the inventory item was made | [optional] 
**ManageStock** | **Boolean** | Defines inventory tracking for product variant | [optional] 
**Upc** | **String** | Universal Product Code. A UPC (UPC-A) is a commonly used identifer for many different products. | [optional] 
**Mpn** | **String** | Manufacturer Part Number. A MPN is an identifier of a particular part design or material used. | [optional] 
**Ean** | **String** | European Article Number. An EAN is a unique 8 or 13-digit identifier that many industries (such as book publishers) use to identify products. | [optional] 
**Isbn** | **String** | International Standard Book Number. An ISBN is a unique identifier for books. | [optional] 
**StoresIds** | **String** | Assign variant to the stores that is specified by comma-separated stores&#39; id | [optional] 
**IsDefault** | **Boolean** | Defines as a default variant | [optional] 
**IsFreeShipping** | **Boolean** | Specifies variant&#39;s free shipping flag that has to be added | [optional] 
**MarketplaceItemProperties** | **String** | String containing the JSON representation of the supplied data | [optional] 
**InStock** | **Boolean** | Set stock status | [optional] 
**BackorderStatus** | **String** | Set backorder status | [optional] 
**TierPrices** | [**ProductAddTierPricesInner[]**](ProductAddTierPricesInner.md) | Defines product&#39;s tier prices | [optional] 
**IsVirtual** | **Boolean** | Defines whether the product is virtual | [optional] [default to $false]

## Examples

- Prepare the resource
```powershell
$ProductVariantAdd = Initialize-PSOpenAPIToolsProductVariantAdd  -ProductId 10 `
 -Name Bag Green XXL `
 -Model bag_01 `
 -Sku bag_01 `
 -Barcode 9770317847001 `
 -Gtin 12345678912345 `
 -Price 99.9 `
 -OldPrice 99.9 `
 -CostPrice 65.9 `
 -FixedCostShippingPrice 5.5 `
 -Attributes null `
 -Description Product variant `
 -SpecialPrice 56.9 `
 -SpriceCreate 2018-08-25 23:56:12 `
 -SpriceModified 2018-12-05 13:46:20 `
 -SpriceExpire 2018-08-25 23:56:12 `
 -AvailableForView false `
 -AvailableForSale false `
 -Weight 23.69 `
 -Width 56.12 `
 -Height 56.12 `
 -Length 56.12 `
 -WeightUnit lb `
 -ShortDescription Short description. This is very short description `
 -WarehouseId 1 `
 -Quantity 6 `
 -CreatedAt 2014-08-09 13:13:13 `
 -Manufacturer Samsung `
 -TaxClassId 9 `
 -MetaTitle category,test `
 -MetaKeywords category,test `
 -MetaDescription category,test `
 -Url /product_variant_slug `
 -StoreId 1 `
 -LangId 3 `
 -ClearCache false `
 -Taxable false `
 -HarmonizedSystemCode 123456 `
 -CountryOfOrigin 123456 `
 -ManageStock false `
 -Upc 9770317847001 `
 -Mpn 9770317847001 `
 -Ean 5901234123457 `
 -Isbn 9783161484100 `
 -StoresIds 1,2 `
 -IsDefault true `
 -IsFreeShipping true `
 -MarketplaceItemProperties {&quot;color&quot;:[&quot;Silver&quot;],&quot;manufacturer&quot;:&quot;Philips&quot;,&quot;features&quot;:[&quot;3 way&quot;],&quot;countPerPack&quot;:1,&quot;watts&quot;:{&quot;unit&quot;:&quot;W&quot;,&quot;measure&quot;:40}} `
 -InStock true `
 -BackorderStatus true `
 -TierPrices null `
 -IsVirtual false
```

- Convert the resource to JSON
```powershell
$ProductVariantAdd | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

