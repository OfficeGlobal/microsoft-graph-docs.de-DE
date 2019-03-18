---
title: Verwenden der Sicherheits-API von Microsoft Graph
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Priority
author: preetikr
ms.prod: security
ms.openlocfilehash: 051bd2a09c59736d50eea5cbfa330ee0d7d2a198
ms.sourcegitcommit: cd4bdb2c6754b1d5658e68909ea6c219466da6df
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30644314"
---
# <a name="use-the-microsoft-graph-security-api"></a>Verwenden der Sicherheits-API von Microsoft Graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

## <a name="threat-indicators-preview"></a>Bedrohungsindikatoren (Vorschau)

Bedrohungsindikatoren, auch als Indicators of Compromise (IoC) bezeichnet, stellen Daten über bekannte Bedrohungen dar, wie beispielsweise bösartige Dateien, URLs, Domänen und IP-Adressen. Kunden können Indikatoren durch internes Sammeln von Informationen zu Bedrohungen (Threat Intelligence) generieren oder Indikatoren von Threat Intelligence Communities, lizenzierten Feeds und anderen Quellen erwerben. Dieser Indikatoren werden dann in verschiedenen Sicherheitstools zum Schutz vor verwandten Bedrohungen verwendet.

Die Microsoft Graph-Sicherheitsentität [tiIndicator](tiindicator.md) ermöglicht es Kunden, Bedrohungsindikatoren an Microsoft-Sicherheitslösungen zu übermitteln, um Blockier- und Warnaktionen bei bösartigen Aktivitäten zu aktivieren oder zu erlauben, wodurch Aktionen für Indikatoren unterdrückt werden, die als nicht relevant für ein Unternehmen eingestuft werden. Beim Senden von Indikatoren werden sowohl die Microsoft-Lösung angegeben, die den Indikator verwendet, als auch die Aktion, die für diesen Indikator angewendet wird.

Sie können die Entität [tiIndicator](tiindicator.md) in Ihre Anwendung integrieren oder eine der folgenden integrierten Threat Intelligence-Plattformen (TIP) verwenden:

