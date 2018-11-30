---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Ordner
ms.openlocfilehash: 834b2cd7c81a947ca1e6d4619f39a8533677e6c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064205"
---
# <a name="folder-resource-type"></a>Folder-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
| **childCount** | Int64          | Die Anzahl von direkt in dem jeweiligen Container enthaltenen untergeordneten Elementen.
| **view**       | [folderView][] | Eine Sammlung von Eigenschaften, welche die empfohlene Ansicht für den Ordner definieren.


## <a name="remarks"></a>Hinweise 

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem][].

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
