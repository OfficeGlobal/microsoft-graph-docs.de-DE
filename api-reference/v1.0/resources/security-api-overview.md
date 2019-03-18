---
title: Verwenden der Sicherheits-API von Microsoft Graph
description: 'Die Sicherheits-API von Microsoft Graph bietet eine einheitliche Oberfläche und ein Schema zur Integration in Sicherheitslösungen von Microsoft- und Ökosystem-Partnern. Auf diese Weise können Kunden Sicherheitsvorgänge optimieren und sich besser vor zunehmenden Cyberbedrohungen schützen. Die Sicherheits-API von Microsoft Graph kann als Dienst zur Aggregation von Verbundsicherheit verwendet werden, um Abfragen an alle integrierten Sicherheitsanbieter zu übermitteln und zusammengefasste Antworten zu erhalten. Verwenden Sie die Microsoft Graph-Sicherheits-API, um Anwendungen zu erstellen, die:'
localization_priority: Priority
author: preetikr
ms.prod: security
ms.openlocfilehash: bd208067c2194766bb5f3d93d0caa21be086dca0
ms.sourcegitcommit: cd4bdb2c6754b1d5658e68909ea6c219466da6df
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30644265"
---
# <a name="use-the-microsoft-graph-security-api"></a>Verwenden der Microsoft Graph-Sicherheits-API

Die Sicherheits-API von Microsoft Graph bietet eine einheitliche Oberfläche und ein Schema zur Integration in Sicherheitslösungen von Microsoft- und Ökosystem-Partnern. Auf diese Weise können Kunden Sicherheitsvorgänge optimieren und sich besser vor zunehmenden Cyberbedrohungen schützen. Die Microsoft Graph-Sicherheits-API fasst Abfragen an alle integrierten Sicherheitsanbieter zusammen und aggregiert die Antworten. Verwenden Sie die Microsoft Graph-Sicherheits-API, um Anwendungen zu erstellen, die:

- Sicherheitswarnungen aus mehreren Quellen konsolidieren und korrelieren
- Die Sperrung kontextbezogener Daten aufheben, um Untersuchungen zu ermöglichen
- Sicherheitsaufgaben, Geschäftsprozesse, Workflows und Berichte automatisieren
- Bedrohungsindikatoren an Microsoft-Produkte zur individuellen Erkennung senden
- Aktionen als Reaktion auf neue Bedrohungen aufrufen
- Einblicke in Sicherheitsdaten liefern, um ein proaktives Risikomanagement zu ermöglichen

Die Sicherheits-API von Microsoft Graph umfasst die folgenden wichtigen Entitäten.

## <a name="alerts"></a>Warnungen

Warnungen sind potenzielle Sicherheitsprobleme im Mandanten des Kunden, die von Sicherheitslösungen von Microsoft oder Partnern identifiziert und entsprechend gekennzeichnet wurden, sodass Maßnahmen ergriffen oder Benachrichtigungen gesendet werden. Mit der Microsoft Graph-Sicherheitsentität [alerts](alert.md) können Sie die Verwaltung von Sicherheitsproblemen über alle integrierten Lösungen hinweg vereinheitlichen und optimieren. Auf diese Weise können Warnungen und Kontext in Anwendungen korreliert werden, wodurch der Bedrohungsschutz und die Reaktionszeit verbessert werden. Mit der Funktion zum Aktualisieren der Warnung können Sie den Status bestimmter Warnungen über unterschiedliche Sicherheitsprodukte und -dienste hinweg, die in die Sicherheits-API von Microsoft Graph integriert sind, synchronisieren, indem Sie die [alerts](alert.md)-Entität aktualisieren.

Warnungen der folgenden Anbieter sind über die Microsoft Graph-Sicherheits-API verfügbar. Die Unterstützung für GET-Warnungen, PATCH-Warnungen (Updates sind über die Microsoft Graph-Sicherheits-API verfügbar, werden aber möglicherweise in der Verwaltungsumgebung des Anbieters nicht angezeigt) und das Abonnieren von Warnungen ("Subscribe" über Webhooks) wird in der folgenden Tabelle aufgeführt.

