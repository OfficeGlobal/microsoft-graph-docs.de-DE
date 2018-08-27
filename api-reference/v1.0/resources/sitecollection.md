---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
ms.openlocfilehash: 84de2a8aa6796051b3b11ebec0d0f8f5934ea1fc
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "19069343"
---
# <a name="sitecollection-resource"></a>SiteCollection-Ressource

Die **siteCollection**-Ressource stellt weitere Informationen zu einer Websitesammlung bereit.

Wenn eine [ **site** ](site.md)-Ressource eine **siteCollection**-Eigenschaft mit einem Wert ungleich NULL hat, ist die Website eine Stammwebsite einer Websitesammlung.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com",
  "root": { "@odata.type": "microsoft.graph.root" }
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname        | Typ     | Beschreibung
|:---------------------|:---------|:---------------------------------------------------
| **hostname**         | string   | Der Hostname der Websitesammlung. Schreibgeschützt.
| **root**             | [root][] | Falls vorhanden gibt dies an, dass dies eine Stammwebsitesammlung in SharePoint ist. Schreibgeschützt.

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Facets/SiteCollection"
}-->
