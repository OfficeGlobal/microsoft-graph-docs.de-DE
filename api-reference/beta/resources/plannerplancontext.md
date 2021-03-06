---
title: Ressourcentyp plannerPlanContext
description: Die Ressource **PlannerPlanContext** stellt die Beziehung zwischen einem PlannerPlan zu einer Benutzeroberfläche außerhalb Planner dar. Pläne in Planner können in anderen Erfahrungen, beispielsweise Microsoft-Teams, zum Nachverfolgen von Arbeit im Zusammenhang mit dieser Erfahrungen verfügbar gemacht werden.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 76260b51bc6f77acf6fac22e80bd676edd8b8e11
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509238"
---
# <a name="plannerplancontext-resource-type"></a>Ressourcentyp plannerPlanContext

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die Ressource **PlannerPlanContext** stellt die Beziehung zwischen einem [PlannerPlan](plannerplan.md) zu einer Benutzeroberfläche außerhalb Planner dar. Pläne in Planner können in anderen Erfahrungen, beispielsweise Microsoft-Teams, zum Nachverfolgen von Arbeit im Zusammenhang mit dieser Erfahrungen verfügbar gemacht werden.
Die Erfahrung, die der Eintrag **PlannerPlanContext** reresents kann auf Basis der **OwnerAppId** -Eigenschaft identifiziert werden:
 - 5e3ce6c0-2b1f-4285-8d4b-75ee78787346: der Kontext Eintrag gehört zum Microsoft-Teams.
 - 00000003-0000-0ff1-CE00-000000000000: der Eintrag Kontext zu SharePoint gehört.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|associationType|String|Nullwerte zulassend. Eine app-benutzerdefinierten Typ der Zuordnung zwischen der [PlannerPlan](plannerplan.md) und die app. Diese Informationen können die app verschiedene Arten von Beziehungen an den gleichen [PlannerPlan](plannerplan.md)verfolgen.|
|createdDateTime|DateTimeOffset|Schreibgeschützt. Datum und Uhrzeit der Erstellung der **PlannerPlanContext** . Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|displayNameSegments|Zeichenfolgenauflistung|Der Name der externen Erfahrung-Segmente. Segmente sind eine hierarchische Struktur, die anderen apps auf die Beziehung anzeigen kann.|
|ownerAppId|String|Schreibgeschützt. Die ID der app, die die **PlannerPlanContext**erstellt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContext"
}-->

```json
{
  "associationType": "Board",
  "createdDateTime": "2015-10-14T00:57:28.4698344Z",
  "displayNameSegments": [
    "Finance Team",
    "Budget Plans"
  ],
  "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontext.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
