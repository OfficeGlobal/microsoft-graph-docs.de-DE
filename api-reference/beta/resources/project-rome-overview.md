---
title: 'Verwenden Sie die Microsoft Graph-API Project ROM entwickelt '
description: 'Project-ROM ist eine Microsoft-Initiative eine Plattform zu erstellen, mit die app-Entwickler umfangreiche Cross-Gerät Erfahrungen erstellen können. Project-ROM kann verschiedene Funktionen, die verschiedene Dienste und Clientendpunkte verbinden, wenn der Benutzer bei sich mit den gleichen Microsoft-Konto oder arbeiten oder Schule Konto. Dadurch können Sie Cross-Gerät und plattformübergreifende Erfahrungen implementieren, die um Benutzeraufgaben statt Geräte zentriert wird. '
ms.openlocfilehash: f779c04a76331d27fdcae6436e758bacfc052f8e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060446"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>Verwenden Sie die Microsoft Graph-API Project ROM entwickelt 

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

[Project-ROM](https://developer.microsoft.com/en-us/windows/project-rome) ist eine Microsoft-Initiative eine Plattform zu erstellen, mit die app-Entwickler umfangreiche Cross-Gerät Erfahrungen erstellen können. Project-ROM kann verschiedene Funktionen, die verschiedene Dienste und Clientendpunkte verbinden, wenn der Benutzer bei sich mit den gleichen Microsoft-Konto oder arbeiten oder Schule Konto. Dadurch können Sie Cross-Gerät und plattformübergreifende Erfahrungen implementieren, die um Benutzeraufgaben statt Geräte zentriert wird. 

Drei Schlüsselfunktionen Project ROM über Microsoft Graph zur einfacheren hervorragende Cross-Gerät Erfahrungen aktivieren verfügbar gemacht werden: Aktivitäten, Geräte und Benachrichtigungen. 

## <a name="activities"></a>Aktivitäten

Aktivitäten in Microsoft Graph können Sie zu Laufwerk Benutzer mit Ihren apps für Geräte und Plattformen. Eine Aktivität ist die Einheit eines Auftrags für Benutzer und besteht aus drei Komponenten:

- Deep-link
- Eine visuelle Darstellung
- Metadaten, die die Aktivität beschreibt mithilfe der [https://schema.org/](https://schema.org/) shared Vokabular

Wenn eine Sitzung von einer Anwendung erstellt wird, wird die Aktivität des Berichtszeitraums Benutzer Engagements entsprechend ein Historienelement hinzugefügt. Jedes Mal wird ein Benutzer mit einer Aktivität reengages, ein neues Historienelement die Aktivität fällig Engagements Benutzer hinzugefügt.

Wenn eine Anwendung Aktivität Benutzerobjekte veröffentlicht, wird das Objekt in einigen der neuen Benutzeroberfläche Flächen in Windows angezeigt; Cortana Benachrichtigungen und Zeitachsen. Sie können in Ihrer Aktivität-Objekten rich-Metadaten (zum Aktivitäten im richtigen Kontext dargestellt werden können) und rich visuelle Objekte (mit [Adaptive Karte](https://adaptivecards.io/) Markup) angeben.

Die folgenden Microsoft Graph-APIs können zum Erstellen und die Benutzeraktivitäten abrufen:

- [Erstellen oder Ersetzen Sie die Aktivität](../api/projectrome-put-activity.md)
- [Abrufen von Aktivitäten](../api/projectrome-get-activities.md)
- [Aktuelle Aktivitäten abrufen](../api/projectrome-get-recent-activities.md)
- [Aktivität löschen](../api/projectrome-delete-activity.md)
- [Verlaufselement erstellen oder ersetzen](../api/projectrome-put-historyitem.md)
- [Verlaufselement](../api/projectrome-delete-historyitem.md) löschen

## <a name="devices"></a>Geräte

Sie können Project-ROM-APIs in Microsoft Graph verwenden:

- Entdecken Sie und Herstellen einer Verbindung des Benutzers Geräte mit
- Starten Sie Remote apps auf diesen Geräten
- Senden von Nachrichten an Ihre apps auf diesen Geräten

Mit diesen APIs können Sie apps erstellen, die umfangreiche Erfahrungen erstellen, die ein einzelnes Gerät transcend. Beispielsweise können Sie Ihre app So starten Sie auf einem größeren Bildschirm erweitern. Oder Sie können eine Mobile Begleit-Erfahrung für eine app auf einem anderen Geräte des Benutzers erstellen.

Die folgenden Microsoft Graph-APIs können Sie die Kommunikation mit anderen Windows-Geräten:

- [Auflisten des Benutzers Geräte](../api/user-list-devices.md)
- [Senden Sie einen Befehl zu einem Gerät](../api/send-device-command.md)
- [Abrufen des Befehlsstatus](../api/get-device-command-status.md)

## <a name="notifications"></a>Benachrichtigungen

Sie können die Benachrichtigungen APIs in Microsoft Graph Benachrichtigungen über mehrere Endpunkte übermittelt werden, die denselben Benutzer, in angemeldet ist verwenden. Sie können einen Benutzer direkt abzielen, beim Bereitstellen von Benachrichtigungen anstelle von Adressen/Gerätekanäle kümmern. Auf diese Weise können Sie auf die rechten Benachrichtigungsszenarien in einer Human-centric, statt eine Gerät-centric Möglichkeit entwerfen konzentrieren. 

Sie können eine Benachrichtigung Rohdaten oder eine direkte visuelle Benachrichtigung veröffentlichen. Wenn eine Benachrichtigung über eine unformatierte Daten an einen Endpunkt Gerät übermittelt werden, können Sie die [Client-SDK](https://github.com/Microsoft/project-rome) (Microsoft Graph-Benachrichtigungen SDK für Windows Project ROM SDK für iOS und Android) klicken Sie dann verwenden, empfangen und Benachrichtigungen verwalten. Wenn eine direkte visuelle Benachrichtigung an einen Endpunkt Gerät gesendet wird, wird die systemeigene plattformspezifische-Benachrichtigung an dem Benutzer angezeigt. 

Weitere Informationen hierzu finden Sie unter [Erstellen und senden Sie eine Benachrichtigung](../api/projectrome-notification-post.md).

