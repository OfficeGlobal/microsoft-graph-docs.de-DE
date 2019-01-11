---
title: Teilnehmerliste Ressourcentyp
description: Der Typ Teilnehmer.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: c125589506dbd529d2b45df4171e9d54b346cbba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869832"
---
# <a name="participant-resource-type"></a>Teilnehmerliste Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Der Typ Teilnehmer.

## <a name="methods"></a>Methoden

| Methode                                                          | Rückgabetyp                              | Beschreibung                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [Abrufen der Teilnehmer](../api/participant-get.md)                    | [Teilnehmer](participant.md)            | Lesen Sie die Eigenschaften des **Teilnehmers** -Objekts.    |
| [ConfigureMixer](../api/participant-configuremixer.md)          | [commsOperation](commsoperation.md)      | Konfigurieren Sie den Teilnehmerliste Audiomixer.            |
| [Einladen](../api/participant-invite.md)                          | [commsOperation](commsoperation.md)      | Einladen eines Teilnehmers zu den Anruf.                 |
| [Stummschalten von Teilnehmern](../api/participant-mute.md)                  | [commsOperation](commsoperation.md)      | Stummschalten eines Teilnehmers im Gespräch.                     |
| [Stummschalten Sie aller Teilnehmer](../api/participant-muteall.md)          | [commsOperation](commsoperation.md)      | Stummschalten Sie aller Teilnehmer an der Besprechung.         |

## <a name="properties"></a>Eigenschaften

| Eigenschaft             | Typ                                     | Beschreibung                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| id                   | Zeichenfolge                                   | Die Teilnehmer-Id.                                          |
| Info                 | [participantInfo](participantinfo.md)    | Die Teilnehmer des Teilnehmers.                          |
| isInLobby            | Boolean                                  | True, wenn der Teilnehmer in der Lobby ist                          |
| isMuted              | Boolean                                  | True, wenn der Teilnehmer stumm geschaltet ist (Client oder Server stumm geschaltet)    |
| mediaStreams         | [MediaStream](mediastream.md) -Auflistung | Die Liste der Mediendatenströme.                                   |
| Metadaten             | Zeichenfolge                                   | Blob-Daten von den Teilnehmer in der Teilnehmerliste einer     |
| recordingInfo        | [recordingInfo](recordinginfo.md)        | Informationen zu gibt an, ob der Teilnehmer Aufzeichnung Funktionalität verfügt. |

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "String (identifier)",
  "info": {"@odata.type": "#microsoft.graph.participantInfo"},
  "isInLobby": true,
  "isMuted": true,
  "mediaStreams": [ { "@odata.type": "#microsoft.graph.mediaStream" } ],
  "metadata": "String",
  "recordingInfo": { "@odata.type": "#microsoft.graph.recordingInfo" }
}
```

## <a name="example"></a>Beispiel

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "info": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "en-US",
    "region": "westus"
  },
  "isInLobby": false,
  "isMuted": false,
  "mediaStreams": [
    {
      "sourceId": "1",
      "direction": "sendReceive",
      "label": "main-audio",
      "mediaType": "audio",
      "serverMuted": false
    }
  ],
  "metadata": "metadata-value",
  "recordingInfo": {
    "status": "recordingCapable"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
