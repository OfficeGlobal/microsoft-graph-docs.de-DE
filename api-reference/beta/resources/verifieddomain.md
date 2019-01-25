---
title: verifiedDomain-Ressourcentyp
description: Gibt eine Domäne für einen Mandanten an. Die **verifiedDomains**-Eigenschaft der **organization**-Entität ist eine Auflistung von VerifiedDomain.
localization_priority: Normal
ms.openlocfilehash: c13c3b3da39b762c26d637deaddafbee5da40160
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513396"
---
# <a name="verifieddomain-resource-type"></a>verifiedDomain-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Gibt eine Domäne für einen Mandanten an. Die **verifiedDomains**-Eigenschaft der [organization](organization.md)-Entität ist eine Auflistung von **VerifiedDomain**.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Funktionen|String|Zum Beispiel „Email“, „OfficeCommunicationsOnline“.|
|isDefault|Boolescher Wert|                **true**, wenn dies die Standarddomäne ist, die dem Mandanten zugeordnet ist, andernfalls **false**.            |
|isInitial|Boolean|**true**, wenn dies die ursprüngliche Domäne ist, die dem Mandanten zugeordnet ist, andernfalls **false**.|
|name|Zeichenfolge|Der Domänenname, zum Beispiel „contoso.onmicrosoft.com“|
|type|String|Z. B. „verwaltet“.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifieddomain"
}-->

```json
{
  "capabilities": "string",
  "isDefault": true,
  "isInitial": true,
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/verifieddomain.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
