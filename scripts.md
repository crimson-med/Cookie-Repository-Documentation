# Scripts Endpoint

## /api/script

### Introduction

This endpoint is to get the script file from the **Cookie Touch Repository**. This endpoint is accessible to everyon.

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

#### Wrong File Type

```json
{status:"400",message:"Wrong file type please make sure to upload .js"}
```

___

Written by **The Falcon** alias **[ ]**.