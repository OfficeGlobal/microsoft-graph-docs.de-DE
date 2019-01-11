---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionStat
localization_priority: Normal
ms.openlocfilehash: 1d2ab438e7aaf5b0a6aede99290394a9a4ea7f0e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879527"
---
# <a name="itemactionstat-resource-type"></a>Ressourcentyp itemActionStat

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **ItemActionStat** Ressource enthält aggregierte Details über eine Aktion über einen Zeitraum.

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemActionStat",
}-->

```json
{
  "actionCount": 123,
  "actorCount": 60
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft    | Typ  | Beschreibung
|:------------|:------|:-------------------------------------------------------
| actionCount | Int32 | Die Anzahl der Häufigkeit, mit die Aktion stattfand. Schreibgeschützt.
| actorCount  | Int32 | Die Anzahl der unterschiedlichen Akteure, die die Aktion ausgeführt. Schreibgeschützt.

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActionStat"
} -->
