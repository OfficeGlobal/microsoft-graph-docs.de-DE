---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Datei
localization_priority: Normal
ms.openlocfilehash: bd2b0fba75ef54586dcfe8b69043669b0681f6b2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816324"
---
# <a name="file-resource-type"></a>File-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
| hashes   | [HashesType](hashes.md) | Hashes des binären Inhalts der Datei, wenn verfügbar. Schreibgeschützt.                                                                                    |
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
