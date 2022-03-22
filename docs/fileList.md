---
title: Fetch file list
---

# Fetch file list

## Request

To fetch actually uploaded files list, **send GET request to:**

`/files`

with parameters:

| Parameter name | Parameter description                 | Parameter type | Required |
|----------------|---------------------------------------|----------------|----------|
| offset         | File list offset (use for pagination) | integer        | false    |
| limit          | Max files in response                 | integer        | false    |

## Response
You fill receive array of files. For more details, see [File model](./fileModel)


### Sample response:
```json
[
    {
        "_id": "6238fe6533a12239d256ed0a",
        "name": "Space Cats — Magic Fly.mp4",
        "size": 9528596,
        "type": "video/mp4",
        "expiresIn": "2022-03-21T23:02:29.361Z",
        "createdAt": "2022-03-21T22:38:29.361Z"
    },
    {
        "_id": "6238fea133a12239d256ed0b",
        "name": "Y2Mate.is - TroyBoi - Afterhours (feat. Diplo & Nina Sky).mp3",
        "size": 4546605,
        "type": "audio/mpeg",
        "expiresIn": "2022-03-21T22:51:29.413Z",
        "createdAt": "2022-03-21T22:39:29.414Z"
    },
    {
        "_id": "6238ff5533a12239d256ed0c",
        "name": "Space Cats — Magic Fly.mp4",
        "size": 9528596,
        "type": "video/mp4",
        "expiresIn": "2022-03-21T23:06:29.545Z",
        "createdAt": "2022-03-21T22:42:29.545Z"
    }
]
```

### Live update
To get file list in live time, connect via WebSocket to https://socket.api.fylik.ru and get 'newFile' event
