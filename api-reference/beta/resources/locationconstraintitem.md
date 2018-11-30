---
title: Ressourcentyp „locationConstraintItem“
description: Die vom Client definierten Bedingungen für den Ort einer Besprechung.
ms.openlocfilehash: f29ff1283d876e726e27473485a183956137f981
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058454"
---
# <a name="locationconstraintitem-resource-type"></a>Ressourcentyp „locationConstraintItem“

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die vom Client definierten Bedingungen für den Ort einer Besprechung

Abgeleitet von [location](location.md).

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  
  ],
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationUri": "string"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| address | [physicalAddress](physicaladdress.md) |Die Adresse des Orts. |
| Koordinaten | [outlookGeoCoordinates](outlookgeocoordinates.md) | Die geografischen Koordinaten und die Erhebung des Orts. |
| displayName  | String | Der Name, der mit dem Ort verknüpft ist                       |
| locationEmailAddress | String | Optionale E-Mail-Adresse des Orts. |
| locationUri | String | Optionaler URI, der den Ort darstellt. |
| resolveAvailability | Boolescher Wert | Wenn „true“ gesetzt ist und die angegebene Ressource gebucht ist, sucht [findMeetingTimes](../api/user-findmeetingtimes.md) nach einer anderen, freien Ressource. Wenn „false“ gesetzt ist und die angegebene Ressource gebucht ist, gibt **findMeetingTimes** die Ressource mit dem höchsten Wert aus dem Cache des Benutzers zurück, ohne zu prüfen, ob diese Ressource frei ist. Der Standardwert ist „true“. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->