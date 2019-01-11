---
title: Ressourcentyp synchronizationProgress
description: Stellt den Fortschritt des ein SynchronizationJob an.
localization_priority: Normal
ms.openlocfilehash: 3c1168cdac6a073842cb5e08d165572591d2d8e0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885386"
---
# <a name="synchronizationprogress-resource-type"></a>Ressourcentyp synchronizationProgress

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
  "@odata.type": "microsoft.graph.synchronizationStatus"
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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
