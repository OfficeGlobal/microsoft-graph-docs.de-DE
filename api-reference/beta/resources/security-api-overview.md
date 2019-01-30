---
title: Verwenden der Sicherheits-API von Microsoft Graph
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Priority
author: preetikr
ms.prod: security
ms.openlocfilehash: 042c63cfee833a1f9c7493a9e35a6bbb8eb2fbaa
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643087"
---
# <a name="use-the-microsoft-graph-security-api"></a>Verwenden der Sicherheits-API von Microsoft Graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die Sicherheits-API von Microsoft Graph bietet eine einheitliche Oberfläche und ein Schema zur Integration in Sicherheitslösungen von Microsoft- und Ökosystem-Partnern. Auf diese Weise können Kunden Sicherheitsvorgänge optimieren und sich besser vor zunehmenden Cyberbedrohungen schützen. Die Sicherheits-API von Microsoft Graph kann als Dienst zur Aggregation von Verbundsicherheit verwendet werden, um Abfragen an alle integrierten Sicherheitsanbieter zu übermitteln und zusammengefasste Antworten zu erhalten. Verwenden Sie die Sicherheits-API von Microsoft Graph, um Anwendungen zu erstellen, die:

- Sicherheitswarnungen aus mehreren Quellen konsolidieren und korrelieren
- Die Sperrung kontextbezogener Daten aufheben, um Untersuchungen zu ermöglichen
- Sicherheitsvorgänge für größere Effizienz automatisieren
- Einblicke in Sicherheitsdaten liefern, um ein proaktives Risikomanagement zu ermöglichen

Die Sicherheits-API von Microsoft Graph umfasst die folgenden wichtigen Entitäten.

## <a name="alerts"></a>Warnungen

Benachrichtigungen sind potenzielle Sicherheitsprobleme im Mandanten des Kunden, die von Sicherheitslösungen von Microsoft oder Partnern identifiziert und entsprechend gekennzeichnet wurden, sodass Maßnahmen ergriffen oder Benachrichtigungen gesendet werden. Mit der [alerts](alert.md)-Entität von Microsoft Graph können Sie Sicherheitswarnungen über alle integrierten Lösungen hinweg vereinheitlichen und optimieren. Auf diese Weise können Warnungen und Kontext in Anwendungen korreliert werden, wodurch der Bedrohungsschutz und die Reaktionszeit verbessert werden. So wird die Effizienz von Sicherheitsvorgängen erhöht, indem die Zeit für die Untersuchung und Lösung von Zwischenfällen reduziert wird. Mit der Funktion zum Aktualisieren der Warnung können Sie den Status bestimmter Warnungen über unterschiedliche Sicherheitsprodukte und -dienste hinweg, die in die Sicherheits-API von Microsoft Graph integriert sind, synchronisieren, indem Sie die [alerts](alert.md)-Entität aktualisieren.

In Microsoft Graph-Sicherheit integrierte Lösungen erhalten Warnungen von den folgenden Sicherheitsanbietern:

- [Azure Security Center](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)
- [Azure Active Directory Identity Protection](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook)
- [Microsoft Cloud Application Security](https://docs.microsoft.com/cloud-app-security/monitor-alerts )
- [Windows Defender Advanced Threat Protection](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/attack-simulations-windows-defender-advanced-threat-protection)
- [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(Vorschau)**
- Microsoft Intune **(private Vorschau)**
- Office 365 ** (bald verfügbar)**
- Azure Advanced Threat Protection **(bald verfügbar)**
- Partnerlösungen, z. B. Palo Alto Networks App Framework

> **Hinweis:** In das Microsoft Graph-Sicherheitsökosystem werden ständige neue Anbieter eingegliedert.

## <a name="secure-score-preview"></a>Secure Score (Vorschau)

[Microsoft Secure Score](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Office-365-Secure-Score-is-now-Microsoft-Secure-Score/ba-p/182358) ist eine Sicherheitsanalyselösung, mit der Sie Einblicke in Ihr Sicherheitsportfolio und in Verbesserungsmöglichkeiten erhalten. Anhand eines einzigen Faktors können Sie verstehen, wie Sie die Risiken in Microsoft-Lösungen minimieren können. Außerdem können Sie Ihre Bewertung mit anderen Organisationen vergleichen und sehen, wie sich Ihre Bewertung im Laufe der Zeit entwickelt hat. Mit der [SecureScore](securescores.md)- und der [SecureScoreControlProfiles](securescorecontrolprofiles.md)-Entität von Microsoft Graph-Sicherheit können Sie die Sicherheits- und Produktivitätsanforderungen Ihrer Organisation abwägen und dabei gleichzeitig die korrekte Mischung von Sicherheitsfunktionen aktivieren. Sie können auch projizieren, wie Ihre Bewertung nach Einführung von Sicherheitsfeatures aussehen würde.

## <a name="common-use-cases"></a>Allgemeine Anwendungsfälle

Im Folgenden werden einige der am häufigsten verwendeten Anfragen das Arbeiten mit der Sicherheit-APIs von Microsoft Graph vorgestellt.

| **Anwendungsfälle**   | **REST-Ressourcen** | **Ausprobieren im Graph-Tester** |
|:---------------|:--------|:----------|
| Warnungen auflisten | [Warnungen auflisten](../api/alert-list.md) | [https://graph.microsoft.com/beta/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=beta&GraphUrl=https://graph.microsoft.com) |
| Warnungen aktualisieren | [Warnung aktualisieren](../api/alert-update.md) | [https://graph.microsoft.com/beta/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com) |
|Sicherheitsbewertungen auflisten|[secureScores auflisten](../api/securescores-list.md)|[https://graph.microsoft.com/beta/security/secureScores](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Profile für Steuerung der Sicherheitsbewertung auflisten|[secureScoreControlProfiles auflisten](../api/securescorecontrolprofiles-list.md)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Profile für Steuerung der Sicherheitsbewertung aktualisieren|[secureScoreControlProfiles aktualisieren](../api/securescorecontrolprofiles-update.md)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com)|

Sie können Microsoft Graph-[Webhooks](/graph/webhooks) verwenden, um Benachrichtigungen über Sicherheitsentitäten von Microsoft Graph zu abonnieren und zu erhalten.

## <a name="next-steps"></a>Nächste Schritte

Die Sicherheits-API von Microsoft Graph kann neue Möglichkeiten zum Arbeiten mit anderen Sicherheitslösungen von Microsoft und Partnern eröffnen. Gehen Sie folgendermaßen vor, um loszulegen:

- Führen Sie einen Drilldown zu [Warnungen](alert.md), [secureScore](securescores.md) (Vorschau) und [secureScoreControlProfiles](securescorecontrolprofiles.md) (Vorschau) aus.
- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus. Klicken Sie unter **Beispielabfragen** auf **Mehr Beispiele anzeigen**, und legen Sie die Kategorie „Sicherheit“ auf **ein** fest.
- Versuchen Sie, [Benachrichtigungen zu Entitätsänderungen zu abonnieren und zu erhalten](/graph/webhooks).

Benötigen Sie weitere Ideen? Dann sehen Sie sich an, [wie unsere Partner Microsoft Graph verwenden](https://developer.microsoft.com/graph/graph/examples#partners).

## <a name="see-also"></a>Siehe auch

Code und Beiträge zu den folgenden Beispielen für die Sicherheits-API in Microsoft Graph:

- [ASP.NET (C#)-Beispiel](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Python-Beispiel](https://github.com/microsoftgraph/python-security-rest-sample)
- [Node.js (JavaScript)-Beispiel](https://github.com/microsoftgraph/nodejs-security-sample)

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
