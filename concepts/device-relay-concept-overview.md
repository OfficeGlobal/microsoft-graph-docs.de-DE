---
title: Geräterelay-API in Microsoft Graph (Vorschau)
description: 'Menschen interagieren heute täglich mit mehreren Geräten. Benutzer beginnen Produktivitätsaufgaben und Unterhaltungsaktivitäten häufig auf einem Gerät und setzen diese dann auf einem anderen Gerät fort. Um die Anforderungen Ihrer Kunden zu erfüllen, muss Ihre App nahtlos auf mehreren Geräten und Plattformen einsetzbar sein. '
ms.openlocfilehash: aa3bdd3401be9d26f55d5b3dcc792ed81e7dae87
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092241"
---
# <a name="device-relay-api-in-microsoft-graph-preview"></a>Geräterelay-API in Microsoft Graph (Vorschau)

Menschen interagieren heute täglich mit mehreren Geräten. Benutzer beginnen Produktivitätsaufgaben und Unterhaltungsaktivitäten häufig auf einem Gerät und setzen diese dann auf einem anderen Gerät fort. Um die Anforderungen Ihrer Kunden zu erfüllen, muss Ihre App nahtlos auf mehreren Geräten und Plattformen einsetzbar sein. 

Sie können die Geräterelay-APIs verwenden, um Benutzern eine reibungslose Erfahrung zu ermöglichen. Ermöglichen Sie, dass eine Oberfläche aktiv von einem Gerät auf ein anderes übertragen werden kann, oder verbessern Sie diese, indem Sie mehrere Geräte gleichzeitig verwenden. Dies geschieht über In-App-Aktionen (eine Schaltfläche oder eine Auswahl in Ihrer App), die die Geräterelay-API aufrufen, um die Geräte des Benutzers zu suchen und diesen zu ermöglichen, Ihre App auf diesen anderen Geräten zu starten.

## <a name="why-integrate-with-device-relay"></a>Gründe für die Integration in das Geräterelay

Die Geräterelay-API ermöglicht es Ihrer App, sich selbst zu registrieren und Ihre App auf den Geräten des Benutzers zu suchen sowie Befehle und Benachrichtigungen an diese zu senden. Auf diese Weise können Sie das Hauptaugenmerk auf die Aufgaben legen, an denen Ihre Kunden arbeiten. Sie können auf dem Gerät arbeiten, das für sie am praktischsten ist, indem Sie es suchen und dann Aufgaben dorthin übertragen werden. Es kann auch eine laufende Erfahrung mit Ihrer App verbessert werden, indem andere Geräte damit verwendet werden.

Sie können die Geräterelay-API für Szenarien mit Begleitgeräten oder Fernbedienungen verwenden. Verwenden Sie die Messaging-Funktionen, um einen App-Kanal zwischen zwei Geräten zu erstellen, um benutzerdefinierte Nachrichten zu senden und zu empfangen. Kunden können beispielsweise ihre Telefone zum Steuern der Wiedergabe auf einem Fernseher verwenden. Sie könnten auch eine Begleit-App in einem Produktivitätsszenario bereitstellen, indem kontextbasierte häufig verwendete Aktionen auf einem Telefon angezeigt werden, während Ihre Benutzer in der Hauptansicht Ihrer App auf dem Computer arbeiten.

Ihre Kunden können Oberflächen auch aktiv von einem Gerät zu einem anderen übertragen, indem sie eine Aktion in Ihrer App ausführen. Vielleicht schaut sich ein Benutzer eine Live-Übertragung auf dem Telefon an, während er im Bus sitzt, wenn er jedoch nach Hause kommt, soll die Wiedergabe auf den Computer im Wohnzimmer übertragen werden. Produktivitätsszenarien werden vom Geräterelay ebenfalls unterstützt. 

### <a name="extend-the-experience"></a>Erweitern der Oberfläche

Erweitern Sie Ihre App, indem Sie UX zum Suchen von Geräten und zum Starten der App auf diesen Geräten bereitstellen. Der Benutzer könnte beispielsweise auf seinem Telefon an einer Bestellung arbeiten, den Computer in seinem Büro suchen und die App dort starten, um die Eingabe der Bestellung abzuschließen.  

### <a name="augment-the-experience"></a>Verbessern der Oberfläche

Erstellen Sie eine Begleitoberfläche für Ihre App auf einem anderen Gerät des Benutzers. Die App könnte beispielsweise UX umfassen, um sich selbst auf anderen Geräten zu starten. In einem Spiel kann der Benutzer die App auf einem Gerät mit einem größeren Bildschirm starten (z. B. von einem PC zu einer Xbox). Auf der Xbox ist eine Vollansicht des Spiels (Ich-Perspektive) möglich, wohingegen auf dem Gerät mit einem kleineren Bildschirm eine andere Ansicht mit zusätzlichem Kontext vorhanden ist (eine allgemeine Ansicht des Spielelevels, in der die Position des Spiels und der Gegner angezeigt werden).  

### <a name="enrich-the-experience"></a>Optimieren der Oberfläche

Fügen Sie der App zusätzliche Steuerungsmöglichkeiten hinzu. Stellen Sie für die Haupt-App beispielsweise Fernbedienungsfunktionen von einem Begleitgerät bereit. Wenn der Benutzer eine App von einem Gerät auf einem anderen startet, könnte auf dem Zielgerät die vollständige Oberfläche (z. B. ein 3D-Modell in einer Design-App) angezeigt werden, wohingegen auf dem Quellgerät eine Liste der häufigsten Aktionen anhand des Status der App auf dem Zielgerät angezeigt wird (z. B. drehen, Größe ändern, Farbpalette).

## <a name="see-also"></a>Siehe auch

- [Geräteübergreifende Oberflächen in Microsoft Graph](cross-device-concept-overview.md)
- [Informationen zur Geräterelay-API](/graph/api/resources/project-rome-overview?view=graph-rest-beta)
- [Informationen zu Project Rome](https://aka.ms/projectrome)
