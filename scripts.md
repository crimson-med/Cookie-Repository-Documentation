# Scripts Endpoint

## /api/script

### Introduction

This endpoint is to get the list of all scripts in the **Cookie Touch Repository**. This endpoint is accessible to everyone.

### Request

#### POST Request

No parameters needed.

### Response

#### Success

Returns an array of Script Structures:

 -  [Script Structure](/data-structures/script-structure.md)

> on **success** the content of the file will directly be sent back as **raw**.

#### Failure

```json
{status:"402",message:"An error occured please contact an administrator."}
```

## /api/author

### Introduction

This endpoint is to get the list of all scripts from one author in the **Cookie Touch Repository**. This endpoint is accessible to everyone.

### Request

#### POST Request

Parameters(**Body not Header**):
 - **author**
 
> **author** is the name or part of the name to search from.

### Response

#### Success

Returns an array of Script Structures:

 -  [Script Structure](/data-structures/script-structure.md)


#### Failure

```json
{status:"402",message:"An error occured please contact an administrator."}
```

## /api/search

### Introduction

This endpoint is to get the list of all scripts from a search in the **Cookie Touch Repository**. This endpoint is accessible to everyone.

### Request

#### POST Request

Parameters(**Body not Header**):
 - **search**
 
> **search** is the string or tag to search for.

### Response

#### Success

Returns an array of Script Structures:

 -  [Script Structure](/data-structures/script-structure.md)

#### Failure

```json
{status:"402",message:"An error occured please contact an administrator."}
```
___

Written by **The Falcon** alias **[ ]**.