#Script Structure

## Introduction 

In here we will take a look at the different fields sent back on the [`/api/scripts`](/scripts.md) endpoint.

## Example

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

## Analysis

### id

This field simply represents the **script's ID**. This is what you need to send if you want to get the data though `/api/script`.

```json
"id": 1
```

### name

This field simply represents the **script's ID**. This is what you need to send if you want to get the data though `/api/script`.