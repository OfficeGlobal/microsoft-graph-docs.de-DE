---
title: Ressourcentyp „attendeeBase“
description: Der Typ eines Teilnehmers.
localization_priority: Normal
ms.openlocfilehash: d009ef6a58c63017addf8b8a1bdecc1974abbff3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878673"
---
# <a name="attendeebase-resource-type"></a>Ressourcentyp „attendeeBase“

Der Typ eines Teilnehmers.

Abgeleitet von [recipient](recipient.md).

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.recipient",
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
|type|attendeeType| Der Typ eines Teilnehmers. Die möglichen Werte sind: `required`, `optional`, `resource`. Derzeit Wenn Teilnehmer einer Person ist, [FindMeetingTimes](../api/user-findmeetingtimes.md) immer berücksichtigt die Person ist, der die `Required` Typ.|
|emailAddress|[emailAddress](emailaddress.md)|Enthält den Namen und die SMTP-Adresse des Teilnehmers.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
