# ProductAdd
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **String** | Defines product&#39;s name that has to be added | 
**Model** | **String** | Defines product&#39;s model that has to be added | 
**Description** | **String** | Defines product&#39;s description that has to be added | 
**Price** | **Decimal** | Defines product&#39;s price that has to be added | 
**Sku** | **String** | Defines product&#39;s sku that has to be added | [optional] 
**ShortDescription** | **String** | Defines short description | [optional] 
**Type** | **String** | Defines product&#39;s type | [optional] [default to "simple"]
**Status** | **String** | Defines product&#39;s status | [optional] 
**Visible** | **String** | Set visibility status | [optional] 
**CategoryId** | **String** | Defines product add that is specified by category id | [optional] 
**CategoriesIds** | **String** | Defines product add that is specified by comma-separated categories id | [optional] 
**ProductClass** | **String** | A categorization for the product | [optional] 
**ProductType** | **String** | A categorization for the product | [optional] 
**IsVirtual** | **Boolean** | Defines whether the product is virtual | [optional] [default to $false]
**Downloadable** | **Boolean** | Defines whether the product is downloadable | [optional] [default to $false]
**IsSupply** | **Boolean** | If true, it indicates the product as a supply, otherwise it indicates that it is a finished product. | [optional] [default to $true]
**AvailableForView** | **Boolean** | Specifies the set of visible/invisible products for users | [optional] [default to $true]
**AvailableForSale** | **Boolean** | Specifies the set of visible/invisible products for sale | [optional] [default to $true]
**StoreId** | **String** | Store Id | [optional] 
**StoresIds** | **String** | Assign product to the stores that is specified by comma-separated stores&#39; id | [optional] 
**LangId** | **String** | Language id | [optional] 
**OldPrice** | **Decimal** | Defines product&#39;s old price | [optional] 
**SpecialPrice** | **Decimal** | Defines product&#39;s model that has to be added | [optional] 
**WholesalePrice** | **Decimal** | Defines product&#39;s sale price | [optional] 
**CostPrice** | **Decimal** | Defines new product&#39;s cost price | [optional] 
**FixedCostShippingPrice** | **Decimal** | Specifies product&#39;s fixed cost shipping price | [optional] 
**TierPrices** | [**ProductAddTierPricesInner[]**](ProductAddTierPricesInner.md) | Defines product&#39;s tier prices | [optional] 
**GroupPrices** | [**ProductAddGroupPricesInner[]**](ProductAddGroupPricesInner.md) | Defines product&#39;s group prices | [optional] 
**BuyitnowPrice** | **Decimal** | Defines buy it now value | [optional] 
**ReservePrice** | **Decimal** | Defines reserve price value | [optional] 
**Quantity** | **Decimal** | Defines product&#39;s quantity that has to be added | [optional] [default to 0]
**InStock** | **Boolean** | Set stock status | [optional] 
**ManageStock** | **Boolean** | Defines inventory tracking for product | [optional] 
**WarehouseId** | **String** | This parameter is used for selecting a warehouse where you need to set/modify a product quantity. | [optional] 
**BackorderStatus** | **String** | Set backorder status | [optional] 
**MinOrderQuantity** | **Decimal** | The minimum quantity an order must contain, to be eligible to purchase this product. | [optional] 
**MaxOrderQuantity** | **Decimal** | The maximum quantity an order can contain when purchasing the product. | [optional] 
**Weight** | **Decimal** | Weight | [optional] [default to 0]
**WeightUnit** | **String** | Weight Unit | [optional] 
**Width** | **Decimal** | Defines product&#39;s width | [optional] 
**Height** | **Decimal** | Defines product&#39;s height | [optional] 
**Length** | **Decimal** | Defines product&#39;s length | [optional] 
**DimensionsUnit** | **String** | Weight Unit | [optional] 
**Barcode** | **String** | A barcode is a unique code composed of numbers used as a product identifier. | [optional] 
**Upc** | **String** | Universal Product Code. A UPC (UPC-A) is a commonly used identifer for many different products. | [optional] 
**Ean** | **String** | European Article Number. An EAN is a unique 8 or 13-digit identifier that many industries (such as book publishers) use to identify products. | [optional] 
**Isbn** | **String** | International Standard Book Number. An ISBN is a unique identifier for books. | [optional] 
**Gtin** | **String** | Global Trade Item Number. An GTIN is an identifier for trade items. | [optional] 
**Mpn** | **String** | Manufacturer Part Number. A MPN is an identifier of a particular part design or material used. | [optional] 
**Asin** | **String** | Amazon Standard Identification Number. | [optional] 
**ProductReference** | **String** | Groups all variations, that you want to combine into one product. | [optional] 
**HarmonizedSystemCode** | **String** | Harmonized System Code. An HSC is a 6-digit identifier that allows participating countries to classify traded goods on a common basis for customs purposes | [optional] 
**CountryOfOrigin** | **String** | The country where the inventory item was made | [optional] 
**Manufacturer** | **String** | Defines product&#39;s manufacturer | [optional] 
**ManufacturerId** | **String** | Defines product&#39;s manufacturer by manufacturer_id | [optional] 
**ManufacturerInfo** | [**ProductAddManufacturerInfo**](ProductAddManufacturerInfo.md) |  | [optional] 
**BrandName** | **String** | Defines product brand name | [optional] 
**ImageUrl** | **String** | Image Url | [optional] 
**ImageName** | **String** | Defines image&#39;s name | [optional] 
**AdditionalImageUrls** | **String[]** | Image Url | [optional] 
**Files** | [**ProductAddFilesInner[]**](ProductAddFilesInner.md) | File Url | [optional] 
**SizeChart** | [**ProductAddSizeChart**](ProductAddSizeChart.md) |  | [optional] 
**RelatedProductsIds** | **String** | Defines product&#39;s related products ids that has to be added | [optional] 
**UpSellProductsIds** | **String** | Defines product&#39;s up-sell products ids that has to be added | [optional] 
**CrossSellProductsIds** | **String** | Defines product&#39;s cross-sell products ids that has to be added | [optional] 
**AttributeSetName** | **String** | Defines product’s attribute set name in Magento | [optional] [default to "Default"]
**AttributeName** | **String** | Defines product’s attribute name separated with a comma in Magento | [optional] 
**SearchKeywords** | **String** | Defines unique search keywords | [optional] 
**Tags** | **String** | Product tags | [optional] 
**Materials** | **String[]** | A list of material strings for materials used in the product. | [optional] 
**Certifications** | [**ProductAddCertificationsInner[]**](ProductAddCertificationsInner.md) | An array of product certifications. The list of possible certifications can be obtained using the &quot;&quot;&lt;i&gt;category.info&lt;/i&gt;&quot;&quot; method (&lt;i&gt;additional_fields-&gt;rules-&gt;product_certifications&lt;/i&gt;). | [optional] 
**Specifics** | [**ProductAddSpecificsInner[]**](ProductAddSpecificsInner.md) | An array of Item Specific Name/Value pairs used by the seller to provide descriptive details of an item in a structured manner.         The list of possible specifications can be obtained using the category.info method (additional_fields-&gt;product_specifics).         &lt;b&gt;The structure of the parameter is different for specific platforms.&lt;/b&gt; | [optional] 
**AvailFrom** | **String** | Allows to schedule a time in the future that the item becomes available. The value should be greater than the current date and time. | [optional] 
**SpriceCreate** | **String** | Defines the date of special price creation | [optional] 
**SpriceModified** | **String** | Defines the date of special price modification | [optional] 
**SpriceExpire** | **String** | Defines the term of special price offer duration | [optional] 
**CreatedAt** | **String** | Defines the date of entity creation | [optional] 
**AutoRenew** | **Boolean** | When true, automatically renews a listing upon its expiration. | [optional] [default to $false]
**WhenMade** | **String** | An enumerated string for the era in which the maker made the product. | [optional] [default to "made_to_order"]
**MetaTitle** | **String** | Defines unique meta title for each entity | [optional] 
**MetaKeywords** | **String** | Defines unique meta keywords for each entity | [optional] 
**MetaDescription** | **String** | Defines unique meta description of a entity | [optional] 
**Url** | **String** | Defines unique product&#39;s URL | [optional] 
**SeoUrl** | **String** | Defines unique URL for SEO | [optional] 
**TaxClassId** | **String** | Defines tax classes where entity has to be added | [optional] 
**Taxable** | **Boolean** | Specifies whether a tax is charged | [optional] [default to $true]
**SalesTax** | [**ProductAddSalesTax**](ProductAddSalesTax.md) |  | [optional] 
**Condition** | **String** | The human-readable label for the condition (e.g., &quot;&quot;New&quot;&quot;). | [optional] 
**ConditionDescription** | **String** | Detailed description of the product condition. | [optional] 
**AllowDisplayCondition** | **Boolean** | Flag used to determine whether the product condition is shown to the customer on the product page. | [optional] 
**PaymentMethods** | **String[]** | Identifies the payment method (such as PayPal) that the seller will accept when the buyer pays for the item. Look at cart.info method response for allowed values.&lt;hr&gt;&lt;div style&#x3D;&quot;&quot;font-style:normal&quot;&quot;&gt;Param structure:&lt;div style&#x3D;&quot;&quot;margin-left: 2%;&quot;&quot;&gt;&lt;code style&#x3D;&quot;&quot;padding:0; background-color:#ffffff;font-size:85%;font-family:monospace;&quot;&quot;&gt;payment_methods[0] &#x3D; string&lt;/br&gt;payment_methods[1] &#x3D; string&lt;/br&gt;&lt;/code&gt;&lt;/div&gt;&lt;/div&gt; | [optional] 
**PaypalEmail** | **String** | Valid PayPal email address for the PayPal account that the seller will use if they offer PayPal as a payment method for the listing. | [optional] 
**ShippingTemplateId** | **Int32** | The numeric ID of the shipping template associated with the products in Etsy. You can find possible values in the &quot;&quot;cart.info&quot;&quot; API method response, in the field shipping_zones[]-&gt;id. | [optional] [default to 0]
**ShippingDetails** | [**ProductAddShippingDetailsInner[]**](ProductAddShippingDetailsInner.md) | The shipping details, including flat and calculated shipping costs and shipping insurance costs. Look at cart.info method response for allowed values.&lt;hr&gt;&lt;div style&#x3D;&quot;&quot;font-style:normal&quot;&quot;&gt;Param structure:&lt;div style&#x3D;&quot;&quot;margin-left: 2%;&quot;&quot;&gt;&lt;code style&#x3D;&quot;&quot;padding:0; background-color:#ffffff;font-size:85%;font-family:monospace;&quot;&quot;&gt;shipping_details[0][&lt;b&gt;shipping_type&lt;/b&gt;] &#x3D; string &lt;/br&gt;shipping_details[0][&lt;b&gt;shipping_service&lt;/b&gt;] &#x3D; string&lt;/br&gt;shipping_details[0][&lt;b&gt;shipping_cost&lt;/b&gt;] &#x3D; decimal&lt;/br&gt;shipping_details[1][&lt;b&gt;shipping_type&lt;/b&gt;] &#x3D; string &lt;/br&gt;shipping_details[1][&lt;b&gt;shipping_service&lt;/b&gt;] &#x3D; string&lt;/br&gt;shipping_details[1][&lt;b&gt;shipping_cost&lt;/b&gt;] &#x3D; decimal&lt;/br&gt;&lt;/code&gt;&lt;/div&gt;&lt;/div&gt; | [optional] 
**IsFreeShipping** | **Boolean** | Specifies product&#39;s free shipping flag that has to be added | [optional] 
**DeliveryCode** | **String** | The delivery promise that applies to offer | [optional] 
**DeliveryType** | **String** | Defines the type of the delivery. | [optional] 
**DeliveryTime** | **Int32** | Defines delivery time in days. | [optional] 
**DeliveryOptionIds** | **String** | Defines delivery options for product by ids. | [optional] 
**PackageDetails** | [**ProductAddPackageDetails**](ProductAddPackageDetails.md) |  | [optional] 
**LogisticInfo** | [**ProductAddLogisticInfoInner[]**](ProductAddLogisticInfoInner.md) | Defines product&#39;s logistic channel settings | [optional] 
**ListingDuration** | **String** | Describes the number of days the seller wants the listing to be active. Look at cart.info method response for allowed values. | [optional] 
**ListingType** | **String** | Indicates the selling format of the marketplace listing. | [optional] [default to "FixedPrice"]
**CategoryType** | **String** | Specifies the type of category (e.g., apparel or other) for the product being added. | [optional] 
**ReturnAccepted** | **Boolean** | Indicates whether the seller allows the buyer to return the item. | [optional] 
**SellerProfiles** | [**ProductAddSellerProfiles**](ProductAddSellerProfiles.md) |  | [optional] 
**AuctionConfidentialityLevel** | **String** | This allows buyers to remain anonymous when the bid or buy an item. | [optional] 
**BestOffer** | [**ProductAddBestOffer**](ProductAddBestOffer.md) |  | [optional] 
**ProductionPartnerIds** | **String** | Defines product&#39;s production partner ids that has to be added | [optional] 
**MarketplaceItemProperties** | **String** | String containing the JSON representation of the supplied data | [optional] 
**ClearCache** | **Boolean** | Is cache clear required | [optional] [default to $true]
**ViewedCount** | **Int32** | Specifies the number of product&#39;s reviews | [optional] [default to 0]
**OrderedCount** | **Int32** | Defines how many times the product was ordered | [optional] [default to 0]
**ShopSectionId** | **Int32** | Add Shop Section Id | [optional] 
**ReturnPolicyId** | **Int32** | Add Return Policy Id | [optional] 
**PersonalizationDetails** | [**ProductAddPersonalizationDetails**](ProductAddPersonalizationDetails.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductAdd = Initialize-PSOpenAPIToolsProductAdd  -Name Bag `
 -Model bag_01 `
 -Description Product description `
 -Price 99.9 `
 -Sku bag_01 `
 -ShortDescription Short description. This is very short description `
 -Type configurable `
 -Status disabled `
 -Visible search `
 -CategoryId 6 `
 -CategoriesIds 23,56 `
 -ProductClass Shirts `
 -ProductType BICYCLE `
 -IsVirtual false `
 -Downloadable true `
 -IsSupply false `
 -AvailableForView false `
 -AvailableForSale false `
 -StoreId 1 `
 -StoresIds 1,2 `
 -LangId 3 `
 -OldPrice 99.9 `
 -SpecialPrice 56.9 `
 -WholesalePrice 56.12 `
 -CostPrice 65.9 `
 -FixedCostShippingPrice 5.5 `
 -TierPrices null `
 -GroupPrices null `
 -BuyitnowPrice 65.9 `
 -ReservePrice 65.9 `
 -Quantity 6 `
 -InStock true `
 -ManageStock false `
 -WarehouseId 1 `
 -BackorderStatus true `
 -MinOrderQuantity 1 `
 -MaxOrderQuantity 1 `
 -Weight 23.69 `
 -WeightUnit lb `
 -Width 56.12 `
 -Height 56.12 `
 -Length 56.12 `
 -DimensionsUnit cm `
 -Barcode 9770317847001 `
 -Upc 9770317847001 `
 -Ean 5901234123457 `
 -Isbn 9783161484100 `
 -Gtin 12345678912345 `
 -Mpn 9770317847001 `
 -Asin 97703178470 `
 -ProductReference 5901234123457 `
 -HarmonizedSystemCode 123456 `
 -CountryOfOrigin 123456 `
 -Manufacturer Samsung `
 -ManufacturerId 1 `
 -ManufacturerInfo null `
 -BrandName Abidas `
 -ImageUrl https://docs.api2cart.com/img/logo.png `
 -ImageName abibas.png `
 -AdditionalImageUrls null `
 -Files null `
 -SizeChart null `
 -RelatedProductsIds 4,5 `
 -UpSellProductsIds 4,5 `
 -CrossSellProductsIds 4,5 `
 -AttributeSetName Shoes `
 -AttributeName Color,Manufacturer `
 -SearchKeywords key1,key2,key3 `
 -Tags tag1,tag2 `
 -Materials materials[0]&#x3D;Aluminum&amp;materials[1]&#x3D;Brass `
 -Certifications null `
 -Specifics null `
 -AvailFrom avail_from&#x3D;2029-10-25T15:54:37-0500 `
 -SpriceCreate 2018-08-25 23:56:12 `
 -SpriceModified 2018-12-05 13:46:20 `
 -SpriceExpire 2018-08-25 23:56:12 `
 -CreatedAt 2014-08-09 13:13:13 `
 -AutoRenew false `
 -WhenMade 2020_2025 `
 -MetaTitle category,test `
 -MetaKeywords category,test `
 -MetaDescription category,test `
 -Url /product_slug `
 -SeoUrl some seo url `
 -TaxClassId 9 `
 -Taxable false `
 -SalesTax null `
 -Condition Like New `
 -ConditionDescription Almost perfect condition, a few scratches `
 -AllowDisplayCondition false `
 -PaymentMethods payment_methods[0]&#x3D;CashOnPickup&amp;payment_methods[1]&#x3D;PayPal `
 -PaypalEmail paypall@mail.com `
 -ShippingTemplateId 40256592690 `
 -ShippingDetails null `
 -IsFreeShipping true `
 -DeliveryCode 24uurs-23 `
 -DeliveryType PARCEL `
 -DeliveryTime 1 `
 -DeliveryOptionIds 6956548250505111111,6956548250505111112 `
 -PackageDetails null `
 -LogisticInfo null `
 -ListingDuration Days_3 `
 -ListingType Auction `
 -CategoryType Apparel `
 -ReturnAccepted true `
 -SellerProfiles null `
 -AuctionConfidentialityLevel public `
 -BestOffer null `
 -ProductionPartnerIds 4,5 `
 -MarketplaceItemProperties {&quot;color&quot;:[&quot;Silver&quot;],&quot;manufacturer&quot;:&quot;Philips&quot;,&quot;features&quot;:[&quot;3 way&quot;],&quot;countPerPack&quot;:1,&quot;watts&quot;:{&quot;unit&quot;:&quot;W&quot;,&quot;measure&quot;:40}} `
 -ClearCache false `
 -ViewedCount 9 `
 -OrderedCount 15 `
 -ShopSectionId &#x60;12345678&#x60; `
 -ReturnPolicyId &#x60;12345678&#x60; `
 -PersonalizationDetails null
```

- Convert the resource to JSON
```powershell
$ProductAdd | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

