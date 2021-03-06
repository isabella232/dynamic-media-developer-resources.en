---
description: For internal use only. See the Image Rendering Material Catalog Reference–Catalog Attributes section.
seo-description: For internal use only. See the Image Rendering Material Catalog Reference–Catalog Attributes section.
seo-title: getImageRenderingPublishSettings
solution: Experience Manager
title: getImageRenderingPublishSettings
topic: Scene7 Image Production System API
uuid: b1c253b5-febe-4dc7-95a1-a5f4789030e7
---

# getImageRenderingPublishSettings{#getimagerenderingpublishsettings}

For internal use only. See the Image Rendering Material Catalog Reference–Catalog Attributes section.

Syntax 

## Authorized User Types {#section-1097e0563c61480a8e97822dc3527070}

* `IpsAdmin` 
* `IpsCompanyAdmin` 
* `TrialSiteAdmin` 
* `ImagePortalAdmin`

## Parameters {#section-4f2cb8c589384816bb2525654ec49963}

**Input (getImageRenderingPublishSettingsParam)** 

|  Name  | Type  | Required  | Description  |
|---|---|---|---|
|  ` *`companyHandle`*`  | `xsd:string`  | Yes  | The handle to the company whose image rendering publishing settings you wish to get.  |
|  ` *`contextHandle`*`  | `xsd:string`  | Yes  | Handle to the publish context.  |

**Output (getImageRenderingPublishSettingsReturn)** 

|  Name  | Type  | Required  | Description  |
|---|---|---|---|
|  ` *`publishSettingsArray`*`  | `type:ConfigSettingArray`  | Yes  | Image rendering publishing settings.  |

