---
title: Ressourcentyp bookingCurrency
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 9d4feac66e72c756173113101a88bf8bbe35563a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518198"
---
# <a name="bookingcurrency-resource-type"></a>Ressourcentyp bookingCurrency

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Stellt eine monetäre Währung, die von einem [BookingBusiness](bookingbusiness.md)unterstützt.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Liste bookingCurrencies](../api/bookingcurrency-list.md) | [BookingCurrency](bookingcurrency.md) -Auflistung |Abrufen einer Liste von **BookingCurrency** -Objekten für ein Microsoft Bookings Unternehmen verfügbar.|
|[Abrufen von bookingCurrency](../api/bookingcurrency-get.md) | [bookingCurrency](bookingcurrency.md) |Rufen Sie die Eigenschaften eines **BookingCurrency** -Objekts.|


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Ein 3-Zeichen Währungscode, basierend auf [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html). Beispiel für US-Dollar der Währungscode ist US-Dollar und für Australien Dollar ist AUD. Schreibgeschützt.|
|Symbol|String| Das Währungssymbol. Beispielsweise ist das Währungssymbol für US-Dollar und Australien Dollar $.  |

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingCurrency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingcurrency.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
