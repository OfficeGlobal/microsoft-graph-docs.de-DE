---
title: timeZoneInformation-Ressourcentyp
description: Stellt eine Zeitzone dar. Unterstützte Format ist Windows und bei der Internet Assigned Numbers Authority (IANA) Zeit Zone (auch bekannt als Olson-Zeitzone)
ms.openlocfilehash: 5508f20812b8327a068364df7eb33c5072c3512e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061671"
---
# <a name="timezoneinformation-resource-type"></a>timeZoneInformation-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine Zeitzone dar. Das unterstützte Format ist Windows und auch das Format der [IANA-Zeitzone (Internet Assigned Numbers Authority)](https://www.iana.org/time-zones) (auch bekannt als Olson-Zeitzone) wenn das derzeitige bekannte Problem behoben ist.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Alias|String|Ein Bezeichner für die Zeitzone.|
|displayName|string|Eine Anzeigezeichenfolge, die die Zeitzone darstellt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneInformation"
}-->

```json
{
  "alias": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->