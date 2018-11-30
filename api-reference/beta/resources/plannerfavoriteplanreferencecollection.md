---
title: Ressourcentyp plannerFavoritePlanReferenceCollection
description: " der Wert ist das PlannerFavoritePlanReference-Objekt."
ms.openlocfilehash: 78544e17604a0938cc0e88969e2542fc26bdff1b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064247"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a>Ressourcentyp plannerFavoritePlanReferenceCollection

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die Ressource **PlannerFavoritePlanReferenceCollection** stellt die Auflistung von Verweisen auf Pläne, die von einem Benutzer als Favoriten markiert sind. Diese Ressource ist ein offener Typ und ist Teil des [PlannerUser](planneruser.md) -Objekts. Der Name der Eigenschaft in der Eigenschaft-Wert-Paar ist die ID des entsprechenden Plans. der Wert ist das [PlannerFavoritePlanReference](plannerfavoriteplanreference.md) -Objekt.


## <a name="properties"></a>Eigenschaften
Sie können die Eigenschaften dieses Typs open definieren. Werden die Eigenschaftennamen `id` Werte der [PlannerPlan](plannerplan.md) Ressourcen und deren Werte muss [PlannerFavoritePlanReference](plannerfavoriteplanreference.md) -Objekte. Wenn ein Element in der Liste der Favoriten entfernen möchten, legen Sie den Wert der Eigenschaft `null`.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"
}-->

```json
{
  "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
    "@odata.type": "microsoft.graph.plannerFavoritePlanReference",
    "orderHint": "8586866870001551087",
    "planTitle": "Customer reviews"
  },
  "uZWtCtli30CGoWLIWSat1mQAC0ai": {
    "@odata.type": "microsoft.graph.plannerFavoritePlanReference",
    "orderHint": "8586848705198093378",
    "planTitle": "Order Management (December 2017)"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
