---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SpecialFolder
localization_priority: Normal
ms.openlocfilehash: 4c1facae90ea8981b1e83087d11e2d81a0354617
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820097"
---
# <a name="specialfolder-resource-type"></a>SpecialFolder-Ressourcentyp

Die **SpecialFolder**-Ressource gruppiert ordnerbezogene Datenelement in einer einzelnen Struktur.

Wenn ein **DriveItem** über ein **specialFolder**-Facet ungleich Null verfügt, stellt das Element einen speziellen (benannten) Ordner dar.
Auf spezielle Ordner können Sie direkt über die [Sammlung spezieller Ordner](../api/drive-get-specialfolder.md) zugreifen.

Spezielle Ordner bieten einfache Aliase für den Zugriff auf bekannte Ordner, ohne dass der Ordner anhand des Pfads nachgeschlagen werden muss (wofür eine Lokalisierung erforderlich wäre) oder anhand einer ID auf den Ordner verwiesen werden muss. Wenn ein spezieller Ordner umbenannt oder an eine andere Position innerhalb des Laufwerks verschoben wird, kann mit dieser Syntax weiterhin dieser Ordner zurückgegeben werden.

Spezielle Ordner werden automatisch erstellt, wenn eine Anwendung das erste Mal versucht, einen Ordner zu schreiben, wenn noch keiner vorhanden ist. Wenn ein Benutzer einen speziellen Ordner löscht, wird dieser neu erstellt, wenn erneut in den Ordner geschrieben wird.

**Hinweis:** Wenn Ihre App nur den **Files.Read**-Bereich angefordert hat und einen speziellen Ordner anfordert, der nicht vorhanden ist, wird als Antwort der Fehler `403 Forbidden` zurückgegeben.

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.specialFolder"
}-->
```json
{
  "name": "string"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft  | Typ   | Beschreibung                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| name      | string | Der eindeutige Bezeichner für dieses Element in der `/drive/special`-Sammlung |

## <a name="special-folders"></a>Spezielle Ordner

Im Folgenden sind spezielle Ordner aufgelistet, die in OneDrive Personal und OneDrive for Business zur Verfügung stehen.

| Name        | Ordner-ID    | Beschreibung                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| Anwendungsstamm    | `approot`    | Der persönliche Ordner der Anwendung. In der Regel unter `/Apps/{Application Name}` |
| Eigene Aufnahmen | `cameraroll` | Der Sicherungsordner für Eigene Aufnahmen. In OneDrive for Business nicht verfügbar.   |
| Dokumente   | `documents`  | Der Ordner „Dokumente“.                                                    |
| Musik       | `music`      | Der Ordner „Musik“. In OneDrive for Business nicht verfügbar.                |
| Fotos      | `photos`     | Der Ordner „Fotos“.                                                       |

## <a name="remarks"></a>Bemerkungen 

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SpecialFolder"
} -->
