---
title: Arbeiten mit der API für Anrufe und Onlinebesprechungen in Microsoft Graph
description: Durch die API für Anrufe und Onlinebesprechungen von Microsoft Graph werden die Interaktionsmöglichkeiten Ihrer Apps und Dienste mit Benutzern um Sprach- und Videofeatures erweitert. Mit der API können Sie Anrufe erstellen und Anrufe von Benutzern und Anwendungen in Microsoft Teams erhalten. Mit diesen APIs können Sie eine Dienstanwendung (Bot) erstellen, die als Teilnehmer an einem Anruf oder einer Besprechung agieren kann.
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: ab01bc71ccb4f7490a60c47712198f72032fc157
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525150"
---
# <a name="working-with-the-calls-and-online-meetings-api-in-microsoft-graph"></a>Arbeiten mit der API für Anrufe und Onlinebesprechungen in Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Durch die API für Anrufe und Onlinebesprechungen von Microsoft Graph werden die Interaktionsmöglichkeiten Ihrer Apps und Dienste mit Benutzern um Sprach- und Videofeatures erweitert. Mit der API können Sie Anrufe erstellen und Anrufe von Benutzern und Anwendungen in Microsoft Teams erhalten. Mit diesen APIs können Sie eine Dienstanwendung (Bot) erstellen, die als Teilnehmer an einem Anruf oder einer Besprechung agieren kann.

## <a name="call-types"></a>Anruftypen

Anrufe werden als Peer-to-Peer-Anrufe oder Anrufe mit mehreren Teilnehmern kategorisiert. Ein Benutzer kann einen Peer-to-Peer-Anruf mit Ihrem Bot starten oder den Bot zu einer bestehenden Konferenz mit mehreren Teilnehmern einladen. Es sind keine Berechtigungen erforderlich, wenn der Benutzer den Bot zu einem Peer-to-Peer-Aufruf einlädt. Damit Ihr Bot an einem Gespräch mit mehreren Teilnehmern teilnehmen kann, muss er vom Mandantenadministrator die Berechtigung zur Teilnahme an einem Gruppenanruf erhalten.

![Abbildung mit Peer-to-Peer-Anruf und Anruf mit mehreren Teilnehmern](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/call-types.png)

Wenn der Bot den Anruf erstellt, muss er entweder die Berechtigung zum Initiieren eines Anrufs oder zum Initiieren eines Gruppenanrufs haben. Ihr Bot hat die Möglichkeit, Peer-to-Peer-Anrufe oder Anrufe mit mehreren Teilnehmern zu erstellen.

- Für einen Peer-to-Peer-Anruf muss der Bot nur ein Ziel und keine Besprechungskoordinaten angeben. 
- Wenn Ihr Bot einen Anruf mit mehreren Teilnehmern initiiert, wird hinter den Kulissen eine Ad-hoc-Besprechung eingerichtet, der alle Personen beitreten. Falls Besprechungskoordinaten angegeben werden, wird ein Anruf mit mehreren Teilnehmern eingerichtet, auch wenn nur ein Ziel vorhanden ist.

Ein Anruf kann als Peer-to-Peer-Anruf beginnen und zu einem Anruf mit mehreren Teilnehmern eskaliert werden. Es wird automatisch eine Konferenz bereitgestellt, und das Medium wird auf die Konferenz als neues Ziel umgeleitet. Ihr Bot kann die Eskalation initiieren, indem er andere Teilnehmer einlädt, sofern der Bot die Berechtigung zum Initiieren von Gruppenanrufen besitzt. Wenn die Eskalation von einem anderen Teilnehmer eingeleitet wird und der Bot keine Berechtigung zum Teilnehmen an Gruppenanrufen besitzt, wird der Bot aus dem Anruf entfernt.

> **Wichtig:** Wenn ein Anruf von einem Peer-to-Peer-Anruf zu einem Anruf mit mehreren Teilnehmern eskaliert wird, sind nicht alle Features für mehrere Teilnehmer verfügbar. Insbesondere empfängt der Bot keine Listenupdates.

## <a name="signaling"></a>Signalisierung

### <a name="incoming-call"></a>Eingehender Anruf

Um einen eingehenden Anruf empfangen zu können, müssen Sie den anrufenden Bot registrieren. Wenn der Bot die eingehende Benachrichtigung erhält, hat er die folgenden Optionen.

| Methode                              | Beschreibung                                  |
|:------------------------------------|:---------------------------------------------|
| [Antworten](../api/call-answer.md)     | Annehmen des eingehenden Anrufs.                    |
| [Ablehnen](../api/call-reject.md)     | Ablehnen des Anrufs und Auflegen.                  |
| [Umleiten](../api/call-redirect.md) | Umleitung des Anrufs.                           |

Der Bot kann den Aufruf zu einem anderen Benutzer oder einem Bot umleiten. Der Bot kann ihn auch an die Voicemail eines Benutzers umleiten.

![Abbildung mit einem Bot, der einen Anruf an eine Voicemail umleitet](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/call-handling.png)

> **Wichtig:** Das Umleiten oder Tätigen ausgehender Anrufe an PSTN wird derzeit nicht unterstützt.

### <a name="in-call"></a>Während des Anrufs

Vorgänge für den Bot sind im Anrufobjekt verfügbar. Diese wirken sich auf den Bot als Teilnehmer am Anruf aus.

