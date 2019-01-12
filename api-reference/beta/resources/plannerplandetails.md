---
title: plannerPlanDetails-Ressourcentyp
description: Die **plannerPlanDetails**-Ressource stellt die zusätzlichen Informationen zu einem Plan dar. Jedes plan-Objekt hat ein Detailobjekt.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: dfb142c8fbd6b2354a3a2d03d29480d119284146
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942381"
---
# <a name="plannerplandetails-resource-type"></a>plannerPlanDetails-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **plannerPlanDetails**-Ressource stellt die zusätzlichen Informationen zu einem Plan dar. Jedes [plan](plannerplan.md)-Objekt hat ein Detailobjekt.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[plannerPlanDetails abrufen](../api/plannerplandetails-get.md) | [plannerPlanDetails](plannerplandetails.md) |Lesen Sie die Eigenschaften und die Beziehungen eines **PlannerPlanDetails** -Objekts.|
|[Update](../api/plannerplandetails-update.md) | [plannerPlanDetails](plannerplandetails.md)    |Aktualisieren eines **PlannerPlanDetails** -Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|Ein Objekt, das die Beschreibungen der sechs Kategorien angibt, die den Aufgaben im Plan zugeordnet werden können.|
|id|Zeichenfolge| Schreibgeschützt. Die ID des die Details des Plans. Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet. [Format Validierung](tasks-identifiers-disclaimer.md) erfolgt für den Dienst.|
|sharedWith|[plannerUserIds](planneruserids.md)|Der Satz von Benutzer-IDs, die mit diesem Plan freigegeben werden. Wenn Sie Office 365 Gruppen verwenden, verwenden Sie die API-Gruppen zum Verwalten der Gruppenmitgliedschaft zum Planen [der Gruppe](group.md) freigeben. Sie können auch vorhandene Mitglieder der Gruppe zu dieser Auflistung hinzufügen, obwohl es nicht erforderlich ist, damit sie Zugriff auf den Besitz der Gruppe Plan. |
|contextDetails|[plannerPlanContextDetailsCollection](plannerplancontextdetailscollection.md)|Schreibgeschützt. Eine Auflistung von zusätzlichen Informationen im Zusammenhang mit [PlannerPlanContext](plannerplancontext.md) -Einträge, die für den Container [PlannerPlan](plannerplan.md) definiert sind. |

## <a name="relationships"></a>Beziehungen
Keine.


## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "contextDetails": {"@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
