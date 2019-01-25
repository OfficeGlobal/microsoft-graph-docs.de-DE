---
title: Ressourcentyp governanceSubject
description: Stellt Benutzern, Gruppen und Service-Prinzipale in privilegierten Identity Management (PIM) verwaltet werden.
localization_priority: Normal
ms.openlocfilehash: a83825a147429c81b3e83b2f2fb384672d2f527e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519164"
---
# <a name="governancesubject-resource-type"></a>Ressourcentyp governanceSubject

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt Benutzern, Gruppen und Service-Prinzipale in privilegierten Identity Management (PIM) verwaltet werden.


## <a name="properties"></a>Eigenschaften
| Eigenschaft  | Typ       |Beschreibung|
|:----------|:----------|:----------|
|id         |string     | Die Id des Betreffs.|
|type       |String     |Der Typ des Betreffs. Der Wert kann sein ``User``, ``Group``, und ``ServicePrincipal``.|
|displayName|Zeichenfolge     |Der Anzeigename des Betreffs.|
|E-Mail      |Zeichenfolge     |Die e-Mail-Adresse des Betreffs Benutzer. Wenn der Betreff in anderen Typen ist, ist leer.|
|principalName|String   |Den Prinzipalnamen des Benutzers Betreff. Wenn der Betreff in anderen Typen ist, ist leer.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSubject"
}-->

```json
{
  "id": "String",  
  "displayName": "String",
  "email": "String",
  "principalName": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancesubject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
