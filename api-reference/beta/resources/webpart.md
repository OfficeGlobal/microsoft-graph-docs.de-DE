---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
ms.openlocfilehash: e9bb612e20bc3d2416503f571f5abf364215efb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061142"
---
# <a name="webpart-resource"></a>WebPart-Ressource

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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

## <a name="remarks"></a>Hinweise

Webparts können ihre eigenen erforderlichen Eigenschaften unter **Daten**definieren.

Weitere Informationen zu Seiten finden Sie unter [SitePage](sitepage.md).
<!-- {
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control"
} -->