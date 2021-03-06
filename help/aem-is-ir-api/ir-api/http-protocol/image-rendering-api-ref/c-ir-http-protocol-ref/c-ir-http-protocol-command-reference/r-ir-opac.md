---
description: Opacity. Specifies material opacity.
seo-description: Opacity. Specifies material opacity.
seo-title: opac
solution: Experience Manager
title: opac
topic: Scene7 Image Serving - Image Rendering API
uuid: 0f5b11f0-af65-4abd-947e-7a28cb8de263
---

# opac{#opac}

Opacity. Specifies material opacity.

 ` opac= *`val`*`

<table id="simpletable_6AB8CD75F526469FBC9FEAE049792EF2"> 
 <tr class="strow"> 
  <td class="stentry"> <p> <span class="varname"> val </span> </p> </td> 
  <td class="stentry"> <p>Material opacity (percent); 0…100 </p> </td> 
 </tr> 
</table>

The following material/object combinations support variable opacity:

* Solid color and repeatable textures applied to texturable overlap objects. 
* Window covering materials applied to window covering frame objects. 
* Decals applied to texturable objects or wall objects.

If the material includes an image with an alpha channel, `opac=` can be used to make the image more transparent, but not more opaque.

## Properties {#section-352f7b82ede54159b6afb90ae4b559ec}

Material attribute. Ignored if the current object selection or the material does not support opacity.

## Default {#section-bd45105b1e614f96ad5d521e3ef65736}

`opac=100`, for a fully opaque material (if the image does not include an alpha channel). 
