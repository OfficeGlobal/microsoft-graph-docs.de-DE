# <a name="microsoft-graph-security-api-overview"></a>Microsoft Graph Sicherheits-API (Übersicht)

Mit der Sicherheits-API von Microsoft Graph können Sie eine Verbindung mit Microsoft Security-Produkten, Dienstleistungen und Partnern herstellen, um die Sicherheitsoperationen zu optimieren und den Schutz vor Bedrohungen und die Erkennungs- und Antwortkapazitäten zu verbessern. Die Microsoft Graph Sicherheits-API ist ein zwischengeschalteter Service (oder ein Makler), der eine einzige Programmierschnittstelle für die Verbindung mehrerer [Sicherheits-Anbieter für Microsoft Graphty](../api-reference/v1.0/resources/securityvendorinformation.md) (auch Sicherheitsanbieter oder Anbieter genannt), bereitstellt. Anforderungen an die Microsoft Graph-Sicherheits-API sind mit allen anwendbaren Sicherheitsanbietern verbunden. Die Ergebnisse werden aggregiert und in einem gemeinsamen Schema an die anfordernde Anwendung zurückgegeben, wie in der folgenden Abbildung dargestellt. Weitere Informationen hierzu finden Sie unter [Microsoft Graph Sicherheits-Datenfluss](security-dataflow.md).

![security_overview_diagram_1.PNG](./images/security_overview_diagram_1.png)

Informationen zur Autorisierung finden Sie unter [Autorisierung und Sicherheits-API](security-authorization.md). Weitere Informationen zu Berechtigungen, einschließlich delegierten und Anwendungsberechtigungen, finden Sie unter [Berechtigungen](permissions_reference.md#security-permissions).

## <a name="why-use-the-microsoft-graph-security-api"></a>Gründe für die Verwendung der Microsoft Graph Sicherheits-API

Die [Microsoft Graph Sicherheits-API](../api-reference/v1.0/resources/security-api-overview.md) stellt auf einfache Weise die Verbindung mit anderen Microsoft und Sicherheitsprodukten der Microsoft Partner und Dienste her. Sie ermöglicht Ihnen, den Wert dieser Lösungen besser zu erkennen und ggf. zu erweitern.

### <a name="unify-and-standardize-alert-tracking"></a>Vereinheitlichen und standardisieren Sie die Nachverfolgung von Meldungen

Schreiben Sie den Code einmal, um Meldungen von einer beliebigen in Microsoft Graph integrierten Sicherheitslösung zu integrieren und behalten Sie den Meldungszustand und Zuordnungen über alle Lösungen hinweg synchronisiert. Sie können Meldungen auch auf Sicherheits-Informationen und Ereignis-Management (SIEM) streamen, wie beispielsweise Splunk und IBM QRadar über [Azure Monitor](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub). Ausführliche Informationen zur Integration von SIEM in den Sicherheits-API Entitäten finden Sie unter [Integrieren in SIEM](security_siemintegration.md).

### <a name="correlate-security-alerts-to-improve-threat-protection-and-response"></a>Korrelieren Sie Sicherheitshinweise für die Verbesserung des Schutzes und der Antwortzeit

Korrelieren Sie Meldungen über Sicherheitslösungen hinweg mit einem vereinheitlichten Schema für Meldungen. Dies ermöglicht Ihnen nicht nur, bearbeitungsfähige Informationen zu Meldungen zu erhalten, sondern Sicherheitsanalysten ebenfalls, Meldungen schwenken und mit Dokumenten und Benutzer-Informationen anzureichern, wodurch eine schnellere Anwort auf Bedrohungen und den Schutz von Dokumenten gewährleistet wird.  

### <a name="update-alert-tags-status-and-assignments"></a>Aktualisieren von Meldungs-Tags, Zustand und Zuordnungen

Markieren Sie Meldungen mit zusätzlichem Kontext oder Nachrichten zu Bedrohungen, um für die Antwort und Wartung zu informieren. Stellen Sie sicher, dass Kommentare und Feedback zu Meldungen für die Sichtbarkeit in allen Arbeitsabläufen erfasst werden. Halten Sie den Zustand der Meldungen und Zurodnungen synchron, sodass alle integrierten Lösungen den aktuellen Zustand wiedergeben. Verwenden Sie Webhook-Abonnements, um Benachrichtigungen zu Änderungen zu erhalten.  

### <a name="unlock-security-context-to-drive-investigation"></a>Entsperren Sie den Sicherheitskontext für Untersuchungszwecke

Gewinnen Sie Einblicke in den sicherheitsrelevanten Bestand (z. B. Benutzer, Hosts und Apps), und fügen Sie organisatorischen Kontext von anderen Microsoft Graph-Anbietern (Azure Active Directory, Microsoft Intune, Office 365) hinzu, um Business- und Sicherheitskontexte zusammenzubringen und die Reaktion auf Sicherheitsrisiken zu verbessern.

### <a name="proactively-manage-security-risks-preview"></a>Proaktive Verwaltung von Sicherheitsrisiken (Vorschau)

Verwenden Sie die Microsoft Secure Score (Vorschau), um einen Einblick in die Sicherheit Ihrer Organisation bereitzustellen, Verbesserungsvorschläge einzuholen und eine verbesserte Bewertung zu projektieren, nachdem diese Vorschläge integriert wurden. Auf einfache Weise messen Sie Ihren Fortschritt mit der Zeit und erhalten Einsichten zu spezifischen Veränderungen, die zur Verbesserung Ihrer Bewertung geführt haben.

## <a name="benefits-of-using-the-microsoft-graph-security-api"></a>Vorteile der Verwendung der Microsoft Graph Sicherheits-API

Die folgende Tabelle enthält die Vorteile, auf die verschiedene Sicherheitslösungen durch die Integration in der Microsoft Graph-Sicherheits-API zugreifen können.  

|**Bereich**     | **Vorteile**|
|:---------------|:---------|
|**Managed Security-Dienstanbieter (MSSPs)**|<ul><li>Optimierte Integration in Werkzeuge für Sicherheitsoperationen und Dienste.</li> <li>Reduzierung von Zeit und Aufwand für die Bereitstellung und Wartung.</li> <li>Die Möglichkeit, MSSP-Kunden einen Mehrwert zu bieten.</li></ul>|
|**SIEM und IT-Lösungen zum Risiko-Management**|<ul><li>Nahtlose Integration mit Microsoft Security-Lösungen und Ökosystempartner.</li> <li>Reichhaltige Metadaten zu Meldungen.</li> <li>Bessere Korrelation von Meldungen.</li></ul>|
|**Anwendungen** <br> (Bedrohungsnachrichten, Mobil, Cloud, IOT, Betrugserkennung, Identität und Zugriff, Risiko und Compliance, Firewall und so weiter)|<ul><li>Einheitliches Bedrohungs-Management, Vorbeugung und Risikomanagement in verschiedenen Sicherheitslösungen.</li> <li>Meldungen, Bestand, Config und Aktionen, die über Microsoft Graph verfügbar gemacht werden.</li> <li>Sofortintegration für Microsoft Graph aktivierte Lösungen.</li></ul>|

## <a name="next-steps"></a>Nächste Schritte

- [Verwendung der Microsoft Graph Sicherheits-API](../api-reference/v1.0/resources/security-api-overview.md)
- Möchten Sie Sicherheitsanbieter werden? Nehmen Sie Verbindung auf, mit dem [Graphsecfeedback](mailto:graphsecfeedback@microsoft.com).
