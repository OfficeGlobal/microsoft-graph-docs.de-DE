---
title: Rufen Sie Ressourcentyp
description: Die Ressource **aufrufen,** wird erstellt, wenn ein eingehender Anruf für die Anwendung vorhanden ist oder die Anwendung einen neuen ausgehenden Anruf über erstellt eine `POST` auf `app/calls`.
author: VinodRavichandran
localization_priority: Priority
ms.openlocfilehash: d2748b410352effb7119a569bdf48c86f2f7c2ad
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810703"
---
# <a name="call-resource-type"></a>Rufen Sie Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die Ressource **aufrufen,** wird erstellt, wenn ein eingehender Anruf für die Anwendung vorhanden ist oder die Anwendung einen neuen ausgehenden Anruf über erstellt eine `POST` auf `app/calls`.

Anrufe können als eine Peer-zu-Peer- oder als Gespräch mit mehreren Teilnehmern eingerichtet sein. Geben Sie zum Erstellen oder Verknüpfen eines Anrufs mit mehreren Teilnehmern, die `chatInfo` und `meetingInfo`. Wenn dies nicht angegeben werden, wird eine neue ad-hoc-Besprechung automatisch erstellt. Für einen eingehenden Anruf, tragen Sie diese Werte in einem Speicher hochverfügbare, sodass die Anwendung für den Anruf erneut an den Fall, dass die Anwendung stürzt ab.

Obwohl die gleiche Identität kann nicht mehrere Male eingeladen werden, ist es möglich, für eine Anwendung zur Teilnahme an der gleichen Besprechung mehrmals. Jedes Mal, wenn die Anwendung Joins Gespräch distinct `id` wird bereitgestellt, um dieses Aufrufs zur Besprechung. Es wird empfohlen, dass Sie separate Identitäten verwenden, an der Besprechung teilnehmen, damit die Clients wie die verschiedenen Teilnehmer anzeigen.

## <a name="methods"></a>Methoden

