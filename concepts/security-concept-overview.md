---
title: Übersicht über die Sicherheits-API von Microsoft Graph
description: Sie können die Sicherheits-API von Microsoft Graph verwenden, um eine Verbindung zu Microsoft-Sicherheitsprodukten, -Diensten- und -Partnern herzustellen, um Sicherheitsvorgänge zu optimieren und den Schutz vor Bedrohungen, deren Erkennung sowie die Reaktionsmöglichkeiten zu verbessern. Die Sicherheits-API von Microsoft Graph ist ein zwischengeschalteter Dienst (oder Broker), der eine einzige programmgesteuerte Schnittstelle bietet, um mehrere Microsoft Graph-Sicherheitsanbieter (auch als Sicherheitsanbieter oder Anbieter bezeichnet) zu verbinden. Anforderungen an die Sicherheits-API von Microsoft Graph gelten im Verbund für alle anwendbaren Sicherheitsanbieter. Die Ergebnisse werden aggregiert und an die anfordernde Anwendung in einem gemeinsamen Schema zurückgegeben, wie im folgenden Diagramm dargestellt. Einzelheiten hierzu finden Sie unter „Datenfluss der Sicherheits-API in Microsoft Graph“.
ms.openlocfilehash: b5e1fb3d60cfc55cb940a217aaba872175887297
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092173"
---
# <a name="microsoft-graph-security-api-overview"></a>Übersicht über die Sicherheits-API von Microsoft Graph

Sie können die Sicherheits-API von Microsoft Graph verwenden, um eine Verbindung zu Microsoft-Sicherheitsprodukten, -Diensten- und -Partnern herzustellen, um Sicherheitsvorgänge zu optimieren und den Schutz vor Bedrohungen, deren Erkennung sowie die Reaktionsmöglichkeiten zu verbessern. Die Sicherheits-API von Microsoft Graph ist ein zwischengeschalteter Dienst (oder Broker), der eine einzige programmgesteuerte Schnittstelle bietet, um mehrere [Microsoft Graph-Sicherheitsanbieter](/graph/api/resources/securityvendorinformation?view=graph-rest-1.0) (auch als Sicherheitsanbieter oder Anbieter bezeichnet) zu verbinden. Anforderungen an die Sicherheits-API von Microsoft Graph gelten im Verbund für alle anwendbaren Sicherheitsanbieter. Die Ergebnisse werden aggregiert und an die anfordernde Anwendung in einem gemeinsamen Schema zurückgegeben, wie im folgenden Diagramm dargestellt. Einzelheiten hierzu finden Sie unter [Datenfluss der Sicherheits-API in Microsoft Graph](security-dataflow.md).

![security_overview_diagram_1.png](./images/security-overview-diagram-1.png)

