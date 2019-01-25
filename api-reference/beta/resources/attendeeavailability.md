---
title: Ressourcentyp „attendeeAvailability“
description: Typ und Verfügbarkeit eines Teilnehmers
localization_priority: Normal
ms.openlocfilehash: f831a88a14fc6ec970332208389e15a5adc49377
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508937"
---
# <a name="attendeeavailability-resource-type"></a>Ressourcentyp „attendeeAvailability“

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Typ und Verfügbarkeit eines Teilnehmers

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|attendee|[AttendeeBase](attendeebase.md)|Der Typ des Teilnehmers. Unterschieden wird zwischen Personen und Ressourcen. Bei Personen wird zusätzlich differenziert zwischen erforderlichen und optionalen Teilnehmern.|
|availability|String| Der Verfügbarkeitsstatus des Teilnehmers. Mögliche Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere` und `unknown`.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeeavailability.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
