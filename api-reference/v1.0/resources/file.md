---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Datei
ms.openlocfilehash: 2201533457863c3cac6b7a9463f80e37bd5a569a
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23267465"
---
# <a name="file-resource-type"></a>File-Ressourcentyp

Die **File**-Ressource gruppiert dateibezogene Datenelemente in einer einzelnen Struktur.

Wenn ein [**DriveItem**](driveitem.md) ein **file**-Facet ungleich Null aufweist, stellt das Element eine Datei dar. Neben anderen Eigenschaften weisen Dateien eine **content**-Beziehung auf, die den Bytedatenstrom der Datei enthält.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.file"
}-->

```json
{
  "hashes": {"@odata.type": "microsoft.graph.hashes"},
  "mimeType": "string"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ                    | Beschreibung                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| hashes   | [Hashes](hashes.md) | Hashes des binären Inhalts der Datei, wenn verfügbar. Schreibgeschützt.                                                                                    |
| mimeType | Zeichenfolge                  | Der MIME-Typ für die Datei. Dieser wird von der Logik auf dem Server bestimmt und stimmt möglicherweise nicht mit dem Wert überein, der bereitgestellt wurde, als die Datei hochgeladen wurde. Schreibgeschützt. |

## <a name="remarks"></a>Bemerkungen 

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
