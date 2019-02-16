---
title: attendeeDataModel-Ressourcentyp
description: Der Typ eines Teilnehmers.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e8659b88cae8b9d2a94177593da40b61363fa23b
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057387"
---
# <a name="attendeedatamodel-resource-type"></a>attendeeDataModel-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt eine Person oder Ressource dar, die in einer Besprechung eingeschlossen wird.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "type"
  ],
  "@odata.type": "microsoft.graph.attendeeDataModel"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|type|attendeeType| Der Typ eines Teilnehmers. Die möglichen Werte sind: `required`, `optional`, `resource`. Wenn es sich bei dem Teilnehmer um eine Person handelt, ist [findMeetingTimes](../api/user-findmeetingtimes.md) immer der `required` Typ der Person.|
|emailAddress|[emailAddress](emailaddress.md)|Enthält den Namen und die SMTP-Adresse des Teilnehmers.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeedatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->