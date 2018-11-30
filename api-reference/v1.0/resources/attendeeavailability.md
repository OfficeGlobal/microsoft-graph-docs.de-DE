---
title: Ressourcentyp „attendeeAvailability“
description: Typ und Verfügbarkeit eines Teilnehmers
ms.openlocfilehash: 446dfb77d8f85021f41795038c3c1d597c6f1a6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016839"
---
# <a name="attendeeavailability-resource-type"></a>Ressourcentyp „attendeeAvailability“

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
|availability|freeBusyStatus| Der Verfügbarkeitsstatus des Teilnehmers. Die möglichen Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
