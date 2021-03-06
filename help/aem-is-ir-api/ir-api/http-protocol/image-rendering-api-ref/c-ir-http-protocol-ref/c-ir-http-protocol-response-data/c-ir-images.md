---
description: Image data is returned if a request successfully completes, and if the request either does not include a req= command, or if req= has one of the following values  img, debug
seo-description: Image data is returned if a request successfully completes, and if the request either does not include a req= command, or if req= has one of the following values  img, debug
seo-title: Images
solution: Experience Manager
title: Images
topic: Scene7 Image Serving - Image Rendering API
uuid: 8e8c5ec9-dc15-4894-b6a1-8e5241f03977
---

# Images{#images}

Image data is returned if a request successfully completes, and if the request either does not include a req= command, or if req= has one of the following values: img, debug

The HTTP response MIME type is determined by `fmt=`, or, if `fmt=` is not specified, it depends on the value of `attribute::Format`.

The HTTP response status is '200 OK' if the request method was an unconditional `GET` or `HEAD`.

The server may reply with status '304' (not modified) and not return any image data in response to a conditional `GET` request (with the [!DNL If-Modified-Since] field present in the `request-header`). 
