---
title: assignedPlan-Ressourcentyp
description: Die **assignedPlans**-Eigenschaft der user-Entität und der oganization-Entität ist eine Sammlung von **assignedPlan**.
localization_priority: Normal
ms.openlocfilehash: d1f3df6a88ab688206d26db6fc0afe1e1d4a4f60
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852997"
---
# <a name="assignedplan-resource-type"></a>assignedPlan-Ressourcentyp

Die **assignedPlans**-Eigenschaft der [user](user.md)-Entität und der [oganization](organization.md)-Entität ist eine Sammlung von **assignedPlan**.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|assignedDateTime|DateTimeOffset|Datum und Uhrzeit der Zuweisung des Plans, z. B.: 2013-01-02T19:32:30Z. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|capabilityStatus|String|Z. B. „Aktiviert“.|
|service|String|Der Name des Diensts. z. B. „Exchange“.|
|servicePlanId|Guid|Eine GUID, die den Serviceplan identifiziert.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedPlan"
}-->

```json
{
  "assignedDateTime": "String (timestamp)",
  "capabilityStatus": "string",
  "service": "string",
  "servicePlanId": "guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
