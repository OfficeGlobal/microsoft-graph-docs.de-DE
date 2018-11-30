---
title: plannerAppliedCategories-Ressourcentyp
description: Die Ressource **AppliedCategoriesCollection** stellt die Auflistung von Kategorien (oder Etiketten), die mit einer Aufgabe angewendet wurden. Es ist Teil des PlannerTask-Objekts.
ms.openlocfilehash: 0bb7987c3da62f2302b08ab43fa00d09763e0c1d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064487"
---
# <a name="plannerappliedcategories-resource-type"></a>plannerAppliedCategories-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **AppliedCategoriesCollection**-Ressource stellt die Sammlung von Kategorien (oder Bezeichnungen) dar, die auf eine Aufgabe angewendet wurden. Sie ist Teil des [plannerTask](plannertask.md)-Objekts. Auf eine Aufgabe können bis zu 6 Kategorien angewendet werden. Kategoriebeschreibungen wie `category1`, `category2` usw. sind Teil des [planDetails ](plannerplandetails.md)-Objekts. Es handelt sich um einen offenen Typ.

## <a name="properties"></a>Eigenschaften
Eigenschaften mit offenem Typ können vom Client definiert werden. In diesem Fall muss der Client jedoch `category1`, `category2`, `category3`, `category4`, `category5` und/oder `category6` als Eigenschaften angeben, deren Wert das boolesche `true` ist, wenn die entsprechenden Kategorien auf die Aufgabe angewendet werden. Nachfolgend ein Beispiel. Wenn sie nicht zutreffen, werden Eigenschaften automatisch entfernt, indem ihre Werte auf das boolesche `false` festgelegt werden. 

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAppliedCategories"
}-->

```json
{
  "String-value": true
}
```

Beispiel: 

```json
{
  "category1": true,
  "category3": true,
  "category5": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->