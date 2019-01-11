---
title: Referenz zu Microsoft Graph-REST-API, Version 1.0
description: Willkommen bei der Referenz zu Microsoft Graph-REST-API für den v1.0-Endpunkt.
localization_priority: Priority
ms.openlocfilehash: 6e0dde56aae7857e9ae042f89ba5eb6b01737efa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829074"
---
# <a name="microsoft-graph-rest-api-v10-reference"></a>Referenz zu Microsoft Graph-REST-API, Version 1.0

Willkommen bei der Referenz zu Microsoft Graph-REST-API für den v1.0-Endpunkt.

API-Sätze auf dem v1.0-Endpunkt (`https://graph.microsoft.com/v1.0`) sind allgemein verfügbar und haben einen strengen Überprüfungs- und Feedbackprozess mit Kunden durchlaufen, um praktischen Produktionsanforderungen zu entsprechen. Die Updates für APIs an diesem Endpunkt sind additiven Charakters und verursachen keine Probleme in vorhandenen App-Szenarien.

## <a name="common-use-cases"></a>Allgemeine Anwendungsfälle

Die Leistungsfähigkeit von Microsoft Graph liegt in der einfachen Navigation durch Entitäten und Beziehungen über verschiedene Dienste hinweg, die auf einem einzigen Microsoft Graph-REST-Endpunkt verfügbar gemacht werden.

Eine Anzahl von diesen Diensten dienen dazu, umfangreiche Szenarien zu einem [Benutzer](./resources/user.md) und zu einer [Gruppe](./resources/group.md) zu ermöglichen.

### <a name="user-centric-use-cases-in-v10"></a>Benutzerorientierte Anwendungsfälle in Version 1.0

1. [Abrufen von Profil](./api/user-get.md) und [Foto](./resources/profilephoto.md) einer Benutzerin, Lisa.
2. [Abrufen von Profilinformationen über Lisas Manager](./api/user-list-manager.md) und [die IDs ihrer direkten Mitarbeiter](./api/user-list-directreports.md), die alle in Azure AD gespeichert sind.
3. [Zugreifen auf Lisas Dateien auf OneDrive for Business](./api/driveitem-list-children.md), auf die [Identität](./resources/identityset.md) der letzten Person, die dort eine [Datei](./resources/driveitem.md) geändert hat, und Navigieren zum Profil dieser Person.
4. [Zugreifen auf Lisas Kalender ](./api/calendar-get.md) in Exchange Online und [Bestimmen der besten Zeit für Lisa, um sich in den nächsten zwei Wochen mit ihrem Team zu treffen](./api/user-findmeetingtimes.md).
5. [Abonnieren](./api/subscription-post-subscriptions.md) und [Nachverfolgen von Änderungen](./api/event-delta.md) in Lisas Kalender und Mitteilen, wenn Lisa mehr als 80 % ihrer Zeit in Besprechungen verbringt.
6. [Festlegen automatischer Antworten](./api/user-update-mailboxsettings.md#example), wenn Lisa nicht im Büro ist.
7. [Abrufen der Personen, die für Lisa am relevantesten sind](./api/user-list-people.md), basierend auf Kommunikation, Zusammenarbeit und Geschäftsbeziehungen.
8. Abrufen der neuesten Umsatzprognose aus einem [Diagramm](./resources/chart.md) in einer Excel-Datei in Lisas OneDrive for Business.
9. [Finden der Aufgaben, die Lisa in Planner zugewiesen sind](./api/planneruser-list-tasks.md).

### <a name="office-365-group-use-cases-in-v10"></a>Office 365-Gruppe Anwendungsfälle in Version 1.0

1. Ausführen eines Berichts auf Office 365-Gruppen in einer Organisation und Identifizieren der Gruppe mit der meisten [Kommunikation zwischen Gruppenmitgliedern](./api/reportroot-getoffice365groupsactivitycounts.md).
2. [Suchen der Pläne dieser Office 365-Gruppe](./api/plannergroup-list-plans.md) und [Zuweisen von Aufgaben](./resources/plannerassignments.md) in diesem Plan.
3. [Beginnen einer neuen Unterhaltung](./api/group-post-conversations.md) in der Office 365-Gruppe, um zu ermitteln, ob Mitglieder[eine weitere Gruppe erstellen möchten](./api/group-post-groups.md), um die Arbeitslast zu teilen.
4. [Abrufen des Standardnotizbuchs](./api/notebook-get.md) für die Gruppe und [Erstellen einer Seite](./api/section-post-pages.md), um die Ergebnisse der Untersuchung zu notieren.

## <a name="other-api-versions"></a>Andere API-Versionen

Es gibt zurzeit 2 Versionen von Microsoft Graph-REST-APIs – Version 1.0 und Beta.
Wenn Sie an neuen oder erweiterten APIs interessiert sind, die sich noch im Vorschaustatus befinden, gehen Sie auf [Referenz zu Microsoft Graph-Beta-Endpunkt](/graph/api/overview?toc=./ref/toc.json&view=graph-rest-beta). Beachten Sie, dass APIs im Vorschaustatus geändert werden können und ohne Ankündigung Probleme in vorhandenen Szenarien verursachen können. Verlassen Sie sich in der Produktion nicht auf APIs im Beta-Endpunkt.

Weitere Informationen finden Sie unter [Versionsverwaltung und Support](/graph/versioning-and-support).

## <a name="connect-with-us"></a>Setzen Sie sich mit uns in Verbindung.

Gibt es weitere APIs oder Features, die Sie in Microsoft Graph sehen möchten? Posten Sie neue Feature-Anforderungen auf [UserVoice](https://officespdev.uservoice.com/forums/224641-general/filters/new?category_id=101632).

Haben Sie Feedback für vorhandene Microsoft Graph APIs? Setzen Sie sich mit uns auf [Github](https://github.com/microsoftgraph/microsoft-graph-docs/issues) in Verbindung.

Bei Fragen oder mit Ihr Code mithilfe von Microsoft-Hilfe
