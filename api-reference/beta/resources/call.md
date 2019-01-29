---
title: call-Ressourcentyp
description: Die **call**-Ressource wird erstellt, wenn es einen eingehenden Anruf für die Anwendung gibt oder die Anwendung einen neuen ausgehenden Anruf über `POST` in `app/calls` erstellt.
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: a7eb47d65d07cbdb88712a3b71b7de24b7d366cc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572962"
---
# <a name="call-resource-type"></a>call-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **call**-Ressource wird erstellt, wenn es einen eingehenden Anruf für die Anwendung gibt oder die Anwendung einen neuen ausgehenden Anruf über `POST` in `app/calls` erstellt.

Anrufe können als Peer-to-Peer-Anruf oder als Anruf mit mehreren Teilnehmern eingerichtet werden. Geben Sie zum Erstellen oder Beitreten eines Anrufs mit mehreren Teilnehmern `chatInfo` und `meetingInfo` an. Wenn Sie diese Informationen nicht angeben, wird automatisch eine neue Ad-hoc-Besprechung erstellt. Zeichnen Sie diese Werte für einen eingehenden Anruf in einem hoch verfügbaren Speicher auf, damit die Anwendung dem Anruf erneut beitreten kann, falls sie abstürzt.

Dieselbe Identität kann zwar nicht mehrere Male verwendet werden, eine Anwendung kann aber derselben Besprechung mehrere Male beitreten. Jedes Mal, wenn die Anwendung beitritt, wird ein anderer Anruf `id` für diesen Anruf für die Besprechung bereitgestellt. Es wird empfohlen, dass Sie separate Identitäten verwenden, um an der Besprechung teilzunehmen, damit diese in den Clients als unterschiedliche Teilnehmer angezeigt werden.

## <a name="methods"></a>Methoden

