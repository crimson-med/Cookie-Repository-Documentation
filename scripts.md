# Scripts Endpoint

## /api/script

### Introduction

This endpoint is to get the list of all scripts in the **Cookie Touch Repository**. This endpoint is accessible to everyone.

### Request

#### POST Request

No parameters needed.

### Response

#### Success

```json
{
 "id": 1,
 "name": "Test Script",
 "version": "1.0.0",
 "type": 1,
 "author": "The Falcon",
 "tags": "fishing, incarnam, kamas",
 "description": "A simple test script for incarnam.",
 "uploaded": "2018-02-25T06:48:00.000Z",
 "filename": "test.js",
 "vote": 1
}
```
> on **success** the content of the file will directly be sent back as **raw**.

#### Failure

```json
{status:"402",message:"An error occured please contact an administrator."}

___

Written by **The Falcon** alias **[ ]**.