| Sicherheitsanbieter | <p align="center">GET-Warnung</p>| <p align="center">PATCH-Warnung</p>| <p align="center">Warnung abonnieren</p>|
|:------------------|:---------|:-----------|:------------------|
|[Azure Security Center](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|[Azure Active Directory Identity Protection](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook) | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
| [Microsoft Cloud App Security](https://docs.microsoft.com/cloud-app-security/monitor-alerts) | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|[Windows Defender Advanced Threat Protection](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/attack-simulations-windows-defender-advanced-threat-protection)| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center"> [Dateiproblem](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Azure Advanced Threat Protection](https://docs.microsoft.com/azure-advanced-threat-protection/understanding-security-alerts#security-alert-categories)| <p align="center">&#x2713;</p> | <p align="center"> [Dateiproblem](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [Dateiproblem](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|Office 365 <ul><li> [Standard](https://docs.microsoft.com/de-DE/office365/securitycompliance/alert-policies#default-alert-policies)</li> <li>[Cloud-App-Sicherheit](https://docs.microsoft.com/de-DE/office365/securitycompliance/anomaly-detection-policies-in-ocas)</li></ul> | <p align="center">&#x2713;</p> | <p align="center"> [Dateiproblem](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [Dateiproblem](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Azure Information Protection](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(Vorschau)**| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|[Azure Sentinel](https://docs.microsoft.com/azure/sentinel/quickstart-get-visibility) **(Vorschau)**| <p align="center">&#x2713;</p> | <p align="center"> [Dateiproblem](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [Dateiproblem](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Palo Alto Networks](https://docs.paloaltonetworks.com/pan-os/9-0/pan-os-web-interface-help/monitor/monitor-logs/log-types.html)| <p align="center">&#x2713;</p> | <p align="center"> [Dateiproblem](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [Dateiproblem](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
> **Hinweis:** In das Microsoft Graph-Sicherheitsökosystem werden ständige neue Anbieter eingegliedert. Um neue Anbieter anzufordern oder erweiterte Unterstützung von bestehenden Anbietern zu erhalten, [melden Sie ein Problem im GitHub-Repository der Microsoft Graph-Sicherheits-API](https://github.com/microsoftgraph/security-api-solutions/issues/new) an.

## <a name="common-use-cases"></a>Allgemeine Anwendungsfälle

Im Folgenden werden einige der am häufigsten verwendeten Anfragen das Arbeiten mit der Microsoft Graph-Sicherheits-API vorgestellt:

| **Anwendungsfälle**   | **REST-Ressourcen** | **Ausprobieren im Graph-Tester** |
|:---------------|:--------|:----------|
| Warnungen auflisten | [Warnungen auflisten](../api/alert-list.md) | [https://graph.microsoft.com/v1.0/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) |
| Warnungen aktualisieren | [Warnung aktualisieren](../api/alert-update.md) | [https://graph.microsoft.com/v1.0/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com) |

Sie können Microsoft Graph-[Webhooks](/graph/webhooks) verwenden, um Benachrichtigungen über Sicherheitsentitäten von Microsoft Graph zu abonnieren und zu erhalten.

## <a name="resources"></a>Ressourcen

Code und Beiträge zu den folgenden Beispielen für die Microsoft Graph-Sicherheits-API:

- [ASP.NET (C#)-Beispiel](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Python-Beispiel](https://github.com/microsoftgraph/python-security-rest-sample)
- [Node.js (JavaScript)-Beispiel](https://github.com/microsoftgraph/nodejs-security-sample)

Interaktion mit der Community:

- [Treten Sie der technische Access-Community bei](https://aka.ms/graphsecuritycommunity)
- [Diskutieren auf StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

## <a name="next-steps"></a>Nächste Schritte

Die Sicherheits-API von Microsoft Graph kann neue Möglichkeiten zum Arbeiten mit anderen Sicherheitslösungen von Microsoft und Partnern eröffnen. Gehen Sie folgendermaßen vor, um loszulegen:

- Führen Sie einen Drilldown zu [Warnungen](alert.md) aus.
- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus. Klicken Sie unter **Beispielabfragen** auf **Mehr Beispiele anzeigen**, und legen Sie die Kategorie „Sicherheit“ auf **ein** fest.
- Versuchen Sie, [Benachrichtigungen zu Entitätsänderungen zu abonnieren und zu erhalten](/graph/webhooks).

Benötigen Sie weitere Ideen? Dann sehen Sie sich an, [wie unsere Partner Microsoft Graph verwenden](https://developer.microsoft.com/graph/graph/examples#partners).

## <a name="see-also"></a>Weitere Artikel

[Code und Beiträge](https://github.com/microsoftgraph/security-api-solutions/blob/master/CONTRIBUTING.md) zu den folgenden Beispielen für die Microsoft Graph-Sicherheits-API:

- [ASP.NET (C#)-Beispiel](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Python-Beispiel](https://github.com/microsoftgraph/python-security-rest-sample)
- [Node.js (JavaScript)-Beispiel](https://github.com/microsoftgraph/nodejs-security-sample)
- [PowerShell-Beispiel](https://aka.ms/graphsecuritypowershellsample)
- [Andere Beispiele oder Einbringen einer neuen Stichprobe](https://aka.ms/graphsecurityapicode)

Weitere Optionen zur Verbindung mit der Microsoft Graph-Sicherheits-API finden Sie hier:

- [Microsoft Graph-Sicherheitsconnectors für Logic Apps, Flow Apps und PowerApps](https://aka.ms/graphsecurityconnectors)
- [Microsoft Graph-Sicherheitsconnectors für Power BI](https://aka.ms/graphsecuritypowerbiconnectordoc)
- [Beispiele für ein Jupyter-Notizbuch](https://aka.ms/graphsecurityjupyternotebooks)

Interaktion mit der Community:

- [Treten Sie der technische Access-Community bei](https://aka.ms/graphsecuritycommunity)
- [Diskutieren auf StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph-security)