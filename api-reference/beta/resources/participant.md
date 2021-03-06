---
title: Teilnehmerliste Ressourcentyp
description: Der Typ Teilnehmer.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f49526824b2b6c4eb4a5065f05ab4c765d299faa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508146"
---
# <a name="participant-resource-type"></a>Teilnehmerliste Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| id                   | String                                   | Die Teilnehmer-Id.                                          |
| Info                 | [participantInfo](participantinfo.md)    | Die Teilnehmer des Teilnehmers.                          |
| isInLobby            | Boolescher Wert                                  | True, wenn der Teilnehmer in der Lobby ist                          |
| isMuted              | Boolescher Wert                                  | True, wenn der Teilnehmer stumm geschaltet ist (Client oder Server stumm geschaltet)    |
| mediaStreams         | [MediaStream](mediastream.md) -Auflistung | Die Liste der Mediendatenströme.                                   |
| $metadata             | String                                   | Blob-Daten von den Teilnehmer in der Teilnehmerliste einer     |
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
<!--
{
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/participant.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
