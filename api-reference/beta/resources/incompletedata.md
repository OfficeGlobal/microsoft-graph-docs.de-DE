---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
ms.openlocfilehash: f2493263d5293b95cbe386b46c56429d11dda089
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525087"
---
# <a name="incompletedata-resource-type"></a>Ressourcentyp incompleteData

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": [
    "Error: /api-reference/beta/resources/incompletedata.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
