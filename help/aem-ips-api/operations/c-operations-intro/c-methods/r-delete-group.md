---
description: Deletes a group.
seo-description: Deletes a group.
seo-title: deleteGroup
solution: Experience Manager
title: deleteGroup
topic: Scene7 Image Production System API
uuid: 84401f38-0844-40a1-bc05-beff55393c86
index: y
internal: n
snippet: y
---

# deleteGroup{#deletegroup}

Deletes a group.

 Syntax 

## Authorized User Types {#section-ebcc67723663494db0562275b1873460}

* `IpsAdmin` 
* `IpsCompanyAdmin` 
* `ImagePortalAdmin`

## Parameters {#section-42775102ec724c36ae5241eea1a00b8e}

**Input (deleteGroupParam)** 

|  Name  | Type  | Required  | Description  |
|---|---|---|---|
|  ` *`companyHandle`*`  | `xsd:string`  | Yes  | The handle to the company that belongs to the group that you want to delete.  |
|  ` *`groupHandle`*`  | `xsd:string`  | Yes  | The handle to the group that you want to delete.  |

**Output (deleteGroupParam)**

The IPS API does not return a response for this operation.

## Examples {#section-8f8501af3b3348a1b5701cf9622bf6e4}

This sample code deletes a group from a company. It requires a group handle, which you must obtain from another operation.

**Request** 

```java
<ns1:deleteGroupParam xmlns:ns1="http://www.scene7.com/IpsApi/xsd">
   <ns1:companyHandle>47</ns1:companyHandle>
   <ns1:groupHandle>241</ns1:groupHandle>
</ns1:deleteGroupParam>
```

**Response**

None. 