---
title: Arbeiten mit den Anrufe und dazu dient, onlinebesprechungen-API in Microsoft Graph
description: Ruft das Microsoft Graph und dazu dient, onlinebesprechungen API Fügt eine neue Dimension, wie Ihre apps und Diensten mit Benutzern interagieren können von Sprach- und Videofunktionen aktivieren. Die API ermöglicht Ihnen das Erstellen von Anrufen und Entgegennehmen von Anrufen von Benutzern und Anwendungen in Microsoft-Teams. Diese APIs können Sie eine dienstanwendung (Robot) erstellen, die als Teilnehmer in einem Anruf oder Besprechung fungieren kann.
author: VinodRavichandran
ms.openlocfilehash: 1b7efc774dfee0e0617d5c4f99ba08351c9f2a1f
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380562"
---
# <a name="working-with-the-calls-and-online-meetings-api-in-microsoft-graph"></a>Arbeiten mit den Anrufe und dazu dient, onlinebesprechungen-API in Microsoft Graph

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Ruft das Microsoft Graph und dazu dient, onlinebesprechungen API Fügt eine neue Dimension, wie Ihre apps und Diensten mit Benutzern interagieren können von Sprach- und Videofunktionen aktivieren. Die API ermöglicht Ihnen das Erstellen von Anrufen und Entgegennehmen von Anrufen von Benutzern und Anwendungen in Microsoft-Teams. Diese APIs können Sie eine dienstanwendung (Robot) erstellen, die als Teilnehmer in einem Anruf oder Besprechung fungieren kann.

## <a name="call-types"></a>Anruftypen

Anrufe werden als Peer-zu-Peer- oder mehr Teilnehmern Anrufe kategorisiert. Ein Benutzer kann mit Ihrem Bot Peer-zu-Peer-Anruf initiieren oder Ihre Bot in einer laufenden Konferenz mit mehreren Teilnehmern einladen. Wenn der Benutzer den Robot zu einem Peer-zu-Peer-Anruf einladen ist, sind keine Berechtigungen erforderlich. Für Ihre Bot auf im Gespräch mit mehreren Teilnehmern teilnehmen muss der Bot Berechtigung aus der mandantenadministrator an einem gruppenanruf teilnehmen.

![Ein Bild mit Peer-zu-Peer und mit mehreren Teilnehmern Anrufe](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/call-types.png)

Wenn Ihre Bot den Anruf erstellt, soll initiieren oder die initiieren reaktionsgruppenanruf Berechtigung verfügen. Ihre Bot hat die Möglichkeit, einen Peer-zu-Peer-Anruf oder eines Anrufs mit mehreren Teilnehmern zu erstellen.

- Für einen Peer-zu-Peer-Anruf muss den Robot nur von einem Ziel und keine Besprechung Koordinaten angeben. 
- Ihre Bot ein Anrufs mit mehreren Teilnehmern initiiert, eine ad-hoc-Besprechung im Hintergrund eingerichtet ist, und jeder der Konferenz teilnimmt. Besprechung Koordinaten angegeben, ist ein Anruf mit mehreren Teilnehmern eingerichtet, auch wenn nur ein Ziel vorhanden ist.

Gespräch möglicherweise als Peer-zu-Peer-starten und an Konferenzen mit mehreren Teilnehmern ausweiten. Eine Konferenz wird automatisch bereitgestellt und die Medien an der Konferenz umgeleitet werden. Ihre Bot können Ausweitung initiieren durch einladen weiterer Personen, sofern Ihr Bot die initiieren reaktionsgruppenanruf-Berechtigung verfügt. Die Ausweitung von einem anderen Teilnehmer initiiert, und den Robot verfügt nicht über Join-Gruppe-Call-Berechtigung, wird Ihre Bot aus dem Aufruf gelöscht.

> **Wichtig:** Wenn ein Anruf an mit mehreren Teilnehmern über Peer-zu-Peer-eskaliert wird, sind nicht alle mit mehreren Teilnehmern Features verfügbar. Insbesondere erhalten den Robot nicht Teilnehmerliste Updates.

## <a name="signaling"></a>Signale

### <a name="incoming-call"></a>Eingehender Anruf

Wenn Sie einen eingehenden Anruf erhalten, müssen Sie den aufrufenden Robot registrieren. Wenn der Bot der Benachrichtigung über eingehende empfängt, hat sie die folgenden Optionen.

| Methode                              | Beschreibung                                  |
|:------------------------------------|:---------------------------------------------|
| [Antwort](../api/call-answer.md)     | Nehmen Sie den eingehenden Anruf.                    |
| [Ablehnen](../api/call-reject.md)     | Ablehnen und Auflegen des Anrufs.                  |
| [Redirect](../api/call-redirect.md) | Umleiten des Anrufs.                           |

Der Bot können den Anruf an einen anderen Benutzer oder eine Bot umleiten. Der Bot können auch es an die Voicemail des Benutzers umleiten.

![Bild mit einer Bot Umleiten eines Anrufs an Voicemail](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/call-handling.png)

> **Wichtig:** Umleiten von oder ausgehende Anrufe an PSTN wird derzeit nicht unterstützt.

### <a name="in-call"></a>Während des Anrufs

Vorgänge für den Robot stehen für die Anruf-Objekt. Diese wirken sich auf den Robot als den Teilnehmer in den Anruf.

