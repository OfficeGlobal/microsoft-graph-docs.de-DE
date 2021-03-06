---
title: Ressourcentyp bookingSchedulingPolicy
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3dee3314818d46c4131526dc92565eb4f8ca6ea2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523449"
---
# <a name="bookingschedulingpolicy-resource-type"></a>Ressourcentyp bookingSchedulingPolicy

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Repräsentiert den Satz von Richtlinien, die bestimmen, wie Termine in einem Kalender Microsoft Bookings erstellt werden soll.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|allowStaffSelection|Boolescher Wert|"True" If Kunden für die Buchen eine bestimmte Person auswählen können.|
|maximumAdvance|Dauer|Maximale Anzahl der Tage im voraus, die ein buchen hergestellt werden kann. Es folgt das [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format.|
|minimumLeadTime|Dauer|Die minimale Zeitspanne vor dem Buchungen und-absagen vorgenommen werden müssen. Es folgt das [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format.|
|sendConfirmationsToOwner|Boolescher Wert| True, wenn das Unternehmen per e-Mail benachrichtigen, wenn ein buchen erstellt oder geändert wird. Verwenden Sie die e-Mail-Adresse in der **e-Mail** -Eigenschaft der Entität **BookingBusiness** für das Unternehmen angegeben. |
|timeSlotInterval|Dauer|Dauer der jedes Zeitintervall im [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format gekennzeichnet.|

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingSchedulingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingschedulingpolicy.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
