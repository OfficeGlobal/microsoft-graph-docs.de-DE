---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Ordner
localization_priority: Normal
ms.openlocfilehash: af22487f017830481af6f39e113b80009f2e567f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512752"
---
# <a name="folder-resource-type"></a>Folder-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

<!--
{
  "type": "#page.annotation",
  "description": "folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/folder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
