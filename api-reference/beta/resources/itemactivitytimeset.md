---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
ms.openlocfilehash: 2ff3e1a2356c43457fe251928728632bd2228b10
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809892"
---
# <a name="itemactivitytimeset-resource-type"></a>ItemActivityTimeSet-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **ItemActivityTimeSet**-Ressource enthält Informationen darüber, wann eine [Aktivität][activity] in einem Element stattfindet.

[activity]: itemactivity.md

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivityTimeSet",
  "@type.aka": "oneDrive.times",
  "@property.aka": "observedDateTime=observedTime recordedDateTime=recordedTime"
}-->

```json
{
  "observedDateTime": "String (timestamp)",
  "recordedDateTime": "String (timestamp)"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname    | Typ           | Beschreibung
|:-----------------|:---------------|:-----------------------------------------
| observedDateTime | DateTimeOffset | Wann die Ausführung der Aktivität beobachtet wurde.
| recordedDateTime | DateTimeOffset | Wann die Beobachtung vom Dienst aufgezeichnet wurde.

Der Unterschied zwischen den Zeiten **observed** und **recorded** ist besonders wichtig bei Offline-Zusammenarbeitsszenarien.
Wenn ein Benutzer offline eine Datei kommentiert, wird der Zeitpunkt des Kommentars als **observedDateTime** festgelegt.
Wenn sich der Benutzer zu einem späteren Zeitpunkt erneut mit der Cloud verbindet und die Änderungen hochgeladen werden, wird dieser Zeitpunkt als **recordedDateTime** festgelegt.

## <a name="remarks"></a>Hinweise

Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet"
} -->
