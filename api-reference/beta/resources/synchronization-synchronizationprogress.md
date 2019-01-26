---
title: Ressourcentyp synchronizationProgress
description: Stellt den Fortschritt des ein SynchronizationJob an.
localization_priority: Normal
ms.openlocfilehash: 39351f07720d44679675396f9e995f5e78e25fcc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572745"
---
# <a name="synchronizationprogress-resource-type"></a>Ressourcentyp synchronizationProgress

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt den Fortschritt des ein [SynchronizationJob](synchronization-synchronizationjob.md) an.

## <a name="properties"></a>Eigenschaften

| Eigenschaft                              | Typ      | Beschreibung    |
|:--------------------------------------|:----------|:---------------|
|completedUnits|Int32|Die Zähler Fortschritt das Verhältnis der; die Anzahl der Einheiten von Änderungen, die bereits verarbeitet.|
|progressObservationDateTime|DateTimeOffset|Der Zeitpunkt der eine Beobachtung Fortschritt als Offset in Minuten aus UTC.|
|totalUnits|Int32|Die als Nenner des Fortschritts das Verhältnis der; eine Anzahl von Einheiten Änderungen verarbeitet werden, um die Synchronisierung ausführen.|
|Einheiten|String|Eine optionale Beschreibung der Einheiten.|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationProgress"
}-->

```json
{
  "completedUnits": 1025,
  "progressObservationDateTime": "2017-10-10T17:00:00Z",
  "totalUnits": 3024,
  "units": "pages"
}

```

<!-- uuid: 15571993-7e2f-4842-84d5-01ceb67cdc05
20185-08-14 22:30:00 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationprogress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
