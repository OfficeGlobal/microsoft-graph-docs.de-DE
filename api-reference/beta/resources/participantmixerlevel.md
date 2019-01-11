---
title: Ressourcentyp participantMixerLevel
description: Konfiguration der Mixer Ebenen zur angegebenen audio-Teilnehmer
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 8a7b77c07240fbb5face70eb8ea21be55b85f1fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874137"
---
# <a name="participantmixerlevel-resource-type"></a>Ressourcentyp participantMixerLevel

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Konfiguration der Mixer Ebenen zur angegebenen audio-Teilnehmer

## <a name="properties"></a>Eigenschaften

| Eigenschaft               | Typ                                                      | Beschreibung                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| Vermeiden von                | [audioDuckingConfiguration](audioduckingconfiguration.md) | Konfiguration der benutzerdefinierte Mischung (welchen Phasen an- und Abmelden) andere Quellen für diese Teilnehmer zu vermeiden.       |
| exclusiveMode          | Boolean                                                   | Gibt an, ob von der Mischung Quellen ohne explizite Quellebene entfernt werden soll.                       |
| Teilnehmer            | String                                                    | Die Teilnehmer für den Mischer konfiguriert wird.                                             |
| sourceLevels           | [AudioSourceLevel](audiosourcelevel.md) -Auflistung        | Konfiguration für andere Datenquellen.                                                              |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.participantMixerLevel"
}-->
```json
{
  "ducking": { "@odata.type": "#microsoft.graph.audioDuckingConfiguration" },
  "exclusiveMode": true,
  "participant": "String",
  "sourceLevels": [ { "@odata.type": "#microsoft.graph.audioSourceLevel" } ]
}
```

## <a name="example---mixer-level"></a>Beispiel - Mixer-Ebene

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participantMixerLevel"
}-->
```json
{
  "ducking": {
    "@odata.type": "#microsoft.graph.audioDuckingParameters",
    "rampActive": 1000,
    "rampInactive": 1000,
    "lowerLevel": 20,
    "upperLevel": 100
  },
  "exclusiveMode": true,
  "participant": "123456W77E24E4D85F80597083CB830",
  "sourceLevels": [
    {
      "@odata.type": "#microsoft.graph.audioSourceLevel",
      "duckOthers": false,
      "level": 100,
      "participant": "8A34A46B3D174ADC8DCEDC4E7D572698"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participantMixerLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
