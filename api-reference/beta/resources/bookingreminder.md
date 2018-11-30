---
title: Ressourcentyp bookingReminder
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: f5f7b30c296433dd96ffa14a75e3f0286e8a16a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062340"
---
# <a name="bookingreminder-resource-type"></a>Ressourcentyp bookingReminder

 > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.
 
Stellt dar, wann und an eine e-Mail-Benachrichtigung gesendet.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|message|String|Die Nachricht in der Erinnerung.|
|Offset|Duration|Der Zeitraum vor dem Beginn des Termins, die die Erinnerung gesendet werden soll. Es wird im [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format angegeben.|
|recipients|String| Die Personen, die empfangen müssen die Erinnerung. Mögliche Werte sind: `allAttendees`, `staff` und `customer`.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingReminder"
}-->

```json
{
  "message": "String",
  "offset": "String (timestamp)",
  "recipients": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingReminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->