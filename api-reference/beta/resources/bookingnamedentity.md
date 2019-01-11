---
title: Ressourcentyp bookingNamedEntity
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: fa307d0ee07b43a44210fc6ceaf4c74a29999caa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860501"
---
# <a name="bookingnamedentity-resource-type"></a>Ressourcentyp bookingNamedEntity

 > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.
 
Dies ist ein Basistyp für Microsoft Bookings Entitäten, die einen Anzeigenamen ein, beispielsweise bereitstellen, [BookingBusiness](bookingbusiness.md), [BookingPerson](bookingperson.md), [BookingService](bookingservice.md).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|displayName|String|Ein Name für die abgeleitete Entität, welche mit Kunden Schnittstellen.|
|id|String| Die ID für die abgeleitete Entität. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingNamedEntity"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingNamedEntity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
