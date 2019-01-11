---
title: Ressourcentyp bookingReminder
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: 1f1708d4ac9606ad5c862cb9b1bc73e1ddcfec4a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853865"
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
