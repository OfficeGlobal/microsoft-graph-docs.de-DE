---
title: Ressourcentyp plannerRecentPlanReferenceCollection
description: Die Ressource **PlannerRecentPlanReferenceCollection** stellt die Auflistung von Verweisen auf Pläne, die von einem Benutzer zuletzt angezeigt wurden. Diese Ressource ist ein offener Typ und ist Teil des PlannerUser-Objekts. Der Name der Eigenschaft ist die ID des entsprechenden Plans. Der Wert in der Eigenschaft-Wert-Paar ist das PlannerRecentPlanReference-Objekt.
ms.openlocfilehash: b22f7367a1826c95889b63a6884885ce49497c33
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065995"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a>Ressourcentyp plannerRecentPlanReferenceCollection

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die Ressource **PlannerRecentPlanReferenceCollection** stellt die Auflistung von Verweisen auf Pläne, die von einem Benutzer zuletzt angezeigt wurden. Diese Ressource ist ein offener Typ und ist Teil des [PlannerUser](planneruser.md) -Objekts. Der Name der Eigenschaft ist die ID des entsprechenden Plans. Der Wert in der Eigenschaft-Wert-Paar ist das [PlannerRecentPlanReference](plannerrecentplanreference.md) -Objekt.
Hinzufügen von neuen verweisen auf diese Auflistung wird automatisch die ältesten Einträge entfernt, wenn die Größe der Auflistung einen festgelegten Höchstwert überschreitet.


## <a name="properties"></a>Eigenschaften
Sie können die Eigenschaften dieses Typs open definieren. Werden die Eigenschaftennamen `id` Werte der [PlannerPlan](plannerplan.md) Ressourcen und deren Werte muss [PlannerRecentPlanReference](plannerrecentplanreference.md) -Objekte. Wenn ein Element in der Liste der Favoriten entfernen möchten, legen Sie den Wert der Eigenschaft `null`.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"
}-->

```json
{
  "7oTB5aMIAE2rVo-1N-L7RmQAGX2q": {
    "@odata.type": "microsoft.graph.plannerRecentPlanReference",
    "lastAccessedDateTime": "2017-12-02T22:49:46.155Z",
    "planTitle": "Purchase Workflow"
  },
  "iKNMHkk3vEWpSF7F7iZWIGQAAMMw": {
    "@odata.type": "microsoft.graph.plannerRecentPlanReference",
    "lastAccessedDateTime": "2017-12-03T21:59:28.975Z",
    "planTitle": "New Year's Office Party"
  }
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerRecentPlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
