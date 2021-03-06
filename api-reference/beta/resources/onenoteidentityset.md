---
title: Ressourcentyp oneNoteIdentitySet
description: '**Unterstützung in Kürze verfügbar**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: e149d5548ce3585bbcda1f0a199fa97d7543af77
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642471"
---
# <a name="onenoteidentityset-resource-type"></a>Ressourcentyp oneNoteIdentitySet

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Unterstützung in Kürze verfügbar**

Der OneNoteIdentitySet-Typ ist eine verschlüsselte Auflistung von [OneNoteIdentity](onenoteidentity.md) -Objekten.
Es wird verwendet, um einen Satz von Identitäten zugeordnet sind verschiedene Ereignisse für einen _Notizbuch_, einem _Bereich_ oder einer _Seite_, z. B. _von erstellt_ oder _zuletzt geändert von_darstellen. 
 
Aktuell enthält einen einzelnen Schlüssel, _**Benutzer**_.  In Zukunft können die Schlüssel wie das Gerät oder einer Anwendung das Element hinzugefügt werden.

In Zukunft werden sollen dieses Typs mit [IdentitySet](identityset.md) zusammengeführt

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.oneNoteIdentity"}
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|user|[oneNoteIdentity](onenoteidentity.md)|Eine OneNoteIdentity-Ressource, die einen Benutzer darstellt.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteidentityset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
