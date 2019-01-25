---
title: Ressourcentyp bookingCustomer
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cd4991b28f1dee0ba647a7f95b70817beffbef95
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522217"
---
# <a name="bookingcustomer-resource-type"></a>Ressourcentyp bookingCustomer

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Stellt ein Kunde von einer [BookingBsiness](bookingbusiness.md)dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Liste von Kunden](../api/bookingbusiness-list-customers.md) | [BookingCustomer](bookingcustomer.md) -Auflistung | Abrufen einer Liste von **BookingCustomer** -Objekten. |
|[Erstellen von bookingCustomer](../api/bookingbusiness-post-customers.md) | [bookingCustomer](bookingcustomer.md) | Erstellen eines neuen **BookingCustomer** -Objekts. |
|[Abrufen von bookingCustomer](../api/bookingcustomer-get.md) | [bookingCustomer](bookingcustomer.md) |Lesen Sie die Eigenschaften und die Beziehungen eines **BookingCustomer** -Objekts.|
|[Update](../api/bookingcustomer-update.md) | [bookingCustomer](bookingcustomer.md) |Aktualisieren eines **BookingCustomer** -Objekts. |
|[Delete](../api/bookingcustomer-delete.md) | Keine |Löscht ein Objekt **BookingCustomer** . |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|displayName|String|Der Name des Kunden.|
|emailAddress|String|Die SMTP-Adresse des Kunden.|
|id|Zeichenfolge| Die ID des Kunden. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCustomer"
}-->

```json
{
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingCustomer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingcustomer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
