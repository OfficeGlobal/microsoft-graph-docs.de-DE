---
title: plannerGroup-Ressourcentyp
description: Die Ressource **PlannerGroup** bietet Zugriff auf Ressourcen Planner für eine Gruppe. Es enthält keine verwendbaren Eigenschaften.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 6e60db0a3f33bc47d0ea63b7a773b7bb691cd5be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981420"
---
# <a name="plannergroup-resource-type"></a>plannerGroup-Ressourcentyp

Die **plannerGroup**-Ressource bietet einer [Gruppe](group.md) Zugriff auf Planner-Ressourcen. Sie enthält keine verwendbaren Eigenschaften.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Pläne auflisten](../api/plannergroup-list-plans.md) |[plannerPlan](plannerplan.md)-Sammlung| Dient zum Abrufen einer **plannerPlan**-Objektsammlung.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Schreibgeschützt. Bezeichner der **plannerGroup**-Ressource.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|plans|[plannerPlan](plannerplan.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu. Gibt die [plannerPlans](plannerplan.md) im Besitz der Gruppe zurück.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
