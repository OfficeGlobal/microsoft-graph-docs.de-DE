# <a name="use-the-microsoft-graph-security-api"></a>Verwendung der Sicherheits-API von Microsoft Graph

Die Microsoft Graph Security API bietet eine einheitliche Schnittstelle und ein einheitliches Schema für die Integration mit Sicherheitslösungen von Microsoft und Ökosystempartnern. Dies ermöglicht es Kunden, die Sicherheitsabläufe zu verbessern und sich besser gegen zunehmende Cyber-Bedrohungen zu schützen. Die Microsoft Graph Security API kann als Verbundsicherheits-Aggregationsdienst verwendet werden, um Abfragen an alle integrierten Sicherheitsanbieter zu senden, um aggregierte Antworten zu erhalten. Verwenden von Microsoft Graph Sicherheits-API, um Anwendungen zu erstellen, die:

- Sicherheitshinweise aus mehreren Quellen konsolidieren und sie korrelieren
- Kontextdaten entsperren, um Untersuchungen zu informieren
- Sicherheitsoperationen für mehr Effizienz automatisieren
- Sichtbarkeit in Sicherheitsdaten umwandeln, um ein proaktives Risikomanagement zu ermöglichen

Die Microsoft Graph-Security-API enthält die folgenden Schlüsselelemente.

## <a name="alerts"></a>Warnungen

Warnmeldungen sind potenzielle Sicherheitsprobleme innerhalb des Mandanten eines Kunden, die Microsoft oder Partner-Sicherheitslösungen identifiziert und für Aktionen oder Benachrichtigungen gekennzeichnet haben. Mit der Entität Microsoft Graph Security [Alarme](alert.md) können Sie Sicherheitsprobleme in allen integrierten Lösungen vereinheitlichen und optimieren. Dadurch können Anwendungen auch Warnungen und Kontext korrelieren, um den Schutz und die Reaktion auf eine Bedrohung zu verbessern. Dadurch wird die betriebliche Effizienz der Sicherheit durch die Verkürzung der Untersuchungszeit und der Zeit bis zur Lösung von Vorfällen erhöht. Mit der Möglichkeit zur Aktualisierung von Benachrichtigungen können Sie den Status bestimmter Benachrichtigungen über verschiedene Sicherheitsprodukte und -dienste hinweg synchronisieren, die in die Microsoft Graph Security API integriert sind, indem Sie Ihre Entität [Alarme](alert.md) aktualisieren.

Microsoft Graph Security-integrierte Lösungen erhalten Warnmeldungen von den folgenden Sicherheitsanbietern:

- Azure Security Center
- Azure Active Directory Identity Protection
- Azure Information Protection
- Microsoft Cloud Application Security
- Windows Defender Advanced Threat Protection
- Microsoft Intune (private Vorschau)
- Office 365 (bald verfügbar)
- Partnerlösungen wie Palo Alto Networks App Framework

> **Hinweis:** Neue Anbieter werden laufend in das Microsoft Graph Security Ökosystem eingebunden.

## <a name="common-use-cases"></a>Allgemeine Anwendungsfälle

Im Folgenden finden Sie einige der beliebtesten Anfragen für die Arbeit mit der Microsoft Graph Security API:

| **Anwendungsfälle**   | **REST-Ressourcen** | **Ausprobieren im Graph-Tester** |
|:---------------|:--------|:----------|
| Warnungen auflisten | [Warnungen auflisten](../api/alert_list.md) | [https://graph.microsoft.com/v1.0/security/alerts](https://developer.microsoft.com/en-us/graph/graph-explorer?request=security/alerts&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) |
| Warnungen aktualisieren | [Warnung aktualisieren](../api/alert_update.md) | [https://graph.microsoft.com/v1.0/security/alerts/{alert-id}](https://developer.microsoft.com/en-us/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com) |

Sie können Microsoft Graph [Webhooks](../../../concepts/webhooks.md) verwenden, um Benachrichtigungen über Updates von Microsoft Graph Security Entitäten zu abonnieren und erhalten.

## <a name="resources"></a>Ressourcen

Code und Beitrag zu diesen Stichproben der Microsoft Graph Security API:

- [Stichprobe für ASP.NET (C#)](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Python-Stichprobe](https://github.com/microsoftgraph/python-security-rest-sample)
- [Node.js (JavaScript) Stichprobe](https://github.com/microsoftgraph/nodejs-security-sample)

Sich in der Community engagieren

- [Der Tech-Community beitreten](https://aka.ms/graphsecuritycommunity)
- [Über StackOverflow diskutieren](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

## <a name="next-steps"></a>Nächste Schritte

Die Microsoft Graph Security API kann Ihnen neue Möglichkeiten eröffnen, mit verschiedenen Sicherheitslösungen von Microsoft und Partnern zu arbeiten. Folgen Sie diesen Schritten, um loszulegen:

- Ausführen eines Drilldowns in [Alarme](alert.md).
- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus. Wählen Sie unter **Stichproben-Abfragen** **Weitere Beispiele anzeigen** , und stellen Sie die Kategorie Sicherheit auf **aktiviert**ein.
- Versuchen Sie, [zu abonnieren und Benachrichtigungen](../../../concepts/webhooks.md) bei Änderungen an der Entität zu erhalten.

Benötigen Sie weitere Ideen? Dann sehen Sie sich an, [wie unsere Partner Microsoft Graph verwenden](https://developer.microsoft.com/graph/graph/examples#partners).
