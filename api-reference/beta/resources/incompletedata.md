---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
ms.openlocfilehash: add1e3612f65e203f2437419cbb105b78025aa0a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807511"
---
# <a name="incompletedata-resource-type"></a>Ressourcentyp incompleteData

 > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **IncompleteData** Facetten gibt an, dass eine Ressource mit unvollständiger Daten generiert wurde.
Die Eigenschaften innerhalb können Informationen über bereitzustellen, Grund, warum es unvollständige Daten.

## <a name="json-representation"></a>JSON-Darstellung

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft                  | Typ           | Beschreibung
|:--------------------------|:---------------|:--------------------------------
| missingDataBeforeDateTime | DateTimeOffset | Der Dienst hat keine Quelldaten vor dem angegebenen Zeitpunkt.
| wasThrottled              | Boolescher Wert        | Einige Daten wurde nicht übermäßig viele Aktivitäten aufgezeichnet.

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData"
} -->
