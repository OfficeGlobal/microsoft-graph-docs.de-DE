---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Kontingent
localization_priority: Normal
ms.openlocfilehash: 58969adb525736b8a665844a5fa4b48ae4ca1831
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848412"
---
# <a name="quota-resource-type"></a>Quota-Ressourcentyp

Die **quota**-Ressource enthält Details zu Leerzeichenbeschränkungen auf einer[Laufwerk](drive.md)-Ressource.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.quota"
}-->

```json
{
  "deleted": 1024,
  "remaining": 1024,
  "state": "normal | nearing | critical | exceeded",
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname | Typ   | Beschreibung                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| gesamt         | Int64  | Zulässige Speicherplatz in Byte. Schreibgeschützt.                           |
| verwendet          | Int64  | Gesamter verwendeter Speicherplatz in Byte. Schreibgeschützt.                                      |
| verbleibende     | Int64  | Gesamter verbleibender Speicherplatz vor dem Erreichen des Speicherkontingents in Byte. Schreibgeschützt. |
| gelöscht       | Int64  | Gesamte Dateien genutzter Speicherplatz im Papierkorb in Byte. Schreibgeschützt.      |
| state         | string | Wert der Enumeration, die den Zustand des Speicherplatzes angibt. Schreibgeschützt. |

## <a name="state-enumeration"></a>Status Enumeration

| Wert      | Beschreibung                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | Das Laufwerk verfügt über ausreichend verbleibendes Kontingent.                                                                                                                               |
| `nearing`  | Verbleibendes Kontingent weniger als 10 % des gesamten Kontingentplatzes.                                                                                                                      |
| `critical` | Verbleibendes Kontingent weniger als 1 % des gesamten Kontingentplatzes.                                                                                                                       |
| `exceeded` | Das verwendete Kontingent hat das gesamte Kontingent überschritten. Neue Dateien oder Ordner können nicht hinzugefügt werden, wenn sie nicht unter dem Betrag für das Gesamtkontingent liegen oder mehr Speicherplatz erworben wird. |

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/quota.md:
      Found potential enums in resource example that weren't defined in a table:(normal, nearing,critical,exceeded) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Quota"
} -->
