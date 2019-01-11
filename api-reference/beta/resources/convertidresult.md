---
title: Ressourcentyp convertIdResult
description: Das Ergebnis einer ID formatkonvertierung, die von der Funktion TranslateExchangeIds durchgeführt.
localization_priority: Normal
ms.openlocfilehash: 7e1878de3d3b7ddee36d799c928d6a130b578200
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821455"
---
# <a name="convertidresult-resource-type"></a>Ressourcentyp convertIdResult

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Das Ergebnis einer ID formatkonvertierung, die von der Funktion [TranslateExchangeIds](../api/user-translateexchangeids.md) durchgeführt.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------|:-----|:------------|
| sourceId | String | Der Bezeichner, der konvertiert wurde. Dieser Wert ist der ursprüngliche, nicht konvertierten Bezeichner. |
| targetId | String | Der Bezeichner konvertierte. Dieser Wert ist nicht vorhanden, wenn die Konvertierung fehlgeschlagen ist. |
| errorDetails | [Allgemeiner Fehler](genericerror.md) | Ein Error-Objekt zurück, der den Grund für die Konvertierungsfehler angibt. Dieser Wert ist nicht vorhanden, wenn die Konvertierung erfolgreich war. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```
