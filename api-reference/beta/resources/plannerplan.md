---
title: plannerPlan-Ressourcentyp
description: Die Ressource **PlannerPlan** stellt einen Plan in Office 365. Ein Plan kann eine Gruppe Besitz und enthält eine Auflistung von PlannerTasks. Sie können auch eine Auflistung von PlannerBuckets verfügen. Jedes Plan-Objekt ist ein Details-Objekt, das Informationen über den Plan enthalten kann. Weitere Informationen zu den Beziehungen zwischen Gruppen, Pläne und Aufgaben finden Sie unter Planner.
ms.openlocfilehash: 236b6cb5d35e11a30bcb4371e0563b56ac93de8f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060346"
---
# <a name="plannerplan-resource-type"></a>plannerPlan-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die Ressource **PlannerPlan** stellt einen Plan in Office 365. Ein Plan kann eine [Gruppe](group.md) Besitz und enthält eine Auflistung von [PlannerTasks](plannertask.md). Sie können auch eine Auflistung von [PlannerBuckets](plannerbucket.md)verfügen. Jedes Plan-Objekt ist ein [Details](plannerplandetails.md) -Objekt, das Informationen über den Plan enthalten kann. Weitere Informationen zu den Beziehungen zwischen Gruppen, Pläne und Aufgaben finden Sie unter [Planner](planner-overview.md).



## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[plannerPlan abrufen](../api/plannerplan-get.md) | [plannerPlan](plannerplan.md) |Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerPlan**-Objekts.|
|[Buckets auflisten](../api/plannerplan-list-buckets.md) |[plannerBucket](plannerbucket.md)-Sammlung| Dient zum Abrufen einer **plannerBucket**-Objektsammlung.|
|[Aufgaben auflisten](../api/plannerplan-list-tasks.md) |[plannerTask](plannertask.md)-Sammlung| Dient zum Abrufen einer **plannerTask**-Objektsammlung.|
|[Update](../api/plannerplan-update.md) | [plannerPlan](plannerplan.md) |Dient zum Aktualisieren eines **plannerPlan**-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|createdDateTime|DateTimeOffset|Schreibgeschützt. Datum und Uhrzeit der Erstellung des Plans. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|id|String| Schreibgeschützt. ID des Plans. Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet. [Format Validierung](tasks-identifiers-disclaimer.md) erfolgt für den Dienst.|
|owner|String|Die ID der [Gruppe](group.md) , die den Plan besitzt. Eine gültige Gruppe muss vorhanden sein, bevor Sie dieses Feld festgelegt werden kann. Diese Eigenschaft kann nicht aktualisiert werden, nachdem er festgelegt wurde.|
|title|String|Erforderlich.  Der Titel des Plans.|
|createdBy|[identitySet](identityset.md)|Schreibgeschützt. Der Benutzer, der den Plan erstellt hat.|
|Kontext|[plannerPlanContextCollection](plannerplancontextcollection.md)| Schreibgeschützt. Zusätzliche Benutzererlebnis, in denen dieser Plan verwendet wird, dargestellt als [PlannerPlanContext](plannerplancontext.md) Einträge.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|buckets|[plannerBucket](plannerbucket.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu. Sammlung von Buckets im Plan.|
|Details|[plannerPlanDetails](plannerplandetails.md)| Schreibgeschützt. Lässt Nullwerte zu. Weitere Details über den Plan.|
|tasks|[plannerTask](plannertask.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu. Sammlung von Aufgaben im Plan.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "contexts": {
    "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
        "@odata.type": "#microsoft.graph.plannerPlanContext",
        "associationType": "Board",
        "createdDateTime": "2015-10-14T00:57:28.4698344Z",
        "displayNameSegments": [
            "Finance Team",
            "Budget Plans"
        ],
        "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
    }
  },
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->