| Methode                                                            | Rückgabetyp                                       | Beschreibung                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [Abrufen von Anrufen](../api/call-get.md)                                    | [Anruf](call.md)                                   | Lesen Sie die Eigenschaften des Objekts **aufrufen** .      |
| [Delete](../api/call-delete.md)                                   |                                                   | Löschen oder Auflegen einer aktiven **aufrufen**.        |
| **Behandlung von Anrufen**                                                 |                                                   |                                              |
| [Antwort](../api/call-answer.md)                                   |                                                   | Beantworten eines eingehenden Anrufs an.                     |
| [Ablehnen](../api/call-reject.md)                                   |                                                   | Ablehnen eines eingehenden Anrufs an.                     |
| [Redirect](../api/call-redirect.md)                               |                                                   | Umleiten eines eingehenden Anrufs an.                   |
| [Transfer](../api/call-transfer.md)                               |                                                   | Weiterleiten eines Anrufs                              |
| **Mehrere Teilnehmer**                                                   |                                                   |                                              |
| [Liste Teilnehmer](../api/call-list-participants.md)             | [Teilnehmer](participant.md) -Auflistung          | Rufen Sie eine objektauflistung von Teilnehmer.         |
| [Einladen von Teilnehmern](../api/participant-invite.md)               | [commsOperation](commsoperation.md)               | Einladen von Teilnehmern zum aktiven Anruf.      |
| [Stummschalten Sie aller Teilnehmer](../api/participant-muteall.md)            | [commsOperation](commsoperation.md)               | Stummschalten Sie aller Teilnehmer in den Anruf.           |
| [Konfigurieren von Audiomixer](../api/participant-configuremixer.md)     | [commsOperation](commsoperation.md)               | Konfigurieren von Audio in der Unterhaltung mit mehreren Teilnehmern.  |
| [Erstellen von audioRoutingGroup](../api/call-post-audioroutinggroups.md)| [audioRoutingGroup](audioroutinggroup.md)         | Erstellen Sie eine neue AudioRoutingGroup, durch die Veröffentlichung auf der AudioRoutingGroups-Auflistung. |
| [Liste audioRoutingGroups](../api/call-list-audioroutinggroups.md) | [AudioRoutingGroup](audioroutinggroup.md) -Auflistung|Rufen Sie eine Auflistung der AudioRoutingGroup-Objekts.  |
| **Interaktive Sprachantwort**                                    |                                                   |                                              |
| [PlayPrompt](../api/call-playprompt.md)                           | [playPromptOperation](playpromptoperation.md)     | Wiedergabe Prompt in den Anruf.                     |
| [Record](../api/call-record.md)                                   | [recordOperation](recordoperation.md)             | Notieren Sie den Anruf.                             |
| [CancelMediaProcessing](../api/call-cancelmediaprocessing.md)     | [commsOperation](commsoperation.md)               | Medienverarbeitung abzubrechen.                     |
| [SubscribeToTone](../api/call-subscribetotone.md)                 | [commsOperation](commsoperation.md)               | Abonnieren Sie DTMF-Töne.                     |
| **Teilnehmerliste Self-Vorgänge**                                   |                                                   |                                              |
| [Stummschalten](../api/call-mute.md)                                       | [commsOperation](commsoperation.md)               | Stumm Zuschalten in den Anruf.                       |
| [Stummschaltung aufheben](../api/call-unmute.md)                                   | [commsOperation](commsoperation.md)               | Aktiviert self in den Anruf.                     |
| [UpdateMetadata](../api/call-updatemetadata.md)                   | [commsOperation](commsoperation.md)               | Aktualisieren Sie in der Teilnehmerliste einer Metadaten für sich selbst.          |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md) |                                                   | Starten Sie und beenden Sie die Freigabe Bildschirm in den Anruf                                             |

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ                                                                                                   | Beschreibung                                                                                                                                                                                         |
| :------------------ | :------------------------------------------------------------------------------------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| activeModalities    | Zeichenfolgenauflistung                                                                                      | Die Liste der aktiven Modalitäten. Mögliche Werte sind: `unknown`, `audio`, `video`, `videoBasedScreenSharing` und `data`. Schreibgeschützt. Server generiert wurde.                                                    |
| answeredBy          | [participantInfo](participantinfo.md)                                                                  | Der Teilnehmer, der den Anruf beantwortet. Schreibgeschützt. Server generiert wurde.                                                                                                                                |
| callRoutes          | [CallRoute](callroute.md) -Auflistung                                                                   | Die Routinginformationen wie der Anruf umgeleitet wurde. Schreibgeschützt. Server generiert wurde.                                                                                                                |
| callbackUri         | Zeichenfolge                                                                                                 | Der Rückruf oder Abonnement-ID auf dem Rückrufe zugestellt werden.                                                                                                                               |
| chatInfo            | [chatInfo](chatinfo.md)                                                                                | Die Chat-Informationen.                                                                                                                                                                               |
| Richtung           | Zeichenfolge                                                                                                 | Die Richtung des Anrufs. Die mögliche Werte sind `incoming` oder `outgoing`. Schreibgeschützt. Server generiert wurde.                                                                                            |
| id                  | Zeichenfolge                                                                                                 | Schreibgeschützt. Server generiert wurde.                                                                                                                                                                        |
| mediaConfig         | [AppHostedMediaConfig](apphostedmediaconfig.md) oder [serviceHostedMediaConfig](servicehostedmediaconfig.md) | Die Medienkonfiguration.                                                                                                                                                                        |
| meetingCapability   | [meetingCapability](meetingcapability.md)                                                              | Die Funktionen von einer Besprechung enthält.                                                                                                                                                             |
| meetingInfo         | [OrganizerMeetingInfo](organizermeetinginfo.md) oder [tokenMeetingInfo](tokenmeetinginfo.md)             | Die Informationen der Besprechung.                                                                                                                                                                            |
| myParticipantId     | Zeichenfolge                                                                                                 | Schreibgeschützt. Server generiert wurde.                                                                                                                                                                        |
| requestedModalities | Collection von Objekten des Typs „String“                                                                                      | Die Liste der angeforderten Modalitäten. | Mögliche Werte sind: `unknown`, `audio`, `video`, `videoBasedScreenSharing` und `data`.                                                                            |
| resultInfo          | [resultInfo](resultinfo.md)                                                                            | Informationen zu den Ergebnissen. Beispielsweise kann der Grund für die Beendigung enthalten. Schreibgeschützt. Server generiert wurde.                                                                                                       |
| ringingTimeoutInSeconds | Int32                                                                                              | Timeout für ausgehende Peer-zu-Peer-Anrufe Klingeln                                                                                                                                                     |
| routingPolicies     | Collection von Objekten des Typs „String“                                                                                      | Mögliche Werte: sind `none`, `noMissedCall`, `disableForwardingExceptPhone` und `disableForwarding`.                                                                                                   |
| source              | [participantInfo](participantinfo.md)                                                                  | Der Absender des Anrufs.                                                                                                                                                                         |
| state               | Zeichenfolge                                                                                                 | Der Zustand des Anrufs. Mögliche Werte: `incoming`, `establishing`, `ringing`, `established`, `hold`, `transferring`, `transferAccepted`, `redirecting`, `terminating`, `terminated`. Schreibgeschützt. Server generiert wurde.                         |
| Betreff             | Zeichenfolge                                                                                                 | Der Betreff der Unterhaltung.                                                                                                                                                                    |
| Ziele             | [ParticipantInfo](participantinfo.md) -Auflistung                                                       | Die Ziele des Anrufs.                                                                                                                                                                            |
| tenantId            | Zeichenfolge                                                                                                 | TenantId in Azure Active Directory.                                                                                                                                                                 |
| terminationReason   | Zeichenfolge                                                                                                 | Schreibgeschützt. Server generiert wurde.                                                                                                                                                                        |
| toneInfo            | [toneInfo](toneinfo.md)                                                                                | Schreibgeschützt. Server generiert wurde.                                                                                                                                                                        |

