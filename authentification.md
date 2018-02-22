# Authentication Endpoint

## /api/auth

### Introduction

This endpoint is where you can authenticate. This will create a session so you will need to **save the returned cookie**.

Once authed you will be able to access the following endpoints: **auth/logout, contribute, vote.**

### Request

####POST REQUEST

Parameters(**Body not Header**):
 - **email**
 - **password** (hashed --> sha256)
 - **stats** (can be null)
 - **finance** (can be null)

### Response

#### Success

```json
{status:"200",message:"Account Authorized"}
```
#### Failure

```json
{status:"401",message:"Account Unauthorized"}
```

___

Written by **The Falcon** alias **[ ]**.