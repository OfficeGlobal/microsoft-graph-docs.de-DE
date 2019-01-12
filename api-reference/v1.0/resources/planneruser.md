---
title: plannerUser-Ressourcentyp
description: Die Ressource **PlannerUser** bieten Zugriff auf Ressourcen Planner für einen Benutzer. Es enthält keine verwendbaren Eigenschaften.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b73e422e232a96068f4545def0f0fdbd9f74ff07
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953560"
---
# <a name="planneruser-resource-type"></a>plannerUser-Ressourcentyp

Die **plannerUser**-Ressource bietet einem [Benutzer](user.md) Zugriff auf Planner-Ressourcen. Sie enthält keine verwendbaren Eigenschaften.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Pläne auflisten](../api/planneruser-list-plans.md) |[plannerPlan](plannerplan.md)-Sammlung| Dient zum Abrufen einer **plannerPlan**-Objektsammlung.|
|[Aufgaben auflisten](../api/planneruser-list-tasks.md) |[plannerTask](plannertask.md)-Sammlung| Dient zum Abrufen einer **plannerTask**-Objektsammlung.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|Zeichenfolge| Schreibgeschützt. Bezeichner der plannerUser-Ressource.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|plans|[plannerPlan](plannerplan.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu. Gibt die dem Benutzer zugewiesenen [plannerTasks](plannertask.md) zurück.|
|tasks|[plannerTask](plannertask.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu. Gibt die für den Benutzer freigegebenen [plannerPlans](plannerplan.md) zurück.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
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
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
