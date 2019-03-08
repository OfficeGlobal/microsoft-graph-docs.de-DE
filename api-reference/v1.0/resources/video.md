---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Video
localization_priority: Normal
ms.openlocfilehash: deba8cccb5f0ab80ca03395ef9f798719d542b8d
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480803"
---
# <a name="video-resource-type"></a>Video-Ressourcentyp

Die **Video**-Ressource gruppiert videobezogene Datenelemente in einer einzelnen Struktur.

Wenn ein [**DriveItem**](driveitem.md) ein **video**-Facet ungleich Null aufweist, stellt das Element eine Videodatei dar. Die Eigenschaften der **Video**-Ressource werden durch Extrahieren von Metadaten aus der Datei aufgefüllt.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.video"
}-->

```json
{
  "audioBitsPerSample": 16,
  "audioChannels": 1,
  "audioFormat": "AAC",
  "audioSamplesPerSecond": 44100,
  "bitrate": 39101896,
  "duration": 8053,
  "fourCC": "H264",
  "frameRate": 239.877,
  "height": 1280,
  "width": 720
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname             | Typ   | Beschreibung
|:--------------------------|:-------|:----------------------------------------
| **audioBitsPerSample**    | Int32  | Anzahl von Audiobits pro Sample.
| **audioChannels**         | Int32  | Anzahl der Audiokanäle.
| **audioFormat**           | Zeichenfolge | Name des Audioformats (AAC, MP3 usw.).
| **audioSamplesPerSecond** | Int32  | Anzahl der Audiosamples pro Sekunde.
| **bitrate**               | Int32  | Bitrate des Videos in Bits pro Sekunde.
| **duration**              | Int64  | Dauer der Datei in Millisekunden.
| **fourCC**                | string | „Vier Zeichencode“-Name des Videoformats.
| **frameRate**             | double | Framerate des Videos.
| **height**                | Int32  | Die Höhe des Videos in Pixel.
| **width**                 | Int32  | Die Breite des Videos in Pixel.

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a>Bemerkungen

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "Facets/Video"
} -->
