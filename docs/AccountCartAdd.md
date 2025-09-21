# AccountCartAdd
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CartId** | **String** | Store’s identifier which you can get from cart_list method | 
**StoreUrl** | **String** | A web address of a store that you would like to connect to API2Cart | [optional] 
**BridgeUrl** | **String** | This parameter allows to set up store with custom bridge url (also you must use store_root parameter if a bridge folder is not in the root folder of the store) | [optional] 
**StoreRoot** | **String** | Absolute path to the store root directory (used with &quot;&quot;bridge_url&quot;&quot; parameter) | [optional] 
**StoreKey** | **String** | Set this parameter if bridge is already uploaded to store | [optional] 
**ValidateVersion** | **Boolean** | Specify if api2cart should validate cart version | [optional] [default to $false]
**Verify** | **Boolean** | Enables or disables cart&#39;s verification | [optional] [default to $true]
**DbTablesPrefix** | **String** | DB tables prefix | [optional] 
**UserAgent** | **String** | This parameter allows you to set your custom user agent, which will be used in requests to the store. Please use it cautiously, as the store&#39;s firewall may block specific values. | [optional] 
**FtpHost** | **String** | FTP connection host | [optional] 
**FtpUser** | **String** | FTP User | [optional] 
**FtpPassword** | **String** | FTP Password | [optional] 
**FtpPort** | **Int32** | FTP Port | [optional] 
**FtpStoreDir** | **String** | FTP Store dir | [optional] 
**Var3dcartPrivateKey** | **String** | 3DCart Private Key | [optional] 
**Var3dcartAccessToken** | **String** | 3DCart Token | [optional] 
**Var3dcartapiApiKey** | **String** | 3DCart API Key | [optional] 
**AmazonSpClientId** | **String** | Amazon SP API app client id | [optional] 
**AmazonSpClientSecret** | **String** | Amazon SP API app client secret | [optional] 
**AmazonSpRefreshToken** | **String** | Amazon SP API OAuth refresh token | [optional] 
**AmazonSpAwsRegion** | **String** | Amazon AWS Region | [optional] 
**AmazonSpApiEnvironment** | **String** | Amazon SP API environment | [optional] [default to "production"]
**AmazonSellerId** | **String** | Amazon Seller ID (Merchant token) | [optional] 
**AspdotnetstorefrontApiUser** | **String** | It&#39;s a AspDotNetStorefront account for which API is available | [optional] 
**AspdotnetstorefrontApiPass** | **String** | AspDotNetStorefront API Password | [optional] 
**BigcommerceapiAdminAccount** | **String** | It&#39;s a BigCommerce account for which API is enabled | [optional] 
**BigcommerceapiApiPath** | **String** | BigCommerce API URL | [optional] 
**BigcommerceapiApiKey** | **String** | Bigcommerce API Key | [optional] 
**BigcommerceapiClientId** | **String** | Client ID of the requesting app | [optional] 
**BigcommerceapiAccessToken** | **String** | Access token authorizing the app to access resources on behalf of a user | [optional] 
**BigcommerceapiContext** | **String** | API Path section unique to the store | [optional] 
**BolApiKey** | **String** | Bol API Key | [optional] 
**BolApiSecret** | **String** | Bol API Secret | [optional] 
**BolRetailerId** | **Int32** | Bol Retailer ID | [optional] 
**BigcartelUserName** | **String** | Subdomain of store | [optional] 
**BigcartelPassword** | **String** | BigCartel account password | [optional] 
**BricklinkConsumerKey** | **String** | Bricklink Consumer Key | [optional] 
**BricklinkConsumerSecret** | **String** | Bricklink Consumer Secret | [optional] 
**BricklinkToken** | **String** | Bricklink Access Token | [optional] 
**BricklinkTokenSecret** | **String** | Bricklink Access Token Secret | [optional] 
**DemandwareClientId** | **String** | Demandware client id | [optional] 
**DemandwareApiPassword** | **String** | Demandware api password | [optional] 
**DemandwareUserName** | **String** | Demandware user name | [optional] 
**DemandwareUserPassword** | **String** | Demandware user password | [optional] 
**EbayClientId** | **String** | Application ID (AppID). | [optional] 
**EbayClientSecret** | **String** | Shared Secret from eBay application | [optional] 
**EbayRuname** | **String** | The RuName value that eBay assigns to your application. | [optional] 
**EbayAccessToken** | **String** | Used to authenticate API requests. | [optional] 
**EbayRefreshToken** | **String** | Used to renew the access token. | [optional] 
**EbayEnvironment** | **String** | eBay environment | [optional] [default to "production"]
**EbaySiteId** | **Int32** | eBay global ID | [optional] [default to 0]
**WalmartClientId** | **String** | Walmart client ID. For the region &#39;ca&#39; use Consumer ID | [optional] 
**WalmartClientSecret** | **String** | Walmart client secret. For the region &#39;ca&#39; use Private Key | [optional] 
**WalmartEnvironment** | **String** | Walmart environment | [optional] [default to "production"]
**WalmartChannelType** | **String** | Walmart WM_CONSUMER.CHANNEL.TYPE header | [optional] 
**WalmartRegion** | **String** | Walmart region | [optional] [default to "us"]
**EcwidAcessToken** | **String** | Access token authorizing the app to access resources on behalf of a user | [optional] 
**EcwidStoreId** | **String** | Store Id | [optional] 
**LazadaAppId** | **String** | Lazada App ID | [optional] 
**LazadaAppSecret** | **String** | Lazada App Secret | [optional] 
**LazadaRefreshToken** | **String** | Lazada Refresh Token | [optional] 
**LazadaRegion** | **String** | Lazada API endpoint Region | [optional] 
**LightspeedApiKey** | **String** | LightSpeed api key | [optional] 
**LightspeedApiSecret** | **String** | LightSpeed api secret | [optional] 
**EtsyKeystring** | **String** | Etsy keystring | [optional] 
**EtsySharedSecret** | **String** | Etsy shared secret | [optional] 
**EtsyAccessToken** | **String** | Access token authorizing the app to access resources on behalf of a user | [optional] 
**EtsyTokenSecret** | **String** | Secret token authorizing the app to access resources on behalf of a user | [optional] 
**EtsyClientId** | **String** | Etsy Client Id | [optional] 
**EtsyRefreshToken** | **String** | Etsy Refresh token | [optional] 
**FacebookAppId** | **String** | Facebook App ID | [optional] 
**FacebookAppSecret** | **String** | Facebook App Secret | [optional] 
**FacebookAccessToken** | **String** | Facebook Access Token | [optional] 
**FacebookBusinessId** | **String** | Facebook Business ID | [optional] 
**NetoApiKey** | **String** | Neto API Key | [optional] 
**NetoApiUsername** | **String** | Neto User Name | [optional] 
**ShoplineAccessToken** | **String** | Shopline APP Key | [optional] 
**ShoplineAppKey** | **String** | Shopline APP Key | [optional] 
**ShoplineAppSecret** | **String** | Shopline App Secret | [optional] 
**ShoplineSharedSecret** | **String** | Shopline Shared Secret | [optional] 
**ShopifyAccessToken** | **String** | Access token authorizing the app to access resources on behalf of a user | [optional] 
**ShopifyApiKey** | **String** | Shopify API Key | [optional] 
**ShopifyApiPassword** | **String** | Shopify API Password | [optional] 
**ShopifySharedSecret** | **String** | Shared secret | [optional] 
**ShopeePartnerId** | **String** | Shopee Partner ID | [optional] 
**ShopeePartnerKey** | **String** | Shopee Partner Key | [optional] 
**ShopeeShopId** | **String** | Shopee SHOP ID | [optional] 
**ShopeeRefreshToken** | **String** | Shopee Refresh Token | [optional] 
**ShopeeRegion** | **String** | Shopee API endpoint Region. Use for Chinese Mainland or Brazil. | [optional] 
**ShopeeEnvironment** | **String** | Shopee Environment | [optional] [default to "production"]
**ShoplazzaAccessToken** | **String** | Access token authorizing the app to access resources on behalf of a user | [optional] 
**ShoplazzaSharedSecret** | **String** | Shared secret | [optional] 
**ShopwareAccessKey** | **String** | Shopware access key | [optional] 
**UnasApiKey** | **String** | UNAS API Key | [optional] 
**ShopwareApiKey** | **String** | Shopware api key | [optional] 
**ShopwareApiSecret** | **String** | Shopware client secret access key | [optional] 
**MivaAccessToken** | **String** | Miva access token | [optional] 
**MivaSignature** | **String** | Miva signature | [optional] 
**TiendanubeUserId** | **Int32** | Tiendanube User ID | [optional] 
**TiendanubeAccessToken** | **String** | Tiendanube Access Token | [optional] 
**TiendanubeClientSecret** | **String** | Tiendanube Client Secret | [optional] 
**VolusionLogin** | **String** | It&#39;s a Volusion account for which API is enabled | [optional] 
**VolusionPassword** | **String** | Volusion API Password | [optional] 
**HybrisClientId** | **String** | Omni Commerce Connector Client ID | [optional] 
**HybrisClientSecret** | **String** | Omni Commerce Connector Client Secret | [optional] 
**HybrisUsername** | **String** | User Name | [optional] 
**HybrisPassword** | **String** | User password | [optional] 
**HybrisWebsites** | [**AccountCartAddHybrisWebsitesInner[]**](AccountCartAddHybrisWebsitesInner.md) | Websites to stores mapping data | [optional] 
**SquareClientId** | **String** | Square (Weebly) Client ID | [optional] 
**SquareClientSecret** | **String** | Square (Weebly) Client Secret | [optional] 
**SquareRefreshToken** | **String** | Square (Weebly) Refresh Token | [optional] 
**SquarespaceApiKey** | **String** | Squarespace API Key | [optional] 
**SquarespaceClientId** | **String** | Squarespace Connector Client ID | [optional] 
**SquarespaceClientSecret** | **String** | Squarespace Connector Client Secret | [optional] 
**SquarespaceAccessToken** | **String** | Squarespace access token | [optional] 
**SquarespaceRefreshToken** | **String** | Squarespace refresh token | [optional] 
**CommercehqApiKey** | **String** | CommerceHQ api key | [optional] 
**CommercehqApiPassword** | **String** | CommerceHQ api password | [optional] 
**WcConsumerKey** | **String** | Woocommerce consumer key | [optional] 
**WcConsumerSecret** | **String** | Woocommerce consumer secret | [optional] 
**MagentoConsumerKey** | **String** | Magento Consumer Key | [optional] 
**MagentoConsumerSecret** | **String** | Magento Consumer Secret | [optional] 
**MagentoAccessToken** | **String** | Magento Access Token | [optional] 
**MagentoTokenSecret** | **String** | Magento Token Secret | [optional] 
**PrestashopWebserviceKey** | **String** | Prestashop webservice key | [optional] 
**WixAppId** | **String** | Wix App ID | [optional] 
**WixAppSecretKey** | **String** | Wix App Secret Key | [optional] 
**WixInstanceId** | **String** | Wix Instance ID | [optional] 
**WixRefreshToken** | **String** | Wix refresh token | [optional] 
**MercadoLibreAppId** | **String** | Mercado Libre App ID | [optional] 
**MercadoLibreAppSecretKey** | **String** | Mercado Libre App Secret Key | [optional] 
**MercadoLibreRefreshToken** | **String** | Mercado Libre Refresh Token | [optional] 
**ZidClientId** | **Int32** | Zid Client ID | [optional] 
**ZidClientSecret** | **String** | Zid Client Secret | [optional] 
**ZidAccessToken** | **String** | Zid Access Token | [optional] 
**ZidAuthorization** | **String** | Zid Authorization | [optional] 
**ZidRefreshToken** | **String** | Zid refresh token | [optional] 
**FlipkartClientId** | **String** | Flipkart Client ID | [optional] 
**FlipkartClientSecret** | **String** | Flipkart Client Secret | [optional] 
**AllegroClientId** | **String** | Allegro Client ID | [optional] 
**AllegroClientSecret** | **String** | Allegro Client Secret | [optional] 
**AllegroAccessToken** | **String** | Allegro Access Token | [optional] 
**AllegroRefreshToken** | **String** | Allegro Refresh Token | [optional] 
**AllegroEnvironment** | **String** | Allegro Environment | [optional] [default to "production"]
**ZohoClientId** | **String** | Zoho Client ID | [optional] 
**ZohoClientSecret** | **String** | Zoho Client Secret | [optional] 
**ZohoRefreshToken** | **String** | Zoho Refresh Token | [optional] 
**ZohoRegion** | **String** | Zoho API endpoint Region | [optional] 
**OttoClientId** | **String** | Otto Client ID | [optional] 
**OttoClientSecret** | **String** | Otto Client Secret | [optional] 
**OttoAppId** | **String** | Otto App ID | [optional] 
**OttoRefreshToken** | **String** | Otto Refresh Token | [optional] 
**OttoEnvironment** | **String** | Otto Environment | [optional] [default to "production"]
**OttoAccessToken** | **String** | Otto Access Token | [optional] 
**TiktokshopAppKey** | **String** | TikTok Shop App Key | [optional] 
**TiktokshopAppSecret** | **String** | TikTok Shop App Secret | [optional] 
**TiktokshopRefreshToken** | **String** | TikTok Shop Refresh Token | [optional] 
**TiktokshopAccessToken** | **String** | TikTok Shop Access Token | [optional] 
**SallaClientId** | **String** | Salla Client ID | [optional] 
**SallaClientSecret** | **String** | Salla Client Secret | [optional] 
**SallaRefreshToken** | **String** | Salla Refresh Token | [optional] 
**SallaAccessToken** | **String** | Salla Access Token | [optional] 
**TemuAppKey** | **String** | Temu App Key | [optional] 
**TemuAppSecret** | **String** | Temu App Secret | [optional] 
**TemuAccessToken** | **String** | Temu Access Token | [optional] 
**TemuRegion** | **String** | Temu API endpoint Region. | [optional] 