| Methode                                                            | Beschreibung                                  |
|:------------------------------------------------------------------|:---------------------------------------------|
| [Stummschalten](../api/call-mute.md)                                       | Stumm Zuschalten in den Anruf.                       |
| [Stummschaltung aufheben](../api/call-unmute.md)                                   | Aktiviert self in den Anruf.                     |
| [UpdateMetadata](../api/call-updatemetadata.md)                   | Aktualisieren Sie in der Teilnehmerliste einer Metadaten für sich selbst.          |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md) | Starten Sie und beenden Sie die Freigabe Bildschirm in den Anruf.   |

Verwenden Sie zur Interaktion mit anderen Teilnehmern auf den Anruf, das Teilnehmer-Objekt.

| Methode                                                            | Beschreibung                                  |
|:------------------------------------------------------------------|:---------------------------------------------|
| [Liste Teilnehmer](../api/call-list-participants.md)             | Rufen Sie eine objektauflistung von Teilnehmer.         |
| [Einladen von Teilnehmern](../api/participant-invite.md)               | Einladen von Teilnehmern zum aktiven Anruf.      |
| [Stummschalten Sie aller Teilnehmer](../api/participant-muteall.md)            | Stummschalten Sie aller Teilnehmer in den Anruf.           |

## <a name="media"></a>Medien

Medienverarbeitung durch Microsoft Real-Time Media-Plattform verwaltet. Der Real-Time Media-Plattform unterstützt Bots in Microsoft-Teams, Audio-/Videoanrufen und Besprechungen zu beteiligen. Sie können in Echtzeit Bots an Anrufe Peer-zu-Peer und mit mehreren Teilnehmern teilnehmen.

Wenn der Bot einen eingehenden Anruf beantwortet oder einen neuen oder vorhandenen Anruf verknüpft, muss der Real-Time Media-Plattform zu informieren, wie Medien behandelt werden sollen. Wenn Sie ein System interaktive Sprachantwort (IVR) erstellen, können Sie auf Microsoft Dienst gehostet Medien Verarbeitungskomponenten teurer Audiosignale abnimmt. Wenn Ihre Bot direkten Zugriff auf Mediendaten erforderlich sind, bieten wir eine Medienoption Anwendung gehostet mit dem Real-Time Media SDK.

### <a name="service-hosted-media"></a>Media-Dienst gehostet

Bots können den Workflow verwalten und Verschiebung Verarbeitung von Audiosignalen zur Microsoft Real-Time Media-Plattform. Mit Medien-Dienst gehostet haben Sie mehrere Optionen zu implementieren und Hosten Ihrer Bot. Erwägen Sie eine der verfügbaren [SDKs](https://developer.microsoft.com/graph/code-samples-and-sdks). Ein Dienst gehostet Media Bot kann als statusfreie Dienst implementiert werden, wie Medien lokal nicht verarbeitet.

| Methode                                                        | Beschreibung                                             |
|:--------------------------------------------------------------|:--------------------------------------------------------|
| [PlayPrompt](../api/call-playprompt.md)                       | Wiedergabe eines Audioclips für dem Benutzer.                         |
| [Record](../api/call-record.md)                               | Optional wiedergeben Sie eine Aufforderung, und zeichnen Sie Audioclips.      |
| [SubscribeToTone](../api/call-subscribetotone.md)             | DTMF-Töne vom Benutzer abonnieren.                  |
| [CancelMediaProcessing](../api/call-cancelmediaprocessing.md) | Brechen Sie alle Medien Verarbeitung bereits in der Warteschlange ab.             |

### <a name="application-hosted-media"></a>Media Anwendung gehostet

Für den Robot zum direkten Zugriff auf die Medien zu erhalten benötigt der Bot eine Berechtigung für die Medien zugreifen. Der Real-Time Media-Bibliothek und dynamische SDK können beim Erstellen von rich-Real-Time Media Bots aufrufen. Eine Anwendung gehostet Bot muss in einer Windows-Umgebung gehostet werden. [Anwendung gehostet Media Beispiele](https://github.com/microsoftgraph/microsoft-graph-comms-samples) zeigen, wie den Robot in verschiedenen Azure-Plattformen (einschließlich Clouddiensten und Fabric Service) zu erstellen.

Das [Microsoft Graph Anrufe SDK](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html) können Sie um die Erstellung von Programmen zu vereinfachen. Das SDK bietet Funktionen zum Verwalten der Status der Ressourcen im Arbeitsspeicher und in Bot-Entwickler medienstapel abrufen.

Media-SDK ermöglicht den Robot senden und Empfangen von Audio-, Video- und videobasierte Bildschirmfreigabe Content. Video-basierte Bildschirmfreigabe wird als eine Videokanal modelliert. Der Bot können die gemischte Audiokanal und mehrere video-Kanäle abonnieren. Für die Videokanal hat den Robot Möglichkeit zum Senden und Empfangen von Video als codierten Stream h. 264 oder als decodierten unformatierte Frames.

> **Hinweis:** Sie können die Microsoft.Graph.Calls.Media-API nicht zum Aufzeichnen oder anderweitig beibehalten Media-Inhalten von Anrufen oder Besprechungen, die Ihre Bot greift auf.

## <a name="see-also"></a>Weitere Artikel

[Anrufe und onlinebesprechung API-Beispiele](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)

[Bekannte Probleme](/graph/known-issues#calls-and-online-meetings)