- [Palo Alto Networks – MineMeld Threat Intelligence Sharing](https://www.paloaltonetworks.com/products/secure-the-network/subscriptions/minemeld)
- [MISP – Open Source Threat Intelligence Platform](http://www.misp-project.org/) verfügbar im [TI-Beispiel](https://aka.ms/tipmispsample)

Bedrohungsindikatoren, die über die Microsoft Graph-Sicherheits-API gesendet werden, sind heute in [Azure Sentinel](https://docs.microsoft.com/azure/sentinel/overview) (Vorschau) verfügbar, sodass Sie Bedrohungsindikatoren mit Protokolldaten korrelieren können, um Warnmeldungen über bösartige Aktivitäten zu erhalten. Unterstützung für andere Microsoft-Sicherheitsdienste, einschließlich Azure Firewall, wird in Kürze verfügbar sein.

## <a name="security-actions-preview"></a>Sicherheitsaktionen (Vorschau)

Ergreifen Sie sofortige Maßnahmen zum Schutz vor Bedrohungen mit der Microsoft Graph-Sicherheitsentität [securityAction](securityaction.md). Wenn ein Sicherheitsanalytiker einen neuen Indikator entdeckt, z. B. eine bösartige Datei, URL, Domäne oder IP-Adresse, kann der Schutz in Ihren Microsoft-Sicherheitslösungen sofort aktiviert werden. Rufen Sie eine Aktion für einen bestimmten Anbieter auf, zeigen Sie alle ausgeführten Aktionen an, und brechen Sie eine Aktion bei Bedarf ab. Probieren Sie Sicherheitsmaßnahmen mit [Windows Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) (demnächst verfügbar) aus, um bösartige Aktivitäten auf Ihren Windows-Endpunkten mithilfe von Eigenschaften zu blockieren, die in Warnmeldungen angezeigt oder bei Untersuchungen identifiziert wurden.

## <a name="secure-score-preview"></a>Secure Score (Vorschau)

[Microsoft Secure Score](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Office-365-Secure-Score-is-now-Microsoft-Secure-Score/ba-p/182358) ist eine Sicherheitsanalyselösung, mit der Sie Einblicke in Ihr Sicherheitsportfolio und in Verbesserungsmöglichkeiten erhalten. Anhand eines einzigen Faktors können Sie verstehen, wie Sie die Risiken in Microsoft-Lösungen minimieren können. Außerdem können Sie Ihre Bewertung mit anderen Organisationen vergleichen und sehen, wie sich Ihre Bewertung im Laufe der Zeit entwickelt hat. Mit der [SecureScore](securescores.md)- und der [SecureScoreControlProfiles](securescorecontrolprofiles.md)-Entität von Microsoft Graph-Sicherheit können Sie die Sicherheits- und Produktivitätsanforderungen Ihrer Organisation abwägen und dabei gleichzeitig die korrekte Mischung von Sicherheitsfunktionen aktivieren. Sie können auch projizieren, wie Ihre Bewertung nach Einführung von Sicherheitsfeatures aussehen würde.

## <a name="common-use-cases"></a>Allgemeine Anwendungsfälle

Im Folgenden werden einige der am häufigsten verwendeten Anfragen das Arbeiten mit der Sicherheit-APIs von Microsoft Graph vorgestellt.

| **Anwendungsfälle**   | **REST-Ressourcen** | **Ausprobieren im Graph-Tester** |
|:---------------|:--------|:----------|
| Warnungen auflisten | [Warnungen auflisten](../api/alert-list.md) | [https://graph.microsoft.com/beta/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=beta&GraphUrl=https://graph.microsoft.com) |
| Warnungen aktualisieren | [Warnung aktualisieren](../api/alert-update.md) </br> [Mehrere Warnungen aktualisieren](../api/alert-updatealerts.md) | [https://graph.microsoft.com/beta/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com) </br> [https://graph.microsoft.com/beta/security/alerts/updateAlerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/updateAlerts&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) |
| Sicherheitsaktion abrufen | [Sicherheitsaktion abrufen](../api/securityaction-get.md) (Vorschau)|[https://graph.microsoft.com/beta/security/securityActions/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions/{id}&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Sicherheitsaktionen auflisten| [Sicherheitsaktionen auflisten](../api/securityactions-list.md) (Vorschau)|[https://graph.microsoft.com/beta/security/securityActions](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Sicherheitsaktionen erstellen|[Sicherheitsaktionen erstellen](../api/securityactions-post.md) (Vorschau)|[https://graph.microsoft.com/beta/security/securityActions](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Sicherheitsaktionen abbrechen|[Sicherheitsaktionen abbrechen](../api/securityaction-cancelsecurityaction.md) (Vorschau)| [https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions/{id}/cancelSecurityAction&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) |
|TI-Indikator abrufen|[TI-Indikator abrufen](../api/tiindicator-get.md) (Vorschau)| [https://graph.microsoft.com/beta/security/tiIndicators/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/{id}&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|TI-Indikatoren auflisten | [TI-Indikatoren auflisten](../api/tiindicators-list.md) (Vorschau) | [https://graph.microsoft.com/beta/security/tiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|TI-Indikator erstellen|[TI-Indikator erstellen](../api/tiindicators-post.md) (Vorschau)|[https://graph.microsoft.com/beta/security/tiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|TI-Indikatoren senden|[TI-Indikatoren senden](../api/tiindicator-submittiindicators.md) (Vorschau)| [https://graph.microsoft.com/beta/security/tiIndicators/submitTiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/submitTiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) |
|TI-Indikatoren aktualisieren|[TI-Indikator aktualisieren](../api/tiindicator-update.md) (Vorschau) </br>[Mehrere TI-Indikatoren aktualisieren](../api/tiindicator-updatetiindicators.md) (Vorschau)| [https://graph.microsoft.com/beta/security/tiIndicators/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/{id}&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) </br>[https://graph.microsoft.com/beta/security/tiIndicators/updateTiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/updateTiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|TI-Indikatoren löschen|[TI-Indikator löschen](../api/tiindicator-delete.md) (Vorschau) </br>[Mehrere TI-Indikatoren löschen](../api/tiindicator-deletetiindicators.md) (Vorschau) </br>[TI-Indikator durch externalId löschen](../api/tiindicator-deletetiindicatorsbyexternalid.md) (Vorschau)| LÖSCHEN </br>[https://graph.microsoft.com/beta/security/tiIndicators/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/{id}&method=DELETE&version=beta&GraphUrl=https://graph.microsoft.com) </br>POST</br>[https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/deleteTiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)</br>POST</br>[https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicatorsByExternalId](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/deleteTiIndicatorsByExternalId&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Sicherheitsbewertungen auflisten|[secureScores auflisten](../api/securescores-list.md)|[https://graph.microsoft.com/beta/security/secureScores](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Profile für Steuerung der Sicherheitsbewertung auflisten|[secureScoreControlProfiles auflisten](../api/securescorecontrolprofiles-list.md)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Profile für Steuerung der Sicherheitsbewertung aktualisieren|[secureScoreControlProfiles aktualisieren](../api/securescorecontrolprofiles-update.md)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com)|

Sie können Microsoft Graph-[Webhooks](/graph/webhooks) verwenden, um Benachrichtigungen über Aktualisierungen von Entitäten der Microsoft Graph-Sicherheits-API zu abonnieren und zu empfangen.

## <a name="next-steps"></a>Nächste Schritte

Die Sicherheits-API von Microsoft Graph kann neue Möglichkeiten zum Arbeiten mit anderen Sicherheitslösungen von Microsoft und Partnern eröffnen. Gehen Sie folgendermaßen vor, um loszulegen:

- Führen Sie einen Drilldown zu [Warnungen](alert.md), [tiIndicator](tiindicator.md) (Vorschau), [securityAction](securityaction.md) (Vorschau), [secureScore](securescores.md) (Vorschau), and [secureScoreControlProfiles](securescorecontrolprofiles.md) (Vorschau) aus.
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/security-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
