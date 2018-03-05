# Scripts Endpoint

## /api/script

### Introduction

This endpoint is to get the list of all scripts in the **Cookie Touch Repository**. This endpoint is accessible to everyone.

### Request

#### POST Request

No parameters needed.

### Response

#### Success

returns an array of Script Structures:
[
, 
Script2 Structure
]
```
> on **success** the content of the file will directly be sent back as **raw**.

#### Failure

```json
{status:"402",message:"An error occured please contact an administrator."}

___

Written by **The Falcon** alias **[ ]**.