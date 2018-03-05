# Script Endpoint

## /api/script

### Introduction

This endpoint is to get the script file from the **Cookie Touch Repository**. This endpoint is accessible to everyone.

### Request

#### POST Request

Parameters(**Body not Header**):
 - **scriptID**
 
> **scriptID** is the ID of the script to dpwnload the data from.

### Response

#### Success

```json
file output
```
> on **success** the content of the file will directly be sent back as **raw**.

#### Failure

```json
{status:"402",message:"An error occured please contact an administrator."}
```

___

Written by **The Falcon** alias **[ ]**.

