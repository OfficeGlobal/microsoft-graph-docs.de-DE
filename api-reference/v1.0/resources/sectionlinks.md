---
title: sectionLinks-Ressourcentyp
description: Links zum Öffnen eines OneNote-Abschnitts.
ms.openlocfilehash: 4ca6221992c75f410839538d8080c084c8486903
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017071"
---
# <a name="sectionlinks-resource-type"></a>sectionLinks-Ressourcentyp

Links zum Öffnen eines OneNote-Abschnitts.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sectionLinks"
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
|oneNoteClientUrl|[externalLink](externallink.md)|Öffnet den Abschnitt im systemeigenen OneNote-Client, sofern er installiert ist.|
|oneNoteWebUrl|[externalLink](externallink.md)|Öffnet den Abschnitt in OneNote Online.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->