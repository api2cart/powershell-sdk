# ProductUpdateBatch
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**NestedItemsUpdateBehaviour** | **String** |  Determines how updates to nested items should be handled.&lt;hr&gt;&lt;div style&#x3D;&quot;&quot;font-style:normal&quot;&quot;&gt;  Values description:  &lt;div style&#x3D;&quot;&quot;margin-left: 2%; padding-top: 2%&quot;&quot;&gt;    &lt;div style&#x3D;&quot;&quot;font-size:85%&quot;&quot;&gt;      &lt;b&gt;  replace&lt;/b&gt;: This option indicates that the nested items should be completely replaced with the new data provided. &lt;/br&gt;      &lt;b&gt;  merge&lt;/b&gt;: With this option, updates to nested items are merged with the existing data. &lt;/br&gt;    &lt;/div&gt;  &lt;/div&gt;&lt;/div&gt; | [optional] [default to "replace"]
**ClearCache** | **Boolean** |  | [optional] [default to $false]
**Reindex** | **Boolean** |  | [optional] [default to $false]
**Payload** | [**ProductUpdateBatchPayloadInner[]**](ProductUpdateBatchPayloadInner.md) | Contains an array of product objects. The list of properties may vary depending on the specific platform. | 

## Examples

- Prepare the resource
```powershell
$ProductUpdateBatch = Initialize-PSOpenAPIToolsProductUpdateBatch  -NestedItemsUpdateBehaviour null `
 -ClearCache null `
 -Reindex null `
 -Payload null
```

- Convert the resource to JSON
```powershell
$ProductUpdateBatch | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

