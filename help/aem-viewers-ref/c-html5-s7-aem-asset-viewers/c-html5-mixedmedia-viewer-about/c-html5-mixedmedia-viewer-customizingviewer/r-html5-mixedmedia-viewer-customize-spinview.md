---
description: Main view consists of the spin image when the current asset is a spin set.
seo-description: Main view consists of the spin image when the current asset is a spin set.
seo-title: Spin view
solution: Experience Manager
title: Spin view
topic: Dynamic media
uuid: f1edbcc4-966a-4ec6-8ba9-a76f3ae51733
---

# Spin view{#spin-view}

Main view consists of the spin image when the current asset is a spin set.

<!--<a id="section_061E550C1C1D4DB2BD663A898895B38C"></a>-->

**CSS properties of the main viewer area**

The appearance of the viewing area is controlled with the following CSS class selector:

```
.s7mixedmediaviewer .s7spinview
```

<table id="table_94EE3F5BBE4547C0B4943471CEE7EDE4"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> <p> CSS property </p> </th> 
   <th colname="col2" class="entry"> <p>Description </p> </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> background-color </span> </p> </td> 
   <td colname="col2"> <p> Background color in hexadecimal format of the spin view. </p> </td> 
  </tr> 
 </tbody> 
</table>

Example - to make the spin view transparent.

```
.s7mixedmediaviewer .s7spinview { 
 background-color: transparent; 
}
```

