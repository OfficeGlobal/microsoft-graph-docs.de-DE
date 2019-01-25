---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c019da7cb10a8c26faa8d338c54436043f83db8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510239"
---
# <a name="webpart-resource"></a>WebPart-Ressource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **WebPart** -Ressource stellt Typ und von Renderinginformationen für ein Webpart auf einer [SitePage](sitepage.md)dar.

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "string (guid)",
  "data": {
    "instanceId": "string (guid) (optional)"
  }
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft                | Typ             | Beschreibung
|:------------------------|:-----------------|:----------------------------------
| **type**                | String           | Ein eindeutiger Bezeichner, der den WebPart angibt. Schreibgeschützt.
| **data**                | [sitePageData][] | Die erforderlichen Eigenschaften für das WebPart (hängt vom WebPart)

[sitePageData]: sitepagedata.md

## <a name="remarks"></a>Bemerkungen

Webparts können ihre eigenen erforderlichen Eigenschaften unter **Daten**definieren.

Weitere Informationen zu Seiten finden Sie unter [SitePage](sitepage.md).
<!--
{
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control",
  "suppressions": [
    "Error: /api-reference/beta/resources/webpart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
