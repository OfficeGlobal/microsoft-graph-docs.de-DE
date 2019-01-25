---
title: plannerAssignment-Ressourcentyp
description: Die **plannerAssignment**-Ressource stellt die Zuweisung einer Aufgabe zu einem Benutzer dar. Dieser Typ wird im offenen Typ plannerAssignments verwendet.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 054cd42eedd27a7fe11abc2e5578a56da667e05d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522504"
---
# <a name="plannerassignment-resource-type"></a>plannerAssignment-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **plannerAssignment**-Ressource stellt die Zuweisung einer Aufgabe zu einem Benutzer dar. Dieser Typ wird im offenen Typ [plannerAssignments](plannerassignments.md) verwendet.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|assignedBy|[identitySet](identityset.md)|Die Identität des Benutzers, der die Zuweisung der Aufgabe durchgeführt hat, d. h. der Zuweisende.|
|assignedDateTime|DateTimeOffset|Uhrzeit, zu der die Aufgabe zugewiesen wurde. Der Zeitstempeltyp stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|orderHint|String|Hinweis, der verwendet wird, um zugewiesene Personen in einer Aufgabe anzuordnen. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignment"
}-->

```json
{
  "assignedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "assignedDateTime": "String (timestamp)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
