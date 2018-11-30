---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Video
ms.openlocfilehash: a9bf228d814526d089fb102444e6952558b07e1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064941"
---
# <a name="video-resource-type"></a>Video-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
| **audioFormat**           | string | Name des Audioformats (AAC, MP3 usw.).
| **audioSamplesPerSecond** | Int32  | Anzahl der Audiosamples pro Sekunde.
| **bitrate**               | Int32  | Bitrate des Videos in Bits pro Sekunde.
| **duration**              | Int64  | Dauer der Datei in Millisekunden.
| **fourCC**                | string | „Vier Zeichencode“-Name des Videoformats.
| **framerate**             | double | Framerate des Videos.
| **height**                | Int32  | Die Höhe des Videos in Pixel.
| **width**                 | Int32  | Die Breite des Videos in Pixel.

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a>Bemerkungen

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).





<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": ""
}-->
