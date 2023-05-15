---
title: "Create exactMatchSession"
description: "Create a new exactMatchSession object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: apiPageType
---

# Create exactMatchSession
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new exactMatchSession object.

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
POST /dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [exactMatchSession](../resources/exactmatchsession.md) object.

You can specify the following properties when creating an **exactMatchSession**.

**TODO: Remove properties that don't apply**
|Property|Type|Description|
|:---|:---|:---|
|creationDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md). Optional.|
|startDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md). Optional.|
|lastUpdatedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md). Optional.|
|completionDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md). Optional.|
|error|[classificationError](../resources/classificationerror.md)|**TODO: Add Description** Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md). Optional.|
|dataStoreId|String|**TODO: Add Description** Inherited from [exactMatchSessionBase](../resources/exactmatchsessionbase.md). Optional.|
|remainingBlockCount|Int32|**TODO: Add Description** Inherited from [exactMatchSessionBase](../resources/exactmatchsessionbase.md). Optional.|
|totalBlockCount|Int32|**TODO: Add Description** Inherited from [exactMatchSessionBase](../resources/exactmatchsessionbase.md). Optional.|
|state|String|**TODO: Add Description** Inherited from [exactMatchSessionBase](../resources/exactmatchsessionbase.md). Optional.|
|uploadCompletionDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [exactMatchSessionBase](../resources/exactmatchsessionbase.md). Optional.|
|processingCompletionDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [exactMatchSessionBase](../resources/exactmatchsessionbase.md). Optional.|
|totalJobCount|Int32|**TODO: Add Description** Inherited from [exactMatchSessionBase](../resources/exactmatchsessionbase.md). Optional.|
|remainingJobCount|Int32|**TODO: Add Description** Inherited from [exactMatchSessionBase](../resources/exactmatchsessionbase.md). Optional.|
|uploadAgentId|String|**TODO: Add Description** Optional.|
|fields|String collection|**TODO: Add Description** Optional.|
|fileName|String|**TODO: Add Description** Optional.|
|checksum|String|**TODO: Add Description** Optional.|
|dataUploadURI|String|**TODO: Add Description** Optional.|
|rowsPerBlock|Int32|**TODO: Add Description** Optional.|
|salt|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `201 Created` response code and an [exactMatchSession](../resources/exactmatchsession.md) object in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "create_exactmatchsession_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.exactMatchSession",
  "creationDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "completionDateTime": "String (timestamp)",
  "error": {
    "@odata.type": "microsoft.graph.classificationError"
  },
  "dataStoreId": "String",
  "remainingBlockCount": "Integer",
  "totalBlockCount": "Integer",
  "state": "String",
  "uploadCompletionDateTime": "String (timestamp)",
  "processingCompletionDateTime": "String (timestamp)",
  "totalJobCount": "Integer",
  "remainingJobCount": "Integer",
  "uploadAgentId": "String",
  "fields": [
    "String"
  ],
  "fileName": "String",
  "checksum": "String",
  "dataUploadURI": "String",
  "rowsPerBlock": "Integer",
  "salt": "String"
}
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.exactMatchSession"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.exactMatchSession",
  "id": "ab8cf3ab-36b0-b07a-e010-dfbc942fe48b",
  "creationDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "completionDateTime": "String (timestamp)",
  "error": {
    "@odata.type": "microsoft.graph.classificationError"
  },
  "dataStoreId": "String",
  "remainingBlockCount": "Integer",
  "totalBlockCount": "Integer",
  "state": "String",
  "uploadCompletionDateTime": "String (timestamp)",
  "processingCompletionDateTime": "String (timestamp)",
  "totalJobCount": "Integer",
  "remainingJobCount": "Integer",
  "uploadAgentId": "String",
  "fields": [
    "String"
  ],
  "fileName": "String",
  "checksum": "String",
  "dataUploadURI": "String",
  "rowsPerBlock": "Integer",
  "salt": "String"
}
```

