---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Ordner
localization_priority: Normal
ms.openlocfilehash: fab5db026b47aa84f7d097a19782b70eac6b6064
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821420"
---
# <a name="folder-resource-type"></a>Folder-Ressourcentyp

Die **Folder**-Ressource gruppiert ordnerbezogene Daten für ein Element in einer einzelnen Struktur. [**DriveItems**](driveitem.md) mit einem **Ordner**-Facet, das nicht Null ist, sind Container für andere DriveItems.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.folder"
}-->

```json
{
  "childCount": 1024,
  "view": { "@odata.type": "microsoft.graph.folderView" }
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft       | Typ           | Beschreibung
|:---------------|:---------------|:-------------------------------------------
| **childCount** | Int32          | Die Anzahl von direkt in dem jeweiligen Container enthaltenen untergeordneten Elementen.
| **view**       | [folderView][] | Eine Sammlung von Eigenschaften, welche die empfohlene Ansicht für den Ordner definieren.

## <a name="remarks"></a>Hinweise 

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem][].

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
