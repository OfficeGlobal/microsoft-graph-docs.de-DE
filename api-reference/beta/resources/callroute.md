---
title: Ressourcentyp callRoute
description: Der Typ des CallRoute.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cfa470c4d3a03655221cab1f29baa60d00a8cf6c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512801"
---
# <a name="callroute-resource-type"></a>Ressourcentyp callRoute

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Der Typ des CallRoute.

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ                          | Beschreibung                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| Final               | [identitySet](identityset.md) | Die Identität, die in die Unterhaltung aufgelöst wurde.               |
| Original            | [identitySet](identityset.md) | Die Identität, die ursprünglich in den Anruf verwendet wurde.           |
| routingType         | String                        | Mögliche Werte sind: `forwarded`, `lookup` und `selfFork`.  |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRoute"
}-->
```json
{
  "final": {"@odata.type": "#microsoft.graph.identitySet"},
  "original": {"@odata.type": "#microsoft.graph.identitySet"},
  "routingType": "forwarded | lookup | selfFork"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/callroute.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
