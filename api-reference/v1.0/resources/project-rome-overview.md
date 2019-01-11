---
title: Verwenden Sie die Microsoft Graph-API Project ROM entwickelt
description: Project-ROM handelt es sich um eine Microsoft-Initiative zum Erstellen eines Cross-Geräts Plattform auftritt. Project-ROM ermöglicht einer app auf einem lokalen Client oder Dienst zur Interaktion mit apps und Dienste auf einem remote-Host, wenn der Benutzer mit der gleichen Microsoft-Konto signiert, mit denen sie auf dem Clientgerät anmelden. Dies ermöglicht es Ihnen zu Programm Cross-Gerät und plattformübergreifende Erfahrungen, die um Benutzeraufgaben statt Geräte zentriert werden.
localization_priority: Normal
ms.openlocfilehash: d103bb68560a39cc4491460969a36bb81bb6da44
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840964"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>Verwenden Sie die Microsoft Graph-API Project ROM entwickelt

[Project-ROM](https://developer.microsoft.com/en-us/windows/project-rome) handelt es sich um eine Microsoft-Initiative zum Erstellen eines Cross-Geräts Plattform auftritt. Project-ROM ermöglicht einer app auf einem lokalen Client oder Dienst zur Interaktion mit apps und Dienste auf einem remote-Host, wenn der Benutzer mit der gleichen Microsoft-Konto signiert, mit denen sie auf dem Clientgerät anmelden. Dies ermöglicht es Ihnen zu Programm Cross-Gerät und plattformübergreifende Erfahrungen, die um Benutzeraufgaben statt Geräte zentriert werden.

Eine wichtige Komponente wird über Microsoft Graph so ermöglicht es den verfügbar gemacht: Aktivitäten.

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

