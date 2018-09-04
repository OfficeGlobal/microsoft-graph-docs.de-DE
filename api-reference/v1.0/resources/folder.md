---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Ordner
ms.openlocfilehash: c0ab787f1c1f04ff77eeb69979dc6a825d4f3c33
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23266562"
---
# <a name="folder-resource-type"></a>Ordner-Ressourcentyp

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
| **Ansicht**       | [folderView][] | Eine Sammlung von Eigenschaften, welche die empfohlene Ansicht für den Ordner definieren.

## <a name="remarks"></a>Hinweise 

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem][].

[folderView]: folderView.md
[DriveItem]: driveItem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
