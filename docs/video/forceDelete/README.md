---
title: Video Force Delete
---

<Block>

# Video Force Delete Endpoint

The video force delete endpoint hard deletes a video and returns a confirmation message.

For example, the `/api/forceDelete/video/Bakemonogatari-OP1.webm` endpoint will hard delete the Bakemonogatari-OP1.webm video and return a confirmation message.

## URL

```sh
DELETE /api/forceDelete/video/{basename}
```

## Authentication

**Required Permission**: force delete video

**Roles with Permission**: Admin

## Parameters

None

## Response

```json
{
    message: "The Video 'Bakemonogatari-OP1.webm' was deleted.",
}
```

<Example>

<CURL>
```bash
curl -X DELETE -H "Authorization: Bearer {token}" https://api.animethemes.moe/forceDelete/video/Bakemonogatari-OP1.webm
```
</CURL>

</Example>

</Block>