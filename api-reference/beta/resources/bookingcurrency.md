---
title: Ressourcentyp bookingCurrency
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 7e2289bfa6c6aac62f12d7321d06caaafbc41f8c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956003"
---
# <a name="bookingcurrency-resource-type"></a>Ressourcentyp bookingCurrency

 > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.
 
Stellt eine monetäre Währung, die von einem [BookingBusiness](bookingbusiness.md)unterstützt.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Liste bookingCurrencies](../api/bookingcurrency-list.md) | [BookingCurrency](bookingcurrency.md) -Auflistung |Abrufen einer Liste von **BookingCurrency** -Objekten für ein Microsoft Bookings Unternehmen verfügbar.|
|[Abrufen von bookingCurrency](../api/bookingcurrency-get.md) | [bookingCurrency](bookingcurrency.md) |Rufen Sie die Eigenschaften eines **BookingCurrency** -Objekts.|


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|Zeichenfolge| Ein 3-Zeichen Währungscode, basierend auf [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html). Beispiel für US-Dollar der Währungscode ist US-Dollar und für Australien Dollar ist AUD. Schreibgeschützt.|
|Symbol|Zeichenfolge| Das Währungssymbol. Beispielsweise ist das Währungssymbol für US-Dollar und Australien Dollar $.  |

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCurrency"
}-->

```json
{
  "id": "String (identifier)",
  "symbol": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingCurrency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
