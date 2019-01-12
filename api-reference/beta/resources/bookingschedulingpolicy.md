---
title: Ressourcentyp bookingSchedulingPolicy
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 039d76b00787c9bf2e4f0bee4eb927a7628a9e76
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914637"
---
# <a name="bookingschedulingpolicy-resource-type"></a>Ressourcentyp bookingSchedulingPolicy

 > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.
 
Repräsentiert den Satz von Richtlinien, die bestimmen, wie Termine in einem Kalender Microsoft Bookings erstellt werden soll.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|allowStaffSelection|Boolescher Wert|"True" If Kunden für die Buchen eine bestimmte Person auswählen können.|
|maximumAdvance|Duration|Maximale Anzahl der Tage im voraus, die ein buchen hergestellt werden kann. Es folgt das [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format.|
|minimumLeadTime|Duration|Die minimale Zeitspanne vor dem Buchungen und-absagen vorgenommen werden müssen. Es folgt das [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format.|
|sendConfirmationsToOwner|Boolescher Wert| True, wenn das Unternehmen per e-Mail benachrichtigen, wenn ein buchen erstellt oder geändert wird. Verwenden Sie die e-Mail-Adresse in der **e-Mail** -Eigenschaft der Entität **BookingBusiness** für das Unternehmen angegeben. |
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