| Methode                                                            | Rückgabetyp                                       | Beschreibung                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [Get call](../api/call-get.md)                                    | [call](call.md)                                   | Lesen der Eigenschaften des **call**-Objekts.      |
| [Delete](../api/call-delete.md)                                   |                                                   | Löschen oder Auflegen eines aktiven **Anrufs**.        |
| **Anrufverarbeitung**                                                 |                                                   |                                              |
| [Answer](../api/call-answer.md)                                   |                                                   | Beantworten eines eingehenden Anrufs.                     |
| [Reject](../api/call-reject.md)                                   |                                                   | Ablehnen eines eingehenden Anrufs.                     |
| [Redirect](../api/call-redirect.md)                               |                                                   | Umleiten eines eingehenden Anrufs.                   |
| [Transfer](../api/call-transfer.md)                               |                                                   | Weiterleiten eines Anrufs.                              |
| **Mehrere Teilnehmer**                                                   |                                                   |                                              |
| [List participants](../api/call-list-participants.md)             | [participant](participant.md)-Auflistung          | Abrufen einer Auflistung von Teilnehmerobjekten.         |
| [Invite Participants](../api/participant-invite.md)               | [commsOperation](commsoperation.md)               | Einladen von Teilnehmern zum aktiven Anruf.      |
| [Mute All Participants](../api/participant-muteall.md)            | [commsOperation](commsoperation.md)               | Stummschalten aller Teilnehmer in dem Anruf.           |
| [Configure Audio Mixer](../api/participant-configuremixer.md)     | [commsOperation](commsoperation.md)               | Konfigurieren von Audio in der Unterhaltung mit mehreren Teilnehmern.  |
| [Create audioRoutingGroup](../api/call-post-audioroutinggroups.md)| [audioRoutingGroup](audioroutinggroup.md)         | Erstellen einer neuen audioRoutingGroup durch Veröffentlichen in der audioRoutingGroup-Auflistung. |
| [List audioRoutingGroups](../api/call-list-audioroutinggroups.md) | [audioRoutingGroup](audioroutinggroup.md)-Auflistung|Abrufen einer aAudioRoutingGroup-Objektauflistung.  |
| **Interactive-Voice-Response**                                    |                                                   |                                              |
| [PlayPrompt](../api/call-playprompt.md)                           | [playPromptOperation](playpromptoperation.md)     | Wiedergabeaufforderung in dem Anruf.                     |
| [Record](../api/call-record.md)                                   | [recordOperation](recordoperation.md)             | Aufzeichnen des Anrufs.                             |
| [CancelMediaProcessing](../api/call-cancelmediaprocessing.md)     | [commsOperation](commsoperation.md)               | Abbrechen der Medienverarbeitung.                     |
| [SubscribeToTone](../api/call-subscribetotone.md)                 | [commsOperation](commsoperation.md)               | Abonnieren von DTMF-Tönen.                     |
| **Self Participant Operations**                                   |                                                   |                                              |
| [Mute](../api/call-mute.md)                                       | [commsOperation](commsoperation.md)               | Sich selbst stummschalten in dem Anruf.                       |
| [Unmute](../api/call-unmute.md)                                   | [commsOperation](commsoperation.md)               | Stummschaltung für sich selbst in dem Anruf aufheben.                     |
| [UpdateMetadata](../api/call-updatemetadata.md)                   | [commsOperation](commsoperation.md)               | Aktualisieren der Metadaten für sich selbst in der Teilnehmerliste.          |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md) |                                                   | Starten und Beenden des Freigabebildschirms in dem Anruf.                                             |

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ                                                                                                   | Beschreibung                                                                                                                                                                                         |
| :------------------ | :------------------------------------------------------------------------------------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| activeModalities    | „modality“-Auflistung                                                                                      | Die Liste der aktiven Modalitäten. Mögliche Werte: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`. Schreibgeschützt. Vom Server generiert.                                                    |
| answeredBy          | [participantInfo](participantinfo.md)                                                                  | Der Teilnehmer, der den Anruf angenommen hat. Schreibgeschützt. Vom Server generiert.                                                                                                                                |
| callRoutes          | [callRoute](callroute.md)-Auflistung                                                                   | Die Routinginformationen, wie der Anruf umgeleitet wurde. Schreibgeschützt. Vom Server generiert.                                                                                                                |
| callbackUri         | Zeichenfolge                                                                                                 | Die Rückruf- oder Abonnement-ID für Rückrufe.                                                                                                                               |
| chatInfo            | [chatInfo](chatinfo.md)                                                                                | Die Chatinformationen.                                                                                                                                                                               |
| direction           | callDirection                                                                                          | Die Richtung des Anrufs. Die möglichen Werte sind: `incoming` oder `outgoing`. Schreibgeschützt. Vom Server generiert.                                                                                            |
| id                  | String                                                                                                 | Schreibgeschützt. Vom Server generiert.                                                                                                                                                                        |
| mediaConfig         | [mediaConfig](mediaconfig.md)                                                                          | Die Medienkonfiguration.                                                                                                                                                                        |
| meetingCapability   | [meetingCapability](meetingcapability.md)                                                              | Enthält die Funktionen einer Besprechung.                                                                                                                                                             |
| meetingInfo         | [meetingInfo](meetinginfo.md)                                                                          | Die Besprechungsinformationen.                                                                                                                                                                            |
| myParticipantId     | Zeichenfolge                                                                                                 | Schreibgeschützt. Vom Server generiert.                                                                                                                                                                        |
| requestedModalities | „modality“-Auflistung                                                                                      | Die Liste der angeforderten Modalitäten. | Mögliche Werte: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.                                                                            |
| resultInfo          | [resultInfo](resultinfo.md)                                                                            | Die Ergebnisinformationen. Kann beispielsweise einen Grund für die Beendigung enthalten. Schreibgeschützt. Vom Server generiert.                                                                                                       |
| ringingTimeoutInSeconds | Int32                                                                                              | Timeout für Rufzeichen für ausgehende Peer-to-Peer-Anrufe                                                                                                                                                     |
| routingPolicies     | „routingPolicy“-Auflistung                                                                                      | Mögliche Werte: `none`, `noMissedCall`, `disableForwardingExceptPhone`, `disableForwarding`                                                                                                   |
| source              | [participantInfo](participantinfo.md)                                                                  | Ursprung des Anrufs.                                                                                                                                                                         |
| state               | callState                                                                                                 | Der Anrufstatus. Mögliche Werte: `incoming`, `establishing`, `ringing`, `established`, `hold`, `transferring`, `transferAccepted`, `redirecting`, `terminating`, `terminated`. Schreibgeschützt. Vom Server generiert.                         |
| subject             | Zeichenfolge                                                                                                 | Der Betreff der Unterhaltung.                                                                                                                                                                    |
| targets             | [participantInfo](participantinfo.md)-Auflistung                                                       | Die Ziele des Anrufs.                                                                                                                                                                            |
| tenantId            | Zeichenfolge                                                                                                 | Mandanten-ID in Azure Active Directory.                                                                                                                                                                 |
| terminationReason   | Zeichenfolge                                                                                                 | Schreibgeschützt. Vom Server generiert.                                                                                                                                                                        |
| toneInfo            | [toneInfo](toneinfo.md)                                                                                | Schreibgeschützt. Vom Server generiert.                                                                                                                                                                        |

> Hinweis: Eigenschaften, die als `Server generated` gekennzeichnet sind, werden bei der Verarbeitung von `POST` in `app/calls` ignoriert.

## <a name="relationships"></a>Beziehungen

| Beziehung        | Typ                                                 | Beschreibung                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
| audioRoutingGroups  | [audioRoutingGroup](audioroutinggroup.md)-Auflistung | Schreibgeschützt. Nullwerte zulassend.                                                |
| operations          | [commsOperation](commsoperation.md)-Auflistung       | Schreibgeschützt. Nullwerte zulassend.                                                |
| participants        | [participant](participant.md)-Auflistung             | Schreibgeschützt. Nullwerte zulassend.                                                |

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
    "mediaConfig",
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
  "activeModalities": ["modality"],
  "answeredBy": {"@odata.type": "microsoft.graph.participantInfo"},
  "callRoutes": [{"@odata.type": "microsoft.graph.callRoute"}],
  "callbackUri": "String",
  "chatInfo": {"@odata.type": "microsoft.graph.chatInfo"},
  "direction": "callDirection",
  "id": "String (identifier)",
  "mediaConfig": {"@odata.type": "microsoft.graph.mediaConfig"},
  "meetingCapability": {"@odata.type": "microsoft.graph.meetingCapability"},
  "meetingInfo": {"@odata.type": "microsoft.graph.meetingInfo"},
  "myParticipantId": "String",
  "requestedModalities": ["modality"],
  "resultInfo": {"@odata.type": "microsoft.graph.resultInfo"},
  "ringingTimeoutInSeconds": 1024,
  "routingPolicies": ["routingPolicy"],
  "source": {"@odata.type": "microsoft.graph.participantInfo"},
  "state": "callState",
  "subject": "String",
  "targets": [{"@odata.type": "microsoft.graph.participantInfo"}],
  "tenantId": "String",
  "terminationReason": "String",
  "toneInfo": {"@odata.type": "microsoft.graph.toneInfo"}
}
```

> **Hinweis:** In einer mit Microsoft Teams geplanten Besprechung finden Sie eine Teilnahme-URL. So extrahieren Sie die Daten aus der URL und füllen `chatInfo` und `meetingInfo`.

```http
https://teams.microsoft.com/l/meetup-join/19%3ameeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%224b444206-207c-42f8-92a6-e332b41c88a2%22%7d
decodes to:
https://teams.microsoft.com/l/meetup-join/19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2/0?context={"Tid":"72f988bf-86f1-41af-91ab-2d7cd011db47","Oid":"4b444206-207c-42f8-92a6-e332b41c88a2"}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call",
  "truncated": true
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
<!--
{
  "type": "#page.annotation",
  "description": "call resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/call.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
