---
title: Verwenden der Aktivitätsfeed-API in Microsoft Graph zur Erstellung geräteübergreifender Oberflächen
description: Wenn Sie Aktivitäten verwenden, können diese Microsoft-Oberflächen zu einer größeren Akzeptanz Ihrer App führen. Die Anzeige von Aktivitäten in Apps kann Benutzern außerdem helfen, genau dort weiterzumachen, wo sie zuvor aufgehört haben – auf jedem Gerät und auf jeder Plattform, inklusive Windows, Android und iOS.
ms.openlocfilehash: 768326a5a18962f28aebe2e66b7dbd2a95b1a7bb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092153"
---
# <a name="using-the-activity-feed-api-in-microsoft-graph-to-enable-cross-device-experiences"></a>Verwenden der Aktivitätsfeed-API in Microsoft Graph zur Erstellung geräteübergreifender Oberflächen

Aktivitäten ermöglichen es Benutzern, wichtige Aufgaben in einer App schnell auf einem anderen Gerät fortzusetzen, und machen sie so produktiver. Mit Oberflächen wie der Windows Timeline, Windows Sets, Cortana „Pick up where I left off“ und Microsoft Launcher fördert Microsoft die Benutzerproduktivität in Ihren Apps. Dabei basieren alle diese Features auf dem Aktivitätsfeed.Wenn Sie Aktivitäten verwenden, können diese Microsoft-Oberflächen zu einer größeren Akzeptanz Ihrer App führen. Die Anzeige von Aktivitäten in Apps kann Benutzern außerdem helfen, genau dort weiterzumachen, wo sie zuvor aufgehört haben – auf jedem Gerät und auf jeder Plattform, inklusive Windows, Android und iOS.

## <a name="why-integrate-with-activities"></a>Gründe für die Integration von Aktivitäten
### <a name="enable-experiences-that-flow-seamlessly-between-windows-android-linux-and-ios-devices"></a>Oberflächen mit nahtlosem Wechsel zwischen Windows-, Android-, Linux- und iOS-Geräten 
Was zeichnet eine tolle Anwendung aus? Sie hilft Benutzern, Großartiges zu leisten, und unterstützt eine breite Palette an Kreativitäts-, Produktivitäts- und Entertainment-Szenarien. Eine einmal begonnene Aufgabe fortzuführen, kann jedoch schwierig sein, insbesondere dann, wenn der Benutzer sie auf einem anderen Gerät oder einer anderen Plattform fortsetzen möchte. Durch das Einbinden von Aktivitäten in Anwendungen ermöglichen Sie es Ihren Benutzern, im Handumdrehen zu ihren letzten Aufgaben zurückzukehren, und zwar auf jedem beliebigen Bildschirm. Sie können mühelos zwischen Internet, Mobilgerät und Desktop wechseln. Anhand von Verlaufselementen sehen sie ihre zuletzt durchgeführten Aktivitäten, inklusive Angaben zu ihrem genauen Zeitpunkt und ihrer genauen Dauer.   

Jede Benutzeraktivität stellt ein separates Ziel in der App dar: eine Produktseite, eine TV-Serie, ein Dokument oder eine aktive Kampagne in einem Spiel. Zum Fortsetzten der Aktivität in der App braucht es lediglich einen Deep-Link. Mit der Methode zum [Abrufen der letzten Aktivitäten](/graph/api/projectrome-get-recent-activities?view=graph-rest-1.0) können Sie beispielsweise eine Liste der zuletzt angesehenen Produkte für eine Shopping-App oder eine aktuelle Leseliste mit Büchern und Zeitungsartikeln erstellen. 

### <a name="create-richer-activities-for-any-experience-with-adaptive-cards"></a>Funktionsreichere Aktivitäten für jede Oberfläche dank adaptiver Karten
Gerenderte Aktivitäten in Microsoft-Oberflächen wie Windows Timeline werden mithilfe des [Adaptive Card](https://adaptivecards.io/)-Frameworks dargestellt. Dieses Framework ermöglicht die Erstellung attraktiver, funktionsreicher Karten zur Darstellung von App-Aktivitäten. Mithilfe des Adaptive Card-SDK können Sie auch in Ihren eigenen Apps funktionsreiche Karten rendern. Wenn Sie nicht für jede Aktivität eine eigene adaptive Karte bereitstellen, erstellt Microsoft automatisch eine einfache Aktivitätskarte mit dem Anwendungsnamen und dem Anwendungssymbol, dem Pflichtfeld „Titel“ und einem optionalen Feld „Beschreibung“. 

### <a name="let-microsoft-help-drive-app-usage-with-features-that-reach-hundreds-of-millions-of-customers"></a>Fördern der App-Akzeptanz mit Microsoft und Features mit einer Zielgruppe von Hunderten Millionen Kunden
Eine Integration von Benutzeraktivitäten ermöglicht es Benutzern nicht nur, Aktivitäten in Ihrer App nahtlos fortzusetzen, sondern macht auch den Zugriff auf einen wachsenden Satz an Microsoft-Oberflächen für Windows, iOS und Android möglich: Oberflächen, die speziell dafür optimiert sind, die Benutzerproduktivität zu steigern und den Benutzern die Verwendung Ihrer App auf sämtlichen Geräten zu erlauben. Mit Microsoft Graph genügt eine einmalige Integration von Benutzeraktivitäten und Sie erreichen Hunderte Millionen Heimanwender sowie Firmenkunden im zweistelligen Millionenbereich, die Windows sowie Microsoft-Produkte für iOS- und Android-Geräte verwenden.

![Screenshot von Windows Timeline](https://winblogs.azureedge.net/win/2017/05/22-591a3ec9833f4.jpg)

## <a name="see-also"></a>Weitere Artikel

- [Geräteübergreifende Oberflächen in Microsoft Graph](cross-device-concept-overview.md)
- [Verwenden der Aktivitätsfeed-API zur geräteübergreifenden Fortsetzung von Benutzeraktivitäten](/graph/api/resources/activity-feed-api-overview?view=graph-rest-1.0)
- [Veröffentlichen von Aktivitäten und Verlaufselementen in einer einzigen Anforderung per „deep insert“](/graph/api/projectrome-put-activity?view=graph-rest-1.0#example-2---deep-insert)
- [Informationen zu Project Rome](https://aka.ms/projectrome)
