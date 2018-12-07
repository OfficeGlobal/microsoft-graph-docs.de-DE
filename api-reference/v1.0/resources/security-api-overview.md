---
title: Verwenden der Sicherheits-API von Microsoft Graph
description: 'Die Microsoft Graph-Security-API bietet eine einheitliche Schnittstelle und Schema für die Integration der Sicherheitsfunktionen von Microsoft und Ökosystems Partnern. Dies ermöglicht Kunden Sicherheit Geschäftsabläufe zu optimieren und besser Schutz gegen Bedrohungen im Internet zu erhöhen. Sicherheit-API von Microsoft Graph kann zum Senden von Abfragen an alle Onboarded Sicherheitsanbieter abzurufenden aggregierte Antworten als ein Verbundbenutzer Aggregation Sicherheitsdienst verwendet werden. Verwenden von Microsoft Graph Sicherheit API Anwendungen erstellen, die:'
ms.openlocfilehash: b675ecd66081aec29f2727a394a91d9e2ee5fd5b
ms.sourcegitcommit: 4aebfaefc23e02a98b2fec35958cd2110020f15f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/06/2018
ms.locfileid: "27184518"
---
# <a name="use-the-microsoft-graph-security-api"></a>Verwenden der Sicherheits-API von Microsoft Graph

Die Microsoft Graph-Security-API bietet eine einheitliche Schnittstelle und Schema für die Integration der Sicherheitsfunktionen von Microsoft und Ökosystems Partnern. Dies ermöglicht Kunden Sicherheit Geschäftsabläufe zu optimieren und besser Schutz gegen Bedrohungen im Internet zu erhöhen. Sicherheit-API von Microsoft Graph kann zum Senden von Abfragen an alle Onboarded Sicherheitsanbieter abzurufenden aggregierte Antworten als ein Verbundbenutzer Aggregation Sicherheitsdienst verwendet werden. Verwenden von Microsoft Graph Sicherheit API Anwendungen erstellen, die:

- Konsolidieren Sie und korrelieren Sie Sicherheitshinweise aus mehreren Quellen
- Entsperren von Kontextdaten um Untersuchungen zu informieren.
- Automatisieren von Sicherheitsoperationen für größere Effizienz
- Transparenz für Sicherheitsdaten zur Ermöglichung von proaktiven Risikomanagement

Die Microsoft Graph-Security-API enthält die folgenden wichtigen Elemente.

## <a name="alerts"></a>Warnungen

Bei Benachrichtigungen handelt es sich um potenzielle Sicherheitsrisiken innerhalb eines Kunden Mandanten, die von Microsoft oder Partner sicherheitslösungen haben erkannt und für eine Aktion oder Benachrichtigung gekennzeichnet sind. Mit dieser Entität Microsoft Graph Security [Benachrichtigungen](alert.md) können Sie vereinheitlichen und Optimieren von Sicherheitsprobleme in alle integrierten Lösungen. Auf diese Weise können auch Applikationen zum Korrelieren von Warnungen und Kontext zum Schutz und die Antwortzeit zu verbessern. Diese entsperren Betriebseffizienz Sicherheit durch die Reduzierung von Untersuchung Zeit und Auflösung für Vorfälle. Mit der Funktion warnmeldungsaktualisierungs können Sie den Status von bestimmten Warnungen synchronisieren, über verschiedene Security-Produkte und Dienste, die mit der Microsoft Graph Security-API integriert sind, durch Aktualisieren der Entität [Benachrichtigungen](alert.md) .

Microsoft Graph Sicherheit Language-integrated Lösungen werden von die folgenden Sicherheitsanbieter Benachrichtigungen erhalten:

- [Azure-Sicherheitscenter](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)
- [Azure Active Directory-Schutz](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook)
- [Microsoft-Cloud-Anwendungssicherheit](https://docs.microsoft.com/cloud-app-security/monitor-alerts )
- [Windows-Defender erweiterte Schutz](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/attack-simulations-windows-defender-advanced-threat-protection)
- [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(Vorschau)**
- Microsoft Intune **(private Preview)**
- Office 365 **(bald verfügbar)**
- Azure erweiterte Threat Protection **(bald verfügbar)**
- Partnerlösungen wie Palo auch Netzwerke App-Framework

> **Hinweis:** Neue Anbieter sind kontinuierlich Onboarding auf das Microsoft Graph Security-Ökosystem.

## <a name="common-use-cases"></a>Allgemeine Anwendungsfälle

Im folgenden sind einige der am häufigsten verwendeten Anforderungen für die Arbeit mit Microsoft Graph Security-API:

| **Anwendungsfälle**   | **REST-Ressourcen** | **Versuchen Sie es im Graph-Explorer** |
|:---------------|:--------|:----------|
| Warnungen auflisten | [Warnungen auflisten](../api/alert-list.md) | [https://graph.microsoft.com/v1.0/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) |
| Aktualisieren von Benachrichtigungen | [Warnung aktualisieren](../api/alert-update.md) | [https://graph.microsoft.com/v1.0/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com) |

Sie können Microsoft Graph [Webhooks](/graph/webhooks) abonnieren und Benachrichtigungen zu Updates für Microsoft Graph Security Entitäten verwenden.

## <a name="resources"></a>Ressourcen

Code und beitragen zu dieser Microsoft Graph Sicherheit API-Beispiele:

- [Beispiel für ASP.NET (c#)](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Python-Beispiel](https://github.com/microsoftgraph/python-security-rest-sample)
- [Beispiel Node.js (JavaScript)](https://github.com/microsoftgraph/nodejs-security-sample)

Bitten Sie die Community:

- [Teilnehmen an der Technikcommunity](https://aka.ms/graphsecuritycommunity)
- [Besprechen Sie StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

## <a name="next-steps"></a>Nächste Schritte

Sicherheit-API von Microsoft Graph können neue Methoden, die Sie mit anderen Sicherheits-Lösungen von Microsoft und Partnern ausschließlich zu öffnen. Führen Sie diese Schritte, um die ersten Schritte beim:

- Ausführen eines Drilldowns in [Benachrichtigungen](alert.md).
- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus. Wählen Sie unter **Beispielabfragen** **Weitere Beispiele anzeigen** , und legen Sie die Kategorie Sicherheit auf **aktiviert**.
- Versuchen Sie es [abonnieren und Empfangen von Benachrichtigungen](/graph/webhooks) Entität ändert.

Benötigen Sie weitere Ideen? Dann sehen Sie sich an, [wie unsere Partner Microsoft Graph verwenden](https://developer.microsoft.com/graph/graph/examples#partners).
