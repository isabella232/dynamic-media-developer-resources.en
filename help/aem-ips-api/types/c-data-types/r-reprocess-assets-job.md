---
description: Job type to allow reprocessing of previously uploaded master files, including reripping PDFs and reoptimizing images.
seo-description: Job type to allow reprocessing of previously uploaded master files, including reripping PDFs and reoptimizing images.
seo-title: ReprocessAssetsJob
solution: Experience Manager
title: ReprocessAssetsJob
topic: Scene7 Image Production System API
uuid: b31838ed-a74f-4a77-8798-d7e8b71d3f90
index: y
internal: n
snippet: y
---

# ReprocessAssetsJob{#reprocessassetsjob}

Job type to allow reprocessing of previously uploaded master files, including reripping PDFs and reoptimizing images.

 Syntax 

## Parameters {#section-2fc9bea56b6d4b72b80d4f04c5f9b862}

<table id="table_04100BB8ABD84EF68B0A7CE3AD946414"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> <p>Name </p> </th> 
   <th colname="col2" class="entry"> <p>Type </p> </th> 
   <th colname="col3" class="entry"> <p>Description </p> </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> assetHandleArray</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> types:HandleArray</span> </p> </td> 
   <td colname="col3"> <p>Asset handle. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> readyForPublish</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> xsd:boolean</span> </p> </td> 
   <td colname="col3"> <p>Whether the files are marked ready for publishing. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> preservePublishState</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> xsd:boolean</span> </p> </td> 
   <td colname="col3"> <p>Controls whether the publish state of an existing asset is preserved when overwriting. If not set, the company default setting is used. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> createMask</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> xsd:boolean</span> </p> </td> 
   <td colname="col3"> <p>Whether to create a mask. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> preserveCrop</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> xsd:boolean</span> </p> </td> 
   <td colname="col3">Controls preservation of any existing crop definition. Defaults to <span class="codeph"> true</span>. </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> manualCropOptions</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> types:ManualCropOptions</span> </p> </td> 
   <td colname="col3"> <p>Manual crop options. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> autoColorCropOptions</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> types:AutoColorCropOptions</span> </p> </td> 
   <td colname="col3"> <p>Options for automatic crops of images based on color. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> autoTransparentCropOptions</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> types:AutoTransparentCropOptions</span> </p> </td> 
   <td colname="col3"> <p>Removes white space from the edges of images, based on transparency. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> photoshopOptions</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> types:PhotoshopOptions</span> </p> </td> 
   <td colname="col3"> <p>Options for uploading Photoshop files to the Image Server. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> postScriptOptions</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> types:PostScriptOptions</span> </p> </td> 
   <td colname="col3"> <p>Options for uploading PostScript files to the Image Server. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> pdfOptions</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> types:PDFOptions</span> </p> </td> 
   <td colname="col3"> <p>Options for uploading PDF files to the Image Server. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> mediaOptions</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> types:MediaOptions</span> </p> </td> 
   <td colname="col3"> <p>A/V media file options. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> illustratorOptions</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> types:IllustratorOptions</span> </p> </td> 
   <td colname="col3"> <p>Options for uploading Illustrator files to the Image Server. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> colorManagementOptions</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> types:ColorManagementOptions</span> </p> </td> 
   <td colname="col3"> <p>Options that you can specify during an upload. The set affects how the color is managed for the upload. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> autoSetCreationOptions</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> types:AutoSetCreationOptions</span> </p> </td> 
   <td colname="col3"> <p>Array of automatic set generation scripts to apply to uploaded files. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> projectHandleArray</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> types:HandleArray</span> </p> </td> 
   <td colname="col3"> <p>An array of project handles. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> emailSetting</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> xsd:string</span> </p> </td> 
   <td colname="col3"> <p>Options for email settings. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> postJobOnlyIfFiles</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> xsd:boolean</span> </p> </td> 
   <td colname="col3"> <p>Whether to upload only files. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> postHttpUrl</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> xsd:string</span> </p> </td> 
   <td colname="col3"> <p>URL to file upload location. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> postImageServingPublishJob</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> types:ImageServingPublishJob</span> </p> </td> 
   <td colname="col3"> <p>Job details for an image serving publish job to be run after the upload is complete. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> postImageRenderingPublishJob</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> types:ImageRenderingPublishJob</span> </p> </td> 
   <td colname="col3"> <p>Job details for an image rendering publish job to be run after the upload is complete. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> postVideoPublishJob</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> types:VideoPublishJob</span> </p> </td> 
   <td colname="col3"> <p>Job details for a video publish job to be run after the upload is complete. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> inDesignOptions</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> types:InDesignOptions</span> </p> </td> 
   <td colname="col3"> <p>Options for uploading InDesign files to the image server. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> knockoutBackground</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> types:KnockoutBackgroundOptions</span> </p> </td> 
   <td colname="col3"> <p>Mask the background for selected images. This lets you overlay them in other layers with a transparency outside of subject image. </p> <p>Optional. </p> <p>See<a href="../../types/c-data-types/r-knockout-background-options.md#reference-9196371848964d91842b337640791c9c" format="dita" scope="local"> KnockoutBackgroundOptions</a> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"> <span class="varname"> unsharpMaskOptions</span> </span> </p> </td> 
   <td colname="col2"> <p><span class="codeph"> types:UnsharpMaskOptions</span> </p> </td> 
   <td colname="col3"> <p>Options that let you control unsharp mask settings when creating an optimized pyramid TIF file. Use these settings to help improve image sharpness. </p> <p>See <a href="http://microsite.omniture.com/t2/help/en_US/s7/ips_api/types/r_unsharp_mask_options.html#reference_B9A96244D7EE4424BC4AC3C23BE3BE3D"> UnsharpMaskOptions</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Notes**

Choices for `*CropOptions` include:

* `manualCropOptions` 
* `autoColorCropOptions` 
* `autoTransparentCropOptions`

Choices for `*PublishJob` include:

* `postImageServingPublishJob` 
* `postImageRenderingPublishJob` 
* `postVideoPublishJob`