> Hinweis: Eigenschaften als markiert `Server generated` werden ignoriert, bei der Verarbeitung von `POST` auf `app/calls`.

## <a name="relationships"></a>Beziehungen

| Beziehung        | Typ                                                 | Beschreibung                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
| audioRoutingGroups  | [AudioRoutingGroup](audioroutinggroup.md) -Auflistung | Schreibgeschützt. Lässt Nullwerte zu.                                                |
| Vorgänge          | [CommsOperation](commsoperation.md) -Auflistung       | Schreibgeschützt. Lässt Nullwerte zu.                                                |
| participants        | [Teilnehmer](participant.md) -Auflistung             | Schreibgeschützt. Lässt Nullwerte zu.                                                |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "activeModalities",
    "answeredBy",
    "callRoutes",
    "chatInfo",
    "direction",
    "id",
    "meetingCapability",
    "meetingInfo",
    "myParticipantId",
    "resultInfo",
    "ringingTimeoutInSeconds",
    "routingPolicies",
    "state",
    "targets",
    "tenantId",
    "terminationReason",
    "toneInfo"
  ],
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "activeModalities": ["unknown | audio | video | videoBasedScreenSharing | data"],
  "answeredBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "callRoutes": [{"@odata.type": "#microsoft.graph.callRoute"}],
  "callbackUri": "String",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "direction": "incoming | outgoing",
  "id": "String (identifier)",
  "mediaConfig": {"@odata.type": "#microsoft.graph.mediaConfig"},
  "meetingCapability": {"@odata.type": "#microsoft.graph.meetingCapability"},
  "meetingInfo": {"@odata.type": "#microsoft.graph.meetingInfo"},
  "myParticipantId": "String",
  "requestedModalities": ["unknown | audio | video | videoBasedScreenSharing | data"],
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "ringingTimeoutInSeconds": 1024,
  "routingPolicies": ["none | noMissedCall | disableForwardingExceptPhone | disableForwarding"],
  "source": {"@odata.type": "#microsoft.graph.participantInfo"},
  "state": "incoming | establishing | ringing | established | hold | transferring | transferAccepted | redirecting | terminating | terminated",
  "subject": "String",
  "targets": [{"@odata.type": "#microsoft.graph.participantInfo"}],
  "tenantId": "String",
  "terminationReason": "String",
  "toneInfo": {"@odata.type": "#microsoft.graph.toneInfo"}
}
```

> **Hinweis:** Join-URL aus einer Besprechung, die mit Microsoft-Teams, werden Sie feststellen. So extrahieren Sie die Daten aus der URL und die Füllung `chatInfo` und `meetingInfo`.

```http
https://teams.microsoft.com/l/meetup-join/19%3ameeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%224b444206-207c-42f8-92a6-e332b41c88a2%22%7d
decodes to:
https://teams.microsoft.com/l/meetup-join/19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2/0?context={"Tid":"72f988bf-86f1-41af-91ab-2d7cd011db47","Oid":"4b444206-207c-42f8-92a6-e332b41c88a2"}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call",
  truncated: true
}-->
```json
{
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "id": "4b444206-207c-42f8-92a6-e332b41c88a2"
      }
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
