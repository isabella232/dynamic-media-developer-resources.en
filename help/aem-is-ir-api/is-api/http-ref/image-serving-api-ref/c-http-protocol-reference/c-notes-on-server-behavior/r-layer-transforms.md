---
description: Transforms are applied to source images and text layers.
seo-description: Transforms are applied to source images and text layers.
seo-title: Layer transforms
solution: Experience Manager
title: Layer transforms
topic: Scene7 Image Serving - Image Rendering API
uuid: b32b5af4-66ad-474a-9bca-4b6da8f43bf9
---

# Layer transforms{#layer-transforms}

Transforms are applied to source images and text layers.

The following operations are applied to source images, in the given order, to achieve the desired spatial relationship with layer 0:

1. Apply `crop=`, if specified. 
1. Scale based on `size=` or, if `size=` is not specified, based on `scale=`, or, if `scale=` is not specified, based on `res=`, or, if `res=`is not specified, use the full resolution source image. 
1. Apply `flip=`, if specified. 
1. Apply `rotate=`, if specified. 
1. Apply `extend=`, if specified. 
1. Position the layer in the canvas based on `origin=` and `pos=` (see below).

The following transforms are applied to text layers:

1. The text box size is determined by `size=`, or the text width and height, if `size=` is only partially or not at all provided. The text is aligned within the text box using the rtf text alignment attributes. Text may be cropped by the text box. 
1. Scale the text content based on the resolution specified with `textAttr=`. 
1. Apply `rotate=`, if specified. 
1. Apply `extend=`, if specified. 
1. Position the layer in the canvas based on `origin=` and `pos=`(see below).

For both image and text layers, the last step-positioning the layer in the canvas-does not apply to layer 0, since layer 0 effectively constitutes the canvas. 