Weitere Informationen zur Autorisierung finden Sie unter [Autorisierung und Sicherheits-API von Microsoft Graph](security-authorization.md). Weitere Informationen zu Berechtigungen, einschließlich delegierter und Anwendungsberechtigungen, finden Sie unter [Berechtigungen](permissions-reference.md#security-permissions).

## <a name="why-use-the-microsoft-graph-security-api"></a>Vorteile der Sicherheits-API von Microsoft Graph

Die [Sicherheits-API von Microsoft Graph](/graph/api/resources/security-api-overview?view=graph-rest-1.0) erleichtert das Herstellen einer Verbindung mit Sicherheitsprodukten und -diensten von verschiedenen Microsoft-Partnern. Sie ermöglicht es Ihnen, den Wert dieser Lösungen besser zu erkennen und ggf. zu erweitern.

### <a name="unify-and-standardize-alert-tracking"></a>Vereinheitlichen und Standardisieren der Warnungsverfolgung

Schreiben Sie einmalig Code, um Warnungen aus beliebigen in Microsoft Graph integrierten Sicherheitslösungen zu integrieren, und halten Sie Warnungsstatus und Aufgaben für alle Lösungen synchronisiert. Sie können Warnungen auch zu SIEM-Lösungen (Security Information and Event Management) wie Splunk und IBM QRadar über [Azure Monitor](https://docs.microsoft.com/de-DE/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub) streamen. Informationen zur Integration von SIEM in die Sicherheits-API finden Sie unter [Integrieren in SIEM](security-siemintegration.md).

### <a name="correlate-security-alerts-to-improve-threat-protection-and-response"></a>Korrelierende Sicherheitswarnungen zur Verbesserung des Bedrohungsschutzes und der Reaktion

Korrelieren Sie Warnungen über Sicherheitslösungen hinweg mit einem einheitlichen Warnungsschema. Auf diese Weise erhalten Sie nicht nur umsetzbare Informationen zu Warnungen; Sicherheitsanalysten können damit auch Warnungen auch mit Informationen zu Ressourcen und Benutzern ergänzen, wodurch eine schnellere Reaktion auf Bedrohungen und der Schutz von Objekten ermöglicht wird.  

### <a name="update-alert-tags-status-and-assignments"></a>Aktualisieren von Warnungskategorien, -status und -zuweisungen

Kategorisieren Sie Benachrichtigungen mit zusätzlichem Kontext oder Informationen zu Bedrohungen, um über die Reaktion und Behebung zu informieren. Stellen Sie sicher, dass Kommentare und Feedback zu Warnungen für alle Workflows sichtbar sind. Synchronisierung Sie Warnungsstatus und -zuweisungen, damit alle integrierten Lösungen den aktuellen Status widerspiegeln. Verwenden Sie Webhook-Abonnements, um über Änderungen benachrichtigt zu werden.  

### <a name="unlock-security-context-to-drive-investigation"></a>Aufheben der Sperrung von Sicherheitskontext zu Untersuchungszwecken

Gewinnen Sie Einblicke in den sicherheitsrelevanten Bestand (z. B. Benutzer, Hosts und Apps), und fügen Sie organisatorischen Kontext von anderen Microsoft Graph-Anbietern (Azure Active Directory, Microsoft Intune, Office 365) hinzu, um Business- und Sicherheitskontexte zusammenzubringen und die Reaktion auf Sicherheitsrisiken zu verbessern.

### <a name="proactively-manage-security-risks-preview"></a>Proaktives Verwalten von Sicherheitsrisiken (Vorschau)

Verwenden Sie Microsoft Secure Store (Vorschau), um Einblicke in die Sicherheitsanforderungen Ihrer Organisation bereitzustellen und Vorschläge zur Verbesserung zu erhalten und eine Verbesserung vorherzusagen, nachdem diese Vorschläge umgesetzt wurden. Messen Sie ganz einfach Ihre Fortschritte im Zeitablauf, und erhalten Sie Einblicke in bestimmte Änderungen, die zu Verbesserung führen.

## <a name="benefits-of-using-the-microsoft-graph-security-api"></a>Vorteile der Verwendung der Sicherheits-API von Microsoft Graph

In der folgenden Tabelle sin die Vorteile aufgeführt, die unterschiedliche Sicherheitslösungen durch Integration in die Sicherheits-API von Microsoft Graph nutzen können.  

|**Bereich**     | **Nutzen**|
|:---------------|:---------|
|**Managed Security Service Providers (MSSPs)**|<ul><li>Optimierte Integration in Sicherheitstools und -dienste.</li> <li>Reduzierter Zeitaufwand und weniger Aufwand für Bereitstellung und Wartung.</li> <li>Die Möglichkeit, MSSP-Kunden einen Mehrwert bereitzustellen.</li></ul>|
|**SIEM- und Risikomanagementlösungen**|<ul><li>Nahtlose Integration in Microsoft-Sicherheitslösungen und Ökosystempartner.</li> <li>Vielfältige Warnungsmetadaten.</li> <li>Bessere Warnungskorrelation.</li></ul>|
|**Anwendungen** <br>(Informationen zu Bedrohungen, Mobile, Cloud, IOT, Betrugsaufdeckung, Identität & Zugriff, Risiko & Compliance, Firewall usw.)|<ul><li>Einheitliche Bedrohungsverwaltung, Verhinderung und einheitliches Risikomanagement über unterschiedliche Sicherheitslösungen hinweg.</li> <li>Benachrichtigungen, Bestand, Konfiguration und Aktionen werden über Microsoft Graph verfügbar gemacht.</li> <li>Sofortige Integration in Microsoft Graph-aktivierte Lösungen.</li></ul>|

## <a name="api-reference"></a>API-Referenz
Suchen Sie die API-Referenz für diesen Dienst?

- [Sicherheits-API in Microsoft Graph v1.0](/graph/api/resources/security-api-overview?view=graph-rest-1.0)
- [Sicherheits-API in Microsoft Graph, Betaversion](/graph/api/resources/security-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a>Nächste Schritte

- [Verwenden der Sicherheits-API von Microsoft Graph](/graph/api/resources/security-api-overview?view=graph-rest-1.0)
- Möchten Sie erfahren, wie Sie ein Sicherheitsanbieter werden können? Wenden Sie sich an [graphsecfeedback](mailto:graphsecfeedback@microsoft.com).
