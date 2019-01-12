---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7fb11fc9dc2f55b853ec512255ffa06f8a53cef6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933673"
---
# <a name="sitecollection-resource"></a>SiteCollection-Ressource

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **siteCollection**-Ressource stellt weitere Informationen zu einer Websitesammlung bereit.

Wenn eine [ **site** ](site.md)-Ressource eine **siteCollection**-Eigenschaft mit einem Wert ungleich NULL hat, ist die Website eine Stammwebsite einer Websitesammlung.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "dataLocationCode", "root"
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com",
  "dataLocationCode": "EUR",
  "root": { "@odata.type": "microsoft.graph.root" }
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname        | Typ     | Beschreibung
|:---------------------|:---------|:---------------------------------------------------
| **hostname**         | string   | Der Hostname der Websitesammlung. Schreibgeschützt.
| **dataLocationCode** | string   | Der Code geografische Region, in dem diese Websitesammlung befindet. Schreibgeschützt.
| **root**             | [root][] | Falls vorhanden, gibt an, dass dies eine Stammwebsitesammlung in SharePoint ist. Schreibgeschützt.

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
