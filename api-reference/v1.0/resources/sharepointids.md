---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: sharepointIds
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d65700806c24b0d82d61d05e1e409292bce010a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919162"
---
# <a name="sharepointids-resource-type"></a>SharePointIds-Ressourcentyp

Die **SharePointIds**-Ressource gruppiert die verschiedenen Bezeichner für ein in einer SharePoint-Website oder auf OneDrive for Business gespeichertes Element in einer einzelnen Struktur.

**Hinweis:** von OneDrive Personal zurückgegebene Elemente umfassen kein **SharePointIds**-Facet.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "listId", "listItemId", "listItemUniqueId", "siteId", "siteUrl", "webId" ],
  "@odata.type": "microsoft.graph.sharepointIds"
}-->

```json
{
    "listId": "string",
    "listItemId": "string",
    "listItemUniqueId": "string",
    "siteId": "string",
    "siteUrl": "url",
    "webId": "string"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft         | Typ         | Beschreibung
|:-----------------|:-------------|:-------------------------------------------
| listId           | string       | Der eindeutige Bezeichner (GUID) für die Liste des Elements in SharePoint.
| listItemId       | string       | Ein ganzzahliger Bezeichner für das Element innerhalb der Liste.
| listItemUniqueId | string       | Der eindeutige Bezeichner (GUID) für das Element in OneDrive for Business oder auf einer SharePoint-Website.
| siteId           | string       | Der eindeutige Bezeichner (GUID) für die Websitesammlung (SPSite) des Elements.
| siteUrl          | string (URL) | Die SharePoint-URL für die Website, die das Element enthält.
| webId            | string       | Der eindeutige Bezeichner (GUID) für die Website (SPWeb) des Elements.

## <a name="remarks"></a>Bemerkungen

Weitere Informationen über die Facets einer **driveItem**-Ressource finden Sie unter [**driveItem**](driveitem.md).



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->
