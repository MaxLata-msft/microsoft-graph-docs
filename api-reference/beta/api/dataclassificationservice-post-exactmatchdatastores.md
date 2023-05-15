---
title: "Create exactMatchDataStore"
description: "Create a new exactMatchDataStore object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: apiPageType
---

# Create exactMatchDataStore
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [exactMatchDataStore](../resources/exactmatchdatastore.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /dataClassification/exactMatchDataStores
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [exactMatchDataStore](../resources/exactmatchdatastore.md) object.

You can specify the following properties when creating an **exactMatchDataStore**.

**TODO: Remove properties that don't apply**
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description** Inherited from [exactMatchDataStoreBase](../resources/exactmatchdatastorebase.md). Optional.|
|description|String|**TODO: Add Description** Inherited from [exactMatchDataStoreBase](../resources/exactmatchdatastorebase.md). Optional.|
|dataLastUpdatedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [exactMatchDataStoreBase](../resources/exactmatchdatastorebase.md). Optional.|
|columns|[exactDataMatchStoreColumn](../resources/exactdatamatchstorecolumn.md) collection|**TODO: Add Description** Inherited from [exactMatchDataStoreBase](../resources/exactmatchdatastorebase.md). Optional.|
|maximumNumberOfTokens|Int32|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `201 Created` response code and an [exactMatchDataStore](../resources/exactmatchdatastore.md) object in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "create_exactmatchdatastore_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/dataClassification/exactMatchDataStores
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.exactMatchDataStore",
  "displayName": "String",
  "description": "String",
  "dataLastUpdatedDateTime": "String (timestamp)",
  "columns": [
    {
      "@odata.type": "microsoft.graph.exactDataMatchStoreColumn"
    }
  ],
  "maximumNumberOfTokens": "Integer"
}
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.exactMatchDataStore"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.exactMatchDataStore",
  "id": "5ec21fc8-3698-8092-eb34-2db7995bb80f",
  "displayName": "String",
  "description": "String",
  "dataLastUpdatedDateTime": "String (timestamp)",
  "columns": [
    {
      "@odata.type": "microsoft.graph.exactDataMatchStoreColumn"
    }
  ],
  "maximumNumberOfTokens": "Integer"
}
```

