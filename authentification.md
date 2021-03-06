# Authentication Endpoint

## /api/auth

### Introduction

This endpoint is where you can authenticate. This will create a session so you will need to **save the returned cookie**.

Once authenticated you will be able to access the following endpoints: **auth/logout, contribute, vote.**

### Request

####POST REQUEST

Parameters(**Body not Header**):
 - **email**
 - **password** (hashed --> sha256)
 - **stats** (can be null)
 - **finance** (can be null)
 
> **stats** represents the data to update the server statistics (Format to be defined).

>**finance** represents the data from the packet `XX` to let us keep trac of average price evolution (Format to be defined).

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

## /api/auth/logout

### Introduction

This endpoint is where you can de-authenticate. This will destroy the current session.

Once de-authenticated you will **not** be able to access the following endpoints: **auth/logout, contribute, vote.**

### Request

####POST REQUEST

Parameters(**Body not Header**):

 - None

### Response

#### Success

```json
{status:"200",message:"Logged Out Succesful"}
```
#### Failure

```json
{status:"401",message:"Logged Out Unsuccesful"}
```

___

Written by **The Falcon** alias **[ ]**.