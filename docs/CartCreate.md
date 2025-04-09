# CartCreate
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CartId** | **String** | Store’s identifier which you can get from cart_list method | 
**StoreUrl** | **String** | A web address of a store that you would like to connect to API2Cart | [optional] 
**BridgeUrl** | **String** | This parameter allows to set up store with custom bridge url (also you must use store_root parameter if a bridge folder is not in the root folder of the store) | [optional] 
**StoreRoot** | **String** | Absolute path to the store root directory (used with &quot;&quot;bridge_url&quot;&quot; parameter) | [optional] 
**StoreKey** | **String** | Set this parameter if bridge is already uploaded to store | [optional] 
**SharedSecret** | **String** | Shared secret | [optional] 
**ValidateVersion** | **Boolean** | Specify if api2cart should validate cart version | [optional] [default to $false]
**Verify** | **Boolean** | Enables or disables cart&#39;s verification | [optional] [default to $true]
**DbTablesPrefix** | **String** | DB tables prefix | [optional] 
**UserAgent** | **String** | This parameter allows you to set your custom user agent, which will be used in requests to the store. Please use it cautiously, as the store&#39;s firewall may block specific values. | [optional] 
**FtpHost** | **String** | FTP connection host | [optional] 
**FtpUser** | **String** | FTP User | [optional] 
**FtpPassword** | **String** | FTP Password | [optional] 
**FtpPort** | **Int32** | FTP Port | [optional] 
**FtpStoreDir** | **String** | FTP Store dir | [optional] 
**ApiKey3dcart** | **String** | 3DCart API Key | [optional] 
**AdminAccount** | **String** | It&#39;s a BigCommerce account for which API is enabled | [optional] 
**ApiPath** | **String** | BigCommerce API URL | [optional] 
**ApiKeyBigcommerce** | **String** | Bigcommerce API Key | [optional] 
**ClientId** | **String** | Client ID of the requesting app | [optional] 
**AccessToken** | **String** | Access token authorizing the app to access resources on behalf of a user | [optional] 
**Context** | **String** | API Path section unique to the store | [optional] 
**AccessToken** | **String** | Access token authorizing the app to access resources on behalf of a user | [optional] 
**ApiKeyShopify** | **String** | Shopify API Key | [optional] 
**ApiPassword** | **String** | Shopify API Password | [optional] 
**AccessTokenShopify** | **String** | Access token authorizing the app to access resources on behalf of a user | [optional] 
**ApiKey** | **String** | Neto API Key | [optional] 
**ApiUsername** | **String** | Neto User Name | [optional] 
**EncryptedPassword** | **String** | Volusion API Password | [optional] 
**Login** | **String** | It&#39;s a Volusion account for which API is enabled | [optional] 
**ApiUserAdnsf** | **String** | It&#39;s a AspDotNetStorefront account for which API is available | [optional] 
**ApiPass** | **String** | AspDotNetStorefront API Password | [optional] 
**PrivateKey** | **String** | 3DCart Application Private Key | [optional] 
**AppToken** | **String** | 3DCart Token from Application | [optional] 
**EtsyKeystring** | **String** | Etsy keystring | [optional] 
**EtsySharedSecret** | **String** | Etsy shared secret | [optional] 
**TokenSecret** | **String** | Secret token authorizing the app to access resources on behalf of a user | [optional] 
**EtsyClientId** | **String** | Etsy Client Id | [optional] 
**EtsyRefreshToken** | **String** | Etsy Refresh token | [optional] 
**EbayClientId** | **String** | Application ID (AppID). | [optional] 
**EbayClientSecret** | **String** | Shared Secret from eBay application | [optional] 
**EbayRuname** | **String** | The RuName value that eBay assigns to your application. | [optional] 
**EbayAccessToken** | **String** | Used to authenticate API requests. | [optional] 
**EbayRefreshToken** | **String** | Used to renew the access token. | [optional] 
**EbayEnvironment** | **String** | eBay environment | [optional] [default to "production"]
**EbaySiteId** | **Int32** | eBay global ID | [optional] [default to 0]
**DwClientId** | **String** | Demandware client id | [optional] 
**DwApiPass** | **String** | Demandware api password | [optional] 
**DemandwareUserName** | **String** | Demandware user name | [optional] 
**DemandwareUserPassword** | **String** | Demandware user password | [optional] 
**StoreId** | **String** | Store Id | 
**SellerId** | **String** | Seller Id | [optional] 
**Environment** | **String** |  | [optional] [default to "production"]
**HybrisClientId** | **String** | Omni Commerce Connector Client ID | [optional] 
**HybrisClientSecret** | **String** | Omni Commerce Connector Client Secret | [optional] 
**HybrisUsername** | **String** | User Name | [optional] 
**HybrisPassword** | **String** | User password | [optional] 
**HybrisWebsites** | [**AccountCartAddHybrisWebsitesInner[]**](AccountCartAddHybrisWebsitesInner.md) | Websites to stores mapping data | [optional] 
**WalmartClientId** | **String** | Walmart client ID. For the region &#39;ca&#39; use Consumer ID | [optional] 
**WalmartClientSecret** | **String** | Walmart client secret. For the region &#39;ca&#39; use Private Key | [optional] 
**WalmartEnvironment** | **String** | Walmart environment | [optional] [default to "production"]
**WalmartChannelType** | **String** | Walmart WM_CONSUMER.CHANNEL.TYPE header | [optional] 
**WalmartRegion** | **String** | Walmart region | [optional] [default to "us"]
**LightspeedApiKey** | **String** | LightSpeed api key | [optional] 
**LightspeedApiSecret** | **String** | LightSpeed api secret | [optional] 
**ShoplazzaAccessToken** | **String** | Access token authorizing the app to access resources on behalf of a user | [optional] 
**ShoplazzaSharedSecret** | **String** | Shared secret | [optional] 
**ShopwareAccessKey** | **String** | Shopware access key | [optional] 
**ShopwareApiKey** | **String** | Shopware api key | [optional] 
**ShopwareApiSecret** | **String** | Shopware client secret access key | [optional] 
**CommercehqApiKey** | **String** | CommerceHQ api key | [optional] 
**CommercehqApiPassword** | **String** | CommerceHQ api password | [optional] 
**Var3dcartPrivateKey** | **String** | 3DCart Private Key | [optional] 
**Var3dcartAccessToken** | **String** | 3DCart Token | [optional] 
**WcConsumerKey** | **String** | Woocommerce consumer key | [optional] 
**WcConsumerSecret** | **String** | Woocommerce consumer secret | [optional] 
**MagentoConsumerKey** | **String** | Magento Consumer Key | [optional] 
**MagentoConsumerSecret** | **String** | Magento Consumer Secret | [optional] 
**MagentoAccessToken** | **String** | Magento Access Token | [optional] 
**MagentoTokenSecret** | **String** | Magento Token Secret | [optional] 
**PrestashopWebserviceKey** | **String** | Prestashop webservice key | [optional] 
**WixAppId** | **String** | Wix App ID | 
**WixAppSecretKey** | **String** | Wix App Secret Key | 
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

