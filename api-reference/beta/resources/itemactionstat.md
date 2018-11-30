---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionStat
ms.openlocfilehash: f7e9351bc4a394005cffc712aa444c999a51b363
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064934"
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
