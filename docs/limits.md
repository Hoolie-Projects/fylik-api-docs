---
title: Fetch Fylik upload limits
---

# Fetch Fylik upload limits

Fylik API limits amount of uploads and max uploading file size.

## Request

To fetch upload limits, **send GET request to:**

`/limits`

## Response
You will receive JSON with limits

### Sample response:
```json
{
    "maxFileSize": 104857600, // Max uploading file size in bytes
    "maxFilesPerClient": 3 // Max amount of files to be uploaded per IP
}
```
