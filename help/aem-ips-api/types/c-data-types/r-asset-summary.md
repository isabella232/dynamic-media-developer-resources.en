---
description: Metadata search results that contain summarized information about an asset.
seo-description: Metadata search results that contain summarized information about an asset.
seo-title: AssetSummary
solution: Experience Manager
title: AssetSummary
topic: Scene7 Image Production System API
uuid: 24c0d152-5e46-4051-867b-045e89eb5c38
index: y
internal: n
snippet: y
---

# AssetSummary{#assetsummary}

Metadata search results that contain summarized information about an asset.

 Syntax 

## Parameters {#section-ebc75cc024d94c439260d2e71873cc74}

|  Name  | Type  | Description  |
|---|---|---|
|  ` *`assetHandle`*`  | `xsd:string`  | Asset handle.  |
|  ` *`type`*`  | `xsd:string`  | Asset type. The "Asset Types" constant defines the possible values. Optional.  |
|  ` *`name`*`  | `xsd:string`  | Asset name. Optional.  |
|  ` *`folder`*`  | `xsd:string`  | The folder that contains the asset.  |
|  ` *`filename`*`  | `xsd:string`  | Asset's file name.  |
|  ` *`created`*`  | `xsd:dateTime`  | Asset creation date.  |
|  ` *`createUser`*`  | `xsd:string`  | The user who created the asset.  |
|  ` *`lastModified`*`  | `xsd:dateTime`  | The date that the asset was last updated.  |
|  ` *`lastModifyUser`*`  | `xsd:string`  | The last user who modified the asset.  |
|  ` *`metadataArray`*`  | `types:MetadataArray`  | Array of metadata values associated with the asset.  |
|  ` *`score`*`  | `xsd:double`  | Defines the precision in case of a similarity search (0 = no match, 1 = exact match).  |
|  ` *`scoreDetail`*`  | `xsd:string`  | Holds detailed information about similar areas as a result of a similarity search.  |
