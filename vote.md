# Vote Endpoint

## /api/vote

### Introduction

This endpoint is where a authenticated user can vote for a script.

The vote system is a simple **up/down system**. It is limited to only **one vote** per user.

### Request

####POST REQUEST

Parameters(**Body not Header**):
 - **script**
 - **vote**
 
> **script** represents the id of the script (integer).

> **vote** represents the value **up** or **down** (string).

**PS: There is no need to specify the user voting as this endpoint is only accessible after authentication.**

### Response

#### Success

```json
{status:"200",message:"Account Authorized"}
```
#### Failure

```json
{status:"401",message:"Account Unauthorized"}
```

#### Already Voted

```json
{status:"400",message:"You have already voted."}
```
___

Written by **The Falcon** alias **[ ]**.