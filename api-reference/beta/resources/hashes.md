---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Hashes
localization_priority: Normal
ms.openlocfilehash: 551b09cee9fa662d357ee763b67ce78bea03425f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514845"
---
# <a name="hashes-resource-type"></a>Hash-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **Hashes**-Ressourcengruppen machen Hashes in einer einzelnen Struktur für ein Element verfügbar.

**Hinweis:** Nicht alle Dienste geben einen Wert für alle aufgeführten Hash-Eigenschaften an.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "sha1Hash", "crc32Hash", "quickXorHash" ],
  "@odata.type": "microsoft.graph.hashes"
}-->

```json
{
  "crc32Hash": "string (hex)",
  "sha1Hash": "string (hex)",
  "quickXorHash": "string (base64)"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft         | Typ   | Beschreibung                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| **sha1Hash**     | String | SHA1-Hash für den Inhalt der Datei (sofern zutreffend). Schreibgeschützt. |
| **crc32Hash**    | String | Der Wert der CRC32 der Datei (sofern zutreffend). Schreibgeschützt.            |
| **quickXorHash** | String | Ein proprietärer Hash der Datei, die verwendet werden kann, um festzustellen, ob sich der Inhalt der Datei (sofern zutreffend) geändert hat. Schreibgeschützt. |

**Hinweis:** In einigen Fällen stehen möglicherweise keine Hash-Werte zur Verfügung. Wenn dies der Fall ist, werden die Hash-Werte für ein Element nach dem Download des Elements aktualisiert.

## <a name="remarks"></a>Hinweise

In OneDrive for Business und SharePoint Server 2016 sind **sha1Hash** und **crc32Hash** nicht verfügbar.

In OneDrive Personal ist **quickXorHash** nicht verfügbar.

Wie Sie **quickXorHash** für eine Datei berechnen, bezieht sich dieser auf den [quickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm)-Codeausschnitt.

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).


<!--
{
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes",
  "suppressions": [
    "Error: /api-reference/beta/resources/hashes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
