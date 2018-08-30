---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
ms.openlocfilehash: 92882910ecf86d19e1f0a8a5767d148f5aa95775
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264035"
---
# <a name="hashes-resource-type"></a>Hash-Ressourcentyp

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
| **sha1Hash**     | Zeichenfolge | SHA1-Hash für den Inhalt der Datei (sofern zutreffend). Schreibgeschützt. |
| **crc32Hash**    | Zeichenfolge | Der Wert der CRC32 der Datei in little endian (sofern verfügbar). Schreibgeschützt.            |
| **quickXorHash** | Zeichenfolge | Ein proprietärer Hash der Datei, die verwendet werden kann, um festzustellen, ob sich der Inhalt der Datei (sofern zutreffend) geändert hat. Schreibgeschützt. |

**Hinweis:** In einigen Fällen stehen möglicherweise keine Hash-Werte zur Verfügung. Wenn dies der Fall ist, werden die Hash-Werte für ein Element nach dem Download des Elements aktualisiert.

## <a name="remarks"></a>Hinweise

In OneDrive for Business und SharePoint Server 2016 sind **sha1Hash** und **crc32Hash** nicht verfügbar.

In OneDrive Personal ist **quickXorHash** nicht verfügbar.

Wie Sie **quickXorHash** für eine Datei berechnen, bezieht sich dieser auf den [quickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm)-Codeausschnitt.
Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
