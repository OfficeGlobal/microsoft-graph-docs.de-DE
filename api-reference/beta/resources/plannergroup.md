---
title: plannerGroup-Ressourcentyp
description: Die **plannerGroup**-Ressource bietet einer Gruppe Zugriff auf Planner-Ressourcen. Sie enthält keine verwendbaren Eigenschaften.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 84bb20d0b13f9a99db2f8c59b20e0c9c7c87f93f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513781"
---
# <a name="plannergroup-resource-type"></a>plannerGroup-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannergroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
