---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Datei
localization_priority: Normal
ms.openlocfilehash: 7478ba064b5193ce7ddcd8685fc571a72d4b0057
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480407"
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
| mimeType | string                  | Der MIME-Typ für die Datei. Dieser wird von der Logik auf dem Server bestimmt und stimmt möglicherweise nicht mit dem Wert überein, der bereitgestellt wurde, als die Datei hochgeladen wurde. Schreibgeschützt. |

## <a name="remarks"></a>Bemerkungen 

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
