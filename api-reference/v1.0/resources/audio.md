---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Audio
ms.openlocfilehash: e68b70565f0eccd7847fba2b8085661071a75ae7
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23266233"
---
# <a name="audio-facet"></a>Audio-Facet

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
| **album**             | Zeichenfolge  | Der Titel des Albums, zu dem die Audiodatei gehört                          |
| **albumArtist**       | Zeichenfolge  | Der Künstler, der für das Album genannt ist, zu dem die Audiodatei gehört                    |
| **artist**            | Zeichenfolge  | Der zur Audiodatei gehörende Künstler                            |
| **bitrate**           | Int64   | Die Bitrate in KBit/s                                           |
| **composers**         | Zeichenfolge  | Der Name des Komponisten der Audiodatei                          |
| **copyright**         | Zeichenfolge  | Urheberrechtsinformationen zur Audiodatei                            |
| **disc**              | Int16   | Die Nummer der CD, von der die Audiodatei stammt.                    |
| **discCount**         | Int16   | Die Gesamtanzahl von CDs im Album                             |
| **duration**          | Int64   | Die Dauer der Audiodatei in Millisekunden                |
| **genre**             | Zeichenfolge  | Das Genre der Audiodatei                                        |
| **hasDrm**            | boolean | Angabe, ob die Datei DRM-geschützt ist (Digital Rights Management, Verwaltung digitaler Rechte)   |
| **isVariableBitrate** | boolean | Angabe, ob die Datei mit variabler Bitrate codiert ist            |
| **title**             | Zeichenfolge  | Der Titel der Audiodatei                                         |
| **track**             | Int32   | Die Nummer des der Audiodatei entsprechenden Titels auf der Quell-CD    |
| **trackCount**        | Int32   | Die Gesamtanzahl von Audiotiteln auf der Quell-CD der Audiodatei |
| **year**              | Int32   | Das Jahr, in dem die Audiodatei aufgenommen wurde                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a>Bemerkungen

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
