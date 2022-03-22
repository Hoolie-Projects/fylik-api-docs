---
title: File upload
---

# File upload

## Request

To upload a file, **send POST request to*

`/upload`

with your file as `file` field.

## Response
You fill file object like [File model](./fileModel)


### Sample response:
```json
{
    "_id": "6238fe6533a12239d256ed0a",
    "name": "Space Cats — Magic Fly.mp4",
    "size": 9528596,
    "type": "video/mp4",
    "expiresIn": "2022-03-21T23:02:29.361Z",
    "createdAt": "2022-03-21T22:38:29.361Z"
}
```

## See also
 - [Upload limits](/limits)
