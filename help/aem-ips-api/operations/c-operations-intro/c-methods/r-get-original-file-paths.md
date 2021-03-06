---
description: Gets the original file paths of a company’s assets.
seo-description: Gets the original file paths of a company’s assets.
seo-title: getOriginalFilePaths
solution: Experience Manager
title: getOriginalFilePaths
topic: Scene7 Image Production System API
uuid: c4acf288-1a57-4295-806b-348f15a089cc
---

# getOriginalFilePaths{#getoriginalfilepaths}

Gets the original file paths of a company’s assets.

 Syntax 

## Authorized User Types {#section-da8d8561e9174e938f3595a5d6e50089}

* `IpsUser` 
* `IpsAdmin` 
* `IpsCompanyAdmin` 
* `TrialSiteAdmin` 
* `TrialSiteUser` 
* `ImagePortalContrib` 
* `ImagePortalContribUser`

>[!NOTE]
>
>Requires read access to the asset.

## Parameters {#section-a6b394daba6e49a8882cf3051035d9d1}

**Input (getOriginalFilePathsParam)** 

|  Name  | Type  | Required  | Description  |
|---|---|---|---|
|  ` *`companyHandle`*`  | `xsd:string`  | Yes  | The handle to the company.  |
|  ` *`assetHandleArray`*`  | `types:HandleArray`  | Yes  | Array of handles to assets whose original file path you want to obtain.  |

**Output (getOriginalFilePathsReturn)** 

|  Name  | Type  | Required  | Description  |
|---|---|---|---|
|  ` *`originalFileArray`*`  | `types:StringArray`  | Yes  | The array of strings that represent the original file paths.  |

## Examples {#section-a966e783a2ba49f5b6b0f961329ab2f8}

This code sample returns the file paths of assets specified with unique asset handles in an asset handle array.

**Request** 

```java
<ns1:getOriginalFilePathsParam xmlns:ns1="http://www.scene7.com/IpsApi/xsd">
   <ns1:companyHandle>47</ns1:companyHandle>
   <ns1:assetHandleArray>
      <ns1:items>24265|1|17061</ns1:items>
      <ns1:items>24267|1|17063</ns1:items>
   </ns1:assetHandleArray>
</ns1:getOriginalFilePathsParam>
```

**Response** 

```java
<getOriginalFilePathsReturn xmlns="http://www.scene7.com/IpsApi/xsd">
   <originalFileArray>
      <items>MyCompany/Autumn Leaves.jpg</items>
      <items>MyCompany/Desert Landscape.jpg</items>
   </originalFileArray>
</getOriginalFilePathsReturn>
```

