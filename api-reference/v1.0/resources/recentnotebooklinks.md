---
title: recentNotebookLinks-Ressourcentyp
description: Links zum Öffnen eines OneNote-Notizbuchs. Dieser Ressourcentyp ist als Eigenschaft für eine recentNotebook-Ressource vorhanden.
localization_priority: Normal
ms.openlocfilehash: 846047bd602d19cb4745e0a63f0326aaf7bfb512
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810584"
---
# <a name="recentnotebooklinks-resource-type"></a>recentNotebookLinks-Ressourcentyp

Links zum Öffnen eines OneNote-Notizbuchs. Dieser Ressourcentyp ist als Eigenschaft für eine [recentNotebook](recentnotebook.md)-Ressource vorhanden.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|oneNoteClientUrl|[externalLink](externallink.md)|Öffnet das Notizbuch im systemeigenen OneNote-Client, sofern er installiert ist.|
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
<!-- {
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
