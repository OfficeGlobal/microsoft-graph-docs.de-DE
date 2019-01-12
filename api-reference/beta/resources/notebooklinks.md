---
title: notebookLinks-Ressourcentyp
description: Links zum Öffnen eines OneNote-Notizbuchs.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: da6896fccbea412fb29d88e02088dd7a52e25173
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956178"
---
# <a name="notebooklinks-resource-type"></a>notebookLinks-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Links zum Öffnen eines OneNote-Notizbuchs.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.notebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|oneNoteClientUrl|[externalLink](externallink.md)|Öffnet das Notizbuch im systemeigenen OneNote-Client, sofern er installiert ist.|
|oneNoteWebUrl|[externalLink](externallink.md)|Öffnet das Notizbuch in OneNote Online.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
