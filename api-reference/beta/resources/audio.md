---
author: VinodRavichandran
ms.date: 09/10/2017
title: Audio
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cd1f1af0e1ddcd1d56853c708da7ba03be740812
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573634"
---
# <a name="audio-facet"></a>Facet „Audio“

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die Ressource **Audio** führt audiobezogene Eigenschaften für ein Element in einer einzelnen Struktur zusammen.

Wenn ein [**DriveItem**](driveitem.md)-Element ein **file**-Facet ungleich Null aufweist, stellt das Element eine Audiodatei dar. Die Eigenschaften der **Audio**-Ressource werden durch Extrahieren von Metadaten aus der Datei aufgefüllt. 

## <a name="json-representation"></a>JSON-Darstellung

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.audio" } -->
```json
{
  "album": "string",
  "albumArtist": "string",
  "artist": "string",
  "bitrate": 128,
  "composers": "string",
  "copyright": "string",
  "disc": 0,
  "discCount": 0,
  "duration": 567,
  "genre": "string",
  "hasDrm": false,
  "isVariableBitrate": false,
  "title": "string",
  "track": 1,
  "trackCount": 16,
  "year": 2014
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname         | Typ    | Beschreibung                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| **album**             | string  | Der Titel des Albums, zu dem die Audiodatei gehört                          |
| **albumArtist**       | string  | Der Künstler, der für das Album genannt ist, zu dem die Audiodatei gehört                    |
| **artist**            | string  | Der zur Audiodatei gehörende Künstler                            |
| **bitrate**           | Int64   | Die Bitrate in KBit/s                                           |
| **composers**         | string  | Der Name des Komponisten der Audiodatei                          |
| **copyright**         | string  | Urheberrechtsinformationen zur Audiodatei                            |
| **disc**              | Int16   | Die Nummer der CD, von der die Audiodatei stammt                    |
| **discCount**         | Int16   | Die Gesamtanzahl von CDs im Album                             |
| **duration**          | Int64   | Die Dauer der Audiodatei in Millisekunden                |
| **genre**             | string  | Das Genre der Audiodatei                                        |
| **hasDrm**            | boolean | Angabe, ob die Datei DRM-geschützt ist (Digital Rights Management, Verwaltung digitaler Rechte)   |
| **isVariableBitrate** | boolean | Angabe, ob die Datei mit variabler Bitrate codiert ist            |
| **title**             | string  | Der Titel der Audiodatei                                         |
| **track**             | Int32   | Die Nummer des der Audiodatei entsprechenden Titels auf der Quell-CD    |
| **trackCount**        | Int32   | Die Gesamtanzahl von Audiotiteln auf der Quell-CD der Audiodatei |
| **year**              | Int32   | Das Jahr, in dem die Audiodatei aufgenommen wurde                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a>Bemerkungen

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).

<!--
{
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio",
  "suppressions": [
    "Error: /api-reference/beta/resources/audio.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
