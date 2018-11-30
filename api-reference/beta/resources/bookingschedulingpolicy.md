---
title: Ressourcentyp bookingSchedulingPolicy
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: 7a16e9a2ec4e64978dd3c20f7510cfd42d76e826
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061566"
---
# <a name="bookingschedulingpolicy-resource-type"></a>Ressourcentyp bookingSchedulingPolicy

 > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.
 
Repräsentiert den Satz von Richtlinien, die bestimmen, wie Termine in einem Kalender Microsoft Bookings erstellt werden soll.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|allowStaffSelection|Boolesch|"True" If Kunden für die Buchen eine bestimmte Person auswählen können.|
|maximumAdvance|Duration|Maximale Anzahl der Tage im voraus, die ein buchen hergestellt werden kann. Es folgt das [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format.|
|minimumLeadTime|Duration|Die minimale Zeitspanne vor dem Buchungen und-absagen vorgenommen werden müssen. Es folgt das [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format.|
|sendConfirmationsToOwner|Boolesch| True, wenn das Unternehmen per e-Mail benachrichtigen, wenn ein buchen erstellt oder geändert wird. Verwenden Sie die e-Mail-Adresse in der **e-Mail** -Eigenschaft der Entität **BookingBusiness** für das Unternehmen angegeben. |
|timeSlotInterval|Duration|Dauer der jedes Zeitintervall im [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format gekennzeichnet.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingSchedulingPolicy"
}-->

```json
{
  "allowStaffSelection": true,
  "maximumAdvance": "String (timestamp)",
  "minimumLeadTime": "String (timestamp)",
  "sendConfirmationsToOwner": true,
  "timeSlotInterval": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingSchedulingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->