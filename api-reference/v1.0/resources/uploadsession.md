---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
ms.openlocfilehash: fc03a25a790786c6d25d160a8b7f867c726dfc1b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860704"
---
# <a name="uploadsession-resource"></a>UploadSession-Ressource

Die **UploadSession**-Ressource enthält Informationen zum Hochladen von großen Dateien auf OneDrive, OneDrive for Business oder SharePoint-Dokumentbibliotheken.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "uploadUrl", "nextExpectedRanges" ],
  "@odata.type": "microsoft.graph.uploadSession"
}-->

```json
{
  "uploadUrl": "https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337",
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["0-"]
}
```

## <a name="properties"></a>Eigenschaften


| Eigenschaft       | Typ              |Beschreibung
|:-------------------|:------------------|:------------------------------------
| expirationDateTime | DateTimeOffset    | Datum und Uhrzeit in UTC, wenn die Upload Sitzung abläuft. Die vollständige Datei muss hochgeladen werden, bevor dieser Ablaufzeitpunkt erreicht wird.
| nextExpectedRanges | String collection | Eine Zusammenstellung von Bytebereichen, die dem Server für die Datei fehlen. Diese Bereiche sind Null indiziert und haben das Format "Anfang-Ende" (z. B. zeigt "0-26" die ersten 27 Bytes der Datei an).
| uploadUrl          | String            | Der URL-Endpunkt, der PUT-Anfragen für Bytebereiche der Datei akzeptiert.

## <a name="see-also"></a>Siehe auch

- [Hochladen großer Dateien mit einer Uploadsitzung](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->
