---
title: patternedRecurrence-Ressourcentyp
description: Serienmuster und -bereich.
ms.openlocfilehash: 10a90db032cd7461e28bc096fd6213df44f3ea45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017020"
---
# <a name="patternedrecurrence-resource-type"></a>patternedRecurrence-Ressourcentyp

Serienmuster und -bereich.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Muster|[RecurrencePattern](recurrencepattern.md)|Die Häufigkeit eines Ereignisses.|
|Bereich|[RecurrenceRange](recurrencerange.md)|Die Dauer eines Ereignisses.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.patternedRecurrence"
}-->

```json
{
  "pattern": {"@odata.type": "microsoft.graph.recurrencePattern"},
  "range": {"@odata.type": "microsoft.graph.recurrenceRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
