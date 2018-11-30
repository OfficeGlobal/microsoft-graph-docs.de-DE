---
title: Verwenden Sie die Microsoft Graph-Sicherheit API
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: 556725597b7b020bc7ef5b55857ae59dfb127e80
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063557"
---
# <a name="use-the-microsoft-graph-security-api"></a>Verwenden Sie die Microsoft Graph-Sicherheit API

 > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die Microsoft Graph-Security-API bietet eine einheitliche Schnittstelle und Schema für die Integration der Sicherheitsfunktionen von Microsoft und Ökosystems Partnern. Dies ermöglicht Kunden Sicherheit Geschäftsabläufe zu optimieren und besser Schutz gegen Bedrohungen im Internet zu erhöhen. Sicherheit-API von Microsoft Graph kann zum Senden von Abfragen an alle Onboarded Sicherheitsanbieter abzurufenden aggregierte Antworten als ein Verbundbenutzer Aggregation Sicherheitsdienst verwendet werden. Verwenden von Microsoft Graph Sicherheit API Anwendungen erstellen, die:

- Konsolidieren Sie und korrelieren Sie Sicherheitshinweise aus mehreren Quellen
- Entsperren von Kontextdaten um Untersuchungen zu informieren.
- Automatisieren von Sicherheitsoperationen für größere Effizienz
- Transparenz für Sicherheitsdaten zur Ermöglichung von proaktiven Risikomanagement

Die Microsoft Graph-Security-API enthält die folgenden wichtigen Elemente.

## <a name="alerts"></a>Warnungen

Bei Benachrichtigungen handelt es sich um potenzielle Sicherheitsrisiken innerhalb eines Kunden Mandanten, die von Microsoft oder Partner sicherheitslösungen haben erkannt und für eine Aktion oder Benachrichtigung gekennzeichnet sind. Mit dieser Entität Microsoft Graph Security [Benachrichtigungen](alert.md) können Sie vereinheitlichen und Optimieren von Sicherheitsprobleme in alle integrierten Lösungen. Auf diese Weise können auch Applikationen zum Korrelieren von Warnungen und Kontext zum Schutz und die Antwortzeit zu verbessern. Diese entsperren Betriebseffizienz Sicherheit durch die Reduzierung von Untersuchung Zeit und Auflösung für Vorfälle. Mit der Funktion warnmeldungsaktualisierungs können Sie den Status von bestimmten Warnungen synchronisieren, über verschiedene Security-Produkte und Dienste, die mit der Microsoft Graph Security-API integriert sind, durch Aktualisieren der Entität [Benachrichtigungen](alert.md) .

Microsoft Graph Sicherheit Language-integrated Lösungen werden von die folgenden Sicherheitsanbieter Benachrichtigungen erhalten:

- Azure-Sicherheitscenter
- Azure Active Directory-Schutz
- Azure Information Protection
- Microsoft-Cloud-Anwendungssicherheit
- Windows-Defender erweiterte Schutz
- Microsoft Intune (private Preview)
- Office 365 (bald verfügbar)
- Azure erweiterte Threat Protection (bald verfügbar)
- Partnerlösungen wie Palo auch Netzwerke App-Framework

> **Hinweis:** Neue Anbieter sind kontinuierlich Onboarding auf das Microsoft Graph Security-Ökosystem.

## <a name="secure-score-preview"></a>Secure Score (Preview)

[Microsoft Secure Score](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Office-365-Secure-Score-is-now-Microsoft-Secure-Score/ba-p/182358) ist eine Sicherheit Analytics-Lösung, die Sie Einblick in das Portfolio Sicherheit und aufgeteilte zur Verfügung stehen. Mit einem einzigen Faktor können Sie besser verstehen, was Sie getan haben, um das Risiko in Microsoft-Lösungen zu reduzieren. Auch können Sie Ihr Ergebnis mit anderen Organisationen vergleichen und finden Sie unter wie Ihre Punktzahl über einen Zeitraum Trend wurde hat. Microsoft Graph [SecureScore](securescores.md) und [SecureScoreControlProfiles](securescorecontrolprofiles.md) Sicherheitsbereich unterstützen Sie bei der Anforderungen Ihrer Organisation Sicherheit und Produktivität beim Aktivieren der entsprechenden Mischung der Sicherheitsfeatures auszugleichen. Sie können auch project, was Ihr Ergebnis wäre, nachdem Sie die Sicherheitsfeatures übernehmen.

## <a name="common-use-cases"></a>Allgemeine Anwendungsfälle

Im folgenden sind einige der am häufigsten verwendeten Anforderungen für die Arbeit mit Microsoft Graph Security-API.

| **Anwendungsfälle**   | **REST-Ressourcen** | **Versuchen Sie es im Graph-Explorer** |
|:---------------|:--------|:----------|
| Warnungen auflisten | [Warnungen auflisten](../api/alert-list.md) | [https://graph.microsoft.com/beta/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=beta&GraphUrl=https://graph.microsoft.com) |
| Aktualisieren von Benachrichtigungen | [Warnung aktualisieren](../api/alert-update.md) | [https://graph.microsoft.com/beta/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com) |
|Liste sicherer Bewertungen|[Liste secureScores](../api/securescores-list.md) (Vorschau)|[https://graph.microsoft.com/beta/security/secureScores](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Liste sicherer Score Steuerelement Profile|[Liste secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) (Vorschau)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Update secure Score Steuerelement Profile|[SecureScoreControlProfiles aktualisieren](../api/securescorecontrolprofiles-update.md) (Vorschau)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com)|

Sie können Microsoft Graph [Webhooks](/graph/webhooks) abonnieren und Benachrichtigungen zu Updates für Microsoft Graph Security Entitäten verwenden.

## <a name="next-steps"></a>Nächste Schritte

Sicherheit-API von Microsoft Graph können neue Methoden, die Sie mit anderen Sicherheits-Lösungen von Microsoft und Partnern ausschließlich zu öffnen. Führen Sie diese Schritte, um die ersten Schritte beim:

- Ausführen eines Drilldowns in [Benachrichtigungen](alert.md), [SecureScore](securescores.md) (Preview) und [SecureScoreControlProfiles](securescorecontrolprofiles.md) (Preview).
- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus. Wählen Sie unter **Beispielabfragen** **Weitere Beispiele anzeigen** , und legen Sie die Kategorie Sicherheit auf **aktiviert**.
- Versuchen Sie es [abonnieren und Empfangen von Benachrichtigungen](/graph/webhooks) Entität ändert.

Benötigen Sie weitere Ideen? Dann sehen Sie sich an, [wie unsere Partner Microsoft Graph verwenden](https://developer.microsoft.com/graph/graph/examples#partners).

## <a name="see-also"></a>Siehe auch

Code und beitragen zu dieser Microsoft Graph Sicherheit API-Beispiele:

- [Beispiel für ASP.NET (c#)](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Python-Beispiel](https://github.com/microsoftgraph/python-security-rest-sample)
- [Beispiel Node.js (JavaScript)](https://github.com/microsoftgraph/nodejs-security-sample)

Bitten Sie die Community:

- [Teilnehmen an der Technikcommunity](https://aka.ms/graphsecuritycommunity)
- [Besprechen Sie StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph-security)
