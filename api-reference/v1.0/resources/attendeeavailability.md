---
title: Ressourcentyp „attendeeAvailability“
description: Die Verfügbarkeit eines Teilnehmers.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 63014553824b833e2e4cdfb03485fcb7962c01a0
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936248"
---
# <a name="attendeeavailability-resource-type"></a>Ressourcentyp „attendeeAvailability“

Die Verfügbarkeit eines Teilnehmers.

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
|attendee|[attendeeBase](attendeebase.md)|Die e-Mail-Adresse und den Typ des Teilnehmers – unabhängig davon, ob es sich um eine Person oder eine Ressource handelt, und ob Sie erforderlich oder optional ist, wenn es sich um eine Person handelt|
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