## Examples

- Prepare the resource
```powershell
$AccountCartAdd = Initialize-PSOpenAPIToolsAccountCartAdd  -CartId Opencart14 `
 -StoreUrl http://mystore.com `
 -BridgeUrl https://your-store.com/custom/bridge/path/bridge.php `
 -StoreRoot /home/www/stores/magento1922 `
 -StoreKey ab37fc230bc5df63a5be1b11220949be `
 -ValidateVersion true `
 -Verify false `
 -DbTablesPrefix oc_ `
 -UserAgent Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:47.0) Gecko/20100101 Firefox/47.0 `
 -FtpHost ftp.mystore.com `
 -FtpUser user `
 -FtpPassword G4}q215D4_H9$Be `
 -FtpPort 22 `
 -FtpStoreDir /public `
 -Var3dcartPrivateKey 7dba81f90bdbe25e7000e73214ca51b `
 -Var3dcartAccessToken 4Grr_ZCLNNoSUuhAjesKuchxo9SL `
 -Var3dcartapiApiKey 82cc921c6a5c67082cc921c6a5c6707e1d6e6862ba3201a `
 -AmazonSpClientId amzn1.application-oa2-client.11e000e1f47d4998aca3733716d3b5a4 `
 -AmazonSpClientSecret 2c987428209f235443221255bde064f4bdf8a65165a80f5d22760a83cb `
 -AmazonSpRefreshToken Atzr|IwEBIPUI-bwRTdDgKNQ_g56C30wGqymtx30c9MdDC7Emwmojhs20k5BBG2hHtJiGZ_7OfG7khd1RuQr6KEst4qyWbo_eXi5S_T_VOxzJUuksG1cFOGFpFK-cnhReNzAeZIpZeJT7_ROy1csEFlQfC8FJS3bsbSkkbTz2ZcTN7_7ey0HVlhyfFizgROeSeOI24Wjs9l_KKzZW0jvi_oC2cxlIcyknnHLK6KMNz2rTXqQJWRtlK9xPJDdbcUa5STA8MQru91cxNBpSkZN_cq9OOELhbsIGKD75y7nZ3yJU4uHQC_9iBQQoFm0biKgi-kEQwOhwws8 `
 -AmazonSpAwsRegion us-east-1 `
 -AmazonSpApiEnvironment sandbox `
 -AmazonSellerId 13P636B2M1N4WR `
 -AspdotnetstorefrontApiUser admin `
 -AspdotnetstorefrontApiPass f6471ef78f72b41849a8b8b67791b0b5 `
 -BigcommerceapiAdminAccount admin `
 -BigcommerceapiApiPath http://mystore.bigcommerce.com/api/v1 `
 -BigcommerceapiApiKey 6b89704cd75738cb0f9f6468d5462aba `
 -BigcommerceapiClientId p1r37bt131z86675nofv9xmhietoe4t `
 -BigcommerceapiAccessToken igse8e4rdmzkxdi937qe69d59en1imw `
 -BigcommerceapiContext stores/etplnf8o8v `
 -BolApiKey 51369628-feee-11ed-be56-0242ac120002 `
 -BolApiSecret 8fGzEsbEP5z2MNZubmIil87m-sWzTkj?KDQKrmzmU!fA6aAUNMdKRp7LMWHwE!G37UMfnWByHBGSXJHkAG?QcuYTO2uklv4idIHwUMLHK!OO1yfRlWh! `
 -BolRetailerId 145001 `
 -BigcartelUserName subdomain `
 -BigcartelPassword 4GrrZCLNNoSUuhAjesKuchxo9SL `
 -BricklinkConsumerKey 26F6CDA087D9444EAA71AC09E7A1D39A `
 -BricklinkConsumerSecret a46abc3kxyinlbggy06i9g975xqo6gjq `
 -BricklinkToken ktv4n9rgrj0evjuy2t6p2xlb1f8u5pmy `
 -BricklinkTokenSecret a46abc3kxyinlbggy06i9g975xqo6gjq `
 -DemandwareClientId b849eb85-v8b9-1dw8-9fe2-97e1d6ffc7b0 `
 -DemandwareApiPassword testpassword `
 -DemandwareUserName admin `
 -DemandwareUserPassword 12345 `
 -EbayClientId a9psel85v1wy5faeyjw03y0r `
 -EbayClientSecret gmz3iz45x2 `
 -EbayRuname gmz3iz45x2 `
 -EbayAccessToken v^1.1#i ... AjRV4yNjA&#x3D; `
 -EbayRefreshToken v^1.1#i ... rAewqVasdA&#x3D; `
 -EbayEnvironment sandbox `
 -EbaySiteId 101 `
 -WalmartClientId 423f6A24-123z-8654-989u-6fa96478289 `
 -WalmartClientSecret 1gf85fea-8974-2648-w12w-rt54284tdf54 `
 -WalmartEnvironment production `
 -WalmartChannelType 0f3e4dd4-0514-4346-b39d-af0e00ea066d `
 -WalmartRegion us `
 -EcwidAcessToken igse8e4rdmzkxdi937qe69d59en1imw `
 -EcwidStoreId 1 `
 -LazadaAppId 112577 `
 -LazadaAppSecret er33raICJ79Q5b0EsR9stmRnjE9XQ2WH `
 -LazadaRefreshToken EAAPP06rM2n8BO4mZBuMPnu9zS0MaMbN7ue8aUkcxw4zewU337mVVb5br `
 -LazadaRegion Malaysia `
 -LightspeedApiKey cf5444729c2abd6b6a5d983691767cb5 `
 -LightspeedApiSecret 2620ee52a8bc942f9d5d3a575f4d363e `
 -EtsyKeystring a9psel85v1wy5faeyjw03y0r `
 -EtsySharedSecret gmz3iz45x2 `
 -EtsyAccessToken igse8e4rdmzkxdi937qe69d59en1imw `
 -EtsyTokenSecret igse8e4rdmzkxdi937qe69d59en1imw `
 -EtsyClientId w0fi0igk2w29bjcd7ydr2s35 `
 -EtsyRefreshToken 223577551.L07_RE-y7unmKf2dox4djsHkVxwpUfs1ikG_uQmHhF-aASEReNn_Qns1Wqn3dDa0ZMxrt9CIael3dgudeDZb31ZUdS `
 -FacebookAppId 6516912365277570 `
 -FacebookAppSecret 737cf6bd2879cb6c7e5a8ff9cd63f3d46b0b5b7b `
 -FacebookAccessToken EAAPP06rM2n8BO4mZBuMPnu9zS0MaMbN7ue8aUAhqbS58clzJwyp1rYRMpP31QJGziqtYbKypdVx3Cs0RpuufoUeLsbfX195XIB8VTlkcxw4zewU337mVVb5br `
 -FacebookBusinessId 294042786906655 `
 -NetoApiKey bbca57d8ff3c3677128112c15556d9e3 `
 -NetoApiUsername mylogin `
 -ShoplineAccessToken igse8e4rdmzkxdi937qe69d59en1imw `
 -ShoplineAppKey 737cf6bd2879cb6c7e5a8ff9cd63f3d46b0b5b7b `
 -ShoplineAppSecret 1701d123bb5cc14cd2732dcaed90638316c0a09 `
 -ShoplineSharedSecret 1701d123bb5cc14cd2732dcaed90638316c0a09 `
 -ShopifyAccessToken igse8e4rdmzkxdi937qe69d59en1imw `
 -ShopifyApiKey bbca57d8ff3c3677128112c15556d9e3 `
 -ShopifyApiPassword 860f3a6fc87632301a42cd88e4b5ab3d `
 -ShopifySharedSecret gmz3iz45x2 `
 -ShopeePartnerId 1276777 `
 -ShopeePartnerKey 6a46494b4d746576554646626775617a577542774850636375464d6a736d5598 `
 -ShopeeShopId 137968 `
 -ShopeeRefreshToken EAAPP06rM2n8BO4mZBuMPnu9zS0MaMbN7ue8aUkcxw4zewU987mVVb5br `
 -ShopeeRegion CN `
 -ShopeeEnvironment sandbox `
 -ShoplazzaAccessToken igse8e4rdmzkxdi937qe69d59en1imw `
 -ShoplazzaSharedSecret gmz3iz45x2 `
 -ShopwareAccessKey SWSCS3O1RJBSRNBYQLFIYJN2ZQ `
 -UnasApiKey c238908e29ceb6e6ad3df15f89a6234709d3f000 `
 -ShopwareApiKey SWSCS3O1RJBSRNBYQLFIYJN2ZQ `
 -ShopwareApiSecret V3NYNWg2b1dZdHBUWDN1cmdKdGhnenp5enVJYlJ0WlJvOFF2bnQ `
 -MivaAccessToken 227cbe434a1e358d72db0de993x9d9fd `
 -MivaSignature 1hpkrebfdsObGTor/0Gk9XcNBUQohrxrw67Sg9AM9ps&#x3D; `
 -TiendanubeUserId 1234 `
 -TiendanubeAccessToken 75bde7bb0b437475423e7e87c142c06052f80199 `
 -TiendanubeClientSecret 5e3588f514a5ae0d0fa063d1b556531e25c83fa7e47472ed `
 -VolusionLogin admin `
 -VolusionPassword 7943CA5F3990E00D9A4CCF0BD998211F `
 -HybrisClientId api_client_1 `
 -HybrisClientSecret secret_phrase_1 `
 -HybrisUsername admin `
 -HybrisPassword nimda `
 -HybrisWebsites null `
 -SquareClientId sq0idp-qwer_1pvuTYe9cAf1lmxyQ `
 -SquareClientSecret c8d7077fce7b2b111111111898170695a01473a2ad `
 -SquareRefreshToken EQAAlquVXMr6xIcPu7qPkIEAZ0thqChhQuowrvZIqOlwhOwhtmyh4ZRfesdRc434 `
 -SquarespaceApiKey 8f7849d5-1411-47f2-9722-aa81c2a48d95 `
 -SquarespaceClientId 9UGbUtS2V96BxRGmfOjsGAhTdsr9Vxxx `
 -SquarespaceClientSecret GPZkUFkIKWg0KLE6rajsFMMYA9ma0udaaq2bYwBDXXX&#x3D; `
 -SquarespaceAccessToken SWSCS3O1RJBSRNBYQLFIYJN2ZQ `
 -SquarespaceRefreshToken def50eyfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe657e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65de64a0c865d `
 -CommercehqApiKey sJrD-LM0eddhe63rfgfva0dDydXfre4 `
 -CommercehqApiPassword 4Grr_ZCLNNoSUuhAjesKuchxo9SL `
 -WcConsumerKey ck_26d8e2ad604f3917e429df6961722282bdcf109d `
 -WcConsumerSecret cs_931ced666118a15c5f7b4a33a15gf5589cbeba55 `
 -MagentoConsumerKey ktv4n9rgrj0evjuy2t6p2xlb1f8u5pmy `
 -MagentoConsumerSecret a46abc3kxyinlbggy06i9g975xqo6gjq `
 -MagentoAccessToken igse8e4rdmzkxdi937qe69d59en1imw `
 -MagentoTokenSecret igse8e4rdmzkxdi937qe69d59en1imw `
 -PrestashopWebserviceKey CKJ1ZEWRJWRLTPVBQJ9FGGRORD4AGS96 `
 -WixAppId 6b0b5b7b-7d87-45b5-bf34-ac6b438e63da `
 -WixAppSecretKey 316c0a09-f195-42be-74f6-a02cebb9cae6 `
 -WixInstanceId 58b893a4-6b16-5c2f-qt78-qa3r61t32rt8 `
 -WixRefreshToken 
        OAUTH2.eyJraWQiOiJkZ0x3cjNRMCIsImFsZyI6IkhTMjU2In0.
        eyJkYXRhIjoie1wiaWRcIjpcImJlZjM3MmRmLTUyNGItNDI3NS05M2RkL
        Tg4NDBlOTU3ZWU2OFwifSIsImlhdCI6MTY0ODA0NTEyNiwiZXhwIjoxNzExMTE3MTI2fQ.
        VRR2lGSbcTVmaArtmyyhy6o4WRDwTn-nlDCQpZ97eYw
       `
 -MercadoLibreAppId 211188015100135 `
 -MercadoLibreAppSecretKey e2qoG2zklLlfP7cEngEJ94YjhkejkjAm `
 -MercadoLibreRefreshToken TG-63h13529vb5464110188d2x9-703754376 `
 -ZidClientId 1234 `
 -ZidClientSecret nl5l1lE0vxgv6cV111fHsdlOOIfb0Ms5IR7l4Igs `
 -ZidAccessToken def50eyfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe657e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65de64a0c865d `
 -ZidAuthorization def50eyfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe657e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65de64a0c865d `
 -ZidRefreshToken def50eyfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe657e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65de64a0c865d `
 -FlipkartClientId 19414773883a13a850b6a52350b7246499a24 `
 -FlipkartClientSecret nl5l1lE0vxgv6cV111fHsdlOOIfb0Ms5IR7l4Igs `
 -AllegroClientId 2915e189ce3d23d23d2327d204ae6a0bd `
 -AllegroClientSecret DNHtqdL2WPIefeUhQWYgtXPS23fgbfgasdsGHHJGhg3RTFDQWFGZmVoFRT5IfkQj1E7eR5 `
 -AllegroAccessToken eyJhbGciOiJSUzI1NiIsInR5cCI6IsfddfdfdeyJ1c2VyX25hbWUiOiI5NDUxMzE1MSIsInNjb3BlIjpbImFsbGVncm86YXBpOm9yZGVyczpyZWFkIiwiYWxsZWdybzphcGk6cHJvZmlsZTp3cml0ZSIsImFsbGVncm86YXBpOnNhbGU6b2ZmZXJzOndyaXRlIiwiYWxsZWdybzphcGk6YmlsbGluZzpyZWFkIiwiYWxsZWdybzphcGk6Y2FtcGFpZ25zIiwiYWxsZWdybzphcGk6ZGlzcHV0ZXMiLCJhbGxlZ3JvOmFwaTpzYWxlOm9mZmVyczpyZWFkIiwiYWxsZWdybzphcGk6YmlkcyIsImFsbGVncm86YXBpOm9yZGVyczp3cml0ZSIsImFsbGVncm86YXBpOnBheW1lbnRzOndyaXRlIiwiYWxsZWdybzphcGk6c2FsZTpzZXR0aW5nczp3cml0ZSIsImFsbGVncm86YXBpOnByb2ZpbGU6cmVhZCIsImFsbGVncm86YXBpOnJhdGluZ3MiLCJhbGxlZ3JvOmFwaTpzYWxlOnNldHRpbmdzOnJlYWQiLCJhbGxlZ3JvOmFwaTpwYXltZW50czpyZWFkIiwiYWxsZWdybzphcGk6bWVzc2FnaW5nIl0sI `
 -AllegroRefreshToken eyJhbGciOiJSUzI1NiIsInR5cCI6IsfddfdfdeyJ1c2VyX25hbWUiOiI5NDUxMzE1MSIsInNjb3BlIjpbImFsbGVncm86YXBpOm9yZGVyczpyZWFkIiwiYWxsZWdybzphcGk6cHJvZmlsZTp3cml0ZSIsImFsbGVncm86YXBpOnNhbGU6b2ZmZXJzOndyaXRlIiwiYWxsZWdybzphcGk6YmlsbGluZzpyZWFkIiwiYWxsZWdybzphcGk6Y2FtcGFpZ25zIiwiYWxsZWdybzphcGk6ZGlzcHV0ZXMiLCJhbGxlZ3JvOmFwaTpzYWxlOm9mZmVyczpyZWFkIiwiYWxsZWdybzphcGk6YmlkcyIsImFsbGVncm86YXBpOm9yZGVyczp3cml0ZSIsImFsbGVncm86YXBpOnBheW1lbnRzOndyaXRlIiwiYWxsZWdybzphcGk6c2FsZTpzZXR0aW5nczp3cml0ZSIsImFsbGVncm86YXBpOnByb2ZpbGU6cmVhZCIsImFsbGVncm86YXBpOnJhdGluZ3MiLCJhbGxlZ3JvOmFwaTpzYWxlOnNldHRpbmdzOnJlYWQiLCJhbGxlZ3JvOmFwaTpwYXltZW50czpyZWFkIiwiYWxsZWdybzphcGk6bWVzc2FnaW5nIl0sI `
 -AllegroEnvironment sandbox `
 -ZohoClientId 1000.FLCHGI2LS1111111TOR4OGB697W4IX `
 -ZohoClientSecret c8d7077fce7b2b111111111898170695a01473a2ad `
 -ZohoRefreshToken 1000.11111111111111111111111111111111.1b3ca6f054341a111118abf928beb33b `
 -ZohoRegion Europe `
 -OttoClientId 911a3dbf-d261-4763-cc81-052876465b55 `
 -OttoClientSecret 9887a82a-2879-421e-a6wc-54e986b3458c `
 -OttoAppId 6eaef6a3-822e-425b-8mc9-53750063e34d `
 -OttoRefreshToken eyJhbGciOiJSUzI1NiIsInR5cCI6IsfddfdfdeyJ1c2VyX25hbWUiOiI5NDUxMzE1MSIsInNjb3BlIjpbImFsbGVncm86YXBpOm9yZGVyczpyZWFkIiwiYWxsZWdybzphcGk6cHJvZmlsZTp3cml0ZSIsImFsbGVncm86YXBpOnNhbGU6b2ZmZXJzOndyaXRlIiwiYWxsZWdybzphcGk6YmlsbGluZzpyZWFkIiwiYWxsZWdybzphcGk6Y2FtcGFpZ25zIiwiYWxsZWdybzphcGk6ZGlzcHV0ZXMiLCJhbGxlZ3JvOmFwaTpzYWxlOm9mZmVyczpyZWFkIiwiYWxsZWdybzphcGk6YmlkcyIsImFsbGVncm86YXBpOm9yZGVyczp3cml0ZSIsImFsbGVncm86YXBpOnBheW1lbnRzOndyaXRlIiwiYWxsZWdybzphcGk6c2FsZTpzZXR0aW5nczp3cml0ZSIsImFsbGVncm86YXBpOnByb2ZpbGU6cmVhZCIsImFsbGVncm86YXBpOnJhdGluZ3MiLCJhbGxlZ3JvOmFwaTpzYWxlOnNldHRpbmdzOnJlYWQiLCJhbGxlZ3JvOmFwaTpwYXltZW50czpyZWFkIiwiYWxsZWdybzphcGk6bWVzc2FnaW5nIl0sI `
 -OttoEnvironment sandbox `
 -OttoAccessToken eyJhbGciOiJS34535f45f54f5656deyJ1c2VyX25hbWUiOiI5NDUxMzE1MSIsInNjb3BlIjpbImFsbGVncm86YXBpOm9yZGVyczpyZWFkIiwiYWxsZWdybzphcGk6cHJvZmlsZTp3cml0ZSIsImFsbGVncm86YXBpOnNhbGU6b2ZmZXJzOndyaXRlIiwiYWxsZWdybzphcGk6YmlsbGluZzpyZWFkIiwiYWxsZWdybzphcGk6Y2FtcGFpZ25zIiwiYWxsZWdybzphcGk6ZGlzcHV0ZXMiLCJhbGxlZ3JvOmFwaTpzYWxlOm9mZmVyczpyZWFkIiwiYWxsZWdybzphcGk6YmlkcyIsImFsbGVncm86YXBpOm9yZGVyczp3cml0ZSIsImFsbGVncm86YXBpOnBheW1lbnRzOndyaXRlIiwiYWxsZWdybzphcGk6c2FsZTpzZXR0aW5nczp3cml0ZSIsImFsbGVncm86YXBpOnByb2ZpbGU6cmVhZCIsImFsbGVncm86YXBpOnJhdGluZ3MiLCJhbGxlZ3JvOmFwaTpzYWxlOnNldHRpbmdzOnJlYWQiLCJhbGxlZ3JvOmFwaTpwYXltZW50czpyZWFkIiwiYWxsZWdybzphcGk6bWVzc2FnaW5nIl0sI `
 -TiktokshopAppKey 6arbhkzno8nbv `
 -TiktokshopAppSecret d95820a05a0cd54fb394fcd26fgat63999b183bc `
 -TiktokshopRefreshToken TTP_NTUxZTNhYTQ2ZDk2YmRmZWNmYWY2YWY12345NGYwNjQ3YjkzYTllYjA0YmNlMw `
 -TiktokshopAccessToken TTP_Fw8r12345kW03FYd09DG-9INtpw361hWthei12345iPJ5AUv99fLSCYD9-Uu12345TgNRzKZxi5-tfFMtdWqglEt5_iCk `
 -SallaClientId 1bxxxcf9-5xx4-xxx-bxxf-929b8xxxxe11 `
 -SallaClientSecret 8x88axxxc25e1fxxxa1c06fxxx150xx5 `
 -SallaRefreshToken oxy_rt_zxxxxiY2xxZWWxxxxlU-tROxxxxx2JzS2fwzxxxxxkU.p3xxxkCIyFexxxxP50WwZYfhw5_wg1xxxxV5F-8xxXc `
 -SallaAccessToken oxy_rt_zxxxxiY2xxZWWxxxxlU-tROxxxxx2JzS2fwzxxxxxkU.p3xxxkCIyFexxxxP50WwZYfhw5_wg1xxxxV5F-8xxXc `
 -TemuAppKey 4ebbc9190ae410443d65b4c2faca9811 `
 -TemuAppSecret 4782d2d827276688bf4758bed55dbdd4bbe79a78 `
 -TemuAccessToken uplv3hfyt5kcwoymrgnajnbl1ow5qxlz4sqhev6hl3xosz5dejrtyl2jre6 `
 -TemuRegion US
```

- Convert the resource to JSON
```powershell
$AccountCartAdd | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

