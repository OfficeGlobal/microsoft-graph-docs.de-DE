---
title: plannerPlanDetails-Ressourcentyp
description: Die **plannerPlanDetails**-Ressource stellt die zusätzlichen Informationen zu einem Plan dar. Jedes plan-Objekt hat ein Detailobjekt.
localization_priority: Normal
ms.openlocfilehash: 59064093b485b6c82bd5b2e0b59ca1868e8517e4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867739"
---
# <a name="plannerplandetails-resource-type"></a>plannerPlanDetails-Ressourcentyp


Die **plannerPlanDetails**-Ressource stellt die zusätzlichen Informationen zu einem Plan dar. Jedes [plan](plannerplan.md)-Objekt hat ein Detailobjekt.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[plannerPlanDetails abrufen](../api/plannerplandetails-get.md) | [plannerPlanDetails](plannerplandetails.md) |Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerPlanDetails**-Objekts.|
|[Update](../api/plannerplandetails-update.md) | [plannerPlanDetails](plannerplandetails.md)    |Dient zum Aktualisieren des **plannerPlanDetails**-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|Ein Objekt, das die Beschreibungen der sechs Kategorien angibt, die den Aufgaben im Plan zugeordnet werden können.|
|id|Zeichenfolge| Schreibgeschützt. ID des die Details des Plans. Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet. [Format Validierung](planner-identifiers-disclaimer.md) erfolgt für den Dienst.|
|sharedWith|[plannerUserIds](planneruserids.md)|Der Satz von Benutzer-IDs, für die dieser Plan freigegeben ist. Wenn Sie Office 365 Gruppen nutzen, verwenden Sie die Gruppen-API zum Verwalten von Gruppenmitgliedschaften, um den Plan der [Gruppe](group.md) freizugeben. Sie können auch vorhandene Mitglieder der Gruppe zu dieser Sammlung hinzufügen, dies ist jedoch nicht erforderlich, damit sie auf den im Besitz der Gruppe befindlichen Plan zugreifen können. |

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
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
