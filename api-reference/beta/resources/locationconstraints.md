---
title: locationConstraints-Ressourcentyp
description: Die vom Client definierten Bedingungen für den Ort einer Besprechung
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b9ac80069a7ffe61171a9e24feb2e65895c469bd
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057380"
---
# <a name="locationconstraints-resource-type"></a>locationConstraints-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die vom Client definierten Bedingungen für den Ort einer Besprechung

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationConstraints"
}-->

```json
{
  "isRequired": true,
  "locations": [{"@odata.type": "microsoft.graph.locationConstraintItem"}],
  "suggestLocation": true
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|isRequired|Boolescher Wert|Der Client fordert den Dienst auf, in der Antwort einen Besprechungsort für die Besprechung anzugeben. Ist diese Eigenschaft auf „true“ gesetzt und alle Ressourcen sind gebucht, gibt [findMeetingTimes](../api/user-findmeetingtimes.md) keine Besprechungsterminvorschläge zurück. Ist diese Eigenschaft auf „false“ gesetzt und alle Ressourcen sind gebucht, sucht **findMeetingTimes** trotzdem nach Besprechungsterminen, jedoch nicht nach Orten. |
|locations|[locationConstraintItem](locationconstraintitem.md) collection|Einschränkungsinformationen für einen oder mehrere Orte, die der Kunde für die Besprechung anfordert|
|suggestLocation|Boolean|Der Client fordert den Dienst auf, einen oder mehrere Besprechungsorte vorzuschlagen.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationConstraints resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/locationconstraints.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->