## Examples

- Prepare the resource
```powershell
$CartCreate = Initialize-PSOpenAPIToolsCartCreate  -CartId Opencart14 `
 -StoreUrl http://mystore.com `
 -BridgeUrl https://your-store.com/custom/bridge/path/bridge.php `
 -StoreRoot /home/www/stores/magento1922 `
 -StoreKey ab37fc230bc5df63a5be1b11220949be `
 -SharedSecret gmz3iz45x2 `
 -ValidateVersion true `
 -Verify false `
 -DbTablesPrefix oc_ `
 -UserAgent Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:47.0) Gecko/20100101 Firefox/47.0 `
 -FtpHost ftp.mystore.com `
 -FtpUser user `
 -FtpPassword G4}q215D4_H9$Be `
 -FtpPort 22 `
 -FtpStoreDir /public `
 -ApiKey3dcart 82cc921c6a5c67082cc921c6a5c6707e1d6e6862ba3201a `
 -AdminAccount admin `
 -ApiPath http://mystore.bigcommerce.com/api/v1 `
 -ApiKeyBigcommerce 6b89704cd75738cb0f9f6468d5462aba `
 -ClientId p1r37bt131z86675nofv9xmhietoe4t `
 -AccessToken igse8e4rdmzkxdi937qe69d59en1imw `
 -Context stores/etplnf8o8v `
 -AccessToken igse8e4rdmzkxdi937qe69d59en1imw `
 -ApiKeyShopify bbca57d8ff3c3677128112c15556d9e3 `
 -ApiPassword 860f3a6fc87632301a42cd88e4b5ab3d `
 -AccessTokenShopify igse8e4rdmzkxdi937qe69d59en1imw `
 -ApiKey bbca57d8ff3c3677128112c15556d9e3 `
 -ApiUsername mylogin `
 -EncryptedPassword 7943CA5F3990E00D9A4CCF0BD998211F `
 -Login admin `
 -ApiUserAdnsf admin `
 -ApiPass f6471ef78f72b41849a8b8b67791b0b5 `
 -PrivateKey 2xo0m9ib5ty7rv84num9uic3e9mio0cy73nsdey7e5270 `
 -AppToken 82cc921c6a5c67082cc921c6a5c6707e1d6e6862ba3201a `
 -EtsyKeystring a9psel85v1wy5faeyjw03y0r `
 -EtsySharedSecret gmz3iz45x2 `
 -TokenSecret igse8e4rdmzkxdi937qe69d59en1imw `
 -EtsyClientId w0fi0igk2w29bjcd7ydr2s35 `
 -EtsyRefreshToken 223577551.L07_RE-y7unmKf2dox4djsHkVxwpUfs1ikG_uQmHhF-aASEReNn_Qns1Wqn3dDa0ZMxrt9CIael3dgudeDZb31ZUdS `
 -EbayClientId a9psel85v1wy5faeyjw03y0r `
 -EbayClientSecret gmz3iz45x2 `
 -EbayRuname gmz3iz45x2 `
 -EbayAccessToken v^1.1#i ... AjRV4yNjA&#x3D; `
 -EbayRefreshToken v^1.1#i ... rAewqVasdA&#x3D; `
 -EbayEnvironment sandbox `
 -EbaySiteId 101 `
 -DwClientId b849eb85-v8b9-1dw8-9fe2-97e1d6ffc7b0 `
 -DwApiPass testpassword `
 -DemandwareUserName admin `
 -DemandwareUserPassword 12345 `
 -StoreId 1 `
 -SellerId A9PSDFGFGHFOQD `
 -Environment sandbox `
 -HybrisClientId api_client_1 `
 -HybrisClientSecret secret_phrase_1 `
 -HybrisUsername admin `
 -HybrisPassword nimda `
 -HybrisWebsites null `
 -WalmartClientId 423f6A24-123z-8654-989u-6fa96478289 `
 -WalmartClientSecret 1gf85fea-8974-2648-w12w-rt54284tdf54 `
 -WalmartEnvironment production `
 -WalmartChannelType 0f3e4dd4-0514-4346-b39d-af0e00ea066d `
 -WalmartRegion us `
 -LightspeedApiKey cf5444729c2abd6b6a5d983691767cb5 `
 -LightspeedApiSecret 2620ee52a8bc942f9d5d3a575f4d363e `
 -ShoplazzaAccessToken igse8e4rdmzkxdi937qe69d59en1imw `
 -ShoplazzaSharedSecret gmz3iz45x2 `
 -ShopwareAccessKey SWSCS3O1RJBSRNBYQLFIYJN2ZQ `
 -ShopwareApiKey SWSCS3O1RJBSRNBYQLFIYJN2ZQ `
 -ShopwareApiSecret V3NYNWg2b1dZdHBUWDN1cmdKdGhnenp5enVJYlJ0WlJvOFF2bnQ `
 -CommercehqApiKey sJrD-LM0eddhe63rfgfva0dDydXfre4 `
 -CommercehqApiPassword 4Grr_ZCLNNoSUuhAjesKuchxo9SL `
 -Var3dcartPrivateKey 7dba81f90bdbe25e7000e73214ca51b `
 -Var3dcartAccessToken 4Grr_ZCLNNoSUuhAjesKuchxo9SL `
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
 -AllegroEnvironment sandbox
```

- Convert the resource to JSON
```powershell
$CartCreate | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

