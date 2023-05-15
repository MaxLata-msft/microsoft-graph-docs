---
title: "exactMatchDataStore resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: resourcePageType
---

# exactMatchDataStore resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [exactMatchDataStoreBase](../resources/exactmatchdatastorebase.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List exactMatchDataStores](../api/dataclassificationservice-list-exactmatchdatastores.md)|[exactMatchDataStore](../resources/exactmatchdatastore.md) collection|Get a list of the [exactMatchDataStore](../resources/exactmatchdatastore.md) objects and their properties.|
|[Create exactMatchDataStore](../api/dataclassificationservice-post-exactmatchdatastores.md)|[exactMatchDataStore](../resources/exactmatchdatastore.md)|Create a new [exactMatchDataStore](../resources/exactmatchdatastore.md) object.|
|[Get exactMatchDataStore](../api/exactmatchdatastore-get.md)|[exactMatchDataStore](../resources/exactmatchdatastore.md)|Read the properties and relationships of an [exactMatchDataStore](../resources/exactmatchdatastore.md) object.|
|[Update exactMatchDataStore](../api/exactmatchdatastore-update.md)|[exactMatchDataStore](../resources/exactmatchdatastore.md)|Update the properties of an [exactMatchDataStore](../resources/exactmatchdatastore.md) object.|
|[Delete exactMatchDataStore](../api/dataclassificationservice-delete-exactmatchdatastores.md)|None|Delete an [exactMatchDataStore](../resources/exactmatchdatastore.md) object.|
|[lookup](../api/exactmatchdatastore-lookup.md)|String collection|**TODO: Add Description**|
|[List sessions](../api/exactmatchdatastore-list-sessions.md)|[exactMatchSession](../resources/exactmatchsession.md) collection|Get the exactMatchSession resources from the sessions navigation property.|
|[Create exactMatchSession](../api/exactmatchdatastore-post-sessions.md)|[exactMatchSession](../resources/exactmatchsession.md)|Create a new exactMatchSession object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|columns|[exactDataMatchStoreColumn](../resources/exactdatamatchstorecolumn.md) collection|**TODO: Add Description** Inherited from [exactMatchDataStoreBase](../resources/exactmatchdatastorebase.md).|
|dataLastUpdatedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [exactMatchDataStoreBase](../resources/exactmatchdatastorebase.md).|
|description|String|**TODO: Add Description** Inherited from [exactMatchDataStoreBase](../resources/exactmatchdatastorebase.md).|
|displayName|String|**TODO: Add Description** Inherited from [exactMatchDataStoreBase](../resources/exactmatchdatastorebase.md).|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|maximumNumberOfTokens|Int32|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|sessions|[exactMatchSession](../resources/exactmatchsession.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.exactMatchDataStore",
  "baseType": "microsoft.graph.exactMatchDataStoreBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exactMatchDataStore",
  "id": "String (identifier)",
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

