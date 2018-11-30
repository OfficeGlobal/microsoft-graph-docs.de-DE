---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
ms.openlocfilehash: d54246002c158270ae23cf81cdc93673f40bd78c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061883"
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
