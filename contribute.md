# Contribute Endpoint

## /api/contribute

### Introduction

This endpoint is to send scripts/themes to the **Cookie Touch Repository**. This endpoint is only accessible to authenticated users.

### Request

#### POST Request

Parameters(**Body not Header**):
 - **uploadedFile**
 
> **uploadedFile** is the key to the file whoch should be uploaded in **.js** format.

![fileUpload](/assets/fileUpload.png)

### Response

#### Success

```json
{"title":"Cookie Touch API","version":"1.0.0.0","description":"This is the API for handling themes and scripts in Cookie Touch."}
```
> **title** returns the current title of the API.

> **version** returns the current version of the API.

> **description** returns the current description of the API.

#### Failure

If you can't contact this endpoint this means the API is offline. If this is the case please contact me or contact a member of the Admin team on discord.
___

Written by **The Falcon** alias **[ ]**.