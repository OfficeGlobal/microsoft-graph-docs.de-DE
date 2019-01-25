---
title: Ressourcentyp „attendeeBase“
description: Der Typ eines Teilnehmers.
localization_priority: Normal
ms.openlocfilehash: bce1550c107f2114d02744091b5863360ab0bcea
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517456"
---
# <a name="attendeebase-resource-type"></a>Ressourcentyp „attendeeBase“

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Der Typ eines Teilnehmers.

Abgeleitet von [recipient](recipient.md).

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|type|String| Der Typ eines Teilnehmers. Mögliche Werte sind: `required`, `optional` und `resource`. Ist der Teilnehmer eine Person, geht [findMeetingTimes](../api/user-findmeetingtimes.md) aktuell grundsätzlich davon aus, dass diese Person vom Typ `Required` ist.|
|emailAddress|[emailAddress](emailaddress.md)|Enthält den Namen und die SMTP-Adresse des Teilnehmers.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeebase.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
