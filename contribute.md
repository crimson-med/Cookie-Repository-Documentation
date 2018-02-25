# Contribute Endpoint

## /api/contribute

### Introduction

This endpoint is to send scripts/themes to the **Cookie Touch Repository**. This endpoint is only accessible to authenticated users.

### Request

#### POST Request

Parameters(**Body not Header**):
 - **uploadedFile**
 
> **uploadedFile** is the key to the file which should be uploaded in **.js** format.

![fileUpload](/assets/fileUpload.png)

### Response

#### Success

```json
{status:"200",message:"Upload Successful."}
```

#### Failure

```json
{status:"402",message:"An error occured please contact an administrator."}
```
___

Written by **The Falcon** alias **[ ]**.