| Methode                                                            | Beschreibung                                  |
|:------------------------------------------------------------------|:---------------------------------------------|
| [Mute](../api/call-mute.md)                                       | Sich selbst im Anruf stummschalten.                       |
| [Unmute](../api/call-unmute.md)                                   | Stummschaltung für sich selbst in dem Anruf aufheben.                     |
| [UpdateMetadata](../api/call-updatemetadata.md)                   | Aktualisieren der Metadaten für sich selbst in der Teilnehmerliste.          |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md) | Starten und Beenden der Bildschirmübertragung in dem Anruf.   |

Verwenden Sie für die Interaktion mit anderen Teilnehmern an dem Anruf das participants-Objekt.

| Methode                                                            | Beschreibung                                  |
|:------------------------------------------------------------------|:---------------------------------------------|
| [Teilnehmer auflisten](../api/call-list-participants.md)             | Abrufen einer Sammlung von Teilnehmerobjekten.         |
| [Teilnehmer einladen](../api/participant-invite.md)               | Einladen von Teilnehmern zum aktiven Anruf.      |
| [Alle Teilnehmer stummschalten](../api/participant-muteall.md)            | Stummschalten aller Teilnehmer in dem Anruf.           |

## <a name="media"></a>Medien

Die Verarbeitung von Medien wird über die Microsoft Real-Time Media-Plattform verwaltet. Über die Real-Time Media-Plattform können Bots in Microsoft Teams an Audio-/Videoanrufen und Besprechungen teilnehmen. Dadurch können Echtzeitbots an Peer-to-Peer-Anrufen und an Anrufen mit mehreren Teilnehmern teilnehmen.

Wenn der Bot auf einen eingehenden Anruf antwortet oder einem neuen oder bestehenden Anruf beitritt, muss er der Real-Time Media-Plattform mitteilen, wie Medien behandelt werden. Wenn Sie ein IVR-System (Interactive Voice Response) erstellen, können Sie die kostspielige Audioverarbeitung auf von Microsoft gehostete Mediakomponenten verlagern. Für den Fall, dass Ihr Bot direkten Zugriff auf Mediendatenströme benötigt, bieten wir eine von der Anwendung gehostete Medienoption über das Real-Time Media-SDK an.

### <a name="service-hosted-media"></a>Vom Dienst gehostete Medien

Bots können den Workflow verwalten und die Audioverarbeitung auf die Microsoft Real-Time Media-Plattform verlagern. Mit vom Dienst gehosteten Medien haben Sie mehrere Optionen zum Implementieren und Hosten Ihres Bots. Erwägen Sie die Verwendung des verfügbaren [SDKs](https://developer.microsoft.com/graph/code-samples-and-sdks). Ein vom Dienst gehosteter Medienbot kann als statusfreier Dienst implementiert werden, da er keine Medien lokal verarbeitet.

| Methode                                                        | Beschreibung                                             |
|:--------------------------------------------------------------|:--------------------------------------------------------|
| [PlayPrompt](../api/call-playprompt.md)                       | Wiedergegeben eines Audioclips für den Benutzer.                         |
| [Record](../api/call-record.md)                               | Optionales Wiedergeben einer Eingabeaufforderung und Aufzeichnen eines Audioclips.      |
| [SubscribeToTone](../api/call-subscribetotone.md)             | Abonnieren von MFV-Tönen vom Benutzer.                  |
| [CancelMediaProcessing](../api/call-cancelmediaprocessing.md) | Abbrechen jeglicher Medienverarbeitung, die sich bereits in der Warteschlange befindet.             |

### <a name="application-hosted-media"></a>Von der Anwendung gehostete Medien

Für den direkten Zugriff auf die Medien benötigt der Bot die „Access-Media“-Berechtigung. Mit der Real-Time Media-Bibliothek und dem zustandsbehafteten SDK können Sie funktionsreiche Bots für Medienanrufe in Echtzeit erstellen. Ein in der Anwendung gehosteter Bot muss in einer Windows-Umgebung gehostet werden. Die [Beispiele für in der Anwendung gehostete Medien](https://github.com/microsoftgraph/microsoft-graph-comms-samples) veranschaulichen, wie Sie den Bot auf verschiedenen Azure-Plattformen (einschließlich Cloud Services und Service Fabric) erstellen.

Sie können das [SDK für Microsoft Graph-Anrufe](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html) verwenden, um die Erstellung von Bots zu vereinfachen. Das SDK bietet Funktionen zum Verwalten der Zustände der Ressourcen im Arbeitsspeicher und zum Abrufen des Medienstapels der Bot-Entwickler.

Das Medien-SDK ermöglicht dem Bot das Senden und Empfangen von Audio, Video und Inhalten videobasierter Bildschirmübertragung. Die videobasierte Bildschirmübertragung wird als Videokanal modelliert. Der Bot kann den gemischten Audiokanal und mehrere Videokanäle abonnieren. Der Bot kann Video für den Videokanal entweder als codierten H.264-Stream oder als decodierte Raw-Frames senden und empfangen.

> **Hinweis:** Sie dürfen die Microsoft.Graph.Calls.Media-API nicht verwenden, um Medieninhalte aus Anrufen oder Besprechungen, auf die der Bot zugreift, aufzuzeichnen oder auf andere Weise zu speichern.

## <a name="see-also"></a>Siehe auch

[Beispiele für die API für Anrufe und Onlinebesprechungen](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)

[Bekannte Probleme](/graph/known-issues#calls-and-online-meetings)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/calls-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
