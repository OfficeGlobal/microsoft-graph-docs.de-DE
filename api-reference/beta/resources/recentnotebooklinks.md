---
title: recentNotebookLinks-Ressourcentyp
description: Enthält Links zu einem OneNote-Notizbuch öffnen. Dieser Ressourcentyp ist als Eigenschaft für eine recentNotebook-Ressource vorhanden.
localization_priority: Normal
ms.openlocfilehash: 328f337d63645cdd52722a4216006920c493f9e7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525885"
---
# <a name="recentnotebooklinks-resource-type"></a>recentNotebookLinks-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Enthält Links zu einem OneNote-Notizbuch öffnen. Dieser Ressourcentyp ist als Eigenschaft für eine [recentNotebook](recentnotebook.md)-Ressource vorhanden.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|oneNoteClientUrl|[externalLink](externallink.md)|Wird das Notizbuch im OneNote-Client geöffnet, wenn es installiert ist.|
|oneNoteWebUrl|[externalLink](externallink.md)|Öffnet das Notizbuch in OneNote Online.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/recentnotebooklinks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
