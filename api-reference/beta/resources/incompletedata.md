---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
ms.openlocfilehash: 4319ab0f36e12ddd28ca9bb6c7bfd48043228504
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059184"
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
| wasThrottled              | Boolesch        | Einige Daten wurde nicht übermäßig viele Aktivitäten aufgezeichnet.

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData"
} -->
