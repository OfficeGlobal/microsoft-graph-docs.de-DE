---
title: FormatProtection-Ressourcentyp
description: Stellt den Formatschutz eines Bereichsobjekts dar.
localization_priority: Normal
ms.openlocfilehash: 0b4add2e30a1e475adcb162903f771ce760f9285
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805621"
---
# <a name="formatprotection-resource-type"></a>FormatProtection-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt den Formatschutz eines Bereichsobjekts dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[FormatProtection abrufen](../api/formatprotection-get.md) | [FormatProtection](formatprotection.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des formatProtection-Objekts.|
|[Update](../api/formatprotection-update.md) | [FormatProtection](formatprotection.md)  |Dient zum Aktualisieren des FormatProtection-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|formulaHidden|boolean|Zeigt an, ob Excel die Formel für die Zellen im Bereich ausblendet. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Einstellung zur Formelausblendung hat.|
|locked|boolean|Gibt an, ob Excel die Zellen im Objekt sperrt. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Einstellung zum Sperren hat.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.formatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
