---
title: Ressourcentyp onlineMeeting
description: Erfasst Informationen zu der Besprechung, einschließlich der Join-URL, die Teilnehmerliste und die Beschreibung an.
author: VinodRavichandran
ms.openlocfilehash: 3a2b26ac212bd7a77428dab9f5618db8165de65b
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380478"
---
# <a name="onlinemeeting-resource-type"></a>Ressourcentyp onlineMeeting

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Erfasst Informationen zu der Besprechung, einschließlich der Join-URL, die Teilnehmerliste und die Beschreibung an.

## <a name="methods"></a>Methoden

| Methode         | Rückgabetyp | Beschreibung |
|:---------------|:--------|:----------|
| [Abrufen von onlineMeeting](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | Lesen Sie Eigenschaften und Beziehungen OnlineMeeting-Objekts. |

## <a name="properties"></a>Eigenschaften

| Eigenschaft                  | Typ                                                   | Beschreibung                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| accessLevel               | Zeichenfolge                                                 | Die Zugriffsebene, die Zulassung der online-Besprechung steuert. Mögliche Werte sind: `everyone`, `invited`, `locked`, `sameEnterprise` und `unknown`. |
| audioConferencing         | [audioConferencing](audioconferencing.md)              | Stellt Access Telefoninformationen für einen OnlineMeeting. |
| canceledDateTime          | DateTime                                               | Der Zeitpunkt, wann die Besprechung abgebrochen wurde. |
| chatInfo                  | [chatInfo](chatinfo.md)                                | Die Chat diese Besprechung zugeordnet. |
| creationDateTime          | DateTime                                               | Die Uhrzeit der Erstellung die Besprechung. ReadOnly.
| endDateTime               | DateTime                                               | Die Endzeit der Besprechung. |
| entryExitAnnouncement     | Boolescher Wert                                                | Der Anwesenheitsstatus des Ankündigungen für die onlinebesprechung. Wenn die Anwesenheit Ankündigungen aktiviert sind, wird die online-Besprechung den Namen der Verknüpfung Participantswho die Besprechung per Audio-ankündigen. |
| expirationDateTime        | DateTime                                               | Absolute (Coordinated Universal Time, UTC) Datum und Uhrzeit nach dem kann die onlinebesprechung gelöscht werden. Datum und Uhrzeit müssen zwischen ein Jahr vor und zehn Jahren nach dem das aktuelle Datum und die Uhrzeit auf dem Server sein. |
| id                        | Zeichenfolge                                                 | Die ID der online-Besprechung zugeordnet. In einer HTTP GET-Anforderung verwendet wird, als ID zu. Schreibgeschützt. Server generiert wurde. |
| isCancelled               | Boolean                                                | Gibt an, ob die Besprechung abgebrochen wurde. |
| joinUrl                   | Zeichenfolge                                                 | Die URL, die verwendet wird, wenn die onlinebesprechung aus dem Internet verbunden ist. |
| meetingType               | Zeichenfolge                                                 | Mögliche Werte sind: `meetNow`, `scheduled`, `recurring`,`broadcast` |
| participants              | [meetingParticipants](meetingparticipants.md)          | Die Teilnehmer der Besprechung online zugeordnet.  Dazu gehören der Organisator und die Teilnehmer. |
| startDateTime             | DateTime                                               | Startzeit der Besprechung. |
| Betreff                   | Zeichenfolge                                                 | Der Betreff der onlinebesprechung. |

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "accessLevel": "everyone | invited | locked | sameEnterprise",
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "canceledDateTime": "String (timestamp)",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "entryExitAnnouncement": true,
  "expirationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "isCancelled": false,
  "joinUrl": "String",
  "meetingType": "meetNow | scheduled | recurring | broadcast",
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
