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

This field simply represents the **script's name**. This is what you need to send if you want to get the data through `/api/script`. However this is not recommended as scrips are not obligated to have unique names.

```json
"name": "Test Script"
```

### version

This field simply represents the **script's version**. it should be composed of only three whole numbers seperated by a dot.

```json
"version": "1.0.0"
```

### type

This field simply represents the **script's type**. It can only have two values:

 - 1
 - 2
 
Where:
  - 1 = Script
 
  - 2 = Theme

```json
"type": 1

```

### author

This field simply represents the **script's author**. It is determined through the person that uploaded the script.

```json
"author": "The Falcon"
```

### tags

This field simply represents the **script's tags**. tags should be strings seperated by a comma. The comma will be there to implement a more complex system later.

```json
"tags": "fishing, incarnam, kamas"
```

### description

This field simply represents the **script's description**. This gives a simple explanation of what the script can do.

```json
"description": "A simple test script for incarnam."
```

### uploaded

This field simply represents the **script's uploaded  time**. This will give back the date the script was uploaded to the repository.

```json
"uploaded": "2018-02-25T06:48:00.000Z"
```

### filename

This field simply represents the **script's file name**. This will give back the file name of the script.

```json
"filename": "test.js"
```


### vote

This field simply represents the **script's  vote  level**. This number is calculated through this:

 - **Original Value** = 0

 - **Vote Up** = Original Value + 1

 - **Vote Down** = Original Value -1 

```json
"vote": 1
```
___

Written by **The Falcon** alias **[ ]**.
