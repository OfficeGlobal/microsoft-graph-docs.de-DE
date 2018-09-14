# <a name="microsoft-graph-security-api-overview"></a>Sicherheits-API von Microsoft Graph  (Übersicht)

Mit der Sicherheits-API von Microsoft Graph können Sie eine Verbindung mit Microsoft-Sicherheitsprodukten, Diensten und Partnern herstellen, um die Sicherheitsoperationen zu optimieren und den Schutz vor Bedrohungen und die Erkennungs- und Antwortkapazitäten zu verbessern. Die Sicherheits-API von Microsoft Graph ist ein zwischengeschalteter Dienst (oder ein Makler), der eine einzige befehlsorientierte Benutzerschnittstelle für die Verbindung mehrerer [Sicherheitsanbieter für Microsoft Graph](../api-reference/v1.0/resources/securityvendorinformation.md) (auch Sicherheitsanbieter oder Anbieter genannt), bereitstellt. Anforderungen an die Sicherheits-API von Microsoft Graph sind mit allen anwendbaren Sicherheitsanbietern verbunden. Die Ergebnisse werden wie in der folgenden Abbildung aggregiert und in einem gemeinsamen Schema an die anfordernde Anwendung zurückgegeben. Weitere Informationen hierzu finden Sie unter [Microsoft Graph Sicherheitsdatenfluss](security-dataflow.md).

![security_overview_diagram_1.PNG](./images/security_overview_diagram_1.png)

Informationen zur Autorisierung finden Sie unter [Autorisierung und Sicherheits-API](security-authorization.md). Weitere Informationen zu Berechtigungen, einschließlich delegierten und Anwendungsberechtigungen, finden Sie unter [Berechtigungen](permissions_reference.md#security-permissions).

## <a name="why-use-the-microsoft-graph-security-api"></a>Gründe für die Verwendung der Sicherheits-API von Microsoft Graph

Die [Sicherheits-API Microsoft Graph](../api-reference/v1.0/resources/security-api-overview.md) stellt auf einfache Weise die Verbindung mit anderen Sicherheitsprodukten und Diensten von Microsoft und Microsoft Partnern her. Mit ihr können Sie den Wert dieser Lösungen besser realisieren und erweitern.

### <a name="unify-and-standardize-alert-tracking"></a>Vereinheitlichen und standardisieren der Nachverfolgung von Warnungen

Schreiben Sie den Code einmal, um Warnungen von einer beliebigen in Microsoft Graph integrierten Sicherheitslösung zu integrieren und behalten Sie den Warnungsstatus und Aufgaben über alle Lösungen hinweg synchronisiert. Sie können Warnungen auch auf Sicherheitsinformationen und Ereignis-Management (SIEM) streamen, wie beispielsweise Splunk und IBM QRadar über [Azure Monitor](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub). Ausführliche Informationen zur Integration von SIEM in den Sicherheits-API-Entitäten finden Sie unter [Integrieren in SIEM](security_siemintegration.md).

### <a name="correlate-security-alerts-to-improve-threat-protection-and-response"></a>Korrelieren der Sicherheitshinweise für die Verbesserung des Schutzes und der Antwortzeit

Korrelieren Sie Warnungen über Sicherheitslösungen hinweg mit einem vereinheitlichten Schema für Warnungen. Dies ermöglicht nicht nur Ihnen, bearbeitungsfähige Informationen zu Warnungen zu erhalten, sondern auch den Sicherheitsanalysten, Warnungen zu schwenken und mit Dokumenten und Benutzerinformationen anzureichern, wodurch eine schnellere Antwort auf Bedrohungen und den Schutz von Dokumenten gewährleistet wird.  

### <a name="update-alert-tags-status-and-assignments"></a>Aktualisieren von Warnungs-Tags, Zustand und Aufgaben

Markieren Sie Warnungen mit zusätzlichem Kontext oder Nachrichten zu Bedrohungen, um für die Antwort und Wartung zu informieren. Stellen Sie sicher, dass Kommentare und Feedback zu Warnungen für die Sichtbarkeit in allen Arbeitsabläufen erfasst werden. Halten Sie den Warungsstatus und die Aufgaben synchron, sodass alle integrierten Lösungen den aktuellen Zustand wiedergeben. Verwenden Sie Webhook-Abonnements, um Benachrichtigungen zu Änderungen zu erhalten.  

### <a name="unlock-security-context-to-drive-investigation"></a>Aufheben der Sperrung des Sicherheitskontexts zu Untersuchungszwecken

Gewinnen Sie Einblicke in den sicherheitsrelevanten Bestand (z. B. Benutzer, Hosts und Apps), und fügen Sie organisatorischen Kontext von anderen Microsoft Graph-Anbietern (Azure Active Directory, Microsoft Intune, Office 365) hinzu, um Business- und Sicherheitskontexte zusammenzubringen und die Reaktion auf Sicherheitsrisiken zu verbessern.

### <a name="proactively-manage-security-risks-preview"></a>Proaktive Verwaltung von Sicherheitsrisiken (Vorschau)

Verwenden Sie Microsoft Secure Score (Vorschau), um einen Einblick in die Sicherheit Ihrer Organisation bereitzustellen, Verbesserungsvorschläge einzuholen und eine verbesserte Bewertung zu projektieren, nachdem diese Vorschläge integriert wurden. Auf einfache Weise messen Sie im Verlauf der Zeit Ihren Fortschritt und erhalten Einblicke zu spezifischen Veränderungen, die zur Verbesserung Ihrer Bewertung geführt haben.

## <a name="benefits-of-using-the-microsoft-graph-security-api"></a>Vorteile der Verwendung der Sicherheits-API von Microsoft Graph

Die folgende Tabelle enthält die Vorteile, auf die verschiedene Sicherheitslösungen durch die Integration in der Microsoft Graph-Sicherheits-API zugreifen können.  

|**Bereich**     | **Vorteile**|
|:---------------|:---------|
|**Managed Security-Dienstanbieter (MSSPs)**|<ul><li>Optimierte Integration in Tools und Diensten für Sicherheitsoperationen.</li> <li>Reduzierung der Zeit und des Aufwands für die Bereitstellung und Wartung.</li> <li>Die Möglichkeit, MSSP-Kunden einen Mehrwert zu bieten.</li></ul>|
|**SIEM- und IT-Lösungen zum Risiko-Management**|<ul><li>Nahtlose Integration mit Microsoft-Sicherheitslösungen und Ökosystempartnern.</li> <li>Reichhaltige Metadaten zu Warnungen.</li> <li>Bessere Korrelation von Warnungen.</li></ul>|
|**Anwendungen** <br>(Bedrohungsnachrichten, Mobil, Cloud, IOT, Betrugserkennung, Identität und Zugriff, Risiko und Compliance, Firewall und so weiter)|<ul><li>Einheitliches Bedrohungsmanagement, Vorbeugung und Risikomanagement in verschiedenen Sicherheitslösungen.</li> <li>Warnungen, Bestand, Konfiguration und Aktionen, die über Microsoft Graph verfügbar gemacht werden.</li> <li>Sofortintegration für von Microsoft Graph aktivierte Lösungen.</li></ul>|

## <a name="next-steps"></a>Nächste Schritte

- [Verwendung der Sicherheits-API von Microsoft Graph](../api-reference/v1.0/resources/security-api-overview.md)
- Möchten Sie Sicherheitsanbieter werden? Nehmen Sie Verbindung auf, mit dem [Graphsecfeedback](mailto:graphsecfeedback@microsoft.com).
