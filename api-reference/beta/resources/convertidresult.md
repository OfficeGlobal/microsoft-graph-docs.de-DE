---
title: Ressourcentyp convertIdResult
description: Das Ergebnis einer ID formatkonvertierung, die von der Funktion TranslateExchangeIds durchgeführt.
ms.openlocfilehash: 3a17399ffe44c43c78f7b50933b2e847a3e64f32
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059472"
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