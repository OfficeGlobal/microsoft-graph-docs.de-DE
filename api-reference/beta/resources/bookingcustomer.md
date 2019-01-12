---
title: Ressourcentyp bookingCustomer
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: b213e4026ee33886c0e56db9790efff09fd8c522
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925105"
---
# <a name="bookingcustomer-resource-type"></a>Ressourcentyp bookingCustomer

 > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.
 
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
|displayName|Zeichenfolge|Der Name des Kunden.|
|emailAddress|Zeichenfolge|Die SMTP-Adresse des Kunden.|
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
<!-- {
  "type": "#page.annotation",
  "description": "bookingCustomer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
